# Comparing `tmp/mllm-0.1.1.tar.gz` & `tmp/mllm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mllm-0.1.1.tar", max compression
+gzip compressed data, was "mllm-0.1.2.tar", max compression
```

## Comparing `mllm-0.1.1.tar` & `mllm-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-04-26 18:14:18.983376 mllm-0.1.1/LICENSE
--rw-r--r--   0        0        0     1608 2024-04-27 04:44:15.927956 mllm-0.1.1/README.md
--rw-r--r--   0        0        0      159 2024-04-26 20:09:13.679618 mllm-0.1.1/mllm/__init__.py
--rw-r--r--   0        0        0     1983 2024-04-26 19:57:01.938681 mllm-0.1.1/mllm/db/conn.py
--rw-r--r--   0        0        0      541 2024-04-26 19:57:07.955475 mllm-0.1.1/mllm/db/models.py
--rw-r--r--   0        0        0     8301 2024-04-26 20:18:49.506166 mllm-0.1.1/mllm/llm.py
--rw-r--r--   0        0        0      872 2024-04-26 20:05:40.818311 mllm-0.1.1/mllm/models.py
--rw-r--r--   0        0        0     5661 2024-04-26 19:58:53.250721 mllm-0.1.1/mllm/prompt.py
--rw-r--r--   0        0        0      793 2024-04-26 20:06:05.547334 mllm-0.1.1/mllm/util.py
--rw-r--r--   0        0        0      376 2024-04-27 04:47:06.447979 mllm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 mllm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-27 16:19:02.140835 mllm-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1855 2024-04-27 16:19:02.140994 mllm-0.1.2/README.md
+-rw-r--r--   0        0        0      154 2024-04-27 16:19:02.141169 mllm-0.1.2/mllm/__init__.py
+-rw-r--r--   0        0        0     1983 2024-04-27 16:19:02.141340 mllm-0.1.2/mllm/db/conn.py
+-rw-r--r--   0        0        0      541 2024-04-27 16:19:02.141445 mllm-0.1.2/mllm/db/models.py
+-rw-r--r--   0        0        0      852 2024-04-27 16:19:02.141546 mllm-0.1.2/mllm/models.py
+-rw-r--r--   0        0        0     5661 2024-04-27 16:19:02.141676 mllm-0.1.2/mllm/prompt.py
+-rw-r--r--   0        0        0     8270 2024-04-27 16:19:02.141835 mllm-0.1.2/mllm/router.py
+-rw-r--r--   0        0        0      793 2024-04-27 16:19:02.141946 mllm-0.1.2/mllm/util.py
+-rw-r--r--   0        0        0      390 2024-04-27 16:19:43.355808 mllm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 mllm-0.1.2/PKG-INFO
```

### Comparing `mllm-0.1.1/LICENSE` & `mllm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mllm-0.1.1/README.md` & `mllm-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,80 @@
-# yapr
+# MLLM
 
-yapr (Yet Another Prompt)
+MultiModal Large Language Models
 
 ## Installation
 
 ```sh
-pip install yapr
+pip install mllm
 ```
 
-llms?
-
 ## Usage
 
-Create an LLM provider from the API keys found in the current system env vars
+Create an MLLM router from the API keys found in the current system env vars
 
 ```python
-from yapr import LLMProvider, RoleThread
+import os
+from mllm import MLLMRouter
+
+os.environ["OPENAI_API_KEY"] = "..."
+os.environ["ANTHROPIC_API_KEY"] = "..."
+os.environ["GEMINI_API_KEY"] = "..."
 
-llm_provider = LLMProvider.from_env()
+router = MLLMRouter.from_env()
 ```
 
 Create a new role based chat thread
 
 ```python
+from mllm import RoleThread
+
 thread = RoleThread()
-thread.post(role="user", msg="How are you?")
+thread.post(role="user", msg="How are you?", images=["data:image/jpeg;base64,..."])
 ```
 
