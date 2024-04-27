# Comparing `tmp/agentic_security-0.1.1.tar.gz` & `tmp/agentic_security-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentic_security-0.1.1.tar", max compression
+gzip compressed data, was "agentic_security-0.1.2.tar", max compression
```

## Comparing `agentic_security-0.1.1.tar` & `agentic_security-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0    11367 2024-04-26 18:36:08.131913 agentic_security-0.1.1/LICENSE
--rw-r--r--   0        0        0     8168 2024-04-26 18:36:08.131913 agentic_security-0.1.1/Readme.md
--rw-r--r--   0        0        0        0 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/__init__.py
--rw-r--r--   0        0        0      438 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/__main__.py
--rw-r--r--   0        0        0     8903 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/agent.py
--rw-r--r--   0        0        0     3833 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/app.py
--rw-r--r--   0        0        0     2722 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/http_spec.py
--rw-r--r--   0        0        0        0 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_actor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_actor/__main__.py
--rw-r--r--   0        0        0     3333 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_actor/fuzzer.py
--rw-r--r--   0        0        0     1209 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_actor/refusal.py
--rw-r--r--   0        0        0      458 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_actor/test_refusal.py
--rw-r--r--   0        0        0     3889 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/__init__.py
--rw-r--r--   0        0        0     9183 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/data.py
--rw-r--r--   0        0        0        0 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/modules/__init__.py
--rw-r--r--   0        0        0     6593 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/modules/adaptive_attacks.py
--rw-r--r--   0        0        0     2446 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/modules/test_adaptive_attacks.py
--rw-r--r--   0        0        0     2645 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/stenography_fn.py
--rw-r--r--   0        0        0      739 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/test_data.py
--rw-r--r--   0        0        0     2365 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/report_chart.py
--rw-r--r--   0        0        0    26906 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/static/index.html
--rw-r--r--   0        0        0     1961 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/test_spec.py
--rw-r--r--   0        0        0     1278 2024-04-26 18:36:08.131913 agentic_security-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9428 1970-01-01 00:00:00.000000 agentic_security-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11367 2024-04-27 14:21:32.822184 agentic_security-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9192 2024-04-27 14:21:32.822184 agentic_security-0.1.2/Readme.md
+-rw-r--r--   0        0        0       64 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/__init__.py
+-rw-r--r--   0        0        0      560 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/__main__.py
+-rw-r--r--   0        0        0     8903 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/agent.py
+-rw-r--r--   0        0        0     3833 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/app.py
+-rw-r--r--   0        0        0     2900 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/http_spec.py
+-rw-r--r--   0        0        0     2265 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/lib.py
+-rw-r--r--   0        0        0        0 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_actor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_actor/__main__.py
+-rw-r--r--   0        0        0     3333 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_actor/fuzzer.py
+-rw-r--r--   0        0        0     1209 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_actor/refusal.py
+-rw-r--r--   0        0        0      458 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_actor/test_refusal.py
+-rw-r--r--   0        0        0     3889 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_data/__init__.py
+-rw-r--r--   0        0        0     9183 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_data/data.py
+-rw-r--r--   0        0        0        0 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_data/modules/__init__.py
+-rw-r--r--   0        0        0     6593 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_data/modules/adaptive_attacks.py
+-rw-r--r--   0        0        0     2446 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_data/modules/test_adaptive_attacks.py
+-rw-r--r--   0        0        0     2645 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_data/stenography_fn.py
+-rw-r--r--   0        0        0      725 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/probe_data/test_data.py
+-rw-r--r--   0        0        0     2365 2024-04-27 14:21:32.822184 agentic_security-0.1.2/agentic_security/report_chart.py
+-rw-r--r--   0        0        0    26899 2024-04-27 14:21:32.826184 agentic_security-0.1.2/agentic_security/static/index.html
+-rw-r--r--   0        0        0      651 2024-04-27 14:21:32.826184 agentic_security-0.1.2/agentic_security/test_lib.py
+-rw-r--r--   0        0        0     1961 2024-04-27 14:21:32.826184 agentic_security-0.1.2/agentic_security/test_spec.py
+-rw-r--r--   0        0        0     1318 2024-04-27 14:21:32.826184 agentic_security-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10534 1970-01-01 00:00:00.000000 agentic_security-0.1.2/PKG-INFO
```

### Comparing `agentic_security-0.1.1/LICENSE` & `agentic_security-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/Readme.md` & `agentic_security-0.1.2/Readme.md`

 * *Files 17% similar despite different names*

```diff
@@ -24,22 +24,20 @@
 ## Features
 
 - Customizable Rule Sets or Agent based attacks🛠️
 - Comprehansive fuzzing for any LLMs 🧪
 - LLM API integration and stress testing 🛠️
 - Wide range of fuzzing and attack techniques 🌀
 
