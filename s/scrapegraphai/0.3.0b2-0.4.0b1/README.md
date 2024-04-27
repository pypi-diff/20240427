# Comparing `tmp/scrapegraphai-0.3.0b2.tar.gz` & `tmp/scrapegraphai-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.3.0b2.tar", max compression
+gzip compressed data, was "scrapegraphai-0.4.0b1.tar", max compression
```

## Comparing `scrapegraphai-0.3.0b2.tar` & `scrapegraphai-0.4.0b1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1065 2024-04-26 17:28:54.380029 scrapegraphai-0.3.0b2/LICENSE
--rw-r--r--   0        0        0     7907 2024-04-26 17:28:54.380029 scrapegraphai-0.3.0b2/README.md
--rw-r--r--   0        0        0     1646 2024-04-26 17:29:20.023930 scrapegraphai-0.3.0b2/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      258 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     3623 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     4628 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2494 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2191 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2380 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3120 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      202 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      829 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      290 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      839 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      584 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3375 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6860 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7236 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-26 17:28:54.408029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5165 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6444 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4507 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6118 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     1635 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      242 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1742 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1443 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0     1504 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     1070 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-04-26 17:28:54.412029 scrapegraphai-0.3.0b2/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     9534 1970-01-01 00:00:00.000000 scrapegraphai-0.3.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-27 12:46:06.048965 scrapegraphai-0.4.0b1/LICENSE
+-rw-r--r--   0        0        0     7907 2024-04-27 12:46:06.048965 scrapegraphai-0.4.0b1/README.md
+-rw-r--r--   0        0        0     1646 2024-04-27 12:46:23.221054 scrapegraphai-0.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      258 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     3817 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     4868 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2493 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2192 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2378 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3120 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      202 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-04-27 12:46:06.076965 scrapegraphai-0.4.0b1/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      290 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      839 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      584 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3729 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6860 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7236 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5165 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6444 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4507 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6118 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     1635 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      287 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1443 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0     1504 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      731 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1070 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-04-27 12:46:06.080965 scrapegraphai-0.4.0b1/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     9534 1970-01-01 00:00:00.000000 scrapegraphai-0.4.0b1/PKG-INFO
```

### Comparing `scrapegraphai-0.3.0b2/LICENSE` & `scrapegraphai-0.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/README.md` & `scrapegraphai-0.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/pyproject.toml` & `scrapegraphai-0.4.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.3.0b2"
+version = "0.4.0b1"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.4.0b1/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.4.0b1/scrapegraphai/graphs/abstract_graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,56 +37,64 @@
         llm_params = {**llm_defaults, **llm_config}
 
         # Instantiate the language model based on the model name
         if "gpt-" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["openai"][llm_params["model"]]
             except KeyError:
-                raise ValueError("Model not supported")
+                raise KeyError("Model not supported")
             return OpenAI(llm_params)
 
         elif "azure" in llm_params["model"]:
             # take the model after the last dash
             llm_params["model"] = llm_params["model"].split("/")[-1]
             try:
                 self.model_token = models_tokens["azure"][llm_params["model"]]
             except KeyError:
-                raise ValueError("Model not supported")
+                raise KeyError("Model not supported")
             return AzureOpenAI(llm_params)
 
         elif "gemini" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["gemini"][llm_params["model"]]
             except KeyError:
-                raise ValueError("Model not supported")
+                raise KeyError("Model not supported")
             return Gemini(llm_params)
 
         elif "ollama" in llm_params["model"]:
             llm_params["model"] = llm_params["model"].split("/")[-1]
 
             # allow user to set model_tokens in config
             if "model_tokens" in llm_params:
                 self.model_token = llm_params["model_tokens"]
             elif llm_params["model"] in models_tokens["ollama"]:
                 try:
                     self.model_token = models_tokens["ollama"][llm_params["model"]]
                 except KeyError:
-                    raise ValueError("Model not supported")
+                    raise KeyError("Model not supported")
 
             return Ollama(llm_params)
         elif "hugging_face" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["hugging_face"][llm_params["model"]]
             except KeyError:
-                raise ValueError("Model not supported")
+                raise KeyError("Model not supported")
             return HuggingFace(llm_params)
         else:
             raise ValueError(
                 "Model provided by the configuration not supported")
 
+    def get_state(self, key=None) -> dict:
+        """""
+        Obtain the current state
+        """
+        if key is not None:
+            return self.final_state[key]
+        return self.final_state
+
     def get_execution_info(self):
         """
         Returns the execution information of the graph.
         """
         return self.execution_info
 
     @abstractmethod
