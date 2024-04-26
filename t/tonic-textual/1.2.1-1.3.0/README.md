# Comparing `tmp/tonic_textual-1.2.1.tar.gz` & `tmp/tonic_textual-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_textual-1.2.1.tar", max compression
+gzip compressed data, was "tonic_textual-1.3.0.tar", max compression
```

## Comparing `tonic_textual-1.2.1.tar` & `tonic_textual-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1084 2023-08-21 15:18:32.578537 tonic_textual-1.2.1/LICENSE
--rw-r--r--   0        0        0      598 2024-04-16 20:46:13.943637 tonic_textual-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      972 2023-11-03 19:05:54.671774 tonic_textual-1.2.1/README.md
--rw-r--r--   0        0        0       19 2024-04-16 20:46:34.697498 tonic_textual-1.2.1/tonic_textual/__init__.py
--rw-r--r--   0        0        0    14228 2024-04-16 14:31:27.775440 tonic_textual-1.2.1/tonic_textual/api.py
--rw-r--r--   0        0        0        0 2023-11-03 19:05:54.674583 tonic_textual-1.2.1/tonic_textual/classes/__init__.py
--rw-r--r--   0        0        0      789 2023-11-15 15:30:22.056092 tonic_textual-1.2.1/tonic_textual/classes/api_responses/redaction_response.py
--rw-r--r--   0        0        0      668 2024-02-28 13:39:57.539026 tonic_textual-1.2.1/tonic_textual/classes/api_responses/single_detection_result.py
--rw-r--r--   0        0        0      348 2024-04-16 14:31:52.343889 tonic_textual-1.2.1/tonic_textual/classes/custom_model.py
--rw-r--r--   0        0        0     8183 2024-04-16 14:27:25.096645 tonic_textual-1.2.1/tonic_textual/classes/dataset.py
--rw-r--r--   0        0        0     1633 2023-11-14 22:48:18.528603 tonic_textual-1.2.1/tonic_textual/classes/datasetfile.py
--rw-r--r--   0        0        0       95 2023-11-03 19:05:54.674583 tonic_textual-1.2.1/tonic_textual/classes/generator_config.py
--rw-r--r--   0        0        0     4684 2024-04-16 20:44:13.013231 tonic_textual-1.2.1/tonic_textual/classes/httpclient.py
--rw-r--r--   0        0        0     1864 2024-04-16 14:27:25.098640 tonic_textual-1.2.1/tonic_textual/classes/tonic_exception.py
--rw-r--r--   0        0        0       92 2023-11-03 19:05:54.674583 tonic_textual-1.2.1/tonic_textual/enums/pii_state.py
--rw-r--r--   0        0        0        0 2023-11-03 19:05:54.674583 tonic_textual-1.2.1/tonic_textual/services/__init__.py
--rw-r--r--   0        0        0      610 2023-11-03 19:05:54.674583 tonic_textual-1.2.1/tonic_textual/services/dataset.py
--rw-r--r--   0        0        0      552 2023-11-03 19:05:54.674583 tonic_textual-1.2.1/tonic_textual/services/datasetfile.py
--rw-r--r--   0        0        0     1885 1970-01-01 00:00:00.000000 tonic_textual-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-02-17 17:17:54.164782 tonic_textual-1.3.0/LICENSE
+-rw-r--r--   0        0        0      972 2024-02-17 17:17:54.164871 tonic_textual-1.3.0/README.md
+-rw-r--r--   0        0        0      598 2024-04-26 22:23:38.075685 tonic_textual-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       19 2024-04-26 22:23:38.076054 tonic_textual-1.3.0/tonic_textual/__init__.py
+-rw-r--r--   0        0        0    16432 2024-04-26 22:23:38.076252 tonic_textual-1.3.0/tonic_textual/api.py
+-rw-r--r--   0        0        0        0 2024-02-17 17:17:54.168806 tonic_textual-1.3.0/tonic_textual/classes/__init__.py
+-rw-r--r--   0        0        0      789 2024-02-17 17:17:54.168921 tonic_textual-1.3.0/tonic_textual/classes/api_responses/redaction_response.py
+-rw-r--r--   0        0        0      668 2024-02-23 23:38:13.865340 tonic_textual-1.3.0/tonic_textual/classes/api_responses/single_detection_result.py
+-rw-r--r--   0        0        0      348 2024-02-17 17:17:54.169331 tonic_textual-1.3.0/tonic_textual/classes/custom_model.py
+-rw-r--r--   0        0        0     8183 2024-04-19 18:36:12.557423 tonic_textual-1.3.0/tonic_textual/classes/dataset.py
+-rw-r--r--   0        0        0     1633 2024-02-17 17:17:54.169557 tonic_textual-1.3.0/tonic_textual/classes/datasetfile.py
+-rw-r--r--   0        0        0     4845 2024-04-26 22:23:38.076471 tonic_textual-1.3.0/tonic_textual/classes/httpclient.py
+-rw-r--r--   0        0        0     1864 2024-04-19 18:36:12.557633 tonic_textual-1.3.0/tonic_textual/classes/tonic_exception.py
+-rw-r--r--   0        0        0      121 2024-04-26 22:23:38.076887 tonic_textual-1.3.0/tonic_textual/enums/pii_state.py
+-rw-r--r--   0        0        0        0 2024-02-17 17:17:54.170004 tonic_textual-1.3.0/tonic_textual/services/__init__.py
+-rw-r--r--   0        0        0      610 2024-02-17 17:17:54.170141 tonic_textual-1.3.0/tonic_textual/services/dataset.py
+-rw-r--r--   0        0        0      552 2024-02-17 17:17:54.170230 tonic_textual-1.3.0/tonic_textual/services/datasetfile.py
+-rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 tonic_textual-1.3.0/PKG-INFO
```

### Comparing `tonic_textual-1.2.1/LICENSE` & `tonic_textual-1.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 TOИIC
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 TOИIC
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `tonic_textual-1.2.1/pyproject.toml` & `tonic_textual-1.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tonic-textual"
-version = "1.2.1"
+version = "1.3.0"
 description = "Wrappers around the Tonic Textual API"
 authors = ["Adam Kamor <adam@tonic.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.tonic.ai/"
 keywords = ["tonic.ai", "tonic", "tonic textual"]
```