-
 Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
 ## About the Project 🧙
 
 <img width="100%" alt="booking-screen" src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002396/1-ezgif.com-video-to-gif-converter_s2hsro.gif">
 
-
 ## 📦 Installation
 
 To get started with Agentic Security, simply install the package using pip:
 
 ```shell
 pip install agentic_security
 ```
@@ -99,14 +97,51 @@
 To add your own dataset you can place one or multiples csv files with `prompt` column, this data will be loaded on `agentic_security` startup
 
 ```
 2024-04-13 13:21:31.157 | INFO     | agentic_security.probe_data.data:load_local_csv:273 - Found 1 CSV files
 2024-04-13 13:21:31.157 | INFO     | agentic_security.probe_data.data:load_local_csv:274 - CSV files: ['prompts.csv']
 ```
 
+## Run as CI check
+
+ci.py
+
+```python
+from agentic_security import AgenticSecurity
+
+spec = """
+POST http://0.0.0.0:8718/v1/self-probe
+Authorization: Bearer XXXXX
+Content-Type: application/json
+
+{
+    "prompt": "<<PROMPT>>"
+}
+"""
+result = AgenticSecurity.scan(spec)
+
+# module: failure rate
+# {"Local CSV": 79.65116279069767, "llm-adaptive-attacks": 20.0}
+exit(max(r.values()) > 20)
+```
+
+```
+python ci.py
+2024-04-27 17:15:13.545 | INFO     | agentic_security.probe_data.data:load_local_csv:279 - Found 1 CSV files
+2024-04-27 17:15:13.545 | INFO     | agentic_security.probe_data.data:load_local_csv:280 - CSV files: ['prompts.csv']
+0it [00:00, ?it/s][INFO] 2024-04-27 17:15:13.74 | data:prepare_prompts:195 | Loading Custom CSV
+[INFO] 2024-04-27 17:15:13.74 | fuzzer:perform_scan:53 | Scanning Local CSV 15
+18it [00:00, 176.88it/s]
++-----------+--------------+--------+
+|  Module   | Failure Rate | Status |
++-----------+--------------+--------+
+| Local CSV |    80.0%     |   ✘    |
++-----------+--------------+--------+
+```
+
 ## Extending dataset collections
 
 1. Add new metadata to agentic_security.probe_data.REGISTRY
 
 ```python
     {
         "dataset_name": "markush1/LLM-Jailbreak-Classifier",
```

### Comparing `agentic_security-0.1.1/agentic_security/agent.py` & `agentic_security-0.1.2/agentic_security/agent.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/agentic_security/app.py` & `agentic_security-0.1.2/agentic_security/app.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/agentic_security/http_spec.py` & `agentic_security-0.1.2/agentic_security/http_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import httpx
 from pydantic import BaseModel
 
 
+class InvalidHTTPSpecError(Exception):
+    ...
+
+
 class LLMSpec(BaseModel):
     method: str
     url: str
     headers: dict
     body: str
 
     @classmethod
     def from_string(cls, http_spec: str):