```

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.4.0b1/scrapegraphai/graphs/base_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 """
 Module for creating the base graphs
  """
 import time
+import warnings
 from langchain_community.callbacks import get_openai_callback
 
 
 class BaseGraph:
     """
     BaseGraph manages the execution flow of a graph composed of interconnected nodes.
 
     Attributes:
-        nodes (dict): A dictionary mapping each node's name to its corresponding node instance.
-        edges (dict): A dictionary representing the directed edges of the graph where each 
+        nodes (list): A dictionary mapping each node's name to its corresponding node instance.
+        edges (list): A dictionary representing the directed edges of the graph where each
                       key-value pair corresponds to the from-node and to-node relationship.
         entry_point (str): The name of the entry point node from which the graph execution begins.
 
     Methods:
-        execute(initial_state): Executes the graph's nodes starting from the entry point and 
+        execute(initial_state): Executes the graph's nodes starting from the entry point and
                                 traverses the graph based on the provided initial state.
 
     Args:
         nodes (iterable): An iterable of node instances that will be part of the graph.
-        edges (iterable): An iterable of tuples where each tuple represents a directed edge 
+        edges (iterable): An iterable of tuples where each tuple represents a directed edge
                           in the graph, defined by a pair of nodes (from_node, to_node).
         entry_point (BaseNode): The node instance that represents the entry point of the graph.
     """
 
-    def __init__(self, nodes: dict, edges: dict, entry_point: str):
+    def __init__(self, nodes: list, edges: list, entry_point: str):
         """
         Initializes the graph with nodes, edges, and the entry point.
         """
-        self.nodes = {node.node_name: node for node in nodes}
-        self.edges = self._create_edges(edges)
+
+        self.nodes = nodes
+        self.edges = self._create_edges({e for e in edges})
         self.entry_point = entry_point.node_name
 
-    def _create_edges(self, edges: dict) -> dict:
+        if nodes[0].node_name != entry_point.node_name:
+            # raise a warning if the entry point is not the first node in the list
+            warnings.warn(
+                "Careful! The entry point node is different from the first node if the graph.")
+
+    def _create_edges(self, edges: list) -> dict:
         """
         Helper method to create a dictionary of edges from the given iterable of tuples.
 
         Args:
             edges (iterable): An iterable of tuples representing the directed edges.
 
         Returns:
@@ -47,42 +54,43 @@
         edge_dict = {}
         for from_node, to_node in edges:
             edge_dict[from_node.node_name] = to_node.node_name
         return edge_dict
 
     def execute(self, initial_state: dict) -> dict:
         """
-        Executes the graph by traversing nodes starting from the entry point. The execution 
-        follows the edges based on the result of each node's execution and continues until 
+        Executes the graph by traversing nodes starting from the entry point. The execution
+        follows the edges based on the result of each node's execution and continues until
         it reaches a node with no outgoing edges.
 
         Args:
             initial_state (dict): The initial state to pass to the entry point node.
 
         Returns:
             dict: The state after execution has completed, which may have been altered by the nodes.
         """
-        current_node_name = self.entry_point
+        print(self.nodes)
+        current_node_name = self.nodes[0]
         state = initial_state
 
         # variables for tracking execution info
         total_exec_time = 0.0
         exec_info = {}
         cb_total = {
             "total_tokens": 0,
             "prompt_tokens": 0,
             "completion_tokens": 0,
             "successful_requests": 0,
             "total_cost_USD": 0.0,
         }
 
-        while current_node_name is not None:
+        for index in self.nodes:
 
             curr_time = time.time()
-            current_node = self.nodes[current_node_name]
+            current_node = index
 
             with get_openai_callback() as cb:
                 result = current_node.execute(state)
                 node_exec_time = time.time() - curr_time
                 total_exec_time += node_exec_time
 
                 cb = {
```

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.4.0b1/scrapegraphai/graphs/script_creator_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" 
+"""
 Module for creating the smart scraper
 """
 from .base_graph import BaseGraph
 from ..nodes import (
     FetchNode,
     ParseNode,
     RAGNode,
@@ -53,25 +53,25 @@
             output=["answer"],
             node_config={"llm": self.llm_model},
             library=self.library,
             website=self.source
         )
 
         return BaseGraph(
-            nodes={
+            nodes=[
                 fetch_node,
                 parse_node,
                 rag_node,
                 generate_scraper_node,
-            },
-            edges={
+            ],
+            edges=[
                 (fetch_node, parse_node),
                 (parse_node, rag_node),
                 (rag_node, generate_scraper_node)
-            },
+            ],
             entry_point=fetch_node
         )
 
     def run(self) -> str:
         """
         Executes the web scraping process and returns the answer to the prompt.
         """
