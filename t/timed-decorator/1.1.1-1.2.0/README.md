# Comparing `tmp/timed_decorator-1.1.1.tar.gz` & `tmp/timed_decorator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timed_decorator-1.1.1.tar", last modified: Thu Apr 25 15:34:34 2024, max compression
+gzip compressed data, was "timed_decorator-1.2.0.tar", last modified: Fri Apr 26 18:36:28 2024, max compression
```

## Comparing `timed_decorator-1.1.1.tar` & `timed_decorator-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:34:34.700541 timed_decorator-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 15:34:30.000000 timed_decorator-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-04-25 15:34:34.700541 timed_decorator-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-25 15:34:30.000000 timed_decorator-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-25 15:34:30.000000 timed_decorator-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:34:34.700541 timed_decorator-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 15:34:30.000000 timed_decorator-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:34:34.696541 timed_decorator-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-25 15:34:30.000000 timed_decorator-1.1.1/tests/test_usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:34:34.700541 timed_decorator-1.1.1/timed_decorator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:34:30.000000 timed_decorator-1.1.1/timed_decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-25 15:34:30.000000 timed_decorator-1.1.1/timed_decorator/nested_timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-25 15:34:30.000000 timed_decorator-1.1.1/timed_decorator/simple_timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-25 15:34:30.000000 timed_decorator-1.1.1/timed_decorator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:34:34.700541 timed_decorator-1.1.1/timed_decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-04-25 15:34:34.000000 timed_decorator-1.1.1/timed_decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 15:34:34.000000 timed_decorator-1.1.1/timed_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:34:34.000000 timed_decorator-1.1.1/timed_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 15:34:34.000000 timed_decorator-1.1.1/timed_decorator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:36:28.216610 timed_decorator-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-26 18:36:21.000000 timed_decorator-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10847 2024-04-26 18:36:28.216610 timed_decorator-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-26 18:36:21.000000 timed_decorator-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-26 18:36:21.000000 timed_decorator-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:36:28.216610 timed_decorator-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 18:36:21.000000 timed_decorator-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:36:28.216610 timed_decorator-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-26 18:36:21.000000 timed_decorator-1.2.0/tests/test_usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:36:28.216610 timed_decorator-1.2.0/timed_decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 18:36:21.000000 timed_decorator-1.2.0/timed_decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-26 18:36:21.000000 timed_decorator-1.2.0/timed_decorator/nested_timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-26 18:36:21.000000 timed_decorator-1.2.0/timed_decorator/simple_timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-26 18:36:21.000000 timed_decorator-1.2.0/timed_decorator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:36:28.216610 timed_decorator-1.2.0/timed_decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10847 2024-04-26 18:36:28.000000 timed_decorator-1.2.0/timed_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-26 18:36:28.000000 timed_decorator-1.2.0/timed_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:36:28.000000 timed_decorator-1.2.0/timed_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 18:36:28.000000 timed_decorator-1.2.0/timed_decorator.egg-info/top_level.txt
```

### Comparing `timed_decorator-1.1.1/LICENSE` & `timed_decorator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timed_decorator-1.1.1/PKG-INFO` & `timed_decorator-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timed-decorator
-Version: 1.1.1
+Version: 1.2.0
 Summary: A timing decorator for python functions.
 Author-email: George Stoica <george.stoica@senticlab.com>
 Maintainer-email: George Stoica <george.stoica@senticlab.com>
 License: Copyright (c) 2012-2024 Scott Chacon and others
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -35,15 +35,15 @@
 License-File: LICENSE
 
 # timed-decorator
 
 ## Installation
 
 ```
-pip install git+https://github.com/ancestor-mithril/timed-decorator.git@master
+pip install timed-decorator
 ```
 
 ## Usage
 
 Attach it to the function you want to time and run the application. 
 
 ```py
@@ -80,14 +80,16 @@
     * `collect_gc` (`bool`): If `True`, runs a full garbage collection before timing the wrapped function. Default: `True`.
     * `use_seconds` (`bool`): If `True`, displays the elapsed time in seconds. Default: `False`.
     * `precision` (`int`): Used in conjunction with `use_seconds`, represents the decimal points used for printing seconds. Default: `9`.
     * `show_args` (`bool`): If `True`, displays the function arguments according to `display_level`. Useful when timing function calls with arguments of different magnitude. Default: `False`.
     * `show_kwargs` (`bool`): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
     * `display_level` (`int`): The level of verbosity used when printing function arguments ad keyword arguments. If `0`, prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays, tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
     * `sep` (`str`): The separator used when printing function arguments and keyword arguments. Default: `', '`.
+    * `file_path` (str): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Can't be used in conjunction with `logger_name`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`.
+    * `logger_name` (str): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`. See [Using a logger](#using-a-logger).
 
 2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after substracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
 ### Examples
 
 Simple usage.
 ```py
