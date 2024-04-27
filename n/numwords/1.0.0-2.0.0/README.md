# Comparing `tmp/numwords-1.0.0.tar.gz` & `tmp/numwords-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numwords-1.0.0.tar", last modified: Wed Sep 22 08:03:04 2021, max compression
+gzip compressed data, was "numwords-2.0.0.tar", last modified: Sat Apr 27 15:00:24 2024, max compression
```

## Comparing `numwords-1.0.0.tar` & `numwords-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 ankurgoswami   (501) staff       (20)        0 2021-09-22 08:03:04.734022 numwords-1.0.0/
--rw-r--r--   0 ankurgoswami   (501) staff       (20)     1078 2021-09-21 17:57:57.000000 numwords-1.0.0/LICENSE
--rw-r--r--   0 ankurgoswami   (501) staff       (20)      726 2021-09-22 08:03:04.733773 numwords-1.0.0/PKG-INFO
--rw-r--r--   0 ankurgoswami   (501) staff       (20)      266 2021-09-22 08:00:04.000000 numwords-1.0.0/README.md
-drwxr-xr-x   0 ankurgoswami   (501) staff       (20)        0 2021-09-22 08:03:04.731989 numwords-1.0.0/numwords/
--rw-r--r--   0 ankurgoswami   (501) staff       (20)       26 2021-09-22 07:43:22.000000 numwords-1.0.0/numwords/__init__.py
--rw-r--r--   0 ankurgoswami   (501) staff       (20)     2597 2021-09-22 07:43:08.000000 numwords-1.0.0/numwords/core.py
-drwxr-xr-x   0 ankurgoswami   (501) staff       (20)        0 2021-09-22 08:03:04.733436 numwords-1.0.0/numwords.egg-info/
--rw-r--r--   0 ankurgoswami   (501) staff       (20)      726 2021-09-22 08:03:04.000000 numwords-1.0.0/numwords.egg-info/PKG-INFO
--rw-r--r--   0 ankurgoswami   (501) staff       (20)      223 2021-09-22 08:03:04.000000 numwords-1.0.0/numwords.egg-info/SOURCES.txt
--rw-r--r--   0 ankurgoswami   (501) staff       (20)        1 2021-09-22 08:03:04.000000 numwords-1.0.0/numwords.egg-info/dependency_links.txt
--rw-r--r--   0 ankurgoswami   (501) staff       (20)        7 2021-09-22 08:03:04.000000 numwords-1.0.0/numwords.egg-info/requires.txt
--rw-r--r--   0 ankurgoswami   (501) staff       (20)        9 2021-09-22 08:03:04.000000 numwords-1.0.0/numwords.egg-info/top_level.txt
--rw-r--r--   0 ankurgoswami   (501) staff       (20)       38 2021-09-22 08:03:04.734107 numwords-1.0.0/setup.cfg
--rw-r--r--   0 ankurgoswami   (501) staff       (20)      686 2021-09-22 08:02:43.000000 numwords-1.0.0/setup.py
+drwxrwxrwx   0 ankur     (1000) ankur     (1000)        0 2024-04-27 15:00:24.192368 numwords-2.0.0/
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)     1099 2024-04-27 11:08:09.000000 numwords-2.0.0/LICENSE
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)     1380 2024-04-27 15:00:24.180686 numwords-2.0.0/PKG-INFO
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)      975 2024-04-27 14:59:50.000000 numwords-2.0.0/README.md
+drwxrwxrwx   0 ankur     (1000) ankur     (1000)        0 2024-04-27 15:00:24.032359 numwords-2.0.0/numwords/
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)       51 2024-04-27 14:59:50.000000 numwords-2.0.0/numwords/__init__.py
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)     3552 2024-04-27 14:59:50.000000 numwords-2.0.0/numwords/core.py
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)     1154 2024-04-27 14:59:50.000000 numwords-2.0.0/numwords/mappings.py
+drwxrwxrwx   0 ankur     (1000) ankur     (1000)        0 2024-04-27 15:00:24.169332 numwords-2.0.0/numwords.egg-info/
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)     1380 2024-04-27 15:00:23.000000 numwords-2.0.0/numwords.egg-info/PKG-INFO
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)      244 2024-04-27 15:00:23.000000 numwords-2.0.0/numwords.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)        1 2024-04-27 15:00:23.000000 numwords-2.0.0/numwords.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)        7 2024-04-27 15:00:23.000000 numwords-2.0.0/numwords.egg-info/requires.txt
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)        9 2024-04-27 15:00:23.000000 numwords-2.0.0/numwords.egg-info/top_level.txt
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)       38 2024-04-27 15:00:24.193674 numwords-2.0.0/setup.cfg
+-rwxrwxrwx   0 ankur     (1000) ankur     (1000)      711 2024-04-27 14:59:50.000000 numwords-2.0.0/setup.py
```

### Comparing `numwords-1.0.0/LICENSE` & `numwords-2.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 अंkur गोswami
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019 अंkur गोswami
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

