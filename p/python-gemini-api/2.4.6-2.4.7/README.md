# Comparing `tmp/python_gemini_api-2.4.6.tar.gz` & `tmp/python_gemini_api-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_gemini_api-2.4.6.tar", last modified: Wed Apr 24 13:05:42 2024, max compression
+gzip compressed data, was "python_gemini_api-2.4.7.tar", last modified: Sat Apr 27 13:17:03 2024, max compression
```

## Comparing `python_gemini_api-2.4.6.tar` & `python_gemini_api-2.4.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.695928 python_gemini_api-2.4.6/
--rw-rw-rw-   0        0        0     1097 2024-04-24 10:59:38.000000 python_gemini_api-2.4.6/LICENSE
--rw-rw-rw-   0        0        0    36565 2024-04-24 13:05:42.693663 python_gemini_api-2.4.6/PKG-INFO
--rw-rw-rw-   0        0        0    35262 2024-04-24 10:16:55.000000 python_gemini_api-2.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.632745 python_gemini_api-2.4.6/gemini/
--rw-rw-rw-   0        0        0     1511 2024-04-24 13:05:29.000000 python_gemini_api-2.4.6/gemini/__init__.py
--rw-rw-rw-   0        0        0    15192 2024-03-18 04:20:24.000000 python_gemini_api-2.4.6/gemini/async_client.py
--rw-rw-rw-   0        0        0    19096 2024-04-17 13:21:33.000000 python_gemini_api-2.4.6/gemini/client.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.634745 python_gemini_api-2.4.6/gemini/src/
--rw-rw-rw-   0        0        0        0 2024-03-05 10:25:37.000000 python_gemini_api-2.4.6/gemini/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.638765 python_gemini_api-2.4.6/gemini/src/extensions/
--rw-rw-rw-   0        0        0       40 2024-03-16 06:40:55.000000 python_gemini_api-2.4.6/gemini/src/extensions/__init__.py
--rw-rw-rw-   0        0        0      622 2024-03-18 04:30:10.000000 python_gemini_api-2.4.6/gemini/src/extensions/replit.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.648091 python_gemini_api-2.4.6/gemini/src/misc/
--rw-rw-rw-   0        0        0      265 2024-04-17 09:46:31.000000 python_gemini_api-2.4.6/gemini/src/misc/__init__.py
--rw-rw-rw-   0        0        0     9279 2024-04-05 10:13:11.000000 python_gemini_api-2.4.6/gemini/src/misc/constants.py
--rw-rw-rw-   0        0        0     3063 2024-03-18 04:29:01.000000 python_gemini_api-2.4.6/gemini/src/misc/decorator.py
--rw-rw-rw-   0        0        0     2421 2024-04-20 13:54:53.000000 python_gemini_api-2.4.6/gemini/src/misc/exceptions.py
--rw-rw-rw-   0        0        0     4487 2024-04-17 09:46:59.000000 python_gemini_api-2.4.6/gemini/src/misc/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.654773 python_gemini_api-2.4.6/gemini/src/model/
--rw-rw-rw-   0        0        0       88 2024-03-16 06:40:55.000000 python_gemini_api-2.4.6/gemini/src/model/__init__.py
--rw-rw-rw-   0        0        0     8611 2024-03-18 04:29:31.000000 python_gemini_api-2.4.6/gemini/src/model/image.py
--rw-rw-rw-   0        0        0     1858 2024-03-31 11:20:09.000000 python_gemini_api-2.4.6/gemini/src/model/output.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.662227 python_gemini_api-2.4.6/gemini/src/model/parser/
--rw-rw-rw-   0        0        0      130 2024-03-17 09:52:54.000000 python_gemini_api-2.4.6/gemini/src/model/parser/__init__.py
--rw-rw-rw-   0        0        0     1490 2024-03-05 10:15:40.000000 python_gemini_api-2.4.6/gemini/src/model/parser/base.py
--rw-rw-rw-   0        0        0     5433 2024-03-31 11:20:09.000000 python_gemini_api-2.4.6/gemini/src/model/parser/custom_parser.py
--rw-rw-rw-   0        0        0     7692 2024-03-31 11:20:09.000000 python_gemini_api-2.4.6/gemini/src/model/parser/response_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.664369 python_gemini_api-2.4.6/gemini/src/modules/
--rw-rw-rw-   0        0        0        0 2024-03-29 00:25:32.000000 python_gemini_api-2.4.6/gemini/src/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.672401 python_gemini_api-2.4.6/gemini/src/modules/openrouter/
--rw-rw-rw-   0        0        0      102 2024-04-21 13:59:49.000000 python_gemini_api-2.4.6/gemini/src/modules/openrouter/__init__.py
--rw-rw-rw-   0        0        0     3048 2024-04-24 12:55:46.000000 python_gemini_api-2.4.6/gemini/src/modules/openrouter/async_client.py
--rw-rw-rw-   0        0        0     4753 2024-04-24 12:56:08.000000 python_gemini_api-2.4.6/gemini/src/modules/openrouter/client.py
--rw-rw-rw-   0        0        0      501 2024-04-24 12:55:26.000000 python_gemini_api-2.4.6/gemini/src/modules/openrouter/const.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.677577 python_gemini_api-2.4.6/gemini/src/modules/voice/
--rw-rw-rw-   0        0        0       88 2024-03-18 04:18:39.000000 python_gemini_api-2.4.6/gemini/src/modules/voice/__init__.py
--rw-rw-rw-   0        0        0     2441 2024-03-18 04:18:26.000000 python_gemini_api-2.4.6/gemini/src/modules/voice/google.py
--rw-rw-rw-   0        0        0     3144 2024-03-17 14:01:32.000000 python_gemini_api-2.4.6/gemini/src/modules/voice/openai.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.691491 python_gemini_api-2.4.6/python_gemini_api.egg-info/
--rw-rw-rw-   0        0        0    36565 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1102 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      111 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 13:05:42.695928 python_gemini_api-2.4.6/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-04-24 10:59:38.000000 python_gemini_api-2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.538878 python_gemini_api-2.4.7/
+-rw-rw-rw-   0        0        0     1097 2024-04-24 10:59:38.000000 python_gemini_api-2.4.7/LICENSE
+-rw-rw-rw-   0        0        0    36504 2024-04-27 13:17:03.537298 python_gemini_api-2.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0    35177 2024-04-27 13:15:58.000000 python_gemini_api-2.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.475836 python_gemini_api-2.4.7/gemini/
+-rw-rw-rw-   0        0        0     1511 2024-04-27 13:15:12.000000 python_gemini_api-2.4.7/gemini/__init__.py
+-rw-rw-rw-   0        0        0    15192 2024-03-18 04:20:24.000000 python_gemini_api-2.4.7/gemini/async_client.py
+-rw-rw-rw-   0        0        0    19096 2024-04-17 13:21:33.000000 python_gemini_api-2.4.7/gemini/client.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.477836 python_gemini_api-2.4.7/gemini/src/
+-rw-rw-rw-   0        0        0        0 2024-03-05 10:25:37.000000 python_gemini_api-2.4.7/gemini/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.482330 python_gemini_api-2.4.7/gemini/src/extensions/
+-rw-rw-rw-   0        0        0       40 2024-03-16 06:40:55.000000 python_gemini_api-2.4.7/gemini/src/extensions/__init__.py
+-rw-rw-rw-   0        0        0      622 2024-03-18 04:30:10.000000 python_gemini_api-2.4.7/gemini/src/extensions/replit.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.491676 python_gemini_api-2.4.7/gemini/src/misc/
+-rw-rw-rw-   0        0        0      265 2024-04-17 09:46:31.000000 python_gemini_api-2.4.7/gemini/src/misc/__init__.py
+-rw-rw-rw-   0        0        0     9279 2024-04-05 10:13:11.000000 python_gemini_api-2.4.7/gemini/src/misc/constants.py
+-rw-rw-rw-   0        0        0     3063 2024-03-18 04:29:01.000000 python_gemini_api-2.4.7/gemini/src/misc/decorator.py
+-rw-rw-rw-   0        0        0     2421 2024-04-20 13:54:53.000000 python_gemini_api-2.4.7/gemini/src/misc/exceptions.py
+-rw-rw-rw-   0        0        0     4487 2024-04-17 09:46:59.000000 python_gemini_api-2.4.7/gemini/src/misc/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.496863 python_gemini_api-2.4.7/gemini/src/model/
+-rw-rw-rw-   0        0        0       88 2024-03-16 06:40:55.000000 python_gemini_api-2.4.7/gemini/src/model/__init__.py
+-rw-rw-rw-   0        0        0     8611 2024-03-18 04:29:31.000000 python_gemini_api-2.4.7/gemini/src/model/image.py
+-rw-rw-rw-   0        0        0     1858 2024-03-31 11:20:09.000000 python_gemini_api-2.4.7/gemini/src/model/output.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.503762 python_gemini_api-2.4.7/gemini/src/model/parser/
+-rw-rw-rw-   0        0        0      130 2024-03-17 09:52:54.000000 python_gemini_api-2.4.7/gemini/src/model/parser/__init__.py
+-rw-rw-rw-   0        0        0     1490 2024-03-05 10:15:40.000000 python_gemini_api-2.4.7/gemini/src/model/parser/base.py
+-rw-rw-rw-   0        0        0     5433 2024-03-31 11:20:09.000000 python_gemini_api-2.4.7/gemini/src/model/parser/custom_parser.py
+-rw-rw-rw-   0        0        0     7692 2024-03-31 11:20:09.000000 python_gemini_api-2.4.7/gemini/src/model/parser/response_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.506158 python_gemini_api-2.4.7/gemini/src/modules/
+-rw-rw-rw-   0        0        0        0 2024-03-29 00:25:32.000000 python_gemini_api-2.4.7/gemini/src/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.513313 python_gemini_api-2.4.7/gemini/src/modules/openrouter/
+-rw-rw-rw-   0        0        0      102 2024-04-21 13:59:49.000000 python_gemini_api-2.4.7/gemini/src/modules/openrouter/__init__.py
+-rw-rw-rw-   0        0        0     3048 2024-04-27 13:13:20.000000 python_gemini_api-2.4.7/gemini/src/modules/openrouter/async_client.py
+-rw-rw-rw-   0        0        0     4753 2024-04-24 12:56:08.000000 python_gemini_api-2.4.7/gemini/src/modules/openrouter/client.py
+-rw-rw-rw-   0        0        0      505 2024-04-24 13:06:12.000000 python_gemini_api-2.4.7/gemini/src/modules/openrouter/const.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.518672 python_gemini_api-2.4.7/gemini/src/modules/voice/
+-rw-rw-rw-   0        0        0       88 2024-03-18 04:18:39.000000 python_gemini_api-2.4.7/gemini/src/modules/voice/__init__.py
+-rw-rw-rw-   0        0        0     2441 2024-03-18 04:18:26.000000 python_gemini_api-2.4.7/gemini/src/modules/voice/google.py
+-rw-rw-rw-   0        0        0     3144 2024-03-17 14:01:32.000000 python_gemini_api-2.4.7/gemini/src/modules/voice/openai.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.534679 python_gemini_api-2.4.7/python_gemini_api.egg-info/
+-rw-rw-rw-   0        0        0    36504 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 13:17:03.538878 python_gemini_api-2.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     2204 2024-04-27 13:14:03.000000 python_gemini_api-2.4.7/setup.py
```

### Comparing `python_gemini_api-2.4.6/LICENSE` & `python_gemini_api-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/PKG-INFO` & `python_gemini_api-2.4.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gemini-api
-Version: 2.4.6
+Version: 2.4.7
 Summary: The python package that returns Response of Google Gemini through API.
 Home-page: https://github.com/dsdanielpark/Gemini-API
 Author: Daniel Park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -20,14 +20,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx[http2]>=0.20.0
 Requires-Dist: requests
 Requires-Dist: browser_cookie3
 Requires-Dist: loguru
 Requires-Dist: pydantic
+Requires-Dist: aiohttp
 Provides-Extra: voice
 Requires-Dist: gTTS; extra == "voice"
 Requires-Dist: SpeechRecognition; extra == "voice"
 Requires-Dist: openai; extra == "voice"
 Requires-Dist: anthropic; extra == "voice"
 
 
