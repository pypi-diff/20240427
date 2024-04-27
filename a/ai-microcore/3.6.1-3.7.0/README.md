# Comparing `tmp/ai_microcore-3.6.1.tar.gz` & `tmp/ai_microcore-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_microcore-3.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ai_microcore-3.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ai_microcore-3.6.1.tar` & `ai_microcore-3.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.6.1/LICENSE
--rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.6.1/README.md
--rwxr-xr-x   0        0        0     3988 2024-04-23 23:26:29.842689 ai_microcore-3.6.1/microcore/__init__.py
--rwxr-xr-x   0        0        0     6667 2024-04-23 20:32:58.168012 ai_microcore-3.6.1/microcore/_env.py
--rwxr-xr-x   0        0        0     3790 2024-04-20 15:07:06.612137 ai_microcore-3.6.1/microcore/_llm_functions.py
--rwxr-xr-x   0        0        0      786 2024-04-20 12:35:24.174582 ai_microcore-3.6.1/microcore/_prepare_llm_args.py
--rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.6.1/microcore/ai_func/__init__.py
--rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.6.1/microcore/ai_func/python_ai_func.j2
--rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.6.1/microcore/ai_modules.py
--rwxr-xr-x   0        0        0    11591 2024-04-20 14:59:40.736447 ai_microcore-3.6.1/microcore/configuration.py
--rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.6.1/microcore/embedding_db/__init__.py
--rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.6.1/microcore/embedding_db/chromadb.py
--rwxr-xr-x   0        0        0     8400 2024-04-23 02:00:56.476715 ai_microcore-3.6.1/microcore/file_storage.py
--rwxr-xr-x   0        0        0     4725 2024-04-20 12:35:24.223611 ai_microcore-3.6.1/microcore/json_parsing.py
--rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.6.1/microcore/llm/__init__.py
--rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.6.1/microcore/llm/_openai_llm_v0.py
--rwxr-xr-x   0        0        0     5120 2024-04-18 17:18:22.746984 ai_microcore-3.6.1/microcore/llm/_openai_llm_v1.py
--rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.6.1/microcore/llm/anthropic.py
--rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.6.1/microcore/llm/google_genai.py
--rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.6.1/microcore/llm/google_vertex_ai.py
--rwxr-xr-x   0        0        0     3413 2024-04-23 17:22:46.408066 ai_microcore-3.6.1/microcore/llm/local_llm.py
--rwxr-xr-x   0        0        0     5815 2024-04-23 19:57:00.633732 ai_microcore-3.6.1/microcore/llm/local_transformers.py
--rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.6.1/microcore/llm/openai_llm.py
--rwxr-xr-x   0        0        0     2490 2024-04-22 18:59:09.500665 ai_microcore-3.6.1/microcore/logging.py
--rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.6.1/microcore/message_types.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.6.1/microcore/templating/__init__.py
--rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.6.1/microcore/templating/jinja2.py
--rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.6.1/microcore/text2speech/elevenlabs.py
--rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.6.1/microcore/types.py
--rwxr-xr-x   0        0        0     1601 2024-04-19 09:12:25.103139 ai_microcore-3.6.1/microcore/ui.py
--rwxr-xr-x   0        0        0     9089 2024-04-21 17:42:07.690371 ai_microcore-3.6.1/microcore/utils.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.6.1/microcore/wrappers/__init__.py
--rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.6.1/microcore/wrappers/llm_response_wrapper.py
--rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.6.1/microcore/wrappers/prompt_wrapper.py
--rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.6.1/pyproject.toml
--rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.6.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.7.0/LICENSE
+-rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.7.0/README.md
+-rwxr-xr-x   0        0        0     3985 2024-04-26 20:52:07.847195 ai_microcore-3.7.0/microcore/__init__.py
+-rwxr-xr-x   0        0        0     6943 2024-04-26 20:19:54.776713 ai_microcore-3.7.0/microcore/_env.py
+-rwxr-xr-x   0        0        0     3790 2024-04-20 15:07:06.612137 ai_microcore-3.7.0/microcore/_llm_functions.py
+-rwxr-xr-x   0        0        0      881 2024-04-26 20:19:54.634711 ai_microcore-3.7.0/microcore/_prepare_llm_args.py
+-rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.7.0/microcore/ai_func/__init__.py
+-rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.7.0/microcore/ai_func/python_ai_func.j2
+-rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.7.0/microcore/ai_modules.py
+-rwxr-xr-x   0        0        0    12344 2024-04-26 20:20:57.360040 ai_microcore-3.7.0/microcore/configuration.py
+-rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.7.0/microcore/embedding_db/__init__.py
+-rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.7.0/microcore/embedding_db/chromadb.py
+-rwxr-xr-x   0        0        0     8400 2024-04-23 02:00:56.476715 ai_microcore-3.7.0/microcore/file_storage.py
+-rwxr-xr-x   0        0        0     4725 2024-04-20 12:35:24.223611 ai_microcore-3.7.0/microcore/json_parsing.py
+-rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.7.0/microcore/llm/__init__.py
+-rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.7.0/microcore/llm/_openai_llm_v0.py
+-rwxr-xr-x   0        0        0     5120 2024-04-18 17:18:22.746984 ai_microcore-3.7.0/microcore/llm/_openai_llm_v1.py
+-rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.7.0/microcore/llm/anthropic.py
+-rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.7.0/microcore/llm/google_genai.py
+-rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.7.0/microcore/llm/google_vertex_ai.py
+-rwxr-xr-x   0        0        0     3413 2024-04-23 17:22:46.408066 ai_microcore-3.7.0/microcore/llm/local_llm.py
+-rwxr-xr-x   0        0        0     9787 2024-04-26 20:29:14.713168 ai_microcore-3.7.0/microcore/llm/local_transformers.py
+-rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.7.0/microcore/llm/openai_llm.py
+-rwxr-xr-x   0        0        0     2490 2024-04-22 18:59:09.500665 ai_microcore-3.7.0/microcore/logging.py
+-rwxr-xr-x   0        0        0     1669 2024-04-26 20:21:12.539912 ai_microcore-3.7.0/microcore/message_types.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.7.0/microcore/templating/__init__.py
+-rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.7.0/microcore/templating/jinja2.py
+-rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.7.0/microcore/text2speech/elevenlabs.py
+-rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.7.0/microcore/types.py
+-rwxr-xr-x   0        0        0     1601 2024-04-19 09:12:25.103139 ai_microcore-3.7.0/microcore/ui.py
+-rwxr-xr-x   0        0        0     9089 2024-04-21 17:42:07.690371 ai_microcore-3.7.0/microcore/utils.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.7.0/microcore/wrappers/__init__.py
+-rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.7.0/microcore/wrappers/llm_response_wrapper.py
+-rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.7.0/microcore/wrappers/prompt_wrapper.py
+-rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.7.0/PKG-INFO
```

### Comparing `ai_microcore-3.6.1/LICENSE` & `ai_microcore-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/README.md` & `ai_microcore-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/__init__.py` & `ai_microcore-3.7.0/microcore/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,38 +9,34 @@
 
 import os
 import microcore.ui  # noqa
 from .embedding_db import SearchResult, AbstractEmbeddingDB
 from .file_storage import storage
 from ._env import configure, env, config
 from .logging import use_logging