### Comparing `tonic_textual-1.2.1/README.md` & `tonic_textual-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.2.1/tonic_textual/api.py` & `tonic_textual-1.3.0/tonic_textual/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import io
 import json
 import os
 import requests
 
 from time import sleep
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Dict
 from urllib.parse import urlencode
 
-from tqdm.utils import CallbackIOWrapper
-from tqdm import tqdm
 from tonic_textual.classes.api_responses.single_detection_result import SingleDetectionResult
 from tonic_textual.classes.custom_model import CustomModel
-from tonic_textual.classes.generator_config import GeneratorConfig
 from tonic_textual.classes.httpclient import HttpClient
 from tonic_textual.classes.api_responses.redaction_response import RedactionResponse
 from tonic_textual.enums.pii_state import PiiState
 from tonic_textual.services.dataset import DatasetService
 from tonic_textual.services.datasetfile import DatasetFileService
 from tonic_textual.classes.dataset import Dataset
 from tonic_textual.classes.datasetfile import DatasetFile
@@ -26,28 +23,38 @@
 
     Parameters
     ----------
     base_url : str
         The URL to your Tonic Textual instance. Do not include trailing backslashes.
     api_key : str
         Your API token. This argument is optional. Instead of providing the API token here, it is recommended that you set the API key in your environment as the value of TONIC_TEXTUAL_API_KEY.
