# Comparing `tmp/atksh_utils-0.8.5.tar.gz` & `tmp/atksh_utils-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh_utils-0.8.5.tar", last modified: Thu Apr 25 04:54:49 2024, max compression
+gzip compressed data, was "atksh_utils-0.8.6.tar", last modified: Fri Apr 26 23:51:51 2024, max compression
```

## Comparing `atksh_utils-0.8.5.tar` & `atksh_utils-0.8.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.409314 atksh_utils-0.8.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.413315 atksh_utils-0.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.409314 atksh_utils-0.8.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.413315 atksh_utils-0.8.5/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.413315 atksh_utils-0.8.5/src/atksh_utils/basic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/basic/functools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.413315 atksh_utils-0.8.5/src/atksh_utils/nlp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/nlp/str_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25773 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6309 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/askgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:51.097839 atksh_utils-0.8.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:51.085840 atksh_utils-0.8.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:51.089840 atksh_utils-0.8.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-26 23:51:51.097839 atksh_utils-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-26 23:51:51.097839 atksh_utils-0.8.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:51.085840 atksh_utils-0.8.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:51.089840 atksh_utils-0.8.6/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:51.093840 atksh_utils-0.8.6/src/atksh_utils/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/basic/functools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:51.093840 atksh_utils-0.8.6/src/atksh_utils/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/nlp/str_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:51.093840 atksh_utils-0.8.6/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25773 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/openai/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6309 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/openai/askgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/openai/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/openai/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21429 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 23:51:50.000000 atksh_utils-0.8.6/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:51.093840 atksh_utils-0.8.6/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-26 23:51:51.000000 atksh_utils-0.8.6/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-26 23:51:51.000000 atksh_utils-0.8.6/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 23:51:51.000000 atksh_utils-0.8.6/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 23:51:51.000000 atksh_utils-0.8.6/src/atksh_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-26 23:51:51.000000 atksh_utils-0.8.6/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 23:51:51.000000 atksh_utils-0.8.6/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:51.093840 atksh_utils-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:51:46.000000 atksh_utils-0.8.6/tests/__init__.py
```

### Comparing `atksh_utils-0.8.5/.github/workflows/publish_to_pypi.yaml` & `atksh_utils-0.8.6/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.5/.gitignore` & `atksh_utils-0.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.5/LICENSE` & `atksh_utils-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.5/PKG-INFO` & `atksh_utils-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.8.5
+Version: 0.8.6
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh_utils-0.8.5/README.md` & `atksh_utils-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.5/pyproject.toml` & `atksh_utils-0.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.5/src/atksh_utils/basic/functools.py` & `atksh_utils-0.8.6/src/atksh_utils/basic/functools.py`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.5/src/atksh_utils/nlp/str_kernel.py` & `atksh_utils-0.8.6/src/atksh_utils/nlp/str_kernel.py`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.5/src/atksh_utils/openai/api.py` & `atksh_utils-0.8.6/src/atksh_utils/openai/api.py`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.5/src/atksh_utils/openai/askgpt.py` & `atksh_utils-0.8.6/src/atksh_utils/openai/askgpt.py`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.5/src/atksh_utils/openai/functional.py` & `atksh_utils-0.8.6/src/atksh_utils/openai/functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,16 +94,18 @@
             "description": function_description,
             "parameters": {
                 "type": "object",
                 "properties": parameters["properties"] if args else None,
                 "required": required if args else None,
             },
         }
-        if return_type:
-            function_info["return_type"] = return_type
+        # if return_type:
+        #     function_info["return_type"] = return_type
+        # else:
+        #     raise ValueError(f"Function {self.func.__name__} must have a return type.")
 
         return function_info
 
     def extract_description_from_docstring(self, docstring):
         """
         Extracts the function description from the docstring.
```

### Comparing `atksh_utils-0.8.5/src/atksh_utils/openai/prompt.py` & `atksh_utils-0.8.6/src/atksh_utils/openai/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,16 @@
 - Never output `Call functions` part but only output `output(n)` part.
 - Instead of `...`, you must call functions by tool calling as given tools or functions.
 - Once you say `I will use ...`, you must call the function in a function calling manner.
 - Otherwise, you will be asked 'Why didn't you use the function you said you would use?'
 - **Never forget to, Call the functions if you state that you will use them.**
 - `answer_subtask` function must be called as many as possible to answer the question.
   - Especially, if you need gather information from multiple sources or calculate something, you must use `answer_subtask` function.
+
+Overall, you must call the functions by tool calling as much as possible to answer the question.
 """.strip()
 
 
 def generate_prompt(more: str = "") -> str:
     return f"""
 ### Instructions
 You are LogicalGPT, an AI designed to provide expert-level responses to questions on any topic, and you use the given tools to answer the questions in a step-by-step manner.
```

### Comparing `atksh_utils-0.8.5/src/atksh_utils/openai/token.py` & `atksh_utils-0.8.6/src/atksh_utils/openai/token.py`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.5/src/atksh_utils/openai/tool.py` & `atksh_utils-0.8.6/src/atksh_utils/openai/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     subtask_model_name = ai.model_name
 
     def answer_subtask(
         context_description: str,
         subtask_description: str,
         output_format: str,
         subtask_argments_for_each_subtask: List[str],
-    ):
+    ) -> str:
         """Answers the subtask of the main task described by the parent AI. Given the context and the subtask, provide each solution for each subtask_argments_for_each_subtask. Every text should be instruction for AI. After calling this function, you will get the solutions for each subtask_argments_for_each_subtask. So, you must generate the unifined text from the solutions. Don't wait for this calling.
 
         :param context_description: The context description, which is the important information to solve the subtask.
         :type context_description: str
         :param subtask_description: The subtask description, which is the specific task to solve. This takes an argument from subtask_argments_for_each_subtask. So, the subtask is done in parallel.
         :type subtask_description: str
         :param output_format: The output format of the subtask.
@@ -525,29 +525,29 @@
     if verbose():
         print("=== Pip Install ===")
         print(ret)
         print("===================")
     return ret
 
 
-def clear_all_python_session():
+def clear_all_python_session() -> bool:
     """Clears the exec_python_code session.
 
     :return: True if the session is cleared successfully.
     :rtype: bool
     """
     try:
         if os.path.exists(SESSION_PATH):
             os.remove(SESSION_PATH)
         return True
     except:
         return False
 
 
-def wait_sec(seconds: int = 1):
+def wait_sec(seconds: int = 1) -> str:
     """Wait for the given seconds(1 second by default). This is useful when you want to write a too long text. 1 secons enables you to write about 4096 tokens. So before reaching the limit, you can use this function to wait for a while.
 
     :param seconds: The seconds to wait.
     :type seconds: int, optional
     :return: waited message.
     :rtype: str
     """
```

### Comparing `atksh_utils-0.8.5/src/atksh_utils.egg-info/PKG-INFO` & `atksh_utils-0.8.6/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.8.5
+Version: 0.8.6
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh_utils-0.8.5/src/atksh_utils.egg-info/SOURCES.txt` & `atksh_utils-0.8.6/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

