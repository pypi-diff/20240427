# Comparing `tmp/scrapegraphai-0.3.0b1.tar.gz` & `tmp/scrapegraphai-0.3.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.3.0b1.tar", max compression
+gzip compressed data, was "scrapegraphai-0.3.0b2.tar", max compression
```

## Comparing `scrapegraphai-0.3.0b1.tar` & `scrapegraphai-0.3.0b2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     1065 2024-04-26 17:16:41.541549 scrapegraphai-0.3.0b1/LICENSE
--rw-r--r--   0        0        0     7907 2024-04-26 17:16:41.541549 scrapegraphai-0.3.0b1/README.md
--rw-r--r--   0        0        0     1646 2024-04-26 17:17:00.325693 scrapegraphai-0.3.0b1/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      258 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     3623 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     4628 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2494 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2191 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2380 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3120 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      202 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      829 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      290 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      839 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      539 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3375 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6893 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7236 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5165 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6444 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4507 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     1635 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      242 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1742 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1443 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0     1504 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     1070 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     9534 1970-01-01 00:00:00.000000 scrapegraphai-0.3.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-26 17:28:54.380029 scrapegraphai-0.3.0b2/LICENSE
+-rw-r--r--   0        0        0     7907 2024-04-26 17:28:54.380029 scrapegraphai-0.3.0b2/README.md
+-rw-r--r--   0        0        0     1646 2024-04-26 17:29:20.023930 scrapegraphai-0.3.0b2/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      258 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     3623 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     4628 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2494 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2191 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2380 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3120 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      202 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      290 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      839 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      584 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3375 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6860 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7236 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5165 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6444 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4507 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6118 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     1635 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      242 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1443 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0     1504 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     1070 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     9534 1970-01-01 00:00:00.000000 scrapegraphai-0.3.0b2/PKG-INFO
```

### Comparing `scrapegraphai-0.3.0b1/LICENSE` & `scrapegraphai-0.3.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/README.md` & `scrapegraphai-0.3.0b2/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/pyproject.toml` & `scrapegraphai-0.3.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.3.0b1"
+version = "0.3.0b2"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.3.0b2/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.3.0b2/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.3.0b2/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.3.0b2/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.3.0b2/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.3.0b2/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.3.0b2/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.3.0b2/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.3.0b2/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.3.0b2/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.3.0b2/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/models/gemini.py` & `scrapegraphai-0.3.0b2/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.3.0b2/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/models/ollama.py` & `scrapegraphai-0.3.0b2/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/models/openai.py` & `scrapegraphai-0.3.0b2/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.3.0b2/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.3.0b2/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 from .generate_answer_node import GenerateAnswerNode
 from .parse_node import ParseNode
 from .rag_node import RAGNode
 from .text_to_speech_node import TextToSpeechNode
 from .image_to_text_node import ImageToTextNode
 from .search_internet_node import SearchInternetNode
 from .generate_scraper_node import GenerateScraperNode
+from .search_link_node import SearchLinkNode
 from .robots_node import RobotsNode
```

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/generate_answer_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
     A node that generates an answer using a language model (LLM) based on the user's input
     and the content extracted from a webpage. It constructs a prompt from the user's input
     and the scraped content, feeds it to the LLM, and parses the LLM's response to produce
     an answer.
 
     Attributes:
-        llm (ChatOpenAI): An instance of a language model client, configured for generating answers.
+        llm: An instance of a language model client, configured for generating answers.
         node_name (str): The unique identifier name for the node, defaulting 
         to "GenerateAnswerNode".
         node_type (str): The type of the node, set to "node" indicating a 
         standard operational node.
 
     Args:
         llm: An instance of the language model client (e.g., ChatOpenAI) used 
@@ -40,15 +40,15 @@
     """
 
     def __init__(self, input: str, output: List[str], node_config: dict,
                  node_name: str = "GenerateAnswer"):
         """
         Initializes the GenerateAnswerNode with a language model client and a node name.
         Args:
-            llm (OpenAIImageToText): An instance of the OpenAIImageToText class.
+            llm: An instance of the OpenAIImageToText class.
             node_name (str): name of the node
         """
         super().__init__(node_name, "node", input, output, 2, node_config)
         self.llm_model = node_config["llm"]
 
     def execute(self, state):
         """
```

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.3.0b2/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.3.0b2/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.3.0b2/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.3.0b2/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.3.0b2/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/utils/remover.py` & `scrapegraphai-0.3.0b2/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.3.0b2/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.3.0b2/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.3.0b2/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b1/PKG-INFO` & `scrapegraphai-0.3.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.3.0b1
+Version: 0.3.0b2
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >3.9,<4.0
```

