# Comparing `tmp/agentic_security-0.0.4.tar.gz` & `tmp/agentic_security-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentic_security-0.0.4.tar", max compression
+gzip compressed data, was "agentic_security-0.1.1.tar", max compression
```

## Comparing `agentic_security-0.0.4.tar` & `agentic_security-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11367 2024-04-26 18:21:56.944152 agentic_security-0.0.4/LICENSE
--rw-r--r--   0        0        0     9125 2024-04-26 18:21:56.944152 agentic_security-0.0.4/Readme.md
--rw-r--r--   0        0        0        0 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/__init__.py
--rw-r--r--   0        0        0      438 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/__main__.py
--rw-r--r--   0        0        0     8903 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/agent.py
--rw-r--r--   0        0        0     3833 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/app.py
--rw-r--r--   0        0        0     2722 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/http_spec.py
--rw-r--r--   0        0        0        0 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_actor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_actor/__main__.py
--rw-r--r--   0        0        0     3333 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_actor/fuzzer.py
--rw-r--r--   0        0        0     1209 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_actor/refusal.py
--rw-r--r--   0        0        0      458 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_actor/test_refusal.py
--rw-r--r--   0        0        0     3889 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_data/__init__.py
--rw-r--r--   0        0        0     9183 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_data/data.py
--rw-r--r--   0        0        0        0 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_data/modules/__init__.py
--rw-r--r--   0        0        0     6593 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_data/modules/adaptive_attacks.py
--rw-r--r--   0        0        0     2446 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_data/modules/test_adaptive_attacks.py
--rw-r--r--   0        0        0     2645 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_data/stenography_fn.py
--rw-r--r--   0        0        0      739 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/probe_data/test_data.py
--rw-r--r--   0        0        0     2365 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/report_chart.py
--rw-r--r--   0        0        0    26906 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/static/index.html
--rw-r--r--   0        0        0     1961 2024-04-26 18:21:56.944152 agentic_security-0.0.4/agentic_security/test_spec.py
--rw-r--r--   0        0        0     1241 2024-04-26 18:21:56.948153 agentic_security-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    10389 1970-01-01 00:00:00.000000 agentic_security-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11367 2024-04-26 18:36:08.131913 agentic_security-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8168 2024-04-26 18:36:08.131913 agentic_security-0.1.1/Readme.md
+-rw-r--r--   0        0        0        0 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/__init__.py
+-rw-r--r--   0        0        0      438 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/__main__.py
+-rw-r--r--   0        0        0     8903 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/agent.py
+-rw-r--r--   0        0        0     3833 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/app.py
+-rw-r--r--   0        0        0     2722 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/http_spec.py
+-rw-r--r--   0        0        0        0 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_actor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_actor/__main__.py
+-rw-r--r--   0        0        0     3333 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_actor/fuzzer.py
+-rw-r--r--   0        0        0     1209 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_actor/refusal.py
+-rw-r--r--   0        0        0      458 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_actor/test_refusal.py
+-rw-r--r--   0        0        0     3889 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/__init__.py
+-rw-r--r--   0        0        0     9183 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/data.py
+-rw-r--r--   0        0        0        0 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/modules/__init__.py
+-rw-r--r--   0        0        0     6593 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/modules/adaptive_attacks.py
+-rw-r--r--   0        0        0     2446 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/modules/test_adaptive_attacks.py
+-rw-r--r--   0        0        0     2645 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/stenography_fn.py
+-rw-r--r--   0        0        0      739 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/probe_data/test_data.py
+-rw-r--r--   0        0        0     2365 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/report_chart.py
+-rw-r--r--   0        0        0    26906 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/static/index.html
+-rw-r--r--   0        0        0     1961 2024-04-26 18:36:08.131913 agentic_security-0.1.1/agentic_security/test_spec.py
+-rw-r--r--   0        0        0     1278 2024-04-26 18:36:08.131913 agentic_security-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9428 1970-01-01 00:00:00.000000 agentic_security-0.1.1/PKG-INFO
```

### Comparing `agentic_security-0.0.4/LICENSE` & `agentic_security-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/Readme.md` & `agentic_security-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: agentic_security
+Version: 0.1.1
+Summary: Agentic LLM vulnerability scanner
+Home-page: https://github.com/msoedov/agentic_security
+License: MIT
+Keywords: LLM vulnerability scanner,llm security,llm adversarial attacks,prompt injection,prompt leakage,prompt injection attacks,prompt leakage prevention,llm vulnerabilities,owasp-llm-top-10
+Author: Alexander Miasoiedov
+Author-email: msoedov@gmail.com
+Maintainer: Alexander Miasoiedov
+Maintainer-email: msoedov@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: cache-to-disk (>=2.0.0,<3.0.0)
+Requires-Dist: datasets (>=1.14.0,<2.0.0)
+Requires-Dist: fastapi (>=0.109.1,<0.111.0)
+Requires-Dist: fire (>=0.5.0,<0.6.0)
+Requires-Dist: httpx (>=0.25.1,<0.28.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: pandas (>=1.4,<3.0)
+Requires-Dist: uvicorn (>=0.23.2,<0.30.0)
+Project-URL: Repository, https://github.com/msoedov/agentic_security
+Description-Content-Type: text/markdown
+
 <p align="center">
 
 <h1 align="center">Agentic Security</h1>
 
 <p align="center">
     The open-source Agentic LLM Vulnerability Scanner .
     <br />
@@ -17,34 +46,28 @@
 <img alt="GitHub Issues" src="https://img.shields.io/github/issues/msoedov/agentic_security" />
 <img alt="GitHub Pull Requests" src="https://img.shields.io/github/issues-pr/msoedov/agentic_security" />
 <img alt="Github License" src="https://img.shields.io/github/license/msoedov/agentic_security" />
 </p>
   </p>
 </p>
 
-## About the Project 🧙
+## Features
 
-<img width="100%" alt="booking-screen" src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002396/1-ezgif.com-video-to-gif-converter_s2hsro.gif">
+- Customizable Rule Sets or Agent based attacks🛠️
+- Comprehansive fuzzing for any LLMs 🧪
+- LLM API integration and stress testing 🛠️
+- Wide range of fuzzing and attack techniques 🌀
 
-<p align="center"></p>
-<h3 align="center">LLM threat vectors scanner</h3>
 
-|   |   |
-| --- | --- |
-| <b>Prebuilt Datasets of Prompts</b><br /><br /><br/><b>Focused on OWASP top 10 LLM</b><br /><br /><br /><b>Integration under 1 min</b><br />| <img src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002416/12-ezgif.com-video-to-gif-converter_jspzmx.gif" /> |
+Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
-## Features
+## About the Project 🧙
 
-- Comprehensive Threat Detection 🛡️: Scans for a wide array of LLM vulnerabilities including prompt injection, jailbreaking, hallucinations, biases, and other malicious exploitation attempts.
-- OWASP Top 10 for LLMs scan: to test the list of the most critical LLM vulnerabilities.
-- Privacy-centric Architecture 🔒: Ensures that all data scanning and analysis occur on-premise or in a local environment, with no external data transmission, maintaining strict data privacy.
-- Comprehensive Reporting Tools 📊: Offers detailed reports of vulnerability, helping teams to quickly understand and respond to security incidents.
-- Customizable Rule Sets 🛠️: Allows users to define custom attack rules and parameters to meet specific prompt attacks needs and compliance standards.
+<img width="100%" alt="booking-screen" src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002396/1-ezgif.com-video-to-gif-converter_s2hsro.gif">
 
-Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
 ## 📦 Installation
 
 To get started with Agentic Security, simply install the package using pip:
 
 ```shell
 pip install agentic_security
@@ -270,7 +293,8 @@
 <a href="https://cal.com/alexander-myasoedov-go2tfs/30min"><img src="https://cal.com/book-with-cal-dark.svg" alt="Book us with Cal.com"></a>
 
 Book a 1-on-1 Session with the founders, to discuss any issues, provide feedback, or explore how we can improve agentic_security for you.
 
 ## Repo Activity
 
 <img width="100%" src="https://repobeats.axiom.co/api/embed/2b4b4e080d21ef9174ca69bcd801145a71f67aaf.svg" />
+
```

### Comparing `agentic_security-0.0.4/agentic_security/agent.py` & `agentic_security-0.1.1/agentic_security/agent.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/app.py` & `agentic_security-0.1.1/agentic_security/app.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/http_spec.py` & `agentic_security-0.1.1/agentic_security/http_spec.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/probe_actor/fuzzer.py` & `agentic_security-0.1.1/agentic_security/probe_actor/fuzzer.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/probe_actor/refusal.py` & `agentic_security-0.1.1/agentic_security/probe_actor/refusal.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/probe_data/__init__.py` & `agentic_security-0.1.1/agentic_security/probe_data/__init__.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/probe_data/data.py` & `agentic_security-0.1.1/agentic_security/probe_data/data.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/probe_data/modules/adaptive_attacks.py` & `agentic_security-0.1.1/agentic_security/probe_data/modules/adaptive_attacks.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/probe_data/modules/test_adaptive_attacks.py` & `agentic_security-0.1.1/agentic_security/probe_data/modules/test_adaptive_attacks.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/probe_data/stenography_fn.py` & `agentic_security-0.1.1/agentic_security/probe_data/stenography_fn.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/probe_data/test_data.py` & `agentic_security-0.1.1/agentic_security/probe_data/test_data.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/report_chart.py` & `agentic_security-0.1.1/agentic_security/report_chart.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/static/index.html` & `agentic_security-0.1.1/agentic_security/static/index.html`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/agentic_security/test_spec.py` & `agentic_security-0.1.1/agentic_security/test_spec.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.0.4/pyproject.toml` & `agentic_security-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentic_security"
-version = "0.0.4"
+version = "0.1.1"
 description = "Agentic LLM vulnerability scanner"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 repository = "https://github.com/msoedov/agentic_security"
 license = "MIT"
 readme = "Readme.md"
 keywords = [
@@ -28,25 +28,25 @@
 python = "^3.9"
 fastapi = ">=0.109.1,<0.111.0"
 uvicorn = ">=0.23.2,<0.30.0"
 fire = "^0.5.0"
 loguru = "^0.7.2"
 httpx = ">=0.25.1,<0.28.0"
 cache-to-disk = "^2.0.0"
-pandas = "^1.4.0"
+pandas = ">=1.4,<3.0"
 datasets = "^1.14.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.10.1,<25.0.0"
 mypy = "^1.6.1"
 httpx = ">=0.25.1,<0.28.0"
-pytest = "^7.4.3"
+pytest = ">=7.4.3,<9.0.0"
 pre-commit = "^3.5.0"
 inline-snapshot = "^0.8.0"
-
+langchain-groq = "^0.1.3"
 
 [tool.ruff]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `agentic_security-0.0.4/PKG-INFO` & `agentic_security-0.1.1/Readme.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: agentic_security
-Version: 0.0.4
-Summary: Agentic LLM vulnerability scanner
-Home-page: https://github.com/msoedov/agentic_security
-License: MIT
-Keywords: LLM vulnerability scanner,llm security,llm adversarial attacks,prompt injection,prompt leakage,prompt injection attacks,prompt leakage prevention,llm vulnerabilities,owasp-llm-top-10
-Author: Alexander Miasoiedov
-Author-email: msoedov@gmail.com
-Maintainer: Alexander Miasoiedov
-Maintainer-email: msoedov@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: cache-to-disk (>=2.0.0,<3.0.0)
-Requires-Dist: datasets (>=1.14.0,<2.0.0)
-Requires-Dist: fastapi (>=0.109.1,<0.111.0)
-Requires-Dist: fire (>=0.5.0,<0.6.0)
-Requires-Dist: httpx (>=0.25.1,<0.28.0)
-Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: pandas (>=1.4.0,<2.0.0)
-Requires-Dist: uvicorn (>=0.23.2,<0.30.0)
-Project-URL: Repository, https://github.com/msoedov/agentic_security
-Description-Content-Type: text/markdown
-
 <p align="center">
 
 <h1 align="center">Agentic Security</h1>
 
 <p align="center">
     The open-source Agentic LLM Vulnerability Scanner .
     <br />
@@ -46,34 +17,28 @@
 <img alt="GitHub Issues" src="https://img.shields.io/github/issues/msoedov/agentic_security" />
 <img alt="GitHub Pull Requests" src="https://img.shields.io/github/issues-pr/msoedov/agentic_security" />
 <img alt="Github License" src="https://img.shields.io/github/license/msoedov/agentic_security" />
 </p>
   </p>
 </p>
 
-## About the Project 🧙
+## Features
 
-<img width="100%" alt="booking-screen" src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002396/1-ezgif.com-video-to-gif-converter_s2hsro.gif">
+- Customizable Rule Sets or Agent based attacks🛠️
+- Comprehansive fuzzing for any LLMs 🧪
+- LLM API integration and stress testing 🛠️
+- Wide range of fuzzing and attack techniques 🌀
 
-<p align="center"></p>
-<h3 align="center">LLM threat vectors scanner</h3>
 
-|   |   |
-| --- | --- |
-| <b>Prebuilt Datasets of Prompts</b><br /><br /><br/><b>Focused on OWASP top 10 LLM</b><br /><br /><br /><b>Integration under 1 min</b><br />| <img src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002416/12-ezgif.com-video-to-gif-converter_jspzmx.gif" /> |
+Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
-## Features
+## About the Project 🧙
 
-- Comprehensive Threat Detection 🛡️: Scans for a wide array of LLM vulnerabilities including prompt injection, jailbreaking, hallucinations, biases, and other malicious exploitation attempts.
-- OWASP Top 10 for LLMs scan: to test the list of the most critical LLM vulnerabilities.
-- Privacy-centric Architecture 🔒: Ensures that all data scanning and analysis occur on-premise or in a local environment, with no external data transmission, maintaining strict data privacy.
-- Comprehensive Reporting Tools 📊: Offers detailed reports of vulnerability, helping teams to quickly understand and respond to security incidents.
-- Customizable Rule Sets 🛠️: Allows users to define custom attack rules and parameters to meet specific prompt attacks needs and compliance standards.
+<img width="100%" alt="booking-screen" src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002396/1-ezgif.com-video-to-gif-converter_s2hsro.gif">
 
-Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
 ## 📦 Installation
 
 To get started with Agentic Security, simply install the package using pip:
 
 ```shell
 pip install agentic_security
@@ -299,8 +264,7 @@
 <a href="https://cal.com/alexander-myasoedov-go2tfs/30min"><img src="https://cal.com/book-with-cal-dark.svg" alt="Book us with Cal.com"></a>
 
 Book a 1-on-1 Session with the founders, to discuss any issues, provide feedback, or explore how we can improve agentic_security for you.
 
 ## Repo Activity
 
 <img width="100%" src="https://repobeats.axiom.co/api/embed/2b4b4e080d21ef9174ca69bcd801145a71f67aaf.svg" />
-
```

