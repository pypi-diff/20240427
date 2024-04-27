# Comparing `tmp/pyais-2.6.3.tar.gz` & `tmp/pyais-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyais-2.6.3.tar", last modified: Fri Apr  5 12:49:34 2024, max compression
+gzip compressed data, was "pyais-2.6.4.tar", last modified: Sat Apr 27 11:13:07 2024, max compression
```

## Comparing `pyais-2.6.3.tar` & `pyais-2.6.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:49:34.083509 pyais-2.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 12:49:27.000000 pyais-2.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25671 2024-04-05 12:49:34.083509 pyais-2.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-04-05 12:49:27.000000 pyais-2.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:49:34.075509 pyais-2.6.3/pyais/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/ais_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17381 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    64771 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16770 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:49:34.083509 pyais-2.6.3/pyais.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25671 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-05 12:49:27.000000 pyais-2.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 12:49:34.083509 pyais-2.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:49:34.079509 pyais-2.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    61986 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_decode_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    32404 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_file_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_generic_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_nmea.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_tag_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_talker_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_tcp_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_udp_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:13:07.777566 pyais-2.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-27 11:12:58.000000 pyais-2.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25573 2024-04-27 11:13:07.777566 pyais-2.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-04-27 11:12:58.000000 pyais-2.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:13:07.773566 pyais-2.6.4/pyais/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/ais_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17381 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64771 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16770 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:13:07.777566 pyais-2.6.4/pyais.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25573 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-27 11:12:58.000000 pyais-2.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 11:13:07.777566 pyais-2.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:13:07.777566 pyais-2.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61986 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_decode_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32404 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_file_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_generic_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_nmea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_tag_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_talker_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_tcp_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_udp_stream.py
```

### Comparing `pyais-2.6.3/LICENSE` & `pyais-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/PKG-INFO` & `pyais-2.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.6.3
+Version: 2.6.4
 Summary: AIS message decoding
 Author-email: Leon Morten Richter <misc@leonmortenrichter.de>
 Maintainer-email: Leon Morten Richter <misc@leonmortenrichter.de>
 License: MIT License
         
         Copyright (c) 2019 M0r13n
         
