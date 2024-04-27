# Comparing `tmp/instructor-1.2.2.tar.gz` & `tmp/instructor-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-1.2.2.tar", max compression
+gzip compressed data, was "instructor-1.2.3.tar", max compression
```

## Comparing `instructor-1.2.2.tar` & `instructor-1.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2024-04-20 01:01:31.282748 instructor-1.2.2/LICENSE
--rw-r--r--   0        0        0     9715 2024-04-20 01:01:31.282748 instructor-1.2.2/README.md
--rw-r--r--   0        0        0     1445 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/_types/__init__.py
--rw-r--r--   0        0        0      654 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/_types/_alias.py
--rw-r--r--   0        0        0        0 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/cli.py
--rw-r--r--   0        0        0     3792 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/files.py
--rw-r--r--   0        0        0     5348 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/hub.py
--rw-r--r--   0        0        0     8255 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6476 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/usage.py
--rw-r--r--   0        0        0     9666 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/client.py
--rw-r--r--   0        0        0     2453 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/client_anthropic.py
--rw-r--r--   0        0        0     2348 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/client_cohere.py
--rw-r--r--   0        0        0     1379 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/client_groq.py
--rw-r--r--   0        0        0     1709 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/client_mistral.py
--rw-r--r--   0        0        0     8968 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2985 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/citation.py
--rw-r--r--   0        0        0     7929 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2165 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2580 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    11052 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/partial.py
--rw-r--r--   0        0        0     1733 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4381 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/validators.py
--rw-r--r--   0        0        0      346 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/exceptions.py
--rw-r--r--   0        0        0     7878 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/function_calls.py
--rw-r--r--   0        0        0      852 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/mode.py
--rw-r--r--   0        0        0     4877 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/patch.py
--rw-r--r--   0        0        0    13509 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/py.typed
--rw-r--r--   0        0        0     8898 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/retry.py
--rw-r--r--   0        0        0     4860 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/utils.py
--rw-r--r--   0        0        0     2364 2024-04-20 01:01:31.350749 instructor-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    11657 1970-01-01 00:00:00.000000 instructor-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-27 17:59:46.310827 instructor-1.2.3/LICENSE
+-rw-r--r--   0        0        0     9716 2024-04-27 17:59:46.310827 instructor-1.2.3/README.md
+-rw-r--r--   0        0        0     1445 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/_types/_alias.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3792 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/files.py
+-rw-r--r--   0        0        0     5348 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8255 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6476 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/usage.py
+-rw-r--r--   0        0        0     9747 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/client.py
+-rw-r--r--   0        0        0     2453 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/client_anthropic.py
+-rw-r--r--   0        0        0     2348 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/client_cohere.py
+-rw-r--r--   0        0        0     1379 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/client_groq.py
+-rw-r--r--   0        0        0     1709 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/client_mistral.py
+-rw-r--r--   0        0        0     8968 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2985 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     7929 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2165 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2580 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    11052 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     1733 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4381 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      346 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/exceptions.py
+-rw-r--r--   0        0        0     8020 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/function_calls.py
+-rw-r--r--   0        0        0      852 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/mode.py
+-rw-r--r--   0        0        0     4877 2024-04-27 17:59:46.378827 instructor-1.2.3/instructor/patch.py
+-rw-r--r--   0        0        0    13509 2024-04-27 17:59:46.378827 instructor-1.2.3/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-04-27 17:59:46.378827 instructor-1.2.3/instructor/py.typed
+-rw-r--r--   0        0        0     9532 2024-04-27 17:59:46.378827 instructor-1.2.3/instructor/retry.py
+-rw-r--r--   0        0        0     5505 2024-04-27 17:59:46.378827 instructor-1.2.3/instructor/utils.py
+-rw-r--r--   0        0        0     2364 2024-04-27 17:59:46.378827 instructor-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    11658 1970-01-01 00:00:00.000000 instructor-1.2.3/PKG-INFO
```

### Comparing `instructor-1.2.2/LICENSE` & `instructor-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/README.md` & `instructor-1.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 [![Downloads](https://img.shields.io/pypi/dm/instructor.svg)](https://pypi.python.org/pypi/instructor)
 
 
 ## Key Features
 
 - **Response Models**: Specify Pydantic models to define the structure of your LLM outputs
 - **Retry Management**: Easily configure the number of retry attempts for your requests
-   **Validation**: Ensure LLM responses conform to your expectations with Pydantic validation
+- **Validation**: Ensure LLM responses conform to your expectations with Pydantic validation
 - **Streaming Support**: Work with Lists and Partial responses effortlessly
-   **Flexible Backends**: Seamlessly integrate with various LLM providers beyond OpenAI
+- **Flexible Backends**: Seamlessly integrate with various LLM providers beyond OpenAI
 
 ## Get Started in Minutes
 
 Install Instructor with a single command:
 
 ```bash
 pip install -U instructor
@@ -154,15 +154,15 @@
 )
 
 assert isinstance(resp, User)
 assert resp.name == "Jason"
 assert resp.age == 25
 ```
 
-## Type are infered correctly
+## Type are inferred correctly
 
 This was the dream of instructor but due to the patching of openai, it wasnt possible for me to get typing to work well. Now, with the new client, we can get typing to work well! We've also added a few `create_*` methods to make it easier to create iterables and partials, and to access the original completion.
 
 ### Calling `create`
 
 ```python
 import openai
@@ -182,15 +182,15 @@
     messages=[
         {"role": "user", "content": "Create a user"},
     ],
     response_model=User,
 )
 ```
 
-Now if you use a IDE, you can see the type is correctly infered.
+Now if you use a IDE, you can see the type is correctly inferred.
 
 ![type](./docs/blog/posts/img/type.png)
 
 ### Handling async: `await create`
 
 This will also work correctly with asynchronous clients.
 
@@ -294,15 +294,15 @@
     # name=None age=None
     # name='' age=None
     # name='John' age=None
     # name='John Doe' age=None
     # name='John Doe' age=30
 ```
 
-Notice now that the type infered is `Generator[User, None]`
+Notice now that the type inferred is `Generator[User, None]`
 
 ![generator](./docs/blog/posts/img/generator.png)
 
 ### Streaming Iterables: `create_iterable`
 
 We get an iterable of objects when we want to extract multiple objects.
```

### Comparing `instructor-1.2.2/instructor/__init__.py` & `instructor-1.2.3/instructor/__init__.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/_types/_alias.py` & `instructor-1.2.3/instructor/_types/_alias.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/cli/cli.py` & `instructor-1.2.3/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/cli/files.py` & `instructor-1.2.3/instructor/cli/files.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/cli/hub.py` & `instructor-1.2.3/instructor/cli/hub.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/cli/jobs.py` & `instructor-1.2.3/instructor/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/cli/usage.py` & `instructor-1.2.3/instructor/cli/usage.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/client.py` & `instructor-1.2.3/instructor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,18 @@
 
 
 def from_openai(
     client: Union[openai.OpenAI, openai.AsyncOpenAI],
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs,
 ) -> Instructor | AsyncInstructor:
-    provider = get_provider(str(client.base_url))
+    if hasattr(client, "base_url"):
+        provider = get_provider(str(client.base_url))
+    else:
+        provider = Provider.OPENAI
 
     assert isinstance(
         client, (openai.OpenAI, openai.AsyncOpenAI)
     ), "Client must be an instance of openai.OpenAI or openai.AsyncOpenAI"
 
     if provider in {Provider.ANYSCALE, Provider.TOGETHER}:
         assert mode in {
@@ -312,16 +315,15 @@
 
 
 @overload
 def from_litellm(
     completion: Callable,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs,
-) -> Instructor:
-    ...
+) -> Instructor: ...
 
 
 @overload
 def from_litellm(
     completion: Awaitable,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs,
```

### Comparing `instructor-1.2.2/instructor/client_anthropic.py` & `instructor-1.2.3/instructor/client_anthropic.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/client_cohere.py` & `instructor-1.2.3/instructor/client_cohere.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/client_groq.py` & `instructor-1.2.3/instructor/client_groq.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/client_mistral.py` & `instructor-1.2.3/instructor/client_mistral.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/distil.py` & `instructor-1.2.3/instructor/distil.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/dsl/citation.py` & `instructor-1.2.3/instructor/dsl/citation.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/dsl/iterable.py` & `instructor-1.2.3/instructor/dsl/iterable.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/dsl/maybe.py` & `instructor-1.2.3/instructor/dsl/maybe.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/dsl/parallel.py` & `instructor-1.2.3/instructor/dsl/parallel.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/dsl/partial.py` & `instructor-1.2.3/instructor/dsl/partial.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/dsl/simple_type.py` & `instructor-1.2.3/instructor/dsl/simple_type.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/dsl/validators.py` & `instructor-1.2.3/instructor/dsl/validators.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/function_calls.py` & `instructor-1.2.3/instructor/function_calls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from typing import Any, Dict, Optional, Type, TypeVar
-from docstring_parser import parse
+import logging
 from functools import wraps
-from pydantic import BaseModel, create_model
+from typing import Annotated, Any, Dict, Optional, Type, TypeVar
+
+from docstring_parser import parse
 from openai.types.chat import ChatCompletion
-from typing import Any, Dict, Optional, Type
-from instructor.mode import Mode
-from instructor.utils import extract_json_from_codeblock
+from pydantic import BaseModel, Field, TypeAdapter, create_model
+
 from instructor.exceptions import IncompleteOutputException
 from instructor.mode import Mode
-import logging
-
+from instructor.utils import extract_json_from_codeblock
 
 T = TypeVar("T")
 
 logger = logging.getLogger("instructor")
 
 
 class OpenAISchema(BaseModel):  # type: ignore[misc]
@@ -115,15 +114,20 @@
     @classmethod
     def parse_anthropic_tools(
         cls: Type[BaseModel],
         completion: ChatCompletion,
         validation_context: Optional[Dict[str, Any]] = None,
         strict: Optional[bool] = None,
     ) -> BaseModel:
-        tool_call = [c.input for c in completion.content if c.type == "tool_use"][0]
+        tool_calls = [c.input for c in completion.content if c.type == "tool_use"]
+
+        tool_calls_validator = TypeAdapter(
+            Annotated[list, Field(min_length=1, max_length=1)]
+        )
+        tool_call = tool_calls_validator.validate_python(tool_calls)[0]
 
         return cls.model_validate(tool_call, context=validation_context, strict=strict)  # type:ignore
 
     @classmethod
     def parse_anthropic_json(
         cls: Type[BaseModel],
         completion,
```

### Comparing `instructor-1.2.2/instructor/mode.py` & `instructor-1.2.3/instructor/mode.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/patch.py` & `instructor-1.2.3/instructor/patch.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/process_response.py` & `instructor-1.2.3/instructor/process_response.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.2/instructor/retry.py` & `instructor-1.2.3/instructor/retry.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,30 +58,35 @@
             if (
                 content.type == "tool_use"
                 and isinstance(exception, ValidationError)
                 and content.name == exception.title
             ):
                 tool_use_id = content.id
 
-        assert tool_use_id is not None, "Tool use ID not found in the response"
         yield {
             "role": "assistant",
             "content": assistant_content,
         }
-        yield {
-            "role": "user",
-            "content": [
-                {
-                    "type": "tool_result",
-                    "tool_use_id": tool_use_id,
-                    "content": f"Validation Error found:\n{exception}\nRecall the function correctly, fix the errors",
-                    "is_error": True,
-                }
-            ],
-        }
+        if tool_use_id is not None:
+            yield {
+                "role": "user",
+                "content": [
+                    {
+                        "type": "tool_result",
+                        "tool_use_id": tool_use_id,
+                        "content": f"Validation Error found:\n{exception}\nRecall the function correctly, fix the errors",
+                        "is_error": True,
+                    }
+                ],
+            }
+        else:
+            yield {
+                "role": "user",
+                "content": f"Validation Error due to no tool invocation:\n{exception}\nRecall the function correctly, fix the errors",
+            }
         return
     if mode == Mode.ANTHROPIC_JSON:
         from anthropic.types import Message
 
         assert isinstance(response, Message)
         yield {
             "role": "user",
@@ -124,14 +129,18 @@
     args,
     kwargs,
     max_retries: int | Retrying = 1,
     strict: Optional[bool] = None,
     mode: Mode = Mode.TOOLS,
 ) -> T_Model:
     total_usage = CompletionUsage(completion_tokens=0, prompt_tokens=0, total_tokens=0)
+    if mode in {Mode.ANTHROPIC_TOOLS, Mode.ANTHROPIC_JSON}:
+        from anthropic.types import Usage as AnthropicUsage
+
+        total_usage = AnthropicUsage(input_tokens=0, output_tokens=0)
 
     # If max_retries is int, then create a Retrying object
     if isinstance(max_retries, int):
         logger.debug(f"max_retries: {max_retries}")
         max_retries = Retrying(
             stop=stop_after_attempt(max_retries),
             reraise=True,
@@ -185,14 +194,19 @@
     args,
     kwargs,
     max_retries: int | AsyncRetrying = 1,
     strict: Optional[bool] = None,
     mode: Mode = Mode.TOOLS,
 ) -> T:
     total_usage = CompletionUsage(completion_tokens=0, prompt_tokens=0, total_tokens=0)
+    if mode in {Mode.ANTHROPIC_TOOLS, Mode.ANTHROPIC_JSON}:
+        from anthropic.types import Usage as AnthropicUsage
+
+        total_usage = AnthropicUsage(input_tokens=0, output_tokens=0)
+
     # If max_retries is int, then create a AsyncRetrying object
     if isinstance(max_retries, int):
         logger.debug(f"max_retries: {max_retries}")
         max_retries = AsyncRetrying(
             stop=stop_after_attempt(max_retries),
             reraise=True,
         )
@@ -223,20 +237,20 @@
                     if mode in {Mode.ANTHROPIC_TOOLS, Mode.ANTHROPIC_JSON}:
                         kwargs["messages"] = merge_consecutive_messages(
                             kwargs["messages"]
                         )
                     raise InstructorRetryException(
                         e,
                         last_completion=response,
-                        n_attempts=e.attempt_number,
+                        n_attempts=attempt.retry_state.attempt_number,
                         messages=kwargs["messages"],
                         total_usage=total_usage,
                     ) from e
     except RetryError as e:
         logger.exception(f"Failed after retries: {e.last_attempt.exception}")
         raise InstructorRetryException(
             e,
             last_completion=response,
-            n_attempts=e.attempt_number,
+            n_attempts=attempt.retry_state.attempt_number,
             messages=kwargs["messages"],
             total_usage=total_usage,
         ) from e
```

### Comparing `instructor-1.2.2/instructor/utils.py` & `instructor-1.2.3/instructor/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 import inspect
 import json
+import logging
 from typing import Callable, Generator, Iterable, AsyncGenerator, TypeVar
 
 from pydantic import BaseModel
-
+from openai.types import CompletionUsage as OpenAIUsage
 from openai.types.chat import (
     ChatCompletion,
     ChatCompletionMessage,
     ChatCompletionMessageParam,
 )
 
+logger = logging.getLogger("instructor")
 T_Model = TypeVar("T_Model", bound=BaseModel)
 
 from enum import Enum
 
 
 class Provider(Enum):
     OPENAI = "openai"
@@ -89,19 +91,35 @@
                     capturing = False
                     break  # Cease yielding upon closing the current JSON object
             elif capturing:
                 yield char
 
 
 def update_total_usage(response: T_Model, total_usage) -> T_Model | ChatCompletion:
-    if isinstance(response, ChatCompletion) and response.usage is not None:
-        total_usage.completion_tokens += response.usage.completion_tokens or 0
-        total_usage.prompt_tokens += response.usage.prompt_tokens or 0
-        total_usage.total_tokens += response.usage.total_tokens or 0
+    response_usage = getattr(response, "usage", None)
+    if isinstance(response_usage, OpenAIUsage):
+        total_usage.completion_tokens += response_usage.completion_tokens or 0
+        total_usage.prompt_tokens += response_usage.prompt_tokens or 0
+        total_usage.total_tokens += response_usage.total_tokens or 0
         response.usage = total_usage  # Replace each response usage with the total usage
+        return response
+
+    # Anthropic usage
+    try:
+        from anthropic.types import Usage as AnthropicUsage
+
+        if isinstance(response_usage, AnthropicUsage):
+            total_usage.input_tokens += response_usage.input_tokens or 0
+            total_usage.output_tokens += response_usage.output_tokens or 0
+            response.usage = total_usage
+            return response
+    except ImportError:
+        pass
+
+    logger.debug("No compatible response.usage found, token usage not updated.")
     return response
 
 
 def dump_message(message: ChatCompletionMessage) -> ChatCompletionMessageParam:
     """Dumps a message to a dict, to be returned to the OpenAI API.
     Workaround for an issue with the OpenAI API, where the `tool_calls` field isn't allowed to be present in requests
     if it isn't used.
```

### Comparing `instructor-1.2.2/pyproject.toml` & `instructor-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "instructor"
-version = "1.2.2"
+version = "1.2.3"
 description = "structured outputs for llm"
 authors = ["Jason Liu <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "instructor"}]
 repository = "https://github.com/jxnl/instructor"
```

### Comparing `instructor-1.2.2/PKG-INFO` & `instructor-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 1.2.2
+Version: 1.2.3
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -50,17 +50,17 @@
 [![Downloads](https://img.shields.io/pypi/dm/instructor.svg)](https://pypi.python.org/pypi/instructor)
 
 
 ## Key Features
 
 - **Response Models**: Specify Pydantic models to define the structure of your LLM outputs
 - **Retry Management**: Easily configure the number of retry attempts for your requests
-   **Validation**: Ensure LLM responses conform to your expectations with Pydantic validation
+- **Validation**: Ensure LLM responses conform to your expectations with Pydantic validation
 - **Streaming Support**: Work with Lists and Partial responses effortlessly
-   **Flexible Backends**: Seamlessly integrate with various LLM providers beyond OpenAI
+- **Flexible Backends**: Seamlessly integrate with various LLM providers beyond OpenAI
 
 ## Get Started in Minutes
 
 Install Instructor with a single command:
 
 ```bash
 pip install -U instructor
@@ -197,15 +197,15 @@
 )
 
 assert isinstance(resp, User)
 assert resp.name == "Jason"
 assert resp.age == 25
 ```
 
-## Type are infered correctly
+## Type are inferred correctly
 
 This was the dream of instructor but due to the patching of openai, it wasnt possible for me to get typing to work well. Now, with the new client, we can get typing to work well! We've also added a few `create_*` methods to make it easier to create iterables and partials, and to access the original completion.
 
 ### Calling `create`
 
 ```python
 import openai
@@ -225,15 +225,15 @@
     messages=[
         {"role": "user", "content": "Create a user"},
     ],
     response_model=User,
 )
 ```
 
-Now if you use a IDE, you can see the type is correctly infered.
+Now if you use a IDE, you can see the type is correctly inferred.
 
 ![type](./docs/blog/posts/img/type.png)
 
 ### Handling async: `await create`
 
 This will also work correctly with asynchronous clients.
 
@@ -337,15 +337,15 @@
     # name=None age=None
     # name='' age=None
     # name='John' age=None
     # name='John Doe' age=None
     # name='John Doe' age=30
 ```
 
-Notice now that the type infered is `Generator[User, None]`
+Notice now that the type inferred is `Generator[User, None]`
 
 ![generator](./docs/blog/posts/img/generator.png)
 
 ### Streaming Iterables: `create_iterable`
 
 We get an iterable of objects when we want to extract multiple objects.
```