@@ -321,7 +323,61 @@
 ```
         sleeping_fn() -> total time: 1000592700ns, own time: 1000592700ns
                 sleeping_fn() -> total time: 500687200ns, own time: 500687200ns
         other_fn() -> total time: 1036725800ns, own time: 536038600ns
         sleeping_fn() -> total time: 1000705600ns, own time: 1000705600ns
 nested_fn() -> total time: 4152634300ns, own time: 1114610200ns
 ```
+
+### Using a logger
+```py
+import logging
+from time import sleep
+
+from timed_decorator.simple_timed import timed
+
+logging.basicConfig()
+logging.root.setLevel(logging.NOTSET)
+
+
+@timed(logger_name='TEST_LOGGER')
+def fn():
+    sleep(1)
+
+
+fn()
+fn()
+```
+Prints
+```
+INFO:TEST_LOGGER:fn() -> total time: 1000368900ns
+INFO:TEST_LOGGER:fn() -> total time: 1001000200ns
+```
+
+Capture a logger's input
+```py
+import logging
+from io import StringIO
+from time import sleep
+
+from timed_decorator.simple_timed import timed
+
+log_stream = StringIO()
+log_handler = logging.StreamHandler(log_stream)
+logging.root.setLevel(logging.NOTSET)
+logging.getLogger('TEST_LOGGER').addHandler(log_handler)
+
+
+@timed(logger_name='TEST_LOGGER')
+def fn():
+    sleep(1)
+
+
+fn()
+fn()
+
+print(log_stream.getvalue().split('\n')[:-1])
+```
+Prints
+```
+['fn() -> total time: 1000214700ns', 'fn() -> total time: 1000157800ns']
+```
```

### Comparing `timed_decorator-1.1.1/README.md` & `timed_decorator-1.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # timed-decorator
 
 ## Installation
 
 ```
-pip install git+https://github.com/ancestor-mithril/timed-decorator.git@master
+pip install timed-decorator
 ```
 
 ## Usage
 
 Attach it to the function you want to time and run the application. 
 
 ```py
@@ -44,14 +44,16 @@
     * `collect_gc` (`bool`): If `True`, runs a full garbage collection before timing the wrapped function. Default: `True`.
     * `use_seconds` (`bool`): If `True`, displays the elapsed time in seconds. Default: `False`.
     * `precision` (`int`): Used in conjunction with `use_seconds`, represents the decimal points used for printing seconds. Default: `9`.
     * `show_args` (`bool`): If `True`, displays the function arguments according to `display_level`. Useful when timing function calls with arguments of different magnitude. Default: `False`.
     * `show_kwargs` (`bool`): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
     * `display_level` (`int`): The level of verbosity used when printing function arguments ad keyword arguments. If `0`, prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays, tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
     * `sep` (`str`): The separator used when printing function arguments and keyword arguments. Default: `', '`.
+    * `file_path` (str): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Can't be used in conjunction with `logger_name`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`.
+    * `logger_name` (str): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`. See [Using a logger](#using-a-logger).
 
 2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after substracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
 ### Examples
 
 Simple usage.
 ```py
@@ -285,7 +287,61 @@
 ```
         sleeping_fn() -> total time: 1000592700ns, own time: 1000592700ns
                 sleeping_fn() -> total time: 500687200ns, own time: 500687200ns
         other_fn() -> total time: 1036725800ns, own time: 536038600ns
         sleeping_fn() -> total time: 1000705600ns, own time: 1000705600ns
 nested_fn() -> total time: 4152634300ns, own time: 1114610200ns
 ```
+
+### Using a logger
+```py
+import logging
+from time import sleep
+
+from timed_decorator.simple_timed import timed
+
+logging.basicConfig()
+logging.root.setLevel(logging.NOTSET)
+
+
+@timed(logger_name='TEST_LOGGER')
+def fn():
+    sleep(1)
+
+
+fn()
+fn()
+```
+Prints
+```
+INFO:TEST_LOGGER:fn() -> total time: 1000368900ns
+INFO:TEST_LOGGER:fn() -> total time: 1001000200ns
+```
+
+Capture a logger's input
+```py
+import logging
+from io import StringIO
+from time import sleep
+
+from timed_decorator.simple_timed import timed
+
+log_stream = StringIO()
+log_handler = logging.StreamHandler(log_stream)
+logging.root.setLevel(logging.NOTSET)
+logging.getLogger('TEST_LOGGER').addHandler(log_handler)
+
+
+@timed(logger_name='TEST_LOGGER')
+def fn():
+    sleep(1)
+
+
+fn()
+fn()
+
+print(log_stream.getvalue().split('\n')[:-1])
+```
+Prints
+```
+['fn() -> total time: 1000214700ns', 'fn() -> total time: 1000157800ns']
+```
```

### Comparing `timed_decorator-1.1.1/pyproject.toml` & `timed_decorator-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "timed-decorator"
-version = "1.1.1"
+version = "1.2.0"
 #requires-python = ">=3.10"
 requires-python = ">=3.7"
 description = "A timing decorator for python functions."
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "George Stoica", email = "george.stoica@senticlab.com"},
```

### Comparing `timed_decorator-1.1.1/timed_decorator/utils.py` & `timed_decorator-1.2.0/timed_decorator/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import logging
 from collections.abc import Sequence
