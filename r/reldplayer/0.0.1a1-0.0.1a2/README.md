# Comparing `tmp/reldplayer-0.0.1a1.tar.gz` & `tmp/reldplayer-0.0.1a2.tar.gz`

## Comparing `reldplayer-0.0.1a1.tar` & `reldplayer-0.0.1a2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/.gitattributes
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/.python-version
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/LICENSE
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/requirements-dev.lock
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/requirements.lock
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/__main__.py
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/autogui.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/console.py
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/main.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/metaMgr.py
--rw-r--r--   0        0        0    16373 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/rawconsole.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/wndMgr.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/models/__init__.py
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/models/file.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/utils/screen.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/src/reldplayer/utils/wip.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/.gitignore
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/README.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 reldplayer-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/.gitattributes
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/.python-version
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/requirements-dev.lock
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/requirements.lock
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/__main__.py
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/autogui.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/console.py
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/main.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/metaMgr.py
+-rw-r--r--   0        0        0    16417 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/rawconsole.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/wndMgr.py
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/models/__init__.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/models/file.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/utils/screen.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/utils/wip.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/.gitignore
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/README.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/PKG-INFO
```

### Comparing `reldplayer-0.0.1a1/LICENSE` & `reldplayer-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/requirements-dev.lock` & `reldplayer-0.0.1a2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/src/reldplayer/autogui.py` & `reldplayer-0.0.1a2/src/reldplayer/autogui.py`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/src/reldplayer/console.py` & `reldplayer-0.0.1a2/src/reldplayer/console.py`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/src/reldplayer/main.py` & `reldplayer-0.0.1a2/src/reldplayer/main.py`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/src/reldplayer/metaMgr.py` & `reldplayer-0.0.1a2/src/reldplayer/metaMgr.py`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/src/reldplayer/rawconsole.py` & `reldplayer-0.0.1a2/src/reldplayer/rawconsole.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         Args:
             *args: Variable length argument list.
 
         Returns:
             None
         """
         subprocess.Popen( # noqa
-        [self.path, *args],
+        [self.path, *(str(arg) for arg in args)],
         stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
         creationflags=
             subprocess.DETACHED_PROCESS |
             subprocess.CREATE_NEW_PROCESS_GROUP | 
             subprocess.CREATE_BREAKAWAY_FROM_JOB
     )
 
@@ -60,15 +60,15 @@
         Returns:
             bytes: The output of the query execution.
         """
         try:
             if not len(args):
                 queryed = [self.path]
             else:
-                queryed = [self.path, *args]
+                queryed = [self.path, *(str(arg) for arg in args)]
 
             proc : subprocess.CompletedProcess = subprocess.run(
                 queryed,
                 capture_output=True,
                 timeout=timeout
             )
             comm : bytes = proc.stdout
```

### Comparing `reldplayer-0.0.1a1/src/reldplayer/wndMgr.py` & `reldplayer-0.0.1a2/src/reldplayer/wndMgr.py`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/src/reldplayer/models/__init__.py` & `reldplayer-0.0.1a2/src/reldplayer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/src/reldplayer/models/file.py` & `reldplayer-0.0.1a2/src/reldplayer/models/file.py`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/src/reldplayer/utils/screen.py` & `reldplayer-0.0.1a2/src/reldplayer/utils/screen.py`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/src/reldplayer/utils/wip.py` & `reldplayer-0.0.1a2/src/reldplayer/utils/wip.py`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/.gitignore` & `reldplayer-0.0.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `reldplayer-0.0.1a1/pyproject.toml` & `reldplayer-0.0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "reldplayer"
-version = "0.0.1a1"
+version = "0.0.1a2"
 description = "a reimagined pyldplayer that better suits scripting needs"
 authors = [
     { name = "ZackaryW", email = "36378555+ZackaryW@users.noreply.github.com" }
 ]
 dependencies = [
     
 ]
```

### Comparing `reldplayer-0.0.1a1/PKG-INFO` & `reldplayer-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: reldplayer
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: a reimagined pyldplayer that better suits scripting needs
 Author-email: ZackaryW <36378555+ZackaryW@users.noreply.github.com>
 Requires-Python: >=3.8
 Provides-Extra: all
 Requires-Dist: psutil>=5.8.0; extra == 'all'
 Requires-Dist: pyautogui>=0.9.54; extra == 'all'
 Requires-Dist: pydantic>=2.6.4; extra == 'all'
```

