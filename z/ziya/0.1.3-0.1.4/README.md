# Comparing `tmp/ziya-0.1.3.tar.gz` & `tmp/ziya-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziya-0.1.3.tar", max compression
+gzip compressed data, was "ziya-0.1.4.tar", max compression
```

## Comparing `ziya-0.1.3.tar` & `ziya-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.3/LICENSE
--rw-r--r--   0        0        0     2072 2024-04-26 01:28:16.357186 ziya-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.3/app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.3/app/agents/__init__.py
--rw-r--r--   0        0        0     4266 2024-04-24 04:42:40.748800 ziya-0.1.3/app/agents/agent.py
--rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.3/app/agents/prompts.py
--rw-r--r--   0        0        0     1704 2024-04-26 01:28:16.352143 ziya-0.1.3/app/main.py
--rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.3/app/server.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.3/app/utils/__init__.py
--rw-r--r--   0        0        0     2278 2024-04-24 04:42:40.749189 ziya-0.1.3/app/utils/directory_util.py
--rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.3/app/utils/gitignore_parser.py
--rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.3/app/utils/logging_utils.py
--rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.3/app/utils/print_tree_util.py
--rw-r--r--   0        0        0      716 2024-04-26 01:28:16.352353 ziya-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3622 2024-04-24 04:42:38.591520 ziya-0.1.3/static/app.js
--rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.3/static/favicon.ico
--rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.3/static/sendPayload.js
--rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.3/static/ziya.css
--rw-r--r--   0        0        0      800 2024-04-23 01:33:44.760779 ziya-0.1.3/templates/index.html
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 ziya-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2072 2024-04-26 01:28:16.357186 ziya-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.4/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.4/app/agents/__init__.py
+-rw-r--r--   0        0        0     4349 2024-04-27 03:42:52.802293 ziya-0.1.4/app/agents/agent.py
+-rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.4/app/agents/prompts.py
+-rw-r--r--   0        0        0     1705 2024-04-27 04:11:07.716382 ziya-0.1.4/app/main.py
+-rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.4/app/server.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.4/app/utils/__init__.py
+-rw-r--r--   0        0        0     2512 2024-04-27 03:12:25.454451 ziya-0.1.4/app/utils/directory_util.py
+-rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.4/app/utils/gitignore_parser.py
+-rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.4/app/utils/logging_utils.py
+-rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.4/app/utils/print_tree_util.py
+-rw-r--r--   0        0        0      716 2024-04-27 04:14:00.391091 ziya-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3622 2024-04-24 04:42:38.591520 ziya-0.1.4/static/app.js
+-rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.4/static/favicon.ico
+-rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.4/static/sendPayload.js
+-rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.4/static/ziya.css
+-rw-r--r--   0        0        0      800 2024-04-23 01:33:44.760779 ziya-0.1.4/templates/index.html
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 ziya-0.1.4/PKG-INFO
```

### Comparing `ziya-0.1.3/LICENSE` & `ziya-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ziya-0.1.3/README.md` & `ziya-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ziya-0.1.3/app/agents/agent.py` & `ziya-0.1.4/app/agents/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import botocore
+
 from typing import Generator, List, Tuple, Set, Union
 
 import tiktoken
 from langchain.agents import AgentExecutor
 from langchain.agents.format_scratchpad import format_xml
 from langchain_aws import ChatBedrock
 from langchain_community.document_loaders import TextLoader
@@ -34,14 +36,17 @@
 }[os.environ.get("ZIYA_AWS_MODEL", "haiku")]
 logger.info(f"Using Claude Model: {model_id}")
 
 model = ChatBedrock(
     model_id=model_id,
     model_kwargs={"max_tokens": 4096},
     credentials_profile_name=aws_profile if aws_profile else None,
+    config=botocore.config.Config(
+        read_timeout=900
+    )
 )
 
 
 def get_combined_document_contents() -> str:
     user_codebase_dir: str = os.environ["ZIYA_USER_CODEBASE_DIR"]
     print(f"Reading user's current codebase: {user_codebase_dir}")
```

### Comparing `ziya-0.1.3/app/agents/prompts.py` & `ziya-0.1.4/app/agents/prompts.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.3/app/main.py` & `ziya-0.1.4/app/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     parser = argparse.ArgumentParser(description="Run with custom options")
     parser.add_argument("--exclude", default=[], type=lambda x: x.split(','),
                         help="List of files or directories to exclude (e.g., --exclude 'tst,build,*.py')")
     parser.add_argument("--include", default=[], type=lambda x: x.split(','),
                         help="List of directories to include (e.g., --include 'src,static'). Only directories for now")
     parser.add_argument("--profile", type=str, default=None,
                         help="AWS profile to use (e.g., --profile ziya)")
-    parser.add_argument("--model", type=str, choices=["sonnet", "haiku", "opus"], default="haiku",
+    parser.add_argument("--model", type=str, choices=["sonnet", "haiku", "opus"], default="sonnet",
                         help="AWS Bedrock Model to use  (e.g., --model sonnet)")
     parser.add_argument("--port", type=int, default=6969,
                         help="Port number to run Ziya frontend on (e.g., --port 8080)")
     args = parser.parse_args()
 
     additional_excluded_dirs = ','.join([item for item in args.exclude])
     os.environ["ZIYA_ADDITIONAL_EXCLUDE_DIRS"] = additional_excluded_dirs
```

### Comparing `ziya-0.1.3/app/server.py` & `ziya-0.1.4/app/server.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.3/app/utils/directory_util.py` & `ziya-0.1.4/app/utils/directory_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,11 +47,15 @@
     for pattern in included_relative_dirs:
         for root, dirs, files in os.walk(os.path.normpath(os.path.join(user_codebase_dir, pattern))):
             # Filter out ignored directories
             dirs[:] = [d for d in dirs if not should_ignore(os.path.join(root, d))]
 
             for file in files:
                 file_path = os.path.join(root, file)
-                if not should_ignore(file_path):
+                if not should_ignore(file_path) and not is_image_file(file_path):
                     file_set.add(file_path)
 
     return list(file_set)
+
+def is_image_file(file_path: str) -> bool:
+    image_extensions = ['.jpg', '.jpeg', '.png', '.gif', '.bmp', '.svg', '.ico']
+    return any(file_path.lower().endswith(ext) for ext in image_extensions)
```

### Comparing `ziya-0.1.3/app/utils/gitignore_parser.py` & `ziya-0.1.4/app/utils/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.3/app/utils/print_tree_util.py` & `ziya-0.1.4/app/utils/print_tree_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.3/pyproject.toml` & `ziya-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziya"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Vishnu Krishnaprasad <vishnukool@gmail.com>"]
 readme = "README.md"
 include = ["static/**/*", "templates/**/*", "pyproject.toml"]
 packages = [
     { include = "app" },
 ]
```

### Comparing `ziya-0.1.3/static/app.js` & `ziya-0.1.4/static/app.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.3/static/favicon.ico` & `ziya-0.1.4/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ziya-0.1.3/static/sendPayload.js` & `ziya-0.1.4/static/sendPayload.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.3/static/ziya.css` & `ziya-0.1.4/static/ziya.css`

 * *Files identical despite different names*

### Comparing `ziya-0.1.3/templates/index.html` & `ziya-0.1.4/templates/index.html`

 * *Files identical despite different names*

### Comparing `ziya-0.1.3/PKG-INFO` & `ziya-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziya
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Vishnu Krishnaprasad
 Author-email: vishnukool@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

