# Comparing `tmp/nl2query-0.1.5.tar.gz` & `tmp/nl2query-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nl2query-0.1.5.tar", max compression
+gzip compressed data, was "nl2query-0.1.6.tar", max compression
```

## Comparing `nl2query-0.1.5.tar` & `nl2query-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1073 2023-06-25 23:12:59.048784 nl2query-0.1.5/LICENSE
--rwxr-xr-x   0        0        0     3847 2023-08-12 17:39:45.212803 nl2query-0.1.5/README.md
--rwxr-xr-x   0        0        0      261 2023-08-06 23:25:17.006176 nl2query-0.1.5/nl2query/__init__.py
--rwxr-xr-x   0        0        0     1717 2023-08-06 23:25:17.009173 nl2query-0.1.5/nl2query/base.py
--rwxr-xr-x   0        0        0     4924 2023-08-12 17:04:31.284930 nl2query-0.1.5/nl2query/cypherquery.py
--rwxr-xr-x   0        0        0     3287 2023-08-12 17:04:08.893318 nl2query-0.1.5/nl2query/kustoquery.py
--rwxr-xr-x   0        0        0     3708 2023-08-12 17:03:28.059420 nl2query-0.1.5/nl2query/mongoquery.py
--rwxr-xr-x   0        0        0     3268 2023-08-12 17:05:30.862117 nl2query-0.1.5/nl2query/pandasquery.py
--rwxr-xr-x   0        0        0      499 2023-08-12 17:38:43.052542 nl2query-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 nl2query-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-27 04:11:08.690098 nl2query-0.1.6/LICENSE
+-rw-r--r--   0        0        0     6743 2024-04-27 04:11:08.690098 nl2query-0.1.6/README.md
+-rw-r--r--   0        0        0      359 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/__init__.py
+-rw-r--r--   0        0        0     1717 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/base.py
+-rw-r--r--   0        0        0     4924 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/cypherquery.py
+-rw-r--r--   0        0        0     3287 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/kustoquery.py
+-rw-r--r--   0        0        0     8278 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/mongoquery.py
+-rw-r--r--   0        0        0     3268 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/pandasquery.py
+-rw-r--r--   0        0        0      515 2024-04-27 04:11:08.690098 nl2query-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7242 1970-01-01 00:00:00.000000 nl2query-0.1.6/PKG-INFO
```

### Comparing `nl2query-0.1.5/LICENSE` & `nl2query-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.5/nl2query/base.py` & `nl2query-0.1.6/nl2query/base.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.5/nl2query/cypherquery.py` & `nl2query-0.1.6/nl2query/cypherquery.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.5/nl2query/kustoquery.py` & `nl2query-0.1.6/nl2query/kustoquery.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.5/nl2query/mongoquery.py` & `nl2query-0.1.6/nl2query/pandasquery.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,67 @@
 import re
 
+import pandas as pd
 import torch
 from transformers import AutoModelForSeq2SeqLM, AutoTokenizer
 
 from .base import QueryLanguage
 
 
-class MongoQuery(QueryLanguage):
-    """Base QueryLanguage class extended to perform query generation for MongoDB"""
+class PandasQuery(QueryLanguage):
+    """Base QueryLanguage class extended to perform query generation for Pandas"""
 
-    def __init__(
-        self,
-        collection_keys: list,
-        collection_name: str,
-        path: str = "Chirayu/nl2mongo",
-    ):
-        """Constructor for MongoQuery class"""
+    def __init__(self, df: object, df_name: str, path: str = "Chirayu/nl2pandas"):
+        """Constructor for PandasQuery class"""
         self.path = path
-        self.collection_keys = collection_keys
-        self.collection_keys.remove("index")
-        # self.keys_mapping = {'"'+key.lower()+'"' : '"'+key+'"' for key in self.collection_keys}
-        self.keys_mapping = {key.lower(): key for key in self.collection_keys}
-        self.collection_name = collection_name
+        self.df = df
+        self.df_name = df_name
+        self.col_mapping = {
+            "'" + col.lower() + "'": "'" + col + "'" for col in self.df.columns
+        }
         self._load_model()
-        # self.db = db
 
     def _load_model(self) -> object:
-        """Constructor for MongoQuery class"""
+        """Constructor for PandasQuery class"""
         model = AutoModelForSeq2SeqLM.from_pretrained(self.path)
         self.tokenizer = AutoTokenizer.from_pretrained(self.path)
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.model = model.to(device)
         return self.model, self.tokenizer
 
     def preprocess(self, text: str) -> str:
-        """Pre-Process the user's textual query by converting all the text to lowercase and inserting all the keys of collections in the query itself."""
+        """Pre-Process the user's textual query by converting all the text to lowercase and inserting columns of dataframe in the query itself."""
         text = (
-            "mongo: "
+            "pandas: "
             + text
             + " | "
-            + self.collection_name
+            + self.df_name
             + " : "
-            + ", ".join(self.collection_keys)
+            + ", ".join(self.df.columns)
         )
-        # TO-DO: Won't work nicely for (improve the splitting) - what 'pclass' has average age of passengers greater than the age of person named 'Braund, Mr. Owen Harris'?
         upper_text = {i.lower(): i for i in text.split() if i.lower() != i}
-        # print(upper_text)
+
         # print(text.lower())
         return text.lower(), upper_text
 
+        # return text
+
     def generate_query(
         self,
         textual_query: str,
-        num_beams: int = 20,
-        max_length: int = 256,
+        num_beams: int = 10,
+        max_length: int = 128,
         repetition_penalty: int = 2.5,
         length_penalty: int = 1,
         early_stopping: bool = True,
         top_p: int = 0.95,
         top_k: int = 50,
         num_return_sequences: int = 1,
     ) -> str:
-        """Execute the CodeT5 to generate the query for the MongoDB framework."""
+        """Execute the CodeT5 to generate the query for the pandas framework."""
         query, upper_text = self.preprocess(textual_query)
         input_ids = self.tokenizer.encode(
             query, return_tensors="pt", add_special_tokens=True
         )
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         input_ids = input_ids.to(device)
 
@@ -85,15 +81,15 @@
                 generated_id,
                 skip_special_tokens=True,
                 clean_up_tokenization_spaces=True,
             )
             for generated_id in generated_ids
         ][0]
         # print(query)
-        # print(self.keys_mapping)
         pattern = "|".join(
-            re.escape(key) for key in {**self.keys_mapping, **upper_text}.keys()
+            re.escape(key) for key in {**self.col_mapping, **upper_text}.keys()
         )
         query = re.sub(
-            pattern, lambda x: {**self.keys_mapping, **upper_text}[x.group()], query
+            pattern, lambda x: {**self.col_mapping, **upper_text}[x.group()], query
         )
+
         return query
```

