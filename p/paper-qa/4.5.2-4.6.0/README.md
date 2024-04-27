# Comparing `tmp/paper_qa-4.5.2.tar.gz` & `tmp/paper_qa-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper_qa-4.5.2.tar", last modified: Thu Apr 18 05:44:19 2024, max compression
+gzip compressed data, was "paper_qa-4.6.0.tar", last modified: Sat Apr 27 01:40:28 2024, max compression
```

## Comparing `paper_qa-4.5.2.tar` & `paper_qa-4.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:44:19.291207 paper_qa-4.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 05:42:23.000000 paper_qa-4.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-18 05:44:19.291207 paper_qa-4.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-04-18 05:42:23.000000 paper_qa-4.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-18 05:42:23.000000 paper_qa-4.5.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:44:19.291207 paper_qa-4.5.2/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-18 05:44:19.000000 paper_qa-4.5.2/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-18 05:44:19.000000 paper_qa-4.5.2/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:44:19.000000 paper_qa-4.5.2/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 05:44:19.000000 paper_qa-4.5.2/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 05:44:19.000000 paper_qa-4.5.2/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:44:19.287207 paper_qa-4.5.2/paperqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:44:19.287207 paper_qa-4.5.2/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (127)    32138 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/llms.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-18 05:42:23.000000 paper_qa-4.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 05:44:19.291207 paper_qa-4.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:44:19.291207 paper_qa-4.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    63137 2024-04-18 05:42:23.000000 paper_qa-4.5.2/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:40:28.187847 paper_qa-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 01:38:35.000000 paper_qa-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-27 01:40:28.187847 paper_qa-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-04-27 01:38:35.000000 paper_qa-4.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-27 01:38:35.000000 paper_qa-4.6.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:40:28.183847 paper_qa-4.6.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-27 01:40:28.000000 paper_qa-4.6.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-27 01:40:28.000000 paper_qa-4.6.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 01:40:28.000000 paper_qa-4.6.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-27 01:40:28.000000 paper_qa-4.6.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 01:40:28.000000 paper_qa-4.6.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:40:28.183847 paper_qa-4.6.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:40:28.183847 paper_qa-4.6.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32138 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32006 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/llms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-27 01:38:35.000000 paper_qa-4.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 01:40:28.187847 paper_qa-4.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:40:28.183847 paper_qa-4.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    63137 2024-04-27 01:38:35.000000 paper_qa-4.6.0/tests/test_paperqa.py
```

### Comparing `paper_qa-4.5.2/LICENSE` & `paper_qa-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.2/PKG-INFO` & `paper_qa-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 4.5.2
+Version: 4.6.0
 Summary: LLM Chain for answering questions from docs
 Author-email: Andrew White <white.d.andrew@gmail.com>
 Maintainer-email: James Braza <jamesbraza@gmail.com>, Andrew White <white.d.andrew@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `paper_qa-4.5.2/README.md` & `paper_qa-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.2/paper_qa.egg-info/PKG-INFO` & `paper_qa-4.6.0/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 4.5.2
+Version: 4.6.0
 Summary: LLM Chain for answering questions from docs
 Author-email: Andrew White <white.d.andrew@gmail.com>
 Maintainer-email: James Braza <jamesbraza@gmail.com>, Andrew White <white.d.andrew@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `paper_qa-4.5.2/paperqa/__init__.py` & `paper_qa-4.6.0/paperqa/__init__.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.2/paperqa/contrib/zotero.py` & `paper_qa-4.6.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.2/paperqa/docs.py` & `paper_qa-4.6.0/paperqa/docs.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.2/paperqa/llms.py` & `paper_qa-4.6.0/paperqa/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -833,27 +833,27 @@
         elif "claude" in llm:
             return AnthropicLLMModel(config={"model": llm})
         else:
             raise ValueError(f"Could not guess model type for {llm}. ")
     return OpenAILLMModel()
 
 
-def embedding_model_factory(embedding: str) -> EmbeddingModel:
+def embedding_model_factory(embedding: str, **kwargs) -> EmbeddingModel:
     if embedding == "langchain":
-        return LangchainEmbeddingModel()
-    elif embedding == "sentence-transformers":  # noqa: RET505
-        return SentenceTransformerEmbeddingModel()
-    elif embedding.startswith("hybrid"):
+        return LangchainEmbeddingModel(**kwargs)
+    if embedding == "sentence-transformers":
+        return SentenceTransformerEmbeddingModel(**kwargs)
+    if embedding.startswith("hybrid"):
         embedding_model_name = "-".join(embedding.split("-")[1:])
         return HybridEmbeddingModel(
             models=[
                 OpenAIEmbeddingModel(name=embedding_model_name),
-                SparseEmbeddingModel(),
+                SparseEmbeddingModel(**kwargs),
             ]
         )
-    elif embedding == "sparse":
-        return SparseEmbeddingModel()
-    return OpenAIEmbeddingModel(name=embedding)
+    if embedding == "sparse":
+        return SparseEmbeddingModel(**kwargs)
+    return OpenAIEmbeddingModel(name=embedding, **kwargs)
 
 
 def vector_store_factory(embedding: str) -> NumpyVectorStore:
     return NumpyVectorStore(embedding_model=embedding_model_factory(embedding))
```

### Comparing `paper_qa-4.5.2/paperqa/prompts.py` & `paper_qa-4.6.0/paperqa/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 select_paper_prompt = (
     "Select papers that may help answer the question below. "
     "Papers are listed as $KEY: $PAPER_INFO. "
     "Return a list of keys, separated by commas. "
     'Return "None", if no papers are applicable. '
     "Choose papers that are relevant, from reputable sources, and timely "
-    "(if the question requires timely information). \n\n"
+    "(if the question requires timely information).\n\n"
     "Question: {question}\n\n"
     "Papers: {papers}\n\n"
     "Selected keys:"
 )
 citation_prompt = (
     "Provide the citation for the following text in MLA Format. "
     "If reporting date accessed, the current year is 2024\n\n"
```

### Comparing `paper_qa-4.5.2/paperqa/readers.py` & `paper_qa-4.6.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.2/paperqa/types.py` & `paper_qa-4.6.0/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.2/paperqa/utils.py` & `paper_qa-4.6.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.2/pyproject.toml` & `paper_qa-4.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     {email = "jamesbraza@gmail.com", name = "James Braza"},
     {email = "white.d.andrew@gmail.com", name = "Andrew White"},
 ]
 name = "paper-qa"
 readme = "README.md"
 requires-python = ">=3.8"
 urls = {repository = "https://github.com/whitead/paper-qa"}
-version = "4.5.2"
+version = "4.6.0"
 
 [tool.codespell]
 check-filenames = true
 check-hidden = true
 # SEE: https://github.com/codespell-project/codespell/issues/1212#issuecomment-1744768533
 ignore-regex = ".{1024}|.*codespell-ignore.*"
 ignore-words-list = "aadd,ser"
```

### Comparing `paper_qa-4.5.2/tests/test_paperqa.py` & `paper_qa-4.6.0/tests/test_paperqa.py`

 * *Files identical despite different names*

