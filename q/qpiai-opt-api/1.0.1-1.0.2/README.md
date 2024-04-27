# Comparing `tmp/qpiai-opt-api-1.0.1.tar.gz` & `tmp/qpiai_opt_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qpiai-opt-api-1.0.1.tar", last modified: Tue Oct  4 09:13:48 2022, max compression
+gzip compressed data, was "qpiai_opt_api-1.0.2.tar", last modified: Sat Apr 27 12:15:57 2024, max compression
```

## Comparing `qpiai-opt-api-1.0.1.tar` & `qpiai_opt_api-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-10-04 09:13:48.936418 qpiai-opt-api-1.0.1/
--rw-rw-rw-   0        0        0     1108 2022-09-07 10:46:39.000000 qpiai-opt-api-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2039 2022-10-04 09:13:48.936418 qpiai-opt-api-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      537 2022-09-07 10:59:59.000000 qpiai-opt-api-1.0.1/README.txt
--rw-rw-rw-   0        0        0       86 2022-09-07 10:57:15.000000 qpiai-opt-api-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      825 2022-10-04 09:13:48.939412 qpiai-opt-api-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-04 09:13:48.918323 qpiai-opt-api-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-10-04 09:13:48.923309 qpiai-opt-api-1.0.1/src/qpiai_opt/
--rw-rw-rw-   0        0        0        0 2022-10-04 09:03:02.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-04 09:13:48.927874 qpiai-opt-api-1.0.1/src/qpiai_opt/problem/
--rw-rw-rw-   0        0        0      319 2022-10-04 08:59:32.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/problem/__init__.py
--rw-rw-rw-   0        0        0     1182 2022-10-04 08:07:01.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/problem/max_cut.py
--rw-rw-rw-   0        0        0     1001 2022-10-04 08:07:01.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/problem/max_independet_set.py
--rw-rw-rw-   0        0        0      890 2022-10-04 08:07:01.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/problem/number_partition.py
--rw-rw-rw-   0        0        0      802 2022-10-04 08:07:01.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/problem/qubo.py
--rw-rw-rw-   0        0        0      959 2022-10-04 08:07:01.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/problem/vertex_cover.py
-drwxrwxrwx   0        0        0        0 2022-10-04 09:13:48.929868 qpiai-opt-api-1.0.1/src/qpiai_opt/solver/
--rw-rw-rw-   0        0        0       43 2022-10-04 08:59:39.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/solver/__init__.py
--rw-rw-rw-   0        0        0     2698 2022-10-04 08:52:24.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/solver/solver.py
-drwxrwxrwx   0        0        0        0 2022-10-04 09:13:48.931731 qpiai-opt-api-1.0.1/src/qpiai_opt/wrappers/
--rw-rw-rw-   0        0        0       98 2022-10-04 08:59:50.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/wrappers/__init__.py
--rw-rw-rw-   0        0        0     1798 2022-10-04 08:07:01.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/wrappers/dwave.py
--rw-rw-rw-   0        0        0     1932 2022-10-04 08:07:01.000000 qpiai-opt-api-1.0.1/src/qpiai_opt/wrappers/qiskit.py
-drwxrwxrwx   0        0        0        0 2022-10-04 09:13:48.935746 qpiai-opt-api-1.0.1/src/qpiai_opt_api.egg-info/
--rw-rw-rw-   0        0        0     2039 2022-10-04 09:13:48.000000 qpiai-opt-api-1.0.1/src/qpiai_opt_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      622 2022-10-04 09:13:48.000000 qpiai-opt-api-1.0.1/src/qpiai_opt_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-04 09:13:48.000000 qpiai-opt-api-1.0.1/src/qpiai_opt_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-10-04 09:13:48.000000 qpiai-opt-api-1.0.1/src/qpiai_opt_api.egg-info/top_level.txt
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1099 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/LICENSE.txt
+-rw-r--r--   0 akshat    (1005) akshat    (1005)     3484 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/PKG-INFO
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1709 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/README.md
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)       84 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/pyproject.toml
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      796 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/setup.cfg
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.961112 qpiai_opt_api-1.0.2/src/
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/src/qpiai_opt/
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/__init__.py
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      319 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/__init__.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1187 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/max_cut.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1006 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/max_independet_set.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      895 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/number_partition.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      807 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/qubo.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      964 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/vertex_cover.py
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/src/qpiai_opt/solver/
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)       43 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/solver/__init__.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     2698 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/solver/solver.py
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)       98 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/__init__.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1798 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/dwave.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1932 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/qiskit.py
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/
+-rw-r--r--   0 akshat    (1005) akshat    (1005)     3484 2024-04-27 12:15:57.000000 qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/PKG-INFO
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      621 2024-04-27 12:15:57.000000 qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)        1 2024-04-27 12:15:57.000000 qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)       10 2024-04-27 12:15:57.000000 qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/top_level.txt
```

### Comparing `qpiai-opt-api-1.0.1/LICENSE.txt` & `qpiai_opt_api-1.0.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-MIT License
-
-Copyright (c) 2022 Sagar B Dollin, QpiAI India Private Limited
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+MIT License
+
+Copyright (c) 2022 Sagar B Dollin, QpiAI India Private Limited
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `qpiai-opt-api-1.0.1/setup.cfg` & `qpiai_opt_api-1.0.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2071 7069 6169 2d6f 7074 2d61 7069   = qpiai-opt-api
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 310d 0a61 7574 686f 7220 3d20 5361 6761  1..author = Saga
-00000040: 7220 4220 446f 6c6c 696e 0d0a 6465 7363  r B Dollin..desc
-00000050: 7269 7074 696f 6e20 3d20 5170 6941 492d  ription = QpiAI-
-00000060: 4f70 742d 4150 4920 6973 2061 2061 6e20  Opt-API is a an 
-00000070: 696e 7465 7266 6163 6520 7079 7468 6f6e  interface python
-00000080: 2070 6163 6b61 6765 2074 6f20 6163 6365   package to acce
-00000090: 7373 2051 7069 4149 2d4f 7074 2073 6f6c  ss QpiAI-Opt sol
-000000a0: 7665 7273 206f 6e20 636c 6f75 640d 0a6c  vers on cloud..l
-000000b0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000c0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-000000d0: 642c 204c 4943 454e 5345 2e74 7874 0d0a  d, LICENSE.txt..
-000000e0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000f0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-00000100: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
-00000110: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-00000120: 6c61 622e 7170 6961 692e 7465 6368 2f71  lab.qpiai.tech/q
-00000130: 7069 7175 616e 7475 6d2f 6f70 7469 6d69  piquantum/optimi
-00000140: 7361 7469 6f6e 2f71 7069 6169 2d6f 7074  sation/qpiai-opt
-00000150: 2d61 7069 2f0d 0a70 726f 6a65 6374 5f75  -api/..project_u
-00000160: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
-00000170: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-00000180: 6974 6c61 622e 7170 6961 692e 7465 6368  itlab.qpiai.tech
-00000190: 2f71 7069 7175 616e 7475 6d2f 6f70 7469  /qpiquantum/opti
-000001a0: 6d69 7361 7469 6f6e 2f71 7069 6169 2d6f  misation/qpiai-o
-000001b0: 7074 2d61 7069 2f2d 2f69 7373 7565 730d  pt-api/-/issues.
-000001c0: 0a09 7265 706f 7369 746f 7279 203d 2068  ..repository = h
-000001d0: 7474 7073 3a2f 2f67 6974 6c61 622e 7170  ttps://gitlab.qp
-000001e0: 6961 692e 7465 6368 2f71 7069 7175 616e  iai.tech/qpiquan
-000001f0: 7475 6d2f 6f70 7469 6d69 7361 7469 6f6e  tum/optimisation
-00000200: 2f71 7069 6169 2d6f 7074 2d61 7069 2f0d  /qpiai-opt-api/.
-00000210: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-00000220: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000230: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000240: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
-00000250: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000260: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
-00000270: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-00000280: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-00000290: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
-000002a0: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-000002b0: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
-000002c0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
-000002d0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-000002e0: 332e 380d 0a0d 0a5b 6f70 7469 6f6e 732e  3.8....[options.
-000002f0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-00000300: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
-00000310: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000320: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000330: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7170 6961 692d 6f70 742d 6170 690a  = qpiai-opt-api.
+00000020: 7665 7273 696f 6e20 3d20 312e 302e 320a  version = 1.0.2.
+00000030: 6175 7468 6f72 203d 2053 6167 6172 2042  author = Sagar B
+00000040: 2044 6f6c 6c69 6e0a 6465 7363 7269 7074   Dollin.descript
+00000050: 696f 6e20 3d20 5170 6941 492d 4f70 742d  ion = QpiAI-Opt-
+00000060: 4150 4920 6973 2061 2061 6e20 696e 7465  API is a an inte
+00000070: 7266 6163 6520 7079 7468 6f6e 2070 6163  rface python pac
+00000080: 6b61 6765 2074 6f20 6163 6365 7373 2051  kage to access Q
+00000090: 7069 4149 2d4f 7074 2073 6f6c 7665 7273  piAI-Opt solvers
+000000a0: 206f 6e20 636c 6f75 640a 6c6f 6e67 5f64   on cloud.long_d
+000000b0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+000000c0: 653a 2052 4541 444d 452e 6d64 2c20 4c49  e: README.md, LI
+000000d0: 4345 4e53 452e 7478 740a 6c6f 6e67 5f64  CENSE.txt.long_d
+000000e0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+000000f0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+00000100: 6172 6b64 6f77 6e0a 7572 6c20 3d20 6874  arkdown.url = ht
+00000110: 7470 733a 2f2f 6769 746c 6162 2e71 7069  tps://gitlab.qpi
+00000120: 6169 2e74 6563 682f 7170 6971 7561 6e74  ai.tech/qpiquant
+00000130: 756d 2f6f 7074 696d 6973 6174 696f 6e2f  um/optimisation/
+00000140: 7170 6961 692d 6f70 742d 6170 692f 0a70  qpiai-opt-api/.p
+00000150: 726f 6a65 6374 5f75 726c 7320 3d20 0a09  roject_urls = ..
+00000160: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
+00000170: 7470 733a 2f2f 6769 746c 6162 2e71 7069  tps://gitlab.qpi
+00000180: 6169 2e74 6563 682f 7170 6971 7561 6e74  ai.tech/qpiquant
+00000190: 756d 2f6f 7074 696d 6973 6174 696f 6e2f  um/optimisation/
+000001a0: 7170 6961 692d 6f70 742d 6170 692f 2d2f  qpiai-opt-api/-/
+000001b0: 6973 7375 6573 0a09 7265 706f 7369 746f  issues..reposito
+000001c0: 7279 203d 2068 7474 7073 3a2f 2f67 6974  ry = https://git
+000001d0: 6c61 622e 7170 6961 692e 7465 6368 2f71  lab.qpiai.tech/q
+000001e0: 7069 7175 616e 7475 6d2f 6f70 7469 6d69  piquantum/optimi
+000001f0: 7361 7469 6f6e 2f71 7069 6169 2d6f 7074  sation/qpiai-opt
+00000200: 2d61 7069 2f0a 636c 6173 7369 6669 6572  -api/.classifier
+00000210: 7320 3d20 0a09 5072 6f67 7261 6d6d 696e  s = ..Programmin
+00000220: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000230: 7468 6f6e 203a 3a20 330a 094c 6963 656e  thon :: 3..Licen
+00000240: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000250: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000260: 650a 094f 7065 7261 7469 6e67 2053 7973  e..Operating Sys
+00000270: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000280: 6e64 656e 740a 0a5b 6f70 7469 6f6e 735d  ndent..[options]
+00000290: 0a70 6163 6b61 6765 5f64 6972 203d 200a  .package_dir = .
+000002a0: 093d 2073 7263 0a70 6163 6b61 6765 7320  .= src.packages 
+000002b0: 3d20 6669 6e64 3a0a 7079 7468 6f6e 5f72  = find:.python_r
+000002c0: 6571 7569 7265 7320 3d20 3e3d 332e 380a  equires = >=3.8.
+000002d0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+000002e0: 6573 2e66 696e 645d 0a77 6865 7265 203d  es.find].where =
+000002f0: 2073 7263 0a0a 5b65 6767 5f69 6e66 6f5d   src..[egg_info]
+00000300: 0a74 6167 5f62 7569 6c64 203d 200a 7461  .tag_build = .ta
+00000310: 675f 6461 7465 203d 2030 0a0a            g_date = 0..
```

