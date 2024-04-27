# Comparing `tmp/ziya-0.1.5.tar.gz` & `tmp/ziya-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziya-0.1.5.tar", max compression
+gzip compressed data, was "ziya-0.1.6.tar", max compression
```

## Comparing `ziya-0.1.5.tar` & `ziya-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.5/LICENSE
--rw-r--r--   0        0        0     2072 2024-04-26 01:28:16.357186 ziya-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.5/app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.5/app/agents/__init__.py
--rw-r--r--   0        0        0     4349 2024-04-27 03:42:52.802293 ziya-0.1.5/app/agents/agent.py
--rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.5/app/agents/prompts.py
--rw-r--r--   0        0        0     2827 2024-04-27 19:14:13.797079 ziya-0.1.5/app/main.py
--rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.5/app/server.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.5/app/utils/__init__.py
--rw-r--r--   0        0        0     2512 2024-04-27 03:12:25.454451 ziya-0.1.5/app/utils/directory_util.py
--rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.5/app/utils/gitignore_parser.py
--rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.5/app/utils/logging_utils.py
--rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.5/app/utils/print_tree_util.py
--rw-r--r--   0        0        0      654 2024-04-27 05:58:10.286931 ziya-0.1.5/app/utils/version_util.py
--rw-r--r--   0        0        0      716 2024-04-27 19:15:08.354394 ziya-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3622 2024-04-24 04:42:38.591520 ziya-0.1.5/static/app.js
--rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.5/static/favicon.ico
--rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.5/static/sendPayload.js
--rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.5/static/ziya.css
--rw-r--r--   0        0        0      800 2024-04-23 01:33:44.760779 ziya-0.1.5/templates/index.html
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 ziya-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2072 2024-04-26 01:28:16.357186 ziya-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.6/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.6/app/agents/__init__.py
+-rw-r--r--   0        0        0     4349 2024-04-27 03:42:52.802293 ziya-0.1.6/app/agents/agent.py
+-rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.6/app/agents/prompts.py
+-rw-r--r--   0        0        0     3146 2024-04-27 20:21:37.939016 ziya-0.1.6/app/main.py
+-rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.6/app/server.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.6/app/utils/__init__.py
+-rw-r--r--   0        0        0     2512 2024-04-27 03:12:25.454451 ziya-0.1.6/app/utils/directory_util.py
+-rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.6/app/utils/gitignore_parser.py
+-rw-r--r--   0        0        0      527 2024-04-27 20:33:01.898238 ziya-0.1.6/app/utils/langchain_validation_util.py
+-rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.6/app/utils/logging_utils.py
+-rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.6/app/utils/print_tree_util.py
+-rw-r--r--   0        0        0      631 2024-04-27 19:40:53.572399 ziya-0.1.6/app/utils/version_util.py
+-rw-r--r--   0        0        0      716 2024-04-27 20:33:49.088179 ziya-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3622 2024-04-24 04:42:38.591520 ziya-0.1.6/static/app.js
+-rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.6/static/favicon.ico
+-rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.6/static/sendPayload.js
+-rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.6/static/ziya.css
+-rw-r--r--   0        0        0      800 2024-04-23 01:33:44.760779 ziya-0.1.6/templates/index.html
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 ziya-0.1.6/PKG-INFO
```

### Comparing `ziya-0.1.5/LICENSE` & `ziya-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/README.md` & `ziya-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/app/agents/agent.py` & `ziya-0.1.6/app/agents/agent.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/app/agents/prompts.py` & `ziya-0.1.6/app/agents/prompts.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/app/main.py` & `ziya-0.1.6/app/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,90 @@
+import argparse
 import os
 import subprocess
 import sys
 from typing import Optional
 
 from langchain_cli.cli import serve
-import argparse
 
 from app.utils.logging_utils import logger
+from app.utils.langchain_validation_util import validate_langchain_vars
 from app.utils.version_util import get_current_version, get_latest_version
 
 
-def update_package(current_version: str, latest_version: Optional[str]) -> None:
-    try:
-        logger.info(f"Updating ziya from {current_version} to {latest_version}")
-        subprocess.check_call([sys.executable, '-m', 'pip', 'install', '--upgrade', 'ziya'])
-        logger.info("Update completed. Next time you run ziya it will be with the latest version.")
-
-    except Exception as e:
-        logger.info(f"Unexpected error upgrading ziya: {e}")
-
-
-def main():
-    os.environ["ZIYA_USER_CODEBASE_DIR"] = os.getcwd()
-
+def parse_arguments():
     parser = argparse.ArgumentParser(description="Run with custom options")
     parser.add_argument("--exclude", default=[], type=lambda x: x.split(','),
                         help="List of files or directories to exclude (e.g., --exclude 'tst,build,*.py')")
     parser.add_argument("--include", default=[], type=lambda x: x.split(','),
                         help="List of directories to include (e.g., --include 'src,static'). Only directories for now")
     parser.add_argument("--profile", type=str, default=None,
                         help="AWS profile to use (e.g., --profile ziya)")
     parser.add_argument("--model", type=str, choices=["sonnet", "haiku", "opus"], default="sonnet",
-                        help="AWS Bedrock Model to use  (e.g., --model sonnet)")
+                        help="AWS Bedrock Model to use (e.g., --model sonnet)")
     parser.add_argument("--port", type=int, default=6969,
                         help="Port number to run Ziya frontend on (e.g., --port 8080)")
     parser.add_argument("--version", action="store_true",
                         help="Prints the version of Ziya")
