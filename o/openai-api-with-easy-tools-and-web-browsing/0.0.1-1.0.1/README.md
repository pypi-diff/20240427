# Comparing `tmp/openai_api_with_easy_tools_and_web_browsing-0.0.1.tar.gz` & `tmp/openai_api_with_easy_tools_and_web_browsing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_with_easy_tools_and_web_browsing-0.0.1.tar", last modified: Sat Apr 27 14:27:59 2024, max compression
+gzip compressed data, was "openai_api_with_easy_tools_and_web_browsing-1.0.1.tar", last modified: Sat Apr 27 14:44:30 2024, max compression
```

## Comparing `openai_api_with_easy_tools_and_web_browsing-0.0.1.tar` & `openai_api_with_easy_tools_and_web_browsing-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 14:27:59.912845 openai_api_with_easy_tools_and_web_browsing-0.0.1/
--rw-rw-rw-   0        0        0     1087 2024-04-26 15:11:03.000000 openai_api_with_easy_tools_and_web_browsing-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      957 2024-04-27 14:27:59.912845 openai_api_with_easy_tools_and_web_browsing-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-27 14:08:28.000000 openai_api_with_easy_tools_and_web_browsing-0.0.1/README.md
--rw-rw-rw-   0        0        0      713 2024-04-27 14:09:08.000000 openai_api_with_easy_tools_and_web_browsing-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 14:27:59.912845 openai_api_with_easy_tools_and_web_browsing-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-27 14:27:59.897219 openai_api_with_easy_tools_and_web_browsing-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 14:27:59.912845 openai_api_with_easy_tools_and_web_browsing-0.0.1/src/openai_api_with_easy_tools_and_web_browsing.egg-info/
--rw-rw-rw-   0        0        0      957 2024-04-27 14:27:59.000000 openai_api_with_easy_tools_and_web_browsing-0.0.1/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2024-04-27 14:27:59.000000 openai_api_with_easy_tools_and_web_browsing-0.0.1/src/openai_api_with_easy_tools_and_web_browsing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 14:27:59.000000 openai_api_with_easy_tools_and_web_browsing-0.0.1/src/openai_api_with_easy_tools_and_web_browsing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-27 14:27:59.000000 openai_api_with_easy_tools_and_web_browsing-0.0.1/src/openai_api_with_easy_tools_and_web_browsing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11022 2024-04-27 14:20:05.000000 openai_api_with_easy_tools_and_web_browsing-0.0.1/src/openai_api_with_easy_tools_and_web_browsing.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:27:59.897219 openai_api_with_easy_tools_and_web_browsing-0.0.1/tests/
--rw-rw-rw-   0        0        0     2596 2024-04-27 14:25:47.000000 openai_api_with_easy_tools_and_web_browsing-0.0.1/tests/test.py
--rw-rw-rw-   0        0        0     2720 2024-04-27 14:26:00.000000 openai_api_with_easy_tools_and_web_browsing-0.0.1/tests/test_fr.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:44:30.495058 openai_api_with_easy_tools_and_web_browsing-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2024-04-26 15:11:03.000000 openai_api_with_easy_tools_and_web_browsing-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3792 2024-04-27 14:44:30.495058 openai_api_with_easy_tools_and_web_browsing-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3065 2024-04-27 14:43:09.000000 openai_api_with_easy_tools_and_web_browsing-1.0.1/README.md
+-rw-rw-rw-   0        0        0      713 2024-04-27 14:44:00.000000 openai_api_with_easy_tools_and_web_browsing-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 14:44:30.495058 openai_api_with_easy_tools_and_web_browsing-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 14:44:30.479045 openai_api_with_easy_tools_and_web_browsing-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 14:44:30.495058 openai_api_with_easy_tools_and_web_browsing-1.0.1/src/openai_api_with_easy_tools_and_web_browsing.egg-info/
+-rw-rw-rw-   0        0        0     3792 2024-04-27 14:44:30.000000 openai_api_with_easy_tools_and_web_browsing-1.0.1/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2024-04-27 14:44:30.000000 openai_api_with_easy_tools_and_web_browsing-1.0.1/src/openai_api_with_easy_tools_and_web_browsing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 14:44:30.000000 openai_api_with_easy_tools_and_web_browsing-1.0.1/src/openai_api_with_easy_tools_and_web_browsing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-27 14:44:30.000000 openai_api_with_easy_tools_and_web_browsing-1.0.1/src/openai_api_with_easy_tools_and_web_browsing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11022 2024-04-27 14:20:05.000000 openai_api_with_easy_tools_and_web_browsing-1.0.1/src/openai_api_with_easy_tools_and_web_browsing.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:44:30.495058 openai_api_with_easy_tools_and_web_browsing-1.0.1/tests/
+-rw-rw-rw-   0        0        0     2596 2024-04-27 14:25:47.000000 openai_api_with_easy_tools_and_web_browsing-1.0.1/tests/test.py
+-rw-rw-rw-   0        0        0     2720 2024-04-27 14:26:00.000000 openai_api_with_easy_tools_and_web_browsing-1.0.1/tests/test_fr.py
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-0.0.1/LICENSE` & `openai_api_with_easy_tools_and_web_browsing-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_with_easy_tools_and_web_browsing-0.0.1/pyproject.toml` & `openai_api_with_easy_tools_and_web_browsing-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openai_api_with_easy_tools_and_web_browsing"
-version = "0.0.1"
+version = "1.0.1"
 authors = [
   { name="ThomLecha", email="hamster12@hotmail.fr" },
 ]
 description = "An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools"
 
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-0.0.1/src/openai_api_with_easy_tools_and_web_browsing.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.1/src/openai_api_with_easy_tools_and_web_browsing.py`

 * *Files identical despite different names*

### Comparing `openai_api_with_easy_tools_and_web_browsing-0.0.1/tests/test.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `openai_api_with_easy_tools_and_web_browsing-0.0.1/tests/test_fr.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.1/tests/test_fr.py`

 * *Files identical despite different names*