### Comparing `qpiai-opt-api-1.0.1/src/qpiai_opt/problem/max_cut.py` & `qpiai_opt_api-1.0.2/src/qpiai_opt/problem/max_cut.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
         arbitrary_types_allowed = True
 
     num_nodes: int = 100
     graph: Optional[Union[dict, nx.Graph]] = None
     penalty: int = 2
     max_evaluations: int = 1000
     load_gset: Optional[str] = None
-    problem_type = "maximumCut"
+    problem_type: str = "maximumCut"
```

### Comparing `qpiai-opt-api-1.0.1/src/qpiai_opt/problem/max_independet_set.py` & `qpiai_opt_api-1.0.2/src/qpiai_opt/problem/max_independet_set.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,8 +19,8 @@
         '''
     class Config:
         arbitrary_types_allowed = True
     num_nodes: int = 100
     graph: Optional[Union[dict, nx.Graph]] = None
     penalty: int = 2
     max_evaluations: int = 1000
-    problem_type = "maximumIndependentSet"
+    problem_type: str = "maximumIndependentSet"
```

### Comparing `qpiai-opt-api-1.0.1/src/qpiai_opt/problem/number_partition.py` & `qpiai_opt_api-1.0.2/src/qpiai_opt/problem/number_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     class Config:
         arbitrary_types_allowed = True
 
     length: int = 100
     numbers: Optional[list] = None
     penalty: int = 2
     max_evaluations: int = 1000
-    problem_type = "numberPartition"
+    problem_type: str = "numberPartition"
```

### Comparing `qpiai-opt-api-1.0.1/src/qpiai_opt/problem/qubo.py` & `qpiai_opt_api-1.0.2/src/qpiai_opt/problem/qubo.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     :param max_evaluations: Number of maximum evaluations to be run to search the solution.
     '''
     class Config:
         arbitrary_types_allowed = True
     num_variables: int = 100
     qubo_dict: dict = None
     max_evaluations: int = 1000