-
+    verify: bool
+        Whether SSL Certification verification is performed.  This is enabled by default.
     Examples
     --------
     >>> TonicTextual("http://localhost:3000")
     '''
-    def __init__(self, base_url : str, api_key: Optional[str] = None):
+    def __init__(self, base_url : str, api_key: Optional[str] = None, verify: bool = True):
         if api_key is None:
             api_key = os.environ.get("TONIC_TEXTUAL_API_KEY")
             if api_key is None:
                 raise Exception("No API key provided. Either provide an API key, or set the API key as the value of the TONIC_TEXTUAL_API_KEY environment variable.")
         self.api_key = api_key
-        self.client = HttpClient(base_url, self.api_key)
+        self.client = HttpClient(base_url, self.api_key, verify)
         self.dataset_service = DatasetService(self.client)
         self.datasetfile_service = DatasetFileService(self.client)
+        self.verify = verify
+
+    @staticmethod
+    def _validate_generator_options(generator_default: PiiState, generator_config: Dict[str, PiiState]) -> None:
+        invalid_pii_states = [v for v in list(generator_config.values()) if v not in PiiState._member_names_]
+        if(len(invalid_pii_states)>0):
+            raise Exception("Invalid configuration for generator_config. The allowed values are Off, Synthesis, and Redaction.")
+        if generator_default not in PiiState._member_names_:
+            raise Exception("Invalid option for generator_default. The allowed values are Off, Synthesis, and Redaction.")
 
     def create_dataset(self, dataset_name:str):
         """Creates a dataset. A dataset is a collection of 1 or more files for Tonic Textual to scan and redact.
 
         Parameters
         -----
         dataset_name : str
@@ -106,140 +113,176 @@
 
         Returns
         ------
         List[DatasetFile]
         A list of all of the files in the dataset.
         """
         return self.datasetfile_service.get_files(dataset_id)
-      
+
     def unredact_bulk(self, redacted_strings: List[str]) -> List[str]:
             """Removes redaction from a list of strings. Returns the strings with the original values.
-            
+
             Parameters
             ----------
             redacted_strings : List[str]
                 The list of redacted strings from which to remove the redaction.
-    
+
             Returns
             -------
             List[str]
                 The list of strings with the redaction removed.
             """
-            
-            response = self.client.http_post("/api/unredact", data=redacted_strings)            
+
+            response = self.client.http_post("/api/unredact", data=redacted_strings)
             return response
-    
+
     def unredact(self, redacted_string: str) -> str:
             """Removes the redaction from a provided string. Returns the string with the original values.
-            
+
             Parameters
             ----------
             redacted_string : str
                 The redacted string from which to remove the redaction.
-    
+
             Returns
             -------
             str
                 The string with the redaction removed.
             """
-            
-            response = self.client.http_post("/api/unredact", data=[redacted_string])            
+
+            response = self.client.http_post("/api/unredact", data=[redacted_string])
             return response
-    
-    def redact(self, string: str, generator_config: GeneratorConfig = dict(), custom_models: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:
+
+    def redact(self, string: str, generator_config: Dict[str, PiiState] = dict(), generator_default: PiiState = PiiState.Redaction, custom_models: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:
             """Redacts a string. Depending on the configured handling for each sensitive data type, values can be either redacted, synthesized, or ignored.
-            
+
             Parameters
             ----------
             string : str
                 The string to redact.
-            
-            generator_config: GeneratorConfig
+
+            generator_config: Dict[str, PiiState]
                 A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
-    
-            custom_models: List[str]
+                Values must be one of "Redaction", "Synthesis", or "Off".
+
+            generator_default: PiiState = PiiState.Redaction
+                The default redaction used for all types not specified in generator_config.
+                Values must be one of "Redaction", "Synthesis", or "Off".
+
+            custom_models: List[str] = []
                 A list of custom model names to use to identify values to redact. To see the list of custom models that you have access to, use the get_custom_models function.
-            
-            random_seed: Optional[int]
+
+            random_seed: Optional[int] = None
                 An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
-                
+
             Returns
             -------
             RedactionResponse
                 The redacted string along with ancillary information.
+
+            Examples
+            --------
+                >>> textual.redact("John Smith is a person", generator_config= {"NAME_GIVEN": "Redaction"}, generator_default="Off") # only redacts NAME_GIVEN
+
             """
-            
-            invalid_pii_states = [v for v in list(generator_config.values()) if v not in PiiState._member_names_]
-            if(len(invalid_pii_states)>0):
-                 raise Exception("Invalid configuration for generatorConfig. The allowed values are Off, Synthesis, and Redaction.")                 
 
+            self._validate_generator_options(generator_default, generator_config)
             endpoint = "/api/redact"
 
-            if random_seed is not None:                 
-                response = self.client.http_post(endpoint, data={"text": string, "generatorConfig": generator_config, "customModels": custom_models}, additionalHeaders={'textual-random-seed':str(random_seed)})
+            if random_seed is not None:
+                additional_headers = {'textual-random-seed':str(random_seed)}
             else:
-                response = self.client.http_post(endpoint, data={"text": string, "generatorConfig": generator_config, "customModels": custom_models})
-            
+                additional_headers = {}
+                
+            response = self.client.http_post(endpoint, data={"text": string, "generatorDefault": generator_default, "generatorConfig": generator_config, "customModels": custom_models}, additional_headers=additional_headers)
             de_id_results = [SingleDetectionResult(x["start"], x["end"], x["label"], x["text"], x["score"]) for x in list(response["deIdentifyResults"])]
 
             return RedactionResponse(response["originalText"], response["redactedText"], response["usage"], de_id_results)
-    
-    def redact_json(self, json_data: Union[str, dict], generator_config: GeneratorConfig = dict(), custom_models: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:   
+
+    def llm_synthesis(self, string: str, generator_config: Dict[str, PiiState] = dict(), generator_default: PiiState = PiiState.Redaction) -> RedactionResponse:
+        """Deidentifies a string by redacting sensitive data and replacing these values with values generated by an LLM.
+
+        Parameters
+        ----------
+        string : str
+                The string to redact.
+
+        generator_config: Dict[str, PiiState]
+                A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
+
+        generator_default: PiiState = PiiState.Redaction
+            The default redaction used for all types not specified in generator_config.
+
+       Returns
+        -------
+                The de-identified string
+        """
+        self._validate_generator_options(generator_default, generator_config)
+        endpoint = "/api/synthesis"
+        response = self.client.http_post(endpoint, data={"text": string, "generatorDefault": generator_default, "generatorConfig": generator_config})
+
+        de_id_results = [SingleDetectionResult(x["start"], x["end"], x["label"], x["text"], x["score"]) for x in
+                         list(response["deIdentifyResults"])]
+
+        return RedactionResponse(response["originalText"], response["redactedText"], response["usage"], de_id_results)
+
+    def redact_json(self, json_data: Union[str, dict], generator_config:Dict[str, PiiState] = dict(), generator_default: PiiState = PiiState.Redaction, custom_models: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:
         """Redacts the values in a JSON blob. Depending on the configured handling for each sensitive data type, values can be either redacted, synthesized, or ignored.
-        
+
         Parameters
         ----------
         json_string : Union[str, dict]
             The JSON whose values will be redacted.  This can be either a JSON string or a Python dictionary
-        
-        generator_config: GeneratorConfig
-            A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
 
-        custom_models: List[str]
+        generator_config: Dict[str, PiiState]
+                A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
+
+        generator_default: PiiState = PiiState.Redaction
+                The default redaction used for all types not specified in generator_config.
+
+        custom_models: List[str] = []
             A list of custom model names to use to identify values to redact. To see the list of custom models that you have access to, use the get_custom_models function.
 
-        random_seed: Optional[int]
-            An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.            
+        random_seed: Optional[int] = None
+            An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
 
         Returns
         -------
         RedactionResponse
             The redacted string along with ancillary information.
         """
-        
-        invalid_pii_states = [v for v in list(generator_config.values()) if v not in PiiState._member_names_]
-        if(len(invalid_pii_states)>0):
-                raise Exception("Invalid configuration for generatorConfig. The allowed values are Off, Synthesis, and Redaction.")                 
-
+        self._validate_generator_options(generator_default, generator_config)
         endpoint = "/api/redact/json"
 
         if isinstance(json_data, str):
-             payload = {"jsonText": json_data, "generatorConfig": generator_config, "customModels": custom_models}
+            json_text = json_data
         elif isinstance(json_data, dict):
-             payload = {"jsonText": json.dumps(json_data), "generatorConfig": generator_config, "customModels": custom_models}
+            json_text = json.dumps(json_data)
         else:
             raise Exception(f'redact_json must receive either a JSON blob as a string or dict().  You passed in type {type(json_data)} which is not supported')
-        
+        payload = {"jsonText": json_text, "generatorDefault":generator_default, "generatorConfig": generator_config, "customModels": custom_models}
+
         try:
             if random_seed is not None:
-                response = self.client.http_post(endpoint, data=payload, additionalHeaders={'textual-random-seed':str(random_seed)})
+                additional_headers = {'textual-random-seed':str(random_seed)}
             else:
-                response = self.client.http_post(endpoint, data=payload)
+                additional_headers = {}
+            response = self.client.http_post(endpoint, data=payload, additional_headers=additional_headers)
         except requests.exceptions.HTTPError as e:
-             if e.response.status_code==400:                  
+             if e.response.status_code==400:
                   raise InvalidJsonForRedactionRequest(e.response.text)
              raise e
-        
+
         de_id_results = [SingleDetectionResult(x["start"], x["end"], x["label"], x["text"], x["score"], x["jsonPath"]) for x in list(response["deIdentifyResults"])]
 
         return RedactionResponse(response["originalText"], response["redactedText"], response["usage"], de_id_results)
 
     def get_custom_models(self) -> List[CustomModel]:
         """Returns all of the custom models that the user owns.
-         
+
         Returns
         -------
         List[CustomModel]
             A list of all of the custom models that the user owns.
         """
 
         with requests.Session() as session:
@@ -247,17 +290,17 @@
             models: List[CustomModel] = []
             for model in response:
                 id = model['id']
                 name = model['name']
                 entities = model['entities']
                 entityNames = [entity['label'] for entity in entities]
                 models.append(CustomModel(id, name, entityNames))
-            
+
             return models
-        
+
     def start_file_redaction(self, file: io.IOBase, file_name: str) -> str:
         """
         Redact a provided file
 
         Parameters
         --------
         file: io.IOBase
@@ -277,48 +320,54 @@
             'file': file
         }
 
         response = self.client.http_post("/api/unattachedfile/upload", files=files)
 
         return response['jobId']
 
-    def download_redacted_file(self, job_id: str, generator_config: GeneratorConfig = dict(), custom_models: List[str] = [], random_seed: Optional[int] = None, num_retries: Optional[int] = 6) -> io.BufferedWriter:
+    def download_redacted_file(self, job_id: str, generator_config: Dict[str, PiiState] = dict(), generator_default: PiiState = PiiState.Redaction, custom_models: List[str] = [], random_seed: Optional[int] = None, num_retries: int = 6) -> bytes:
         """
         Download a redacted file
 
         Parameters
         --------
         job_id: str
             The ID of the redaction job
-                    
-        generator_config: GeneratorConfig
-            A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
 
-        custom_models: List[str]
+        generator_config: Dict[str, PiiState]
+                A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
+
+        generator_default: PiiState = PiiState.Redaction
+                The default redaction used for all types not specified in generator_config.
+
+        custom_models: List[str] = []
             A list of custom model names to use to identify values to redact. To see the list of custom models that you have access to, use the get_custom_models function.
-        
-        random_seed: Optional[int]
+
+        random_seed: Optional[int] = None
             An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
 
-        num_retries: Optional[int]
+        num_retries: int = 6
             An optional value to specify how many times to attempt to download the file.  If a file is not yet ready for download, there will be a 10 second pause before retrying.  (The default value is 6)
-            
+
         Returns
         -------
-        io.BufferedWriter
-            The redacted file, ready to be written to disc as a buffered byte array
+        bytes
+            The redacted file as byte array
         """
+        self._validate_generator_options(generator_default, generator_config)
         retries = 1
         while(retries <= num_retries):
             try:
                 if random_seed is not None:
-                    return self.client.http_post_download_file(f"/api/unattachedfile/{job_id}/download", data={"generatorConfig": generator_config, "customModels": custom_models}, additionalHeaders={'textual-random-seed':str(random_seed)})
+                    additional_headers = {'textual-random-seed':str(random_seed)}
                 else:
-                    return self.client.http_post_download_file(f"/api/unattachedfile/{job_id}/download", data={"generatorConfig": generator_config, "customModels": custom_models})
+                    additional_headers = {}
+                return self.client.http_post_download_file(f"/api/unattachedfile/{job_id}/download", data={"generatorDefault": generator_default, "generatorConfig": generator_config, "customModels": custom_models}, additional_headers=additional_headers )
+                
+            
             except FileNotReadyForDownload:
                  retries = retries + 1
                  if retries <= num_retries:
                     sleep(10)
 
         retryWord = "retry" if num_retries==1 else "retries"
         raise FileNotReadyForDownload(f"After {num_retries} {retryWord} the file is not yet ready for download.  This is likely due to a high service load.  Please try again later.")
-
```

### Comparing `tonic_textual-1.2.1/tonic_textual/classes/api_responses/redaction_response.py` & `tonic_textual-1.3.0/tonic_textual/classes/api_responses/redaction_response.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.2.1/tonic_textual/classes/api_responses/single_detection_result.py` & `tonic_textual-1.3.0/tonic_textual/classes/api_responses/single_detection_result.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.2.1/tonic_textual/classes/dataset.py` & `tonic_textual-1.3.0/tonic_textual/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.2.1/tonic_textual/classes/datasetfile.py` & `tonic_textual-1.3.0/tonic_textual/classes/datasetfile.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.2.1/tonic_textual/classes/httpclient.py` & `tonic_textual-1.3.0/tonic_textual/classes/httpclient.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,36 +10,39 @@
 
     Parameters
     ----------
     base_url : str
         URL to the Tonic Textual instance.
     api_key : str
         The API token associated to use for the requests.
+    verify : bool
+        Whether SSL Certification verification is performed
     """
 
-    def __init__(self, base_url: str, api_key: str):
+    def __init__(self, base_url: str, api_key: str, verify: bool):
         self.base_url = base_url
         self.headers = {"Authorization": api_key, "User-Agent": "tonic-textual-python-sdk"}
+        self.verify = verify
 
     def http_get_file(self, url: str, session: requests.Session, params: dict={}) -> bytes:
         """Makes a get request to get a file.
 
         Parameters
         ----------
         url : str
             URL to make the get request. The URL is appended to self.base_url.
         params: dict
             Passed as the params parameter of the requests.get request.
 
         """
-        res = session.get(self.base_url + url, params=params, headers=self.headers, verify=False)
+        res = session.get(self.base_url + url, params=params, headers=self.headers, verify=self.verify)
         res.raise_for_status()
         return res.content.decode('utf-8')
     
-    def http_post_download_file(self, url: str, params: dict={}, data={}, additionalHeaders={}) -> bytes:
+    def http_post_download_file(self, url: str, params: dict={}, data={}, additional_headers={}) -> bytes:
         """Makes a POST request to download a file.
 
         Parameters
         ----------
         url : str
             URL to make the get request. The URL is appended to self.base_url.
         params: dict
@@ -47,15 +50,15 @@
         data: dict
             Request body
         additionaHeaders: dict
             Additional HTTP request headers
         """
 
         res = requests.post(
-            self.base_url + url, params=params, json=data, headers=self.headers | additionalHeaders, verify=False
+            self.base_url + url, params=params, json=data, headers=self.headers | additional_headers, verify=self.verify
         )
         try:
             res.raise_for_status()
         except requests.exceptions.HTTPError as err:
             if err.response.status_code==422:
                 raise LicenseInvalid(err)
             if err.response.status_code==409:
@@ -74,33 +77,33 @@
         ----------
         url : str
             URL to make the get request. The URL is appended to self.base_url.
         params: dict
             Passed as the params parameter of the requests.get request.
 
         """
-        res = session.get(self.base_url + url, params=params, headers=self.headers, verify=False)
+        res = session.get(self.base_url + url, params=params, headers=self.headers, verify=self.verify)
         res.raise_for_status()
         return res.json()
 
-    def http_post(self, url, params={}, data={}, files={}, additionalHeaders={}):
+    def http_post(self, url, params={}, data={}, files={}, additional_headers={}):
         """Make a post request.
 
         Parameters
         ----------
         url : str
             URL to make the post request. The URL is appended to self.base_url.
         params: dict
             Passed as the params parameter of the requests.post request.
         data: dict
             Passed as the data parameter of the requests.post request.
         """           
 
         res = requests.post(
-            self.base_url + url, params=params, json=data, headers=self.headers | additionalHeaders, verify=False, files=files
+            self.base_url + url, params=params, json=data, headers=self.headers | additional_headers, verify=self.verify, files=files
         )
         try:
             res.raise_for_status()
         except requests.exceptions.HTTPError as err:
             if err.response.status_code==422:
                 raise LicenseInvalid(err)
             else:
@@ -117,16 +120,16 @@
             URL to make the put request. The URL is appended to self.base_url.
         params: dict
             Passed as the params parameter of the requests.put request.
         data: dict
             Passed as the data parameter of the requests.put request.
         """
         res = requests.put(
-            self.base_url + url, params=params, json=data, headers=self.headers, verify=False
+            self.base_url + url, params=params, json=data, headers=self.headers, verify=self.verify
         )
         res.raise_for_status()
         return res.json()
 
     def http_delete(self, url, params={}):
-        res = requests.delete(self.base_url + url, params = params, headers = self.headers, verify = False)
+        res = requests.delete(self.base_url + url, params = params, headers = self.headers, verify = self.verify)
         res.raise_for_status()
         return res.json()
```

### Comparing `tonic_textual-1.2.1/tonic_textual/classes/tonic_exception.py` & `tonic_textual-1.3.0/tonic_textual/classes/tonic_exception.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.2.1/tonic_textual/services/dataset.py` & `tonic_textual-1.3.0/tonic_textual/services/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.2.1/tonic_textual/services/datasetfile.py` & `tonic_textual-1.3.0/tonic_textual/services/datasetfile.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.2.1/PKG-INFO` & `tonic_textual-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic-textual
-Version: 1.2.1
+Version: 1.3.0
 Summary: Wrappers around the Tonic Textual API
 Home-page: https://www.tonic.ai/
 License: MIT
 Keywords: tonic.ai,tonic,tonic textual
 Author: Adam Kamor
 Author-email: adam@tonic.ai
 Requires-Python: >=3.7,<4.0
@@ -12,15 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: more-itertools (>=8.6.0,<9.0.0)
 Requires-Dist: pandas (>=1.0.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: tqdm (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Overview
```