-from .message_types import UserMsg, AssistantMsg, SysMsg, Msg
+from .message_types import UserMsg, AssistantMsg, SysMsg, Msg, PartialMsg
 from .configuration import ApiType, LLMConfigError, Config
 from .types import BadAIJsonAnswer, BadAIAnswer
 from .wrappers.prompt_wrapper import PromptWrapper
 from .wrappers.llm_response_wrapper import LLMResponse
 from ._llm_functions import llm, allm, llm_parallel
 from .utils import parse, dedent
 
 
 def tpl(file: os.PathLike[str] | str, **kwargs) -> str | PromptWrapper:
     """Renders a prompt template using the provided parameters."""
-    return PromptWrapper(
-        env().tpl_function(file, **kwargs),
-        kwargs
-    )
+    return PromptWrapper(env().tpl_function(file, **kwargs), kwargs)
 
 
 def prompt(template_str: str, remove_indent=True, **kwargs) -> str | PromptWrapper:
     """Renders a prompt template from string using the provided parameters."""
     if remove_indent:
         template_str = dedent(template_str)
     return PromptWrapper(
-        env().jinja_env.from_string(template_str).render(**kwargs),
-        kwargs
+        env().jinja_env.from_string(template_str).render(**kwargs), kwargs
     )
 
 
 fmt = prompt
 
 
 def use_model(name: str):
