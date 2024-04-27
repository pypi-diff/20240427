# Comparing `tmp/fastask-0.4.6.tar.gz` & `tmp/fastask-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastask-0.4.6.tar", last modified: Mon Mar 18 05:31:00 2024, max compression
+gzip compressed data, was "fastask-0.4.7.tar", last modified: Sat Apr 27 04:25:55 2024, max compression
```

## Comparing `fastask-0.4.6.tar` & `fastask-0.4.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bmachado   (501) staff       (20)        0 2024-03-18 05:31:00.121857 fastask-0.4.6/
--rw-r--r--   0 bmachado   (501) staff       (20)     1070 2024-03-17 18:43:05.000000 fastask-0.4.6/LICENSE
--rw-r--r--   0 bmachado   (501) staff       (20)     4256 2024-03-18 05:31:00.121653 fastask-0.4.6/PKG-INFO
--rw-r--r--   0 bmachado   (501) staff       (20)     3941 2024-03-17 18:43:17.000000 fastask-0.4.6/README.md
--rw-r--r--   0 bmachado   (501) staff       (20)      429 2024-03-18 05:30:30.000000 fastask-0.4.6/pyproject.toml
--rw-r--r--   0 bmachado   (501) staff       (20)       38 2024-03-18 05:31:00.121908 fastask-0.4.6/setup.cfg
-drwxr-xr-x   0 bmachado   (501) staff       (20)        0 2024-03-18 05:31:00.118571 fastask-0.4.6/src/
-drwxr-xr-x   0 bmachado   (501) staff       (20)        0 2024-03-18 05:31:00.120329 fastask-0.4.6/src/fastask/
--rw-r--r--   0 bmachado   (501) staff       (20)        0 2024-03-17 18:43:05.000000 fastask-0.4.6/src/fastask/__init__.py
--rw-r--r--   0 bmachado   (501) staff       (20)     3149 2024-03-18 05:30:36.000000 fastask-0.4.6/src/fastask/ask.py
--rw-r--r--   0 bmachado   (501) staff       (20)      818 2024-03-17 18:43:17.000000 fastask-0.4.6/src/fastask/config.py
--rw-r--r--   0 bmachado   (501) staff       (20)     1506 2024-03-17 18:43:17.000000 fastask-0.4.6/src/fastask/history.py
--rw-r--r--   0 bmachado   (501) staff       (20)     7753 2024-03-18 05:28:08.000000 fastask-0.4.6/src/fastask/llm.py
-drwxr-xr-x   0 bmachado   (501) staff       (20)        0 2024-03-18 05:31:00.121395 fastask-0.4.6/src/fastask.egg-info/
--rw-r--r--   0 bmachado   (501) staff       (20)     4256 2024-03-18 05:31:00.000000 fastask-0.4.6/src/fastask.egg-info/PKG-INFO
--rw-r--r--   0 bmachado   (501) staff       (20)      351 2024-03-18 05:31:00.000000 fastask-0.4.6/src/fastask.egg-info/SOURCES.txt
--rw-r--r--   0 bmachado   (501) staff       (20)        1 2024-03-18 05:31:00.000000 fastask-0.4.6/src/fastask.egg-info/dependency_links.txt
--rw-r--r--   0 bmachado   (501) staff       (20)       41 2024-03-18 05:31:00.000000 fastask-0.4.6/src/fastask.egg-info/entry_points.txt
--rw-r--r--   0 bmachado   (501) staff       (20)       37 2024-03-18 05:31:00.000000 fastask-0.4.6/src/fastask.egg-info/requires.txt
--rw-r--r--   0 bmachado   (501) staff       (20)        8 2024-03-18 05:31:00.000000 fastask-0.4.6/src/fastask.egg-info/top_level.txt
+drwxr-xr-x   0 bmachado   (501) staff       (20)        0 2024-04-27 04:25:55.578577 fastask-0.4.7/
+-rw-r--r--   0 bmachado   (501) staff       (20)     1070 2024-03-17 18:43:05.000000 fastask-0.4.7/LICENSE
+-rw-r--r--   0 bmachado   (501) staff       (20)     4256 2024-04-27 04:25:55.578328 fastask-0.4.7/PKG-INFO
+-rw-r--r--   0 bmachado   (501) staff       (20)     3941 2024-03-17 18:43:17.000000 fastask-0.4.7/README.md
+-rw-r--r--   0 bmachado   (501) staff       (20)      429 2024-04-27 04:23:55.000000 fastask-0.4.7/pyproject.toml
+-rw-r--r--   0 bmachado   (501) staff       (20)       38 2024-04-27 04:25:55.578622 fastask-0.4.7/setup.cfg
+drwxr-xr-x   0 bmachado   (501) staff       (20)        0 2024-04-27 04:25:55.575156 fastask-0.4.7/src/
+drwxr-xr-x   0 bmachado   (501) staff       (20)        0 2024-04-27 04:25:55.576918 fastask-0.4.7/src/fastask/
+-rw-r--r--   0 bmachado   (501) staff       (20)        0 2024-03-17 18:43:05.000000 fastask-0.4.7/src/fastask/__init__.py
+-rw-r--r--   0 bmachado   (501) staff       (20)     3796 2024-04-27 03:24:12.000000 fastask-0.4.7/src/fastask/ask.py
+-rw-r--r--   0 bmachado   (501) staff       (20)      888 2024-04-27 03:23:44.000000 fastask-0.4.7/src/fastask/config.py
+-rw-r--r--   0 bmachado   (501) staff       (20)     1506 2024-03-17 18:43:17.000000 fastask-0.4.7/src/fastask/history.py
+-rw-r--r--   0 bmachado   (501) staff       (20)     8325 2024-04-27 04:21:20.000000 fastask-0.4.7/src/fastask/llm.py
+drwxr-xr-x   0 bmachado   (501) staff       (20)        0 2024-04-27 04:25:55.578090 fastask-0.4.7/src/fastask.egg-info/
+-rw-r--r--   0 bmachado   (501) staff       (20)     4256 2024-04-27 04:25:55.000000 fastask-0.4.7/src/fastask.egg-info/PKG-INFO
+-rw-r--r--   0 bmachado   (501) staff       (20)      351 2024-04-27 04:25:55.000000 fastask-0.4.7/src/fastask.egg-info/SOURCES.txt
+-rw-r--r--   0 bmachado   (501) staff       (20)        1 2024-04-27 04:25:55.000000 fastask-0.4.7/src/fastask.egg-info/dependency_links.txt
+-rw-r--r--   0 bmachado   (501) staff       (20)       41 2024-04-27 04:25:55.000000 fastask-0.4.7/src/fastask.egg-info/entry_points.txt
+-rw-r--r--   0 bmachado   (501) staff       (20)       37 2024-04-27 04:25:55.000000 fastask-0.4.7/src/fastask.egg-info/requires.txt
+-rw-r--r--   0 bmachado   (501) staff       (20)        8 2024-04-27 04:25:55.000000 fastask-0.4.7/src/fastask.egg-info/top_level.txt
```

### Comparing `fastask-0.4.6/LICENSE` & `fastask-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastask-0.4.6/PKG-INFO` & `fastask-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastask
-Version: 0.4.6
+Version: 0.4.7
 Summary: The fastest way to get answers in the command line
 Author-email: Brian Machado <nah@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: openai
 Requires-Dist: python-dotenv
