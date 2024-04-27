# Comparing `tmp/ziya-0.1.4.tar.gz` & `tmp/ziya-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziya-0.1.4.tar", max compression
+gzip compressed data, was "ziya-0.1.5.tar", max compression
```

## Comparing `ziya-0.1.4.tar` & `ziya-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.4/LICENSE
--rw-r--r--   0        0        0     2072 2024-04-26 01:28:16.357186 ziya-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.4/app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.4/app/agents/__init__.py
--rw-r--r--   0        0        0     4349 2024-04-27 03:42:52.802293 ziya-0.1.4/app/agents/agent.py
--rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.4/app/agents/prompts.py
--rw-r--r--   0        0        0     1705 2024-04-27 04:11:07.716382 ziya-0.1.4/app/main.py
--rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.4/app/server.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.4/app/utils/__init__.py
--rw-r--r--   0        0        0     2512 2024-04-27 03:12:25.454451 ziya-0.1.4/app/utils/directory_util.py
--rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.4/app/utils/gitignore_parser.py
--rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.4/app/utils/logging_utils.py
--rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.4/app/utils/print_tree_util.py
--rw-r--r--   0        0        0      716 2024-04-27 04:14:00.391091 ziya-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3622 2024-04-24 04:42:38.591520 ziya-0.1.4/static/app.js
--rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.4/static/favicon.ico
--rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.4/static/sendPayload.js
--rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.4/static/ziya.css
--rw-r--r--   0        0        0      800 2024-04-23 01:33:44.760779 ziya-0.1.4/templates/index.html
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 ziya-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2072 2024-04-26 01:28:16.357186 ziya-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.5/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.5/app/agents/__init__.py
+-rw-r--r--   0        0        0     4349 2024-04-27 03:42:52.802293 ziya-0.1.5/app/agents/agent.py
+-rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.5/app/agents/prompts.py
+-rw-r--r--   0        0        0     2827 2024-04-27 19:14:13.797079 ziya-0.1.5/app/main.py
+-rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.5/app/server.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.5/app/utils/__init__.py
+-rw-r--r--   0        0        0     2512 2024-04-27 03:12:25.454451 ziya-0.1.5/app/utils/directory_util.py
+-rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.5/app/utils/gitignore_parser.py
+-rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.5/app/utils/logging_utils.py
+-rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.5/app/utils/print_tree_util.py
+-rw-r--r--   0        0        0      654 2024-04-27 05:58:10.286931 ziya-0.1.5/app/utils/version_util.py
+-rw-r--r--   0        0        0      716 2024-04-27 19:15:08.354394 ziya-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3622 2024-04-24 04:42:38.591520 ziya-0.1.5/static/app.js
+-rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.5/static/favicon.ico
+-rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.5/static/sendPayload.js
+-rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.5/static/ziya.css
+-rw-r--r--   0        0        0      800 2024-04-23 01:33:44.760779 ziya-0.1.5/templates/index.html
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 ziya-0.1.5/PKG-INFO
```

### Comparing `ziya-0.1.4/LICENSE` & `ziya-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/README.md` & `ziya-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/app/agents/agent.py` & `ziya-0.1.5/app/agents/agent.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/app/agents/prompts.py` & `ziya-0.1.5/app/agents/prompts.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/app/server.py` & `ziya-0.1.5/app/server.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/app/utils/directory_util.py` & `ziya-0.1.5/app/utils/directory_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/app/utils/gitignore_parser.py` & `ziya-0.1.5/app/utils/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/app/utils/print_tree_util.py` & `ziya-0.1.5/app/utils/print_tree_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/pyproject.toml` & `ziya-0.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziya"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Vishnu Krishnaprasad <vishnukool@gmail.com>"]
 readme = "README.md"
 include = ["static/**/*", "templates/**/*", "pyproject.toml"]
 packages = [
     { include = "app" },
 ]
```

### Comparing `ziya-0.1.4/static/app.js` & `ziya-0.1.5/static/app.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/static/favicon.ico` & `ziya-0.1.5/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/static/sendPayload.js` & `ziya-0.1.5/static/sendPayload.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/static/ziya.css` & `ziya-0.1.5/static/ziya.css`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/templates/index.html` & `ziya-0.1.5/templates/index.html`

 * *Files identical despite different names*

### Comparing `ziya-0.1.4/PKG-INFO` & `ziya-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziya
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Vishnu Krishnaprasad
 Author-email: vishnukool@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