-    problem_type = "QUBO"
+    problem_type: str = "QUBO"
```

### Comparing `qpiai-opt-api-1.0.1/src/qpiai_opt/problem/vertex_cover.py` & `qpiai_opt_api-1.0.2/src/qpiai_opt/problem/vertex_cover.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,8 +18,8 @@
         """
     class Config:
         arbitrary_types_allowed = True
     num_nodes: int = 100
     graph: Optional[Union[dict, nx.Graph]] = None
     penalty: int = 2
     max_evaluations: int = 1000
-    problem_type = "minimumVertexCover"
+    problem_type: str = "minimumVertexCover"
```

### Comparing `qpiai-opt-api-1.0.1/src/qpiai_opt/solver/solver.py` & `qpiai_opt_api-1.0.2/src/qpiai_opt/solver/solver.py`

 * *Files identical despite different names*

### Comparing `qpiai-opt-api-1.0.1/src/qpiai_opt/wrappers/dwave.py` & `qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/dwave.py`

 * *Files identical despite different names*

### Comparing `qpiai-opt-api-1.0.1/src/qpiai_opt/wrappers/qiskit.py` & `qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/qiskit.py`

 * *Files identical despite different names*

### Comparing `qpiai-opt-api-1.0.1/src/qpiai_opt_api.egg-info/SOURCES.txt` & `qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE.txt
-README.txt
+README.md
 pyproject.toml
 setup.cfg
 src/qpiai_opt/__init__.py
 src/qpiai_opt/problem/__init__.py
 src/qpiai_opt/problem/max_cut.py
 src/qpiai_opt/problem/max_independet_set.py
 src/qpiai_opt/problem/number_partition.py
```

