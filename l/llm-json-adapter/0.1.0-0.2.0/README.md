# Comparing `tmp/llm_json_adapter-0.1.0.tar.gz` & `tmp/llm_json_adapter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_json_adapter-0.1.0.tar", max compression
+gzip compressed data, was "llm_json_adapter-0.2.0.tar", max compression
```

## Comparing `llm_json_adapter-0.1.0.tar` & `llm_json_adapter-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,23 @@
--rw-r--r--   0        0        0     1079 2024-01-20 07:45:43.844833 llm_json_adapter-0.1.0/LICENSE
--rw-r--r--   0        0        0     2160 2024-01-24 05:22:18.627702 llm_json_adapter-0.1.0/README.md
--rw-r--r--   0        0        0      155 2024-01-24 04:55:13.720208 llm_json_adapter-0.1.0/llm_json_adapter/__init__.py
--rw-r--r--   0        0        0       98 2024-01-21 05:53:05.153009 llm_json_adapter-0.1.0/llm_json_adapter/exceptions.py
--rw-r--r--   0        0        0     3384 2024-01-24 05:23:44.121341 llm_json_adapter-0.1.0/llm_json_adapter/llm_json_adapter.py
--rw-r--r--   0        0        0       31 2024-01-24 04:54:05.611060 llm_json_adapter-0.1.0/llm_json_adapter/objects/__init__.py
--rw-r--r--   0        0        0      116 2024-01-24 04:54:05.606028 llm_json_adapter-0.1.0/llm_json_adapter/objects/response.py
--rw-r--r--   0        0        0       31 2024-01-12 07:51:42.212598 llm_json_adapter-0.1.0/llm_json_adapter/providers/__init__.py
--rw-r--r--   0        0        0       31 2024-01-12 07:51:42.215960 llm_json_adapter-0.1.0/llm_json_adapter/providers/google/__init__.py
--rw-r--r--   0        0        0     2966 2024-01-24 05:23:44.129395 llm_json_adapter-0.1.0/llm_json_adapter/providers/google/provider.py
--rw-r--r--   0        0        0       59 2024-01-12 16:42:06.032010 llm_json_adapter-0.1.0/llm_json_adapter/providers/languages.py
--rw-r--r--   0        0        0       31 2024-01-12 07:51:42.223748 llm_json_adapter-0.1.0/llm_json_adapter/providers/openai/__init__.py
--rw-r--r--   0        0        0     3081 2024-01-24 05:23:44.134104 llm_json_adapter-0.1.0/llm_json_adapter/providers/openai/provider.py
--rw-r--r--   0        0        0     1651 2024-01-24 05:23:12.906691 llm_json_adapter-0.1.0/llm_json_adapter/providers/provider.py
--rw-r--r--   0        0        0     2202 2024-01-12 07:57:47.075340 llm_json_adapter-0.1.0/llm_json_adapter/schemas/2020-12.schema.json
--rw-r--r--   0        0        0     1057 2024-02-25 05:01:45.937713 llm_json_adapter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 llm_json_adapter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-01-20 07:45:43.844833 llm_json_adapter-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7844 2024-04-27 09:50:09.674935 llm_json_adapter-0.2.0/README.md
+-rw-r--r--   0        0        0      155 2024-04-27 09:48:21.719088 llm_json_adapter-0.2.0/llm_json_adapter/__init__.py
+-rw-r--r--   0        0        0       98 2024-01-21 05:53:05.153009 llm_json_adapter-0.2.0/llm_json_adapter/exceptions.py
+-rw-r--r--   0        0        0     3859 2024-04-27 04:40:32.390147 llm_json_adapter-0.2.0/llm_json_adapter/llm_json_adapter.py
+-rw-r--r--   0        0        0       31 2024-01-24 04:54:05.611060 llm_json_adapter-0.2.0/llm_json_adapter/objects/__init__.py
+-rw-r--r--   0        0        0      116 2024-01-24 04:54:05.606028 llm_json_adapter-0.2.0/llm_json_adapter/objects/response.py
+-rw-r--r--   0        0        0       31 2024-01-12 07:51:42.212598 llm_json_adapter-0.2.0/llm_json_adapter/providers/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-26 11:52:30.754644 llm_json_adapter-0.2.0/llm_json_adapter/providers/bedrock/__init__.py
+-rw-r--r--   0        0        0     5479 2024-04-27 09:41:28.252544 llm_json_adapter-0.2.0/llm_json_adapter/providers/bedrock/provider.py
+-rw-r--r--   0        0        0       31 2024-01-12 07:51:42.215960 llm_json_adapter-0.2.0/llm_json_adapter/providers/google/__init__.py
+-rw-r--r--   0        0        0     1758 2024-04-27 06:32:24.858417 llm_json_adapter-0.2.0/llm_json_adapter/providers/google/provider.py
+-rw-r--r--   0        0        0       59 2024-01-12 16:42:06.032010 llm_json_adapter-0.2.0/llm_json_adapter/providers/languages.py
+-rw-r--r--   0        0        0       31 2024-04-26 11:52:30.757626 llm_json_adapter-0.2.0/llm_json_adapter/providers/ollama/__init__.py
+-rw-r--r--   0        0        0     1710 2024-04-27 09:38:17.272513 llm_json_adapter-0.2.0/llm_json_adapter/providers/ollama/provider.py
+-rw-r--r--   0        0        0       31 2024-01-12 07:51:42.223748 llm_json_adapter-0.2.0/llm_json_adapter/providers/openai/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-27 09:30:26.045078 llm_json_adapter-0.2.0/llm_json_adapter/providers/openai/provider.py
+-rw-r--r--   0        0        0     4300 2024-04-27 09:17:54.132300 llm_json_adapter-0.2.0/llm_json_adapter/providers/provider.py
+-rw-r--r--   0        0        0     2202 2024-01-12 07:57:47.075340 llm_json_adapter-0.2.0/llm_json_adapter/schemas/2020-12.schema.json
+-rw-r--r--   0        0        0       38 2024-04-26 12:32:08.952374 llm_json_adapter-0.2.0/llm_json_adapter/utilities/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-27 09:10:38.744499 llm_json_adapter-0.2.0/llm_json_adapter/utilities/json_utility.py
+-rw-r--r--   0        0        0     1093 2024-04-27 09:48:40.789767 llm_json_adapter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8294 1970-01-01 00:00:00.000000 llm_json_adapter-0.2.0/PKG-INFO
```

### Comparing `llm_json_adapter-0.1.0/LICENSE` & `llm_json_adapter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_json_adapter-0.1.0/llm_json_adapter/llm_json_adapter.py` & `llm_json_adapter-0.2.0/llm_json_adapter/llm_json_adapter.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,14 +33,22 @@
             from .providers.google import Provider as GoogleProvider
             return GoogleProvider(logger=self._logger,
                                   attributes=self._attributes)
         elif provider_name.lower() == 'openai':
             from .providers.openai import Provider as OpenAIProvider
             return OpenAIProvider(logger=self._logger,
                                   attributes=self._attributes)