@@ -119,14 +115,15 @@
     "use_logging",
     "env",
     "config",
     "Msg",
     "UserMsg",
     "SysMsg",
     "AssistantMsg",
+    "PartialMsg",
     "ApiType",
     "BadAIJsonAnswer",
     "BadAIAnswer",
     "LLMConfigError",
     "LLMResponse",
     "PromptWrapper",
     "parse",
@@ -139,8 +136,8 @@
     "configuration",
     "Config",
     "types",
     "ui",
     # "wrappers",
 ]
 
-__version__ = "3.6.1"
+__version__ = "3.7.0"
```

### Comparing `ai_microcore-3.6.1/microcore/_env.py` & `ai_microcore-3.7.0/microcore/_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,26 +16,31 @@
     jinja_env: jinja2.Environment = None
     tpl_function: TplFunctionType = None
     llm_async_function: LLMAsyncFunctionType = None
     llm_function: LLMFunctionType = None
     llm_before_handlers: list[callable] = field(default_factory=list)
     llm_after_handlers: list[callable] = field(default_factory=list)
     texts: AbstractEmbeddingDB = None
+    model: "PreTrainedModel" = field(default=None, init=False, repr=False)
+    tokenizer: "PreTrainedTokenizer" = field(default=None, init=False, repr=False)
 
     def __post_init__(self):
         global _env
         _env = self
         self.init_templating()
         self.init_llm()
         if self.config.USE_LOGGING:
             from .logging import use_logging
 
             use_logging()
         self.init_similarity_search()
 
+    def make_stopping_criteria(self, seq: str | list[str]) -> list[callable]:
+        raise NotImplementedError
+
     def init_templating(self):
         self.jinja_env = make_jinja2_env(self)
         self.tpl_function = make_tpl_function(self)
 
     def init_llm(self):
         if self.config.LLM_API_TYPE == ApiType.NONE:
```

### Comparing `ai_microcore-3.6.1/microcore/_llm_functions.py` & `ai_microcore-3.7.0/microcore/_llm_functions.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/_prepare_llm_args.py` & `ai_microcore-3.7.0/microcore/_prepare_llm_args.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,11 +16,15 @@
 def prepare_chat_messages(prompt) -> list[dict]:
     """Converts prompt to messages for LLM chat API (OpenAI)"""
     messages = prompt if isinstance(prompt, list) else [prompt]
     return [
         (
             dict(role=DEFAULT_MESSAGE_ROLE, content=msg)
             if isinstance(msg, str)
-            else asdict(msg) if isinstance(msg, Msg) else msg
+            else (
+                asdict(msg, dict_factory=msg.dict_factory)
+                if isinstance(msg, Msg)
+                else msg
+            )
         )
         for msg in messages
     ]
```

### Comparing `ai_microcore-3.6.1/microcore/ai_func/__init__.py` & `ai_microcore-3.7.0/microcore/ai_func/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/ai_modules.py` & `ai_microcore-3.7.0/microcore/ai_modules.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/configuration.py` & `ai_microcore-3.7.0/microcore/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 from dataclasses import dataclass, field, fields
 from pathlib import Path
 from typing import Any
 from typing import Union, Callable
 
 import dotenv
