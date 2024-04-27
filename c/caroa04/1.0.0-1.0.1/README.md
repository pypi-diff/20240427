# Comparing `tmp/caroa04-1.0.0.tar.gz` & `tmp/caroa04-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caroa04-1.0.0.tar", last modified: Fri Apr 26 12:38:51 2024, max compression
+gzip compressed data, was "caroa04-1.0.1.tar", last modified: Sat Apr 27 16:35:13 2024, max compression
```

## Comparing `caroa04-1.0.0.tar` & `caroa04-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.086998 caroa04-1.0.0/
--rw-rw-rw-   0        0        0      179 2024-04-14 17:26:49.000000 caroa04-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3870 2024-04-14 17:26:49.000000 caroa04-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2024-04-14 17:26:49.000000 caroa04-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1102 2024-04-14 17:26:49.000000 caroa04-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      273 2024-04-14 17:26:49.000000 caroa04-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4948 2024-04-26 12:38:51.086998 caroa04-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3797 2024-04-26 12:37:44.000000 caroa04-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.078535 caroa04-1.0.0/docs/
--rw-rw-rw-   0        0        0      628 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4990 2024-04-14 19:01:23.000000 caroa04-1.0.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/history.rst
--rw-rw-rw-   0        0        0      324 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/index.rst
--rw-rw-rw-   0        0        0     1169 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/installation.rst
--rwxrwxrwx   0        0        0      805 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/readme.rst
--rw-rw-rw-   0        0        0       76 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/usage.rst
--rw-rw-rw-   0        0        0     1598 2024-04-26 12:38:09.000000 caroa04-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 12:38:51.086998 caroa04-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.064518 caroa04-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.080541 caroa04-1.0.0/src/caroa04/
--rw-rw-rw-   0        0        0      140 2024-04-14 17:26:49.000000 caroa04-1.0.0/src/caroa04/__init__.py
--rw-rw-rw-   0        0        0    14337 2024-04-26 10:46:42.000000 caroa04-1.0.0/src/caroa04/canmessage.py
--rw-rw-rw-   0        0        0     5977 2024-04-26 12:37:57.000000 caroa04-1.0.0/src/caroa04/caroa04.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.085999 caroa04-1.0.0/src/caroa04.egg-info/
--rw-rw-rw-   0        0        0     4948 2024-04-26 12:38:51.000000 caroa04-1.0.0/src/caroa04.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-26 12:38:51.000000 caroa04-1.0.0/src/caroa04.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 12:38:51.000000 caroa04-1.0.0/src/caroa04.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-26 12:38:51.000000 caroa04-1.0.0/src/caroa04.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-26 12:38:51.000000 caroa04-1.0.0/src/caroa04.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.083998 caroa04-1.0.0/tests/
--rw-rw-rw-   0        0        0       38 2024-04-14 17:26:49.000000 caroa04-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     6899 2024-04-26 12:37:44.000000 caroa04-1.0.0/tests/test_caroa04.py
+drwxrwxrwx   0        0        0        0 2024-04-27 16:35:13.483337 caroa04-1.0.1/
+-rw-rw-rw-   0        0        0      179 2024-04-14 17:26:49.000000 caroa04-1.0.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3870 2024-04-14 17:26:49.000000 caroa04-1.0.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2024-04-14 17:26:49.000000 caroa04-1.0.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1102 2024-04-14 17:26:49.000000 caroa04-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2024-04-14 17:26:49.000000 caroa04-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4975 2024-04-27 16:35:13.482338 caroa04-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3824 2024-04-27 16:31:01.000000 caroa04-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-27 16:35:13.465221 caroa04-1.0.1/docs/
+-rw-rw-rw-   0        0        0      628 2024-04-14 17:26:49.000000 caroa04-1.0.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-1.0.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     4990 2024-04-14 19:01:23.000000 caroa04-1.0.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-04-14 17:26:49.000000 caroa04-1.0.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-1.0.1/docs/history.rst
+-rw-rw-rw-   0        0        0      324 2024-04-14 17:26:49.000000 caroa04-1.0.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1169 2024-04-14 17:26:49.000000 caroa04-1.0.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      805 2024-04-14 17:26:49.000000 caroa04-1.0.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2024-04-14 17:26:49.000000 caroa04-1.0.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       76 2024-04-14 17:26:49.000000 caroa04-1.0.1/docs/usage.rst
+-rw-rw-rw-   0        0        0     1598 2024-04-27 16:34:45.000000 caroa04-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 16:35:13.483337 caroa04-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 16:35:13.413215 caroa04-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 16:35:13.472344 caroa04-1.0.1/src/caroa04/
+-rw-rw-rw-   0        0        0      140 2024-04-14 17:26:49.000000 caroa04-1.0.1/src/caroa04/__init__.py
+-rw-rw-rw-   0        0        0    14337 2024-04-26 10:46:42.000000 caroa04-1.0.1/src/caroa04/canmessage.py
+-rw-rw-rw-   0        0        0     5999 2024-04-27 16:34:50.000000 caroa04-1.0.1/src/caroa04/caroa04.py
+drwxrwxrwx   0        0        0        0 2024-04-27 16:35:13.481337 caroa04-1.0.1/src/caroa04.egg-info/
+-rw-rw-rw-   0        0        0     4975 2024-04-27 16:35:13.000000 caroa04-1.0.1/src/caroa04.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-27 16:35:13.000000 caroa04-1.0.1/src/caroa04.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 16:35:13.000000 caroa04-1.0.1/src/caroa04.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-27 16:35:13.000000 caroa04-1.0.1/src/caroa04.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 16:35:13.000000 caroa04-1.0.1/src/caroa04.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 16:35:13.480338 caroa04-1.0.1/tests/
+-rw-rw-rw-   0        0        0       38 2024-04-14 17:26:49.000000 caroa04-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     6897 2024-04-27 16:31:01.000000 caroa04-1.0.1/tests/test_caroa04.py
```

### Comparing `caroa04-1.0.0/CONTRIBUTING.rst` & `caroa04-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.0/LICENSE` & `caroa04-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.0/PKG-INFO` & `caroa04-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caroa04
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to control the CAROA04 CAN-IO expander device from eletechsup.
 Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/supermete/caroa04/issues
 Project-URL: changelog, https://github.com/supermete/caroa04/blob/master/changelog.md
 Project-URL: homepage, https://github.com/supermete/caroa04
