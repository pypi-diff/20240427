# Comparing `tmp/tool_use-0.1.1rc6.tar.gz` & `tmp/tool_use-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_use-0.1.1rc6.tar", last modified: Wed Apr 17 06:08:38 2024, max compression
+gzip compressed data, was "tool_use-0.2.0.tar", last modified: Sat Apr 27 01:47:26 2024, max compression
```

## Comparing `tool_use-0.1.1rc6.tar` & `tool_use-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.031640 tool_use-0.1.1rc6/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.1.1rc6/MANIFEST.in
--rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-17 06:08:38.031381 tool_use-0.1.1rc6/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      370 2024-04-14 06:28:02.000000 tool_use-0.1.1rc6/README.md
--rw-r--r--   0 kimjaemin   (501) staff       (20)      532 2024-04-14 06:26:15.000000 tool_use-0.1.1rc6/pyproject.toml
--rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-17 06:08:38.031699 tool_use-0.1.1rc6/setup.cfg
--rw-r--r--   0 kimjaemin   (501) staff       (20)      530 2024-04-17 06:08:05.000000 tool_use-0.1.1rc6/setup.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.027573 tool_use-0.1.1rc6/tests/
--rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.1.1rc6/tests/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     4967 2024-04-17 05:56:16.000000 tool_use-0.1.1rc6/tests/test_anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-08 11:36:45.000000 tool_use-0.1.1rc6/tests/test_exception.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-14 05:56:49.000000 tool_use-0.1.1rc6/tests/test_openai_tool_use.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.027720 tool_use-0.1.1rc6/tool_use/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc6/tool_use/__init__.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.030265 tool_use-0.1.1rc6/tool_use/tools/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc6/tool_use/tools/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    17883 2024-04-16 11:57:24.000000 tool_use-0.1.1rc6/tool_use/tools/anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-14 06:13:17.000000 tool_use-0.1.1rc6/tool_use/tools/openai_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.1.1rc6/tool_use/tools/utils.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.030850 tool_use-0.1.1rc6/tool_use/yamls/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      909 2024-04-15 14:13:42.000000 tool_use-0.1.1rc6/tool_use/yamls/anthropic_tool_use.yaml
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.1.1rc6/tool_use/yamls/openai_tool_use.yaml
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.031070 tool_use-0.1.1rc6/tool_use.egg-info/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-17 06:08:37.000000 tool_use-0.1.1rc6/tool_use.egg-info/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-17 06:08:37.000000 tool_use-0.1.1rc6/tool_use.egg-info/SOURCES.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-17 06:08:37.000000 tool_use-0.1.1rc6/tool_use.egg-info/dependency_links.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-17 06:08:37.000000 tool_use-0.1.1rc6/tool_use.egg-info/entry_points.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-17 06:08:37.000000 tool_use-0.1.1rc6/tool_use.egg-info/top_level.txt
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.101899 tool_use-0.2.0/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.2.0/MANIFEST.in
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      106 2024-04-27 01:47:26.101645 tool_use-0.2.0/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      564 2024-04-22 14:29:43.000000 tool_use-0.2.0/README.md
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      553 2024-04-27 01:47:16.000000 tool_use-0.2.0/pyproject.toml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-27 01:47:26.101957 tool_use-0.2.0/setup.cfg
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      527 2024-04-27 01:47:09.000000 tool_use-0.2.0/setup.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.099503 tool_use-0.2.0/tests/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.2.0/tests/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     9400 2024-04-26 08:03:24.000000 tool_use-0.2.0/tests/test_anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-22 14:29:43.000000 tool_use-0.2.0/tests/test_exception.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-22 14:29:43.000000 tool_use-0.2.0/tests/test_openai_tool_use.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.099700 tool_use-0.2.0/tool_use/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.2.0/tool_use/__init__.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.100947 tool_use-0.2.0/tool_use/tools/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.2.0/tool_use/tools/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    18131 2024-04-24 02:37:31.000000 tool_use-0.2.0/tool_use/tools/anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-22 14:44:36.000000 tool_use-0.2.0/tool_use/tools/openai_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.2.0/tool_use/tools/utils.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.101209 tool_use-0.2.0/tool_use/yamls/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      909 2024-04-22 14:29:43.000000 tool_use-0.2.0/tool_use/yamls/anthropic_tool_use.yaml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.2.0/tool_use/yamls/openai_tool_use.yaml
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.101388 tool_use-0.2.0/tool_use.egg-info/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      106 2024-04-27 01:47:26.000000 tool_use-0.2.0/tool_use.egg-info/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-27 01:47:26.000000 tool_use-0.2.0/tool_use.egg-info/SOURCES.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-27 01:47:26.000000 tool_use-0.2.0/tool_use.egg-info/dependency_links.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-27 01:47:26.000000 tool_use-0.2.0/tool_use.egg-info/entry_points.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-27 01:47:26.000000 tool_use-0.2.0/tool_use.egg-info/top_level.txt
```

### Comparing `tool_use-0.1.1rc6/pyproject.toml` & `tool_use-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
-name = "too_use"
-version = "0.1.0"
+name = "tool_use"
+version = "0.2.0"
 description = "Promptflow tool package for OpenAI/Anthropic"
 authors = ["ethan <ethan@wrtn.io>", "JaeminBest <mikjm98@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-promptflow = "1.7.0"
-promptflow-tools = "1.4.0"
 anthropic = "^0.23.1"
+openai = "^1.23.2"
+promptflow = "1.9.0"
+promptflow-tools = "^1.4.0"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
 pre-commit = "^3.6.1"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
```

### Comparing `tool_use-0.1.1rc6/setup.py` & `tool_use-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "tool_use"
 
 setup(
     name=PACKAGE_NAME,
-    version="0.1.1rc6",
+    version="0.2.0",
     description="Promptflow tool package for OpenAI/Anthropic",
     packages=find_packages(),
     entry_points={
         "package_tools": [
             "openai_tool_use = tool_use.tools.utils:list_package_tools",
             "anthropic_tool_use = tool_use.tools.utils:list_package_tools",
         ],
```

### Comparing `tool_use-0.1.1rc6/tests/test_exception.py` & `tool_use-0.2.0/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc6/tests/test_openai_tool_use.py` & `tool_use-0.2.0/tests/test_openai_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc6/tool_use/tools/anthropic_tool_use.py` & `tool_use-0.2.0/tool_use/tools/anthropic_tool_use.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,51 +139,51 @@
     for chunk in chunks:
         last_message = results[-1] if len(results) > 0 else None
         if last_message and "role" in last_message and "content" not in last_message:
             parsed_chunk = parse_section(chunk)
             if "text" in parsed_chunk:
                 last_message["content"] = {
                     "type": "text",
-                    "text": parsed_chunk["text"].strip(),
+                    "text": parsed_chunk["text"].strip().strip("\n"),
                 }
             else:
                 last_message["content"] = parsed_chunk
             # figure out whether there is type called tool_use or tool_result
             is_tool_use |= any(map(lambda x: x["type"] == "tool_use", parsed_chunk))
         else:
-            if chunk.strip() == "":
+            if chunk.strip().strip("\n") == "":
                 continue
-            role = chunk.strip().lower()
+            role = chunk.strip().strip("\n").lower()
             validate_role(role, valid_roles=valid_roles)
             new_message = dict(role=role)
             results.append(new_message)
 
     return results, is_tool_use
 
 
 def parse_section(content: str) -> List[Dict[str, Any]]:
     content_list = []
     # Regex to capture entries by type
     type_entries = re.split(r"\n(?=type:)", content)
     for entry in type_entries:
-        if entry.strip():  # Ensure entry is not just whitespace
+        if entry.strip().strip("\n"):  # Ensure entry is not just whitespace
             entry_data = parse_entry(entry)
             if entry_data["type"] is None:
                 entry_data = {"type": "text", "text": content}
             content_list.append(entry_data)
     if not type_entries:
         return
     return content_list
 
 
 def parse_entry(entry: str) -> Dict[str, Any]:
     # Initial split to separate type from details
     first_line, *details = entry.split("\n")
     type_match = re.match(r"type:\s*(.*)", first_line)
-    type_key = type_match.group(1).strip() if type_match else None
+    type_key = type_match.group(1).strip().strip("\n") if type_match else None
     details = "\n".join(details)
     entry_details = parse_details(details)
     entry_details["type"] = type_key
     return entry_details
 
 
 def parse_details(details: str) -> Dict[str, Any]:
@@ -263,21 +263,21 @@
                             "retry-after", None
                         )
                     else:
                         retry_after_in_header = None
 
                     if not retry_after_in_header:
                         retry_after_seconds = generate_retry_interval(i)
-                        (
+                        error_message = (
                             f"{type(e).__name__} #{i}, but no Retry-After header, "
                             + f"Back off {retry_after_seconds} seconds for retry."
                         )
                     else:
                         retry_after_seconds = float(retry_after_in_header)
-                        (
+                        error_message = (
                             f"{type(e).__name__} #{i}, Retry-After={retry_after_in_header}, "
                             f"Back off {retry_after_seconds} seconds for retry."
                         )
                         # print(msg, file=sys.stderr)
                     time.sleep(retry_after_seconds)
                 except AnthropicError as e:
                     raise WrappedAnthropicError(e)
@@ -397,44 +397,50 @@
 @tool
 @handle_anthropic_error()
 async def anthropic_tool_use(
     connection: AnthropicConnection,
     prompt: PromptTemplate,
     model: ModelEnum,
     max_tokens: int,
-    temperature: float = 1,
-    top_p: float = 1,
-    n: int = 1,
+    temperature: Optional[float] = None,
+    top_p: Optional[float] = None,
+    n: Optional[int] = None,
     stream: Optional[bool] = False,
     stop: Optional[list] = None,  # type: ignore
-    user: Optional[str] = "",
+    user: Optional[str] = None,
     tools: Optional[list[ToolParam]] = None,  # type: ignore
     extra_headers: Optional[dict] = {},
     is_raw_output: Optional[bool] = False,
     **kwargs,
 ) -> str | dict | Message | AsyncMessageStreamManager:  # type: ignore
     chat_str = render_jinja_template(
         prompt, trim_blocks=True, keep_trailing_newline=True, **kwargs
     )
     system, messages, is_tool_use = _parse_chat(chat_str)
     # TODO: remove below type conversion after client can pass json rather than string.
     stream = to_bool(stream)
     params = {
         "model": model,
         "messages": messages,
-        "system": system,
-        "temperature": float(temperature),
-        "top_p": float(top_p),
-        "top_k": int(n),
-        "stop_sequences": stop if stop else None,
         "max_tokens": int(max_tokens)
         if max_tokens is not None and str(max_tokens).lower() != "inf"
         else None,
-        "metadata": {"user_id": user},
     }
+    if system:
+        params["system"] = system
+    if temperature:
+        params["temperature"] = float(temperature)
+    if top_p:
+        params["top_p"] = float(top_p)
+    if n:
+        params["top_k"] = int(n)
+    if stop:
+        params["stop_sequences"] = stop
+    if user:
+        params["metadata"] = {"user_id": user}
 
     if tools is not None:
         for tool_desc in tools:
             if (
                 "name" in tool_desc
                 and "description" in tool_desc
                 and "input_schema" in tool_desc
```

### Comparing `tool_use-0.1.1rc6/tool_use/tools/openai_tool_use.py` & `tool_use-0.2.0/tool_use/tools/openai_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc6/tool_use/tools/utils.py` & `tool_use-0.2.0/tool_use/tools/utils.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc6/tool_use/yamls/anthropic_tool_use.yaml` & `tool_use-0.2.0/tool_use/yamls/anthropic_tool_use.yaml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc6/tool_use/yamls/openai_tool_use.yaml` & `tool_use-0.2.0/tool_use/yamls/openai_tool_use.yaml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc6/tool_use.egg-info/SOURCES.txt` & `tool_use-0.2.0/tool_use.egg-info/SOURCES.txt`

 * *Files identical despite different names*