```

### Comparing `fastask-0.4.6/README.md` & `fastask-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `fastask-0.4.6/src/fastask/ask.py` & `fastask-0.4.7/src/fastask/ask.py`

 * *Files 19% similar despite different names*

```diff
@@ -65,14 +65,27 @@
 
     parser.add_argument(
         '--llm',
         type=str,
         choices=['fastask', 'fastask-local', 'azure', 'groq', 'openai', 'togetherai'],
         help='Select the large language model to use. Default is fastask. All other models and are intended for developer use and require API keys.'
     )
+    
+    parser.add_argument(
+        '--enable-leaderboard',
+        type=bool,
+        default=False,
+        help='Enable the leaderboard.'
+    )
+
+    parser.add_argument(
+        '--set-user',
+        type=str,
+        help='Specify a custom config file to use.'
+    )
 
     parser.add_argument(
         'question',
         nargs='*',
         help='Enter the question you want to ask.'
     )
 
@@ -83,14 +96,26 @@
         parser.print_help(sys.stderr)
         sys.exit(1)
 
     if args.clear:
         history_manager.clear_history()
         print("FastAsk History cleared.")
         exit()
+        
+    if args.enable_leaderboard:
+        config['enable_leaderboard'] = True
+        config_manager.save(config)
+        print("\033[92mLeaderboard enabled.\033[0m")
+        exit()
+        
+    if args.set_user:
+        config['user'] = args.set_user
+        config_manager.save(config)
+        print("\033[92mUser set to", config['user'], "\033[0m")
+        exit()
 
     # use fastask as llm by default if no llm is set
     try:
         llm = config['llm']
     except:
         config['llm'] = 'fastask'
         config_manager.save(config)
```