-        return parse_http_spec(http_spec)
+        try:
+            return parse_http_spec(http_spec)
+        except Exception as e:
+            raise InvalidHTTPSpecError(f"Failed to parse HTTP spec: {e}") from e
 
     async def probe(self, prompt: str) -> httpx.Response:
         """Sends an HTTP request using the `httpx` library.
 
         Replaces a placeholder in the request body with a provided prompt and returns the response.
 
         Args:
```

### Comparing `agentic_security-0.1.1/agentic_security/probe_actor/fuzzer.py` & `agentic_security-0.1.2/agentic_security/probe_actor/fuzzer.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/agentic_security/probe_actor/refusal.py` & `agentic_security-0.1.2/agentic_security/probe_actor/refusal.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/agentic_security/probe_data/__init__.py` & `agentic_security-0.1.2/agentic_security/probe_data/__init__.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/agentic_security/probe_data/data.py` & `agentic_security-0.1.2/agentic_security/probe_data/data.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/agentic_security/probe_data/modules/adaptive_attacks.py` & `agentic_security-0.1.2/agentic_security/probe_data/modules/adaptive_attacks.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/agentic_security/probe_data/modules/test_adaptive_attacks.py` & `agentic_security-0.1.2/agentic_security/probe_data/modules/test_adaptive_attacks.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/agentic_security/probe_data/stenography_fn.py` & `agentic_security-0.1.2/agentic_security/probe_data/stenography_fn.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/agentic_security/probe_data/test_data.py` & `agentic_security-0.1.2/agentic_security/probe_data/test_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from inline_snapshot import snapshot
 
-from .data import ProbeDataset, prepare_prompts
+from .data import prepare_prompts
 
 
 class TestPreparePrompts:
     # Empty dataset_names input returns an empty list
     def test_empty_dataset_list(self):
         # Call the prepare_prompts function with an empty dataset_names list
         prepared_prompts = prepare_prompts([], 100)
```

### Comparing `agentic_security-0.1.1/agentic_security/report_chart.py` & `agentic_security-0.1.2/agentic_security/report_chart.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/agentic_security/static/index.html` & `agentic_security-0.1.2/agentic_security/static/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
                     class="border-b transition-colors hover:bg-muted/50 data-[state=selected]:bg-muted">
                     <th
                       class="h-12 px-4 text-left align-middle font-medium text-muted-foreground [&amp;:has([role=checkbox])]:pr-0">
                       Vulnerability Module
                     </th>
                     <th
                       class="h-12 px-4 text-left align-middle font-medium text-muted-foreground [&amp;:has([role=checkbox])]:pr-0">
-                      % Protection rate
+                      % Strength
                     </th>
                     <th
                       class="h-12 px-4 text-left align-middle font-medium text-muted-foreground [&amp;:has([role=checkbox])]:pr-0">
                       Number of Tokens
                     </th>
                     <th
                       class="h-12 px-4 text-left align-middle font-medium text-muted-foreground [&amp;:has([role=checkbox])]:pr-0">
```

#### html2text {}

```diff
@@ -41,14 +41,14 @@
 whitespace-nowrap rounded-md text-sm font-medium ring-offset-background
 transition-colors focus-visible:outline-none focus-visible:ring-2 focus-
 visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none
 disabled:opacity-50 bg-earth-1 text-earth-foreground hover:bg-earth-1/90 h-10
 px-4 py-2"> Run Scan
 src="imageUrl" alt="Generated Plot">
 ******** SSccaann RReessuullttss ********
-VVuullnneerraabbiilliittyy MMoodduullee %% PPrrootteeccttiioonn rraattee NNuummbbeerr ooff TTookkeennss CCoosstt ((iinn ggpptt--33 ttookkeennss))
+VVuullnneerraabbiilliittyy MMoodduullee %% SSttrreennggtthh NNuummbbeerr ooff TTookkeennss CCoosstt ((iinn ggpptt--33 ttookkeennss))
 click="downloadFailures" class="inline-flex text-gray-100 items-center justify-
 center whitespace-nowrap rounded-md text-sm font-medium ring-offset-background
 transition-colors focus-visible:outline-none focus-visible:ring-2 focus-
 visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none
 disabled:opacity-50 bg-earth-1 text-earth-foreground hover:bg-earth-1/90 h-10
 px-4 py-2"> Download failures
```

### Comparing `agentic_security-0.1.1/agentic_security/test_spec.py` & `agentic_security-0.1.2/agentic_security/test_spec.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.1/PKG-INFO` & `agentic_security-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentic_security
-Version: 0.1.1
+Version: 0.1.2
 Summary: Agentic LLM vulnerability scanner
 Home-page: https://github.com/msoedov/agentic_security
 License: MIT
 Keywords: LLM vulnerability scanner,llm security,llm adversarial attacks,prompt injection,prompt leakage,prompt injection attacks,prompt leakage prevention,llm vulnerabilities,owasp-llm-top-10
 Author: Alexander Miasoiedov
 Author-email: msoedov@gmail.com
 Maintainer: Alexander Miasoiedov
@@ -13,20 +13,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cache-to-disk (>=2.0.0,<3.0.0)
+Requires-Dist: colorama (>=0.4.4,<0.5.0)
 Requires-Dist: datasets (>=1.14.0,<2.0.0)
 Requires-Dist: fastapi (>=0.109.1,<0.111.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: httpx (>=0.25.1,<0.28.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pandas (>=1.4,<3.0)
+Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: uvicorn (>=0.23.2,<0.30.0)
 Project-URL: Repository, https://github.com/msoedov/agentic_security
 Description-Content-Type: text/markdown
 
 <p align="center">
 
 <h1 align="center">Agentic Security</h1>
@@ -53,22 +55,20 @@
 ## Features
 
 - Customizable Rule Sets or Agent based attacks🛠️
 - Comprehansive fuzzing for any LLMs 🧪
 - LLM API integration and stress testing 🛠️
 - Wide range of fuzzing and attack techniques 🌀
 
-
 Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
 ## About the Project 🧙
 
 <img width="100%" alt="booking-screen" src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002396/1-ezgif.com-video-to-gif-converter_s2hsro.gif">
 
-
 ## 📦 Installation
 
 To get started with Agentic Security, simply install the package using pip:
 
 ```shell
 pip install agentic_security
 ```
@@ -128,14 +128,51 @@
 To add your own dataset you can place one or multiples csv files with `prompt` column, this data will be loaded on `agentic_security` startup
 
 ```
 2024-04-13 13:21:31.157 | INFO     | agentic_security.probe_data.data:load_local_csv:273 - Found 1 CSV files
 2024-04-13 13:21:31.157 | INFO     | agentic_security.probe_data.data:load_local_csv:274 - CSV files: ['prompts.csv']
 ```
 
+## Run as CI check
+
+ci.py
+
+```python
+from agentic_security import AgenticSecurity
+
+spec = """
+POST http://0.0.0.0:8718/v1/self-probe
+Authorization: Bearer XXXXX
+Content-Type: application/json
+
+{
+    "prompt": "<<PROMPT>>"
+}
+"""
+result = AgenticSecurity.scan(spec)
+
+# module: failure rate
+# {"Local CSV": 79.65116279069767, "llm-adaptive-attacks": 20.0}
+exit(max(r.values()) > 20)
+```
+
+```
+python ci.py
+2024-04-27 17:15:13.545 | INFO     | agentic_security.probe_data.data:load_local_csv:279 - Found 1 CSV files
+2024-04-27 17:15:13.545 | INFO     | agentic_security.probe_data.data:load_local_csv:280 - CSV files: ['prompts.csv']
+0it [00:00, ?it/s][INFO] 2024-04-27 17:15:13.74 | data:prepare_prompts:195 | Loading Custom CSV
+[INFO] 2024-04-27 17:15:13.74 | fuzzer:perform_scan:53 | Scanning Local CSV 15
+18it [00:00, 176.88it/s]
++-----------+--------------+--------+
+|  Module   | Failure Rate | Status |
++-----------+--------------+--------+
+| Local CSV |    80.0%     |   ✘    |
++-----------+--------------+--------+
+```
+
 ## Extending dataset collections
 
 1. Add new metadata to agentic_security.probe_data.REGISTRY
 
 ```python
     {
         "dataset_name": "markush1/LLM-Jailbreak-Classifier",
```

