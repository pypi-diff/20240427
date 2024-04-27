# Comparing `tmp/fluxional-0.1.1.tar.gz` & `tmp/fluxional-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxional-0.1.1.tar", max compression
+gzip compressed data, was "fluxional-0.1.2.tar", max compression
```

## Comparing `fluxional-0.1.1.tar` & `fluxional-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,33 @@
--rw-r--r--   0        0        0     1066 2023-05-20 20:13:00.439100 fluxional-0.1.1/LICENSE
--rw-r--r--   0        0        0       16 2023-05-20 20:13:00.439100 fluxional-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-22 19:43:11.884726 fluxional-0.1.1/fluxional/__init__.py
--rw-r--r--   0        0        0      725 2023-05-22 20:17:30.415171 fluxional-0.1.1/fluxional/__main__.py
--rw-r--r--   0        0        0       76 2023-05-22 02:41:03.723563 fluxional-0.1.1/fluxional/configs.py
--rw-r--r--   0        0        0      466 2023-05-22 23:11:34.996269 fluxional-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      488 1970-01-01 00:00:00.000000 fluxional-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-02-02 01:48:46.163715 fluxional-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3464 2024-04-22 20:27:58.523354 fluxional-0.1.2/README.md
+-rw-r--r--   0        0        0      398 2024-04-06 03:52:15.283626 fluxional-0.1.2/fluxional/__init__.py
+-rw-r--r--   0        0        0       85 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/__main__.py
+-rw-r--r--   0        0        0     1429 2024-04-03 20:50:44.146193 fluxional-0.1.2/fluxional/cli/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-06 03:52:08.843621 fluxional-0.1.2/fluxional/core/__init__.py
+-rw-r--r--   0        0        0    21257 2024-04-09 17:46:38.063914 fluxional-0.1.2/fluxional/core/app.py
+-rw-r--r--   0        0        0     6976 2024-04-08 20:56:52.652758 fluxional-0.1.2/fluxional/core/core.py
+-rw-r--r--   0        0        0     2927 2024-04-05 19:49:43.040843 fluxional-0.1.2/fluxional/core/events.py
+-rw-r--r--   0        0        0    11708 2024-04-08 20:56:56.662776 fluxional-0.1.2/fluxional/core/handlers.py
+-rw-r--r--   0        0        0        1 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/core/infrastructure/__init__.py
+-rw-r--r--   0        0        0    19616 2024-04-07 16:13:07.372714 fluxional-0.1.2/fluxional/core/infrastructure/base.py
+-rw-r--r--   0        0        0     7603 2024-04-07 16:07:21.912790 fluxional-0.1.2/fluxional/core/infrastructure/cdk.py
+-rw-r--r--   0        0        0     9506 2024-04-07 16:08:36.732773 fluxional-0.1.2/fluxional/core/infrastructure/resources.py
+-rw-r--r--   0        0        0      816 2024-04-07 16:02:37.282853 fluxional-0.1.2/fluxional/core/infrastructure/types.py
+-rw-r--r--   0        0        0     5818 2024-04-08 20:56:58.162781 fluxional-0.1.2/fluxional/core/logic.py
+-rw-r--r--   0        0        0     8343 2024-04-09 17:45:40.573927 fluxional-0.1.2/fluxional/core/settings.py
+-rw-r--r--   0        0        0     4045 2024-04-08 20:57:01.432779 fluxional-0.1.2/fluxional/core/tools.py
+-rw-r--r--   0        0        0     5158 2024-04-06 03:51:27.790814 fluxional-0.1.2/fluxional/core/types.py
+-rw-r--r--   0        0        0       74 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/deployment/__init__.py
+-rw-r--r--   0        0        0     1164 2024-02-02 02:20:07.747714 fluxional-0.1.2/fluxional/deployment/constants.py
+-rw-r--r--   0        0        0    15256 2024-04-03 23:29:19.551745 fluxional-0.1.2/fluxional/deployment/engine.py
+-rw-r--r--   0        0        0      345 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/deployment/exceptions.py
+-rw-r--r--   0        0        0        1 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/deployment/utils.py
+-rw-r--r--   0        0        0     3652 2024-04-05 19:50:15.280830 fluxional-0.1.2/fluxional/dev/__init__.py
+-rw-r--r--   0        0        0     3003 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/dev/client.py
+-rw-r--r--   0        0        0     3350 2024-04-03 20:50:44.146193 fluxional-0.1.2/fluxional/dev/runner.py
+-rw-r--r--   0        0        0      326 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/py.typed
+-rw-r--r--   0        0        0      461 2024-04-03 20:50:44.146193 fluxional-0.1.2/fluxional/types.py
+-rw-r--r--   0        0        0      935 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/utils.py
+-rw-r--r--   0        0        0     1151 2024-04-27 18:14:08.821086 fluxional-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4416 1970-01-01 00:00:00.000000 fluxional-0.1.2/PKG-INFO
```

### Comparing `fluxional-0.1.1/LICENSE` & `fluxional-0.1.2/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 fluxbuild
+Copyright (c) 2023 tj
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