-    args = parser.parse_args()
+    return parser.parse_args()
 
-    current_version = get_current_version()
-    latest_version = get_latest_version()
 
-    if args.version:
-        print(f"Ziya version {current_version}")
-        return
-
-    if latest_version and current_version != latest_version:
-        update_package(current_version, latest_version)
-    else:
-        logger.info(f"Ziya version {current_version} is up to date.")
+def setup_environment(args):
+    os.environ["ZIYA_USER_CODEBASE_DIR"] = os.getcwd()
 
-    additional_excluded_dirs = ','.join([item for item in args.exclude])
+    additional_excluded_dirs = ','.join(args.exclude)
     os.environ["ZIYA_ADDITIONAL_EXCLUDE_DIRS"] = additional_excluded_dirs
 
-    additional_included_dirs = ','.join([item for item in args.include])
+    additional_included_dirs = ','.join(args.include)
     os.environ["ZIYA_ADDITIONAL_INCLUDE_DIRS"] = additional_included_dirs
 
     if args.profile:
         os.environ["ZIYA_AWS_PROFILE"] = args.profile
     if args.model:
         os.environ["ZIYA_AWS_MODEL"] = args.model
 
-    langchain_serve_directory = os.path.dirname(os.path.abspath(__file__))
-    os.chdir(langchain_serve_directory)
+
+def check_version_and_upgrade():
+    current_version = get_current_version()
+    latest_version = get_latest_version()
+
+    if latest_version and current_version != latest_version:
+        update_package(current_version, latest_version)
+    else:
+        logger.info(f"Ziya version {current_version} is up to date.")
+
+
+def update_package(current_version: str, latest_version: Optional[str]) -> None:
+    try:
+        logger.info(f"Updating ziya from {current_version} to {latest_version}")
+        subprocess.check_call([sys.executable, '-m', 'pip', 'install', '--upgrade', 'ziya'])
+        logger.info("Update completed. Next time you run ziya it will be with the latest version.")
+
+    except Exception as e:
+        logger.info(f"Unexpected error upgrading ziya: {e}")
+
+
+def print_version():
+    current_version = get_current_version()
+    print(f"Ziya version {current_version}")
+
+
+def start_server(args):
+    os.chdir(os.path.dirname(os.path.abspath(__file__)))
     serve(port=args.port)
 
 
+def main():
+    args = parse_arguments()
+
+    if args.version:
+        print_version()
+        return
+
+    check_version_and_upgrade()
+    validate_langchain_vars()
+    setup_environment(args)
+    start_server(args)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `ziya-0.1.5/app/server.py` & `ziya-0.1.6/app/server.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/app/utils/directory_util.py` & `ziya-0.1.6/app/utils/directory_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/app/utils/gitignore_parser.py` & `ziya-0.1.6/app/utils/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/app/utils/print_tree_util.py` & `ziya-0.1.6/app/utils/print_tree_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/app/utils/version_util.py` & `ziya-0.1.6/app/utils/version_util.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,14 +10,14 @@
         response = requests.get('https://pypi.org/pypi/ziya/json')
         response.raise_for_status()
         return str(version.parse(response.json()['info']['version']))
     except requests.exceptions.RequestException:
         return None
 
 
-def update_package(package_name: str) -> None:
-    subprocess.check_call([sys.executable, '-m', 'pip', 'install', '--upgrade', package_name])
+def update_package() -> None:
+    subprocess.check_call([sys.executable, '-m', 'pip', 'install', '--upgrade', 'ziya'])
 
 
 def get_current_version() -> str:
     from importlib.metadata import version
     return str(version('ziya'))
```

### Comparing `ziya-0.1.5/pyproject.toml` & `ziya-0.1.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziya"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Vishnu Krishnaprasad <vishnukool@gmail.com>"]
 readme = "README.md"
 include = ["static/**/*", "templates/**/*", "pyproject.toml"]
 packages = [
     { include = "app" },
 ]
```

### Comparing `ziya-0.1.5/static/app.js` & `ziya-0.1.6/static/app.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/static/favicon.ico` & `ziya-0.1.6/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/static/sendPayload.js` & `ziya-0.1.6/static/sendPayload.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/static/ziya.css` & `ziya-0.1.6/static/ziya.css`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/templates/index.html` & `ziya-0.1.6/templates/index.html`

 * *Files identical despite different names*

### Comparing `ziya-0.1.5/PKG-INFO` & `ziya-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziya
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Vishnu Krishnaprasad
 Author-email: vishnukool@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