```

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.4.0b1/scrapegraphai/graphs/search_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     FetchNode,
     ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
 from .abstract_graph import AbstractGraph
 
+
 class SearchGraph(AbstractGraph):
     """ 
     Module for searching info on the internet
     """
 
     def _create_graph(self):
         """
@@ -45,27 +46,27 @@
         generate_answer_node = GenerateAnswerNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
             node_config={"llm": self.llm_model},
         )
 
         return BaseGraph(
-            nodes={
+            nodes=[
                 search_internet_node,
                 fetch_node,
                 parse_node,
                 rag_node,
                 generate_answer_node,
-            },
-            edges={
+            ],
+            edges=[
                 (search_internet_node, fetch_node),
                 (fetch_node, parse_node),
                 (parse_node, rag_node),
                 (rag_node, generate_answer_node)
-            },
+            ],
             entry_point=search_internet_node
         )
 
     def run(self) -> str:
         """
         Executes the web scraping and searching process.
         """
```

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.4.0b1/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-""" 
+"""
 Module for creating the smart scraper
 """
 from .base_graph import BaseGraph
 from ..nodes import (
     FetchNode,
     ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
 from .abstract_graph import AbstractGraph
 
+
 class SmartScraperGraph(AbstractGraph):
     """
     SmartScraper is a comprehensive web scraping tool that automates the process of extracting
     information from web pages using a natural language model to interpret and answer prompts.
     """
 
     def __init__(self, prompt: str, source: str, config: dict):
@@ -48,29 +49,29 @@
         generate_answer_node = GenerateAnswerNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
             node_config={"llm": self.llm_model},
         )
 
         return BaseGraph(
-            nodes={
+            nodes=[
                 fetch_node,
                 parse_node,
                 rag_node,
                 generate_answer_node,
-            },
-            edges={
+            ],
+            edges=[
                 (fetch_node, parse_node),
                 (parse_node, rag_node),
                 (rag_node, generate_answer_node)
-            },
+            ],
             entry_point=fetch_node
         )
 
     def run(self) -> str:
         """
         Executes the web scraping process and returns the answer to the prompt.
         """
-        inputs = {"user_prompt": self.prompt, self.input_key: self.source}  
+        inputs = {"user_prompt": self.prompt, self.input_key: self.source}
         self.final_state, self.execution_info = self.graph.execute(inputs)
 
         return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.4.0b1/scrapegraphai/graphs/speech_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,27 +58,27 @@
             input="answer",
             output=["audio"],
             node_config={"tts_model": OpenAITextToSpeech(
                 self.config["tts_model"])},
         )
 
         return BaseGraph(
-            nodes={
+            nodes=[
                 fetch_node,
                 parse_node,
                 rag_node,
                 generate_answer_node,
                 text_to_speech_node
-            },
-            edges={
+            ],
+            edges=[
                 (fetch_node, parse_node),
                 (parse_node, rag_node),
                 (rag_node, generate_answer_node),
                 (generate_answer_node, text_to_speech_node)
-            },
+            ],
             entry_point=fetch_node
         )
 
     def run(self) -> str:
         """
         Executes the web scraping, summarization, and text-to-speech process.
         """
```

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.4.0b1/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.4.0b1/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.4.0b1/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.4.0b1/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/models/gemini.py` & `scrapegraphai-0.4.0b1/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.4.0b1/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/models/ollama.py` & `scrapegraphai-0.4.0b1/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/models/openai.py` & `scrapegraphai-0.4.0b1/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.4.0b1/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.4.0b1/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/fetch_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from typing import List
 from langchain_community.document_loaders import AsyncHtmlLoader
 from langchain_core.documents import Document
 from .base_node import BaseNode
 from ..utils.remover import remover
+from ..utils.proxy_generator import proxy_generator
 
 
 class FetchNode(BaseNode):
     """
     A node responsible for fetching the HTML content of a specified URL and updating
     the graph's state with this content. It uses the AsyncHtmlLoader for asynchronous
     document loading.
@@ -33,21 +34,24 @@
     Methods:
         execute(state): Fetches the HTML content for the URL specified in the state and
                         updates the state with this content under the 'document' key.
                         The 'url' key must be present in the state for the operation
                         to succeed.
     """
 
-    def __init__(self, input: str, output: List[str], node_name: str = "Fetch"):
+    def __init__(self, input: str, output: List[str], num_prox: int = True,
+                 node_name: str = "Fetch"):
         """
         Initializes the FetchHTMLNode with a node name and node type.
         Arguments:
             node_name (str): name of the node
+            prox_rotation (bool): if you wamt to rotate proxies
         """
         super().__init__(node_name, "node", input, output, 1)
+        self.num_prox = num_prox
 
     def execute(self, state):
         """
         Executes the node's logic to fetch HTML content from a specified URL and
         update the state with this content.
 
         Args:
@@ -74,14 +78,18 @@
         if not source.startswith("http"):
             compressed_document = [Document(page_content=remover(source), metadata={
                 "source": "local_dir"
             })]
 
         # if it is a URL
         else:
-            loader = AsyncHtmlLoader(source)
+            if self.num_prox > 1:
+                loader = AsyncHtmlLoader(
+                    source, proxies=proxy_generator(self.num_prox))
+            else:
+                loader = AsyncHtmlLoader(source)
             document = loader.load()
             compressed_document = [
                 Document(page_content=remover(str(document)))]
 
         state.update({self.output[0]: compressed_document})
         return state
```

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.4.0b1/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.4.0b1/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.4.0b1/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.4.0b1/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.4.0b1/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/utils/remover.py` & `scrapegraphai-0.4.0b1/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.4.0b1/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.4.0b1/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.4.0b1/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.3.0b2/PKG-INFO` & `scrapegraphai-0.4.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.3.0b2
+Version: 0.4.0b1
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >3.9,<4.0
```