+from typing import Union
 
 try:
     from numpy import ndarray
 except ModuleNotFoundError:
     class ndarray:
         pass
 try:
@@ -45,14 +47,31 @@
 
     def __call__(self, nanoseconds):
         if self.use_seconds:
             return f'{nanoseconds / 1e9:.{self.precision}f}s'
         return f'{nanoseconds}ns'
 
 
+class Logger:
+    def __init__(self, file_path: Union[str, None], logger_name: Union[str, None]):
+        assert file_path is None or logger_name is None
+
+        self.file_path = file_path
+        self.logger_name = logger_name
+
+    def __call__(self, string: str):
+        if self.file_path is not None:
+            with open(self.file_path, 'a') as f:
+                f.write(string + '\n')
+        elif self.logger_name is not None:
+            logging.getLogger(self.logger_name).info(string)
+        else:
+            print(string)
+
+
 class InputFormatter:
     def __init__(self, show_args: bool = False, show_kwargs: bool = False, display_level: int = 1, sep: str = ', '):
         self.show_args = show_args
         self.show_kwargs = show_kwargs
         self.display_level = display_level
         self.sep = sep
```

### Comparing `timed_decorator-1.1.1/timed_decorator.egg-info/PKG-INFO` & `timed_decorator-1.2.0/timed_decorator.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timed-decorator
-Version: 1.1.1
+Version: 1.2.0
 Summary: A timing decorator for python functions.
 Author-email: George Stoica <george.stoica@senticlab.com>
 Maintainer-email: George Stoica <george.stoica@senticlab.com>
 License: Copyright (c) 2012-2024 Scott Chacon and others
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -35,15 +35,15 @@
 License-File: LICENSE
 
 # timed-decorator
 
 ## Installation
 
 ```
-pip install git+https://github.com/ancestor-mithril/timed-decorator.git@master
+pip install timed-decorator
 ```
 
 ## Usage
 
 Attach it to the function you want to time and run the application. 
 
 ```py
@@ -80,14 +80,16 @@
     * `collect_gc` (`bool`): If `True`, runs a full garbage collection before timing the wrapped function. Default: `True`.
     * `use_seconds` (`bool`): If `True`, displays the elapsed time in seconds. Default: `False`.
     * `precision` (`int`): Used in conjunction with `use_seconds`, represents the decimal points used for printing seconds. Default: `9`.
     * `show_args` (`bool`): If `True`, displays the function arguments according to `display_level`. Useful when timing function calls with arguments of different magnitude. Default: `False`.
     * `show_kwargs` (`bool`): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
     * `display_level` (`int`): The level of verbosity used when printing function arguments ad keyword arguments. If `0`, prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays, tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
     * `sep` (`str`): The separator used when printing function arguments and keyword arguments. Default: `', '`.
+    * `file_path` (str): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Can't be used in conjunction with `logger_name`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`.
+    * `logger_name` (str): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`. See [Using a logger](#using-a-logger).
 
 2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after substracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
 ### Examples
 
 Simple usage.
 ```py
@@ -321,7 +323,61 @@
 ```
         sleeping_fn() -> total time: 1000592700ns, own time: 1000592700ns
                 sleeping_fn() -> total time: 500687200ns, own time: 500687200ns
         other_fn() -> total time: 1036725800ns, own time: 536038600ns
         sleeping_fn() -> total time: 1000705600ns, own time: 1000705600ns
 nested_fn() -> total time: 4152634300ns, own time: 1114610200ns
 ```
+
+### Using a logger
+```py
+import logging
+from time import sleep
+
+from timed_decorator.simple_timed import timed
+
+logging.basicConfig()
+logging.root.setLevel(logging.NOTSET)
+
+
+@timed(logger_name='TEST_LOGGER')
+def fn():
+    sleep(1)
+
+
+fn()
+fn()
+```
+Prints
+```
+INFO:TEST_LOGGER:fn() -> total time: 1000368900ns
+INFO:TEST_LOGGER:fn() -> total time: 1001000200ns
+```
+
+Capture a logger's input
+```py
+import logging
+from io import StringIO
+from time import sleep
+
+from timed_decorator.simple_timed import timed
+
+log_stream = StringIO()
+log_handler = logging.StreamHandler(log_stream)
+logging.root.setLevel(logging.NOTSET)
+logging.getLogger('TEST_LOGGER').addHandler(log_handler)
+
+
+@timed(logger_name='TEST_LOGGER')
+def fn():
+    sleep(1)
+
+
+fn()
+fn()
+
+print(log_stream.getvalue().split('\n')[:-1])
+```
+Prints
+```
+['fn() -> total time: 1000214700ns', 'fn() -> total time: 1000157800ns']
+```
```

