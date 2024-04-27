# Comparing `tmp/lecroyutils-4.0.1.tar.gz` & `tmp/lecroyutils-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lecroyutils-4.0.1.tar", last modified: Thu Mar 23 07:07:21 2023, max compression
+gzip compressed data, was "lecroyutils-4.0.2.tar", last modified: Sat Apr 27 14:15:11 2024, max compression
```

## Comparing `lecroyutils-4.0.1.tar` & `lecroyutils-4.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 silas     (1000) silas     (1000)        0 2023-03-23 07:07:21.755493 lecroyutils-4.0.1/
--rw-r--r--   0 silas     (1000) silas     (1000)     4664 2023-03-23 07:00:24.000000 lecroyutils-4.0.1/LICENSE
--rw-r--r--   0 silas     (1000) silas     (1000)     2775 2023-03-23 07:07:21.755493 lecroyutils-4.0.1/PKG-INFO
--rw-r--r--   0 silas     (1000) silas     (1000)     1995 2023-03-23 07:00:24.000000 lecroyutils-4.0.1/README.md
--rw-r--r--   0 silas     (1000) silas     (1000)      103 2023-03-23 07:00:24.000000 lecroyutils-4.0.1/pyproject.toml
--rw-r--r--   0 silas     (1000) silas     (1000)      944 2023-03-23 07:07:21.755493 lecroyutils-4.0.1/setup.cfg
-drwxr-xr-x   0 silas     (1000) silas     (1000)        0 2023-03-23 07:07:21.755493 lecroyutils-4.0.1/src/
-drwxr-xr-x   0 silas     (1000) silas     (1000)        0 2023-03-23 07:07:21.755493 lecroyutils-4.0.1/src/lecroyutils/
--rw-r--r--   0 silas     (1000) silas     (1000)        0 2023-03-23 07:00:24.000000 lecroyutils-4.0.1/src/lecroyutils/__init__.py
--rw-r--r--   0 silas     (1000) silas     (1000)     6086 2023-03-23 07:01:14.000000 lecroyutils-4.0.1/src/lecroyutils/control.py
--rw-r--r--   0 silas     (1000) silas     (1000)     8943 2023-03-23 07:00:24.000000 lecroyutils-4.0.1/src/lecroyutils/data.py
-drwxr-xr-x   0 silas     (1000) silas     (1000)        0 2023-03-23 07:07:21.755493 lecroyutils-4.0.1/src/lecroyutils.egg-info/
--rw-r--r--   0 silas     (1000) silas     (1000)     2775 2023-03-23 07:07:21.000000 lecroyutils-4.0.1/src/lecroyutils.egg-info/PKG-INFO
--rw-r--r--   0 silas     (1000) silas     (1000)      315 2023-03-23 07:07:21.000000 lecroyutils-4.0.1/src/lecroyutils.egg-info/SOURCES.txt
--rw-r--r--   0 silas     (1000) silas     (1000)        1 2023-03-23 07:07:21.000000 lecroyutils-4.0.1/src/lecroyutils.egg-info/dependency_links.txt
--rw-r--r--   0 silas     (1000) silas     (1000)       19 2023-03-23 07:07:21.000000 lecroyutils-4.0.1/src/lecroyutils.egg-info/requires.txt
--rw-r--r--   0 silas     (1000) silas     (1000)       12 2023-03-23 07:07:21.000000 lecroyutils-4.0.1/src/lecroyutils.egg-info/top_level.txt
+drwxrwxrwx   0 silas     (1000) silas     (1000)        0 2024-04-27 14:15:11.359533 lecroyutils-4.0.2/
+-rwxrwxrwx   0 silas     (1000) silas     (1000)     4664 2024-04-27 14:14:41.000000 lecroyutils-4.0.2/LICENSE
+-rwxrwxrwx   0 silas     (1000) silas     (1000)     2765 2024-04-27 14:15:11.356323 lecroyutils-4.0.2/PKG-INFO
+-rwxrwxrwx   0 silas     (1000) silas     (1000)     1936 2024-04-27 14:11:53.000000 lecroyutils-4.0.2/README.md
+-rwxrwxrwx   0 silas     (1000) silas     (1000)      103 2024-04-27 14:14:53.000000 lecroyutils-4.0.2/pyproject.toml
+-rwxrwxrwx   0 silas     (1000) silas     (1000)      944 2024-04-27 14:15:11.364439 lecroyutils-4.0.2/setup.cfg
+drwxrwxrwx   0 silas     (1000) silas     (1000)        0 2024-04-27 14:15:11.142920 lecroyutils-4.0.2/src/
+drwxrwxrwx   0 silas     (1000) silas     (1000)        0 2024-04-27 14:15:11.229472 lecroyutils-4.0.2/src/lecroyutils/
+-rwxrwxrwx   0 silas     (1000) silas     (1000)        0 2021-06-21 22:01:22.000000 lecroyutils-4.0.2/src/lecroyutils/__init__.py
+-rwxrwxrwx   0 silas     (1000) silas     (1000)     6218 2024-04-27 14:01:21.000000 lecroyutils-4.0.2/src/lecroyutils/control.py
+-rwxrwxrwx   0 silas     (1000) silas     (1000)     9172 2024-04-27 14:01:21.000000 lecroyutils-4.0.2/src/lecroyutils/data.py
+drwxrwxrwx   0 silas     (1000) silas     (1000)        0 2024-04-27 14:15:11.346171 lecroyutils-4.0.2/src/lecroyutils.egg-info/
+-rwxrwxrwx   0 silas     (1000) silas     (1000)     2765 2024-04-27 14:15:11.000000 lecroyutils-4.0.2/src/lecroyutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 silas     (1000) silas     (1000)      315 2024-04-27 14:15:11.000000 lecroyutils-4.0.2/src/lecroyutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 silas     (1000) silas     (1000)        1 2024-04-27 14:15:11.000000 lecroyutils-4.0.2/src/lecroyutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 silas     (1000) silas     (1000)       19 2024-04-27 14:15:11.000000 lecroyutils-4.0.2/src/lecroyutils.egg-info/requires.txt
+-rwxrwxrwx   0 silas     (1000) silas     (1000)       12 2024-04-27 14:15:11.000000 lecroyutils-4.0.2/src/lecroyutils.egg-info/top_level.txt
```

### Comparing `lecroyutils-4.0.1/LICENSE` & `lecroyutils-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lecroyutils-4.0.1/PKG-INFO` & `lecroyutils-4.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecroyutils
-Version: 4.0.1
+Version: 4.0.2
 Summary: Library to communicate and parse .trc files with/from LeCroy oscilloscopes.
 Home-page: https://github.com/sibartel/lecroyutils
 Author: Silas Bartel
 Author-email: silas.a.bartel@gmail.com
 Project-URL: Bug Tracker, https://github.com/sibartel/lecroyutils/issues
 Keywords: Parse,LeCroy,Scope,Oscilloscope,TRC
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: python-vxi11
 
 # lecroyutils
 
 [![pypi](https://badgen.net/pypi/v/lecroyutils/)](https://pypi.org/project/lecroyutils/)
 
 Library to communicate and parse .trc files with/from LeCroy oscilloscopes.
 
@@ -65,15 +67,14 @@
 
 scope.save_waveform('C1', 'C1_00000_Lecroy.trc')
 ```
 
 ## Related
 * [lecroyparser](https://github.com/bennomeier/leCroyParser)
 * [LecroyScope_python_snippet](https://github.com/ethz-pes/LecroyScope_python_snippet)
-* [lecroydso](https://github.com/TeledyneLeCroy/lecroydso)
 * [python-vxi11](https://github.com/python-ivi/python-vxi11)
 
 ## License
 lecroyutils is licensed under the [MIT](LICENSE) license.
 
 ## Notice
 We are not affiliated, associated, authorized, endorsed by, or in any way officially connected with Teledyne LeCroy, or any of its subsidiaries or its affiliates. The official Teledyne LeCroy github profile can be found at https://github.com/TeledyneLeCroy.
```

### Comparing `lecroyutils-4.0.1/README.md` & `lecroyutils-4.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
 scope.save_waveform('C1', 'C1_00000_Lecroy.trc')
 ```
 
 ## Related
 * [lecroyparser](https://github.com/bennomeier/leCroyParser)
 * [LecroyScope_python_snippet](https://github.com/ethz-pes/LecroyScope_python_snippet)
-* [lecroydso](https://github.com/TeledyneLeCroy/lecroydso)
 * [python-vxi11](https://github.com/python-ivi/python-vxi11)
 
 ## License
 lecroyutils is licensed under the [MIT](LICENSE) license.
 
 ## Notice
 We are not affiliated, associated, authorized, endorsed by, or in any way officially connected with Teledyne LeCroy, or any of its subsidiaries or its affiliates. The official Teledyne LeCroy github profile can be found at https://github.com/TeledyneLeCroy.
```

### Comparing `lecroyutils-4.0.1/setup.cfg` & `lecroyutils-4.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lecroyutils
-version = 4.0.1
+version = 4.0.2
 author = Silas Bartel
 author_email = silas.a.bartel@gmail.com
 description = Library to communicate and parse .trc files with/from LeCroy oscilloscopes.
 license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sibartel/lecroyutils
```

### Comparing `lecroyutils-4.0.1/src/lecroyutils/control.py` & `lecroyutils-4.0.2/src/lecroyutils/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,15 +166,19 @@
     def save_screenshot(self, file_path: AnyStr):
         with open(file_path, 'wb') as f:
             f.write(self._screenshot_raw())
 
     def _waveform_raw(self, source: str) -> bytes:
         self.check_source(source)
         self.scope.write(f'{source}:WF?')
-        return self.scope.read_raw()
+        bin_data = self.scope.read_raw()
+        # Strip query response
+        if bin_data[9:11] == b',#':
+            bin_data = bin_data[10:]
+        return bin_data
 
     def waveform(self, source: str) -> LecroyScopeData:
         return LecroyScopeData(self._waveform_raw(source), source_desc=f'{source}-live')
 
     def save_waveform(self, source: str, file_path: AnyStr):
         with open(file_path, 'wb') as f:
             f.write(self._waveform_raw(source))
```

### Comparing `lecroyutils-4.0.1/src/lecroyutils/data.py` & `lecroyutils-4.0.2/src/lecroyutils/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,27 +121,30 @@
                 self.trigger_times = np.ascontiguousarray(interleaved_data[::2])
                 self.trigger_offsets = np.ascontiguousarray(interleaved_data[1::2])
 
                 points_per_subarray = int(self.count_wave_array / self.subarray_count)
 
                 self.y = self.y.reshape(self.subarray_count, points_per_subarray).T
 
-                self.x = np.tile(np.linspace(
-                    0, points_per_subarray * self.horizontal_interval, num=points_per_subarray
-                ) + self.horizontal_offset, (self.subarray_count, 1)) + self.trigger_times.reshape((-1, 1))
+                self.x = np.tile(
+                    np.linspace(0, points_per_subarray * self.horizontal_interval, num=points_per_subarray),
+                    (self.subarray_count, 1)) + self.trigger_times.reshape((-1, 1)) + self.trigger_offsets.reshape(
+                    (-1, 1))
                 self.x = self.x.T
 
             # now scale the ADC values
             self.y = self.vertical_gain * np.array(self.y) - self.vertical_offset
 
             # If signal exceeds osci display grid: clipped_soft. If signal hits the maximum value limit: clipped_hard.
             self.clipped_soft = np.logical_or(np.amax(self.y, 0) > self.y_max, np.amin(self.y, 0) < self.y_min)
             # Experimental! Tested only with HDO4104
-            self.clipped_hard = np.logical_or(np.amax(self.y, 0) >= (32752 if self._comm_type == 0 else 127),
-                                              np.amin(self.y, 0) <= (-32768 if self._comm_type == 0 else -128))
+            self.clipped_hard = np.logical_or(np.amax(self.y, 0) >= self.vertical_gain * (
+                                                  32752 if self._comm_type == 1 else 127) - self.vertical_offset,
+                                              np.amin(self.y, 0) <= self.vertical_gain * (
+                                                  -32768 if self._comm_type == 1 else -128) - self.vertical_offset)
             if np.any(self.clipped_hard):
                 warn(f'Signal was clipped: {self.source_desc}')
 
             if sparse is not None:
                 indices = int(len(self.x) / sparse) * np.arange(sparse)
 
                 self.x = self.x[indices]
```

### Comparing `lecroyutils-4.0.1/src/lecroyutils.egg-info/PKG-INFO` & `lecroyutils-4.0.2/src/lecroyutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecroyutils
-Version: 4.0.1
+Version: 4.0.2
 Summary: Library to communicate and parse .trc files with/from LeCroy oscilloscopes.
 Home-page: https://github.com/sibartel/lecroyutils
 Author: Silas Bartel
 Author-email: silas.a.bartel@gmail.com
 Project-URL: Bug Tracker, https://github.com/sibartel/lecroyutils/issues
 Keywords: Parse,LeCroy,Scope,Oscilloscope,TRC
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: python-vxi11
 
 # lecroyutils
 
 [![pypi](https://badgen.net/pypi/v/lecroyutils/)](https://pypi.org/project/lecroyutils/)
 
 Library to communicate and parse .trc files with/from LeCroy oscilloscopes.
 
@@ -65,15 +67,14 @@
 
 scope.save_waveform('C1', 'C1_00000_Lecroy.trc')
 ```
 
 ## Related
 * [lecroyparser](https://github.com/bennomeier/leCroyParser)
 * [LecroyScope_python_snippet](https://github.com/ethz-pes/LecroyScope_python_snippet)
-* [lecroydso](https://github.com/TeledyneLeCroy/lecroydso)
 * [python-vxi11](https://github.com/python-ivi/python-vxi11)
 
 ## License
 lecroyutils is licensed under the [MIT](LICENSE) license.
 
 ## Notice
 We are not affiliated, associated, authorized, endorsed by, or in any way officially connected with Teledyne LeCroy, or any of its subsidiaries or its affiliates. The official Teledyne LeCroy github profile can be found at https://github.com/TeledyneLeCroy.
```

