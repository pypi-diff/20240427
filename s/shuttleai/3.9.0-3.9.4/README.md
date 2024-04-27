# Comparing `tmp/shuttleai-3.9.0.tar.gz` & `tmp/shuttleai-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.9.0.tar", last modified: Sat Apr 13 20:33:18 2024, max compression
+gzip compressed data, was "shuttleai-3.9.4.tar", last modified: Sat Apr 27 00:34:09 2024, max compression
```

## Comparing `shuttleai-3.9.0.tar` & `shuttleai-3.9.4.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 20:33:18.571834 shuttleai-3.9.0/
--rw-rw-rw-   0        0        0     4116 2024-04-13 20:33:18.568831 shuttleai-3.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.9.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-13 20:33:18.572840 shuttleai-3.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1274 2024-04-13 20:32:36.000000 shuttleai-3.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 20:33:18.540833 shuttleai-3.9.0/shuttleai/
--rw-rw-rw-   0        0        0      586 2024-04-06 16:43:12.000000 shuttleai-3.9.0/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.9.0/shuttleai/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-13 20:33:18.560840 shuttleai-3.9.0/shuttleai/client/
--rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.9.0/shuttleai/client/__init__.py
--rw-rw-rw-   0        0        0    17395 2024-04-13 20:32:43.000000 shuttleai-3.9.0/shuttleai/client/_async.py
--rw-rw-rw-   0        0        0    15216 2024-04-06 16:44:27.000000 shuttleai-3.9.0/shuttleai/client/_sync.py
--rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.9.0/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-04-13 20:33:18.565834 shuttleai-3.9.0/shuttleai/schemas/
--rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.9.0/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     4108 2024-04-05 22:32:01.000000 shuttleai-3.9.0/shuttleai/schemas/schemas.py
-drwxrwxrwx   0        0        0        0 2024-04-13 20:33:18.566831 shuttleai-3.9.0/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     4116 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 00:34:09.752102 shuttleai-3.9.4/
+-rw-rw-rw-   0        0        0     4116 2024-04-27 00:34:09.750100 shuttleai-3.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.9.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 00:34:09.753102 shuttleai-3.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1274 2024-04-27 00:33:14.000000 shuttleai-3.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:34:09.706102 shuttleai-3.9.4/shuttleai/
+-rw-rw-rw-   0        0        0     1781 2024-04-27 00:33:36.000000 shuttleai-3.9.4/shuttleai/__init__.py
+-rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.9.4/shuttleai/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:34:09.739102 shuttleai-3.9.4/shuttleai/client/
+-rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.9.4/shuttleai/client/__init__.py
+-rw-rw-rw-   0        0        0    17395 2024-04-24 02:47:04.000000 shuttleai-3.9.4/shuttleai/client/_async.py
+-rw-rw-rw-   0        0        0    15217 2024-04-24 02:47:06.000000 shuttleai-3.9.4/shuttleai/client/_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:34:09.742103 shuttleai-3.9.4/shuttleai/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-27 00:24:28.000000 shuttleai-3.9.4/shuttleai/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2726 2024-04-27 00:26:00.000000 shuttleai-3.9.4/shuttleai/helpers/tool_calls.py
+-rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.9.4/shuttleai/log.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:34:09.745103 shuttleai-3.9.4/shuttleai/schemas/
+-rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.9.4/shuttleai/schemas/__init__.py
+-rw-rw-rw-   0        0        0     4108 2024-04-05 22:32:01.000000 shuttleai-3.9.4/shuttleai/schemas/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:34:09.748104 shuttleai-3.9.4/shuttleai.egg-info/
+-rw-rw-rw-   0        0        0     4116 2024-04-27 00:34:09.000000 shuttleai-3.9.4/shuttleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2024-04-27 00:34:09.000000 shuttleai-3.9.4/shuttleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 00:34:09.000000 shuttleai-3.9.4/shuttleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-27 00:34:09.000000 shuttleai-3.9.4/shuttleai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       63 2024-04-27 00:34:09.000000 shuttleai-3.9.4/shuttleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-27 00:34:09.000000 shuttleai-3.9.4/shuttleai.egg-info/top_level.txt
```

### Comparing `shuttleai-3.9.0/PKG-INFO` & `shuttleai-3.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.9.0
+Version: 3.9.4
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shuttleai-3.9.0/README.md` & `shuttleai-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `shuttleai-3.9.0/setup.py` & `shuttleai-3.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
 setup(
     include_package_data=True,
     name='shuttleai', 
-    version='3.9.0',
+    version='3.9.4',
     author='shuttle',
     author_email='noreply@shuttleai.app',
     description="Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai",
     long_description_content_type='text/markdown',
     long_description=long_description,
     packages=find_packages(),
     classifiers=[
```

### Comparing `shuttleai-3.9.0/shuttleai/cli.py` & `shuttleai-3.9.4/shuttleai/cli.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.9.0/shuttleai/client/_async.py` & `shuttleai-3.9.4/shuttleai/client/_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 @Author: ShuttleAI
-@Date: 4-13-2024
+@Date: 4-23-2024
 """
 from __future__ import annotations
 from typing import (
     List,
     Dict,
     Any,
     Union,
```

### Comparing `shuttleai-3.9.0/shuttleai/client/_sync.py` & `shuttleai-3.9.4/shuttleai/client/_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 @Author: ShuttleAI
-@Date: 4-6-2024
+@Date: 4-23-2024
 """
 from typing import Any, Dict, List, Union, Optional, TYPE_CHECKING, Generator
 if TYPE_CHECKING:
     from httpx import Response
 
 from ..log import log
 from ..schemas import Chat, ChatChunk, Image, Audio, Embedding, Models, ShuttleError, Model
```

### Comparing `shuttleai-3.9.0/shuttleai/log.py` & `shuttleai-3.9.4/shuttleai/log.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.9.0/shuttleai/schemas/schemas.py` & `shuttleai-3.9.4/shuttleai/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.9.0/shuttleai.egg-info/PKG-INFO` & `shuttleai-3.9.4/shuttleai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.9.0
+Version: 3.9.4
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