-Chat with the LLM, store the prompt data in the namespace "foo"
+Chat with the MLLM, store the prompt data in the namespace `foo`
 
 ```python
-response = llm_provider.chat(thread, namespace="foo")
-
+response = router.chat(thread, namespace="foo")
 thread.add_msg(response.msg)
 ```
 
 Ask for a structured response
 
 ```python
 from pydantic import BaseModel
 
 class Foo(BaseModel):
     bar: str
     baz: int
 
-thread.post(role="user", msg="Given the {...} can you return that in JSON?")
+thread.post(
+    role="user",
+    msg=f"What are bar and baz in this image? Please output as schema {Foo.model_json_schema()}"
+    images=["data:image/jpeg;base64,..."]
+)
 
-response = llm_provider.chat(thread, namespace="foo", response_schema=Foo)
+response = router.chat(thread, namespace="foo", response_schema=Foo)
 foo_parsed = response.parsed
 
 assert type(foo_parsed) == Foo
 ```
 
-Multimodal
+Find a saved thread or a prompt
 
 ```python
-
-```
-
-Find a saved thread
-
-```python
-
-```
-
-Find a saved prompt
-
-```python
-
+RoleThread.find(id="123")
+Prompt.find(id="456)
 ```
 
 Just store prompts
 
 ```python
-from yapr import Prompt, RoleThread
+from mllm import Prompt, RoleThread
 
 thread = RoleThread()
 
 msg = {
     "role": "user",
     "content": [
         {
```

### Comparing `mllm-0.1.1/mllm/db/conn.py` & `mllm-0.1.2/mllm/db/conn.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.1/mllm/db/models.py` & `mllm-0.1.2/mllm/db/models.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.1/mllm/llm.py` & `mllm-0.1.2/mllm/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from litellm import Router, ModelResponse
 from threadmem import RoleThread, RoleMessage
 from litellm._logging import handler
 from pydantic import BaseModel
 from tenacity import retry, stop_after_attempt
 
-from .models import EnvVarOptModel, LLMProviderOption
+from .models import EnvVarOptModel, MLLMModel, MLLMOption
 from .util import extract_parse_json
 from .prompt import Prompt
 
 
 T = TypeVar("T", bound=BaseModel)
 
 
@@ -23,17 +23,17 @@
     parsed: Optional[T] = None
     time_elapsed: float
     tokens_request: int
     tokens_response: int
     prompt_id: str
 
 
-class LLMProvider:
+class MLLMRouter:
     """
-    A chat provider based on LiteLLM
+    A multimodal chat provider
     """
 
     provider_api_keys: Dict[str, str] = {
         "gpt-4-turbo": "OPENAI_API_KEY",
         "anthropic/claude-3-opus-20240229": "ANTHROPIC_API_KEY",
         "gemini/gemini-pro-vision": "GEMINI_API_KEY",
     }
@@ -97,19 +97,19 @@
         verbose_router_logger = logging.getLogger("LiteLLM Router")
         verbose_router_logger.setLevel(logging.ERROR)
         verbose_logger = logging.getLogger("LiteLLM")
         verbose_logger.setLevel(logging.ERROR)
         handler.setLevel(logging.ERROR)
 
     @classmethod