@@ -70,27 +70,27 @@
 You can instantiate a CaroA04 object and start it to communicate with the device as follows.
 
 .. code-block:: python
 
     from caroa04 import CaroA04
 
     caro = CaroA04()
-    caro.start(0xE0, 'pcan', 250000, 'PCAN_USBBUS1')  # start communication
+    caro.start(0xE0, 'pcan', 250000, 'PCAN_USBBUS1')  # start communication with device node ID 0xE0
 
     caro.do1.phys = True  # set do1 state to True
     print(caro.do1.phys)  # read do1 state
     print(caro.di1.phys)  # read di1 state
 
     print(caro.bitrate.phys)  # read current bitrate
     caro.bitrate.phys = 500000  # set different baudrate (will require device power cycle)
 
     print(caro.node_id.phys)  # read current address code
     caro.node_id.phys = 0xE1  # set address code (will require device power cycle)
 
-    caro.shutdown()  # free the bus
+    caro.stop()  # free the bus
 
 ..
 
 In order to share the bus with other participants, you can assign the bus attribute of the CaroA04 object before starting it.
 You should simply then add CaroA04's listener to the existing bus' notifier.
 
 .. code-block:: python
@@ -102,16 +102,16 @@
     nw.connect(interface='pcan', bitrate=250000, channel='PCAN_USBBUS1')
 
 
     caro = CaroA04()
     caro.bus = nw.bus  # use the bus already started by canopen
     nw.notifier.add_listener(caro.listener)  # add listener so that we can receive messages
 