+from colorama import Fore
 
 _MISSING = object()
 
 TRUE_VALUES = ["1", "TRUE", "YES", "ON", "ENABLED", "Y", "+"]
 """@private"""
 
 
@@ -270,14 +271,35 @@
                     )
                 if not self.LLM_API_VERSION:
                     raise LLMConfigError(
                         "LLM configuration error: "
                         "LLM_API_VERSION is required for using Azure models"
                     )
 
+    def describe(self, return_dict=False):
+        """
+        Informal description of the configuration
+        """
+        default = Config(LLM_API_TYPE=ApiType.NONE, USE_DOT_ENV=False)
+        data = {
+            k.lower().replace("llm_", ""): v
+            for k, v in dict(self).items()
+            if v is not None and v != getattr(default, k) and k != "USE_DOT_ENV"
+        }
+        for k, v in data.items():
+            if "_key" in k and isinstance(v, str):
+                data[k] = v[:1] + "****" + v[-2:]
+        if return_dict:
+            return data
+
+        print("Config:")
+        for k, v in data.items():
+            print(f"  {k}: {Fore.GREEN}{v}{Fore.RESET}")
+        return None
+
 
 class LLMConfigError(ValueError):
     """LLM configuration error"""
 
 
 @dataclass
 class Config(LLMConfig):
```

### Comparing `ai_microcore-3.6.1/microcore/embedding_db/__init__.py` & `ai_microcore-3.7.0/microcore/embedding_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/embedding_db/chromadb.py` & `ai_microcore-3.7.0/microcore/embedding_db/chromadb.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/file_storage.py` & `ai_microcore-3.7.0/microcore/file_storage.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/json_parsing.py` & `ai_microcore-3.7.0/microcore/json_parsing.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/llm/_openai_llm_v0.py` & `ai_microcore-3.7.0/microcore/llm/_openai_llm_v0.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/llm/_openai_llm_v1.py` & `ai_microcore-3.7.0/microcore/llm/_openai_llm_v1.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/llm/anthropic.py` & `ai_microcore-3.7.0/microcore/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/llm/google_genai.py` & `ai_microcore-3.7.0/microcore/llm/google_genai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/llm/google_vertex_ai.py` & `ai_microcore-3.7.0/microcore/llm/google_vertex_ai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/llm/local_llm.py` & `ai_microcore-3.7.0/microcore/llm/local_llm.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/logging.py` & `ai_microcore-3.7.0/microcore/logging.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/templating/jinja2.py` & `ai_microcore-3.7.0/microcore/templating/jinja2.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/text2speech/elevenlabs.py` & `ai_microcore-3.7.0/microcore/text2speech/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/types.py` & `ai_microcore-3.7.0/microcore/types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/ui.py` & `ai_microcore-3.7.0/microcore/ui.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/utils.py` & `ai_microcore-3.7.0/microcore/utils.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/microcore/wrappers/llm_response_wrapper.py` & `ai_microcore-3.7.0/microcore/wrappers/llm_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/pyproject.toml` & `ai_microcore-3.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.1/PKG-INFO` & `ai_microcore-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-microcore
-Version: 3.6.1
+Version: 3.7.0
 Summary: # Minimalistic Foundation for AI Applications
 Keywords: llm,large language models,ai,similarity search,ai search,gpt,openai
 Author-email: Vitalii Stepanenko <mail@vitalii.in>
 Maintainer-email: Vitalii Stepanenko <mail@vitalii.in>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai-microcore Version: 3.6.1 Summary: # Minimalistic
+Metadata-Version: 2.1 Name: ai-microcore Version: 3.7.0 Summary: # Minimalistic
 Foundation for AI Applications Keywords: llm,large language
 models,ai,similarity search,ai search,gpt,openai Author-email: Vitalii
 Stepanenko
 vitalii.in> Maintainer-email: Vitalii Stepanenko
 vitalii.in> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

