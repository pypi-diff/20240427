# Comparing `tmp/shelloracle-1.1.2.tar.gz` & `tmp/shelloracle-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelloracle-1.1.2.tar", last modified: Sat Apr 27 16:41:36 2024, max compression
+gzip compressed data, was "shelloracle-1.3.0.tar", last modified: Sat Apr 27 18:08:04 2024, max compression
```

## Comparing `shelloracle-1.1.2.tar` & `shelloracle-1.3.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.174812 shelloracle-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.174812 shelloracle-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 16:41:29.000000 shelloracle-1.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-27 16:41:29.000000 shelloracle-1.1.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-27 16:41:29.000000 shelloracle-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 16:41:29.000000 shelloracle-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-27 16:41:36.178812 shelloracle-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-27 16:41:29.000000 shelloracle-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-27 16:41:29.000000 shelloracle-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:41:36.178812 shelloracle-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.174812 shelloracle-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/src/shelloracle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/src/shelloracle/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/providers/localai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/providers/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/providers/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/src/shelloracle/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/shell/shelloracle.bash
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/shell/shelloracle.zsh
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/shelloracle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/src/shelloracle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 16:41:29.000000 shelloracle-1.1.2/tests/providers/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 16:41:29.000000 shelloracle-1.1.2/tests/providers/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-27 16:41:29.000000 shelloracle-1.1.2/tests/test_shelloracle.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-27 16:41:29.000000 shelloracle-1.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:08:04.349741 shelloracle-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:08:04.341740 shelloracle-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:08:04.345741 shelloracle-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 18:08:00.000000 shelloracle-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-27 18:08:00.000000 shelloracle-1.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-27 18:08:00.000000 shelloracle-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-27 18:08:00.000000 shelloracle-1.3.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 18:08:00.000000 shelloracle-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-27 18:08:04.349741 shelloracle-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-27 18:08:00.000000 shelloracle-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-27 18:08:00.000000 shelloracle-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 18:08:04.349741 shelloracle-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:08:04.345741 shelloracle-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:08:04.345741 shelloracle-1.3.0/src/shelloracle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 18:08:00.000000 shelloracle-1.3.0/src/shelloracle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-27 18:08:00.000000 shelloracle-1.3.0/src/shelloracle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-27 18:08:00.000000 shelloracle-1.3.0/src/shelloracle/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-27 18:08:00.000000 shelloracle-1.3.0/src/shelloracle/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:08:04.349741 shelloracle-1.3.0/src/shelloracle/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-27 18:08:00.000000 shelloracle-1.3.0/src/shelloracle/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-27 18:08:00.000000 shelloracle-1.3.0/src/shelloracle/providers/localai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-27 18:08:00.000000 shelloracle-1.3.0/src/shelloracle/providers/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-27 18:08:00.000000 shelloracle-1.3.0/src/shelloracle/providers/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:08:04.349741 shelloracle-1.3.0/src/shelloracle/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-27 18:08:00.000000 shelloracle-1.3.0/src/shelloracle/shell/shelloracle.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-27 18:08:00.000000 shelloracle-1.3.0/src/shelloracle/shell/shelloracle.zsh
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-27 18:08:00.000000 shelloracle-1.3.0/src/shelloracle/shelloracle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:08:04.349741 shelloracle-1.3.0/src/shelloracle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-27 18:08:04.000000 shelloracle-1.3.0/src/shelloracle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-27 18:08:04.000000 shelloracle-1.3.0/src/shelloracle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:08:04.000000 shelloracle-1.3.0/src/shelloracle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 18:08:04.000000 shelloracle-1.3.0/src/shelloracle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-27 18:08:04.000000 shelloracle-1.3.0/src/shelloracle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 18:08:04.000000 shelloracle-1.3.0/src/shelloracle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:08:04.349741 shelloracle-1.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:08:04.349741 shelloracle-1.3.0/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 18:08:00.000000 shelloracle-1.3.0/tests/providers/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 18:08:00.000000 shelloracle-1.3.0/tests/providers/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-27 18:08:00.000000 shelloracle-1.3.0/tests/test_shelloracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-27 18:08:00.000000 shelloracle-1.3.0/tox.ini
```

### Comparing `shelloracle-1.1.2/.github/workflows/release.yml` & `shelloracle-1.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.2/.github/workflows/tests.yml` & `shelloracle-1.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.2/.gitignore` & `shelloracle-1.3.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -153,7 +153,13 @@
 cython_debug/
 
 # Jetbrains folder
 .idea/
 
 # Installer dependencies
 /installer/installer/**/*
+
+# Demo scripts
+demo/
+
+# Experimental scripts
+experiments/
```

### Comparing `shelloracle-1.1.2/LICENSE` & `shelloracle-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.2/PKG-INFO` & `shelloracle-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7368 656c  : 2.1.Name: shel
 00000020: 6c6f 7261 636c 650a 5665 7273 696f 6e3a  loracle.Version:
-00000030: 2031 2e31 2e32 0a53 756d 6d61 7279 3a20   1.1.2.Summary: 
+00000030: 2031 2e33 2e30 0a53 756d 6d61 7279 3a20   1.3.0.Summary: 
 00000040: 5368 656c 6c4f 7261 636c 6520 6973 2061  ShellOracle is a
 00000050: 2070 6c75 6767 6162 6c65 2074 6572 6d69   pluggable termi
 00000060: 6e61 6c20 7574 696c 6974 7920 7468 6174  nal utility that
 00000070: 2074 616b 6573 2061 206e 6174 7572 616c   takes a natural
 00000080: 206c 616e 6775 6167 6520 6465 7363 7269   language descri
 00000090: 7074 696f 6e20 6f66 2061 2063 6f6d 6d61  ption of a comma
 000000a0: 6e64 2061 6e64 2073 7562 7374 6974 7574  nd and substitut
@@ -72,339 +72,294 @@
 00000470: 7175 6972 6573 2d44 6973 743a 2070 726f  quires-Dist: pro
 00000480: 6d70 742d 746f 6f6c 6b69 740a 5265 7175  mpt-toolkit.Requ
 00000490: 6972 6573 2d44 6973 743a 2079 6173 7069  ires-Dist: yaspi
 000004a0: 6e0a 5265 7175 6972 6573 2d44 6973 743a  n.Requires-Dist:
 000004b0: 2074 6f6d 6c6b 6974 0a52 6571 7569 7265   tomlkit.Require
 000004c0: 732d 4469 7374 3a20 746f 6d6c 693e 3d31  s-Dist: tomli>=1
 000004d0: 2e31 2e30 3b20 7079 7468 6f6e 5f76 6572  .1.0; python_ver