@@ -80,16 +80,14 @@
 ---
 
 Supports AIVDM/AIVDO messages. Supports single messages, files and
 TCP/UDP sockets. This library has been used and tested extensively in representative real-world scenarios. This includes tests with live feeds from [Spire](https://spire.com/maritime/), the [Norwegian Coastal Administration](https://kystverket.no/en/navigation-and-monitoring/ais/access-to-ais-data/) and others. I test each major release against a selection of public and non-public data sources to ensure the broadest possible compatibility.
 
 You can find the full documentation on [readthedocs](https://pyais.readthedocs.io/en/latest/).
 
-I also wrote a [blog post about AIS decoding](https://leonrichter.de/posts/pyais/) and this lib.
-
 Binary releases (Debian packages) are provided by the [pyais-debian](https://github.com/M0r13n/pyais-debian) starting with version **v2.5.6**. They are downloadable under the [Releases](https://github.com/M0r13n/pyais/releases) page.
 
 # Acknowledgements
 
 ![Jetbrains Logo](./docs/jetbrains_logo.svg)
 
 This project is a grateful recipient of
```

### Comparing `pyais-2.6.3/README.md` & `pyais-2.6.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 ---
 
 Supports AIVDM/AIVDO messages. Supports single messages, files and
 TCP/UDP sockets. This library has been used and tested extensively in representative real-world scenarios. This includes tests with live feeds from [Spire](https://spire.com/maritime/), the [Norwegian Coastal Administration](https://kystverket.no/en/navigation-and-monitoring/ais/access-to-ais-data/) and others. I test each major release against a selection of public and non-public data sources to ensure the broadest possible compatibility.
 
 You can find the full documentation on [readthedocs](https://pyais.readthedocs.io/en/latest/).
 
-I also wrote a [blog post about AIS decoding](https://leonrichter.de/posts/pyais/) and this lib.
-
 Binary releases (Debian packages) are provided by the [pyais-debian](https://github.com/M0r13n/pyais-debian) starting with version **v2.5.6**. They are downloadable under the [Releases](https://github.com/M0r13n/pyais/releases) page.
 
 # Acknowledgements
 
 ![Jetbrains Logo](./docs/jetbrains_logo.svg)
 
 This project is a grateful recipient of
```

### Comparing `pyais-2.6.3/pyais/__init__.py` & `pyais-2.6.4/pyais/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pyais.messages import NMEAMessage, ANY_MESSAGE, AISSentence
 from pyais.stream import TCPConnection, FileReaderStream, IterMessages
 from pyais.encode import encode_dict, encode_msg, ais_to_nmea_0183
 from pyais.decode import decode
 from pyais.tracker import AISTracker, AISTrack
 
 __license__ = 'MIT'
-__version__ = '2.6.3'
+__version__ = '2.6.4'
 __author__ = 'Leon Morten Richter'
 
 __all__ = (
     'encode_dict',
     'encode_msg',
     'ais_to_nmea_0183',
     'NMEAMessage',
```

### Comparing `pyais-2.6.3/pyais/ais_types.py` & `pyais-2.6.4/pyais/ais_types.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/pyais/constants.py` & `pyais-2.6.4/pyais/constants.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/pyais/decode.py` & `pyais-2.6.4/pyais/decode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/pyais/encode.py` & `pyais-2.6.4/pyais/encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/pyais/exceptions.py` & `pyais-2.6.4/pyais/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/pyais/filter.py` & `pyais-2.6.4/pyais/filter.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/pyais/main.py` & `pyais-2.6.4/pyais/main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/pyais/messages.py` & `pyais-2.6.4/pyais/messages.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/pyais/stream.py` & `pyais-2.6.4/pyais/stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/pyais/tracker.py` & `pyais-2.6.4/pyais/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,18 @@
     ship_type: typing.Optional[int] = dataclasses.field(compare=False, default=None)
     to_bow: typing.Optional[int] = dataclasses.field(compare=False, default=None)
     to_stern: typing.Optional[int] = dataclasses.field(compare=False, default=None)
     to_port: typing.Optional[int] = dataclasses.field(compare=False, default=None)
     to_starboard: typing.Optional[int] = dataclasses.field(compare=False, default=None)
     destination: typing.Optional[str] = dataclasses.field(compare=False, default=None)
     last_updated: float = dataclasses.field(compare=False, default_factory=now)
+    name: typing.Optional[str] = dataclasses.field(compare=False, default=None)
+    ais_version: typing.Optional[int] = dataclasses.field(compare=False, default=None)
+    ais_type: typing.Optional[str] = dataclasses.field(compare=False, default=None)
+    status: typing.Optional[str] = dataclasses.field(compare=False, default=None)
 
 
 # compute a set of all fields only once
 FIELDS = dataclasses.fields(AISTrack)
 
 
 def msg_to_track(msg: ANY_MESSAGE, ts_epoch_ms: typing.Optional[float] = None) -> AISTrack:
```

### Comparing `pyais-2.6.3/pyais/util.py` & `pyais-2.6.4/pyais/util.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/pyais.egg-info/PKG-INFO` & `pyais-2.6.4/pyais.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.6.3
+Version: 2.6.4
 Summary: AIS message decoding
 Author-email: Leon Morten Richter <misc@leonmortenrichter.de>
 Maintainer-email: Leon Morten Richter <misc@leonmortenrichter.de>
 License: MIT License
         
         Copyright (c) 2019 M0r13n
         
@@ -80,16 +80,14 @@
 ---
 
 Supports AIVDM/AIVDO messages. Supports single messages, files and
 TCP/UDP sockets. This library has been used and tested extensively in representative real-world scenarios. This includes tests with live feeds from [Spire](https://spire.com/maritime/), the [Norwegian Coastal Administration](https://kystverket.no/en/navigation-and-monitoring/ais/access-to-ais-data/) and others. I test each major release against a selection of public and non-public data sources to ensure the broadest possible compatibility.
 
 You can find the full documentation on [readthedocs](https://pyais.readthedocs.io/en/latest/).
 
-I also wrote a [blog post about AIS decoding](https://leonrichter.de/posts/pyais/) and this lib.
-
 Binary releases (Debian packages) are provided by the [pyais-debian](https://github.com/M0r13n/pyais-debian) starting with version **v2.5.6**. They are downloadable under the [Releases](https://github.com/M0r13n/pyais/releases) page.
 
 # Acknowledgements
 
 ![Jetbrains Logo](./docs/jetbrains_logo.svg)
 
 This project is a grateful recipient of
```

### Comparing `pyais-2.6.3/pyais.egg-info/SOURCES.txt` & `pyais-2.6.4/pyais.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/pyproject.toml` & `pyais-2.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_constants.py` & `pyais-2.6.4/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_decode.py` & `pyais-2.6.4/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_decode_raw.py` & `pyais-2.6.4/tests/test_decode_raw.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_encode.py` & `pyais-2.6.4/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_examples.py` & `pyais-2.6.4/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_file_stream.py` & `pyais-2.6.4/tests/test_file_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_filters.py` & `pyais-2.6.4/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_flags.py` & `pyais-2.6.4/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_generic_stream.py` & `pyais-2.6.4/tests/test_generic_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_main.py` & `pyais-2.6.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_nmea.py` & `pyais-2.6.4/tests/test_nmea.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_socket.py` & `pyais-2.6.4/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_tag_block.py` & `pyais-2.6.4/tests/test_tag_block.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_talker_ids.py` & `pyais-2.6.4/tests/test_talker_ids.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_tcp_stream.py` & `pyais-2.6.4/tests/test_tcp_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_tracker.py` & `pyais-2.6.4/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.3/tests/test_udp_stream.py` & `pyais-2.6.4/tests/test_udp_stream.py`

 * *Files identical despite different names*