@@ -47,18 +48,17 @@
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-ba79-d9f89b637324
 
 
 
 
 
 
-A *unofficial* Python wrapper, [python-gemini-api](https://pypi.org/project/python-gemini-api/), operates through reverse-engineering, utilizing cookie values to interact with [Google Gemini](https://gemini.google.com) for users struggling with frequent authentication problems or unable to authenticate via [Google Authentication](https://developers.google.com/identity/protocols/oauth2?hl=en).
-
-Collaborated competently with [Antonio Cheong](https://github.com/acheong08).
+An **unofficial* Python wrapper, [python-gemini-api](https://pypi.org/project/python-gemini-api/), is available for users facing frequent authentication issues or unable to use [Google Authentication](https://developers.google.com/identity/protocols/oauth2?hl=en). This wrapper uses cookie values to interact with [Google Gemini](https://gemini.google.com) through reverse-engineering. The project involved a collaboration with [Antonio Cheong](https://github.com/acheong08).
 
+On the official side, Google provides partially free, clean [official Gemini APIs and SDKs](https://aistudio.google.com/), which can be accessed and utilized neatly via Python packages, [google-generativeai](https://pypi.org/project/google-generativeai/). 
 <br>
 
 <br>
 
 
 > [!TIP]
 > | 2024-03-26 | [[See Code Examples]](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md)
@@ -137,21 +137,22 @@
 
 ## Authentication
 
 1. Visit https://gemini.google.com/ <br>
     With browser open, try auto-collecting cookies first.
     ```python
     from gemini import Gemini
-    GeminiClient = Gemini(auto_cookies=True)
+    
+    client = Gemini(auto_cookies=True)
 
     # Testing needed as cookies vary by region.
-    # GeminiClient = Gemini(auto_cookies=True, target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"])
-    # GeminiClient = Gemini(auto_cookies=True, target_cookies="all") # You can pass whole cookies
+    # client = Gemini(auto_cookies=True, target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"])
+    # client = Gemini(auto_cookies=True, target_cookies="all") # You can pass whole cookies
 
-    response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
+    response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
     print(response.payload)
     ```
 2. *(Manually)* `F12` for browser console → `Session: Application` → `Cookies` → Copy the value of some working cookie sets. If it doesn't work, go to step 3.
     <details><summary>Some working cookie sets</summary>
     Cookies may vary by account or region. 
       
     First try `__Secure-1PSIDCC` alone. If it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success? Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the entire cookie file.
@@ -178,29 +179,29 @@
 
 ## Quick Start
 
 **Generate content:** returns parsed response.
 ```python
 from gemini import Gemini
 
-cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
-GeminiClient = Gemini(cookies=cookies) # You can use various args
+cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+client = Gemini(cookies=cookies) # You can use various args
 
-response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
+response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 response.payload
 ```
 
 **Generate content from image:** you can use image as input.
 ```python
 from gemini import Gemini
 
-cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
+cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+client = Gemini(cookies=cookies) # You can use various args
 
-GeminiClient = Gemini(cookies=cookies) # You can use various args
-response = GeminiClient.generate_content("What does the text in this image say?", image='folder/image.jpg')
+response = client.generate_content("What does the text in this image say?", image='folder/image.jpg')
 response.payload
 ```
 
 > [!NOTE] 
 > If the generate_content method returns an empty payload, try executing it again without reinitializing the Gemini object.
 
 <br><br>
@@ -209,14 +210,15 @@
 
 *Setting language and Gemini version using environment variables:*
 
 Setting Gemini response language (Optional): Check supported languages [here](https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes). Default is English.
 
 ```python
 import os
+
 os.environ["GEMINI_LANGUAGE"] = "KR"  # Setting Gemini response language (Optional)
 os.environ["GEMINI_ULTRA"] = "1"      # Switch to Gemini-advanced response (Experimental, Optional)
 # In some accounts, access to Gemini Ultra may not be available. If that's the case, please revert it back to "0".
 ```
 
 
 
@@ -235,17 +237,17 @@
     "__Secure-1PSIDCC" : "value",
     "__Secure-1PSID" : "value",
     "__Secure-1PSIDTS" : "value",
     "NID" : "value",
     # Cookies may vary by account or region. Consider sending the entire cookie file.
   }
 
-GeminiClient = Gemini(cookies=cookies)
-# GeminiClient = Gemini(cookie_fp="folder/cookie_file.json") # (*.json, *.txt) are supported.
-# GeminiClient = Gemini(auto_cookies=True) # Or use auto_cookies paprameter
+client = Gemini(cookies=cookies)
+# client = Gemini(cookie_fp="folder/cookie_file.json") # (*.json, *.txt) are supported.
+# client = Gemini(auto_cookies=True) # Or use auto_cookies paprameter
 ```
 
 ##### Auto Cookie Update
 For `auto_cookie` to be set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3) enables automatic cookie collection, though updates may not be complete yet.
 
 
 
@@ -253,15 +255,15 @@
 
 ### # 02. Generate content
 Returns Gemini's response, but the first one might be empty. 
 
 
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
-response = GeminiClient.generate_content(prompt)
+response = client.generate_content(prompt)
 print(response.payload)
 ```
 
 
 > [!IMPORTANT]
 >  DO NOT send same prompt repeatly. **If the session connects successfully and `generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open in the browser, cookies may expire faster. 
 
@@ -284,41 +286,41 @@
 
 ### # 03. Send request
 Send request: returns the request's payload and status_code, making debugging easier.
 ```python
 from gemini import Gemini
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
-GeminiClient = Gemini(cookies=cookies) # You can use various args
+client = Gemini(cookies=cookies) # You can use various args
 
-response_text, response_status = GeminiClient.send_request("Hello, Gemini. What's the weather like in Seoul today?")
+response_text, response_status = client.send_request("Hello, Gemini. What's the weather like in Seoul today?")
 print(response_text)
 ```
 You can track the total number of requests made by accessing the `request_count` property within the `Gemini` class.
 
 <br>
 
 ### # 04. Text generation
 Returns text generated by Gemini.
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
-response = GeminiClient.generate_content(prompt)
+response = client.generate_content(prompt)
 print(response.text)
 ```
 
 
 <br>
 
 ### # 05. Image generation
 Returns images generated by Gemini.
 
 *Async downloader*
 
 ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 generated_images = response.generated_images # Check generated images [Dict]
 
 await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
 # image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
 # await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
@@ -341,15 +343,15 @@
   ```
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+response = client.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
 GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
 
 # You can use byte type image dict for printing images as follow:
 # bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
 # GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
@@ -397,15 +399,15 @@
 
 ### # 06. Retrieving Images from Gemini Responses
 Returns images in response of Gemini.
 
 
 *Async downloader*
 ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 response_images = response.web_images # Check generated images [Dict]
 
 await GeminiImage.save(response_images, "save_dir")
 # image_data_dict = await GeminiImage.fetch_images_dict(response_images)
 # await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
@@ -413,15 +415,15 @@
 <details><summary>Further</summary>
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
-response = GeminiClient.generate_content("Please recommend a travel itinerary for Seoul.")
+response = client.generate_content("Please recommend a travel itinerary for Seoul.")
 response_images = response.web_images # Check response images [Dict]
 
 GeminiImage.save_sync(response_images, save_path="save_dir")
 
 # You can use byte type image dict as follow:
 # bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
 # GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
@@ -465,29 +467,29 @@
 ### # 07. Generate content from images
 Takes an image as input and returns a response.
 
 ```python
 image = 'folder/image.jpg'
 # image = open('folder/image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported.
 
-response = GeminiClient.generate_content("What does the text in this image say?", image=image)
+response = client.generate_content("What does the text in this image say?", image=image)
 response.response_dict
 ```
 
 <br>
 
 ### # 08. Generate content using Google Services
 To begin, you must link Google Workspace to activate this extension via the [Gemini web extension](https://gemini.google.com/extensions). Please refer to the [official notice](https://support.google.com/gemini/answer/13695044) and review the [privacy policies](https://support.google.com/gemini/answer/13594961?visit_id=638457301410420313-1578971242&p=privacy_help&rd=1) for more details.
 
 *extention flags*
 ```
 @Gmail, @Google Drive, @Google Docs, @Google Maps, @Google Flights, @Google Hotels, @YouTube
 ```
 ```python
-response = GeminiClient.generate_content("@YouTube Search clips related with Google Gemini")
+response = client.generate_content("@YouTube Search clips related with Google Gemini")
 response.response_dict
 ```
 <details><summary>Extension description</summary>
   
 - Google Workspace
   - Services: **@Gmail, @Google Drive, @Google Docs** 
   - Description: Summarize, search, and find desired information quickly in your content for efficient personal task management.
@@ -518,36 +520,36 @@
 
 
 ### # 09. Fix context setting RCID
 You can specify a particular response by setting its Response Candidate ID(RCID).
 
 ```python
 # Generate content for the prompt "Give me some information about the USA."
-response1 = GeminiClient.generate_content("Give me some information about the USA.")
+response1 = client.generate_content("Give me some information about the USA.")
 # After reviewing the responses, choose the one you prefer and copy its RCID.
-GeminiClient.rcid = "rc_xxxx"
+client.rcid = "rc_xxxx"
 
 # Now, generate content for the next prompt "How long does it take from LA to New York?"
-response2 = GeminiClient.generate_content("How long does it take from LA to New York?")
+response2 = client.generate_content("How long does it take from LA to New York?")
 
-# However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to None.
-# GeminiClient.rcid = None
+# However, RCID may not persist. If parsing fails, reset `client.rcid` to None.
+# client.rcid = None
 ```
 
 
 
 <br>
 
 ### # 10. Changing the Selected Response from 0 to *n*
 In Gemini, generate_content returns the first response. This may vary depending on length or sorting. Therefore, you can specify the index of the chosen response from 0 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python
 from gemini import GeminiModelOutput
 
 GeminiModelOutput.chosen = 1 # default is 0
-response_choice_1 = GeminiClient.generate_content("Give me some information about the USA.")
+response_choice_1 = client.generate_content("Give me some information about the USA.")
 
 # If not all Gemini returns are necessarily plural, revert back to 0 in case of errors.
 #  GeminiModelOutput.chosen = 0
 ```
 
 <br>
 
@@ -555,18 +557,18 @@
 Parse the response text to extract desired values.
 
 
 Using `Gemini.generate_custom_content`, specify custom parsing to extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and you can pass custom parsing methods as arguments if desired. Refer to [custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/src/model/parser/custom_parser.py).
 
 ```python
 # You can create a parser method that takes response_text as the input for custom_parser.
-response_text, response_status = GeminiClient.send_request("Give me some information about the USA.")
+response_text, response_status = client.send_request("Give me some information about the USA.")
 
 # Use custom_parser function or class inheriting from BaseParser
-response = GeminiClient.generate_custom_content("Give me some information about the USA.", *custom_parser)
+response = client.generate_custom_content("Give me some information about the USA.", *custom_parser)
 ```
 
 https://github.com/dsdanielpark/Gemini-API/blob/31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 <br>
 
 ## Further
 
@@ -575,16 +577,16 @@
 If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks.
 
 ```python
 # Get your proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/
 proxy_url = "http://xxxxx:@smartproxy.crawlbase.com:8012" 
 proxies = {"http": proxy_url, "https": proxy_url}
 
-GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
-GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
+client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
 ```
 
 ### Reusable session object
 For standard cases, use Gemini class; for exceptions, use session objects. When creating a new bot Gemini server, adjust Headers.MAIN.
 ```python
 import requests
 from gemini import Gemini, Headers
@@ -592,16 +594,16 @@
 cookies = {} 
 
 session = requests.Session()
 session.headers = Headers.MAIN
 for key, value in cookies.items():
     session.cookies.update({key: value})
 
-GeminiClient = Gemini(session=session) # You can use various args
-response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
+client = Gemini(session=session) # You can use various args
+response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 ```
 
 
 
 
 <br>
 
@@ -665,21 +667,21 @@
 
 **Sync client is favored over async for Gemini due to rate limiting and blocking issues**, but OpenRouter offers reliable open-source LLMs for [async implementation](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md#openrouter-async-api-client).
 
 ```python
 from gemini import OpenRouter
 
 OPENROUTER_API_KEY = "<your_open_router_api_key>"
-GemmaClient = OpenRouter(api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free")
+gemma_client = OpenRouter(api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free")
 
 prompt = "Do you know UCA academy in Korea? https://blog.naver.com/ulsancoding"
-response = GemmaClient.create_chat_completion(prompt)
+response = gemma_client.create_chat_completion(prompt)
 print(response)
 
-# payload = GemmaClient.generate_content(prompt)
+# payload = gemma_client.generate_content(prompt)
 # print(payload.json())
 ```
 
 The free model list includes:
    - `google/gemma-7b-it:free` - [google/gemma-7b](https://huggingface.co/google/gemma-7b) from Google ***
    - `mistralai/mistral-7b-instruct:free` - [mistralai/Mistral-7B-Instruct-v0.1](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.1) for instruction from Mistral AI ****
    - `huggingfaceh4/zephyr-7b-beta:free` - [HuggingFaceH4/zephyr-7b-beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta) ***
@@ -742,27 +744,29 @@
 
 
 ## License ©️ 
 [MIT](https://opensource.org/license/mit/) license, 2024. We hereby strongly disclaim any explicit or implicit legal liability related to our works. Users are required to use this package responsibly and at their own risk. This project is a personal initiative and is not affiliated with or endorsed by Google. It is recommended to use Google's official API.
 
 
 ## References
-[1]: Paper - [Introducing GEMINI: Multimodal Generative Models](https://arxiv.org/abs/2312.11805) <br>
-[2]: Website - [Google DeepMind :: GEMINI Introduction](https://deepmind.google/technologies/gemini/#introduction) <br>
-[3]: Paper - [GEMMA: A Unified Language Model for Text Generation, Understanding, Translation, Coding, and Math.]() <br>
-[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/gemma/docs) <br>
-[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming Assignments](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email) <br>
-[6]: Blog Post - [Announcing CodeGen: Building Better Developers’ Tools Using LLMs](https://huggingface.co/blog/codegen) <br>
-[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf) <br>
-[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard) <br>
-[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) <br>
-[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API) <br>
-[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai) <br>
-[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner) <br>
-[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart) <br>
+1. [Introducing GEMINI: Multimodal Generative Models](https://arxiv.org/abs/2312.11805)
+2. [Google DeepMind: GEMINI Introduction](https://deepmind.google/technologies/gemini/#introduction)
+3. [GEMMA: A Unified Language Model for Text Generation, Understanding, Translation, Coding, and Math](https://arxiv.org/abs/2403.08295)
+4. [AI at Google: GEMS Documentation](https://ai.google.dev/gemma/docs)
+5. [CodeGMMA: Large Language Models Can Write Realistic Programming Assignments](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email)
+6. [Announcing CodeGen: Building Better Developers' Tools Using LLMs](https://huggingface.co/blog/codegen)
+7. [Google: CodeGen Release](https://huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf)
+8. [acheong08/Bard](https://github.com/acheong08/Bard)
+9. [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API)
+10. [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API)
+11. [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai)
+12. [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner)
+13. [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart)
+
+<br>
 
 
 > *Warning*
 Users assume full legal responsibility for GeminiAPI. Not endorsed by Google. Excessive use may lead to account restrictions. Changes in policies or account status may affect functionality. Utilize issue and discussion pages.
 
 <br>
```

#### html2text {}

```diff
@@ -1,37 +1,41 @@
-Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.6 Summary: The
+Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.7 Summary: The
 python package that returns Response of Google Gemini through API. Home-page:
 https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
 Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: httpx[http2]>=0.20.0 Requires-
 Dist: requests Requires-Dist: browser_cookie3 Requires-Dist: loguru Requires-
-Dist: pydantic Provides-Extra: voice Requires-Dist: gTTS; extra == "voice"
-Requires-Dist: SpeechRecognition; extra == "voice" Requires-Dist: openai; extra
-== "voice" Requires-Dist: anthropic; extra == "voice" # [Gemini Icon]Gemini API
-_[_P_y_P_I_]
+Dist: pydantic Requires-Dist: aiohttp Provides-Extra: voice Requires-Dist:
+gTTS; extra == "voice" Requires-Dist: SpeechRecognition; extra == "voice"
+Requires-Dist: openai; extra == "voice" Requires-Dist: anthropic; extra ==
+"voice" # [Gemini Icon]Gemini API_[_P_y_P_I_]
   _[_p_i_p_ _d_o_w_n_l_o_a_d_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
                 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_d_s_d_a_n_i_e_l_p_a_r_k_%_2_F_G_e_m_i_n_i_-
 _A_P_I_&_c_o_u_n_t___b_g_=_%_2_3_0_0_0_0_0_0_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_v_i_e_w_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]
                                                                     _[_D_o_w_n_l_o_a_d_s_]
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-
-ba79-d9f89b637324 A *unofficial* Python wrapper, [python-gemini-api](https://
-pypi.org/project/python-gemini-api/), operates through reverse-engineering,
-utilizing cookie values to interact with [Google Gemini](https://
-gemini.google.com) for users struggling with frequent authentication problems
-or unable to authenticate via [Google Authentication](https://
-developers.google.com/identity/protocols/oauth2?hl=en). Collaborated
-competently with [Antonio Cheong](https://github.com/acheong08).
+ba79-d9f89b637324 An **unofficial* Python wrapper, [python-gemini-api](https://
+pypi.org/project/python-gemini-api/), is available for users facing frequent
+authentication issues or unable to use [Google Authentication](https://
+developers.google.com/identity/protocols/oauth2?hl=en). This wrapper uses
+cookie values to interact with [Google Gemini](https://gemini.google.com)
+through reverse-engineering. The project involved a collaboration with [Antonio
+Cheong](https://github.com/acheong08). On the official side, Google provides
+partially free, clean [official Gemini APIs and SDKs](https://
+aistudio.google.com/), which can be accessed and utilized neatly via Python
+packages, [google-generativeai](https://pypi.org/project/google-generativeai/).
+
 
 > [!TIP] > | 2024-03-26 | [[See Code Examples]](https://github.com/
 dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md) > > Check out
 temporarily free Open-source LLM APIs with Open Router. (Free limit: 10
 requests/minute)
 ## Contents - [ Gemini API ](#-gemini-api---) - [What is Gemini? ð](#what-
 is-gemini) - [Installation â](#installation-) - [Authentication â]
@@ -88,24 +92,24 @@
 in REST format. **Synchronous clients are preferred over asynchronous ones for
 Gemini because of rate limiting and blocking concerns.** ## Installation ð¦
 ``` pip install python-gemini-api ``` ``` pip install git+https://github.com/
 dsdanielpark/Gemini-API.git ``` For the updated version, use as follows: ```
 pip install -q -U python-gemini-api ``` ## Authentication 1. Visit https://
 gemini.google.com/
 With browser open, try auto-collecting cookies first. ```python from gemini
-import Gemini GeminiClient = Gemini(auto_cookies=True) # Testing needed as
-cookies vary by region. # GeminiClient = Gemini(auto_cookies=True,
-target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"]) # GeminiClient = Gemini
-(auto_cookies=True, target_cookies="all") # You can pass whole cookies response
-= GeminiClient.generate_content("Hello, Gemini. What's the weather like in
-Seoul today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser
-console â `Session: Application` â `Cookies` â Copy the value of some
-working cookie sets. If it doesn't work, go to step 3. Some working cookie sets
-Cookies may vary by account or region. First try `__Secure-1PSIDCC` alone. If
-it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
+import Gemini client = Gemini(auto_cookies=True) # Testing needed as cookies
+vary by region. # client = Gemini(auto_cookies=True, target_cookies=["__Secure-
+1PSID", "__Secure-1PSIDTS"]) # client = Gemini(auto_cookies=True,
+target_cookies="all") # You can pass whole cookies response =
+client.generate_content("Hello, Gemini. What's the weather like in Seoul
+today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser console
+â `Session: Application` â `Cookies` â Copy the value of some working
+cookie sets. If it doesn't work, go to step 3. Some working cookie sets Cookies
+may vary by account or region. First try `__Secure-1PSIDCC` alone. If it
+doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
 Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-
 1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the
 entire cookie file. 3. *(Recommended)* Export Gemini site cookies via a browser
 extension. For instance, use Chrome extension [ExportThisCookies](https://
 chromewebstore.google.com/detail/exportthiscookie/
 dannllckdimllhkiplchkcaoheibealk), open, and copy the txt file contents.
 Further: For manual collection or Required for a few users upon error 4. For
@@ -122,25 +126,26 @@
 assistant.lamda.BardFrontendService/StreamGenerate" â Payload â Form Data
 â Copy the "at" key value. See [this image](assets/nonce_value.pdf) for
 reference. > [!IMPORTANT] > Experiment with different Google accounts and
 browser settings to find a working cookie. Success may vary by IP and account
 status. Once connected, a cookie typically remains effective over a month. Keep
 testing until successful.
 ## Quick Start **Generate content:** returns parsed response. ```python from
-gemini import Gemini cookies = {} # Cookies may vary by account or region.
-Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
-# You can use various args response = GeminiClient.generate_content("Hello,
-Gemini. What's the weather like in Seoul today?") response.payload ```
+gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
+or region. Consider sending the entire cookie file. client = Gemini
+(cookies=cookies) # You can use various args response = client.generate_content
+("Hello, Gemini. What's the weather like in Seoul today?") response.payload ```
 **Generate content from image:** you can use image as input. ```python from
-gemini import Gemini cookies = {} # Cookies may vary by account or region.
-Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
-# You can use various args response = GeminiClient.generate_content("What does
-the text in this image say?", image='folder/image.jpg') response.payload ``` >
-[!NOTE] > If the generate_content method returns an empty payload, try
-executing it again without reinitializing the Gemini object.
+gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
+or region. Consider sending the entire cookie file. client = Gemini
+(cookies=cookies) # You can use various args response = client.generate_content
+("What does the text in this image say?", image='folder/image.jpg')
+response.payload ``` > [!NOTE] > If the generate_content method returns an
+empty payload, try executing it again without reinitializing the Gemini object.
+
 
 ## Usage *Setting language and Gemini version using environment variables:
 * Setting Gemini response language (Optional): Check supported languages [here]
 (https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes).
 Default is English. ```python import os os.environ["GEMINI_LANGUAGE"] = "KR" #
 Setting Gemini response language (Optional) os.environ["GEMINI_ULTRA"] = "1" #
 Switch to Gemini-advanced response (Experimental, Optional) # In some accounts,
@@ -148,73 +153,71 @@
 it back to "0". ```
 ### # 01. Initialization Please explicitly declare `cookies` in dict format.
 You can also enter the path to the file containing the cookie with `cookie_fp`
 (*.json, *.txt supported). Check sample cookie files in [assets](https://
 github.com/dsdanielpark/Gemini-API/tree/main/assets) folder. ```python from
 gemini import Gemini cookies = { "__Secure-1PSIDCC" : "value", "__Secure-1PSID"
 : "value", "__Secure-1PSIDTS" : "value", "NID" : "value", # Cookies may vary by
-account or region. Consider sending the entire cookie file. } GeminiClient =
-Gemini(cookies=cookies) # GeminiClient = Gemini(cookie_fp="folder/
-cookie_file.json") # (*.json, *.txt) are supported. # GeminiClient = Gemini
-(auto_cookies=True) # Or use auto_cookies paprameter ``` ##### Auto Cookie
-Update For `auto_cookie` to be set to `True`, and adjust `target_cookies`.
-Gemini WebUI must be active in the browser. The [browser_cookie3](https://
-github.com/borisbabic/browser_cookie3) enables automatic cookie collection,
-though updates may not be complete yet.
+account or region. Consider sending the entire cookie file. } client = Gemini
+(cookies=cookies) # client = Gemini(cookie_fp="folder/cookie_file.json") #
+(*.json, *.txt) are supported. # client = Gemini(auto_cookies=True) # Or use
+auto_cookies paprameter ``` ##### Auto Cookie Update For `auto_cookie` to be
+set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the
+browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3)
+enables automatic cookie collection, though updates may not be complete yet.
 ### # 02. Generate content Returns Gemini's response, but the first one might
 be empty. ```python prompt = "Hello, Gemini. What's the weather like in Seoul
-today?" response = GeminiClient.generate_content(prompt) print
-(response.payload) ``` > [!IMPORTANT] > DO NOT send same prompt repeatly. **If
-the session connects successfully and `generate_content` runs well, CLOSE
-Gemini website.** If Gemini web stays open in the browser, cookies may expire
-faster.
+today?" response = client.generate_content(prompt) print(response.payload) ```
+> [!IMPORTANT] > DO NOT send same prompt repeatly. **If the session connects
+successfully and `generate_content` runs well, CLOSE Gemini website.** If
+Gemini web stays open in the browser, cookies may expire faster.
 The output of the generate_content function is `GeminiModelOutput`, with the
 following structure: - *rcid*: returns the response candidate id of the chosen
 candidate. - *text*: returns the text of the chosen candidate. - *code*:
 returns the codes of the chosen candidate. - *web_images*: returns a list of
 web images from the chosen candidate. - *generated_images*: returns a list of
 generated images from the chosen candidate. - *payload*: returns the response
 dictionary, if available. https://github.com/dsdanielpark/Gemini-API/blob/
 fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 ### # 03. Send request Send request: returns the request's payload and
 status_code, making debugging easier. ```python from gemini import Gemini
 cookies = {} # Cookies may vary by account or region. Consider sending the
-entire cookie file. GeminiClient = Gemini(cookies=cookies) # You can use
-various args response_text, response_status = GeminiClient.send_request("Hello,
-Gemini. What's the weather like in Seoul today?") print(response_text) ``` You
-can track the total number of requests made by accessing the `request_count`
-property within the `Gemini` class.
+entire cookie file. client = Gemini(cookies=cookies) # You can use various args
+response_text, response_status = client.send_request("Hello, Gemini. What's the
+weather like in Seoul today?") print(response_text) ``` You can track the total
+number of requests made by accessing the `request_count` property within the
+`Gemini` class.
 ### # 04. Text generation Returns text generated by Gemini. ```python prompt =
 "Hello, Gemini. What's the weather like in Seoul today?" response =
-GeminiClient.generate_content(prompt) print(response.text) ```
+client.generate_content(prompt) print(response.text) ```
 ### # 05. Image generation Returns images generated by Gemini. *Async
-downloader* ```python response = GeminiClient.generate_content("Create
-illustrations of Seoul, South Korea.") generated_images =
-response.generated_images # Check generated images [Dict] await
-GeminiImage.save(generated_images, "save_dir", cookies=cookies) #
-image_data_dict = await GeminiImage.fetch_images_dict(generated_images,
-cookies=cookies) # await GeminiImage.save_images(image_data_dict, "save_dir")
-``` Further *Display images in IPython* You can display the image or transmit
-it to another application in byte format. ```python bytes_images_dict =
-GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes
-images dict from IPython.display import display, Image import io for
-image_name, image_bytes in bytes_images_dict.items(): print(image_name) image =
-Image(data=image_bytes) display(image) ``` *Sync downloader* ```python from
-gemini import Gemini, GeminiImage response = GeminiClient.generate_content
-("Create illustrations of Seoul, South Korea.") generated_images =
-response.generated_images # Check generated images [Dict] GeminiImage.save_sync
-(generated_images, save_path="save_dir", cookies=cookies) # You can use byte
-type image dict for printing images as follow: # bytes_images_dict =
-GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
-bytes images dict # GeminiImage.save_images_sync(bytes_images_dict,
-path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
-```python import asyncio from gemini import Gemini, GeminiImage async def
-save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
-# Run the async function if __name__ == "__main__": cookies = {"key" : "value"}
+downloader* ```python response = client.generate_content("Create illustrations
+of Seoul, South Korea.") generated_images = response.generated_images # Check
+generated images [Dict] await GeminiImage.save(generated_images, "save_dir",
+cookies=cookies) # image_data_dict = await GeminiImage.fetch_images_dict
+(generated_images, cookies=cookies) # await GeminiImage.save_images
+(image_data_dict, "save_dir") ``` Further *Display images in IPython* You can
+display the image or transmit it to another application in byte format.
+```python bytes_images_dict = GeminiImage.fetch_images_dict_sync
+(generated_images, cookies) # Get bytes images dict from IPython.display import
+display, Image import io for image_name, image_bytes in bytes_images_dict.items
+(): print(image_name) image = Image(data=image_bytes) display(image) ``` *Sync
+downloader* ```python from gemini import Gemini, GeminiImage response =
+client.generate_content("Create illustrations of Seoul, South Korea.")
+generated_images = response.generated_images # Check generated images [Dict]
+GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+# You can use byte type image dict for printing images as follow: #
+bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images,
+cookies=cookies) # Get bytes images dict # GeminiImage.save_images_sync
+(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path ``` *Async
+downloader wrapper* ```python import asyncio from gemini import Gemini,
+GeminiImage async def save_generated_imagse(generated_imagse,
+save_path="save_dir", cookies=cookies): await GeminiImage.save
+(generated_imagse, save_path=save_path, cookies=cookies) # Run the async
+function if __name__ == "__main__": cookies = {"key" : "value"}
 generated_imagse = response.generated_imagse asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ```
 `GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
 GeminiImage async def save_generated_imagse(generated_imagse,
 save_path="save_dir", cookies=cookies): image_data_dict = await
 GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies) # Get bytes
 images dict asynchronously await GeminiImage.save_images(image_data_dict,
@@ -223,56 +226,55 @@
 Check response images [Dict] asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ``` > [!NOTE] > Use
 GeminiImage for image processing. `web_images` works without cookies, but for
 images like `generated_image` from Gemini, pass cookies. Cookies are needed to
 download images from Google's storage. Check the response or use existing
 cookies variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
-Gemini. *Async downloader* ```python response = GeminiClient.generate_content
-("Create illustrations of Seoul, South Korea.") response_images =
-response.web_images # Check generated images [Dict] await GeminiImage.save
-(response_images, "save_dir") # image_data_dict = await
-GeminiImage.fetch_images_dict(response_images) # await GeminiImage.save_images
-(image_data_dict, "save_dir") ``` Further *Sync downloader* ```python from
-gemini import Gemini, GeminiImage response = GeminiClient.generate_content
-("Please recommend a travel itinerary for Seoul.") response_images =
-response.web_images # Check response images [Dict] GeminiImage.save_sync
-(response_images, save_path="save_dir") # You can use byte type image dict as
-follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images,
-cookies) # Get bytes images dict # GeminiImage.save_images_sync
-(bytes_images_dict, path="save_dir") # Save to path ``` *Async downloader
-wrapper* ```python import asyncio from gemini import Gemini, GeminiImage async
-def save_response_web_imagse(response_images, save_path="save_dir",
-cookies=cookies): await GeminiImage.save(response_images, save_path=save_path,
-cookies=cookies) # Run the async function if __name__ == "__main__": cookies =
-{"key" : "value"} response_images = response.web_images asyncio.run
-(save_response_web_imagse(response_images, save_path="save_dir",
+Gemini. *Async downloader* ```python response = client.generate_content("Create
+illustrations of Seoul, South Korea.") response_images = response.web_images #
+Check generated images [Dict] await GeminiImage.save(response_images,
+"save_dir") # image_data_dict = await GeminiImage.fetch_images_dict
+(response_images) # await GeminiImage.save_images(image_data_dict, "save_dir")
+``` Further *Sync downloader* ```python from gemini import Gemini, GeminiImage
+response = client.generate_content("Please recommend a travel itinerary for
+Seoul.") response_images = response.web_images # Check response images [Dict]
+GeminiImage.save_sync(response_images, save_path="save_dir") # You can use byte
+type image dict as follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync
+(response_images, cookies) # Get bytes images dict #
+GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
+``` *Async downloader wrapper* ```python import asyncio from gemini import
+Gemini, GeminiImage async def save_response_web_imagse(response_images,
+save_path="save_dir", cookies=cookies): await GeminiImage.save(response_images,
+save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+"__main__": cookies = {"key" : "value"} response_images = response.web_images
+asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
 cookies=cookies)) ``` `GeminiImage.save` method logic ``` import asyncio from
 gemini import Gemini, GeminiImage async def save_response_web_imagse
 (response_images, save_path="save_dir", cookies=cookies): image_data_dict =
 await GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get
 bytes images dict asynchronously await GeminiImage.save_images(image_data_dict,
 save_path=save_path) # Run the async function if __name__ == "__main__":
 response_images = response.web_images # Check response images [Dict]
 asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
 cookies=cookies)) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
 image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. response =
-GeminiClient.generate_content("What does the text in this image say?",
-image=image) response.response_dict ```
+client.generate_content("What does the text in this image say?", image=image)
+response.response_dict ```
 ### # 08. Generate content using Google Services To begin, you must link Google
 Workspace to activate this extension via the [Gemini web extension](https://
 gemini.google.com/extensions). Please refer to the [official notice](https://
 support.google.com/gemini/answer/13695044) and review the [privacy policies]
 (https://support.google.com/gemini/answer/13594961?visit_id=638457301410420313-
 1578971242&p=privacy_help&rd=1) for more details. *extention flags* ``` @Gmail,
 @Google Drive, @Google Docs, @Google Maps, @Google Flights, @Google Hotels,
-@YouTube ``` ```python response = GeminiClient.generate_content("@YouTube
-Search clips related with Google Gemini") response.response_dict ``` Extension
+@YouTube ``` ```python response = client.generate_content("@YouTube Search
+clips related with Google Gemini") response.response_dict ``` Extension
 description - Google Workspace - Services: **@Gmail, @Google Drive, @Google
 Docs** - Description: Summarize, search, and find desired information quickly
 in your content for efficient personal task management. - Features: Information
 retrieval, document summarization, information categorization - Google Maps -
 Service: **@Google Maps** - Description: Execute plans using location-based
 information. Note: Google Maps features may be limited in some regions. -
 Features: Route guidance, nearby search, navigation - Google Flights - Service:
@@ -283,62 +285,61 @@
 conversation with a friend. - Features: Packing for travel, sightseeing,
 special relaxation - YouTube - Service: **@YouTube** - Description: Explore
 YouTube videos and ask questions about what interests you. - Features: Problem-
 solving, generating ideas, search, exploring topics
 ### # 09. Fix context setting RCID You can specify a particular response by
 setting its Response Candidate ID(RCID). ```python # Generate content for the
 prompt "Give me some information about the USA." response1 =
-GeminiClient.generate_content("Give me some information about the USA.") #
-After reviewing the responses, choose the one you prefer and copy its RCID.
-GeminiClient.rcid = "rc_xxxx" # Now, generate content for the next prompt "How
-long does it take from LA to New York?" response2 =
-GeminiClient.generate_content("How long does it take from LA to New York?") #
-However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to
-None. # GeminiClient.rcid = None ```
+client.generate_content("Give me some information about the USA.") # After
+reviewing the responses, choose the one you prefer and copy its RCID.
+client.rcid = "rc_xxxx" # Now, generate content for the next prompt "How long
+does it take from LA to New York?" response2 = client.generate_content("How
+long does it take from LA to New York?") # However, RCID may not persist. If
+parsing fails, reset `client.rcid` to None. # client.rcid = None ```
 ### # 10. Changing the Selected Response from 0 to *n* In Gemini,
 generate_content returns the first response. This may vary depending on length
 or sorting. Therefore, you can specify the index of the chosen response from 0
 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python from gemini import GeminiModelOutput GeminiModelOutput.chosen = 1 #
-default is 0 response_choice_1 = GeminiClient.generate_content("Give me some
+default is 0 response_choice_1 = client.generate_content("Give me some
 information about the USA.") # If not all Gemini returns are necessarily
 plural, revert back to 0 in case of errors. # GeminiModelOutput.chosen = 0 ```
 ### # 11. Generate custom content Parse the response text to extract desired
 values. Using `Gemini.generate_custom_content`, specify custom parsing to
 extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and
 you can pass custom parsing methods as arguments if desired. Refer to
 [custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/
 src/model/parser/custom_parser.py). ```python # You can create a parser method
 that takes response_text as the input for custom_parser. response_text,
-response_status = GeminiClient.send_request("Give me some information about the
+response_status = client.send_request("Give me some information about the
 USA.") # Use custom_parser function or class inheriting from BaseParser
-response = GeminiClient.generate_custom_content("Give me some information about
-the USA.", *custom_parser) ``` https://github.com/dsdanielpark/Gemini-API/blob/
+response = client.generate_custom_content("Give me some information about the
+USA.", *custom_parser) ``` https://github.com/dsdanielpark/Gemini-API/blob/
 31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 ## Further ### Use rotating proxies via [Smart Proxy by Crawlbase](https://
 crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api) If you want to
 **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https:
 //crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards
 your connection requests to a **randomly rotating IP address** in a pool of
 proxies before reaching the target website. The combination of AI and ML make
 it more effective to avoid CAPTCHAs and blocks. ```python # Get your proxy url
 at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://
 xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
-proxy_url} GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
-GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of
-Seoul's scenery.") ``` ### Reusable session object For standard cases, use
-Gemini class; for exceptions, use session objects. When creating a new bot
-Gemini server, adjust Headers.MAIN. ```python import requests from gemini
-import Gemini, Headers cookies = {} session = requests.Session()
-session.headers = Headers.MAIN for key, value in cookies.items():
-session.cookies.update({key: value}) GeminiClient = Gemini(session=session) #
-You can use various args response = GeminiClient.generate_content("Hello,
-Gemini. What's the weather like in Seoul today?") ```
+proxy_url} client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's
+scenery.") ``` ### Reusable session object For standard cases, use Gemini
+class; for exceptions, use session objects. When creating a new bot Gemini
+server, adjust Headers.MAIN. ```python import requests from gemini import
+Gemini, Headers cookies = {} session = requests.Session() session.headers =
+Headers.MAIN for key, value in cookies.items(): session.cookies.update({key:
+value}) client = Gemini(session=session) # You can use various args response =
+client.generate_content("Hello, Gemini. What's the weather like in Seoul
+today?") ```
 ## [More features](https://github.com/dsdanielpark/Gemini-API/blob/main/
 documents/README_DEV.md) Explore additional features in [this document](https:/
 /github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md). If you
 want to develop your own simple code, you can start from [this simple code
 example](https://github.com/dsdanielpark/Gemini-API/blob/main/script/
 sample.ipynb).
 ## Google Open-source LLMs If you have sufficient GPU resources, you can
@@ -376,20 +377,20 @@
 models with a 0-dollar token cost primarily; other models may incur charges.
 See more at [free open-source LLM API guide](https://github.com/dsdanielpark/
 Gemini-API/blob/main/documents/README_OPENROUTER.md). **Sync client is favored
 over async for Gemini due to rate limiting and blocking issues**, but
 OpenRouter offers reliable open-source LLMs for [async implementation](https://
 github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_OPENROUTER.md#openrouter-async-api-client). ```python from gemini import
-OpenRouter OPENROUTER_API_KEY = "" GemmaClient = OpenRouter
+OpenRouter OPENROUTER_API_KEY = "" gemma_client = OpenRouter
 (api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free") prompt = "Do you
 know UCA academy in Korea? https://blog.naver.com/ulsancoding" response =
-GemmaClient.create_chat_completion(prompt) print(response) # payload =
-GemmaClient.generate_content(prompt) # print(payload.json()) ``` The free model
-list includes: - `google/gemma-7b-it:free` - [google/gemma-7b](https://
+gemma_client.create_chat_completion(prompt) print(response) # payload =
+gemma_client.generate_content(prompt) # print(payload.json()) ``` The free
+model list includes: - `google/gemma-7b-it:free` - [google/gemma-7b](https://
 huggingface.co/google/gemma-7b) from Google *** - `mistralai/mistral-7b-
 instruct:free` - [mistralai/Mistral-7B-Instruct-v0.1](https://huggingface.co/
 mistralai/Mistral-7B-Instruct-v0.1) for instruction from Mistral AI **** -
 `huggingfaceh4/zephyr-7b-beta:free` - [HuggingFaceH4/zephyr-7b-beta](https://
 huggingface.co/HuggingFaceH4/zephyr-7b-beta) *** - `openchat/openchat-7b:free`
 - [openchat/openchat](https://huggingface.co/openchat/openchat) for chat ** -
 `openrouter/cinematika-7b:free` - [jondurbin/cinematika-7b-v0.1](https://
@@ -438,38 +439,29 @@
 Cheong](https://github.com/acheong08) / teapotv8@proton.me
 - [Daniel Park](https://github.com/DSDanielPark) / parkminwoo1991@gmail.com ##
 License Â©ï¸ [MIT](https://opensource.org/license/mit/) license, 2024. We
 hereby strongly disclaim any explicit or implicit legal liability related to
 our works. Users are required to use this package responsibly and at their own
 risk. This project is a personal initiative and is not affiliated with or
 endorsed by Google. It is recommended to use Google's official API. ##
-References [1]: Paper - [Introducing GEMINI: Multimodal Generative Models]
-(https://arxiv.org/abs/2312.11805)
-[2]: Website - [Google DeepMind :: GEMINI Introduction](https://
-deepmind.google/technologies/gemini/#introduction)
-[3]: Paper - [GEMMA: A Unified Language Model for Text Generation,
-Understanding, Translation, Coding, and Math.]()
-[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/
-gemma/docs)
-[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming
-Assignments](https://storage.googleapis.com/deepmind-media/gemma/
-codegemma_report.pdf?utm_source=substack&utm_medium=email)
-[6]: Blog Post - [Announcing CodeGen: Building Better Developersâ Tools Using
-LLMs](https://huggingface.co/blog/codegen)
-[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/
-collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf)
-[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard)
-[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-
-API)
-[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-
-API)
-[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/
-GoogleCloudPlatform/generative-ai)
-[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-
-runner)
-[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-
-studio_quickstart)
+References 1. [Introducing GEMINI: Multimodal Generative Models](https://
+arxiv.org/abs/2312.11805) 2. [Google DeepMind: GEMINI Introduction](https://
+deepmind.google/technologies/gemini/#introduction) 3. [GEMMA: A Unified
+Language Model for Text Generation, Understanding, Translation, Coding, and
+Math](https://arxiv.org/abs/2403.08295) 4. [AI at Google: GEMS Documentation]
+(https://ai.google.dev/gemma/docs) 5. [CodeGMMA: Large Language Models Can
+Write Realistic Programming Assignments](https://storage.googleapis.com/
+deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email)
+6. [Announcing CodeGen: Building Better Developers' Tools Using LLMs](https://
+huggingface.co/blog/codegen) 7. [Google: CodeGen Release](https://
+huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf) 8.
+[acheong08/Bard](https://github.com/acheong08/Bard) 9. [dsdanielpark/Bard-API]
+(https://github.com/dsdanielpark/Bard-API) 10. [HanaokaYuzu/Gemini-API](https:/
+/github.com/HanaokaYuzu/Gemini-API) 11. [GoogleCloudPlatform/generative-ai]
+(https://github.com/GoogleCloudPlatform/generative-ai) 12. [OpenRouter](https:/
+/github.com/OpenRouterTeam/openrouter-runner) 13. [Google AI Studio](https://
+ai.google.dev/tutorials/ai-studio_quickstart)
 > *Warning* Users assume full legal responsibility for GeminiAPI. Not endorsed
 by Google. Excessive use may lead to account restrictions. Changes in policies
 or account status may affect functionality. Utilize issue and discussion pages.
 
 ## Requirements Python 3.7 or higher.
```

### Comparing `python_gemini_api-2.4.6/README.md` & `python_gemini_api-2.4.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,17 @@
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-ba79-d9f89b637324
 
 
 
 
 
 
-A *unofficial* Python wrapper, [python-gemini-api](https://pypi.org/project/python-gemini-api/), operates through reverse-engineering, utilizing cookie values to interact with [Google Gemini](https://gemini.google.com) for users struggling with frequent authentication problems or unable to authenticate via [Google Authentication](https://developers.google.com/identity/protocols/oauth2?hl=en).
-
-Collaborated competently with [Antonio Cheong](https://github.com/acheong08).
+An **unofficial* Python wrapper, [python-gemini-api](https://pypi.org/project/python-gemini-api/), is available for users facing frequent authentication issues or unable to use [Google Authentication](https://developers.google.com/identity/protocols/oauth2?hl=en). This wrapper uses cookie values to interact with [Google Gemini](https://gemini.google.com) through reverse-engineering. The project involved a collaboration with [Antonio Cheong](https://github.com/acheong08).
 
+On the official side, Google provides partially free, clean [official Gemini APIs and SDKs](https://aistudio.google.com/), which can be accessed and utilized neatly via Python packages, [google-generativeai](https://pypi.org/project/google-generativeai/). 
 <br>
 
 <br>
 
 
 > [!TIP]
 > | 2024-03-26 | [[See Code Examples]](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md)
@@ -105,21 +104,22 @@
 
 ## Authentication
 
 1. Visit https://gemini.google.com/ <br>
     With browser open, try auto-collecting cookies first.
     ```python
     from gemini import Gemini
-    GeminiClient = Gemini(auto_cookies=True)
+    
+    client = Gemini(auto_cookies=True)
 
     # Testing needed as cookies vary by region.
-    # GeminiClient = Gemini(auto_cookies=True, target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"])
-    # GeminiClient = Gemini(auto_cookies=True, target_cookies="all") # You can pass whole cookies
+    # client = Gemini(auto_cookies=True, target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"])
+    # client = Gemini(auto_cookies=True, target_cookies="all") # You can pass whole cookies
 
-    response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
+    response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
     print(response.payload)
     ```
 2. *(Manually)* `F12` for browser console → `Session: Application` → `Cookies` → Copy the value of some working cookie sets. If it doesn't work, go to step 3.
     <details><summary>Some working cookie sets</summary>
     Cookies may vary by account or region. 
       
     First try `__Secure-1PSIDCC` alone. If it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success? Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the entire cookie file.
@@ -146,29 +146,29 @@
 
 ## Quick Start
 
 **Generate content:** returns parsed response.
 ```python
 from gemini import Gemini
 
-cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
-GeminiClient = Gemini(cookies=cookies) # You can use various args
+cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+client = Gemini(cookies=cookies) # You can use various args
 
-response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
+response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 response.payload
 ```
 
 **Generate content from image:** you can use image as input.
 ```python
 from gemini import Gemini
 
-cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
+cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+client = Gemini(cookies=cookies) # You can use various args
 
-GeminiClient = Gemini(cookies=cookies) # You can use various args
-response = GeminiClient.generate_content("What does the text in this image say?", image='folder/image.jpg')
+response = client.generate_content("What does the text in this image say?", image='folder/image.jpg')
 response.payload
 ```
 
 > [!NOTE] 
 > If the generate_content method returns an empty payload, try executing it again without reinitializing the Gemini object.
 
 <br><br>
@@ -177,14 +177,15 @@
 
 *Setting language and Gemini version using environment variables:*
 
 Setting Gemini response language (Optional): Check supported languages [here](https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes). Default is English.
 
 ```python
 import os
+
 os.environ["GEMINI_LANGUAGE"] = "KR"  # Setting Gemini response language (Optional)
 os.environ["GEMINI_ULTRA"] = "1"      # Switch to Gemini-advanced response (Experimental, Optional)
 # In some accounts, access to Gemini Ultra may not be available. If that's the case, please revert it back to "0".
 ```
 
 
 
@@ -203,17 +204,17 @@
     "__Secure-1PSIDCC" : "value",
     "__Secure-1PSID" : "value",
     "__Secure-1PSIDTS" : "value",
     "NID" : "value",
     # Cookies may vary by account or region. Consider sending the entire cookie file.
   }
 
-GeminiClient = Gemini(cookies=cookies)
-# GeminiClient = Gemini(cookie_fp="folder/cookie_file.json") # (*.json, *.txt) are supported.
-# GeminiClient = Gemini(auto_cookies=True) # Or use auto_cookies paprameter
+client = Gemini(cookies=cookies)
+# client = Gemini(cookie_fp="folder/cookie_file.json") # (*.json, *.txt) are supported.
+# client = Gemini(auto_cookies=True) # Or use auto_cookies paprameter
 ```
 
 ##### Auto Cookie Update
 For `auto_cookie` to be set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3) enables automatic cookie collection, though updates may not be complete yet.
 
 
 
@@ -221,15 +222,15 @@
 
 ### # 02. Generate content
 Returns Gemini's response, but the first one might be empty. 
 
 
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
-response = GeminiClient.generate_content(prompt)
+response = client.generate_content(prompt)
 print(response.payload)
 ```
 
 
 > [!IMPORTANT]
 >  DO NOT send same prompt repeatly. **If the session connects successfully and `generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open in the browser, cookies may expire faster. 
 
@@ -252,41 +253,41 @@
 
 ### # 03. Send request
 Send request: returns the request's payload and status_code, making debugging easier.
 ```python
 from gemini import Gemini
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
-GeminiClient = Gemini(cookies=cookies) # You can use various args
+client = Gemini(cookies=cookies) # You can use various args
 
-response_text, response_status = GeminiClient.send_request("Hello, Gemini. What's the weather like in Seoul today?")
+response_text, response_status = client.send_request("Hello, Gemini. What's the weather like in Seoul today?")
 print(response_text)
 ```
 You can track the total number of requests made by accessing the `request_count` property within the `Gemini` class.
 
 <br>
 
 ### # 04. Text generation
 Returns text generated by Gemini.
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
-response = GeminiClient.generate_content(prompt)
+response = client.generate_content(prompt)
 print(response.text)
 ```
 
 
 <br>
 
 ### # 05. Image generation
 Returns images generated by Gemini.
 
 *Async downloader*
 
 ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 generated_images = response.generated_images # Check generated images [Dict]
 
 await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
 # image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
 # await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
@@ -309,15 +310,15 @@
   ```
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+response = client.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
 GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
 
 # You can use byte type image dict for printing images as follow:
 # bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
 # GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
@@ -365,15 +366,15 @@
 
 ### # 06. Retrieving Images from Gemini Responses
 Returns images in response of Gemini.
 
 
 *Async downloader*
 ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 response_images = response.web_images # Check generated images [Dict]
 
 await GeminiImage.save(response_images, "save_dir")
 # image_data_dict = await GeminiImage.fetch_images_dict(response_images)
 # await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
@@ -381,15 +382,15 @@
 <details><summary>Further</summary>
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
-response = GeminiClient.generate_content("Please recommend a travel itinerary for Seoul.")
+response = client.generate_content("Please recommend a travel itinerary for Seoul.")
 response_images = response.web_images # Check response images [Dict]
 
 GeminiImage.save_sync(response_images, save_path="save_dir")
 
 # You can use byte type image dict as follow:
 # bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
 # GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
@@ -433,29 +434,29 @@
 ### # 07. Generate content from images
 Takes an image as input and returns a response.
 
 ```python
 image = 'folder/image.jpg'
 # image = open('folder/image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported.
 
-response = GeminiClient.generate_content("What does the text in this image say?", image=image)
+response = client.generate_content("What does the text in this image say?", image=image)
 response.response_dict
 ```
 
 <br>
 
 ### # 08. Generate content using Google Services
 To begin, you must link Google Workspace to activate this extension via the [Gemini web extension](https://gemini.google.com/extensions). Please refer to the [official notice](https://support.google.com/gemini/answer/13695044) and review the [privacy policies](https://support.google.com/gemini/answer/13594961?visit_id=638457301410420313-1578971242&p=privacy_help&rd=1) for more details.
 
 *extention flags*
 ```
 @Gmail, @Google Drive, @Google Docs, @Google Maps, @Google Flights, @Google Hotels, @YouTube
 ```
 ```python
-response = GeminiClient.generate_content("@YouTube Search clips related with Google Gemini")
+response = client.generate_content("@YouTube Search clips related with Google Gemini")
 response.response_dict
 ```
 <details><summary>Extension description</summary>
   
 - Google Workspace
   - Services: **@Gmail, @Google Drive, @Google Docs** 
   - Description: Summarize, search, and find desired information quickly in your content for efficient personal task management.
@@ -486,36 +487,36 @@
 
 
 ### # 09. Fix context setting RCID
 You can specify a particular response by setting its Response Candidate ID(RCID).
 
 ```python
 # Generate content for the prompt "Give me some information about the USA."
-response1 = GeminiClient.generate_content("Give me some information about the USA.")
+response1 = client.generate_content("Give me some information about the USA.")
 # After reviewing the responses, choose the one you prefer and copy its RCID.
-GeminiClient.rcid = "rc_xxxx"
+client.rcid = "rc_xxxx"
 
 # Now, generate content for the next prompt "How long does it take from LA to New York?"
-response2 = GeminiClient.generate_content("How long does it take from LA to New York?")
+response2 = client.generate_content("How long does it take from LA to New York?")
 
-# However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to None.
-# GeminiClient.rcid = None
+# However, RCID may not persist. If parsing fails, reset `client.rcid` to None.
+# client.rcid = None
 ```
 
 
 
 <br>
 
 ### # 10. Changing the Selected Response from 0 to *n*
 In Gemini, generate_content returns the first response. This may vary depending on length or sorting. Therefore, you can specify the index of the chosen response from 0 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python
 from gemini import GeminiModelOutput
 
 GeminiModelOutput.chosen = 1 # default is 0
-response_choice_1 = GeminiClient.generate_content("Give me some information about the USA.")
+response_choice_1 = client.generate_content("Give me some information about the USA.")
 
 # If not all Gemini returns are necessarily plural, revert back to 0 in case of errors.
 #  GeminiModelOutput.chosen = 0
 ```
 
 <br>
 
@@ -523,18 +524,18 @@
 Parse the response text to extract desired values.
 
 
 Using `Gemini.generate_custom_content`, specify custom parsing to extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and you can pass custom parsing methods as arguments if desired. Refer to [custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/src/model/parser/custom_parser.py).
 
 ```python
 # You can create a parser method that takes response_text as the input for custom_parser.
-response_text, response_status = GeminiClient.send_request("Give me some information about the USA.")
+response_text, response_status = client.send_request("Give me some information about the USA.")
 
 # Use custom_parser function or class inheriting from BaseParser
-response = GeminiClient.generate_custom_content("Give me some information about the USA.", *custom_parser)
+response = client.generate_custom_content("Give me some information about the USA.", *custom_parser)
 ```
 
 https://github.com/dsdanielpark/Gemini-API/blob/31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 <br>
 
 ## Further
 
@@ -543,16 +544,16 @@
 If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks.
 
 ```python
 # Get your proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/
 proxy_url = "http://xxxxx:@smartproxy.crawlbase.com:8012" 
 proxies = {"http": proxy_url, "https": proxy_url}
 
-GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
-GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
+client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
 ```
 
 ### Reusable session object
 For standard cases, use Gemini class; for exceptions, use session objects. When creating a new bot Gemini server, adjust Headers.MAIN.
 ```python
 import requests
 from gemini import Gemini, Headers
@@ -560,16 +561,16 @@
 cookies = {} 
 
 session = requests.Session()
 session.headers = Headers.MAIN
 for key, value in cookies.items():
     session.cookies.update({key: value})
 
-GeminiClient = Gemini(session=session) # You can use various args
-response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
+client = Gemini(session=session) # You can use various args
+response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 ```
 
 
 
 
 <br>
 
@@ -633,21 +634,21 @@
 
 **Sync client is favored over async for Gemini due to rate limiting and blocking issues**, but OpenRouter offers reliable open-source LLMs for [async implementation](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md#openrouter-async-api-client).
 
 ```python
 from gemini import OpenRouter
 
 OPENROUTER_API_KEY = "<your_open_router_api_key>"
-GemmaClient = OpenRouter(api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free")
+gemma_client = OpenRouter(api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free")
 
 prompt = "Do you know UCA academy in Korea? https://blog.naver.com/ulsancoding"
-response = GemmaClient.create_chat_completion(prompt)
+response = gemma_client.create_chat_completion(prompt)
 print(response)
 
-# payload = GemmaClient.generate_content(prompt)
+# payload = gemma_client.generate_content(prompt)
 # print(payload.json())
 ```
 
 The free model list includes:
    - `google/gemma-7b-it:free` - [google/gemma-7b](https://huggingface.co/google/gemma-7b) from Google ***
    - `mistralai/mistral-7b-instruct:free` - [mistralai/Mistral-7B-Instruct-v0.1](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.1) for instruction from Mistral AI ****
    - `huggingfaceh4/zephyr-7b-beta:free` - [HuggingFaceH4/zephyr-7b-beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta) ***
@@ -710,27 +711,29 @@
 
 
 ## License ©️ 
 [MIT](https://opensource.org/license/mit/) license, 2024. We hereby strongly disclaim any explicit or implicit legal liability related to our works. Users are required to use this package responsibly and at their own risk. This project is a personal initiative and is not affiliated with or endorsed by Google. It is recommended to use Google's official API.
 
 
 ## References
-[1]: Paper - [Introducing GEMINI: Multimodal Generative Models](https://arxiv.org/abs/2312.11805) <br>
-[2]: Website - [Google DeepMind :: GEMINI Introduction](https://deepmind.google/technologies/gemini/#introduction) <br>
-[3]: Paper - [GEMMA: A Unified Language Model for Text Generation, Understanding, Translation, Coding, and Math.]() <br>
-[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/gemma/docs) <br>
-[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming Assignments](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email) <br>
-[6]: Blog Post - [Announcing CodeGen: Building Better Developers’ Tools Using LLMs](https://huggingface.co/blog/codegen) <br>
-[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf) <br>
-[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard) <br>
-[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) <br>
-[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API) <br>
-[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai) <br>
-[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner) <br>
-[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart) <br>
+1. [Introducing GEMINI: Multimodal Generative Models](https://arxiv.org/abs/2312.11805)
+2. [Google DeepMind: GEMINI Introduction](https://deepmind.google/technologies/gemini/#introduction)
+3. [GEMMA: A Unified Language Model for Text Generation, Understanding, Translation, Coding, and Math](https://arxiv.org/abs/2403.08295)
+4. [AI at Google: GEMS Documentation](https://ai.google.dev/gemma/docs)
+5. [CodeGMMA: Large Language Models Can Write Realistic Programming Assignments](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email)
+6. [Announcing CodeGen: Building Better Developers' Tools Using LLMs](https://huggingface.co/blog/codegen)
+7. [Google: CodeGen Release](https://huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf)
+8. [acheong08/Bard](https://github.com/acheong08/Bard)
+9. [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API)
+10. [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API)
+11. [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai)
+12. [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner)
+13. [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart)
+
+<br>
 
 
 > *Warning*
 Users assume full legal responsibility for GeminiAPI. Not endorsed by Google. Excessive use may lead to account restrictions. Changes in policies or account status may affect functionality. Utilize issue and discussion pages.
 
 <br>
```

#### html2text {}

```diff
@@ -1,20 +1,24 @@
 # [Gemini Icon]Gemini API_[_P_y_P_I_]
   _[_p_i_p_ _d_o_w_n_l_o_a_d_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
                 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_d_s_d_a_n_i_e_l_p_a_r_k_%_2_F_G_e_m_i_n_i_-
 _A_P_I_&_c_o_u_n_t___b_g_=_%_2_3_0_0_0_0_0_0_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_v_i_e_w_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]
                                                                     _[_D_o_w_n_l_o_a_d_s_]
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-
-ba79-d9f89b637324 A *unofficial* Python wrapper, [python-gemini-api](https://
-pypi.org/project/python-gemini-api/), operates through reverse-engineering,
-utilizing cookie values to interact with [Google Gemini](https://
-gemini.google.com) for users struggling with frequent authentication problems
-or unable to authenticate via [Google Authentication](https://
-developers.google.com/identity/protocols/oauth2?hl=en). Collaborated
-competently with [Antonio Cheong](https://github.com/acheong08).
+ba79-d9f89b637324 An **unofficial* Python wrapper, [python-gemini-api](https://
+pypi.org/project/python-gemini-api/), is available for users facing frequent
+authentication issues or unable to use [Google Authentication](https://
+developers.google.com/identity/protocols/oauth2?hl=en). This wrapper uses
+cookie values to interact with [Google Gemini](https://gemini.google.com)
+through reverse-engineering. The project involved a collaboration with [Antonio
+Cheong](https://github.com/acheong08). On the official side, Google provides
+partially free, clean [official Gemini APIs and SDKs](https://
+aistudio.google.com/), which can be accessed and utilized neatly via Python
+packages, [google-generativeai](https://pypi.org/project/google-generativeai/).
+
 
 > [!TIP] > | 2024-03-26 | [[See Code Examples]](https://github.com/
 dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md) > > Check out
 temporarily free Open-source LLM APIs with Open Router. (Free limit: 10
 requests/minute)
 ## Contents - [ Gemini API ](#-gemini-api---) - [What is Gemini? ð](#what-
 is-gemini) - [Installation â](#installation-) - [Authentication â]
@@ -71,24 +75,24 @@
 in REST format. **Synchronous clients are preferred over asynchronous ones for
 Gemini because of rate limiting and blocking concerns.** ## Installation ð¦
 ``` pip install python-gemini-api ``` ``` pip install git+https://github.com/
 dsdanielpark/Gemini-API.git ``` For the updated version, use as follows: ```
 pip install -q -U python-gemini-api ``` ## Authentication 1. Visit https://
 gemini.google.com/
 With browser open, try auto-collecting cookies first. ```python from gemini
-import Gemini GeminiClient = Gemini(auto_cookies=True) # Testing needed as
-cookies vary by region. # GeminiClient = Gemini(auto_cookies=True,
-target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"]) # GeminiClient = Gemini
-(auto_cookies=True, target_cookies="all") # You can pass whole cookies response
-= GeminiClient.generate_content("Hello, Gemini. What's the weather like in
-Seoul today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser
-console â `Session: Application` â `Cookies` â Copy the value of some
-working cookie sets. If it doesn't work, go to step 3. Some working cookie sets
-Cookies may vary by account or region. First try `__Secure-1PSIDCC` alone. If
-it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
+import Gemini client = Gemini(auto_cookies=True) # Testing needed as cookies
+vary by region. # client = Gemini(auto_cookies=True, target_cookies=["__Secure-
+1PSID", "__Secure-1PSIDTS"]) # client = Gemini(auto_cookies=True,
+target_cookies="all") # You can pass whole cookies response =
+client.generate_content("Hello, Gemini. What's the weather like in Seoul
+today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser console
+â `Session: Application` â `Cookies` â Copy the value of some working
+cookie sets. If it doesn't work, go to step 3. Some working cookie sets Cookies
+may vary by account or region. First try `__Secure-1PSIDCC` alone. If it
+doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
 Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-
 1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the
 entire cookie file. 3. *(Recommended)* Export Gemini site cookies via a browser
 extension. For instance, use Chrome extension [ExportThisCookies](https://
 chromewebstore.google.com/detail/exportthiscookie/
 dannllckdimllhkiplchkcaoheibealk), open, and copy the txt file contents.
 Further: For manual collection or Required for a few users upon error 4. For
@@ -105,25 +109,26 @@
 assistant.lamda.BardFrontendService/StreamGenerate" â Payload â Form Data
 â Copy the "at" key value. See [this image](assets/nonce_value.pdf) for
 reference. > [!IMPORTANT] > Experiment with different Google accounts and
 browser settings to find a working cookie. Success may vary by IP and account
 status. Once connected, a cookie typically remains effective over a month. Keep
 testing until successful.
 ## Quick Start **Generate content:** returns parsed response. ```python from
-gemini import Gemini cookies = {} # Cookies may vary by account or region.
-Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
-# You can use various args response = GeminiClient.generate_content("Hello,
-Gemini. What's the weather like in Seoul today?") response.payload ```
+gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
+or region. Consider sending the entire cookie file. client = Gemini
+(cookies=cookies) # You can use various args response = client.generate_content
+("Hello, Gemini. What's the weather like in Seoul today?") response.payload ```
 **Generate content from image:** you can use image as input. ```python from
-gemini import Gemini cookies = {} # Cookies may vary by account or region.
-Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
-# You can use various args response = GeminiClient.generate_content("What does
-the text in this image say?", image='folder/image.jpg') response.payload ``` >
-[!NOTE] > If the generate_content method returns an empty payload, try
-executing it again without reinitializing the Gemini object.
+gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
+or region. Consider sending the entire cookie file. client = Gemini
+(cookies=cookies) # You can use various args response = client.generate_content
+("What does the text in this image say?", image='folder/image.jpg')
+response.payload ``` > [!NOTE] > If the generate_content method returns an
+empty payload, try executing it again without reinitializing the Gemini object.
+
 
 ## Usage *Setting language and Gemini version using environment variables:
 * Setting Gemini response language (Optional): Check supported languages [here]
 (https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes).
 Default is English. ```python import os os.environ["GEMINI_LANGUAGE"] = "KR" #
 Setting Gemini response language (Optional) os.environ["GEMINI_ULTRA"] = "1" #
 Switch to Gemini-advanced response (Experimental, Optional) # In some accounts,
@@ -131,73 +136,71 @@
 it back to "0". ```
 ### # 01. Initialization Please explicitly declare `cookies` in dict format.
 You can also enter the path to the file containing the cookie with `cookie_fp`
 (*.json, *.txt supported). Check sample cookie files in [assets](https://
 github.com/dsdanielpark/Gemini-API/tree/main/assets) folder. ```python from
 gemini import Gemini cookies = { "__Secure-1PSIDCC" : "value", "__Secure-1PSID"
 : "value", "__Secure-1PSIDTS" : "value", "NID" : "value", # Cookies may vary by
-account or region. Consider sending the entire cookie file. } GeminiClient =
-Gemini(cookies=cookies) # GeminiClient = Gemini(cookie_fp="folder/
-cookie_file.json") # (*.json, *.txt) are supported. # GeminiClient = Gemini
-(auto_cookies=True) # Or use auto_cookies paprameter ``` ##### Auto Cookie
-Update For `auto_cookie` to be set to `True`, and adjust `target_cookies`.
-Gemini WebUI must be active in the browser. The [browser_cookie3](https://
-github.com/borisbabic/browser_cookie3) enables automatic cookie collection,
-though updates may not be complete yet.
+account or region. Consider sending the entire cookie file. } client = Gemini
+(cookies=cookies) # client = Gemini(cookie_fp="folder/cookie_file.json") #
+(*.json, *.txt) are supported. # client = Gemini(auto_cookies=True) # Or use
+auto_cookies paprameter ``` ##### Auto Cookie Update For `auto_cookie` to be
+set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the
+browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3)
+enables automatic cookie collection, though updates may not be complete yet.
 ### # 02. Generate content Returns Gemini's response, but the first one might
 be empty. ```python prompt = "Hello, Gemini. What's the weather like in Seoul
-today?" response = GeminiClient.generate_content(prompt) print
-(response.payload) ``` > [!IMPORTANT] > DO NOT send same prompt repeatly. **If
-the session connects successfully and `generate_content` runs well, CLOSE
-Gemini website.** If Gemini web stays open in the browser, cookies may expire
-faster.
+today?" response = client.generate_content(prompt) print(response.payload) ```
+> [!IMPORTANT] > DO NOT send same prompt repeatly. **If the session connects
+successfully and `generate_content` runs well, CLOSE Gemini website.** If
+Gemini web stays open in the browser, cookies may expire faster.
 The output of the generate_content function is `GeminiModelOutput`, with the
 following structure: - *rcid*: returns the response candidate id of the chosen
 candidate. - *text*: returns the text of the chosen candidate. - *code*:
 returns the codes of the chosen candidate. - *web_images*: returns a list of
 web images from the chosen candidate. - *generated_images*: returns a list of
 generated images from the chosen candidate. - *payload*: returns the response
 dictionary, if available. https://github.com/dsdanielpark/Gemini-API/blob/
 fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 ### # 03. Send request Send request: returns the request's payload and
 status_code, making debugging easier. ```python from gemini import Gemini
 cookies = {} # Cookies may vary by account or region. Consider sending the
-entire cookie file. GeminiClient = Gemini(cookies=cookies) # You can use
-various args response_text, response_status = GeminiClient.send_request("Hello,
-Gemini. What's the weather like in Seoul today?") print(response_text) ``` You
-can track the total number of requests made by accessing the `request_count`
-property within the `Gemini` class.
+entire cookie file. client = Gemini(cookies=cookies) # You can use various args
+response_text, response_status = client.send_request("Hello, Gemini. What's the
+weather like in Seoul today?") print(response_text) ``` You can track the total
+number of requests made by accessing the `request_count` property within the
+`Gemini` class.
 ### # 04. Text generation Returns text generated by Gemini. ```python prompt =
 "Hello, Gemini. What's the weather like in Seoul today?" response =
-GeminiClient.generate_content(prompt) print(response.text) ```
+client.generate_content(prompt) print(response.text) ```
 ### # 05. Image generation Returns images generated by Gemini. *Async
-downloader* ```python response = GeminiClient.generate_content("Create
-illustrations of Seoul, South Korea.") generated_images =
-response.generated_images # Check generated images [Dict] await
-GeminiImage.save(generated_images, "save_dir", cookies=cookies) #
-image_data_dict = await GeminiImage.fetch_images_dict(generated_images,
-cookies=cookies) # await GeminiImage.save_images(image_data_dict, "save_dir")
-``` Further *Display images in IPython* You can display the image or transmit
-it to another application in byte format. ```python bytes_images_dict =
-GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes
-images dict from IPython.display import display, Image import io for
-image_name, image_bytes in bytes_images_dict.items(): print(image_name) image =
-Image(data=image_bytes) display(image) ``` *Sync downloader* ```python from
-gemini import Gemini, GeminiImage response = GeminiClient.generate_content
-("Create illustrations of Seoul, South Korea.") generated_images =
-response.generated_images # Check generated images [Dict] GeminiImage.save_sync
-(generated_images, save_path="save_dir", cookies=cookies) # You can use byte
-type image dict for printing images as follow: # bytes_images_dict =
-GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
-bytes images dict # GeminiImage.save_images_sync(bytes_images_dict,
-path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
-```python import asyncio from gemini import Gemini, GeminiImage async def
-save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
-# Run the async function if __name__ == "__main__": cookies = {"key" : "value"}
+downloader* ```python response = client.generate_content("Create illustrations
+of Seoul, South Korea.") generated_images = response.generated_images # Check
+generated images [Dict] await GeminiImage.save(generated_images, "save_dir",
+cookies=cookies) # image_data_dict = await GeminiImage.fetch_images_dict
+(generated_images, cookies=cookies) # await GeminiImage.save_images
+(image_data_dict, "save_dir") ``` Further *Display images in IPython* You can
+display the image or transmit it to another application in byte format.
+```python bytes_images_dict = GeminiImage.fetch_images_dict_sync
+(generated_images, cookies) # Get bytes images dict from IPython.display import
+display, Image import io for image_name, image_bytes in bytes_images_dict.items
+(): print(image_name) image = Image(data=image_bytes) display(image) ``` *Sync
+downloader* ```python from gemini import Gemini, GeminiImage response =
+client.generate_content("Create illustrations of Seoul, South Korea.")
+generated_images = response.generated_images # Check generated images [Dict]
+GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+# You can use byte type image dict for printing images as follow: #
+bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images,
+cookies=cookies) # Get bytes images dict # GeminiImage.save_images_sync
+(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path ``` *Async
+downloader wrapper* ```python import asyncio from gemini import Gemini,
+GeminiImage async def save_generated_imagse(generated_imagse,
+save_path="save_dir", cookies=cookies): await GeminiImage.save
+(generated_imagse, save_path=save_path, cookies=cookies) # Run the async
+function if __name__ == "__main__": cookies = {"key" : "value"}
 generated_imagse = response.generated_imagse asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ```
 `GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
 GeminiImage async def save_generated_imagse(generated_imagse,
 save_path="save_dir", cookies=cookies): image_data_dict = await
 GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies) # Get bytes
 images dict asynchronously await GeminiImage.save_images(image_data_dict,
@@ -206,56 +209,55 @@
 Check response images [Dict] asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ``` > [!NOTE] > Use
 GeminiImage for image processing. `web_images` works without cookies, but for
 images like `generated_image` from Gemini, pass cookies. Cookies are needed to
 download images from Google's storage. Check the response or use existing
 cookies variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
-Gemini. *Async downloader* ```python response = GeminiClient.generate_content
-("Create illustrations of Seoul, South Korea.") response_images =
-response.web_images # Check generated images [Dict] await GeminiImage.save
-(response_images, "save_dir") # image_data_dict = await
-GeminiImage.fetch_images_dict(response_images) # await GeminiImage.save_images
-(image_data_dict, "save_dir") ``` Further *Sync downloader* ```python from
-gemini import Gemini, GeminiImage response = GeminiClient.generate_content
-("Please recommend a travel itinerary for Seoul.") response_images =
-response.web_images # Check response images [Dict] GeminiImage.save_sync
-(response_images, save_path="save_dir") # You can use byte type image dict as
-follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images,
-cookies) # Get bytes images dict # GeminiImage.save_images_sync
-(bytes_images_dict, path="save_dir") # Save to path ``` *Async downloader
-wrapper* ```python import asyncio from gemini import Gemini, GeminiImage async
-def save_response_web_imagse(response_images, save_path="save_dir",
-cookies=cookies): await GeminiImage.save(response_images, save_path=save_path,
-cookies=cookies) # Run the async function if __name__ == "__main__": cookies =
-{"key" : "value"} response_images = response.web_images asyncio.run
-(save_response_web_imagse(response_images, save_path="save_dir",
+Gemini. *Async downloader* ```python response = client.generate_content("Create
+illustrations of Seoul, South Korea.") response_images = response.web_images #
+Check generated images [Dict] await GeminiImage.save(response_images,
+"save_dir") # image_data_dict = await GeminiImage.fetch_images_dict
+(response_images) # await GeminiImage.save_images(image_data_dict, "save_dir")
+``` Further *Sync downloader* ```python from gemini import Gemini, GeminiImage
+response = client.generate_content("Please recommend a travel itinerary for
+Seoul.") response_images = response.web_images # Check response images [Dict]
+GeminiImage.save_sync(response_images, save_path="save_dir") # You can use byte
+type image dict as follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync
+(response_images, cookies) # Get bytes images dict #
+GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
+``` *Async downloader wrapper* ```python import asyncio from gemini import
+Gemini, GeminiImage async def save_response_web_imagse(response_images,
+save_path="save_dir", cookies=cookies): await GeminiImage.save(response_images,
+save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+"__main__": cookies = {"key" : "value"} response_images = response.web_images
+asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
 cookies=cookies)) ``` `GeminiImage.save` method logic ``` import asyncio from
 gemini import Gemini, GeminiImage async def save_response_web_imagse
 (response_images, save_path="save_dir", cookies=cookies): image_data_dict =
 await GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get
 bytes images dict asynchronously await GeminiImage.save_images(image_data_dict,
 save_path=save_path) # Run the async function if __name__ == "__main__":
 response_images = response.web_images # Check response images [Dict]
 asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
 cookies=cookies)) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
 image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. response =
-GeminiClient.generate_content("What does the text in this image say?",
-image=image) response.response_dict ```
+client.generate_content("What does the text in this image say?", image=image)
+response.response_dict ```
 ### # 08. Generate content using Google Services To begin, you must link Google
 Workspace to activate this extension via the [Gemini web extension](https://
 gemini.google.com/extensions). Please refer to the [official notice](https://
 support.google.com/gemini/answer/13695044) and review the [privacy policies]
 (https://support.google.com/gemini/answer/13594961?visit_id=638457301410420313-
 1578971242&p=privacy_help&rd=1) for more details. *extention flags* ``` @Gmail,
 @Google Drive, @Google Docs, @Google Maps, @Google Flights, @Google Hotels,
-@YouTube ``` ```python response = GeminiClient.generate_content("@YouTube
-Search clips related with Google Gemini") response.response_dict ``` Extension
+@YouTube ``` ```python response = client.generate_content("@YouTube Search
+clips related with Google Gemini") response.response_dict ``` Extension
 description - Google Workspace - Services: **@Gmail, @Google Drive, @Google
 Docs** - Description: Summarize, search, and find desired information quickly
 in your content for efficient personal task management. - Features: Information
 retrieval, document summarization, information categorization - Google Maps -
 Service: **@Google Maps** - Description: Execute plans using location-based
 information. Note: Google Maps features may be limited in some regions. -
 Features: Route guidance, nearby search, navigation - Google Flights - Service:
@@ -266,62 +268,61 @@
 conversation with a friend. - Features: Packing for travel, sightseeing,
 special relaxation - YouTube - Service: **@YouTube** - Description: Explore
 YouTube videos and ask questions about what interests you. - Features: Problem-
 solving, generating ideas, search, exploring topics
 ### # 09. Fix context setting RCID You can specify a particular response by
 setting its Response Candidate ID(RCID). ```python # Generate content for the
 prompt "Give me some information about the USA." response1 =
-GeminiClient.generate_content("Give me some information about the USA.") #
-After reviewing the responses, choose the one you prefer and copy its RCID.
-GeminiClient.rcid = "rc_xxxx" # Now, generate content for the next prompt "How
-long does it take from LA to New York?" response2 =
-GeminiClient.generate_content("How long does it take from LA to New York?") #
-However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to
-None. # GeminiClient.rcid = None ```
+client.generate_content("Give me some information about the USA.") # After
+reviewing the responses, choose the one you prefer and copy its RCID.
+client.rcid = "rc_xxxx" # Now, generate content for the next prompt "How long
+does it take from LA to New York?" response2 = client.generate_content("How
+long does it take from LA to New York?") # However, RCID may not persist. If
+parsing fails, reset `client.rcid` to None. # client.rcid = None ```
 ### # 10. Changing the Selected Response from 0 to *n* In Gemini,
 generate_content returns the first response. This may vary depending on length
 or sorting. Therefore, you can specify the index of the chosen response from 0
 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python from gemini import GeminiModelOutput GeminiModelOutput.chosen = 1 #
-default is 0 response_choice_1 = GeminiClient.generate_content("Give me some
+default is 0 response_choice_1 = client.generate_content("Give me some
 information about the USA.") # If not all Gemini returns are necessarily
 plural, revert back to 0 in case of errors. # GeminiModelOutput.chosen = 0 ```
 ### # 11. Generate custom content Parse the response text to extract desired
 values. Using `Gemini.generate_custom_content`, specify custom parsing to
 extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and
 you can pass custom parsing methods as arguments if desired. Refer to
 [custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/
 src/model/parser/custom_parser.py). ```python # You can create a parser method
 that takes response_text as the input for custom_parser. response_text,
-response_status = GeminiClient.send_request("Give me some information about the
+response_status = client.send_request("Give me some information about the
 USA.") # Use custom_parser function or class inheriting from BaseParser
-response = GeminiClient.generate_custom_content("Give me some information about
-the USA.", *custom_parser) ``` https://github.com/dsdanielpark/Gemini-API/blob/
+response = client.generate_custom_content("Give me some information about the
+USA.", *custom_parser) ``` https://github.com/dsdanielpark/Gemini-API/blob/
 31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 ## Further ### Use rotating proxies via [Smart Proxy by Crawlbase](https://
 crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api) If you want to
 **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https:
 //crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards
 your connection requests to a **randomly rotating IP address** in a pool of
 proxies before reaching the target website. The combination of AI and ML make
 it more effective to avoid CAPTCHAs and blocks. ```python # Get your proxy url
 at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://
 xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
-proxy_url} GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
-GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of
-Seoul's scenery.") ``` ### Reusable session object For standard cases, use
-Gemini class; for exceptions, use session objects. When creating a new bot
-Gemini server, adjust Headers.MAIN. ```python import requests from gemini
-import Gemini, Headers cookies = {} session = requests.Session()
-session.headers = Headers.MAIN for key, value in cookies.items():
-session.cookies.update({key: value}) GeminiClient = Gemini(session=session) #
-You can use various args response = GeminiClient.generate_content("Hello,
-Gemini. What's the weather like in Seoul today?") ```
+proxy_url} client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's
+scenery.") ``` ### Reusable session object For standard cases, use Gemini
+class; for exceptions, use session objects. When creating a new bot Gemini
+server, adjust Headers.MAIN. ```python import requests from gemini import
+Gemini, Headers cookies = {} session = requests.Session() session.headers =
+Headers.MAIN for key, value in cookies.items(): session.cookies.update({key:
+value}) client = Gemini(session=session) # You can use various args response =
+client.generate_content("Hello, Gemini. What's the weather like in Seoul
+today?") ```
 ## [More features](https://github.com/dsdanielpark/Gemini-API/blob/main/
 documents/README_DEV.md) Explore additional features in [this document](https:/
 /github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md). If you
 want to develop your own simple code, you can start from [this simple code
 example](https://github.com/dsdanielpark/Gemini-API/blob/main/script/
 sample.ipynb).
 ## Google Open-source LLMs If you have sufficient GPU resources, you can
@@ -359,20 +360,20 @@
 models with a 0-dollar token cost primarily; other models may incur charges.
 See more at [free open-source LLM API guide](https://github.com/dsdanielpark/
 Gemini-API/blob/main/documents/README_OPENROUTER.md). **Sync client is favored
 over async for Gemini due to rate limiting and blocking issues**, but
 OpenRouter offers reliable open-source LLMs for [async implementation](https://
 github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_OPENROUTER.md#openrouter-async-api-client). ```python from gemini import
-OpenRouter OPENROUTER_API_KEY = "" GemmaClient = OpenRouter
+OpenRouter OPENROUTER_API_KEY = "" gemma_client = OpenRouter
 (api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free") prompt = "Do you
 know UCA academy in Korea? https://blog.naver.com/ulsancoding" response =
-GemmaClient.create_chat_completion(prompt) print(response) # payload =
-GemmaClient.generate_content(prompt) # print(payload.json()) ``` The free model
-list includes: - `google/gemma-7b-it:free` - [google/gemma-7b](https://
+gemma_client.create_chat_completion(prompt) print(response) # payload =
+gemma_client.generate_content(prompt) # print(payload.json()) ``` The free
+model list includes: - `google/gemma-7b-it:free` - [google/gemma-7b](https://
 huggingface.co/google/gemma-7b) from Google *** - `mistralai/mistral-7b-
 instruct:free` - [mistralai/Mistral-7B-Instruct-v0.1](https://huggingface.co/
 mistralai/Mistral-7B-Instruct-v0.1) for instruction from Mistral AI **** -
 `huggingfaceh4/zephyr-7b-beta:free` - [HuggingFaceH4/zephyr-7b-beta](https://
 huggingface.co/HuggingFaceH4/zephyr-7b-beta) *** - `openchat/openchat-7b:free`
 - [openchat/openchat](https://huggingface.co/openchat/openchat) for chat ** -
 `openrouter/cinematika-7b:free` - [jondurbin/cinematika-7b-v0.1](https://
@@ -421,38 +422,29 @@
 Cheong](https://github.com/acheong08) / teapotv8@proton.me
 - [Daniel Park](https://github.com/DSDanielPark) / parkminwoo1991@gmail.com ##
 License Â©ï¸ [MIT](https://opensource.org/license/mit/) license, 2024. We
 hereby strongly disclaim any explicit or implicit legal liability related to
 our works. Users are required to use this package responsibly and at their own
 risk. This project is a personal initiative and is not affiliated with or
 endorsed by Google. It is recommended to use Google's official API. ##
-References [1]: Paper - [Introducing GEMINI: Multimodal Generative Models]
-(https://arxiv.org/abs/2312.11805)
-[2]: Website - [Google DeepMind :: GEMINI Introduction](https://
-deepmind.google/technologies/gemini/#introduction)
-[3]: Paper - [GEMMA: A Unified Language Model for Text Generation,
-Understanding, Translation, Coding, and Math.]()
-[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/
-gemma/docs)
-[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming
-Assignments](https://storage.googleapis.com/deepmind-media/gemma/
-codegemma_report.pdf?utm_source=substack&utm_medium=email)
-[6]: Blog Post - [Announcing CodeGen: Building Better Developersâ Tools Using
-LLMs](https://huggingface.co/blog/codegen)
-[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/
-collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf)
-[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard)
-[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-
-API)
-[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-
-API)
-[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/
-GoogleCloudPlatform/generative-ai)
-[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-
-runner)
-[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-
-studio_quickstart)
+References 1. [Introducing GEMINI: Multimodal Generative Models](https://
+arxiv.org/abs/2312.11805) 2. [Google DeepMind: GEMINI Introduction](https://
+deepmind.google/technologies/gemini/#introduction) 3. [GEMMA: A Unified
+Language Model for Text Generation, Understanding, Translation, Coding, and
+Math](https://arxiv.org/abs/2403.08295) 4. [AI at Google: GEMS Documentation]
+(https://ai.google.dev/gemma/docs) 5. [CodeGMMA: Large Language Models Can
+Write Realistic Programming Assignments](https://storage.googleapis.com/
+deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email)
+6. [Announcing CodeGen: Building Better Developers' Tools Using LLMs](https://
+huggingface.co/blog/codegen) 7. [Google: CodeGen Release](https://
+huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf) 8.
+[acheong08/Bard](https://github.com/acheong08/Bard) 9. [dsdanielpark/Bard-API]
+(https://github.com/dsdanielpark/Bard-API) 10. [HanaokaYuzu/Gemini-API](https:/
+/github.com/HanaokaYuzu/Gemini-API) 11. [GoogleCloudPlatform/generative-ai]
+(https://github.com/GoogleCloudPlatform/generative-ai) 12. [OpenRouter](https:/
+/github.com/OpenRouterTeam/openrouter-runner) 13. [Google AI Studio](https://
+ai.google.dev/tutorials/ai-studio_quickstart)
 > *Warning* Users assume full legal responsibility for GeminiAPI. Not endorsed
 by Google. Excessive use may lead to account restrictions. Changes in policies
 or account status may affect functionality. Utilize issue and discussion pages.
 
 ## Requirements Python 3.7 or higher.
```

### Comparing `python_gemini_api-2.4.6/gemini/__init__.py` & `python_gemini_api-2.4.7/gemini/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     from .src.modules.voice.google import google_tts, google_stt
     from .src.modules.voice.openai import openai_tts, openai_stt
 except ImportError as e:
     pass
 
 gemini_api_key = environ.get("GEMINI_COOKIES")
 
-__version__ = "2.4.6"
+__version__ = "2.4.7"
 __author__ = (
     "daniel park <parkminwoo1991@gmail.com>, antonio cheang <teapotv8@proton.me>, "
     "HanaokaYuzu, CBoYXD, veonua, thewh1teagle, jjkoh95, yihong0618, nishantchauhan949, MeemeeLab, kota113, "
     "sachnun, amit9021, zeelsheladiya, ayansengupta17, thecodekitchen, SalimLouDev, Qewertyy, "
     "senseibence, mirusu400, szv99, sudoAlireza"
 )
```

### Comparing `python_gemini_api-2.4.6/gemini/async_client.py` & `python_gemini_api-2.4.7/gemini/async_client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/client.py` & `python_gemini_api-2.4.7/gemini/client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/extensions/replit.py` & `python_gemini_api-2.4.7/gemini/src/extensions/replit.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/misc/constants.py` & `python_gemini_api-2.4.7/gemini/src/misc/constants.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/misc/decorator.py` & `python_gemini_api-2.4.7/gemini/src/misc/decorator.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/misc/exceptions.py` & `python_gemini_api-2.4.7/gemini/src/misc/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/misc/utils.py` & `python_gemini_api-2.4.7/gemini/src/misc/utils.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/model/image.py` & `python_gemini_api-2.4.7/gemini/src/model/image.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/model/output.py` & `python_gemini_api-2.4.7/gemini/src/model/output.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/model/parser/base.py` & `python_gemini_api-2.4.7/gemini/src/model/parser/base.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/model/parser/custom_parser.py` & `python_gemini_api-2.4.7/gemini/src/model/parser/custom_parser.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/model/parser/response_parser.py` & `python_gemini_api-2.4.7/gemini/src/model/parser/response_parser.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/modules/openrouter/async_client.py` & `python_gemini_api-2.4.7/gemini/src/modules/openrouter/async_client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/modules/openrouter/client.py` & `python_gemini_api-2.4.7/gemini/src/modules/openrouter/client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/modules/voice/google.py` & `python_gemini_api-2.4.7/gemini/src/modules/voice/google.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/gemini/src/modules/voice/openai.py` & `python_gemini_api-2.4.7/gemini/src/modules/voice/openai.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/python_gemini_api.egg-info/PKG-INFO` & `python_gemini_api-2.4.7/python_gemini_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gemini-api
-Version: 2.4.6
+Version: 2.4.7
 Summary: The python package that returns Response of Google Gemini through API.
 Home-page: https://github.com/dsdanielpark/Gemini-API
 Author: Daniel Park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -20,14 +20,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx[http2]>=0.20.0
 Requires-Dist: requests
 Requires-Dist: browser_cookie3
 Requires-Dist: loguru
 Requires-Dist: pydantic
+Requires-Dist: aiohttp
 Provides-Extra: voice
 Requires-Dist: gTTS; extra == "voice"
 Requires-Dist: SpeechRecognition; extra == "voice"
 Requires-Dist: openai; extra == "voice"
 Requires-Dist: anthropic; extra == "voice"
 
 
@@ -47,18 +48,17 @@
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-ba79-d9f89b637324
 
 
 
 
 
 
-A *unofficial* Python wrapper, [python-gemini-api](https://pypi.org/project/python-gemini-api/), operates through reverse-engineering, utilizing cookie values to interact with [Google Gemini](https://gemini.google.com) for users struggling with frequent authentication problems or unable to authenticate via [Google Authentication](https://developers.google.com/identity/protocols/oauth2?hl=en).
-
-Collaborated competently with [Antonio Cheong](https://github.com/acheong08).
+An **unofficial* Python wrapper, [python-gemini-api](https://pypi.org/project/python-gemini-api/), is available for users facing frequent authentication issues or unable to use [Google Authentication](https://developers.google.com/identity/protocols/oauth2?hl=en). This wrapper uses cookie values to interact with [Google Gemini](https://gemini.google.com) through reverse-engineering. The project involved a collaboration with [Antonio Cheong](https://github.com/acheong08).
 
+On the official side, Google provides partially free, clean [official Gemini APIs and SDKs](https://aistudio.google.com/), which can be accessed and utilized neatly via Python packages, [google-generativeai](https://pypi.org/project/google-generativeai/). 
 <br>
 
 <br>
 
 
 > [!TIP]
 > | 2024-03-26 | [[See Code Examples]](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md)
@@ -137,21 +137,22 @@
 
 ## Authentication
 
 1. Visit https://gemini.google.com/ <br>
     With browser open, try auto-collecting cookies first.
     ```python
     from gemini import Gemini
-    GeminiClient = Gemini(auto_cookies=True)
+    
+    client = Gemini(auto_cookies=True)
 
     # Testing needed as cookies vary by region.
-    # GeminiClient = Gemini(auto_cookies=True, target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"])
-    # GeminiClient = Gemini(auto_cookies=True, target_cookies="all") # You can pass whole cookies
+    # client = Gemini(auto_cookies=True, target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"])
+    # client = Gemini(auto_cookies=True, target_cookies="all") # You can pass whole cookies
 
-    response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
+    response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
     print(response.payload)
     ```
 2. *(Manually)* `F12` for browser console → `Session: Application` → `Cookies` → Copy the value of some working cookie sets. If it doesn't work, go to step 3.
     <details><summary>Some working cookie sets</summary>
     Cookies may vary by account or region. 
       
     First try `__Secure-1PSIDCC` alone. If it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success? Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the entire cookie file.
@@ -178,29 +179,29 @@
 
 ## Quick Start
 
 **Generate content:** returns parsed response.
 ```python
 from gemini import Gemini
 
-cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
-GeminiClient = Gemini(cookies=cookies) # You can use various args
+cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+client = Gemini(cookies=cookies) # You can use various args
 
-response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
+response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 response.payload
 ```
 
 **Generate content from image:** you can use image as input.
 ```python
 from gemini import Gemini
 
-cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
+cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+client = Gemini(cookies=cookies) # You can use various args
 
-GeminiClient = Gemini(cookies=cookies) # You can use various args
-response = GeminiClient.generate_content("What does the text in this image say?", image='folder/image.jpg')
+response = client.generate_content("What does the text in this image say?", image='folder/image.jpg')
 response.payload
 ```
 
 > [!NOTE] 
 > If the generate_content method returns an empty payload, try executing it again without reinitializing the Gemini object.
 
 <br><br>
@@ -209,14 +210,15 @@
 
 *Setting language and Gemini version using environment variables:*
 
 Setting Gemini response language (Optional): Check supported languages [here](https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes). Default is English.
 
 ```python
 import os
+
 os.environ["GEMINI_LANGUAGE"] = "KR"  # Setting Gemini response language (Optional)
 os.environ["GEMINI_ULTRA"] = "1"      # Switch to Gemini-advanced response (Experimental, Optional)
 # In some accounts, access to Gemini Ultra may not be available. If that's the case, please revert it back to "0".
 ```
 
 
 
@@ -235,17 +237,17 @@
     "__Secure-1PSIDCC" : "value",
     "__Secure-1PSID" : "value",
     "__Secure-1PSIDTS" : "value",
     "NID" : "value",
     # Cookies may vary by account or region. Consider sending the entire cookie file.
   }
 
-GeminiClient = Gemini(cookies=cookies)
-# GeminiClient = Gemini(cookie_fp="folder/cookie_file.json") # (*.json, *.txt) are supported.
-# GeminiClient = Gemini(auto_cookies=True) # Or use auto_cookies paprameter
+client = Gemini(cookies=cookies)
+# client = Gemini(cookie_fp="folder/cookie_file.json") # (*.json, *.txt) are supported.
+# client = Gemini(auto_cookies=True) # Or use auto_cookies paprameter
 ```
 
 ##### Auto Cookie Update
 For `auto_cookie` to be set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3) enables automatic cookie collection, though updates may not be complete yet.
 
 
 
@@ -253,15 +255,15 @@
 
 ### # 02. Generate content
 Returns Gemini's response, but the first one might be empty. 
 
 
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
-response = GeminiClient.generate_content(prompt)
+response = client.generate_content(prompt)
 print(response.payload)
 ```
 
 
 > [!IMPORTANT]
 >  DO NOT send same prompt repeatly. **If the session connects successfully and `generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open in the browser, cookies may expire faster. 
 
@@ -284,41 +286,41 @@
 
 ### # 03. Send request
 Send request: returns the request's payload and status_code, making debugging easier.
 ```python
 from gemini import Gemini
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
-GeminiClient = Gemini(cookies=cookies) # You can use various args
+client = Gemini(cookies=cookies) # You can use various args
 
-response_text, response_status = GeminiClient.send_request("Hello, Gemini. What's the weather like in Seoul today?")
+response_text, response_status = client.send_request("Hello, Gemini. What's the weather like in Seoul today?")
 print(response_text)
 ```
 You can track the total number of requests made by accessing the `request_count` property within the `Gemini` class.
 
 <br>
 
 ### # 04. Text generation
 Returns text generated by Gemini.
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
-response = GeminiClient.generate_content(prompt)
+response = client.generate_content(prompt)
 print(response.text)
 ```
 
 
 <br>
 
 ### # 05. Image generation
 Returns images generated by Gemini.
 
 *Async downloader*
 
 ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 generated_images = response.generated_images # Check generated images [Dict]
 
 await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
 # image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
 # await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
@@ -341,15 +343,15 @@
   ```
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+response = client.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
 GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
 
 # You can use byte type image dict for printing images as follow:
 # bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
 # GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
@@ -397,15 +399,15 @@
 
 ### # 06. Retrieving Images from Gemini Responses
 Returns images in response of Gemini.
 
 
 *Async downloader*
 ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 response_images = response.web_images # Check generated images [Dict]
 
 await GeminiImage.save(response_images, "save_dir")
 # image_data_dict = await GeminiImage.fetch_images_dict(response_images)
 # await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
@@ -413,15 +415,15 @@
 <details><summary>Further</summary>
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
-response = GeminiClient.generate_content("Please recommend a travel itinerary for Seoul.")
+response = client.generate_content("Please recommend a travel itinerary for Seoul.")
 response_images = response.web_images # Check response images [Dict]
 
 GeminiImage.save_sync(response_images, save_path="save_dir")
 
 # You can use byte type image dict as follow:
 # bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
 # GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
@@ -465,29 +467,29 @@
 ### # 07. Generate content from images
 Takes an image as input and returns a response.
 
 ```python
 image = 'folder/image.jpg'
 # image = open('folder/image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported.
 
-response = GeminiClient.generate_content("What does the text in this image say?", image=image)
+response = client.generate_content("What does the text in this image say?", image=image)
 response.response_dict
 ```
 
 <br>
 
 ### # 08. Generate content using Google Services
 To begin, you must link Google Workspace to activate this extension via the [Gemini web extension](https://gemini.google.com/extensions). Please refer to the [official notice](https://support.google.com/gemini/answer/13695044) and review the [privacy policies](https://support.google.com/gemini/answer/13594961?visit_id=638457301410420313-1578971242&p=privacy_help&rd=1) for more details.
 
 *extention flags*
 ```
 @Gmail, @Google Drive, @Google Docs, @Google Maps, @Google Flights, @Google Hotels, @YouTube
 ```
 ```python
-response = GeminiClient.generate_content("@YouTube Search clips related with Google Gemini")
+response = client.generate_content("@YouTube Search clips related with Google Gemini")
 response.response_dict
 ```
 <details><summary>Extension description</summary>
   
 - Google Workspace
   - Services: **@Gmail, @Google Drive, @Google Docs** 
   - Description: Summarize, search, and find desired information quickly in your content for efficient personal task management.
@@ -518,36 +520,36 @@
 
 
 ### # 09. Fix context setting RCID
 You can specify a particular response by setting its Response Candidate ID(RCID).
 
 ```python
 # Generate content for the prompt "Give me some information about the USA."
-response1 = GeminiClient.generate_content("Give me some information about the USA.")
+response1 = client.generate_content("Give me some information about the USA.")
 # After reviewing the responses, choose the one you prefer and copy its RCID.
-GeminiClient.rcid = "rc_xxxx"
+client.rcid = "rc_xxxx"
 
 # Now, generate content for the next prompt "How long does it take from LA to New York?"
-response2 = GeminiClient.generate_content("How long does it take from LA to New York?")
+response2 = client.generate_content("How long does it take from LA to New York?")
 
-# However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to None.
-# GeminiClient.rcid = None
+# However, RCID may not persist. If parsing fails, reset `client.rcid` to None.
+# client.rcid = None
 ```
 
 
 
 <br>
 
 ### # 10. Changing the Selected Response from 0 to *n*
 In Gemini, generate_content returns the first response. This may vary depending on length or sorting. Therefore, you can specify the index of the chosen response from 0 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python
 from gemini import GeminiModelOutput
 
 GeminiModelOutput.chosen = 1 # default is 0
-response_choice_1 = GeminiClient.generate_content("Give me some information about the USA.")
+response_choice_1 = client.generate_content("Give me some information about the USA.")
 
 # If not all Gemini returns are necessarily plural, revert back to 0 in case of errors.
 #  GeminiModelOutput.chosen = 0
 ```
 
 <br>
 
@@ -555,18 +557,18 @@
 Parse the response text to extract desired values.
 
 
 Using `Gemini.generate_custom_content`, specify custom parsing to extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and you can pass custom parsing methods as arguments if desired. Refer to [custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/src/model/parser/custom_parser.py).
 
 ```python
 # You can create a parser method that takes response_text as the input for custom_parser.
-response_text, response_status = GeminiClient.send_request("Give me some information about the USA.")
+response_text, response_status = client.send_request("Give me some information about the USA.")
 
 # Use custom_parser function or class inheriting from BaseParser
-response = GeminiClient.generate_custom_content("Give me some information about the USA.", *custom_parser)
+response = client.generate_custom_content("Give me some information about the USA.", *custom_parser)
 ```
 
 https://github.com/dsdanielpark/Gemini-API/blob/31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 <br>
 
 ## Further
 
@@ -575,16 +577,16 @@
 If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks.
 
 ```python
 # Get your proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/
 proxy_url = "http://xxxxx:@smartproxy.crawlbase.com:8012" 
 proxies = {"http": proxy_url, "https": proxy_url}
 
-GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
-GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
+client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
 ```
 
 ### Reusable session object
 For standard cases, use Gemini class; for exceptions, use session objects. When creating a new bot Gemini server, adjust Headers.MAIN.
 ```python
 import requests
 from gemini import Gemini, Headers
@@ -592,16 +594,16 @@
 cookies = {} 
 
 session = requests.Session()
 session.headers = Headers.MAIN
 for key, value in cookies.items():
     session.cookies.update({key: value})
 
-GeminiClient = Gemini(session=session) # You can use various args
-response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
+client = Gemini(session=session) # You can use various args
+response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 ```
 
 
 
 
 <br>
 
@@ -665,21 +667,21 @@
 
 **Sync client is favored over async for Gemini due to rate limiting and blocking issues**, but OpenRouter offers reliable open-source LLMs for [async implementation](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md#openrouter-async-api-client).
 
 ```python
 from gemini import OpenRouter
 
 OPENROUTER_API_KEY = "<your_open_router_api_key>"
-GemmaClient = OpenRouter(api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free")
+gemma_client = OpenRouter(api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free")
 
 prompt = "Do you know UCA academy in Korea? https://blog.naver.com/ulsancoding"
-response = GemmaClient.create_chat_completion(prompt)
+response = gemma_client.create_chat_completion(prompt)
 print(response)
 
-# payload = GemmaClient.generate_content(prompt)
+# payload = gemma_client.generate_content(prompt)
 # print(payload.json())
 ```
 
 The free model list includes:
    - `google/gemma-7b-it:free` - [google/gemma-7b](https://huggingface.co/google/gemma-7b) from Google ***
    - `mistralai/mistral-7b-instruct:free` - [mistralai/Mistral-7B-Instruct-v0.1](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.1) for instruction from Mistral AI ****
    - `huggingfaceh4/zephyr-7b-beta:free` - [HuggingFaceH4/zephyr-7b-beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta) ***
@@ -742,27 +744,29 @@
 
 
 ## License ©️ 
 [MIT](https://opensource.org/license/mit/) license, 2024. We hereby strongly disclaim any explicit or implicit legal liability related to our works. Users are required to use this package responsibly and at their own risk. This project is a personal initiative and is not affiliated with or endorsed by Google. It is recommended to use Google's official API.
 
 
 ## References
-[1]: Paper - [Introducing GEMINI: Multimodal Generative Models](https://arxiv.org/abs/2312.11805) <br>
-[2]: Website - [Google DeepMind :: GEMINI Introduction](https://deepmind.google/technologies/gemini/#introduction) <br>
-[3]: Paper - [GEMMA: A Unified Language Model for Text Generation, Understanding, Translation, Coding, and Math.]() <br>
-[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/gemma/docs) <br>
-[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming Assignments](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email) <br>
-[6]: Blog Post - [Announcing CodeGen: Building Better Developers’ Tools Using LLMs](https://huggingface.co/blog/codegen) <br>
-[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf) <br>
-[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard) <br>
-[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) <br>
-[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API) <br>
-[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai) <br>
-[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner) <br>
-[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart) <br>
+1. [Introducing GEMINI: Multimodal Generative Models](https://arxiv.org/abs/2312.11805)
+2. [Google DeepMind: GEMINI Introduction](https://deepmind.google/technologies/gemini/#introduction)
+3. [GEMMA: A Unified Language Model for Text Generation, Understanding, Translation, Coding, and Math](https://arxiv.org/abs/2403.08295)
+4. [AI at Google: GEMS Documentation](https://ai.google.dev/gemma/docs)
+5. [CodeGMMA: Large Language Models Can Write Realistic Programming Assignments](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email)
+6. [Announcing CodeGen: Building Better Developers' Tools Using LLMs](https://huggingface.co/blog/codegen)
+7. [Google: CodeGen Release](https://huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf)
+8. [acheong08/Bard](https://github.com/acheong08/Bard)
+9. [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API)
+10. [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API)
+11. [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai)
+12. [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner)
+13. [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart)
+
+<br>
 
 
 > *Warning*
 Users assume full legal responsibility for GeminiAPI. Not endorsed by Google. Excessive use may lead to account restrictions. Changes in policies or account status may affect functionality. Utilize issue and discussion pages.
 
 <br>
```

#### html2text {}

```diff
@@ -1,37 +1,41 @@
-Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.6 Summary: The
+Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.7 Summary: The
 python package that returns Response of Google Gemini through API. Home-page:
 https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
 Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: httpx[http2]>=0.20.0 Requires-
 Dist: requests Requires-Dist: browser_cookie3 Requires-Dist: loguru Requires-
-Dist: pydantic Provides-Extra: voice Requires-Dist: gTTS; extra == "voice"
-Requires-Dist: SpeechRecognition; extra == "voice" Requires-Dist: openai; extra
-== "voice" Requires-Dist: anthropic; extra == "voice" # [Gemini Icon]Gemini API
-_[_P_y_P_I_]
+Dist: pydantic Requires-Dist: aiohttp Provides-Extra: voice Requires-Dist:
+gTTS; extra == "voice" Requires-Dist: SpeechRecognition; extra == "voice"
+Requires-Dist: openai; extra == "voice" Requires-Dist: anthropic; extra ==
+"voice" # [Gemini Icon]Gemini API_[_P_y_P_I_]
   _[_p_i_p_ _d_o_w_n_l_o_a_d_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
                 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_d_s_d_a_n_i_e_l_p_a_r_k_%_2_F_G_e_m_i_n_i_-
 _A_P_I_&_c_o_u_n_t___b_g_=_%_2_3_0_0_0_0_0_0_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_v_i_e_w_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]
                                                                     _[_D_o_w_n_l_o_a_d_s_]
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-
-ba79-d9f89b637324 A *unofficial* Python wrapper, [python-gemini-api](https://
-pypi.org/project/python-gemini-api/), operates through reverse-engineering,
-utilizing cookie values to interact with [Google Gemini](https://
-gemini.google.com) for users struggling with frequent authentication problems
-or unable to authenticate via [Google Authentication](https://
-developers.google.com/identity/protocols/oauth2?hl=en). Collaborated
-competently with [Antonio Cheong](https://github.com/acheong08).
+ba79-d9f89b637324 An **unofficial* Python wrapper, [python-gemini-api](https://
+pypi.org/project/python-gemini-api/), is available for users facing frequent
+authentication issues or unable to use [Google Authentication](https://
+developers.google.com/identity/protocols/oauth2?hl=en). This wrapper uses
+cookie values to interact with [Google Gemini](https://gemini.google.com)
+through reverse-engineering. The project involved a collaboration with [Antonio
+Cheong](https://github.com/acheong08). On the official side, Google provides
+partially free, clean [official Gemini APIs and SDKs](https://
+aistudio.google.com/), which can be accessed and utilized neatly via Python
+packages, [google-generativeai](https://pypi.org/project/google-generativeai/).
+
 
 > [!TIP] > | 2024-03-26 | [[See Code Examples]](https://github.com/
 dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md) > > Check out
 temporarily free Open-source LLM APIs with Open Router. (Free limit: 10
 requests/minute)
 ## Contents - [ Gemini API ](#-gemini-api---) - [What is Gemini? ð](#what-
 is-gemini) - [Installation â](#installation-) - [Authentication â]
@@ -88,24 +92,24 @@
 in REST format. **Synchronous clients are preferred over asynchronous ones for
 Gemini because of rate limiting and blocking concerns.** ## Installation ð¦
 ``` pip install python-gemini-api ``` ``` pip install git+https://github.com/
 dsdanielpark/Gemini-API.git ``` For the updated version, use as follows: ```
 pip install -q -U python-gemini-api ``` ## Authentication 1. Visit https://
 gemini.google.com/
 With browser open, try auto-collecting cookies first. ```python from gemini
-import Gemini GeminiClient = Gemini(auto_cookies=True) # Testing needed as
-cookies vary by region. # GeminiClient = Gemini(auto_cookies=True,
-target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"]) # GeminiClient = Gemini
-(auto_cookies=True, target_cookies="all") # You can pass whole cookies response
-= GeminiClient.generate_content("Hello, Gemini. What's the weather like in
-Seoul today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser
-console â `Session: Application` â `Cookies` â Copy the value of some
-working cookie sets. If it doesn't work, go to step 3. Some working cookie sets
-Cookies may vary by account or region. First try `__Secure-1PSIDCC` alone. If
-it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
+import Gemini client = Gemini(auto_cookies=True) # Testing needed as cookies
+vary by region. # client = Gemini(auto_cookies=True, target_cookies=["__Secure-
+1PSID", "__Secure-1PSIDTS"]) # client = Gemini(auto_cookies=True,
+target_cookies="all") # You can pass whole cookies response =
+client.generate_content("Hello, Gemini. What's the weather like in Seoul
+today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser console
+â `Session: Application` â `Cookies` â Copy the value of some working
+cookie sets. If it doesn't work, go to step 3. Some working cookie sets Cookies
+may vary by account or region. First try `__Secure-1PSIDCC` alone. If it
+doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
 Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-
 1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the
 entire cookie file. 3. *(Recommended)* Export Gemini site cookies via a browser
 extension. For instance, use Chrome extension [ExportThisCookies](https://
 chromewebstore.google.com/detail/exportthiscookie/
 dannllckdimllhkiplchkcaoheibealk), open, and copy the txt file contents.
 Further: For manual collection or Required for a few users upon error 4. For
@@ -122,25 +126,26 @@
 assistant.lamda.BardFrontendService/StreamGenerate" â Payload â Form Data
 â Copy the "at" key value. See [this image](assets/nonce_value.pdf) for
 reference. > [!IMPORTANT] > Experiment with different Google accounts and
 browser settings to find a working cookie. Success may vary by IP and account
 status. Once connected, a cookie typically remains effective over a month. Keep
 testing until successful.
 ## Quick Start **Generate content:** returns parsed response. ```python from
-gemini import Gemini cookies = {} # Cookies may vary by account or region.
-Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
-# You can use various args response = GeminiClient.generate_content("Hello,
-Gemini. What's the weather like in Seoul today?") response.payload ```
+gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
+or region. Consider sending the entire cookie file. client = Gemini
+(cookies=cookies) # You can use various args response = client.generate_content
+("Hello, Gemini. What's the weather like in Seoul today?") response.payload ```
 **Generate content from image:** you can use image as input. ```python from
-gemini import Gemini cookies = {} # Cookies may vary by account or region.
-Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
-# You can use various args response = GeminiClient.generate_content("What does
-the text in this image say?", image='folder/image.jpg') response.payload ``` >
-[!NOTE] > If the generate_content method returns an empty payload, try
-executing it again without reinitializing the Gemini object.
+gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
+or region. Consider sending the entire cookie file. client = Gemini
+(cookies=cookies) # You can use various args response = client.generate_content
+("What does the text in this image say?", image='folder/image.jpg')
+response.payload ``` > [!NOTE] > If the generate_content method returns an
+empty payload, try executing it again without reinitializing the Gemini object.
+
 
 ## Usage *Setting language and Gemini version using environment variables:
 * Setting Gemini response language (Optional): Check supported languages [here]
 (https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes).
 Default is English. ```python import os os.environ["GEMINI_LANGUAGE"] = "KR" #
 Setting Gemini response language (Optional) os.environ["GEMINI_ULTRA"] = "1" #
 Switch to Gemini-advanced response (Experimental, Optional) # In some accounts,
@@ -148,73 +153,71 @@
 it back to "0". ```
 ### # 01. Initialization Please explicitly declare `cookies` in dict format.
 You can also enter the path to the file containing the cookie with `cookie_fp`
 (*.json, *.txt supported). Check sample cookie files in [assets](https://
 github.com/dsdanielpark/Gemini-API/tree/main/assets) folder. ```python from
 gemini import Gemini cookies = { "__Secure-1PSIDCC" : "value", "__Secure-1PSID"
 : "value", "__Secure-1PSIDTS" : "value", "NID" : "value", # Cookies may vary by
-account or region. Consider sending the entire cookie file. } GeminiClient =
-Gemini(cookies=cookies) # GeminiClient = Gemini(cookie_fp="folder/
-cookie_file.json") # (*.json, *.txt) are supported. # GeminiClient = Gemini
-(auto_cookies=True) # Or use auto_cookies paprameter ``` ##### Auto Cookie
-Update For `auto_cookie` to be set to `True`, and adjust `target_cookies`.
-Gemini WebUI must be active in the browser. The [browser_cookie3](https://
-github.com/borisbabic/browser_cookie3) enables automatic cookie collection,
-though updates may not be complete yet.
+account or region. Consider sending the entire cookie file. } client = Gemini
+(cookies=cookies) # client = Gemini(cookie_fp="folder/cookie_file.json") #
+(*.json, *.txt) are supported. # client = Gemini(auto_cookies=True) # Or use
+auto_cookies paprameter ``` ##### Auto Cookie Update For `auto_cookie` to be
+set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the
+browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3)
+enables automatic cookie collection, though updates may not be complete yet.
 ### # 02. Generate content Returns Gemini's response, but the first one might
 be empty. ```python prompt = "Hello, Gemini. What's the weather like in Seoul
-today?" response = GeminiClient.generate_content(prompt) print
-(response.payload) ``` > [!IMPORTANT] > DO NOT send same prompt repeatly. **If
-the session connects successfully and `generate_content` runs well, CLOSE
-Gemini website.** If Gemini web stays open in the browser, cookies may expire
-faster.
+today?" response = client.generate_content(prompt) print(response.payload) ```
+> [!IMPORTANT] > DO NOT send same prompt repeatly. **If the session connects
+successfully and `generate_content` runs well, CLOSE Gemini website.** If
+Gemini web stays open in the browser, cookies may expire faster.
 The output of the generate_content function is `GeminiModelOutput`, with the
 following structure: - *rcid*: returns the response candidate id of the chosen
 candidate. - *text*: returns the text of the chosen candidate. - *code*:
 returns the codes of the chosen candidate. - *web_images*: returns a list of
 web images from the chosen candidate. - *generated_images*: returns a list of
 generated images from the chosen candidate. - *payload*: returns the response
 dictionary, if available. https://github.com/dsdanielpark/Gemini-API/blob/
 fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 ### # 03. Send request Send request: returns the request's payload and
 status_code, making debugging easier. ```python from gemini import Gemini
 cookies = {} # Cookies may vary by account or region. Consider sending the
-entire cookie file. GeminiClient = Gemini(cookies=cookies) # You can use
-various args response_text, response_status = GeminiClient.send_request("Hello,
-Gemini. What's the weather like in Seoul today?") print(response_text) ``` You
-can track the total number of requests made by accessing the `request_count`
-property within the `Gemini` class.
+entire cookie file. client = Gemini(cookies=cookies) # You can use various args
+response_text, response_status = client.send_request("Hello, Gemini. What's the
+weather like in Seoul today?") print(response_text) ``` You can track the total
+number of requests made by accessing the `request_count` property within the
+`Gemini` class.
 ### # 04. Text generation Returns text generated by Gemini. ```python prompt =
 "Hello, Gemini. What's the weather like in Seoul today?" response =
-GeminiClient.generate_content(prompt) print(response.text) ```
+client.generate_content(prompt) print(response.text) ```
 ### # 05. Image generation Returns images generated by Gemini. *Async
-downloader* ```python response = GeminiClient.generate_content("Create
-illustrations of Seoul, South Korea.") generated_images =
-response.generated_images # Check generated images [Dict] await
-GeminiImage.save(generated_images, "save_dir", cookies=cookies) #
-image_data_dict = await GeminiImage.fetch_images_dict(generated_images,
-cookies=cookies) # await GeminiImage.save_images(image_data_dict, "save_dir")
-``` Further *Display images in IPython* You can display the image or transmit
-it to another application in byte format. ```python bytes_images_dict =
-GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes
-images dict from IPython.display import display, Image import io for
-image_name, image_bytes in bytes_images_dict.items(): print(image_name) image =
-Image(data=image_bytes) display(image) ``` *Sync downloader* ```python from
-gemini import Gemini, GeminiImage response = GeminiClient.generate_content
-("Create illustrations of Seoul, South Korea.") generated_images =
-response.generated_images # Check generated images [Dict] GeminiImage.save_sync
-(generated_images, save_path="save_dir", cookies=cookies) # You can use byte
-type image dict for printing images as follow: # bytes_images_dict =
-GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
-bytes images dict # GeminiImage.save_images_sync(bytes_images_dict,
-path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
-```python import asyncio from gemini import Gemini, GeminiImage async def
-save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
-# Run the async function if __name__ == "__main__": cookies = {"key" : "value"}
+downloader* ```python response = client.generate_content("Create illustrations
+of Seoul, South Korea.") generated_images = response.generated_images # Check
+generated images [Dict] await GeminiImage.save(generated_images, "save_dir",
+cookies=cookies) # image_data_dict = await GeminiImage.fetch_images_dict
+(generated_images, cookies=cookies) # await GeminiImage.save_images
+(image_data_dict, "save_dir") ``` Further *Display images in IPython* You can
+display the image or transmit it to another application in byte format.
+```python bytes_images_dict = GeminiImage.fetch_images_dict_sync
+(generated_images, cookies) # Get bytes images dict from IPython.display import
+display, Image import io for image_name, image_bytes in bytes_images_dict.items
+(): print(image_name) image = Image(data=image_bytes) display(image) ``` *Sync
+downloader* ```python from gemini import Gemini, GeminiImage response =
+client.generate_content("Create illustrations of Seoul, South Korea.")
+generated_images = response.generated_images # Check generated images [Dict]
+GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+# You can use byte type image dict for printing images as follow: #
+bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images,
+cookies=cookies) # Get bytes images dict # GeminiImage.save_images_sync
+(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path ``` *Async
+downloader wrapper* ```python import asyncio from gemini import Gemini,
+GeminiImage async def save_generated_imagse(generated_imagse,
+save_path="save_dir", cookies=cookies): await GeminiImage.save
+(generated_imagse, save_path=save_path, cookies=cookies) # Run the async
+function if __name__ == "__main__": cookies = {"key" : "value"}
 generated_imagse = response.generated_imagse asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ```
 `GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
 GeminiImage async def save_generated_imagse(generated_imagse,
 save_path="save_dir", cookies=cookies): image_data_dict = await
 GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies) # Get bytes
 images dict asynchronously await GeminiImage.save_images(image_data_dict,
@@ -223,56 +226,55 @@
 Check response images [Dict] asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ``` > [!NOTE] > Use
 GeminiImage for image processing. `web_images` works without cookies, but for
 images like `generated_image` from Gemini, pass cookies. Cookies are needed to
 download images from Google's storage. Check the response or use existing
 cookies variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
-Gemini. *Async downloader* ```python response = GeminiClient.generate_content
-("Create illustrations of Seoul, South Korea.") response_images =
-response.web_images # Check generated images [Dict] await GeminiImage.save
-(response_images, "save_dir") # image_data_dict = await
-GeminiImage.fetch_images_dict(response_images) # await GeminiImage.save_images
-(image_data_dict, "save_dir") ``` Further *Sync downloader* ```python from
-gemini import Gemini, GeminiImage response = GeminiClient.generate_content
-("Please recommend a travel itinerary for Seoul.") response_images =
-response.web_images # Check response images [Dict] GeminiImage.save_sync
-(response_images, save_path="save_dir") # You can use byte type image dict as
-follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images,
-cookies) # Get bytes images dict # GeminiImage.save_images_sync
-(bytes_images_dict, path="save_dir") # Save to path ``` *Async downloader
-wrapper* ```python import asyncio from gemini import Gemini, GeminiImage async
-def save_response_web_imagse(response_images, save_path="save_dir",
-cookies=cookies): await GeminiImage.save(response_images, save_path=save_path,
-cookies=cookies) # Run the async function if __name__ == "__main__": cookies =
-{"key" : "value"} response_images = response.web_images asyncio.run
-(save_response_web_imagse(response_images, save_path="save_dir",
+Gemini. *Async downloader* ```python response = client.generate_content("Create
+illustrations of Seoul, South Korea.") response_images = response.web_images #
+Check generated images [Dict] await GeminiImage.save(response_images,
+"save_dir") # image_data_dict = await GeminiImage.fetch_images_dict
+(response_images) # await GeminiImage.save_images(image_data_dict, "save_dir")
+``` Further *Sync downloader* ```python from gemini import Gemini, GeminiImage
+response = client.generate_content("Please recommend a travel itinerary for
+Seoul.") response_images = response.web_images # Check response images [Dict]
+GeminiImage.save_sync(response_images, save_path="save_dir") # You can use byte
+type image dict as follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync
+(response_images, cookies) # Get bytes images dict #
+GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
+``` *Async downloader wrapper* ```python import asyncio from gemini import
+Gemini, GeminiImage async def save_response_web_imagse(response_images,
+save_path="save_dir", cookies=cookies): await GeminiImage.save(response_images,
+save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+"__main__": cookies = {"key" : "value"} response_images = response.web_images
+asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
 cookies=cookies)) ``` `GeminiImage.save` method logic ``` import asyncio from
 gemini import Gemini, GeminiImage async def save_response_web_imagse
 (response_images, save_path="save_dir", cookies=cookies): image_data_dict =
 await GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get
 bytes images dict asynchronously await GeminiImage.save_images(image_data_dict,
 save_path=save_path) # Run the async function if __name__ == "__main__":
 response_images = response.web_images # Check response images [Dict]
 asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
 cookies=cookies)) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
 image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. response =
-GeminiClient.generate_content("What does the text in this image say?",
-image=image) response.response_dict ```
+client.generate_content("What does the text in this image say?", image=image)
+response.response_dict ```
 ### # 08. Generate content using Google Services To begin, you must link Google
 Workspace to activate this extension via the [Gemini web extension](https://
 gemini.google.com/extensions). Please refer to the [official notice](https://
 support.google.com/gemini/answer/13695044) and review the [privacy policies]
 (https://support.google.com/gemini/answer/13594961?visit_id=638457301410420313-
 1578971242&p=privacy_help&rd=1) for more details. *extention flags* ``` @Gmail,
 @Google Drive, @Google Docs, @Google Maps, @Google Flights, @Google Hotels,
-@YouTube ``` ```python response = GeminiClient.generate_content("@YouTube
-Search clips related with Google Gemini") response.response_dict ``` Extension
+@YouTube ``` ```python response = client.generate_content("@YouTube Search
+clips related with Google Gemini") response.response_dict ``` Extension
 description - Google Workspace - Services: **@Gmail, @Google Drive, @Google
 Docs** - Description: Summarize, search, and find desired information quickly
 in your content for efficient personal task management. - Features: Information
 retrieval, document summarization, information categorization - Google Maps -
 Service: **@Google Maps** - Description: Execute plans using location-based
 information. Note: Google Maps features may be limited in some regions. -
 Features: Route guidance, nearby search, navigation - Google Flights - Service:
@@ -283,62 +285,61 @@
 conversation with a friend. - Features: Packing for travel, sightseeing,
 special relaxation - YouTube - Service: **@YouTube** - Description: Explore
 YouTube videos and ask questions about what interests you. - Features: Problem-
 solving, generating ideas, search, exploring topics
 ### # 09. Fix context setting RCID You can specify a particular response by
 setting its Response Candidate ID(RCID). ```python # Generate content for the
 prompt "Give me some information about the USA." response1 =
-GeminiClient.generate_content("Give me some information about the USA.") #
-After reviewing the responses, choose the one you prefer and copy its RCID.
-GeminiClient.rcid = "rc_xxxx" # Now, generate content for the next prompt "How
-long does it take from LA to New York?" response2 =
-GeminiClient.generate_content("How long does it take from LA to New York?") #
-However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to
-None. # GeminiClient.rcid = None ```
+client.generate_content("Give me some information about the USA.") # After
+reviewing the responses, choose the one you prefer and copy its RCID.
+client.rcid = "rc_xxxx" # Now, generate content for the next prompt "How long
+does it take from LA to New York?" response2 = client.generate_content("How
+long does it take from LA to New York?") # However, RCID may not persist. If
+parsing fails, reset `client.rcid` to None. # client.rcid = None ```
 ### # 10. Changing the Selected Response from 0 to *n* In Gemini,
 generate_content returns the first response. This may vary depending on length
 or sorting. Therefore, you can specify the index of the chosen response from 0
 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python from gemini import GeminiModelOutput GeminiModelOutput.chosen = 1 #
-default is 0 response_choice_1 = GeminiClient.generate_content("Give me some
+default is 0 response_choice_1 = client.generate_content("Give me some
 information about the USA.") # If not all Gemini returns are necessarily
 plural, revert back to 0 in case of errors. # GeminiModelOutput.chosen = 0 ```
 ### # 11. Generate custom content Parse the response text to extract desired
 values. Using `Gemini.generate_custom_content`, specify custom parsing to
 extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and
 you can pass custom parsing methods as arguments if desired. Refer to
 [custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/
 src/model/parser/custom_parser.py). ```python # You can create a parser method
 that takes response_text as the input for custom_parser. response_text,
-response_status = GeminiClient.send_request("Give me some information about the
+response_status = client.send_request("Give me some information about the
 USA.") # Use custom_parser function or class inheriting from BaseParser
-response = GeminiClient.generate_custom_content("Give me some information about
-the USA.", *custom_parser) ``` https://github.com/dsdanielpark/Gemini-API/blob/
+response = client.generate_custom_content("Give me some information about the
+USA.", *custom_parser) ``` https://github.com/dsdanielpark/Gemini-API/blob/
 31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 ## Further ### Use rotating proxies via [Smart Proxy by Crawlbase](https://
 crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api) If you want to
 **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https:
 //crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards
 your connection requests to a **randomly rotating IP address** in a pool of
 proxies before reaching the target website. The combination of AI and ML make
 it more effective to avoid CAPTCHAs and blocks. ```python # Get your proxy url
 at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://
 xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
-proxy_url} GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
-GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of
-Seoul's scenery.") ``` ### Reusable session object For standard cases, use
-Gemini class; for exceptions, use session objects. When creating a new bot
-Gemini server, adjust Headers.MAIN. ```python import requests from gemini
-import Gemini, Headers cookies = {} session = requests.Session()
-session.headers = Headers.MAIN for key, value in cookies.items():
-session.cookies.update({key: value}) GeminiClient = Gemini(session=session) #
-You can use various args response = GeminiClient.generate_content("Hello,
-Gemini. What's the weather like in Seoul today?") ```
+proxy_url} client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's
+scenery.") ``` ### Reusable session object For standard cases, use Gemini
+class; for exceptions, use session objects. When creating a new bot Gemini
+server, adjust Headers.MAIN. ```python import requests from gemini import
+Gemini, Headers cookies = {} session = requests.Session() session.headers =
+Headers.MAIN for key, value in cookies.items(): session.cookies.update({key:
+value}) client = Gemini(session=session) # You can use various args response =
+client.generate_content("Hello, Gemini. What's the weather like in Seoul
+today?") ```
 ## [More features](https://github.com/dsdanielpark/Gemini-API/blob/main/
 documents/README_DEV.md) Explore additional features in [this document](https:/
 /github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md). If you
 want to develop your own simple code, you can start from [this simple code
 example](https://github.com/dsdanielpark/Gemini-API/blob/main/script/
 sample.ipynb).
 ## Google Open-source LLMs If you have sufficient GPU resources, you can
@@ -376,20 +377,20 @@
 models with a 0-dollar token cost primarily; other models may incur charges.
 See more at [free open-source LLM API guide](https://github.com/dsdanielpark/
 Gemini-API/blob/main/documents/README_OPENROUTER.md). **Sync client is favored
 over async for Gemini due to rate limiting and blocking issues**, but
 OpenRouter offers reliable open-source LLMs for [async implementation](https://
 github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_OPENROUTER.md#openrouter-async-api-client). ```python from gemini import
-OpenRouter OPENROUTER_API_KEY = "" GemmaClient = OpenRouter
+OpenRouter OPENROUTER_API_KEY = "" gemma_client = OpenRouter
 (api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free") prompt = "Do you
 know UCA academy in Korea? https://blog.naver.com/ulsancoding" response =
-GemmaClient.create_chat_completion(prompt) print(response) # payload =
-GemmaClient.generate_content(prompt) # print(payload.json()) ``` The free model
-list includes: - `google/gemma-7b-it:free` - [google/gemma-7b](https://
+gemma_client.create_chat_completion(prompt) print(response) # payload =
+gemma_client.generate_content(prompt) # print(payload.json()) ``` The free
+model list includes: - `google/gemma-7b-it:free` - [google/gemma-7b](https://
 huggingface.co/google/gemma-7b) from Google *** - `mistralai/mistral-7b-
 instruct:free` - [mistralai/Mistral-7B-Instruct-v0.1](https://huggingface.co/
 mistralai/Mistral-7B-Instruct-v0.1) for instruction from Mistral AI **** -
 `huggingfaceh4/zephyr-7b-beta:free` - [HuggingFaceH4/zephyr-7b-beta](https://
 huggingface.co/HuggingFaceH4/zephyr-7b-beta) *** - `openchat/openchat-7b:free`
 - [openchat/openchat](https://huggingface.co/openchat/openchat) for chat ** -
 `openrouter/cinematika-7b:free` - [jondurbin/cinematika-7b-v0.1](https://
@@ -438,38 +439,29 @@
 Cheong](https://github.com/acheong08) / teapotv8@proton.me
 - [Daniel Park](https://github.com/DSDanielPark) / parkminwoo1991@gmail.com ##
 License Â©ï¸ [MIT](https://opensource.org/license/mit/) license, 2024. We
 hereby strongly disclaim any explicit or implicit legal liability related to
 our works. Users are required to use this package responsibly and at their own
 risk. This project is a personal initiative and is not affiliated with or
 endorsed by Google. It is recommended to use Google's official API. ##
-References [1]: Paper - [Introducing GEMINI: Multimodal Generative Models]
-(https://arxiv.org/abs/2312.11805)
-[2]: Website - [Google DeepMind :: GEMINI Introduction](https://
-deepmind.google/technologies/gemini/#introduction)
-[3]: Paper - [GEMMA: A Unified Language Model for Text Generation,
-Understanding, Translation, Coding, and Math.]()
-[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/
-gemma/docs)
-[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming
-Assignments](https://storage.googleapis.com/deepmind-media/gemma/
-codegemma_report.pdf?utm_source=substack&utm_medium=email)
-[6]: Blog Post - [Announcing CodeGen: Building Better Developersâ Tools Using
-LLMs](https://huggingface.co/blog/codegen)
-[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/
-collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf)
-[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard)
-[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-
-API)
-[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-
-API)
-[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/
-GoogleCloudPlatform/generative-ai)
-[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-
-runner)
-[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-
-studio_quickstart)
+References 1. [Introducing GEMINI: Multimodal Generative Models](https://
+arxiv.org/abs/2312.11805) 2. [Google DeepMind: GEMINI Introduction](https://
+deepmind.google/technologies/gemini/#introduction) 3. [GEMMA: A Unified
+Language Model for Text Generation, Understanding, Translation, Coding, and
+Math](https://arxiv.org/abs/2403.08295) 4. [AI at Google: GEMS Documentation]
+(https://ai.google.dev/gemma/docs) 5. [CodeGMMA: Large Language Models Can
+Write Realistic Programming Assignments](https://storage.googleapis.com/
+deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email)
+6. [Announcing CodeGen: Building Better Developers' Tools Using LLMs](https://
+huggingface.co/blog/codegen) 7. [Google: CodeGen Release](https://
+huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf) 8.
+[acheong08/Bard](https://github.com/acheong08/Bard) 9. [dsdanielpark/Bard-API]
+(https://github.com/dsdanielpark/Bard-API) 10. [HanaokaYuzu/Gemini-API](https:/
+/github.com/HanaokaYuzu/Gemini-API) 11. [GoogleCloudPlatform/generative-ai]
+(https://github.com/GoogleCloudPlatform/generative-ai) 12. [OpenRouter](https:/
+/github.com/OpenRouterTeam/openrouter-runner) 13. [Google AI Studio](https://
+ai.google.dev/tutorials/ai-studio_quickstart)
 > *Warning* Users assume full legal responsibility for GeminiAPI. Not endorsed
 by Google. Excessive use may lead to account restrictions. Changes in policies
 or account status may affect functionality. Utilize issue and discussion pages.
 
 ## Requirements Python 3.7 or higher.
```

### Comparing `python_gemini_api-2.4.6/python_gemini_api.egg-info/SOURCES.txt` & `python_gemini_api-2.4.7/python_gemini_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.6/setup.py` & `python_gemini_api-2.4.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     python_requires=">=3.9",
     install_requires=[
         "httpx[http2]>=0.20.0",
         "requests",
         "browser_cookie3",
         "loguru",
         "pydantic",
+        "aiohttp",
     ],
     extras_require={
         "voice": [
             "gTTS",  # Google Text-to-Speech
             "SpeechRecognition",  # Library for performing speech recognition, with support for several engines and APIs, including Google Speech Recognition
             "openai",  # OpenAI for Text-to-Speech and Speech-to-Text
             "anthropic",  # Anthropic for Text-to-Speech and Speech-to-Text
```

