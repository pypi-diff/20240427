# Comparing `tmp/openai_api_with_easy_tools_and_web_browsing-1.0.2.tar.gz` & `tmp/openai_api_with_easy_tools_and_web_browsing-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_with_easy_tools_and_web_browsing-1.0.2.tar", last modified: Sat Apr 27 14:58:18 2024, max compression
+gzip compressed data, was "openai_api_with_easy_tools_and_web_browsing-1.0.3.tar", last modified: Sat Apr 27 15:17:53 2024, max compression
```

## Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.2.tar` & `openai_api_with_easy_tools_and_web_browsing-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 14:58:18.630079 openai_api_with_easy_tools_and_web_browsing-1.0.2/
--rw-rw-rw-   0        0        0     1087 2024-04-26 15:11:03.000000 openai_api_with_easy_tools_and_web_browsing-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4311 2024-04-27 14:58:18.630079 openai_api_with_easy_tools_and_web_browsing-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3584 2024-04-27 14:55:48.000000 openai_api_with_easy_tools_and_web_browsing-1.0.2/README.md
--rw-rw-rw-   0        0        0      713 2024-04-27 14:57:55.000000 openai_api_with_easy_tools_and_web_browsing-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 14:58:18.630079 openai_api_with_easy_tools_and_web_browsing-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-27 14:58:18.614050 openai_api_with_easy_tools_and_web_browsing-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 14:58:18.630079 openai_api_with_easy_tools_and_web_browsing-1.0.2/src/openai_api_with_easy_tools_and_web_browsing.egg-info/
--rw-rw-rw-   0        0        0     4311 2024-04-27 14:58:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.2/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2024-04-27 14:58:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.2/src/openai_api_with_easy_tools_and_web_browsing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 14:58:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.2/src/openai_api_with_easy_tools_and_web_browsing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-27 14:58:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.2/src/openai_api_with_easy_tools_and_web_browsing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11022 2024-04-27 14:20:05.000000 openai_api_with_easy_tools_and_web_browsing-1.0.2/src/openai_api_with_easy_tools_and_web_browsing.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:58:18.630079 openai_api_with_easy_tools_and_web_browsing-1.0.2/tests/
--rw-rw-rw-   0        0        0     2851 2024-04-27 14:57:27.000000 openai_api_with_easy_tools_and_web_browsing-1.0.2/tests/test.py
--rw-rw-rw-   0        0        0     3073 2024-04-27 14:57:27.000000 openai_api_with_easy_tools_and_web_browsing-1.0.2/tests/test_fr.py
+drwxrwxrwx   0        0        0        0 2024-04-27 15:17:53.368651 openai_api_with_easy_tools_and_web_browsing-1.0.3/
+-rw-rw-rw-   0        0        0     1087 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4568 2024-04-27 15:17:53.366649 openai_api_with_easy_tools_and_web_browsing-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3841 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/README.md
+-rw-rw-rw-   0        0        0      715 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 15:17:53.368651 openai_api_with_easy_tools_and_web_browsing-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 15:17:53.344296 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 15:17:53.366649 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/
+-rw-rw-rw-   0        0        0     4568 2024-04-27 15:17:53.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2024-04-27 15:17:53.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 15:17:53.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-27 15:17:53.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11022 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.py
+drwxrwxrwx   0        0        0        0 2024-04-27 15:17:53.360646 openai_api_with_easy_tools_and_web_browsing-1.0.3/tests/
+-rw-rw-rw-   0        0        0     2851 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/tests/test.py
+-rw-rw-rw-   0        0        0     2990 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/tests/test_fr.py
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.2/LICENSE` & `openai_api_with_easy_tools_and_web_browsing-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.2/PKG-INFO` & `openai_api_with_easy_tools_and_web_browsing-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_with_easy_tools_and_web_browsing
-Version: 1.0.2
+Version: 1.0.3
 Summary: An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools
 Author-email: ThomLecha <hamster12@hotmail.fr>
 Project-URL: Homepage, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing
 Project-URL: Issues, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,16 +12,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openai-api-with-easy-tools-and-web-browsing
 An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools.
 
 Here is an example of capabilities of this library:
+
 If you ask the program:
 *Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result*
+
 The response, using a web search and a custom tool to add two numbers, should be something like:
 *The total population of Paris and New York in 2015 was about 31,082,144 inhabitants. If 10,000,000 is added to this number, it becomes 41,082,144.*
 
 See code below to reproduce this example.
 
 First, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
 
@@ -75,14 +77,16 @@
 openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Return a response to a prompt in 'ponctual' mode ###
 print("\n\n\nPONCTUAL MODE\n")
 prompt = "Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result"
 # Use the 'getLLMAnswerWithWebBrowsingAndTools' function to get a response from a user message
 answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+# The response, using a web search and a custom tool to add two numbers, should be something like:
+# "The total population of Paris and New York in 2015 was about 31,082,144 inhabitants.
+# If 10,000,000 is added to this number, it becomes 41,082,144."
 print(answer)
 
 ### Discussion in 'continuous' mode ###
 print("\n\n\nCONTINUOUS MODE\n")
 openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
-
 ```
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.2/README.md` & `openai_api_with_easy_tools_and_web_browsing-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # openai-api-with-easy-tools-and-web-browsing
 An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools.
 
 Here is an example of capabilities of this library:
