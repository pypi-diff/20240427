# Comparing `tmp/banks-0.2.0.tar.gz` & `tmp/banks-0.3.0.tar.gz`

## Comparing `banks-0.2.0.tar` & `banks-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 banks-0.2.0/MANIFEST.in
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 banks-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 banks-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 banks-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 banks-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 banks-0.2.0/docs/extensions.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 banks-0.2.0/docs/filters.md
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 banks-0.2.0/docs/index.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 banks-0.2.0/docs/macros.md
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 banks-0.2.0/docs/python.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/__about__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/__init__.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/env.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/errors.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/loader.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/prompt.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/extensions/__init__.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/extensions/generate.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/extensions/inference_endpoint.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/filters/__init__.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/filters/lemmatize.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/banks_macros.jinja
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/blog.jinja
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/generate_tweet.jinja
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/run_prompt.jinja
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/run_prompt_process.jinja
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/summarize.jinja
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/summarize_lemma.jinja
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 banks-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_default_templates.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_env.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_loader.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_run_prompt.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_default_templates/blog.jinja.out
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_default_templates/generate_tweet.jinja.out
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_default_templates/summarize.jinja.out
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_default_templates/summarize_lemma.jinja.out
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 banks-0.2.0/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 banks-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 banks-0.2.0/README.md
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 banks-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 banks-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 banks-0.3.0/MANIFEST.in
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 banks-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 banks-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 banks-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 banks-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 banks-0.3.0/docs/async.md
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 banks-0.3.0/docs/index.md
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 banks-0.3.0/docs/prompt.md
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 banks-0.3.0/docs/python.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/__about__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/__init__.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/env.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/errors.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/loader.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/prompt.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/extensions/__init__.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/extensions/generate.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/extensions/inference_endpoint.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/filters/__init__.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/filters/lemmatize.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/templates/banks_macros.jinja
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/templates/blog.jinja
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/templates/generate_tweet.jinja
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/templates/run_prompt.jinja
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/templates/run_prompt_process.jinja
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/templates/summarize.jinja
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 banks-0.3.0/src/banks/templates/summarize_lemma.jinja
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 banks-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 banks-0.3.0/tests/test_default_templates.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 banks-0.3.0/tests/test_env.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 banks-0.3.0/tests/test_loader.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 banks-0.3.0/tests/test_run_prompt.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 banks-0.3.0/tests/test_default_templates/blog.jinja.out
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 banks-0.3.0/tests/test_default_templates/generate_tweet.jinja.out
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 banks-0.3.0/tests/test_default_templates/summarize.jinja.out
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 banks-0.3.0/tests/test_default_templates/summarize_lemma.jinja.out
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 banks-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 banks-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 banks-0.3.0/README.md
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 banks-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 banks-0.3.0/PKG-INFO
```

### Comparing `banks-0.2.0/mkdocs.yml` & `banks-0.3.0/mkdocs.yml`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,17 @@
   name: material
   palette:
     primary: amber
     scheme: slate
 
 nav:
   - Home: 'index.md'
-  - filters.md
-  - extensions.md
-  - macros.md
   - Python API: 'python.md'
+  - Prompt API: 'prompt.md'
+  - asyncio support: 'async.md'
 
 plugins:
   - search
   - mkdocstrings:
       handlers:
         python:
           paths: [src]
```

