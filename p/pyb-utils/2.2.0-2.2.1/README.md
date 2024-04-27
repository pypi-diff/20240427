# Comparing `tmp/pyb_utils-2.2.0.tar.gz` & `tmp/pyb_utils-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyb_utils-2.2.0.tar", max compression
+gzip compressed data, was "pyb_utils-2.2.1.tar", max compression
```

## Comparing `pyb_utils-2.2.0.tar` & `pyb_utils-2.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1077 2023-03-01 18:44:35.352445 pyb_utils-2.2.0/LICENSE
--rw-r--r--   0        0        0     6183 2023-12-27 21:22:36.143484 pyb_utils-2.2.0/README.md
--rw-r--r--   0        0        0      792 2023-12-27 21:22:36.143484 pyb_utils-2.2.0/pyb_utils/__init__.py
--rw-r--r--   0        0        0    10369 2023-12-27 21:22:32.779446 pyb_utils-2.2.0/pyb_utils/bodies.py
--rw-r--r--   0        0        0    11886 2023-12-27 21:22:32.779446 pyb_utils-2.2.0/pyb_utils/camera.py
--rw-r--r--   0        0        0     5337 2023-10-20 20:34:26.280496 pyb_utils-2.2.0/pyb_utils/collision.py
--rw-r--r--   0        0        0     4677 2023-10-30 02:58:20.179407 pyb_utils-2.2.0/pyb_utils/contact.py
--rw-r--r--   0        0        0     2115 2023-09-06 21:19:47.199141 pyb_utils-2.2.0/pyb_utils/frame.py
--rw-r--r--   0        0        0     7061 2023-12-27 21:22:32.779446 pyb_utils-2.2.0/pyb_utils/ghost.py
--rw-r--r--   0        0        0     4976 2023-12-27 21:22:36.143484 pyb_utils-2.2.0/pyb_utils/math.py
--rw-r--r--   0        0        0    11460 2023-11-04 23:55:28.738322 pyb_utils-2.2.0/pyb_utils/named_tuples.py
--rw-r--r--   0        0        0    18767 2023-12-27 21:22:32.779446 pyb_utils-2.2.0/pyb_utils/robots.py
--rw-r--r--   0        0        0      424 2023-10-03 02:07:52.298717 pyb_utils-2.2.0/pyb_utils/utils.py
--rw-r--r--   0        0        0      642 2023-12-27 21:27:12.674316 pyb_utils-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     7024 1970-01-01 00:00:00.000000 pyb_utils-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-01 18:44:35.352445 pyb_utils-2.2.1/LICENSE
+-rw-r--r--   0        0        0     6183 2023-12-27 21:22:36.143484 pyb_utils-2.2.1/README.md
+-rw-r--r--   0        0        0      792 2023-12-27 21:22:36.143484 pyb_utils-2.2.1/pyb_utils/__init__.py
+-rw-r--r--   0        0        0    10369 2023-12-27 21:22:32.779446 pyb_utils-2.2.1/pyb_utils/bodies.py
+-rw-r--r--   0        0        0    11886 2023-12-27 21:22:32.779446 pyb_utils-2.2.1/pyb_utils/camera.py
+-rw-r--r--   0        0        0     5337 2023-10-20 20:34:26.280496 pyb_utils-2.2.1/pyb_utils/collision.py
+-rw-r--r--   0        0        0     4677 2023-10-30 02:58:20.179407 pyb_utils-2.2.1/pyb_utils/contact.py
+-rw-r--r--   0        0        0     2115 2023-09-06 21:19:47.199141 pyb_utils-2.2.1/pyb_utils/frame.py
+-rw-r--r--   0        0        0     7066 2024-04-27 14:18:20.259930 pyb_utils-2.2.1/pyb_utils/ghost.py
+-rw-r--r--   0        0        0     4976 2023-12-27 21:22:36.143484 pyb_utils-2.2.1/pyb_utils/math.py
+-rw-r--r--   0        0        0    11460 2023-11-04 23:55:28.738322 pyb_utils-2.2.1/pyb_utils/named_tuples.py
+-rw-r--r--   0        0        0    18767 2023-12-27 21:22:32.779446 pyb_utils-2.2.1/pyb_utils/robots.py
+-rw-r--r--   0        0        0      424 2023-10-03 02:07:52.298717 pyb_utils-2.2.1/pyb_utils/utils.py
+-rw-r--r--   0        0        0      642 2024-04-27 14:18:42.567925 pyb_utils-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7024 1970-01-01 00:00:00.000000 pyb_utils-2.2.1/PKG-INFO
```

### Comparing `pyb_utils-2.2.0/LICENSE` & `pyb_utils-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyb_utils-2.2.0/README.md` & `pyb_utils-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyb_utils-2.2.0/pyb_utils/__init__.py` & `pyb_utils-2.2.1/pyb_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-2.2.0/pyb_utils/bodies.py` & `pyb_utils-2.2.1/pyb_utils/bodies.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-2.2.0/pyb_utils/camera.py` & `pyb_utils-2.2.1/pyb_utils/camera.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-2.2.0/pyb_utils/collision.py` & `pyb_utils-2.2.1/pyb_utils/collision.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-2.2.0/pyb_utils/contact.py` & `pyb_utils-2.2.1/pyb_utils/contact.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-2.2.0/pyb_utils/frame.py` & `pyb_utils-2.2.1/pyb_utils/frame.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-2.2.0/pyb_utils/ghost.py` & `pyb_utils-2.2.1/pyb_utils/ghost.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         orientation : iterable
             The new orientation of the object, as a quaternion :math:`(x, y, z,
             w)` (optional).
         """
         if position is not None:
             self.position = np.array(position)
         if orientation is not None:
-            orientation = np.array(orientation)
+            self.orientation = np.array(orientation)
 
         world_position, world_orientation = self._compute_world_position()
 
         pyb.resetBasePositionAndOrientation(
             self.uid, list(world_position), list(world_orientation)
         )
```

### Comparing `pyb_utils-2.2.0/pyb_utils/math.py` & `pyb_utils-2.2.1/pyb_utils/math.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-2.2.0/pyb_utils/named_tuples.py` & `pyb_utils-2.2.1/pyb_utils/named_tuples.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-2.2.0/pyb_utils/robots.py` & `pyb_utils-2.2.1/pyb_utils/robots.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-2.2.0/pyproject.toml` & `pyb_utils-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 80
 
 [tool.poetry]
 name = "pyb_utils"
-version = "2.2.0"
+version = "2.2.1"
 description = "Basic utilities for PyBullet, including collision detection, ghost (i.e. visual-only) objects, and cameras."
 authors = ["Adam Heins <mail@adamheins.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `pyb_utils-2.2.0/PKG-INFO` & `pyb_utils-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyb-utils
-Version: 2.2.0
+Version: 2.2.1
 Summary: Basic utilities for PyBullet, including collision detection, ghost (i.e. visual-only) objects, and cameras.
 License: MIT
 Author: Adam Heins
 Author-email: mail@adamheins.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

