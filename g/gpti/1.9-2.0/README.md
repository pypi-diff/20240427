# Comparing `tmp/gpti-1.9.tar.gz` & `tmp/gpti-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpti-1.9.tar", last modified: Sat Apr 27 17:57:56 2024, max compression
+gzip compressed data, was "gpti-2.0.tar", last modified: Sat Apr 27 17:59:42 2024, max compression
```

## Comparing `gpti-1.9.tar` & `gpti-2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 17:57:56.038385 gpti-1.9/
--rw-rw-rw-   0        0        0     1084 2024-01-24 17:14:27.000000 gpti-1.9/LICENSE
--rw-rw-rw-   0        0        0    68491 2024-04-27 17:57:56.038385 gpti-1.9/PKG-INFO
--rw-rw-rw-   0        0        0    66276 2024-04-18 01:56:18.000000 gpti-1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 17:57:56.017878 gpti-1.9/gpti/
--rw-rw-rw-   0        0        0   118538 2024-04-27 17:55:59.000000 gpti-1.9/gpti/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 17:57:56.033973 gpti-1.9/gpti.egg-info/
--rw-rw-rw-   0        0        0    68491 2024-04-27 17:57:55.000000 gpti-1.9/gpti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-04-27 17:57:55.000000 gpti-1.9/gpti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 17:57:55.000000 gpti-1.9/gpti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-27 17:57:55.000000 gpti-1.9/gpti.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-27 17:57:55.000000 gpti-1.9/gpti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 17:57:56.044236 gpti-1.9/setup.cfg
--rw-rw-rw-   0        0        0     1180 2024-04-27 17:55:35.000000 gpti-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 17:59:42.611846 gpti-2.0/
+-rw-rw-rw-   0        0        0     1084 2024-01-24 17:14:27.000000 gpti-2.0/LICENSE
+-rw-rw-rw-   0        0        0    68197 2024-04-27 17:59:42.610102 gpti-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    65998 2024-04-27 17:59:16.000000 gpti-2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 17:59:42.569282 gpti-2.0/gpti/
+-rw-rw-rw-   0        0        0   118538 2024-04-27 17:55:59.000000 gpti-2.0/gpti/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 17:59:42.606561 gpti-2.0/gpti.egg-info/
+-rw-rw-rw-   0        0        0    68197 2024-04-27 17:59:42.000000 gpti-2.0/gpti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-04-27 17:59:42.000000 gpti-2.0/gpti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 17:59:42.000000 gpti-2.0/gpti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-27 17:59:42.000000 gpti-2.0/gpti.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-27 17:59:42.000000 gpti-2.0/gpti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 17:59:42.611846 gpti-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2024-04-27 17:59:30.000000 gpti-2.0/setup.py
```

### Comparing `gpti-1.9/LICENSE` & `gpti-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpti-1.9/PKG-INFO` & `gpti-2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpti
-Version: 1.9
+Version: 2.0
 Summary: This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT
 Home-page: https://github.com/yandricr/gpti-py/
 Author: yandricr
 Author-email: yandribret@gmail.com
 License: MIT
 Project-URL: Documentation, https://nexra.aryahcr.cc/
 Project-URL: Funding, https://ko-fi.com/yandricr