+        elif provider_name.lower() == 'ollama':
+            from .providers.ollama import Provider as OllamaProvider
+            return OllamaProvider(logger=self._logger,
+                                  attributes=self._attributes)
+        elif provider_name.lower() == 'bedrock':
+            from .providers.bedrock import Provider as BedrockProvider
+            return BedrockProvider(logger=self._logger,
+                                   attributes=self._attributes)
         else:
             raise Exception(f'Unknown provider: {provider_name}')
 
     @staticmethod
     def validate_jsonschema(json_schema: dict) -> bool:
         meta_schema_path = Path(
             __file__).parent / 'schemas' / '2020-12.schema.json'
```

### Comparing `llm_json_adapter-0.1.0/llm_json_adapter/providers/google/provider.py` & `llm_json_adapter-0.2.0/llm_json_adapter/providers/google/provider.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-import json
 import logging
-import re
 from typing import Dict, Optional
 
 import google.generativeai as genai
 from google.generativeai.generative_models import GenerativeModel
 
 from ...exceptions import RetryableError
 from ...objects import Response
-from ..languages import languages
+from ...utilities import JsonUtility
 from ..provider import Provider as BaseProvider
 
 
 class Provider(BaseProvider):
     _required_attributes = {
         'api_key': None,
-        'model': 'gemini-pro',
+        'model': 'gemini-1.5-pro-latest',
     }
 
     def __init__(self,
                  logger: Optional[logging.Logger] = None,
                  attributes: Optional[Dict] = None):
         super().__init__(logger=logger, attributes=attributes)
         self._client = self.get_client()