### Comparing `banks-0.2.0/.github/workflows/docs.yml` & `banks-0.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/.github/workflows/test.yml` & `banks-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/docs/index.md` & `banks-0.3.0/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 specifically designed to work with Large Language Models prompts. Similar to other template languages, Banks takes
 in input a generic piece of text called _template_ and gives you back its _rendered_ version, where the generic bits
 are replaced by actual data provided by the user.
 
 ## Features
 
 * Banks currently supports all the features from Jinja2, see [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/#jinja-filters.truncate).
-* [Filters](filters.md): useful to manipulate the text during template rendering.
-* [Extensions](extensions.md): useful to support custom functions (e.g. text generation via OpenAI).
-* [Macros](macros.md): useful to implement complex logic in the template itself instead of Python code.
+* [Filters](prompt.md#filters): useful to manipulate the text during template rendering.
+* [Extensions](prompt.md#extensions): useful to support custom functions (e.g. text generation via OpenAI).
+* [Macros](prompt.md#macros): useful to implement complex logic in the template itself instead of Python code.
 
 ## Installation
 
 Install the latest version of Banks using `pip`:
 
 ```sh
 pip install banks
```

### Comparing `banks-0.2.0/docs/python.md` & `banks-0.3.0/docs/python.md`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/src/banks/env.py` & `banks-0.3.0/src/banks/env.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # SPDX-FileCopyrightText: 2023-present Massimiliano Pippi <mpippi@gmail.com>
 #
 # SPDX-License-Identifier: MIT
+import os
+from distutils.util import strtobool
+
 from jinja2 import Environment, select_autoescape
 
 from banks.extensions import GenerateExtension, HFInferenceEndpointsExtension
 from banks.filters import lemmatize
 from banks.loader import MultiLoader
 
+async_enabled = strtobool(os.environ.get("BANKS_ASYNC_ENABLED", "false"))
+
 # Init the Jinja env
 env = Environment(
     loader=MultiLoader(),
     extensions=[GenerateExtension, HFInferenceEndpointsExtension],
     autoescape=select_autoescape(
         enabled_extensions=("html", "xml"),
-        default_for_string=True,
+        default_for_string=False,
     ),
     trim_blocks=True,
     lstrip_blocks=True,
+    enable_async=bool(async_enabled),
 )
 
 # Setup custom filters
 env.filters["lemmatize"] = lemmatize
 
 
 def with_env(cls):
```

### Comparing `banks-0.2.0/src/banks/loader.py` & `banks-0.3.0/src/banks/loader.py`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/src/banks/extensions/generate.py` & `banks-0.3.0/src/banks/extensions/generate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # SPDX-FileCopyrightText: 2023-present Massimiliano Pippi <mpippi@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 from typing import cast
 
 from jinja2 import nodes
 from jinja2.ext import Extension
-from litellm import ModelResponse, completion
+from litellm import ModelResponse, completion, acompletion
 
 DEFAULT_MODEL = "gpt-3.5-turbo"
 
 
 class GenerateExtension(Extension):
     """
-    `generate` can be used to call the OpenAI API passing the tag text as a prompt and get back some content.
+    `generate` can be used to call the LiteLLM API passing the tag text as a prompt and get back some content.
 
     Example:
         ```
         {% generate "write a tweet with positive sentiment" "gpt-3.5-turbo" %}
         Feeling grateful for all the opportunities that come my way! #positivity #productivity
         ```
     """
@@ -30,22 +30,45 @@
         lineno = next(parser.stream).lineno
 
         # The args passed to the extension:
         # - the prompt text used to generate new text
         # - (optional) the name of the model use to generate new text
         args = [parser.parse_expression()]
 
+        # If there is a comma, the user provided the model name. If not, use
+        # None as the second parameter.
+        if parser.stream.skip_if("comma"):
+            args.append(parser.parse_expression())
+        else:
+            args.append(nodes.Const(None))
+
+        if parser.environment.is_async:
+            return nodes.Output([self.call_method("_agenerate", args)]).set_lineno(lineno)
         return nodes.Output([self.call_method("_generate", args)]).set_lineno(lineno)
 
     def _generate(self, text, model_name=DEFAULT_MODEL):
         """
         Helper callback.
 
         To tweak the prompt used to generate content, change the variable `messages` .
         """
         messages = [
             {"role": "system", "content": "You are a helpful assistant."},
             {"role": "user", "content": text},
         ]
-
         response: ModelResponse = cast(ModelResponse, completion(model=model_name, messages=messages))
         return response["choices"][0]["message"]["content"]
+
+    async def _agenerate(self, text, model_name=DEFAULT_MODEL):
+        """
+        Helper callback.
+
+        To tweak the prompt used to generate content, change the variable `messages` .
+        """
+        print(f"Running {text} with {model_name}")
+        messages = [
+            {"role": "system", "content": "You are a helpful assistant."},
+            {"role": "user", "content": text},
+        ]
+        response: ModelResponse = cast(ModelResponse, await acompletion(model=model_name, messages=messages))
+        print(f"Done running {model_name}")
+        return response["choices"][0]["message"]["content"]
```

### Comparing `banks-0.2.0/src/banks/extensions/inference_endpoint.py` & `banks-0.3.0/src/banks/extensions/inference_endpoint.py`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/src/banks/filters/lemmatize.py` & `banks-0.3.0/src/banks/filters/lemmatize.py`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/tests/test_default_templates.py` & `banks-0.3.0/tests/test_default_templates.py`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/tests/test_loader.py` & `banks-0.3.0/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/tests/test_run_prompt.py` & `banks-0.3.0/tests/test_run_prompt.py`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/.gitignore` & `banks-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/LICENSE.txt` & `banks-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/README.md` & `banks-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 [![docs](https://github.com/masci/banks/actions/workflows/docs.yml/badge.svg)](https://github.com/masci/banks/actions/workflows/docs.yml)
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[Banks](https://en.wikipedia.org/wiki/Arrival_(film)) is the linguist professor who will help you generate meaningful LLM prompts using a template language that makes sense.
-If you're still using `f-strings` for the job, keep reading.
+[Banks](https://en.wikipedia.org/wiki/Arrival_(film)) is the linguist professor who will help you generate meaningful
+LLM prompts using a template language that makes sense. If you're still using `f-strings` for the job, keep reading.
 
-> Docs are currently in the pipes and at the moment this README is the best resource for Banks' users, anyways they are
-> available [here](https://masci.github.io/banks/)
+Docs are available [here](https://masci.github.io/banks/).
 
 -----
 
 **Table of Contents**
 
 - [banks](#banks)
   - [Installation](#installation)
@@ -28,14 +27,15 @@
     - [Generate a blog writing prompt](#generate-a-blog-writing-prompt)
     - [Generate a summarizer prompt](#generate-a-summarizer-prompt)
     - [Lemmatize text while processing a template](#lemmatize-text-while-processing-a-template)
     - [Use a LLM to generate a text while rendering a prompt](#use-a-llm-to-generate-a-text-while-rendering-a-prompt)
     - [Go meta: create a prompt and `generate` its response](#go-meta-create-a-prompt-and-generate-its-response)
     - [Go meta(meta): process a LLM response](#go-metameta-process-a-llm-response)
     - [Reuse templates from files](#reuse-templates-from-files)
+    - [Async support](#async-support)
   - [License](#license)
 
 ## Installation
 
 ```console
 pip install banks
 ```
@@ -185,16 +185,17 @@
 ```
 
 If you paste Banks' output into ChatGPT you would get something like this:
 ```txt
 Climate change is a pressing global issue, but together we can create positive change! Let's embrace renewable energy, protect our planet, and build a sustainable future for generations to come. 🌍💚 #ClimateAction #PositiveFuture
 ```
 
-The `generate` extension uses [LiteLLM](https://github.com/BerriAI/litellm) under the hood, and provided you have the
-proper environment variables set, you can use any model from the supported [model providers](https://docs.litellm.ai/docs/providers).
+> [!TIP]
+> The `generate` extension uses [LiteLLM](https://github.com/BerriAI/litellm) under the hood, and provided you have the
+> proper environment variables set, you can use any model from the supported [model providers](https://docs.litellm.ai/docs/providers).
 
 ### Go meta: create a prompt and `generate` its response
 
 We can leverage Jinja's macro system to generate a prompt, send the result to OpenAI and get a response.
 Let's bring back the blog writing example:
 
 ```py
@@ -272,10 +273,28 @@
 
 
 p = Prompt.from_template("blog.jinja")
 topic = "retrogame computing"
 print(p.text({"topic": topic}))
 ```
 
+### Async support
+
+To run banks within an `asyncio` loop you have to do two things:
+1. set the environment variable `BANKS_ASYNC_ENABLED=true`.
+2. use the `AsyncPrompt` class that has an awaitable `run` method.
+
+Example:
+```python
+from banks import AsyncPrompt
+
+async def main():
+    p = AsyncPrompt.from_template("blog.jinja")
+    result = await p.text({"topic": "AI frameworks"})
+    print(result)
+
+asyncio.run(main())
+```
+
 ## License
 
 `banks` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `banks-0.2.0/pyproject.toml` & `banks-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `banks-0.2.0/PKG-INFO` & `banks-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: banks
-Version: 0.2.0
+Version: 0.3.0
 Summary: A prompt programming language
 Project-URL: Documentation, https://github.com/unknown/banks#readme
 Project-URL: Issues, https://github.com/unknown/banks/issues
 Project-URL: Source, https://github.com/unknown/banks
 Author-email: Massimiliano Pippi <mpippi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -32,19 +32,18 @@
 [![docs](https://github.com/masci/banks/actions/workflows/docs.yml/badge.svg)](https://github.com/masci/banks/actions/workflows/docs.yml)
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[Banks](https://en.wikipedia.org/wiki/Arrival_(film)) is the linguist professor who will help you generate meaningful LLM prompts using a template language that makes sense.
-If you're still using `f-strings` for the job, keep reading.
+[Banks](https://en.wikipedia.org/wiki/Arrival_(film)) is the linguist professor who will help you generate meaningful
+LLM prompts using a template language that makes sense. If you're still using `f-strings` for the job, keep reading.
 
-> Docs are currently in the pipes and at the moment this README is the best resource for Banks' users, anyways they are
-> available [here](https://masci.github.io/banks/)
+Docs are available [here](https://masci.github.io/banks/).
 
 -----
 
 **Table of Contents**
 
 - [banks](#banks)
   - [Installation](#installation)
@@ -52,14 +51,15 @@
     - [Generate a blog writing prompt](#generate-a-blog-writing-prompt)
     - [Generate a summarizer prompt](#generate-a-summarizer-prompt)
     - [Lemmatize text while processing a template](#lemmatize-text-while-processing-a-template)
     - [Use a LLM to generate a text while rendering a prompt](#use-a-llm-to-generate-a-text-while-rendering-a-prompt)
     - [Go meta: create a prompt and `generate` its response](#go-meta-create-a-prompt-and-generate-its-response)
     - [Go meta(meta): process a LLM response](#go-metameta-process-a-llm-response)
     - [Reuse templates from files](#reuse-templates-from-files)
+    - [Async support](#async-support)
   - [License](#license)
 
 ## Installation
 
 ```console
 pip install banks
 ```
@@ -209,16 +209,17 @@
 ```
 
 If you paste Banks' output into ChatGPT you would get something like this:
 ```txt
 Climate change is a pressing global issue, but together we can create positive change! Let's embrace renewable energy, protect our planet, and build a sustainable future for generations to come. 🌍💚 #ClimateAction #PositiveFuture
 ```
 
-The `generate` extension uses [LiteLLM](https://github.com/BerriAI/litellm) under the hood, and provided you have the
-proper environment variables set, you can use any model from the supported [model providers](https://docs.litellm.ai/docs/providers).
+> [!TIP]
+> The `generate` extension uses [LiteLLM](https://github.com/BerriAI/litellm) under the hood, and provided you have the
+> proper environment variables set, you can use any model from the supported [model providers](https://docs.litellm.ai/docs/providers).
 
 ### Go meta: create a prompt and `generate` its response
 
 We can leverage Jinja's macro system to generate a prompt, send the result to OpenAI and get a response.
 Let's bring back the blog writing example:
 
 ```py
@@ -296,10 +297,28 @@
 
 
 p = Prompt.from_template("blog.jinja")
 topic = "retrogame computing"
 print(p.text({"topic": topic}))
 ```
 
+### Async support
+
+To run banks within an `asyncio` loop you have to do two things:
+1. set the environment variable `BANKS_ASYNC_ENABLED=true`.
+2. use the `AsyncPrompt` class that has an awaitable `run` method.
+
+Example:
+```python
+from banks import AsyncPrompt
+
+async def main():
+    p = AsyncPrompt.from_template("blog.jinja")
+    result = await p.text({"topic": "AI frameworks"})
+    print(result)
+
+asyncio.run(main())
+```
+
 ## License
 
 `banks` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