-    caro.start(0xE0, 'pcan')  # start communication
-    caro.shutdown()  # free the bus
+    caro.start(0xE0)  # start communication with node ID 0xE0
+    caro.stop()  # free the bus
 
 ..
 
 Features
 --------
 
 * This library uses the python-can library to communicate with the device. Please refer to its documentation to know about all the CAN interfaces that can be used with this library (https://python-can.readthedocs.io/en/stable/)
```

### Comparing `caroa04-1.0.0/README.rst` & `caroa04-1.0.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -42,27 +42,27 @@
 You can instantiate a CaroA04 object and start it to communicate with the device as follows.
 
 .. code-block:: python
 
     from caroa04 import CaroA04
 
     caro = CaroA04()
-    caro.start(0xE0, 'pcan', 250000, 'PCAN_USBBUS1')  # start communication
+    caro.start(0xE0, 'pcan', 250000, 'PCAN_USBBUS1')  # start communication with device node ID 0xE0
 
     caro.do1.phys = True  # set do1 state to True
     print(caro.do1.phys)  # read do1 state
     print(caro.di1.phys)  # read di1 state
 
     print(caro.bitrate.phys)  # read current bitrate
     caro.bitrate.phys = 500000  # set different baudrate (will require device power cycle)
 
     print(caro.node_id.phys)  # read current address code
     caro.node_id.phys = 0xE1  # set address code (will require device power cycle)
 
-    caro.shutdown()  # free the bus
+    caro.stop()  # free the bus
 
 ..
 
 In order to share the bus with other participants, you can assign the bus attribute of the CaroA04 object before starting it.
 You should simply then add CaroA04's listener to the existing bus' notifier.
 
 .. code-block:: python
@@ -74,16 +74,16 @@
     nw.connect(interface='pcan', bitrate=250000, channel='PCAN_USBBUS1')
 
 
     caro = CaroA04()
     caro.bus = nw.bus  # use the bus already started by canopen
     nw.notifier.add_listener(caro.listener)  # add listener so that we can receive messages
 
-    caro.start(0xE0, 'pcan')  # start communication
-    caro.shutdown()  # free the bus
+    caro.start(0xE0)  # start communication with node ID 0xE0
+    caro.stop()  # free the bus
 
 ..
 
 Features
 --------
 
 * This library uses the python-can library to communicate with the device. Please refer to its documentation to know about all the CAN interfaces that can be used with this library (https://python-can.readthedocs.io/en/stable/)
```

### Comparing `caroa04-1.0.0/docs/Makefile` & `caroa04-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.0/docs/conf.py` & `caroa04-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.0/docs/installation.rst` & `caroa04-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.0/docs/make.bat` & `caroa04-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.0/pyproject.toml` & `caroa04-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caroa04"
-version = "1.0.0"
+version = "1.0.1"
 description = "Library to control the CAROA04 CAN-IO expander device from eletechsup."
 readme = "README.rst"
 requires-python = ">=3.8"
 authors = [
   {name = "Rodolphe Mete Soyding", email = "r.soyding@gmail.com"}
 ]
 maintainers = [
```

### Comparing `caroa04-1.0.0/src/caroa04/canmessage.py` & `caroa04-1.0.1/src/caroa04/canmessage.py`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.0/src/caroa04/caroa04.py` & `caroa04-1.0.1/src/caroa04/caroa04.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 sys.path.append(str(pathlib.Path(__file__).parent))
 
 from canmessage import CanMessageRW, XCanSignal, BOOL, ENUM
 
 logging.basicConfig(level=logging.INFO)
 
 __author__ = "R. Soyding"
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 MSGID_DO_WRITE = 0x100
 MSGID_DO_READ = 0x200
 MSGID_DI_READ = 0x300
 MSGID_PARAM = 0x700
 DEFAULT_NODEID = 0xE0
 
@@ -101,15 +101,15 @@
             self.bitrate
         )
 
         self.message_nodeid.add(
             self.node_id
         )
 
-    def start(self, node_id, interface, bitrate=None, channel=None):
+    def start(self, node_id, interface=None, bitrate=None, channel=None):
         """
         Start the communication.
         :param node_id: node ID (or address code) of the device
         :param interface: CAN interface to be used for the communication
         :param bitrate: CAN speed
         :param channel: channel used for the communication
         :return: None
@@ -159,7 +159,8 @@
 
 if __name__ == "__main__":
     caro = CaroA04()
     caro.start(0xE0, 'pcan', 250000, 'PCAN_USBBUS2')
     caro.do1.phys = True
     print(caro.do1.phys)
     caro.do1.phys = False
+    caro.stop()
```

### Comparing `caroa04-1.0.0/src/caroa04.egg-info/PKG-INFO` & `caroa04-1.0.1/src/caroa04.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caroa04
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to control the CAROA04 CAN-IO expander device from eletechsup.
 Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/supermete/caroa04/issues
 Project-URL: changelog, https://github.com/supermete/caroa04/blob/master/changelog.md
 Project-URL: homepage, https://github.com/supermete/caroa04
@@ -70,27 +70,27 @@
 You can instantiate a CaroA04 object and start it to communicate with the device as follows.
 
 .. code-block:: python
 
     from caroa04 import CaroA04
 
     caro = CaroA04()
-    caro.start(0xE0, 'pcan', 250000, 'PCAN_USBBUS1')  # start communication
+    caro.start(0xE0, 'pcan', 250000, 'PCAN_USBBUS1')  # start communication with device node ID 0xE0
 
     caro.do1.phys = True  # set do1 state to True
     print(caro.do1.phys)  # read do1 state
     print(caro.di1.phys)  # read di1 state
 
     print(caro.bitrate.phys)  # read current bitrate
     caro.bitrate.phys = 500000  # set different baudrate (will require device power cycle)
 
     print(caro.node_id.phys)  # read current address code
     caro.node_id.phys = 0xE1  # set address code (will require device power cycle)
 
-    caro.shutdown()  # free the bus
+    caro.stop()  # free the bus
 
 ..
 
 In order to share the bus with other participants, you can assign the bus attribute of the CaroA04 object before starting it.
 You should simply then add CaroA04's listener to the existing bus' notifier.
 
 .. code-block:: python
@@ -102,16 +102,16 @@
     nw.connect(interface='pcan', bitrate=250000, channel='PCAN_USBBUS1')
 
 
     caro = CaroA04()
     caro.bus = nw.bus  # use the bus already started by canopen
     nw.notifier.add_listener(caro.listener)  # add listener so that we can receive messages
 
-    caro.start(0xE0, 'pcan')  # start communication
-    caro.shutdown()  # free the bus
+    caro.start(0xE0)  # start communication with node ID 0xE0
+    caro.stop()  # free the bus
 
 ..
 
 Features
 --------
 
 * This library uses the python-can library to communicate with the device. Please refer to its documentation to know about all the CAN interfaces that can be used with this library (https://python-can.readthedocs.io/en/stable/)
```

### Comparing `caroa04-1.0.0/src/caroa04.egg-info/SOURCES.txt` & `caroa04-1.0.1/src/caroa04.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.0/tests/test_caroa04.py` & `caroa04-1.0.1/tests/test_caroa04.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         if self.notifier is not None:
             self.notifier.stop()
         if self.bus is not None:
             self.bus.shutdown()
             self.bus = None
 
 
-class TestVirtualCanIoExp1:
+class TestVirtualCaroA04:
     @pytest.fixture(scope="class")
     def caro(self):
         return CaroA04()
 
     @pytest.fixture(scope="class")
     def virtualdevice(self):
         return VirtualDevice()
```

