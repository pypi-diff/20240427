# Comparing `tmp/cheeselog-1.0.0.tar.gz` & `tmp/cheeselog-1.0.1.tar.gz`

## Comparing `cheeselog-1.0.0.tar` & `cheeselog-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cheeselog-1.0.0/CheeseLog/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 cheeselog-1.0.0/CheeseLog/level.py
--rw-r--r--   0        0        0     9882 2020-02-02 00:00:00.000000 cheeselog-1.0.0/CheeseLog/logger.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 cheeselog-1.0.0/CheeseLog/progressBar.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cheeselog-1.0.0/CheeseLog/style.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cheeselog-1.0.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeselog-1.0.0/LICENSE
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 cheeselog-1.0.0/README.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cheeselog-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 cheeselog-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cheeselog-1.0.1/CheeseLog/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 cheeselog-1.0.1/CheeseLog/level.py
+-rw-r--r--   0        0        0    15397 2020-02-02 00:00:00.000000 cheeselog-1.0.1/CheeseLog/logger.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 cheeselog-1.0.1/CheeseLog/progressBar.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cheeselog-1.0.1/CheeseLog/style.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cheeselog-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeselog-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 cheeselog-1.0.1/README.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cheeselog-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 cheeselog-1.0.1/PKG-INFO
```

### Comparing `cheeselog-1.0.0/CheeseLog/style.py` & `cheeselog-1.0.1/CheeseLog/style.py`

 * *Files identical despite different names*

### Comparing `cheeselog-1.0.0/LICENSE` & `cheeselog-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeselog-1.0.0/README.md` & `cheeselog-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cheeselog-1.0.0/pyproject.toml` & `cheeselog-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseLog"
-version = "1.0.0"
+version = "1.0.1"
 description = "日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'log', 'logger' ]
```

### Comparing `cheeselog-1.0.0/PKG-INFO` & `cheeselog-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseLog
-Version: 1.0.0
+Version: 1.0.1
 Summary: 日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseLog
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: log,logger
 Requires-Dist: setproctitle
 Description-Content-Type: text/markdown
```