-000004e0: 7369 6f6e 203c 2022 332e 3131 220a 0a5b  sion < "3.11"..[
-000004f0: 215b 5465 7374 735d 2868 7474 7073 3a2f  ![Tests](https:/
-00000500: 2f67 6974 6875 622e 636f 6d2f 646a 636f  /github.com/djco
-00000510: 706c 6579 2f53 6865 6c6c 4f72 6163 6c65  pley/ShellOracle
-00000520: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000530: 7773 2f74 6573 7473 2e79 6d6c 2f62 6164  ws/tests.yml/bad
-00000540: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
-00000550: 696e 295d 2868 7474 7073 3a2f 2f67 6974  in)](https://git
-00000560: 6875 622e 636f 6d2f 646a 636f 706c 6579  hub.com/djcopley
-00000570: 2f53 6865 6c6c 4f72 6163 6c65 2f61 6374  /ShellOracle/act
-00000580: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f74  ions/workflows/t
-00000590: 6573 7473 2e79 6d6c 290a 5b21 5b50 7950  ests.yml).[![PyP
-000005a0: 4920 7665 7273 696f 6e5d 2868 7474 7073  I version](https
-000005b0: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
-000005c0: 2f70 792f 7368 656c 6c6f 7261 636c 652e  /py/shelloracle.
-000005d0: 7376 6729 5d28 6874 7470 733a 2f2f 6261  svg)](https://ba
-000005e0: 6467 652e 6675 7279 2e69 6f2f 7079 2f73  dge.fury.io/py/s
-000005f0: 6865 6c6c 6f72 6163 6c65 290a 5b21 5b50  helloracle).[![P
-00000600: 7950 4920 5375 7070 6f72 7465 6420 5079  yPI Supported Py
-00000610: 7468 6f6e 2056 6572 7369 6f6e 735d 2868  thon Versions](h
-00000620: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000630: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-00000640: 7369 6f6e 732f 7368 656c 6c6f 7261 636c  sions/shelloracl
-00000650: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-00000660: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
-00000670: 7079 7069 2f73 6865 6c6c 6f72 6163 6c65  pypi/shelloracle
-00000680: 2f29 0a5b 215b 446f 776e 6c6f 6164 735d  /).[![Downloads]
-00000690: 2868 7474 7073 3a2f 2f73 7461 7469 632e  (https://static.
-000006a0: 7065 7079 2e74 6563 682f 6261 6467 652f  pepy.tech/badge/
-000006b0: 7368 656c 6c6f 7261 636c 6529 5d28 6874  shelloracle)](ht
-000006c0: 7470 733a 2f2f 7065 7079 2e74 6563 682f  tps://pepy.tech/
-000006d0: 7072 6f6a 6563 742f 7368 656c 6c6f 7261  project/shellora
-000006e0: 636c 6529 0a0a 2320 5368 656c 6c4f 7261  cle)..# ShellOra
-000006f0: 636c 650a 0a53 6865 6c6c 4f72 6163 6c65  cle..ShellOracle
-00000700: 2069 7320 616e 2069 6e6e 6f76 6174 6976   is an innovativ
-00000710: 6520 7465 726d 696e 616c 2075 7469 6c69  e terminal utili
-00000720: 7479 2064 6573 6967 6e65 6420 666f 7220  ty designed for 
-00000730: 696e 7465 6c6c 6967 656e 7420 7368 656c  intelligent shel
-00000740: 6c20 636f 6d6d 616e 6420 6765 6e65 7261  l command genera
-00000750: 7469 6f6e 2c20 6272 696e 6769 6e67 2061  tion, bringing a
-00000760: 206e 6577 206c 6576 656c 206f 660a 6566   new level of.ef
-00000770: 6669 6369 656e 6379 2074 6f20 796f 7572  ficiency to your
-00000780: 2063 6f6d 6d61 6e64 2d6c 696e 6520 696e   command-line in
-00000790: 7465 7261 6374 696f 6e73 2e20 5368 656c  teractions. Shel
-000007a0: 6c4f 7261 636c 6520 6375 7272 656e 746c  lOracle currentl
-000007b0: 7920 7375 7070 6f72 7473 204f 6c6c 616d  y supports Ollam
-000007c0: 612c 204c 6f63 616c 4149 2c20 616e 6420  a, LocalAI, and 
-000007d0: 4f70 656e 4149 210a 0a21 5b53 6865 6c6c  OpenAI!..![Shell
-000007e0: 4f72 6163 6c65 5d28 6874 7470 733a 2f2f  Oracle](https://
-000007f0: 692e 696d 6775 722e 636f 6d2f 6d67 3172  i.imgur.com/mg1r
-00000800: 437a 642e 6769 6629 0a0a 4578 706c 6f72  Czd.gif)..Explor
-00000810: 6520 6f75 7220 6479 6e61 6d69 6320 6665  e our dynamic fe
-00000820: 6174 7572 6573 2061 6e64 206c 6f6f 6b20  atures and look 
-00000830: 666f 7277 6172 6420 746f 206d 6f72 6520  forward to more 
-00000840: 6578 6369 7469 6e67 2075 7064 6174 6573  exciting updates
-00000850: 2062 7920 6769 7669 6e67 2075 7320 6120   by giving us a 
-00000860: e2ad 9020 616e 6420 6120 f09f 9180 0a0a  ... and a ......
-00000870: 2323 2054 6162 6c65 206f 6620 436f 6e74  ## Table of Cont
-00000880: 656e 7473 0a0a 2d20 5b49 6e74 726f 6475  ents..- [Introdu
-00000890: 6374 696f 6e5d 2823 696e 7472 6f64 7563  ction](#introduc
-000008a0: 7469 6f6e 290a 2d20 5b46 6561 7475 7265  tion).- [Feature
-000008b0: 735d 2823 6665 6174 7572 6573 290a 2d20  s](#features).- 
-000008c0: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2823  [Installation](#
-000008d0: 696e 7374 616c 6c61 7469 6f6e 290a 2d20  installation).- 
-000008e0: 5b55 7361 6765 5d28 2375 7361 6765 290a  [Usage](#usage).
-000008f0: 2d20 5b50 726f 7669 6465 7273 5d28 2370  - [Providers](#p
-00000900: 726f 7669 6465 7273 290a 2d20 5b43 6f6e  roviders).- [Con
-00000910: 6669 6775 7261 7469 6f6e 5d28 2363 6f6e  figuration](#con
-00000920: 6669 6775 7261 7469 6f6e 290a 2d20 5b53  figuration).- [S
-00000930: 7973 7465 6d20 5265 7175 6972 656d 656e  ystem Requiremen
-00000940: 7473 5d28 2373 7973 7465 6d2d 7265 7175  ts](#system-requ
-00000950: 6972 656d 656e 7473 290a 2d20 5b46 6565  irements).- [Fee
-00000960: 6462 6163 6b5d 2823 6665 6564 6261 636b  dback](#feedback
-00000970: 290a 0a23 2320 496e 7472 6f64 7563 7469  )..## Introducti
-00000980: 6f6e 0a0a 4d65 6574 2053 6865 6c6c 4f72  on..Meet ShellOr
-00000990: 6163 6c65 e280 9461 2068 616e 6479 2074  acle...a handy t
-000009a0: 6f6f 6c20 7468 6174 206d 616b 6573 2077  ool that makes w
-000009b0: 6f72 6b69 6e67 2077 6974 6820 7468 6520  orking with the 
-000009c0: 636f 6d6d 616e 6420 6c69 6e65 2061 2062  command line a b
-000009d0: 6974 2073 6d6f 6f74 6865 722e 2054 6869  it smoother. Thi
-000009e0: 7320 7465 726d 696e 616c 2075 7469 6c69  s terminal utili
-000009f0: 7479 206c 6574 7320 796f 750a 6372 6561  ty lets you.crea
-00000a00: 7465 2073 6865 6c6c 2063 6f6d 6d61 6e64  te shell command
-00000a10: 7320 6279 2064 6573 6372 6962 696e 6720  s by describing 
-00000a20: 7768 6174 2079 6f75 2077 616e 7420 746f  what you want to
-00000a30: 2064 6f20 696e 2070 6c61 696e 206c 616e   do in plain lan
-00000a40: 6775 6167 652e 2053 6865 6c6c 4f72 6163  guage. ShellOrac
-00000a50: 6c65 2073 696d 706c 6966 6965 7320 7468  le simplifies th
-00000a60: 6520 7072 6f63 6573 7320 6f66 0a63 7261  e process of.cra
-00000a70: 6674 696e 6720 636f 6d70 6c65 7820 636f  fting complex co
-00000a80: 6d6d 616e 6473 2062 7920 7265 6d6f 7669  mmands by removi
-00000a90: 6e67 2074 6865 206e 6565 6420 746f 2067  ng the need to g
-00000aa0: 6f6f 676c 6520 616e 6420 636f 6d62 206d  oogle and comb m
-00000ab0: 616e 2070 6167 6573 2e0a 0a2a 2a57 6879  an pages...**Why
-00000ac0: 2053 6865 6c6c 4f72 6163 6c65 3f2a 2a0a   ShellOracle?**.
-00000ad0: 0a2a 202a 2a4e 6f20 4d6f 7265 204d 656d  .* **No More Mem
-00000ae0: 6f72 697a 696e 673a 2a2a 2046 6f72 6765  orizing:** Forge
-00000af0: 7420 6162 6f75 7420 7265 6d65 6d62 6572  t about remember
-00000b00: 696e 6720 636f 6d70 6c65 7820 7368 656c  ing complex shel
-00000b10: 6c20 636f 6d6d 616e 6473 2e20 4a75 7374  l commands. Just
-00000b20: 2074 656c 6c20 5368 656c 6c4f 7261 636c   tell ShellOracl
-00000b30: 6520 7768 6174 2079 6f75 206e 6565 642c  e what you need,
-00000b40: 2061 6e64 0a20 2069 7427 6c6c 2067 656e   and.  it'll gen
-00000b50: 6572 6174 6520 7468 6520 636f 6d6d 616e  erate the comman
-00000b60: 6420 666f 7220 796f 752e 0a0a 2a20 2a2a  d for you...* **
-00000b70: 5361 7665 2054 696d 652c 2053 7461 7920  Save Time, Stay 
-00000b80: 466f 6375 7365 643a 2a2a 2053 6179 2067  Focused:** Say g
-00000b90: 6f6f 6462 7965 2074 6f20 6d61 6e75 616c  oodbye to manual
-00000ba0: 2063 6f6d 6d61 6e64 2063 7261 6674 696e   command craftin
-00000bb0: 672e 2053 6865 6c6c 4f72 6163 6c65 2068  g. ShellOracle h
-00000bc0: 656c 7073 2079 6f75 2073 6176 6520 7469  elps you save ti
-00000bd0: 6d65 2061 6e64 2063 6f6e 6365 6e74 7261  me and concentra
-00000be0: 7465 0a20 206f 6e20 7768 6174 2072 6561  te.  on what rea
-00000bf0: 6c6c 7920 6d61 7474 6572 7320 6279 2075  lly matters by u
-00000c00: 7369 6e67 206e 6174 7572 616c 206c 616e  sing natural lan
-00000c10: 6775 6167 6520 6465 7363 7269 7074 696f  guage descriptio
-00000c20: 6e73 2e0a 0a2a 202a 2a41 6461 7074 6162  ns...* **Adaptab
-00000c30: 6c65 2074 6f20 596f 7572 204e 6565 6473  le to Your Needs
-00000c40: 3a2a 2a20 5768 6574 6865 7220 6974 2773  :** Whether it's
-00000c50: 2061 2071 7569 636b 206f 6e65 2d6c 696e   a quick one-lin
-00000c60: 6572 206f 7220 6120 7365 7175 656e 6365  er or a sequence
-00000c70: 206f 6620 636f 6d6d 616e 6473 2c20 5368   of commands, Sh
-00000c80: 656c 6c4f 7261 636c 6520 6973 2066 6c65  ellOracle is fle
-00000c90: 7869 626c 652e 2049 740a 2020 7375 7070  xible. It.  supp
-00000ca0: 6f72 7473 2055 6e69 7820 7069 7065 7320  orts Unix pipes 
-00000cb0: 616e 6420 6b65 6570 7320 7472 6163 6b20  and keeps track 
-00000cc0: 6f66 2079 6f75 7220 636f 6d6d 616e 6420  of your command 
-00000cd0: 6869 7374 6f72 792e 0a0a 2a20 2a2a 596f  history...* **Yo
-00000ce0: 7572 2043 6f6e 7472 6f6c 2c20 596f 7572  ur Control, Your
-00000cf0: 2057 6179 3a2a 2a20 5275 6e20 5368 656c   Way:** Run Shel
-00000d00: 6c4f 7261 636c 6520 6173 2061 2073 656c  lOracle as a sel
-00000d10: 662d 686f 7374 6564 2075 7469 6c69 7479  f-hosted utility
-00000d20: 2074 6f20 6861 7665 2063 6f6d 706c 6574   to have complet
-00000d30: 6520 636f 6e74 726f 6c2e 2054 6169 6c6f  e control. Tailo
-00000d40: 7220 6974 2074 6f20 796f 7572 0a20 2070  r it to your.  p
-00000d50: 7265 6665 7265 6e63 6573 2061 6e64 206d  references and m
-00000d60: 616b 6520 6974 2077 6f72 6b20 6a75 7374  ake it work just
-00000d70: 2074 6865 2077 6179 2079 6f75 2077 616e   the way you wan
-00000d80: 742e 0a0a 4769 7665 2069 7420 6120 7472  t...Give it a tr
-00000d90: 7920 616e 6420 7365 6520 686f 7720 6974  y and see how it
-00000da0: 2066 6974 7320 696e 746f 2079 6f75 7220   fits into your 
-00000db0: 776f 726b 666c 6f77 210a 0a23 2320 4665  workflow!..## Fe
-00000dc0: 6174 7572 6573 0a0a 4b65 7920 6665 6174  atures..Key feat
-00000dd0: 7572 6573 206f 6620 5368 656c 6c4f 7261  ures of ShellOra
-00000de0: 636c 6520 696e 636c 7564 653a 0a0a 2a20  cle include:..* 
-00000df0: 5365 616d 6c65 7373 2073 6865 6c6c 2063  Seamless shell c
-00000e00: 6f6d 6d61 6e64 2067 656e 6572 6174 696f  ommand generatio
-00000e10: 6e20 6672 6f6d 2077 7269 7474 656e 2064  n from written d
-00000e20: 6573 6372 6970 7469 6f6e 730a 2a20 436f  escriptions.* Co
-00000e30: 6d6d 616e 6420 6869 7374 6f72 7920 666f  mmand history fo
-00000e40: 7220 6561 7379 2072 6566 6572 656e 6365  r easy reference
-00000e50: 0a2a 2055 6e69 7820 7069 7065 2073 7570  .* Unix pipe sup
-00000e60: 706f 7274 2066 6f72 2061 6476 616e 6365  port for advance
-00000e70: 6420 636f 6d6d 616e 6420 6368 6169 6e69  d command chaini
-00000e80: 6e67 0a2a 2053 656c 662d 686f 7374 6564  ng.* Self-hosted
-00000e90: 2066 6f72 2066 756c 6c20 636f 6e74 726f   for full contro
-00000ea0: 6c20 6f76 6572 2079 6f75 7220 656e 7669  l over your envi
-00000eb0: 726f 6e6d 656e 740a 2a20 4869 6768 6c79  ronment.* Highly
-00000ec0: 2063 6f6e 6669 6775 7261 626c 6520 746f   configurable to
-00000ed0: 2061 6461 7074 2074 6f20 796f 7572 2070   adapt to your p
-00000ee0: 7265 6665 7265 6e63 6573 0a0a 2323 2049  references..## I
-00000ef0: 6e73 7461 6c6c 6174 696f 6e0a 0a49 6e73  nstallation..Ins
-00000f00: 7461 6c6c 696e 6720 5368 656c 6c4f 7261  talling ShellOra
-00000f10: 636c 6520 6973 2065 6173 7921 0a0a 312e  cle is easy!..1.
-00000f20: 2050 6970 2069 6e73 7461 6c6c 2074 6865   Pip install the
-00000f30: 2060 7368 656c 6c6f 7261 636c 6560 2070   `shelloracle` p
-00000f40: 6163 6b61 6765 0a20 2020 2060 6060 7368  ackage.    ```sh
-00000f50: 656c 6c0a 2020 2020 7079 7468 6f6e 3320  ell.    python3 
-00000f60: 2d6d 2070 6970 2069 6e73 7461 6c6c 2073  -m pip install s
-00000f70: 6865 6c6c 6f72 6163 6c65 0a20 2020 2060  helloracle.    `
-00000f80: 6060 0a32 2e20 436f 6e66 6967 7572 6520  ``.2. Configure 
-00000f90: 5368 656c 6c4f 7261 636c 6520 7769 7468  ShellOracle with
-00000fa0: 2060 7368 656c 6c6f 7261 636c 6520 636f   `shelloracle co
-00000fb0: 6e66 6967 7572 6560 2061 6e64 2066 6f6c  nfigure` and fol
-00000fc0: 6c6f 7720 7468 6520 7072 6f6d 7074 730a  low the prompts.
-00000fd0: 2020 2020 6060 6073 6865 6c6c 0a20 2020      ```shell.   
-00000fe0: 2070 7974 686f 6e33 202d 6d20 7368 656c   python3 -m shel
-00000ff0: 6c6f 7261 636c 6520 636f 6e66 6967 7572  loracle configur
-00001000: 650a 2020 2020 6060 600a 332e 2052 6566  e.    ```.3. Ref
-00001010: 6572 2074 6f20 7468 6520 5b70 726f 7669  er to the [provi
-00001020: 6465 7273 5d28 2370 726f 7669 6465 7273  ders](#providers
-00001030: 2920 7365 6374 696f 6e20 666f 7220 7370  ) section for sp
-00001040: 6563 6966 6963 2064 6574 6169 6c73 2072  ecific details r
-00001050: 6567 6172 6469 6e67 2079 6f75 7220 6368  egarding your ch
-00001060: 6f73 656e 2070 726f 7669 6465 722e 0a0a  osen provider...
-00001070: 2323 2055 7361 6765 0a0a 5368 656c 6c4f  ## Usage..ShellO
-00001080: 7261 636c 6520 6973 2064 6573 6967 6e65  racle is designe
-00001090: 6420 746f 2062 6520 7573 6564 2061 7320  d to be used as 
-000010a0: 6120 4241 5348 2f5a 5348 2077 6964 6765  a BASH/ZSH widge
-000010b0: 7420 6163 7469 7661 7465 6420 6279 2074  t activated by t
-000010c0: 6865 2043 5452 4c2b 4620 6b65 7962 6f61  he CTRL+F keyboa
-000010d0: 7264 2073 686f 7274 6375 742e 0a0a 312e  rd shortcut...1.
-000010e0: 2050 7265 7373 2043 5452 4c2b 460a 322e   Press CTRL+F.2.
-000010f0: 2044 6573 6372 6962 6520 796f 7572 2063   Describe your c
-00001100: 6f6d 6d61 6e64 0a33 2e20 5072 6573 7320  ommand.3. Press 
-00001110: 456e 7465 720a 0a54 6865 2067 656e 6572  Enter..The gener
-00001120: 6174 6564 2063 6f6d 6d61 6e64 2077 696c  ated command wil
-00001130: 6c20 6265 2069 6e73 6572 7465 6420 696e  l be inserted in
-00001140: 746f 2079 6f75 7220 7368 656c 6c20 7072  to your shell pr
-00001150: 6f6d 7074 2061 6674 6572 2061 2062 7269  ompt after a bri
-00001160: 6566 2070 726f 6365 7373 696e 6720 7065  ef processing pe
-00001170: 7269 6f64 2e0a 0a23 2320 5072 6f76 6964  riod...## Provid
-00001180: 6572 730a 0a23 2323 204f 6c6c 616d 610a  ers..### Ollama.
-00001190: 0a42 6566 6f72 6520 7573 696e 6720 5368  .Before using Sh
-000011a0: 656c 6c4f 7261 636c 6520 7769 7468 204f  ellOracle with O
-000011b0: 6c6c 616d 612c 2070 756c 6c20 7468 6520  llama, pull the 
-000011c0: 6d6f 6465 6c20 796f 7520 6368 6f73 6520  model you chose 
-000011d0: 696e 2074 6865 2063 6f6e 6669 6775 7265  in the configure
-000011e0: 2073 7465 702e 0a46 6f72 2065 7861 6d70   step..For examp
-000011f0: 6c65 2c20 6966 2079 6f75 2063 686f 7365  le, if you chose
-00001200: 2060 636f 6465 6c6c 616d 613a 3133 6260   `codellama:13b`
-00001210: 2c20 7275 6e3a 0a0a 6060 6073 6865 6c6c  , run:..```shell
-00001220: 0a6f 6c6c 616d 6120 7075 6c6c 2063 6f64  .ollama pull cod
-00001230: 656c 6c61 6d61 3a31 3362 0a60 6060 0a0a  ellama:13b.```..
-00001240: 5265 6665 7220 746f 2074 6865 205b 4f6c  Refer to the [Ol
-00001250: 6c61 6d61 2064 6f63 735d 2868 7474 7073  lama docs](https
-00001260: 3a2f 2f6f 6c6c 616d 612e 6169 2920 666f  ://ollama.ai) fo
-00001270: 7220 696e 7374 616c 6c61 7469 6f6e 2c20  r installation, 
-00001280: 6176 6169 6c61 626c 6520 6d6f 6465 6c73  available models
-00001290: 2c20 616e 6420 7573 6167 652e 0a0a 2323  , and usage...##
-000012a0: 2320 4f70 656e 4149 0a0a 546f 2075 7365  # OpenAI..To use
-000012b0: 2053 6865 6c6c 4f72 6163 6c65 2077 6974   ShellOracle wit
-000012c0: 6820 7468 6520 4f70 656e 4149 2070 726f  h the OpenAI pro
-000012d0: 7669 6465 722c 2063 7265 6174 6520 616e  vider, create an
-000012e0: 205b 4150 4920 6b65 795d 2868 7474 7073   [API key](https
-000012f0: 3a2f 2f70 6c61 7466 6f72 6d2e 6f70 656e  ://platform.open
-00001300: 6169 2e63 6f6d 2f61 6363 6f75 6e74 2f61  ai.com/account/a
-00001310: 7069 2d6b 6579 7329 2e20 4564 6974 0a79  pi-keys). Edit.y
-00001320: 6f75 7220 607e 2f2e 7368 656c 6c6f 7261  our `~/.shellora
-00001330: 636c 652f 636f 6e66 6967 2e74 6f6d 6c60  cle/config.toml`
-00001340: 2074 6f20 6368 616e 6765 2079 6f75 7220   to change your 
-00001350: 7072 6f76 6964 6572 2061 6e64 2065 6e74  provider and ent
-00001360: 6572 2079 6f75 7220 4150 4920 6b65 792e  er your API key.
-00001370: 0a0a 2323 2320 4c6f 6361 6c41 490a 0a52  ..### LocalAI..R
-00001380: 6566 6572 2074 6f20 7468 6520 5b4c 6f63  efer to the [Loc
-00001390: 616c 4149 2064 6f63 735d 2868 7474 7073  alAI docs](https
-000013a0: 3a2f 2f6c 6f63 616c 6169 2e69 6f2f 2920  ://localai.io/) 
-000013b0: 666f 7220 696e 7374 616c 6c61 7469 6f6e  for installation
-000013c0: 2c20 6176 6169 6c61 626c 6520 6d6f 6465  , available mode
-000013d0: 6c73 2c20 616e 6420 7573 6167 652e 0a0a  ls, and usage...
-000013e0: 2323 2320 4f74 6865 7220 7761 7973 2074  ### Other ways t
-000013f0: 6f20 7275 6e20 5368 656c 6c4f 7261 636c  o run ShellOracl
-00001400: 650a 0a53 6865 6c6c 4f72 6163 6c65 2063  e..ShellOracle c
-00001410: 616e 2062 6520 7275 6e20 6173 2061 2050  an be run as a P
-00001420: 7974 686f 6e20 6d6f 6475 6c65 2077 6974  ython module wit
-00001430: 6820 6070 7974 686f 6e33 202d 6d20 7368  h `python3 -m sh
-00001440: 656c 6c6f 7261 636c 6560 206f 7220 7573  elloracle` or us
-00001450: 696e 6720 6974 7320 656e 7472 7970 6f69  ing its entrypoi
-00001460: 6e74 2060 7368 6f72 603b 2068 6f77 6576  nt `shor`; howev
-00001470: 6572 2c0a 7468 6572 6520 6172 6520 6120  er,.there are a 
-00001480: 6665 7720 6361 7665 6174 7320 7769 7468  few caveats with
-00001490: 2074 6869 7320 6d65 7468 6f64 3a0a 2d20   this method:.- 
-000014a0: 456e 7375 7265 2079 6f75 7220 607e 2f2e  Ensure your `~/.
-000014b0: 6c6f 6361 6c2f 6269 6e60 2064 6972 6563  local/bin` direc
-000014c0: 746f 7279 2069 7320 6164 6465 6420 746f  tory is added to
-000014d0: 2079 6f75 7220 5041 5448 2076 6172 6961   your PATH varia
-000014e0: 626c 6520 666f 7220 7468 6520 656e 7472  ble for the entr
-000014f0: 7970 6f69 6e74 2074 6f20 776f 726b 2e0a  ypoint to work..
-00001500: 2d20 5275 6e6e 696e 6720 5368 656c 6c4f  - Running ShellO
-00001510: 7261 636c 6520 7769 7468 2074 6869 7320  racle with this 
-00001520: 6d65 7468 6f64 2077 696c 6c20 6e6f 7420  method will not 
-00001530: 6175 746f 6d61 7469 6361 6c6c 7920 696e  automatically in
-00001540: 7365 7274 2074 6865 2072 6573 756c 7420  sert the result 
-00001550: 696e 746f 2079 6f75 7220 7368 656c 6c20  into your shell 
-00001560: 7072 6f6d 7074 2e0a 0a23 2323 2054 6970  prompt...### Tip
-00001570: 730a 0a31 2e20 4966 2079 6f75 2070 7265  s..1. If you pre
-00001580: 7373 2043 5452 4c2b 4620 7769 7468 2074  ss CTRL+F with t
-00001590: 6578 7420 696e 2079 6f75 7220 5a4c 4520  ext in your ZLE 
-000015a0: 6275 6666 6572 2c20 616c 6c20 7465 7874  buffer, all text
-000015b0: 206c 6566 7420 6f66 2079 6f75 7220 6375   left of your cu
-000015c0: 7273 6f72 2077 696c 6c20 6361 7272 7920  rsor will carry 
-000015d0: 6f76 6572 2074 6f20 796f 7572 2053 6865  over to your She
-000015e0: 6c6c 4f72 6163 6c65 0a20 2020 7072 6f6d  llOracle.   prom
-000015f0: 7074 2e0a 322e 2055 505f 4152 524f 5720  pt..2. UP_ARROW 
-00001600: 616e 6420 444f 574e 5f41 5252 4f57 2063  and DOWN_ARROW c
-00001610: 7963 6c65 2074 6872 6f75 6768 2079 6f75  ycle through you
-00001620: 7220 7072 6f6d 7074 2068 6973 746f 7279  r prompt history
-00001630: 2e0a 332e 2053 6865 6c6c 4f72 6163 6c65  ..3. ShellOracle
-00001640: 2063 616e 2062 6520 6368 6169 6e65 6420   can be chained 
-00001650: 7769 7468 206f 7468 6572 2063 6f6d 6d61  with other comma
-00001660: 6e64 733b 2074 7279 3a20 6065 6368 6f20  nds; try: `echo 
-00001670: 2266 696e 6420 616c 6c20 7468 6520 7079  "find all the py
-00001680: 7468 6f6e 2066 696c 6573 2069 6e20 6d79  thon files in my
-00001690: 2063 7764 2220 7c20 7368 6f72 600a 0a23   cwd" | shor`..#
-000016a0: 2320 436f 6e66 6967 7572 6174 696f 6e0a  # Configuration.
-000016b0: 0a53 6865 6c6c 4f72 6163 6c65 2773 2063  .ShellOracle's c
-000016c0: 6f6e 6669 6775 7261 7469 6f6e 2069 7320  onfiguration is 
-000016d0: 796f 7572 2067 6174 6577 6179 2074 6f20  your gateway to 
-000016e0: 7461 696c 6f72 696e 6720 7468 6520 7574  tailoring the ut
-000016f0: 696c 6974 7920 746f 206d 6174 6368 2079  ility to match y
-00001700: 6f75 7220 7072 6566 6572 656e 6365 7320  our preferences 
-00001710: 616e 6420 7265 7175 6972 656d 656e 7473  and requirements
-00001720: 2e0a 5468 6520 607e 2f2e 7368 656c 6c6f  ..The `~/.shello
-00001730: 7261 636c 652f 636f 6e66 6967 2e74 6f6d  racle/config.tom
-00001740: 6c60 2066 696c 6520 7365 7276 6573 2061  l` file serves a
-00001750: 7320 7468 6520 636f 6e74 726f 6c20 6365  s the control ce
-00001760: 6e74 6572 2066 6f72 2063 7573 746f 6d69  nter for customi
-00001770: 7a69 6e67 2076 6172 696f 7573 2061 7370  zing various asp
-00001780: 6563 7473 206f 6620 5368 656c 6c4f 7261  ects of ShellOra
-00001790: 636c 6527 730a 6265 6861 7669 6f72 2e0a  cle's.behavior..
-000017a0: 0a23 2320 5379 7374 656d 2052 6571 7569  .## System Requi
-000017b0: 7265 6d65 6e74 730a 0a23 2323 2053 6f66  rements..### Sof
-000017c0: 7477 6172 650a 0a53 6865 6c6c 4f72 6163  tware..ShellOrac
-000017d0: 6c65 2073 7570 706f 7274 7320 4241 5348  le supports BASH
-000017e0: 2061 6e64 205a 5348 206f 6e20 6d61 634f   and ZSH on macO
-000017f0: 5320 616e 6420 4c69 6e75 782e 0a0a 2323  S and Linux...##
-00001800: 2320 4861 7264 7761 7265 0a0a 466f 7220  # Hardware..For 
-00001810: 636c 6f75 6420 7072 6f76 6964 6572 7320  cloud providers 
-00001820: 6c69 6b65 204f 7065 6e41 492c 2074 6865  like OpenAI, the
-00001830: 7265 2061 7265 206e 6f20 7370 6563 6966  re are no specif
-00001840: 6963 2073 7973 7465 6d20 7265 7175 6972  ic system requir
-00001850: 656d 656e 7473 2e0a 0a49 6620 7365 6c66  ements...If self
-00001860: 2d68 6f73 7469 6e67 2c20 7379 7374 656d  -hosting, system
-00001870: 2072 6571 7569 7265 6d65 6e74 7320 7661   requirements va
-00001880: 7279 2062 6173 6564 206f 6e20 7468 6520  ry based on the 
-00001890: 6d6f 6465 6c20 7573 6564 2e20 5265 6665  model used. Refe
-000018a0: 7220 746f 2074 6865 204f 6c6c 616d 6120  r to the Ollama 
-000018b0: 6d6f 6465 6c20 7265 6769 7374 7279 2066  model registry f
-000018c0: 6f72 206d 6f72 650a 696e 666f 726d 6174  or more.informat
-000018d0: 696f 6e2e 0a0a 2323 2046 6565 6462 6163  ion...## Feedbac
-000018e0: 6b0a 0a45 6e63 6f75 6e74 6572 6564 2070  k..Encountered p
-000018f0: 726f 626c 656d 733f 205b 4669 6c65 2061  roblems? [File a
-00001900: 6e20 6973 7375 655d 2868 7474 7073 3a2f  n issue](https:/
-00001910: 2f67 6974 6875 622e 636f 6d2f 646a 636f  /github.com/djco
-00001920: 706c 6579 2f53 6865 6c6c 4f72 6163 6c65  pley/ShellOracle
-00001930: 2f69 7373 7565 732f 6e65 7729 2e20 4665  /issues/new). Fe
-00001940: 6174 7572 6520 7265 7175 6573 7473 2061  ature requests a
-00001950: 7265 2077 656c 636f 6d65 2c0a 616e 6420  re welcome,.and 
-00001960: 636f 6e74 7269 6275 7469 6f6e 7320 6361  contributions ca
-00001970: 6e20 6265 206d 6164 6520 6279 206f 7065  n be made by ope
-00001980: 6e69 6e67 2061 2070 756c 6c20 7265 7175  ning a pull requ
-00001990: 6573 742e 0a                             est..
+000004e0: 7369 6f6e 203c 2022 332e 3131 220a 0a3c  sion < "3.11"..<
+000004f0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000500: 3e0a 2020 3c69 6d67 2073 7263 3d22 6874  >.  <img src="ht
+00000510: 7470 733a 2f2f 692e 696d 6775 722e 636f  tps://i.imgur.co
+00000520: 6d2f 4973 5159 496e 4a2e 706e 6722 2061  m/IsQYInJ.png" a
+00000530: 6c74 3d22 5368 656c 6c4f 7261 636c 6520  lt="ShellOracle 
+00000540: 6c6f 676f 222f 3e0a 3c2f 703e 0a0a 3c68  logo"/>.</p>..<h
+00000550: 3120 616c 6967 6e3d 2263 656e 7465 7222  1 align="center"
+00000560: 3e53 6865 6c6c 4f72 6163 6c65 3c2f 6831  >ShellOracle</h1
+00000570: 3e0a 0a3c 7020 616c 6967 6e3d 2263 656e  >..<p align="cen
+00000580: 7465 7222 3e0a 2020 3c61 2068 7265 663d  ter">.  <a href=
+00000590: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000005a0: 636f 6d2f 646a 636f 706c 6579 2f53 6865  com/djcopley/She
+000005b0: 6c6c 4f72 6163 6c65 2f61 6374 696f 6e73  llOracle/actions
+000005c0: 2f77 6f72 6b66 6c6f 7773 2f74 6573 7473  /workflows/tests
+000005d0: 2e79 6d6c 223e 0a20 2020 2020 203c 696d  .yml">.      <im
+000005e0: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
+000005f0: 6974 6875 622e 636f 6d2f 646a 636f 706c  ithub.com/djcopl
+00000600: 6579 2f53 6865 6c6c 4f72 6163 6c65 2f61  ey/ShellOracle/a
+00000610: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000620: 2f74 6573 7473 2e79 6d6c 2f62 6164 6765  /tests.yml/badge
+00000630: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
+00000640: 2220 616c 743d 2254 6573 7473 223e 0a20  " alt="Tests">. 
+00000650: 203c 2f61 3e0a 2020 3c61 2068 7265 663d   </a>.  <a href=
+00000660: 2268 7474 7073 3a2f 2f62 6164 6765 2e66  "https://badge.f
+00000670: 7572 792e 696f 2f70 792f 7368 656c 6c6f  ury.io/py/shello
+00000680: 7261 636c 6522 3e0a 2020 2020 2020 3c69  racle">.      <i
+00000690: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000006a0: 6261 6467 652e 6675 7279 2e69 6f2f 7079  badge.fury.io/py
+000006b0: 2f73 6865 6c6c 6f72 6163 6c65 2e73 7667  /shelloracle.svg
+000006c0: 2220 616c 743d 2250 7950 4920 7665 7273  " alt="PyPI vers
+000006d0: 696f 6e22 3e0a 2020 3c2f 613e 0a20 203c  ion">.  </a>.  <
+000006e0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000006f0: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
+00000700: 7079 7069 2f73 6865 6c6c 6f72 6163 6c65  pypi/shelloracle
+00000710: 2f22 3e0a 2020 2020 2020 3c69 6d67 2073  /">.      <img s
+00000720: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000730: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000740: 7079 7665 7273 696f 6e73 2f73 6865 6c6c  pyversions/shell
+00000750: 6f72 6163 6c65 2e73 7667 2220 616c 743d  oracle.svg" alt=
+00000760: 2250 7950 4920 5375 7070 6f72 7465 6420  "PyPI Supported 
+00000770: 5079 7468 6f6e 2056 6572 7369 6f6e 7322  Python Versions"
+00000780: 3e0a 2020 3c2f 613e 0a20 203c 6120 6872  >.  </a>.  <a hr
+00000790: 6566 3d22 6874 7470 733a 2f2f 7065 7079  ef="https://pepy
+000007a0: 2e74 6563 682f 7072 6f6a 6563 742f 7368  .tech/project/sh
+000007b0: 656c 6c6f 7261 636c 6522 3e0a 2020 2020  elloracle">.    
+000007c0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+000007d0: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
+000007e0: 7465 6368 2f62 6164 6765 2f73 6865 6c6c  tech/badge/shell
+000007f0: 6f72 6163 6c65 2220 616c 743d 2244 6f77  oracle" alt="Dow
+00000800: 6e6c 6f61 6473 223e 0a20 203c 2f61 3e0a  nloads">.  </a>.
+00000810: 3c2f 703e 0a0a 5368 656c 6c4f 7261 636c  </p>..ShellOracl
+00000820: 6520 6973 2061 6e20 696e 6e6f 7661 7469  e is an innovati
+00000830: 7665 2074 6572 6d69 6e61 6c20 7574 696c  ve terminal util
+00000840: 6974 7920 6465 7369 676e 6564 2066 6f72  ity designed for
+00000850: 2069 6e74 656c 6c69 6765 6e74 2073 6865   intelligent she
+00000860: 6c6c 2063 6f6d 6d61 6e64 2067 656e 6572  ll command gener
+00000870: 6174 696f 6e2c 2062 7269 6e67 696e 6720  ation, bringing 
+00000880: 6120 6e65 7720 6c65 7665 6c20 6f66 0a65  a new level of.e
+00000890: 6666 6963 6965 6e63 7920 746f 2079 6f75  fficiency to you
+000008a0: 7220 636f 6d6d 616e 642d 6c69 6e65 2069  r command-line i
+000008b0: 6e74 6572 6163 7469 6f6e 732e 2053 6865  nteractions. She
+000008c0: 6c6c 4f72 6163 6c65 2063 7572 7265 6e74  llOracle current
+000008d0: 6c79 2073 7570 706f 7274 7320 4f6c 6c61  ly supports Olla
+000008e0: 6d61 2c20 4c6f 6361 6c41 492c 2061 6e64  ma, LocalAI, and
+000008f0: 204f 7065 6e41 4921 0a0a 215b 5368 656c   OpenAI!..![Shel
+00000900: 6c4f 7261 636c 655d 2868 7474 7073 3a2f  lOracle](https:/
+00000910: 2f69 2e69 6d67 7572 2e63 6f6d 2f47 4a58  /i.imgur.com/GJX
+00000920: 3365 4571 2e67 6966 290a 0a53 686f 7720  3eEq.gif)..Show 
+00000930: 796f 7572 2073 7570 706f 7274 2066 6f72  your support for
+00000940: 2053 6865 6c6c 4f72 6163 6c65 2061 6e64   ShellOracle and
+00000950: 206b 6565 7020 616e 2065 7965 206f 7574   keep an eye out
+00000960: 2066 6f72 2065 7863 6974 696e 6720 6e65   for exciting ne
+00000970: 7720 6465 7665 6c6f 706d 656e 7473 2062  w developments b
+00000980: 7920 636c 6963 6b69 6e67 2074 6865 20e2  y clicking the .
+00000990: ad90 2061 6e64 2061 20f0 9f91 8021 0a0a  .. and a ....!..
+000009a0: 2323 2054 6162 6c65 206f 6620 436f 6e74  ## Table of Cont
+000009b0: 656e 7473 0a0a 2d20 5b46 6561 7475 7265  ents..- [Feature
+000009c0: 735d 2823 6665 6174 7572 6573 290a 2d20  s](#features).- 
+000009d0: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2823  [Installation](#
+000009e0: 696e 7374 616c 6c61 7469 6f6e 290a 2d20  installation).- 
+000009f0: 5b55 7361 6765 5d28 2375 7361 6765 290a  [Usage](#usage).
+00000a00: 2d20 5b50 726f 7669 6465 7273 5d28 2370  - [Providers](#p
+00000a10: 726f 7669 6465 7273 290a 2d20 5b43 6f6e  roviders).- [Con
+00000a20: 6669 6775 7261 7469 6f6e 5d28 2363 6f6e  figuration](#con
+00000a30: 6669 6775 7261 7469 6f6e 290a 2d20 5b53  figuration).- [S
+00000a40: 7973 7465 6d20 5265 7175 6972 656d 656e  ystem Requiremen
+00000a50: 7473 5d28 2373 7973 7465 6d2d 7265 7175  ts](#system-requ
+00000a60: 6972 656d 656e 7473 290a 2d20 5b46 6565  irements).- [Fee
+00000a70: 6462 6163 6b5d 2823 6665 6564 6261 636b  dback](#feedback
+00000a80: 290a 0a23 2320 4665 6174 7572 6573 0a0a  )..## Features..
+00000a90: 4b65 7920 6665 6174 7572 6573 206f 6620  Key features of 
+00000aa0: 5368 656c 6c4f 7261 636c 6520 696e 636c  ShellOracle incl
+00000ab0: 7564 653a 0a0a 2a20 5365 616d 6c65 7373  ude:..* Seamless
+00000ac0: 2073 6865 6c6c 2063 6f6d 6d61 6e64 2067   shell command g
+00000ad0: 656e 6572 6174 696f 6e20 6672 6f6d 2077  eneration from w
+00000ae0: 7269 7474 656e 2064 6573 6372 6970 7469  ritten descripti
+00000af0: 6f6e 730a 2a20 436f 6d6d 616e 6420 6869  ons.* Command hi
+00000b00: 7374 6f72 7920 666f 7220 6561 7379 2072  story for easy r
+00000b10: 6566 6572 656e 6365 0a2a 2055 6e69 7820  eference.* Unix 
+00000b20: 7069 7065 2073 7570 706f 7274 2066 6f72  pipe support for
+00000b30: 2061 6476 616e 6365 6420 636f 6d6d 616e   advanced comman
+00000b40: 6420 6368 6169 6e69 6e67 0a2a 2053 656c  d chaining.* Sel
+00000b50: 662d 686f 7374 6564 2066 6f72 2066 756c  f-hosted for ful
+00000b60: 6c20 636f 6e74 726f 6c20 6f76 6572 2079  l control over y
+00000b70: 6f75 7220 656e 7669 726f 6e6d 656e 740a  our environment.
+00000b80: 2a20 4869 6768 6c79 2063 6f6e 6669 6775  * Highly configu
+00000b90: 7261 626c 6520 746f 2061 6461 7074 2074  rable to adapt t
+00000ba0: 6f20 796f 7572 2070 7265 6665 7265 6e63  o your preferenc
+00000bb0: 6573 0a0a 2323 2049 6e73 7461 6c6c 6174  es..## Installat
+00000bc0: 696f 6e0a 0a49 6e73 7461 6c6c 696e 6720  ion..Installing 
+00000bd0: 5368 656c 6c4f 7261 636c 6520 6973 2065  ShellOracle is e
+00000be0: 6173 7921 0a0a 312e 205b 7069 7078 5d28  asy!..1. [pipx](
+00000bf0: 6874 7470 733a 2f2f 7069 7078 2e70 7970  https://pipx.pyp
+00000c00: 612e 696f 2f6c 6174 6573 742f 2920 696e  a.io/latest/) in
+00000c10: 7374 616c 6c20 7468 6520 6073 6865 6c6c  stall the `shell
+00000c20: 6f72 6163 6c65 6020 7061 636b 6167 650a  oracle` package.
+00000c30: 2020 2020 6060 6073 6865 6c6c 0a20 2020      ```shell.   
+00000c40: 2070 6970 7820 696e 7374 616c 6c20 7368   pipx install sh
+00000c50: 656c 6c6f 7261 636c 650a 2020 2020 6060  elloracle.    ``
+00000c60: 600a 322e 2043 6f6e 6669 6775 7265 2053  `.2. Configure S
+00000c70: 6865 6c6c 4f72 6163 6c65 2061 6e64 2066  hellOracle and f
+00000c80: 6f6c 6c6f 7720 7468 6520 7072 6f6d 7074  ollow the prompt
+00000c90: 730a 2020 2020 6060 6073 6865 6c6c 0a20  s.    ```shell. 
+00000ca0: 2020 2073 686f 7220 636f 6e66 6967 7572     shor configur
+00000cb0: 650a 2020 2020 6060 600a 332e 2052 6566  e.    ```.3. Ref
+00000cc0: 6572 2074 6f20 7468 6520 5b70 726f 7669  er to the [provi
+00000cd0: 6465 7273 5d28 2370 726f 7669 6465 7273  ders](#providers
+00000ce0: 2920 7365 6374 696f 6e20 666f 7220 7370  ) section for sp
+00000cf0: 6563 6966 6963 2064 6574 6169 6c73 2072  ecific details r
+00000d00: 6567 6172 6469 6e67 2079 6f75 7220 6368  egarding your ch
+00000d10: 6f73 656e 2070 726f 7669 6465 722e 0a0a  osen provider...
+00000d20: 5570 6772 6164 696e 6720 746f 2074 6865  Upgrading to the
+00000d30: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
+00000d40: 6f66 2053 6865 6c6c 4f72 6163 6c65 2069  of ShellOracle i
+00000d50: 7320 6a75 7374 2061 7320 7369 6d70 6c65  s just as simple
+00000d60: 210a 0a31 2e20 7069 7078 2075 7067 7261  !..1. pipx upgra
+00000d70: 6465 2074 6865 2060 7368 656c 6c6f 7261  de the `shellora
+00000d80: 636c 6560 2070 6163 6b61 6765 0a20 2020  cle` package.   
+00000d90: 2060 6060 7368 656c 6c0a 2020 2070 6970   ```shell.   pip
+00000da0: 7820 7570 6772 6164 6520 7368 656c 6c6f  x upgrade shello
+00000db0: 7261 636c 650a 2020 2060 6060 0a0a 2a49  racle.   ```..*I
+00000dc0: 6e73 7461 6c6c 6174 696f 6e20 7769 7468  nstallation with
+00000dd0: 2060 7069 7060 2069 7320 7375 7070 6f72   `pip` is suppor
+00000de0: 7465 642c 2068 6f77 6576 6572 2c20 6070  ted, however, `p
+00000df0: 6970 7860 2069 7320 7072 6566 6572 7265  ipx` is preferre
+00000e00: 6420 666f 7220 6974 7320 6175 746f 6d61  d for its automa
+00000e10: 7469 6320 656e 7669 726f 6e6d 656e 7420  tic environment 
+00000e20: 6973 6f6c 6174 696f 6e2e 2a0a 0a23 2320  isolation.*..## 
+00000e30: 5573 6167 650a 0a53 6865 6c6c 4f72 6163  Usage..ShellOrac
+00000e40: 6c65 2069 7320 6465 7369 676e 6564 2074  le is designed t
+00000e50: 6f20 6265 2075 7365 6420 6173 2061 2042  o be used as a B
+00000e60: 4153 482f 5a53 4820 7769 6467 6574 2061  ASH/ZSH widget a
+00000e70: 6374 6976 6174 6564 2062 7920 7468 6520  ctivated by the 
+00000e80: 4354 524c 2b46 206b 6579 626f 6172 6420  CTRL+F keyboard 
+00000e90: 7368 6f72 7463 7574 2e0a 0a31 2e20 5072  shortcut...1. Pr
+00000ea0: 6573 7320 4354 524c 2b46 0a32 2e20 4465  ess CTRL+F.2. De
+00000eb0: 7363 7269 6265 2079 6f75 7220 636f 6d6d  scribe your comm
+00000ec0: 616e 640a 332e 2050 7265 7373 2045 6e74  and.3. Press Ent
+00000ed0: 6572 0a0a 5468 6520 6765 6e65 7261 7465  er..The generate
+00000ee0: 6420 636f 6d6d 616e 6420 7769 6c6c 2062  d command will b
+00000ef0: 6520 696e 7365 7274 6564 2069 6e74 6f20  e inserted into 
+00000f00: 796f 7572 2073 6865 6c6c 2070 726f 6d70  your shell promp
+00000f10: 7420 6166 7465 7220 6120 6272 6965 6620  t after a brief 
+00000f20: 7072 6f63 6573 7369 6e67 2070 6572 696f  processing perio
+00000f30: 642e 0a0a 2323 2320 4f74 6865 7220 7761  d...### Other wa
+00000f40: 7973 2074 6f20 7275 6e20 5368 656c 6c4f  ys to run ShellO
+00000f50: 7261 636c 650a 0a53 6865 6c6c 4f72 6163  racle..ShellOrac
+00000f60: 6c65 2063 616e 2062 6520 7275 6e20 6173  le can be run as
+00000f70: 2061 2050 7974 686f 6e20 6d6f 6475 6c65   a Python module
+00000f80: 2077 6974 6820 6070 7974 686f 6e33 202d   with `python3 -
+00000f90: 6d20 7368 656c 6c6f 7261 636c 6560 206f  m shelloracle` o
+00000fa0: 7220 7573 696e 6720 6974 7320 656e 7472  r using its entr
+00000fb0: 7970 6f69 6e74 2060 7368 6f72 602c 2068  ypoint `shor`, h
+00000fc0: 6f77 6576 6572 2c0a 7275 6e6e 696e 6720  owever,.running 
+00000fd0: 5368 656c 6c4f 7261 636c 6520 7769 7468  ShellOracle with
+00000fe0: 2074 6869 7320 6d65 7468 6f64 2077 696c   this method wil
+00000ff0: 6c20 6e6f 7420 6175 746f 6d61 7469 6361  l not automatica
+00001000: 6c6c 7920 696e 7365 7274 2074 6865 2072  lly insert the r
+00001010: 6573 756c 7420 696e 746f 2079 6f75 7220  esult into your 
+00001020: 7368 656c 6c20 7072 6f6d 7074 2e0a 0a23  shell prompt...#
+00001030: 2323 2054 6970 730a 0a31 2e20 4966 2079  ## Tips..1. If y
+00001040: 6f75 2070 7265 7373 2043 5452 4c2b 4620  ou press CTRL+F 
+00001050: 7769 7468 2074 6578 7420 696e 2079 6f75  with text in you
+00001060: 7220 5a4c 4520 6275 6666 6572 2c20 616c  r ZLE buffer, al
+00001070: 6c20 7465 7874 206c 6566 7420 6f66 2079  l text left of y
+00001080: 6f75 7220 6375 7273 6f72 2077 696c 6c20  our cursor will 
+00001090: 6361 7272 7920 6f76 6572 2074 6f20 796f  carry over to yo
+000010a0: 7572 2053 6865 6c6c 4f72 6163 6c65 0a20  ur ShellOracle. 
+000010b0: 2020 7072 6f6d 7074 2e0a 322e 20e2 ac86    prompt..2. ...
+000010c0: efb8 8f20 6172 726f 7720 616e 6420 e2ac  ... arrow and ..
+000010d0: 87ef b88f 2061 7272 6f77 2063 7963 6c65  .... arrow cycle
+000010e0: 2074 6872 6f75 6768 2079 6f75 7220 7072   through your pr
+000010f0: 6f6d 7074 2068 6973 746f 7279 2e0a 332e  ompt history..3.
+00001100: 2053 6865 6c6c 4f72 6163 6c65 2063 616e   ShellOracle can
+00001110: 2062 6520 6368 6169 6e65 6420 7769 7468   be chained with
+00001120: 206f 7468 6572 2063 6f6d 6d61 6e64 733b   other commands;
+00001130: 2074 7279 3a20 6065 6368 6f20 2266 696e   try: `echo "fin
+00001140: 6420 616c 6c20 7468 6520 7079 7468 6f6e  d all the python
+00001150: 2066 696c 6573 2069 6e20 6d79 2063 7764   files in my cwd
+00001160: 2220 7c20 7368 6f72 600a 0a23 2320 5072  " | shor`..## Pr
+00001170: 6f76 6964 6572 730a 0a23 2323 204f 6c6c  oviders..### Oll
+00001180: 616d 610a 0a42 6566 6f72 6520 7573 696e  ama..Before usin
+00001190: 6720 5368 656c 6c4f 7261 636c 6520 7769  g ShellOracle wi
+000011a0: 7468 204f 6c6c 616d 612c 2070 756c 6c20  th Ollama, pull 
+000011b0: 7468 6520 6d6f 6465 6c20 796f 7520 6368  the model you ch
+000011c0: 6f73 6520 696e 2074 6865 2063 6f6e 6669  ose in the confi
+000011d0: 6775 7265 2073 7465 702e 0a46 6f72 2065  gure step..For e
+000011e0: 7861 6d70 6c65 2c20 6966 2079 6f75 2063  xample, if you c
+000011f0: 686f 7365 2060 646f 6c70 6869 6e2d 6d69  hose `dolphin-mi
+00001200: 7374 7261 6c60 2c20 7275 6e3a 0a0a 6060  stral`, run:..``
+00001210: 6073 6865 6c6c 0a6f 6c6c 616d 6120 7075  `shell.ollama pu
+00001220: 6c6c 2064 6f6c 7068 696e 2d6d 6973 7472  ll dolphin-mistr
+00001230: 616c 0a60 6060 0a0a 5265 6665 7220 746f  al.```..Refer to
+00001240: 2074 6865 205b 4f6c 6c61 6d61 2064 6f63   the [Ollama doc
+00001250: 735d 2868 7474 7073 3a2f 2f6f 6c6c 616d  s](https://ollam
+00001260: 612e 6169 2920 666f 7220 696e 7374 616c  a.ai) for instal
+00001270: 6c61 7469 6f6e 2c20 6176 6169 6c61 626c  lation, availabl
+00001280: 6520 6d6f 6465 6c73 2c20 616e 6420 7573  e models, and us
+00001290: 6167 652e 0a0a 2323 2320 4f70 656e 4149  age...### OpenAI
+000012a0: 0a0a 546f 2075 7365 2053 6865 6c6c 4f72  ..To use ShellOr
+000012b0: 6163 6c65 2077 6974 6820 7468 6520 4f70  acle with the Op
+000012c0: 656e 4149 2070 726f 7669 6465 722c 2063  enAI provider, c
+000012d0: 7265 6174 6520 616e 205b 4150 4920 6b65  reate an [API ke
+000012e0: 795d 2868 7474 7073 3a2f 2f70 6c61 7466  y](https://platf
+000012f0: 6f72 6d2e 6f70 656e 6169 2e63 6f6d 2f61  orm.openai.com/a
+00001300: 6363 6f75 6e74 2f61 7069 2d6b 6579 7329  ccount/api-keys)
+00001310: 2e20 4564 6974 0a79 6f75 7220 607e 2f2e  . Edit.your `~/.
+00001320: 7368 656c 6c6f 7261 636c 652f 636f 6e66  shelloracle/conf
+00001330: 6967 2e74 6f6d 6c60 2074 6f20 6368 616e  ig.toml` to chan
+00001340: 6765 2079 6f75 7220 7072 6f76 6964 6572  ge your provider
+00001350: 2061 6e64 2065 6e74 6572 2079 6f75 7220   and enter your 
+00001360: 4150 4920 6b65 792e 0a0a 2323 2320 4c6f  API key...### Lo
+00001370: 6361 6c41 490a 0a52 6566 6572 2074 6f20  calAI..Refer to 
+00001380: 7468 6520 5b4c 6f63 616c 4149 2064 6f63  the [LocalAI doc
+00001390: 735d 2868 7474 7073 3a2f 2f6c 6f63 616c  s](https://local
+000013a0: 6169 2e69 6f2f 2920 666f 7220 696e 7374  ai.io/) for inst
+000013b0: 616c 6c61 7469 6f6e 2c20 6176 6169 6c61  allation, availa
+000013c0: 626c 6520 6d6f 6465 6c73 2c20 616e 6420  ble models, and 
+000013d0: 7573 6167 652e 0a0a 2323 2043 6f6e 6669  usage...## Confi
+000013e0: 6775 7261 7469 6f6e 0a0a 5368 656c 6c4f  guration..ShellO
+000013f0: 7261 636c 6527 7320 636f 6e66 6967 7572  racle's configur
+00001400: 6174 696f 6e20 6973 2079 6f75 7220 6761  ation is your ga
+00001410: 7465 7761 7920 746f 2074 6169 6c6f 7269  teway to tailori
+00001420: 6e67 2074 6865 2075 7469 6c69 7479 2074  ng the utility t
+00001430: 6f20 6d61 7463 6820 796f 7572 2070 7265  o match your pre
+00001440: 6665 7265 6e63 6573 2061 6e64 2072 6571  ferences and req
+00001450: 7569 7265 6d65 6e74 732e 0a54 6865 2060  uirements..The `
+00001460: 7e2f 2e73 6865 6c6c 6f72 6163 6c65 2f63  ~/.shelloracle/c
+00001470: 6f6e 6669 672e 746f 6d6c 6020 6669 6c65  onfig.toml` file
+00001480: 2073 6572 7665 7320 6173 2074 6865 2063   serves as the c
+00001490: 6f6e 7472 6f6c 2063 656e 7465 7220 666f  ontrol center fo
+000014a0: 7220 6375 7374 6f6d 697a 696e 6720 7661  r customizing va
+000014b0: 7269 6f75 7320 6173 7065 6374 7320 6f66  rious aspects of
+000014c0: 2053 6865 6c6c 4f72 6163 6c65 2773 0a62   ShellOracle's.b
+000014d0: 6568 6176 696f 722e 0a0a 2323 2053 7973  ehavior...## Sys
+000014e0: 7465 6d20 5265 7175 6972 656d 656e 7473  tem Requirements
+000014f0: 0a0a 2323 2320 536f 6674 7761 7265 0a0a  ..### Software..
+00001500: 5368 656c 6c4f 7261 636c 6520 7375 7070  ShellOracle supp
+00001510: 6f72 7473 2042 4153 4820 616e 6420 5a53  orts BASH and ZS
+00001520: 4820 6f6e 206d 6163 4f53 2061 6e64 204c  H on macOS and L
+00001530: 696e 7578 2e0a 0a23 2323 2048 6172 6477  inux...### Hardw
+00001540: 6172 650a 0a46 6f72 2063 6c6f 7564 2070  are..For cloud p
+00001550: 726f 7669 6465 7273 206c 696b 6520 4f70  roviders like Op
+00001560: 656e 4149 2c20 7468 6572 6520 6172 6520  enAI, there are 
+00001570: 6e6f 2068 6172 6477 6172 6520 7265 7175  no hardware requ
+00001580: 6972 656d 656e 7473 2e0a 0a49 6620 7275  irements...If ru
+00001590: 6e6e 696e 6720 6c6f 6361 6c6c 792c 2072  nning locally, r
+000015a0: 6566 6572 2074 6f20 796f 7572 206d 6f64  efer to your mod
+000015b0: 656c 2066 6f72 2068 6172 6477 6172 6520  el for hardware 
+000015c0: 7265 7175 6972 656d 656e 7473 2e0a 0a23  requirements...#
+000015d0: 2320 4665 6564 6261 636b 0a0a 456e 636f  # Feedback..Enco
+000015e0: 756e 7465 7265 6420 7072 6f62 6c65 6d73  untered problems
+000015f0: 3f20 5b46 696c 6520 616e 2069 7373 7565  ? [File an issue
+00001600: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001610: 2e63 6f6d 2f64 6a63 6f70 6c65 792f 5368  .com/djcopley/Sh
+00001620: 656c 6c4f 7261 636c 652f 6973 7375 6573  ellOracle/issues
+00001630: 2f6e 6577 292e 2046 6561 7475 7265 2072  /new). Feature r
+00001640: 6571 7565 7374 7320 6172 6520 7765 6c63  equests are welc
+00001650: 6f6d 652c 0a61 6e64 2063 6f6e 7472 6962  ome,.and contrib
+00001660: 7574 696f 6e73 2063 616e 2062 6520 6d61  utions can be ma
+00001670: 6465 2062 7920 6f70 656e 696e 6720 6120  de by opening a 
+00001680: 7075 6c6c 2072 6571 7565 7374 2e0a 0a23  pull request...#
+00001690: 2320 4c69 6365 6e73 650a 0a54 6869 7320  # License..This 
+000016a0: 736f 6674 7761 7265 2069 7320 6c69 6365  software is lice
+000016b0: 6e73 6564 2075 6e64 6572 2074 6865 2047  nsed under the G
+000016c0: 504c 7633 206c 6963 656e 7365 2e0a       PLv3 license..
```

### Comparing `shelloracle-1.1.2/README.md` & `shelloracle-1.3.0/src/shelloracle.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,331 +1,365 @@
-00000000: 5b21 5b54 6573 7473 5d28 6874 7470 733a  [![Tests](https:
-00000010: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6a63  //github.com/djc
-00000020: 6f70 6c65 792f 5368 656c 6c4f 7261 636c  opley/ShellOracl
-00000030: 652f 6163 7469 6f6e 732f 776f 726b 666c  e/actions/workfl
-00000040: 6f77 732f 7465 7374 732e 796d 6c2f 6261  ows/tests.yml/ba
-00000050: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
-00000060: 6169 6e29 5d28 6874 7470 733a 2f2f 6769  ain)](https://gi
-00000070: 7468 7562 2e63 6f6d 2f64 6a63 6f70 6c65  thub.com/djcople
-00000080: 792f 5368 656c 6c4f 7261 636c 652f 6163  y/ShellOracle/ac
-00000090: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-000000a0: 7465 7374 732e 796d 6c29 0a5b 215b 5079  tests.yml).[![Py
-000000b0: 5049 2076 6572 7369 6f6e 5d28 6874 7470  PI version](http
-000000c0: 733a 2f2f 6261 6467 652e 6675 7279 2e69  s://badge.fury.i
-000000d0: 6f2f 7079 2f73 6865 6c6c 6f72 6163 6c65  o/py/shelloracle
-000000e0: 2e73 7667 295d 2868 7474 7073 3a2f 2f62  .svg)](https://b
-000000f0: 6164 6765 2e66 7572 792e 696f 2f70 792f  adge.fury.io/py/
-00000100: 7368 656c 6c6f 7261 636c 6529 0a5b 215b  shelloracle).[![
-00000110: 5079 5049 2053 7570 706f 7274 6564 2050  PyPI Supported P
-00000120: 7974 686f 6e20 5665 7273 696f 6e73 5d28  ython Versions](
-00000130: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000140: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
-00000150: 7273 696f 6e73 2f73 6865 6c6c 6f72 6163  rsions/shellorac
-00000160: 6c65 2e73 7667 295d 2868 7474 7073 3a2f  le.svg)](https:/
-00000170: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-00000180: 2f70 7970 692f 7368 656c 6c6f 7261 636c  /pypi/shelloracl
-00000190: 652f 290a 5b21 5b44 6f77 6e6c 6f61 6473  e/).[![Downloads
-000001a0: 5d28 6874 7470 733a 2f2f 7374 6174 6963  ](https://static
-000001b0: 2e70 6570 792e 7465 6368 2f62 6164 6765  .pepy.tech/badge
-000001c0: 2f73 6865 6c6c 6f72 6163 6c65 295d 2868  /shelloracle)](h
-000001d0: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
-000001e0: 2f70 726f 6a65 6374 2f73 6865 6c6c 6f72  /project/shellor
-000001f0: 6163 6c65 290a 0a23 2053 6865 6c6c 4f72  acle)..# ShellOr
-00000200: 6163 6c65 0a0a 5368 656c 6c4f 7261 636c  acle..ShellOracl
-00000210: 6520 6973 2061 6e20 696e 6e6f 7661 7469  e is an innovati
-00000220: 7665 2074 6572 6d69 6e61 6c20 7574 696c  ve terminal util
-00000230: 6974 7920 6465 7369 676e 6564 2066 6f72  ity designed for
-00000240: 2069 6e74 656c 6c69 6765 6e74 2073 6865   intelligent she
-00000250: 6c6c 2063 6f6d 6d61 6e64 2067 656e 6572  ll command gener
-00000260: 6174 696f 6e2c 2062 7269 6e67 696e 6720  ation, bringing 
-00000270: 6120 6e65 7720 6c65 7665 6c20 6f66 0a65  a new level of.e
-00000280: 6666 6963 6965 6e63 7920 746f 2079 6f75  fficiency to you
-00000290: 7220 636f 6d6d 616e 642d 6c69 6e65 2069  r command-line i
-000002a0: 6e74 6572 6163 7469 6f6e 732e 2053 6865  nteractions. She
-000002b0: 6c6c 4f72 6163 6c65 2063 7572 7265 6e74  llOracle current
-000002c0: 6c79 2073 7570 706f 7274 7320 4f6c 6c61  ly supports Olla
-000002d0: 6d61 2c20 4c6f 6361 6c41 492c 2061 6e64  ma, LocalAI, and
-000002e0: 204f 7065 6e41 4921 0a0a 215b 5368 656c   OpenAI!..![Shel
-000002f0: 6c4f 7261 636c 655d 2868 7474 7073 3a2f  lOracle](https:/
-00000300: 2f69 2e69 6d67 7572 2e63 6f6d 2f6d 6731  /i.imgur.com/mg1
-00000310: 7243 7a64 2e67 6966 290a 0a45 7870 6c6f  rCzd.gif)..Explo
-00000320: 7265 206f 7572 2064 796e 616d 6963 2066  re our dynamic f
-00000330: 6561 7475 7265 7320 616e 6420 6c6f 6f6b  eatures and look
-00000340: 2066 6f72 7761 7264 2074 6f20 6d6f 7265   forward to more
-00000350: 2065 7863 6974 696e 6720 7570 6461 7465   exciting update
-00000360: 7320 6279 2067 6976 696e 6720 7573 2061  s by giving us a
-00000370: 20e2 ad90 2061 6e64 2061 20f0 9f91 800a   ... and a .....
-00000380: 0a23 2320 5461 626c 6520 6f66 2043 6f6e  .## Table of Con
-00000390: 7465 6e74 730a 0a2d 205b 496e 7472 6f64  tents..- [Introd
-000003a0: 7563 7469 6f6e 5d28 2369 6e74 726f 6475  uction](#introdu
-000003b0: 6374 696f 6e29 0a2d 205b 4665 6174 7572  ction).- [Featur
-000003c0: 6573 5d28 2366 6561 7475 7265 7329 0a2d  es](#features).-
-000003d0: 205b 496e 7374 616c 6c61 7469 6f6e 5d28   [Installation](
-000003e0: 2369 6e73 7461 6c6c 6174 696f 6e29 0a2d  #installation).-
-000003f0: 205b 5573 6167 655d 2823 7573 6167 6529   [Usage](#usage)
-00000400: 0a2d 205b 5072 6f76 6964 6572 735d 2823  .- [Providers](#
-00000410: 7072 6f76 6964 6572 7329 0a2d 205b 436f  providers).- [Co
-00000420: 6e66 6967 7572 6174 696f 6e5d 2823 636f  nfiguration](#co
-00000430: 6e66 6967 7572 6174 696f 6e29 0a2d 205b  nfiguration).- [
-00000440: 5379 7374 656d 2052 6571 7569 7265 6d65  System Requireme
-00000450: 6e74 735d 2823 7379 7374 656d 2d72 6571  nts](#system-req
-00000460: 7569 7265 6d65 6e74 7329 0a2d 205b 4665  uirements).- [Fe
-00000470: 6564 6261 636b 5d28 2366 6565 6462 6163  edback](#feedbac
-00000480: 6b29 0a0a 2323 2049 6e74 726f 6475 6374  k)..## Introduct
-00000490: 696f 6e0a 0a4d 6565 7420 5368 656c 6c4f  ion..Meet ShellO
-000004a0: 7261 636c 65e2 8094 6120 6861 6e64 7920  racle...a handy 
-000004b0: 746f 6f6c 2074 6861 7420 6d61 6b65 7320  tool that makes 
-000004c0: 776f 726b 696e 6720 7769 7468 2074 6865  working with the
-000004d0: 2063 6f6d 6d61 6e64 206c 696e 6520 6120   command line a 
-000004e0: 6269 7420 736d 6f6f 7468 6572 2e20 5468  bit smoother. Th
-000004f0: 6973 2074 6572 6d69 6e61 6c20 7574 696c  is terminal util
-00000500: 6974 7920 6c65 7473 2079 6f75 0a63 7265  ity lets you.cre
-00000510: 6174 6520 7368 656c 6c20 636f 6d6d 616e  ate shell comman
-00000520: 6473 2062 7920 6465 7363 7269 6269 6e67  ds by describing
-00000530: 2077 6861 7420 796f 7520 7761 6e74 2074   what you want t
-00000540: 6f20 646f 2069 6e20 706c 6169 6e20 6c61  o do in plain la
-00000550: 6e67 7561 6765 2e20 5368 656c 6c4f 7261  nguage. ShellOra
-00000560: 636c 6520 7369 6d70 6c69 6669 6573 2074  cle simplifies t
-00000570: 6865 2070 726f 6365 7373 206f 660a 6372  he process of.cr
-00000580: 6166 7469 6e67 2063 6f6d 706c 6578 2063  afting complex c
-00000590: 6f6d 6d61 6e64 7320 6279 2072 656d 6f76  ommands by remov
-000005a0: 696e 6720 7468 6520 6e65 6564 2074 6f20  ing the need to 
-000005b0: 676f 6f67 6c65 2061 6e64 2063 6f6d 6220  google and comb 
-000005c0: 6d61 6e20 7061 6765 732e 0a0a 2a2a 5768  man pages...**Wh
-000005d0: 7920 5368 656c 6c4f 7261 636c 653f 2a2a  y ShellOracle?**
-000005e0: 0a0a 2a20 2a2a 4e6f 204d 6f72 6520 4d65  ..* **No More Me
-000005f0: 6d6f 7269 7a69 6e67 3a2a 2a20 466f 7267  morizing:** Forg
-00000600: 6574 2061 626f 7574 2072 656d 656d 6265  et about remembe
-00000610: 7269 6e67 2063 6f6d 706c 6578 2073 6865  ring complex she
-00000620: 6c6c 2063 6f6d 6d61 6e64 732e 204a 7573  ll commands. Jus
-00000630: 7420 7465 6c6c 2053 6865 6c6c 4f72 6163  t tell ShellOrac
-00000640: 6c65 2077 6861 7420 796f 7520 6e65 6564  le what you need
-00000650: 2c20 616e 640a 2020 6974 276c 6c20 6765  , and.  it'll ge
-00000660: 6e65 7261 7465 2074 6865 2063 6f6d 6d61  nerate the comma
-00000670: 6e64 2066 6f72 2079 6f75 2e0a 0a2a 202a  nd for you...* *
-00000680: 2a53 6176 6520 5469 6d65 2c20 5374 6179  *Save Time, Stay
-00000690: 2046 6f63 7573 6564 3a2a 2a20 5361 7920   Focused:** Say 
-000006a0: 676f 6f64 6279 6520 746f 206d 616e 7561  goodbye to manua
-000006b0: 6c20 636f 6d6d 616e 6420 6372 6166 7469  l command crafti
-000006c0: 6e67 2e20 5368 656c 6c4f 7261 636c 6520  ng. ShellOracle 
-000006d0: 6865 6c70 7320 796f 7520 7361 7665 2074  helps you save t
-000006e0: 696d 6520 616e 6420 636f 6e63 656e 7472  ime and concentr
-000006f0: 6174 650a 2020 6f6e 2077 6861 7420 7265  ate.  on what re
-00000700: 616c 6c79 206d 6174 7465 7273 2062 7920  ally matters by 
-00000710: 7573 696e 6720 6e61 7475 7261 6c20 6c61  using natural la
-00000720: 6e67 7561 6765 2064 6573 6372 6970 7469  nguage descripti
-00000730: 6f6e 732e 0a0a 2a20 2a2a 4164 6170 7461  ons...* **Adapta
-00000740: 626c 6520 746f 2059 6f75 7220 4e65 6564  ble to Your Need
-00000750: 733a 2a2a 2057 6865 7468 6572 2069 7427  s:** Whether it'
-00000760: 7320 6120 7175 6963 6b20 6f6e 652d 6c69  s a quick one-li
-00000770: 6e65 7220 6f72 2061 2073 6571 7565 6e63  ner or a sequenc
-00000780: 6520 6f66 2063 6f6d 6d61 6e64 732c 2053  e of commands, S
-00000790: 6865 6c6c 4f72 6163 6c65 2069 7320 666c  hellOracle is fl
-000007a0: 6578 6962 6c65 2e20 4974 0a20 2073 7570  exible. It.  sup
-000007b0: 706f 7274 7320 556e 6978 2070 6970 6573  ports Unix pipes
-000007c0: 2061 6e64 206b 6565 7073 2074 7261 636b   and keeps track
-000007d0: 206f 6620 796f 7572 2063 6f6d 6d61 6e64   of your command
-000007e0: 2068 6973 746f 7279 2e0a 0a2a 202a 2a59   history...* **Y
-000007f0: 6f75 7220 436f 6e74 726f 6c2c 2059 6f75  our Control, You
-00000800: 7220 5761 793a 2a2a 2052 756e 2053 6865  r Way:** Run She
-00000810: 6c6c 4f72 6163 6c65 2061 7320 6120 7365  llOracle as a se
-00000820: 6c66 2d68 6f73 7465 6420 7574 696c 6974  lf-hosted utilit
-00000830: 7920 746f 2068 6176 6520 636f 6d70 6c65  y to have comple
-00000840: 7465 2063 6f6e 7472 6f6c 2e20 5461 696c  te control. Tail
-00000850: 6f72 2069 7420 746f 2079 6f75 720a 2020  or it to your.  
-00000860: 7072 6566 6572 656e 6365 7320 616e 6420  preferences and 
-00000870: 6d61 6b65 2069 7420 776f 726b 206a 7573  make it work jus
-00000880: 7420 7468 6520 7761 7920 796f 7520 7761  t the way you wa
-00000890: 6e74 2e0a 0a47 6976 6520 6974 2061 2074  nt...Give it a t
-000008a0: 7279 2061 6e64 2073 6565 2068 6f77 2069  ry and see how i
-000008b0: 7420 6669 7473 2069 6e74 6f20 796f 7572  t fits into your
-000008c0: 2077 6f72 6b66 6c6f 7721 0a0a 2323 2046   workflow!..## F
-000008d0: 6561 7475 7265 730a 0a4b 6579 2066 6561  eatures..Key fea
-000008e0: 7475 7265 7320 6f66 2053 6865 6c6c 4f72  tures of ShellOr
-000008f0: 6163 6c65 2069 6e63 6c75 6465 3a0a 0a2a  acle include:..*
-00000900: 2053 6561 6d6c 6573 7320 7368 656c 6c20   Seamless shell 
-00000910: 636f 6d6d 616e 6420 6765 6e65 7261 7469  command generati
-00000920: 6f6e 2066 726f 6d20 7772 6974 7465 6e20  on from written 
-00000930: 6465 7363 7269 7074 696f 6e73 0a2a 2043  descriptions.* C
-00000940: 6f6d 6d61 6e64 2068 6973 746f 7279 2066  ommand history f
-00000950: 6f72 2065 6173 7920 7265 6665 7265 6e63  or easy referenc
-00000960: 650a 2a20 556e 6978 2070 6970 6520 7375  e.* Unix pipe su
-00000970: 7070 6f72 7420 666f 7220 6164 7661 6e63  pport for advanc
-00000980: 6564 2063 6f6d 6d61 6e64 2063 6861 696e  ed command chain
-00000990: 696e 670a 2a20 5365 6c66 2d68 6f73 7465  ing.* Self-hoste
-000009a0: 6420 666f 7220 6675 6c6c 2063 6f6e 7472  d for full contr
-000009b0: 6f6c 206f 7665 7220 796f 7572 2065 6e76  ol over your env
-000009c0: 6972 6f6e 6d65 6e74 0a2a 2048 6967 686c  ironment.* Highl
-000009d0: 7920 636f 6e66 6967 7572 6162 6c65 2074  y configurable t
-000009e0: 6f20 6164 6170 7420 746f 2079 6f75 7220  o adapt to your 
-000009f0: 7072 6566 6572 656e 6365 730a 0a23 2320  preferences..## 
-00000a00: 496e 7374 616c 6c61 7469 6f6e 0a0a 496e  Installation..In
-00000a10: 7374 616c 6c69 6e67 2053 6865 6c6c 4f72  stalling ShellOr
-00000a20: 6163 6c65 2069 7320 6561 7379 210a 0a31  acle is easy!..1
-00000a30: 2e20 5069 7020 696e 7374 616c 6c20 7468  . Pip install th
-00000a40: 6520 6073 6865 6c6c 6f72 6163 6c65 6020  e `shelloracle` 
-00000a50: 7061 636b 6167 650a 2020 2020 6060 6073  package.    ```s
-00000a60: 6865 6c6c 0a20 2020 2070 7974 686f 6e33  hell.    python3
-00000a70: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
-00000a80: 7368 656c 6c6f 7261 636c 650a 2020 2020  shelloracle.    
-00000a90: 6060 600a 322e 2043 6f6e 6669 6775 7265  ```.2. Configure
-00000aa0: 2053 6865 6c6c 4f72 6163 6c65 2077 6974   ShellOracle wit
-00000ab0: 6820 6073 6865 6c6c 6f72 6163 6c65 2063  h `shelloracle c
-00000ac0: 6f6e 6669 6775 7265 6020 616e 6420 666f  onfigure` and fo
-00000ad0: 6c6c 6f77 2074 6865 2070 726f 6d70 7473  llow the prompts
-00000ae0: 0a20 2020 2060 6060 7368 656c 6c0a 2020  .    ```shell.  
-00000af0: 2020 7079 7468 6f6e 3320 2d6d 2073 6865    python3 -m she
-00000b00: 6c6c 6f72 6163 6c65 2063 6f6e 6669 6775  lloracle configu
-00000b10: 7265 0a20 2020 2060 6060 0a33 2e20 5265  re.    ```.3. Re
-00000b20: 6665 7220 746f 2074 6865 205b 7072 6f76  fer to the [prov
-00000b30: 6964 6572 735d 2823 7072 6f76 6964 6572  iders](#provider
-00000b40: 7329 2073 6563 7469 6f6e 2066 6f72 2073  s) section for s
-00000b50: 7065 6369 6669 6320 6465 7461 696c 7320  pecific details 
-00000b60: 7265 6761 7264 696e 6720 796f 7572 2063  regarding your c
-00000b70: 686f 7365 6e20 7072 6f76 6964 6572 2e0a  hosen provider..
-00000b80: 0a23 2320 5573 6167 650a 0a53 6865 6c6c  .## Usage..Shell
-00000b90: 4f72 6163 6c65 2069 7320 6465 7369 676e  Oracle is design
-00000ba0: 6564 2074 6f20 6265 2075 7365 6420 6173  ed to be used as
-00000bb0: 2061 2042 4153 482f 5a53 4820 7769 6467   a BASH/ZSH widg
-00000bc0: 6574 2061 6374 6976 6174 6564 2062 7920  et activated by 
-00000bd0: 7468 6520 4354 524c 2b46 206b 6579 626f  the CTRL+F keybo
-00000be0: 6172 6420 7368 6f72 7463 7574 2e0a 0a31  ard shortcut...1
-00000bf0: 2e20 5072 6573 7320 4354 524c 2b46 0a32  . Press CTRL+F.2
-00000c00: 2e20 4465 7363 7269 6265 2079 6f75 7220  . Describe your 
-00000c10: 636f 6d6d 616e 640a 332e 2050 7265 7373  command.3. Press
-00000c20: 2045 6e74 6572 0a0a 5468 6520 6765 6e65   Enter..The gene
-00000c30: 7261 7465 6420 636f 6d6d 616e 6420 7769  rated command wi
-00000c40: 6c6c 2062 6520 696e 7365 7274 6564 2069  ll be inserted i
-00000c50: 6e74 6f20 796f 7572 2073 6865 6c6c 2070  nto your shell p
-00000c60: 726f 6d70 7420 6166 7465 7220 6120 6272  rompt after a br
-00000c70: 6965 6620 7072 6f63 6573 7369 6e67 2070  ief processing p
-00000c80: 6572 696f 642e 0a0a 2323 2050 726f 7669  eriod...## Provi
-00000c90: 6465 7273 0a0a 2323 2320 4f6c 6c61 6d61  ders..### Ollama
-00000ca0: 0a0a 4265 666f 7265 2075 7369 6e67 2053  ..Before using S
-00000cb0: 6865 6c6c 4f72 6163 6c65 2077 6974 6820  hellOracle with 
-00000cc0: 4f6c 6c61 6d61 2c20 7075 6c6c 2074 6865  Ollama, pull the
-00000cd0: 206d 6f64 656c 2079 6f75 2063 686f 7365   model you chose
-00000ce0: 2069 6e20 7468 6520 636f 6e66 6967 7572   in the configur
-00000cf0: 6520 7374 6570 2e0a 466f 7220 6578 616d  e step..For exam
-00000d00: 706c 652c 2069 6620 796f 7520 6368 6f73  ple, if you chos
-00000d10: 6520 6063 6f64 656c 6c61 6d61 3a31 3362  e `codellama:13b
-00000d20: 602c 2072 756e 3a0a 0a60 6060 7368 656c  `, run:..```shel
-00000d30: 6c0a 6f6c 6c61 6d61 2070 756c 6c20 636f  l.ollama pull co
-00000d40: 6465 6c6c 616d 613a 3133 620a 6060 600a  dellama:13b.```.
-00000d50: 0a52 6566 6572 2074 6f20 7468 6520 5b4f  .Refer to the [O
-00000d60: 6c6c 616d 6120 646f 6373 5d28 6874 7470  llama docs](http
-00000d70: 733a 2f2f 6f6c 6c61 6d61 2e61 6929 2066  s://ollama.ai) f
-00000d80: 6f72 2069 6e73 7461 6c6c 6174 696f 6e2c  or installation,
-00000d90: 2061 7661 696c 6162 6c65 206d 6f64 656c   available model
-00000da0: 732c 2061 6e64 2075 7361 6765 2e0a 0a23  s, and usage...#
-00000db0: 2323 204f 7065 6e41 490a 0a54 6f20 7573  ## OpenAI..To us
-00000dc0: 6520 5368 656c 6c4f 7261 636c 6520 7769  e ShellOracle wi
-00000dd0: 7468 2074 6865 204f 7065 6e41 4920 7072  th the OpenAI pr
-00000de0: 6f76 6964 6572 2c20 6372 6561 7465 2061  ovider, create a
-00000df0: 6e20 5b41 5049 206b 6579 5d28 6874 7470  n [API key](http
-00000e00: 733a 2f2f 706c 6174 666f 726d 2e6f 7065  s://platform.ope
-00000e10: 6e61 692e 636f 6d2f 6163 636f 756e 742f  nai.com/account/
-00000e20: 6170 692d 6b65 7973 292e 2045 6469 740a  api-keys). Edit.
-00000e30: 796f 7572 2060 7e2f 2e73 6865 6c6c 6f72  your `~/.shellor
-00000e40: 6163 6c65 2f63 6f6e 6669 672e 746f 6d6c  acle/config.toml
-00000e50: 6020 746f 2063 6861 6e67 6520 796f 7572  ` to change your
-00000e60: 2070 726f 7669 6465 7220 616e 6420 656e   provider and en
-00000e70: 7465 7220 796f 7572 2041 5049 206b 6579  ter your API key
-00000e80: 2e0a 0a23 2323 204c 6f63 616c 4149 0a0a  ...### LocalAI..
-00000e90: 5265 6665 7220 746f 2074 6865 205b 4c6f  Refer to the [Lo
-00000ea0: 6361 6c41 4920 646f 6373 5d28 6874 7470  calAI docs](http
-00000eb0: 733a 2f2f 6c6f 6361 6c61 692e 696f 2f29  s://localai.io/)
-00000ec0: 2066 6f72 2069 6e73 7461 6c6c 6174 696f   for installatio
-00000ed0: 6e2c 2061 7661 696c 6162 6c65 206d 6f64  n, available mod
-00000ee0: 656c 732c 2061 6e64 2075 7361 6765 2e0a  els, and usage..
-00000ef0: 0a23 2323 204f 7468 6572 2077 6179 7320  .### Other ways 
-00000f00: 746f 2072 756e 2053 6865 6c6c 4f72 6163  to run ShellOrac
-00000f10: 6c65 0a0a 5368 656c 6c4f 7261 636c 6520  le..ShellOracle 
-00000f20: 6361 6e20 6265 2072 756e 2061 7320 6120  can be run as a 
-00000f30: 5079 7468 6f6e 206d 6f64 756c 6520 7769  Python module wi
-00000f40: 7468 2060 7079 7468 6f6e 3320 2d6d 2073  th `python3 -m s
-00000f50: 6865 6c6c 6f72 6163 6c65 6020 6f72 2075  helloracle` or u
-00000f60: 7369 6e67 2069 7473 2065 6e74 7279 706f  sing its entrypo
-00000f70: 696e 7420 6073 686f 7260 3b20 686f 7765  int `shor`; howe
-00000f80: 7665 722c 0a74 6865 7265 2061 7265 2061  ver,.there are a
-00000f90: 2066 6577 2063 6176 6561 7473 2077 6974   few caveats wit
-00000fa0: 6820 7468 6973 206d 6574 686f 643a 0a2d  h this method:.-
-00000fb0: 2045 6e73 7572 6520 796f 7572 2060 7e2f   Ensure your `~/
-00000fc0: 2e6c 6f63 616c 2f62 696e 6020 6469 7265  .local/bin` dire
-00000fd0: 6374 6f72 7920 6973 2061 6464 6564 2074  ctory is added t
-00000fe0: 6f20 796f 7572 2050 4154 4820 7661 7269  o your PATH vari
-00000ff0: 6162 6c65 2066 6f72 2074 6865 2065 6e74  able for the ent
-00001000: 7279 706f 696e 7420 746f 2077 6f72 6b2e  rypoint to work.
-00001010: 0a2d 2052 756e 6e69 6e67 2053 6865 6c6c  .- Running Shell
-00001020: 4f72 6163 6c65 2077 6974 6820 7468 6973  Oracle with this
-00001030: 206d 6574 686f 6420 7769 6c6c 206e 6f74   method will not
-00001040: 2061 7574 6f6d 6174 6963 616c 6c79 2069   automatically i
-00001050: 6e73 6572 7420 7468 6520 7265 7375 6c74  nsert the result
-00001060: 2069 6e74 6f20 796f 7572 2073 6865 6c6c   into your shell
-00001070: 2070 726f 6d70 742e 0a0a 2323 2320 5469   prompt...### Ti
-00001080: 7073 0a0a 312e 2049 6620 796f 7520 7072  ps..1. If you pr
-00001090: 6573 7320 4354 524c 2b46 2077 6974 6820  ess CTRL+F with 
-000010a0: 7465 7874 2069 6e20 796f 7572 205a 4c45  text in your ZLE
-000010b0: 2062 7566 6665 722c 2061 6c6c 2074 6578   buffer, all tex
-000010c0: 7420 6c65 6674 206f 6620 796f 7572 2063  t left of your c
-000010d0: 7572 736f 7220 7769 6c6c 2063 6172 7279  ursor will carry
-000010e0: 206f 7665 7220 746f 2079 6f75 7220 5368   over to your Sh
-000010f0: 656c 6c4f 7261 636c 650a 2020 2070 726f  ellOracle.   pro
-00001100: 6d70 742e 0a32 2e20 5550 5f41 5252 4f57  mpt..2. UP_ARROW
-00001110: 2061 6e64 2044 4f57 4e5f 4152 524f 5720   and DOWN_ARROW 
-00001120: 6379 636c 6520 7468 726f 7567 6820 796f  cycle through yo
-00001130: 7572 2070 726f 6d70 7420 6869 7374 6f72  ur prompt histor
-00001140: 792e 0a33 2e20 5368 656c 6c4f 7261 636c  y..3. ShellOracl
-00001150: 6520 6361 6e20 6265 2063 6861 696e 6564  e can be chained
-00001160: 2077 6974 6820 6f74 6865 7220 636f 6d6d   with other comm
-00001170: 616e 6473 3b20 7472 793a 2060 6563 686f  ands; try: `echo
-00001180: 2022 6669 6e64 2061 6c6c 2074 6865 2070   "find all the p
-00001190: 7974 686f 6e20 6669 6c65 7320 696e 206d  ython files in m
-000011a0: 7920 6377 6422 207c 2073 686f 7260 0a0a  y cwd" | shor`..
-000011b0: 2323 2043 6f6e 6669 6775 7261 7469 6f6e  ## Configuration
-000011c0: 0a0a 5368 656c 6c4f 7261 636c 6527 7320  ..ShellOracle's 
-000011d0: 636f 6e66 6967 7572 6174 696f 6e20 6973  configuration is
-000011e0: 2079 6f75 7220 6761 7465 7761 7920 746f   your gateway to
-000011f0: 2074 6169 6c6f 7269 6e67 2074 6865 2075   tailoring the u
-00001200: 7469 6c69 7479 2074 6f20 6d61 7463 6820  tility to match 
-00001210: 796f 7572 2070 7265 6665 7265 6e63 6573  your preferences
-00001220: 2061 6e64 2072 6571 7569 7265 6d65 6e74   and requirement
-00001230: 732e 0a54 6865 2060 7e2f 2e73 6865 6c6c  s..The `~/.shell
-00001240: 6f72 6163 6c65 2f63 6f6e 6669 672e 746f  oracle/config.to
-00001250: 6d6c 6020 6669 6c65 2073 6572 7665 7320  ml` file serves 
-00001260: 6173 2074 6865 2063 6f6e 7472 6f6c 2063  as the control c
-00001270: 656e 7465 7220 666f 7220 6375 7374 6f6d  enter for custom
-00001280: 697a 696e 6720 7661 7269 6f75 7320 6173  izing various as
-00001290: 7065 6374 7320 6f66 2053 6865 6c6c 4f72  pects of ShellOr
-000012a0: 6163 6c65 2773 0a62 6568 6176 696f 722e  acle's.behavior.
-000012b0: 0a0a 2323 2053 7973 7465 6d20 5265 7175  ..## System Requ
-000012c0: 6972 656d 656e 7473 0a0a 2323 2320 536f  irements..### So
-000012d0: 6674 7761 7265 0a0a 5368 656c 6c4f 7261  ftware..ShellOra
-000012e0: 636c 6520 7375 7070 6f72 7473 2042 4153  cle supports BAS
-000012f0: 4820 616e 6420 5a53 4820 6f6e 206d 6163  H and ZSH on mac
-00001300: 4f53 2061 6e64 204c 696e 7578 2e0a 0a23  OS and Linux...#
-00001310: 2323 2048 6172 6477 6172 650a 0a46 6f72  ## Hardware..For
-00001320: 2063 6c6f 7564 2070 726f 7669 6465 7273   cloud providers
-00001330: 206c 696b 6520 4f70 656e 4149 2c20 7468   like OpenAI, th
-00001340: 6572 6520 6172 6520 6e6f 2073 7065 6369  ere are no speci
-00001350: 6669 6320 7379 7374 656d 2072 6571 7569  fic system requi
-00001360: 7265 6d65 6e74 732e 0a0a 4966 2073 656c  rements...If sel
-00001370: 662d 686f 7374 696e 672c 2073 7973 7465  f-hosting, syste
-00001380: 6d20 7265 7175 6972 656d 656e 7473 2076  m requirements v
-00001390: 6172 7920 6261 7365 6420 6f6e 2074 6865  ary based on the
-000013a0: 206d 6f64 656c 2075 7365 642e 2052 6566   model used. Ref
-000013b0: 6572 2074 6f20 7468 6520 4f6c 6c61 6d61  er to the Ollama
-000013c0: 206d 6f64 656c 2072 6567 6973 7472 7920   model registry 
-000013d0: 666f 7220 6d6f 7265 0a69 6e66 6f72 6d61  for more.informa
-000013e0: 7469 6f6e 2e0a 0a23 2320 4665 6564 6261  tion...## Feedba
-000013f0: 636b 0a0a 456e 636f 756e 7465 7265 6420  ck..Encountered 
-00001400: 7072 6f62 6c65 6d73 3f20 5b46 696c 6520  problems? [File 
-00001410: 616e 2069 7373 7565 5d28 6874 7470 733a  an issue](https:
-00001420: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6a63  //github.com/djc
-00001430: 6f70 6c65 792f 5368 656c 6c4f 7261 636c  opley/ShellOracl
-00001440: 652f 6973 7375 6573 2f6e 6577 292e 2046  e/issues/new). F
-00001450: 6561 7475 7265 2072 6571 7565 7374 7320  eature requests 
-00001460: 6172 6520 7765 6c63 6f6d 652c 0a61 6e64  are welcome,.and
-00001470: 2063 6f6e 7472 6962 7574 696f 6e73 2063   contributions c
-00001480: 616e 2062 6520 6d61 6465 2062 7920 6f70  an be made by op
-00001490: 656e 696e 6720 6120 7075 6c6c 2072 6571  ening a pull req
-000014a0: 7565 7374 2e0a                           uest..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7368 656c  : 2.1.Name: shel
+00000020: 6c6f 7261 636c 650a 5665 7273 696f 6e3a  loracle.Version:
+00000030: 2031 2e33 2e30 0a53 756d 6d61 7279 3a20   1.3.0.Summary: 
+00000040: 5368 656c 6c4f 7261 636c 6520 6973 2061  ShellOracle is a
+00000050: 2070 6c75 6767 6162 6c65 2074 6572 6d69   pluggable termi
+00000060: 6e61 6c20 7574 696c 6974 7920 7468 6174  nal utility that
+00000070: 2074 616b 6573 2061 206e 6174 7572 616c   takes a natural
+00000080: 206c 616e 6775 6167 6520 6465 7363 7269   language descri
+00000090: 7074 696f 6e20 6f66 2061 2063 6f6d 6d61  ption of a comma
+000000a0: 6e64 2061 6e64 2073 7562 7374 6974 7574  nd and substitut
+000000b0: 6573 2069 7420 696e 746f 2079 6f75 7220  es it into your 
+000000c0: 7465 726d 696e 616c 2062 7566 6665 722e  terminal buffer.
+000000d0: 0a41 7574 686f 722d 656d 6169 6c3a 2044  .Author-email: D
+000000e0: 616e 6965 6c20 436f 706c 6579 203c 646a  aniel Copley <dj
+000000f0: 636f 706c 6579 4070 726f 746f 6e2e 6d65  copley@proton.me
+00000100: 3e0a 5072 6f6a 6563 742d 5552 4c3a 2048  >.Project-URL: H
+00000110: 6f6d 6570 6167 652c 2068 7474 7073 3a2f  omepage, https:/
+00000120: 2f67 6974 6875 622e 636f 6d2f 646a 636f  /github.com/djco
+00000130: 706c 6579 2f53 6865 6c6c 4f72 6163 6c65  pley/ShellOracle
+00000140: 0a50 726f 6a65 6374 2d55 524c 3a20 5265  .Project-URL: Re
+00000150: 706f 7369 746f 7279 2c20 6874 7470 733a  pository, https:
+00000160: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6a63  //github.com/djc
+00000170: 6f70 6c65 792f 5368 656c 6c4f 7261 636c  opley/ShellOracl
+00000180: 652e 6769 740a 5072 6f6a 6563 742d 5552  e.git.Project-UR
+00000190: 4c3a 2049 7373 7565 732c 2068 7474 7073  L: Issues, https
+000001a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 646a  ://github.com/dj
+000001b0: 636f 706c 6579 2f53 6865 6c6c 4f72 6163  copley/ShellOrac
+000001c0: 6c65 2f69 7373 7565 730a 436c 6173 7369  le/issues.Classi
+000001d0: 6669 6572 3a20 4465 7665 6c6f 706d 656e  fier: Developmen
+000001e0: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
+000001f0: 5072 6f64 7563 7469 6f6e 2f53 7461 626c  Production/Stabl
+00000200: 650a 436c 6173 7369 6669 6572 3a20 456e  e.Classifier: En
+00000210: 7669 726f 6e6d 656e 7420 3a3a 2043 6f6e  vironment :: Con
+00000220: 736f 6c65 0a43 6c61 7373 6966 6965 723a  sole.Classifier:
+00000230: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
+00000240: 6d20 3a3a 204d 6163 4f53 0a43 6c61 7373  m :: MacOS.Class
+00000250: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
+00000260: 2053 7973 7465 6d20 3a3a 2050 4f53 4958   System :: POSIX
+00000270: 203a 3a20 4c69 6e75 780a 436c 6173 7369   :: Linux.Classi
+00000280: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
+00000290: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
+000002a0: 6f70 6572 730a 436c 6173 7369 6669 6572  opers.Classifier
+000002b0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000002c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002d0: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
+000002e0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000002f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000300: 203a 3a20 332e 390a 436c 6173 7369 6669   :: 3.9.Classifi
+00000310: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000320: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000330: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
+00000340: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000350: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000360: 7974 686f 6e20 3a3a 2033 2e31 310a 436c  ython :: 3.11.Cl
+00000370: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000380: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000390: 3a20 5079 7468 6f6e 203a 3a20 332e 3132  : Python :: 3.12
+000003a0: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+000003b0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+000003c0: 6f76 6564 203a 3a20 474e 5520 4765 6e65  oved :: GNU Gene
+000003d0: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+000003e0: 7365 2076 3320 2847 504c 7633 290a 5265  se v3 (GPLv3).Re
+000003f0: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
+00000400: 3d33 2e39 0a44 6573 6372 6970 7469 6f6e  =3.9.Description
+00000410: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+00000420: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
+00000430: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+00000440: 5345 0a52 6571 7569 7265 732d 4469 7374  SE.Requires-Dist
+00000450: 3a20 6874 7470 780a 5265 7175 6972 6573  : httpx.Requires
+00000460: 2d44 6973 743a 206f 7065 6e61 690a 5265  -Dist: openai.Re
+00000470: 7175 6972 6573 2d44 6973 743a 2070 726f  quires-Dist: pro
+00000480: 6d70 742d 746f 6f6c 6b69 740a 5265 7175  mpt-toolkit.Requ
+00000490: 6972 6573 2d44 6973 743a 2079 6173 7069  ires-Dist: yaspi
+000004a0: 6e0a 5265 7175 6972 6573 2d44 6973 743a  n.Requires-Dist:
+000004b0: 2074 6f6d 6c6b 6974 0a52 6571 7569 7265   tomlkit.Require
+000004c0: 732d 4469 7374 3a20 746f 6d6c 693e 3d31  s-Dist: tomli>=1
+000004d0: 2e31 2e30 3b20 7079 7468 6f6e 5f76 6572  .1.0; python_ver
+000004e0: 7369 6f6e 203c 2022 332e 3131 220a 0a3c  sion < "3.11"..<
+000004f0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000500: 3e0a 2020 3c69 6d67 2073 7263 3d22 6874  >.  <img src="ht
+00000510: 7470 733a 2f2f 692e 696d 6775 722e 636f  tps://i.imgur.co
+00000520: 6d2f 4973 5159 496e 4a2e 706e 6722 2061  m/IsQYInJ.png" a
+00000530: 6c74 3d22 5368 656c 6c4f 7261 636c 6520  lt="ShellOracle 
+00000540: 6c6f 676f 222f 3e0a 3c2f 703e 0a0a 3c68  logo"/>.</p>..<h
+00000550: 3120 616c 6967 6e3d 2263 656e 7465 7222  1 align="center"
+00000560: 3e53 6865 6c6c 4f72 6163 6c65 3c2f 6831  >ShellOracle</h1
+00000570: 3e0a 0a3c 7020 616c 6967 6e3d 2263 656e  >..<p align="cen
+00000580: 7465 7222 3e0a 2020 3c61 2068 7265 663d  ter">.  <a href=
+00000590: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000005a0: 636f 6d2f 646a 636f 706c 6579 2f53 6865  com/djcopley/She
+000005b0: 6c6c 4f72 6163 6c65 2f61 6374 696f 6e73  llOracle/actions
+000005c0: 2f77 6f72 6b66 6c6f 7773 2f74 6573 7473  /workflows/tests
+000005d0: 2e79 6d6c 223e 0a20 2020 2020 203c 696d  .yml">.      <im
+000005e0: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
+000005f0: 6974 6875 622e 636f 6d2f 646a 636f 706c  ithub.com/djcopl
+00000600: 6579 2f53 6865 6c6c 4f72 6163 6c65 2f61  ey/ShellOracle/a
+00000610: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000620: 2f74 6573 7473 2e79 6d6c 2f62 6164 6765  /tests.yml/badge
+00000630: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
+00000640: 2220 616c 743d 2254 6573 7473 223e 0a20  " alt="Tests">. 
+00000650: 203c 2f61 3e0a 2020 3c61 2068 7265 663d   </a>.  <a href=
+00000660: 2268 7474 7073 3a2f 2f62 6164 6765 2e66  "https://badge.f
+00000670: 7572 792e 696f 2f70 792f 7368 656c 6c6f  ury.io/py/shello
+00000680: 7261 636c 6522 3e0a 2020 2020 2020 3c69  racle">.      <i
+00000690: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000006a0: 6261 6467 652e 6675 7279 2e69 6f2f 7079  badge.fury.io/py
+000006b0: 2f73 6865 6c6c 6f72 6163 6c65 2e73 7667  /shelloracle.svg
+000006c0: 2220 616c 743d 2250 7950 4920 7665 7273  " alt="PyPI vers
+000006d0: 696f 6e22 3e0a 2020 3c2f 613e 0a20 203c  ion">.  </a>.  <
+000006e0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000006f0: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
+00000700: 7079 7069 2f73 6865 6c6c 6f72 6163 6c65  pypi/shelloracle
+00000710: 2f22 3e0a 2020 2020 2020 3c69 6d67 2073  /">.      <img s
+00000720: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000730: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000740: 7079 7665 7273 696f 6e73 2f73 6865 6c6c  pyversions/shell
+00000750: 6f72 6163 6c65 2e73 7667 2220 616c 743d  oracle.svg" alt=
+00000760: 2250 7950 4920 5375 7070 6f72 7465 6420  "PyPI Supported 
+00000770: 5079 7468 6f6e 2056 6572 7369 6f6e 7322  Python Versions"
+00000780: 3e0a 2020 3c2f 613e 0a20 203c 6120 6872  >.  </a>.  <a hr
+00000790: 6566 3d22 6874 7470 733a 2f2f 7065 7079  ef="https://pepy
+000007a0: 2e74 6563 682f 7072 6f6a 6563 742f 7368  .tech/project/sh
+000007b0: 656c 6c6f 7261 636c 6522 3e0a 2020 2020  elloracle">.    
+000007c0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+000007d0: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
+000007e0: 7465 6368 2f62 6164 6765 2f73 6865 6c6c  tech/badge/shell
+000007f0: 6f72 6163 6c65 2220 616c 743d 2244 6f77  oracle" alt="Dow
+00000800: 6e6c 6f61 6473 223e 0a20 203c 2f61 3e0a  nloads">.  </a>.
+00000810: 3c2f 703e 0a0a 5368 656c 6c4f 7261 636c  </p>..ShellOracl
+00000820: 6520 6973 2061 6e20 696e 6e6f 7661 7469  e is an innovati
+00000830: 7665 2074 6572 6d69 6e61 6c20 7574 696c  ve terminal util
+00000840: 6974 7920 6465 7369 676e 6564 2066 6f72  ity designed for
+00000850: 2069 6e74 656c 6c69 6765 6e74 2073 6865   intelligent she
+00000860: 6c6c 2063 6f6d 6d61 6e64 2067 656e 6572  ll command gener
+00000870: 6174 696f 6e2c 2062 7269 6e67 696e 6720  ation, bringing 
+00000880: 6120 6e65 7720 6c65 7665 6c20 6f66 0a65  a new level of.e
+00000890: 6666 6963 6965 6e63 7920 746f 2079 6f75  fficiency to you
+000008a0: 7220 636f 6d6d 616e 642d 6c69 6e65 2069  r command-line i
+000008b0: 6e74 6572 6163 7469 6f6e 732e 2053 6865  nteractions. She
+000008c0: 6c6c 4f72 6163 6c65 2063 7572 7265 6e74  llOracle current
+000008d0: 6c79 2073 7570 706f 7274 7320 4f6c 6c61  ly supports Olla
+000008e0: 6d61 2c20 4c6f 6361 6c41 492c 2061 6e64  ma, LocalAI, and
+000008f0: 204f 7065 6e41 4921 0a0a 215b 5368 656c   OpenAI!..![Shel
+00000900: 6c4f 7261 636c 655d 2868 7474 7073 3a2f  lOracle](https:/
+00000910: 2f69 2e69 6d67 7572 2e63 6f6d 2f47 4a58  /i.imgur.com/GJX
+00000920: 3365 4571 2e67 6966 290a 0a53 686f 7720  3eEq.gif)..Show 
+00000930: 796f 7572 2073 7570 706f 7274 2066 6f72  your support for
+00000940: 2053 6865 6c6c 4f72 6163 6c65 2061 6e64   ShellOracle and
+00000950: 206b 6565 7020 616e 2065 7965 206f 7574   keep an eye out
+00000960: 2066 6f72 2065 7863 6974 696e 6720 6e65   for exciting ne
+00000970: 7720 6465 7665 6c6f 706d 656e 7473 2062  w developments b
+00000980: 7920 636c 6963 6b69 6e67 2074 6865 20e2  y clicking the .
+00000990: ad90 2061 6e64 2061 20f0 9f91 8021 0a0a  .. and a ....!..
+000009a0: 2323 2054 6162 6c65 206f 6620 436f 6e74  ## Table of Cont
+000009b0: 656e 7473 0a0a 2d20 5b46 6561 7475 7265  ents..- [Feature
+000009c0: 735d 2823 6665 6174 7572 6573 290a 2d20  s](#features).- 
+000009d0: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2823  [Installation](#
+000009e0: 696e 7374 616c 6c61 7469 6f6e 290a 2d20  installation).- 
+000009f0: 5b55 7361 6765 5d28 2375 7361 6765 290a  [Usage](#usage).
+00000a00: 2d20 5b50 726f 7669 6465 7273 5d28 2370  - [Providers](#p
+00000a10: 726f 7669 6465 7273 290a 2d20 5b43 6f6e  roviders).- [Con
+00000a20: 6669 6775 7261 7469 6f6e 5d28 2363 6f6e  figuration](#con
+00000a30: 6669 6775 7261 7469 6f6e 290a 2d20 5b53  figuration).- [S
+00000a40: 7973 7465 6d20 5265 7175 6972 656d 656e  ystem Requiremen
+00000a50: 7473 5d28 2373 7973 7465 6d2d 7265 7175  ts](#system-requ
+00000a60: 6972 656d 656e 7473 290a 2d20 5b46 6565  irements).- [Fee
+00000a70: 6462 6163 6b5d 2823 6665 6564 6261 636b  dback](#feedback
+00000a80: 290a 0a23 2320 4665 6174 7572 6573 0a0a  )..## Features..
+00000a90: 4b65 7920 6665 6174 7572 6573 206f 6620  Key features of 
+00000aa0: 5368 656c 6c4f 7261 636c 6520 696e 636c  ShellOracle incl
+00000ab0: 7564 653a 0a0a 2a20 5365 616d 6c65 7373  ude:..* Seamless
+00000ac0: 2073 6865 6c6c 2063 6f6d 6d61 6e64 2067   shell command g
+00000ad0: 656e 6572 6174 696f 6e20 6672 6f6d 2077  eneration from w
+00000ae0: 7269 7474 656e 2064 6573 6372 6970 7469  ritten descripti
+00000af0: 6f6e 730a 2a20 436f 6d6d 616e 6420 6869  ons.* Command hi
+00000b00: 7374 6f72 7920 666f 7220 6561 7379 2072  story for easy r
+00000b10: 6566 6572 656e 6365 0a2a 2055 6e69 7820  eference.* Unix 
+00000b20: 7069 7065 2073 7570 706f 7274 2066 6f72  pipe support for
+00000b30: 2061 6476 616e 6365 6420 636f 6d6d 616e   advanced comman
+00000b40: 6420 6368 6169 6e69 6e67 0a2a 2053 656c  d chaining.* Sel
+00000b50: 662d 686f 7374 6564 2066 6f72 2066 756c  f-hosted for ful
+00000b60: 6c20 636f 6e74 726f 6c20 6f76 6572 2079  l control over y
+00000b70: 6f75 7220 656e 7669 726f 6e6d 656e 740a  our environment.
+00000b80: 2a20 4869 6768 6c79 2063 6f6e 6669 6775  * Highly configu
+00000b90: 7261 626c 6520 746f 2061 6461 7074 2074  rable to adapt t
+00000ba0: 6f20 796f 7572 2070 7265 6665 7265 6e63  o your preferenc
+00000bb0: 6573 0a0a 2323 2049 6e73 7461 6c6c 6174  es..## Installat
+00000bc0: 696f 6e0a 0a49 6e73 7461 6c6c 696e 6720  ion..Installing 
+00000bd0: 5368 656c 6c4f 7261 636c 6520 6973 2065  ShellOracle is e
+00000be0: 6173 7921 0a0a 312e 205b 7069 7078 5d28  asy!..1. [pipx](
+00000bf0: 6874 7470 733a 2f2f 7069 7078 2e70 7970  https://pipx.pyp
+00000c00: 612e 696f 2f6c 6174 6573 742f 2920 696e  a.io/latest/) in
+00000c10: 7374 616c 6c20 7468 6520 6073 6865 6c6c  stall the `shell
+00000c20: 6f72 6163 6c65 6020 7061 636b 6167 650a  oracle` package.
+00000c30: 2020 2020 6060 6073 6865 6c6c 0a20 2020      ```shell.   
+00000c40: 2070 6970 7820 696e 7374 616c 6c20 7368   pipx install sh
+00000c50: 656c 6c6f 7261 636c 650a 2020 2020 6060  elloracle.    ``
+00000c60: 600a 322e 2043 6f6e 6669 6775 7265 2053  `.2. Configure S
+00000c70: 6865 6c6c 4f72 6163 6c65 2061 6e64 2066  hellOracle and f
+00000c80: 6f6c 6c6f 7720 7468 6520 7072 6f6d 7074  ollow the prompt
+00000c90: 730a 2020 2020 6060 6073 6865 6c6c 0a20  s.    ```shell. 
+00000ca0: 2020 2073 686f 7220 636f 6e66 6967 7572     shor configur
+00000cb0: 650a 2020 2020 6060 600a 332e 2052 6566  e.    ```.3. Ref
+00000cc0: 6572 2074 6f20 7468 6520 5b70 726f 7669  er to the [provi
+00000cd0: 6465 7273 5d28 2370 726f 7669 6465 7273  ders](#providers
+00000ce0: 2920 7365 6374 696f 6e20 666f 7220 7370  ) section for sp
+00000cf0: 6563 6966 6963 2064 6574 6169 6c73 2072  ecific details r
+00000d00: 6567 6172 6469 6e67 2079 6f75 7220 6368  egarding your ch
+00000d10: 6f73 656e 2070 726f 7669 6465 722e 0a0a  osen provider...
+00000d20: 5570 6772 6164 696e 6720 746f 2074 6865  Upgrading to the
+00000d30: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
+00000d40: 6f66 2053 6865 6c6c 4f72 6163 6c65 2069  of ShellOracle i
+00000d50: 7320 6a75 7374 2061 7320 7369 6d70 6c65  s just as simple
+00000d60: 210a 0a31 2e20 7069 7078 2075 7067 7261  !..1. pipx upgra
+00000d70: 6465 2074 6865 2060 7368 656c 6c6f 7261  de the `shellora
+00000d80: 636c 6560 2070 6163 6b61 6765 0a20 2020  cle` package.   
+00000d90: 2060 6060 7368 656c 6c0a 2020 2070 6970   ```shell.   pip
+00000da0: 7820 7570 6772 6164 6520 7368 656c 6c6f  x upgrade shello
+00000db0: 7261 636c 650a 2020 2060 6060 0a0a 2a49  racle.   ```..*I
+00000dc0: 6e73 7461 6c6c 6174 696f 6e20 7769 7468  nstallation with
+00000dd0: 2060 7069 7060 2069 7320 7375 7070 6f72   `pip` is suppor
+00000de0: 7465 642c 2068 6f77 6576 6572 2c20 6070  ted, however, `p
+00000df0: 6970 7860 2069 7320 7072 6566 6572 7265  ipx` is preferre
+00000e00: 6420 666f 7220 6974 7320 6175 746f 6d61  d for its automa
+00000e10: 7469 6320 656e 7669 726f 6e6d 656e 7420  tic environment 
+00000e20: 6973 6f6c 6174 696f 6e2e 2a0a 0a23 2320  isolation.*..## 
+00000e30: 5573 6167 650a 0a53 6865 6c6c 4f72 6163  Usage..ShellOrac
+00000e40: 6c65 2069 7320 6465 7369 676e 6564 2074  le is designed t
+00000e50: 6f20 6265 2075 7365 6420 6173 2061 2042  o be used as a B
+00000e60: 4153 482f 5a53 4820 7769 6467 6574 2061  ASH/ZSH widget a
+00000e70: 6374 6976 6174 6564 2062 7920 7468 6520  ctivated by the 
+00000e80: 4354 524c 2b46 206b 6579 626f 6172 6420  CTRL+F keyboard 
+00000e90: 7368 6f72 7463 7574 2e0a 0a31 2e20 5072  shortcut...1. Pr
+00000ea0: 6573 7320 4354 524c 2b46 0a32 2e20 4465  ess CTRL+F.2. De
+00000eb0: 7363 7269 6265 2079 6f75 7220 636f 6d6d  scribe your comm
+00000ec0: 616e 640a 332e 2050 7265 7373 2045 6e74  and.3. Press Ent
+00000ed0: 6572 0a0a 5468 6520 6765 6e65 7261 7465  er..The generate
+00000ee0: 6420 636f 6d6d 616e 6420 7769 6c6c 2062  d command will b
+00000ef0: 6520 696e 7365 7274 6564 2069 6e74 6f20  e inserted into 
+00000f00: 796f 7572 2073 6865 6c6c 2070 726f 6d70  your shell promp
+00000f10: 7420 6166 7465 7220 6120 6272 6965 6620  t after a brief 
+00000f20: 7072 6f63 6573 7369 6e67 2070 6572 696f  processing perio
+00000f30: 642e 0a0a 2323 2320 4f74 6865 7220 7761  d...### Other wa
+00000f40: 7973 2074 6f20 7275 6e20 5368 656c 6c4f  ys to run ShellO
+00000f50: 7261 636c 650a 0a53 6865 6c6c 4f72 6163  racle..ShellOrac
+00000f60: 6c65 2063 616e 2062 6520 7275 6e20 6173  le can be run as
+00000f70: 2061 2050 7974 686f 6e20 6d6f 6475 6c65   a Python module
+00000f80: 2077 6974 6820 6070 7974 686f 6e33 202d   with `python3 -
+00000f90: 6d20 7368 656c 6c6f 7261 636c 6560 206f  m shelloracle` o
+00000fa0: 7220 7573 696e 6720 6974 7320 656e 7472  r using its entr
+00000fb0: 7970 6f69 6e74 2060 7368 6f72 602c 2068  ypoint `shor`, h
+00000fc0: 6f77 6576 6572 2c0a 7275 6e6e 696e 6720  owever,.running 
+00000fd0: 5368 656c 6c4f 7261 636c 6520 7769 7468  ShellOracle with
+00000fe0: 2074 6869 7320 6d65 7468 6f64 2077 696c   this method wil
+00000ff0: 6c20 6e6f 7420 6175 746f 6d61 7469 6361  l not automatica
+00001000: 6c6c 7920 696e 7365 7274 2074 6865 2072  lly insert the r
+00001010: 6573 756c 7420 696e 746f 2079 6f75 7220  esult into your 
+00001020: 7368 656c 6c20 7072 6f6d 7074 2e0a 0a23  shell prompt...#
+00001030: 2323 2054 6970 730a 0a31 2e20 4966 2079  ## Tips..1. If y
+00001040: 6f75 2070 7265 7373 2043 5452 4c2b 4620  ou press CTRL+F 
+00001050: 7769 7468 2074 6578 7420 696e 2079 6f75  with text in you
+00001060: 7220 5a4c 4520 6275 6666 6572 2c20 616c  r ZLE buffer, al
+00001070: 6c20 7465 7874 206c 6566 7420 6f66 2079  l text left of y
+00001080: 6f75 7220 6375 7273 6f72 2077 696c 6c20  our cursor will 
+00001090: 6361 7272 7920 6f76 6572 2074 6f20 796f  carry over to yo
+000010a0: 7572 2053 6865 6c6c 4f72 6163 6c65 0a20  ur ShellOracle. 
+000010b0: 2020 7072 6f6d 7074 2e0a 322e 20e2 ac86    prompt..2. ...
+000010c0: efb8 8f20 6172 726f 7720 616e 6420 e2ac  ... arrow and ..
+000010d0: 87ef b88f 2061 7272 6f77 2063 7963 6c65  .... arrow cycle
+000010e0: 2074 6872 6f75 6768 2079 6f75 7220 7072   through your pr
+000010f0: 6f6d 7074 2068 6973 746f 7279 2e0a 332e  ompt history..3.
+00001100: 2053 6865 6c6c 4f72 6163 6c65 2063 616e   ShellOracle can
+00001110: 2062 6520 6368 6169 6e65 6420 7769 7468   be chained with
+00001120: 206f 7468 6572 2063 6f6d 6d61 6e64 733b   other commands;
+00001130: 2074 7279 3a20 6065 6368 6f20 2266 696e   try: `echo "fin
+00001140: 6420 616c 6c20 7468 6520 7079 7468 6f6e  d all the python
+00001150: 2066 696c 6573 2069 6e20 6d79 2063 7764   files in my cwd
+00001160: 2220 7c20 7368 6f72 600a 0a23 2320 5072  " | shor`..## Pr
+00001170: 6f76 6964 6572 730a 0a23 2323 204f 6c6c  oviders..### Oll
+00001180: 616d 610a 0a42 6566 6f72 6520 7573 696e  ama..Before usin
+00001190: 6720 5368 656c 6c4f 7261 636c 6520 7769  g ShellOracle wi
+000011a0: 7468 204f 6c6c 616d 612c 2070 756c 6c20  th Ollama, pull 
+000011b0: 7468 6520 6d6f 6465 6c20 796f 7520 6368  the model you ch
+000011c0: 6f73 6520 696e 2074 6865 2063 6f6e 6669  ose in the confi
+000011d0: 6775 7265 2073 7465 702e 0a46 6f72 2065  gure step..For e
+000011e0: 7861 6d70 6c65 2c20 6966 2079 6f75 2063  xample, if you c
+000011f0: 686f 7365 2060 646f 6c70 6869 6e2d 6d69  hose `dolphin-mi
+00001200: 7374 7261 6c60 2c20 7275 6e3a 0a0a 6060  stral`, run:..``
+00001210: 6073 6865 6c6c 0a6f 6c6c 616d 6120 7075  `shell.ollama pu
+00001220: 6c6c 2064 6f6c 7068 696e 2d6d 6973 7472  ll dolphin-mistr
+00001230: 616c 0a60 6060 0a0a 5265 6665 7220 746f  al.```..Refer to
+00001240: 2074 6865 205b 4f6c 6c61 6d61 2064 6f63   the [Ollama doc
+00001250: 735d 2868 7474 7073 3a2f 2f6f 6c6c 616d  s](https://ollam
+00001260: 612e 6169 2920 666f 7220 696e 7374 616c  a.ai) for instal
+00001270: 6c61 7469 6f6e 2c20 6176 6169 6c61 626c  lation, availabl
+00001280: 6520 6d6f 6465 6c73 2c20 616e 6420 7573  e models, and us
+00001290: 6167 652e 0a0a 2323 2320 4f70 656e 4149  age...### OpenAI
+000012a0: 0a0a 546f 2075 7365 2053 6865 6c6c 4f72  ..To use ShellOr
+000012b0: 6163 6c65 2077 6974 6820 7468 6520 4f70  acle with the Op
+000012c0: 656e 4149 2070 726f 7669 6465 722c 2063  enAI provider, c
+000012d0: 7265 6174 6520 616e 205b 4150 4920 6b65  reate an [API ke
+000012e0: 795d 2868 7474 7073 3a2f 2f70 6c61 7466  y](https://platf
+000012f0: 6f72 6d2e 6f70 656e 6169 2e63 6f6d 2f61  orm.openai.com/a
+00001300: 6363 6f75 6e74 2f61 7069 2d6b 6579 7329  ccount/api-keys)
+00001310: 2e20 4564 6974 0a79 6f75 7220 607e 2f2e  . Edit.your `~/.
+00001320: 7368 656c 6c6f 7261 636c 652f 636f 6e66  shelloracle/conf
+00001330: 6967 2e74 6f6d 6c60 2074 6f20 6368 616e  ig.toml` to chan
+00001340: 6765 2079 6f75 7220 7072 6f76 6964 6572  ge your provider
+00001350: 2061 6e64 2065 6e74 6572 2079 6f75 7220   and enter your 
+00001360: 4150 4920 6b65 792e 0a0a 2323 2320 4c6f  API key...### Lo
+00001370: 6361 6c41 490a 0a52 6566 6572 2074 6f20  calAI..Refer to 
+00001380: 7468 6520 5b4c 6f63 616c 4149 2064 6f63  the [LocalAI doc
+00001390: 735d 2868 7474 7073 3a2f 2f6c 6f63 616c  s](https://local
+000013a0: 6169 2e69 6f2f 2920 666f 7220 696e 7374  ai.io/) for inst
+000013b0: 616c 6c61 7469 6f6e 2c20 6176 6169 6c61  allation, availa
+000013c0: 626c 6520 6d6f 6465 6c73 2c20 616e 6420  ble models, and 
+000013d0: 7573 6167 652e 0a0a 2323 2043 6f6e 6669  usage...## Confi
+000013e0: 6775 7261 7469 6f6e 0a0a 5368 656c 6c4f  guration..ShellO
+000013f0: 7261 636c 6527 7320 636f 6e66 6967 7572  racle's configur
+00001400: 6174 696f 6e20 6973 2079 6f75 7220 6761  ation is your ga
+00001410: 7465 7761 7920 746f 2074 6169 6c6f 7269  teway to tailori
+00001420: 6e67 2074 6865 2075 7469 6c69 7479 2074  ng the utility t
+00001430: 6f20 6d61 7463 6820 796f 7572 2070 7265  o match your pre
+00001440: 6665 7265 6e63 6573 2061 6e64 2072 6571  ferences and req
+00001450: 7569 7265 6d65 6e74 732e 0a54 6865 2060  uirements..The `
+00001460: 7e2f 2e73 6865 6c6c 6f72 6163 6c65 2f63  ~/.shelloracle/c
+00001470: 6f6e 6669 672e 746f 6d6c 6020 6669 6c65  onfig.toml` file
+00001480: 2073 6572 7665 7320 6173 2074 6865 2063   serves as the c
+00001490: 6f6e 7472 6f6c 2063 656e 7465 7220 666f  ontrol center fo
+000014a0: 7220 6375 7374 6f6d 697a 696e 6720 7661  r customizing va
+000014b0: 7269 6f75 7320 6173 7065 6374 7320 6f66  rious aspects of
+000014c0: 2053 6865 6c6c 4f72 6163 6c65 2773 0a62   ShellOracle's.b
+000014d0: 6568 6176 696f 722e 0a0a 2323 2053 7973  ehavior...## Sys
+000014e0: 7465 6d20 5265 7175 6972 656d 656e 7473  tem Requirements
+000014f0: 0a0a 2323 2320 536f 6674 7761 7265 0a0a  ..### Software..
+00001500: 5368 656c 6c4f 7261 636c 6520 7375 7070  ShellOracle supp
+00001510: 6f72 7473 2042 4153 4820 616e 6420 5a53  orts BASH and ZS
+00001520: 4820 6f6e 206d 6163 4f53 2061 6e64 204c  H on macOS and L
+00001530: 696e 7578 2e0a 0a23 2323 2048 6172 6477  inux...### Hardw
+00001540: 6172 650a 0a46 6f72 2063 6c6f 7564 2070  are..For cloud p
+00001550: 726f 7669 6465 7273 206c 696b 6520 4f70  roviders like Op
+00001560: 656e 4149 2c20 7468 6572 6520 6172 6520  enAI, there are 
+00001570: 6e6f 2068 6172 6477 6172 6520 7265 7175  no hardware requ
+00001580: 6972 656d 656e 7473 2e0a 0a49 6620 7275  irements...If ru
+00001590: 6e6e 696e 6720 6c6f 6361 6c6c 792c 2072  nning locally, r
+000015a0: 6566 6572 2074 6f20 796f 7572 206d 6f64  efer to your mod
+000015b0: 656c 2066 6f72 2068 6172 6477 6172 6520  el for hardware 
+000015c0: 7265 7175 6972 656d 656e 7473 2e0a 0a23  requirements...#
+000015d0: 2320 4665 6564 6261 636b 0a0a 456e 636f  # Feedback..Enco
+000015e0: 756e 7465 7265 6420 7072 6f62 6c65 6d73  untered problems
+000015f0: 3f20 5b46 696c 6520 616e 2069 7373 7565  ? [File an issue
+00001600: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001610: 2e63 6f6d 2f64 6a63 6f70 6c65 792f 5368  .com/djcopley/Sh
+00001620: 656c 6c4f 7261 636c 652f 6973 7375 6573  ellOracle/issues
+00001630: 2f6e 6577 292e 2046 6561 7475 7265 2072  /new). Feature r
+00001640: 6571 7565 7374 7320 6172 6520 7765 6c63  equests are welc
+00001650: 6f6d 652c 0a61 6e64 2063 6f6e 7472 6962  ome,.and contrib
+00001660: 7574 696f 6e73 2063 616e 2062 6520 6d61  utions can be ma
+00001670: 6465 2062 7920 6f70 656e 696e 6720 6120  de by opening a 
+00001680: 7075 6c6c 2072 6571 7565 7374 2e0a 0a23  pull request...#
+00001690: 2320 4c69 6365 6e73 650a 0a54 6869 7320  # License..This 
+000016a0: 736f 6674 7761 7265 2069 7320 6c69 6365  software is lice
+000016b0: 6e73 6564 2075 6e64 6572 2074 6865 2047  nsed under the G
+000016c0: 504c 7633 206c 6963 656e 7365 2e0a       PLv3 license..
```

### Comparing `shelloracle-1.1.2/pyproject.toml` & `shelloracle-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.2/src/shelloracle/__main__.py` & `shelloracle-1.3.0/src/shelloracle/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,47 @@
 import argparse
+import logging
 from importlib.metadata import version
 
 from . import shelloracle
+from .config import shelloracle_home
+
+
+def configure_logging():
+    root_logger = logging.getLogger()
+    root_logger.setLevel(logging.DEBUG)
+
+    formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(name)s - %(message)s")
+    handler = logging.FileHandler(shelloracle_home / "shelloracle.log")
+    handler.setLevel(logging.DEBUG)
+    handler.setFormatter(formatter)
+
+    root_logger.addHandler(handler)
 
 
 def configure():
     # nest this import in a function to avoid expensive module loads
-    from .configure import configure_shelloracle
-    configure_shelloracle()
+    from .bootstrap import bootstrap_shelloracle
+    bootstrap_shelloracle()
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
     parser.add_argument('--version', action='version', version=f'{__package__} {version(__package__)}')
 
     subparsers = parser.add_subparsers()
     configure_subparser = subparsers.add_parser("configure", help=f"install {__package__} keybindings")
     configure_subparser.set_defaults(action=configure)
 
     return parser.parse_args()
 
 
 def main() -> None:
+    configure_logging()
+
     args = parse_args()
     if action := getattr(args, "action", None):
         action()
         exit(0)
 
     shelloracle.cli()
```

### Comparing `shelloracle-1.1.2/src/shelloracle/configure.py` & `shelloracle-1.3.0/src/shelloracle/bootstrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import tomlkit
 from prompt_toolkit import print_formatted_text, prompt
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.formatted_text import FormattedText
 from prompt_toolkit.shortcuts import confirm
 
-from .config import Configuration, data_home
+from .config import Configuration, shelloracle_home
 from .providers import Provider, Setting, list_providers, get_provider
 
 
 class UserError(Exception):
     ...
 
 
@@ -114,15 +114,15 @@
     config.add("provider", provider_table)
 
     provider_configuration_table = tomlkit.table()
     for setting, value in settings.items():
         provider_configuration_table.add(setting, value)
     provider_table.add(provider.name, provider_configuration_table)
 
-    data_home.mkdir(exist_ok=True)
+    shelloracle_home.mkdir(exist_ok=True)
     with Configuration.filepath.open("w") as config_file:
         tomlkit.dump(config, config_file)
 
 
 def install_keybindings() -> None:
     if not (shells := get_installed_shells()):
         print_warning("Cannot install keybindings: no compatible shells found. "
@@ -161,15 +161,15 @@
     user_selected_provider = prompt(f"Choose your LLM provider ({', '.join(providers)}): ", completer=completer)
     if (provider_name := case_correct_user_input(user_selected_provider, providers)) is None:
         raise UserError(f"Invalid provider: {user_selected_provider or 'no input'}")
     provider = get_provider(provider_name)
     return provider
 
 
-def configure_shelloracle() -> None:
+def bootstrap_shelloracle() -> None:
     try:
         provider = user_select_provider()
         settings = user_configure_settings(provider)
     except UserError as e:
         print_error(str(e))
         return
     except KeyboardInterrupt:
```

### Comparing `shelloracle-1.1.2/src/shelloracle/providers/__init__.py` & `shelloracle-1.3.0/src/shelloracle/providers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,18 @@
 
     def __get__(self, instance: Provider, owner: type[Provider]) -> T:
         if instance is None:
             # Accessing settings as a class attribute is not supported because it prevents
             # inspect.get_members from determining the object type
             raise AttributeError("Settings must be accessed through a provider instance.")
         config = get_config()
-        return config["provider"][owner.name][self.name]
+        try:
+            return config["provider"][owner.name][self.name]
+        except KeyError:
+            return self.default
 
 
 def _providers() -> dict[str, type[Provider]]:
     from .ollama import Ollama
     from .openai import OpenAI
     from .localai import LocalAI
     providers = {
```

### Comparing `shelloracle-1.1.2/src/shelloracle/providers/localai.py` & `shelloracle-1.3.0/src/shelloracle/providers/localai.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.2/src/shelloracle/providers/ollama.py` & `shelloracle-1.3.0/src/shelloracle/providers/ollama.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.2/src/shelloracle/providers/openai.py` & `shelloracle-1.3.0/src/shelloracle/providers/openai.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.2/src/shelloracle/shell/shelloracle.bash` & `shelloracle-1.3.0/src/shelloracle/shell/shelloracle.bash`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __shelloracle__() {
   local output
-  output=$(python3 -m shelloracle) || return
+  output=$(shor) || return
   READLINE_LINE=${output#*$'\t'}
   if [[ -z "$READLINE_POINT" ]]; then
     echo "$READLINE_LINE"
   else
     READLINE_POINT=0x7fffffff
   fi
 }
```

### Comparing `shelloracle-1.1.2/src/shelloracle/shell/shelloracle.zsh` & `shelloracle-1.3.0/src/shelloracle/shell/shelloracle.zsh`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Define the function shelloracle-widget
 shelloracle-widget() {
   # Set options and suppress any error messages
   setopt localoptions noglobsubst noposixbuiltins pipefail no_aliases 2> /dev/null
 
   # Run the shelloracle python module and store the result in the "selected" array
-  local selected=( $(SHOR_DEFAULT_PROMPT=${LBUFFER} python3 -m shelloracle) )
+  local selected=( $(SHOR_DEFAULT_PROMPT=${LBUFFER} shor) )
 
   # Get the return status of the last executed command
   local ret=$?
 
   # Reset the prompt
   zle reset-prompt
```

### Comparing `shelloracle-1.1.2/src/shelloracle/shelloracle.py` & `shelloracle-1.3.0/src/shelloracle/shelloracle.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from __future__ import annotations
 
 import asyncio
+import logging
 import os
 import sys
 from pathlib import Path
+from typing import TYPE_CHECKING
 
-from prompt_toolkit import PromptSession
+from prompt_toolkit import PromptSession, print_formatted_text
 from prompt_toolkit.application import create_app_session_from_tty
+from prompt_toolkit.formatted_text import FormattedText
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.patch_stdout import patch_stdout
 from yaspin import yaspin
+from yaspin.spinners import Spinners
 
 from .config import get_config
 from .providers import get_provider
 
+if TYPE_CHECKING:
+    from yaspin.core import Yaspin
+
+logger = logging.getLogger(__name__)
+
 
 async def prompt_user(default_prompt: str | None = None) -> str:
     # stdin doesn't exist when running as a zle widget
     with create_app_session_from_tty(), patch_stdout():
         history_file = Path.home() / ".shelloracle_history"
         prompt_session: PromptSession = PromptSession(history=FileHistory(str(history_file)))
         # Can I do this with one of the builtin methods?
@@ -31,18 +40,31 @@
 
     :raises ValueError: If the input is more than one line
     :return: The query from the stdin pipe
     """
     if os.isatty(0) or not (lines := sys.stdin.readlines()):  # Return 'None' if fd 0 is a tty (no pipe)
         return None
     if len(lines) > 1:
-        raise ValueError("Multi-line input not supported")
+        raise ValueError("Multi-line input is not supported")
+    logger.debug("using query from stdin: %s", lines)
     return lines[0].rstrip()
 
 
+def spinner() -> Yaspin:
+    """Get the correct spinner based on the user's configuration
+
+    :returns: yaspin object
+    """
+    config = get_config()
+    if not config.spinner_style:
+        return yaspin()
+    style = getattr(Spinners, config.spinner_style)
+    return yaspin(style)
+
+
 async def shelloracle() -> None:
     """ShellOracle program entrypoint
 
     If there is a query from the input pipe, it processes the query to generate a response.
     If there isn't a query from the input pipe, it prompts the user for input.
 
     Environment variables:
@@ -53,27 +75,33 @@
     """
     config = get_config()
     provider = get_provider(config.provider)()
 
     if not (prompt := get_query_from_pipe()):
         default_prompt = os.environ.get("SHOR_DEFAULT_PROMPT")
         prompt = await prompt_user(default_prompt)
+    logger.info("user prompt: %s", prompt)
 
     shell_command = ""
-    with create_app_session_from_tty(), patch_stdout(raw=True), yaspin() as sp:
+    with create_app_session_from_tty(), patch_stdout(raw=True), spinner() as sp:
         async for token in provider.generate(prompt):
             # some models may erroneously return a newline, which causes issues with the status spinner
             token = token.replace("\n", "")
             shell_command += token
             sp.text = shell_command
+    logger.info("generated shell command: %s", shell_command)
     sys.stdout.write(shell_command)
 
 
 def cli() -> None:
     """Run the ShellOracle command line interface
 
     :returns: None
     """
     try:
         asyncio.run(shelloracle())
     except (KeyboardInterrupt, asyncio.exceptions.CancelledError):
         return
+    except Exception as err:
+        logger.exception("An unhandled exception occurred")
+        with create_app_session_from_tty():
+            print_formatted_text(FormattedText([("ansired", f"\n{err}")]))
```

### Comparing `shelloracle-1.1.2/src/shelloracle.egg-info/SOURCES.txt` & `shelloracle-1.3.0/src/shelloracle.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 .gitignore
+CITATION.cff
 LICENSE
 README.md
 pyproject.toml
 tox.ini
 .github/workflows/release.yml
 .github/workflows/tests.yml
 src/shelloracle/__init__.py
 src/shelloracle/__main__.py
+src/shelloracle/bootstrap.py
 src/shelloracle/config.py
-src/shelloracle/configure.py
 src/shelloracle/shelloracle.py
 src/shelloracle.egg-info/PKG-INFO
 src/shelloracle.egg-info/SOURCES.txt
 src/shelloracle.egg-info/dependency_links.txt
 src/shelloracle.egg-info/entry_points.txt
 src/shelloracle.egg-info/requires.txt
 src/shelloracle.egg-info/top_level.txt
```