@@ -32,15 +32,14 @@
 ## Available Models
 
 GPTI provides access to a variety of artificial intelligence models to meet various needs. Currently, the available models include:
 
 - [**ChatGPT**](#gpt)
 - [**ChatGPT v2**](#gpt-v2)
 - [**ChatGPT Web**](#gptweb)
-- [**ChatGPT Prompts**](#gpt-prompts)
 - [**Bing**](#bing)
 - [**LLaMA-2**](#llama2)
 - [**DALL·E**](#dalle)
 - [**DALL-E 2**](#dalle2) (PRO)
 - [**DALL-E Mini**](#dalle-mini)
 - [**Prodia**](#prodia)
 - [**Prodia Stable-Diffusion**](#prodia-stablediffusion)
@@ -199,15 +198,15 @@
         "role": "assistant",
         "content": "Hello, Yandri! How are you today?"
     },
     {
         "role": "user",
         "content": "Can you repeat my name?"
     }
-], markdown=True, stream=False)
+], markdown=False, stream=False)
 
 if res.error != None:
     print(json.dumps(res.error))
 else:
     for chunk in res.stream():
         print(json.dumps(chunk))
 ```
@@ -258,29 +257,14 @@
     "code": 200,
     "status": true,
     "gpt": "Yes, I am familiar with the movie Wonka released in 2023. Wonka is a musical fantasy film directed by Paul King, adapted from the character at the center of Roald Dahl's iconic children's book, \"Charlie and the Chocolate Factory.\" The film follows the story of a young and poor Willy Wonka as he dreams of opening a shop in a chocolate-renowned city and discovers that the industry is controlled by a greedy cartel. The film has a rating of 7.1/10 and has received positive reviews with a score of 83% on Rotten Tomatoes. It was released on December 15, 2023, and has earned $552.1 million at the box office. The cast includes actors such as Timothée Chalamet. Unfortunately, I couldn't find information on whether the movie is available on Netflix.",
     "original": null
 }
 ```
 
-<a id="gpt-prompts"></a>
-## Usage GPT Prompts
-
-```python
-import json
-from gpti import gpt
-
-res = gpt.prompts(lang="en", limit=4, offset=0)
-
-if res.error != None:
-    print(json.dumps(res.error))
-else: 
-    print(json.dumps(res.result))
-```
-
 #### JSON
 
 ```json
 {
     "code": 200,
     "status": true,
     "items": [
```

### Comparing `gpti-1.9/README.md` & `gpti-2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 ## Available Models
 
 GPTI provides access to a variety of artificial intelligence models to meet various needs. Currently, the available models include:
 
 - [**ChatGPT**](#gpt)
 - [**ChatGPT v2**](#gpt-v2)
 - [**ChatGPT Web**](#gptweb)
-- [**ChatGPT Prompts**](#gpt-prompts)
 - [**Bing**](#bing)
 - [**LLaMA-2**](#llama2)
 - [**DALL·E**](#dalle)
 - [**DALL-E 2**](#dalle2) (PRO)
 - [**DALL-E Mini**](#dalle-mini)
 - [**Prodia**](#prodia)
 - [**Prodia Stable-Diffusion**](#prodia-stablediffusion)
@@ -183,15 +182,15 @@
         "role": "assistant",
         "content": "Hello, Yandri! How are you today?"
     },
     {
         "role": "user",
         "content": "Can you repeat my name?"
     }
-], markdown=True, stream=False)
+], markdown=False, stream=False)
 
 if res.error != None:
     print(json.dumps(res.error))
 else:
     for chunk in res.stream():
         print(json.dumps(chunk))
 ```
@@ -242,29 +241,14 @@
     "code": 200,
     "status": true,
     "gpt": "Yes, I am familiar with the movie Wonka released in 2023. Wonka is a musical fantasy film directed by Paul King, adapted from the character at the center of Roald Dahl's iconic children's book, \"Charlie and the Chocolate Factory.\" The film follows the story of a young and poor Willy Wonka as he dreams of opening a shop in a chocolate-renowned city and discovers that the industry is controlled by a greedy cartel. The film has a rating of 7.1/10 and has received positive reviews with a score of 83% on Rotten Tomatoes. It was released on December 15, 2023, and has earned $552.1 million at the box office. The cast includes actors such as Timothée Chalamet. Unfortunately, I couldn't find information on whether the movie is available on Netflix.",
     "original": null
 }
 ```
 
-<a id="gpt-prompts"></a>
-## Usage GPT Prompts
-
-```python
-import json
-from gpti import gpt
-
-res = gpt.prompts(lang="en", limit=4, offset=0)
-
-if res.error != None:
-    print(json.dumps(res.error))
-else: 
-    print(json.dumps(res.result))
-```
-
 #### JSON
 
 ```json
 {
     "code": 200,
     "status": true,
     "items": [
```

### Comparing `gpti-1.9/gpti/__init__.py` & `gpti-2.0/gpti/__init__.py`

 * *Files identical despite different names*

### Comparing `gpti-1.9/gpti.egg-info/PKG-INFO` & `gpti-2.0/gpti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpti
-Version: 1.9
+Version: 2.0
 Summary: This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT
 Home-page: https://github.com/yandricr/gpti-py/
 Author: yandricr
 Author-email: yandribret@gmail.com
 License: MIT
 Project-URL: Documentation, https://nexra.aryahcr.cc/
 Project-URL: Funding, https://ko-fi.com/yandricr
@@ -32,15 +32,14 @@
 ## Available Models
 
 GPTI provides access to a variety of artificial intelligence models to meet various needs. Currently, the available models include:
 
 - [**ChatGPT**](#gpt)
 - [**ChatGPT v2**](#gpt-v2)
 - [**ChatGPT Web**](#gptweb)
-- [**ChatGPT Prompts**](#gpt-prompts)
 - [**Bing**](#bing)
 - [**LLaMA-2**](#llama2)
 - [**DALL·E**](#dalle)
 - [**DALL-E 2**](#dalle2) (PRO)
 - [**DALL-E Mini**](#dalle-mini)
 - [**Prodia**](#prodia)
 - [**Prodia Stable-Diffusion**](#prodia-stablediffusion)
@@ -199,15 +198,15 @@
         "role": "assistant",
         "content": "Hello, Yandri! How are you today?"
     },
     {
         "role": "user",
         "content": "Can you repeat my name?"
     }
-], markdown=True, stream=False)
+], markdown=False, stream=False)
 
 if res.error != None:
     print(json.dumps(res.error))
 else:
     for chunk in res.stream():
         print(json.dumps(chunk))
 ```
@@ -258,29 +257,14 @@
     "code": 200,
     "status": true,
     "gpt": "Yes, I am familiar with the movie Wonka released in 2023. Wonka is a musical fantasy film directed by Paul King, adapted from the character at the center of Roald Dahl's iconic children's book, \"Charlie and the Chocolate Factory.\" The film follows the story of a young and poor Willy Wonka as he dreams of opening a shop in a chocolate-renowned city and discovers that the industry is controlled by a greedy cartel. The film has a rating of 7.1/10 and has received positive reviews with a score of 83% on Rotten Tomatoes. It was released on December 15, 2023, and has earned $552.1 million at the box office. The cast includes actors such as Timothée Chalamet. Unfortunately, I couldn't find information on whether the movie is available on Netflix.",
     "original": null
 }
 ```
 
-<a id="gpt-prompts"></a>
-## Usage GPT Prompts
-
-```python
-import json
-from gpti import gpt
-
-res = gpt.prompts(lang="en", limit=4, offset=0)
-
-if res.error != None:
-    print(json.dumps(res.error))
-else: 
-    print(json.dumps(res.result))
-```
-
 #### JSON
 
 ```json
 {
     "code": 200,
     "status": true,
     "items": [
```

### Comparing `gpti-1.9/setup.py` & `gpti-2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as f:
         _long_description = f.read()
 except Exception as e:
     _long_description = ''
 
 setup(
     name='gpti',
-    version='1.9',
+    version='2.0',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='yandricr',
     author_email='yandribret@gmail.com',
     description='This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT',
```