@@ -27,46 +25,14 @@
     def get_client(self) -> GenerativeModel:
         genai.configure(
             api_key=self.get_attribute('api_key', default_value=None))
         model = genai.GenerativeModel(
             model_name=self.get_attribute('model', default_value=None))
         return model
 
-    def generate_prompt(self,
-                        prompt: str,
-                        function: Response,
-                        language: str = "en",
-                        act_as: Optional[str] = None) -> str:
-        generated_prompt = prompt + "\n\n"
-
-        if act_as is not None:
-            generated_prompt += f"Please answer as {act_as}.\n\n"
-
-        full_language = self.set_language(language)
-        if full_language is not None:
-            full_language = languages[language]
-            generated_prompt += f"Response should be in {full_language}.\n\n"
-
-        json_format = json.dumps(function.parameters)
-        generated_prompt += (
-            f"And use Json format as the response format which defined as following: \n\n"
-            f"\n{json_format}\n\n")
-
-        generated_prompt += "and response json data should be wrapped by the markdown code block\n\n"
-        return generated_prompt
-
-    @staticmethod
-    def extract_json_block(text: str) -> Optional[Dict]:
-        pattern = r'```(.*?)\n(.*?)```'
-        code_blocks = re.findall(pattern, text, re.DOTALL)
-        if len(code_blocks) == 0:
-            return None
-        json_data = code_blocks[0][1]
-        return json.loads(json_data)
-
     async def generate(self,
                        prompt: str,
                        function: Response,
                        language: str = "en",
                        act_as: Optional[str] = None) -> Optional[Dict]:
 
         generated_prompt = self.generate_prompt(
@@ -75,14 +41,15 @@
             language=language,
             act_as=act_as,
         )
 
         try:
             response = self._client.generate_content(generated_prompt)
         except Exception as e:
+            print(e)
             raise RetryableError(f"Google API exception: {e}")
 
-        result = self.extract_json_block(response.text)
+        result = JsonUtility.extract_json_block(text=response.text)
         if not isinstance(result, dict):
             raise RetryableError('Failed to extract json block')
 
         return result
```

### Comparing `llm_json_adapter-0.1.0/llm_json_adapter/providers/openai/provider.py` & `llm_json_adapter-0.2.0/llm_json_adapter/providers/openai/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ..languages import languages
 from ..provider import Provider as BaseProvider
 
 
 class Provider(BaseProvider):
     _required_attributes = {
         'api_key': None,
-        'model': 'gpt-3.5-turbo-1106',
+        'model': 'gpt-3.5-turbo',
         'temperature': 0.67,
         'presence_penalty': 0.0,
         'frequency_penalty': 0.0,
     }
 
     def __init__(self,
                  logger: Optional[logging.Logger] = None,
```

### Comparing `llm_json_adapter-0.1.0/llm_json_adapter/schemas/2020-12.schema.json` & `llm_json_adapter-0.2.0/llm_json_adapter/schemas/2020-12.schema.json`

 * *Files identical despite different names*

### Comparing `llm_json_adapter-0.1.0/pyproject.toml` & `llm_json_adapter-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-json-adapter"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name="Takaaki Mizuno" },
 ]
 description = "Wrapper library to switch LLMs and get results in JSON"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -15,30 +15,31 @@
 
 [project.urls]
 Homepage = "https://github.com/takaaki-mizuno/python-llm-json-adapter"
 Issues = "https://github.com/takaaki-mizuno/python-llm-json-adapter/issues"
 
 [tool.poetry]
 name = "llm-json-adapter"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Takaaki Mizuno"]
 readme = "README.md"
 packages = [{include = "llm_json_adapter"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-openai = "^1.12.0"
-google-generativeai = "^0.3.2"
 jsonschema = "^4.20.0"
 pydantic = "^2.5.3"
 
-
 [tool.poetry.group.dev.dependencies]
 toml = "^0.10.2"
+openai = "^1.12.0"
+google-generativeai = "^0.5.2"
+ollama = "^0.1.9"
+boto3 = "^1.34.93"
 python-dotenv = "^1.0.0"
 pytest = "^7.4.4"
 yapf = "^0.40.2"
 isort = "^5.13.2"
 
 [build-system]
 requires = ["poetry-core"]
```