### Comparing `fastask-0.4.6/src/fastask/config.py` & `fastask-0.4.7/src/fastask/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 class Config:
     def __init__(self):
         self.config_dir = os.path.expanduser('~/.config/fastask')
         self.config_path = os.path.join(self.config_dir, 'config.yaml')
         self.default_config = {
             'llm': 'fastask',
+            'enable_leaderboard': False,
+            'user': ''
         }
         if not os.path.exists(self.config_dir):
             os.makedirs(self.config_dir)
         if not os.path.isfile(self.config_path):
             with open(self.config_path, 'w') as file:
                 yaml.dump(self.default_config, file, default_flow_style=False)
 
@@ -18,7 +20,9 @@
         with open(self.config_path, 'r') as file:
             config = yaml.safe_load(file)
         return config
 
     def save(self, config):
         with open(self.config_path, 'w') as file:
             yaml.dump(config, file, default_flow_style=False)
+
+
```

### Comparing `fastask-0.4.6/src/fastask/history.py` & `fastask-0.4.7/src/fastask/history.py`

 * *Files identical despite different names*

### Comparing `fastask-0.4.6/src/fastask/llm.py` & `fastask-0.4.7/src/fastask/llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,39 +3,52 @@
 import os
 import platform
 import requests
 import json
 import re
 
 from .history import History
+from .config import Config
 
 load_dotenv()
 
+config_manager = Config()
+config = config_manager.load()
+
 class LLM:
     def __init__(self, name):
         self.name = name
 
     def using(self):
         print(f"\033[91mFASTASK: Using {self.name}\033[0m")
 
 class FastAskClient(LLM):
     def __init__(self):
         super().__init__("FastAsk")
 
     def create_client(self, messages):
-        response = requests.post(url="https://fastask.fly.dev/itsfast", json={"messages": messages}).json()
-        return response
+        if config['enable_leaderboard']:
+            response = requests.post(url="https://fastask.fly.dev/itsfast", json={"messages": messages, "user": config['user'], "log": True}).json()
+            return response
+        else:
+            response = requests.post(url="https://fastask.fly.dev/itsfast", json={"messages": messages}).json()
+            return response
 
 class FastAskLocalClient(LLM):
     def __init__(self):
         super().__init__("FastAsk Local")
 
     def create_client(self, messages):
         self.using()
-        response = requests.post(url="http://0.0.0.0:8080/itsfast", json={"messages": messages}).json()
+        
+        if config['enable_leaderboard']==True:
+            response = requests.post(url="http://0.0.0.0:8080/itsfast", json={"messages": messages, "user": config['user'], "log": True}).json()
+            return response
+        else:
+            response = requests.post(url="http://0.0.0.0:8080/itsfast", json={"messages": messages}).json()
         return response
 
 class AzureClient(LLM):
     def __init__(self):
         super().__init__("Azure OpenAI")
         self.api_key = os.environ.get("AZURE_OPENAI_API_KEY")
         self.resource = os.environ.get("AZURE_RESOURCE_GROUP")
@@ -189,15 +202,15 @@
 
     if not client:
         raise ValueError("Invalid client type specified.")
 
     response = client.create_client(messages)
 
     try:
-        commands = parse_response(response['response'])
+        commands = parse_response(response["response"])
         if not commands:
             raise ValueError("No commands found. Please ensure your query is correct.")
         for i, item in enumerate(commands):
             print(f"{i+1}. '{item['command']}' - {item['desc']}")
         history_manager.add(q, response['response'])
     except:
         print(response['response'])
```

### Comparing `fastask-0.4.6/src/fastask.egg-info/PKG-INFO` & `fastask-0.4.7/src/fastask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastask
-Version: 0.4.6
+Version: 0.4.7
 Summary: The fastest way to get answers in the command line
 Author-email: Brian Machado <nah@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: openai
 Requires-Dist: python-dotenv
```