+
 If you ask the program:
 *Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result*
+
 The response, using a web search and a custom tool to add two numbers, should be something like:
 *The total population of Paris and New York in 2015 was about 31,082,144 inhabitants. If 10,000,000 is added to this number, it becomes 41,082,144.*
 
 See code below to reproduce this example.
 
 First, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
 
@@ -61,14 +63,16 @@
 openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Return a response to a prompt in 'ponctual' mode ###
 print("\n\n\nPONCTUAL MODE\n")
 prompt = "Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result"
 # Use the 'getLLMAnswerWithWebBrowsingAndTools' function to get a response from a user message
 answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+# The response, using a web search and a custom tool to add two numbers, should be something like:
+# "The total population of Paris and New York in 2015 was about 31,082,144 inhabitants.
+# If 10,000,000 is added to this number, it becomes 41,082,144."
 print(answer)
 
 ### Discussion in 'continuous' mode ###
 print("\n\n\nCONTINUOUS MODE\n")
 openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
-
 ```
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.2/pyproject.toml` & `openai_api_with_easy_tools_and_web_browsing-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openai_api_with_easy_tools_and_web_browsing"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="ThomLecha", email="hamster12@hotmail.fr" },
 ]
 description = "An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools"
 
 readme = "README.md"
 requires-python = ">=3.8"
@@ -12,8 +12,8 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing"
-Issues = "https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing/issues"
+Issues = "https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing/issues"
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.2/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO` & `openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_with_easy_tools_and_web_browsing
-Version: 1.0.2
+Version: 1.0.3
 Summary: An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools
 Author-email: ThomLecha <hamster12@hotmail.fr>
 Project-URL: Homepage, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing
 Project-URL: Issues, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,16 +12,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openai-api-with-easy-tools-and-web-browsing
 An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools.
 
 Here is an example of capabilities of this library:
+
 If you ask the program:
 *Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result*
+
 The response, using a web search and a custom tool to add two numbers, should be something like:
 *The total population of Paris and New York in 2015 was about 31,082,144 inhabitants. If 10,000,000 is added to this number, it becomes 41,082,144.*
 
 See code below to reproduce this example.
 
 First, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
 
@@ -75,14 +77,16 @@
 openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Return a response to a prompt in 'ponctual' mode ###
 print("\n\n\nPONCTUAL MODE\n")
 prompt = "Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result"
 # Use the 'getLLMAnswerWithWebBrowsingAndTools' function to get a response from a user message
 answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+# The response, using a web search and a custom tool to add two numbers, should be something like:
+# "The total population of Paris and New York in 2015 was about 31,082,144 inhabitants.
+# If 10,000,000 is added to this number, it becomes 41,082,144."
 print(answer)
 
 ### Discussion in 'continuous' mode ###
 print("\n\n\nCONTINUOUS MODE\n")
 openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
-
 ```
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.2/src/openai_api_with_easy_tools_and_web_browsing.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.py`

 * *Files identical despite different names*

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.2/tests/test.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.2/tests/test_fr.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.3/tests/test_fr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import src.openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
 
 # On entre nos clés d'API
-subscriptionKey = "17c15909de1e49d6936f171edf3b7fa8"
-openAIAPIKey = "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"
+subscriptionKey = ""
+openAIAPIKey = ""
 
 ### Création de l'outil de recherche Bing ###
 
 # On crée un moteur de recherche Bing qui synthétise les résultats avec GPT-3.5-turbo
 bingSearchEngine = webBrowsingApiGPT.BingSearchEngine(openAIAPIKey, subscriptionKey, model="gpt-3.5-turbo")
 # On renomme la fonction de recherche Bing (sinon cela ne fonctionne pas en tant que tool dans l'API d'OpenAI)
 bingSearch = bingSearchEngine.bingSearch
```