-    def all_opts(cls) -> List[LLMProviderOption]:
+    def all_opts(cls) -> List[MLLMOption]:
         out = []
         for model, key in cls.provider_api_keys.items():
             out.append(
-                LLMProviderOption(
+                MLLMOption(
                     model=model,
                     env_var=EnvVarOptModel(
                         name=key,
                         description=f"{model} API key",
                         required=True,
                         secret=True,
                     ),
@@ -195,22 +195,22 @@
         thread = RoleThread()
         thread.post(
             "user", "Just checking if you are working... please return 'yes' if you are"
         )
         response = self.chat(thread)
         print("response from checking oai functionality: ", response)
 
-    def options(self) -> List[LLMProviderOption]:
+    def options(self) -> List[MLLMOption]:
         """Dynamically generates options based on the configured providers."""
         options = []
         for model_info in self.model_list:
             model_name = model_info["model_name"]
             api_key_env = self.provider_api_keys.get(model_name)
             if api_key_env:
-                option = LLMProviderOption(
+                option = MLLMOption(
                     model=model_name,
                     env_var=EnvVarOptModel(
                         name=api_key_env,
                         description=f"{model_name} API key",
                         required=True,
                         secret=True,
                     ),
```

### Comparing `mllm-0.1.1/mllm/models.py` & `mllm-0.1.2/mllm/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     description: Optional[str] = None
     required: bool = False
     default: Optional[str] = None
     secret: bool = False
     options: List[str] = []
 
 
-class LLMProviders(BaseModel):
+class MLLMProviders(BaseModel):
     preference: List[str] = []
 
 
-class LLMProviderOption(BaseModel):
+class MLLMOption(BaseModel):
     model: str
     env_var: EnvVarOptModel
 
 
-class LLMProviderModel(BaseModel):
-    options: List[LLMProviderOption]
+class MLLMModel(BaseModel):
+    options: List[MLLMOption]
```

### Comparing `mllm-0.1.1/mllm/prompt.py` & `mllm-0.1.2/mllm/prompt.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.1/mllm/util.py` & `mllm-0.1.2/mllm/util.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.1/PKG-INFO` & `mllm-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,100 +1,97 @@
 Metadata-Version: 2.1
 Name: mllm
-Version: 0.1.1
-Summary: Yet another prompt
+Version: 0.1.2
+Summary: Multimodal Large Language Models
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: litellm (>=1.35.29,<2.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: threadmem (>=0.2.24,<0.3.0)
 Description-Content-Type: text/markdown
 
-# yapr
+# MLLM
 
-yapr (Yet Another Prompt)
+MultiModal Large Language Models
 
 ## Installation
 
 ```sh
-pip install yapr
+pip install mllm
 ```
 
-llms?
-
 ## Usage
 
-Create an LLM provider from the API keys found in the current system env vars
+Create an MLLM router from the API keys found in the current system env vars
 
 ```python
-from yapr import LLMProvider, RoleThread
+import os
+from mllm import MLLMRouter
+
+os.environ["OPENAI_API_KEY"] = "..."
+os.environ["ANTHROPIC_API_KEY"] = "..."
+os.environ["GEMINI_API_KEY"] = "..."
 
-llm_provider = LLMProvider.from_env()
+router = MLLMRouter.from_env()
 ```
 
 Create a new role based chat thread
 
 ```python
+from mllm import RoleThread
+
 thread = RoleThread()
-thread.post(role="user", msg="How are you?")
+thread.post(role="user", msg="How are you?", images=["data:image/jpeg;base64,..."])
 ```
 
-Chat with the LLM, store the prompt data in the namespace "foo"
+Chat with the MLLM, store the prompt data in the namespace `foo`
 
 ```python
-response = llm_provider.chat(thread, namespace="foo")
-
+response = router.chat(thread, namespace="foo")
 thread.add_msg(response.msg)
 ```
 
 Ask for a structured response
 
 ```python
 from pydantic import BaseModel
 
 class Foo(BaseModel):
     bar: str
     baz: int
 
-thread.post(role="user", msg="Given the {...} can you return that in JSON?")
+thread.post(
+    role="user",
+    msg=f"What are bar and baz in this image? Please output as schema {Foo.model_json_schema()}"
+    images=["data:image/jpeg;base64,..."]
+)
 
-response = llm_provider.chat(thread, namespace="foo", response_schema=Foo)
+response = router.chat(thread, namespace="foo", response_schema=Foo)
 foo_parsed = response.parsed
 
 assert type(foo_parsed) == Foo
 ```
 
-Multimodal
+Find a saved thread or a prompt
 
 ```python
-
-```
-
-Find a saved thread
-
-```python
-
-```
-
-Find a saved prompt
-
-```python
-
+RoleThread.find(id="123")
+Prompt.find(id="456)
 ```
 
 Just store prompts
 
 ```python
-from yapr import Prompt, RoleThread
+from mllm import Prompt, RoleThread
 
 thread = RoleThread()
 
 msg = {
     "role": "user",
     "content": [
         {
```

