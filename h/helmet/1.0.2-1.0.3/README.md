# Comparing `tmp/helmet-1.0.2.tar.gz` & `tmp/helmet-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helmet-1.0.2.tar", max compression
+gzip compressed data, was "helmet-1.0.3.tar", max compression
```

## Comparing `helmet-1.0.2.tar` & `helmet-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1279 2024-04-25 07:32:19.032036 helmet-1.0.2/README.md
--rw-r--r--   0        0        0      497 2024-04-25 07:32:19.036036 helmet-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2219 2024-04-25 07:32:19.036036 helmet-1.0.2/src/helmet/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:32:19.036036 helmet-1.0.2/src/helmet/explainers/__init__.py
--rw-r--r--   0        0        0     5236 2024-04-25 07:32:19.036036 helmet-1.0.2/src/helmet/explainers/gradients.py
--rw-r--r--   0        0        0      630 2024-04-25 07:32:19.036036 helmet-1.0.2/src/helmet/explainers/perturbation.py
--rw-r--r--   0        0        0       49 2024-04-25 07:32:19.036036 helmet-1.0.2/src/helmet/model/__init__.py
--rw-r--r--   0        0        0     3541 2024-04-25 07:32:19.036036 helmet-1.0.2/src/helmet/model/base_lm.py
--rw-r--r--   0        0        0     6008 2024-04-25 07:32:19.036036 helmet-1.0.2/src/helmet/model/dec_lm.py
--rw-r--r--   0        0        0     3888 2024-04-25 07:32:19.036036 helmet-1.0.2/src/helmet/updater.py
--rw-r--r--   0        0        0       79 2024-04-25 07:32:19.036036 helmet-1.0.2/src/helmet/utils/constants.py
--rw-r--r--   0        0        0     3277 2024-04-25 07:32:19.036036 helmet-1.0.2/src/helmet/utils/types.py
--rw-r--r--   0        0        0      130 2024-04-25 07:32:19.036036 helmet-1.0.2/src/helmet/utils/utils.py
--rw-r--r--   0        0        0     2039 1970-01-01 00:00:00.000000 helmet-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1279 2024-04-27 13:57:18.920018 helmet-1.0.3/README.md
+-rw-r--r--   0        0        0      497 2024-04-27 13:57:18.920018 helmet-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2652 2024-04-27 13:57:18.920018 helmet-1.0.3/src/helmet/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 13:57:18.920018 helmet-1.0.3/src/helmet/explainers/__init__.py
+-rw-r--r--   0        0        0     5236 2024-04-27 13:57:18.920018 helmet-1.0.3/src/helmet/explainers/gradients.py
+-rw-r--r--   0        0        0      630 2024-04-27 13:57:18.920018 helmet-1.0.3/src/helmet/explainers/perturbation.py
+-rw-r--r--   0        0        0       49 2024-04-27 13:57:18.920018 helmet-1.0.3/src/helmet/model/__init__.py
+-rw-r--r--   0        0        0     3783 2024-04-27 13:57:18.920018 helmet-1.0.3/src/helmet/model/base_lm.py
+-rw-r--r--   0        0        0     5904 2024-04-27 13:57:18.924018 helmet-1.0.3/src/helmet/model/dec_lm.py
+-rw-r--r--   0        0        0     3888 2024-04-27 13:57:18.924018 helmet-1.0.3/src/helmet/updater.py
+-rw-r--r--   0        0        0       79 2024-04-27 13:57:18.924018 helmet-1.0.3/src/helmet/utils/constants.py
+-rw-r--r--   0        0        0     3277 2024-04-27 13:57:18.924018 helmet-1.0.3/src/helmet/utils/types.py
+-rw-r--r--   0        0        0      130 2024-04-27 13:57:18.924018 helmet-1.0.3/src/helmet/utils/utils.py
+-rw-r--r--   0        0        0     2039 1970-01-01 00:00:00.000000 helmet-1.0.3/PKG-INFO
```

### Comparing `helmet-1.0.2/README.md` & `helmet-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `helmet-1.0.2/src/helmet/__init__.py` & `helmet-1.0.3/src/helmet/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import torch
 import transformers
 from transformers import AutoTokenizer
 
-import torch
 from helmet.model import DEC_LM
 from helmet.updater import get_or_create_project
 
 url = "http://localhost:4000"
 
 # Mapping from model_type to model class
 model_type_to_class = {
@@ -50,19 +50,25 @@
         assert torch.cuda.is_available(), AssertionError("cuda is not available")
         torch.device(device)
     
     assert model_type in ["enc", "dec", "enc-dec"], AssertionError("model_type must be either 'enc', 'dec', or 'enc-dec'")
     assert project_id is not None, AssertionError("project_id must be specified")
 
     print("updates will be sent to", platform_url)
-    print("setting up model with config", model_setup)
+    print("setting up model with config, ", model_setup)
 
     model_cls = model_type_to_class[model_type]
 
-    hfModel = model_cls.from_pretrained(model_checkpoint, trust_remote_code=True)
+    # Quantization of the model
+    if device == "cuda":
+        from transformers import BitsAndBytesConfig
+        quantization_config = BitsAndBytesConfig(llm_int8_enable_fp32_cpu_offload=True, load_in_8bit=True)
+        hfModel = model_cls.from_pretrained(model_checkpoint, trust_remote_code=True, config=quantization_config, device_map="auto", torch_dtype = torch.float16 if device == "cuda" else torch.float32)
+    else:
+        hfModel = model_cls.from_pretrained(model_checkpoint, trust_remote_code=True)
 
     if device == "cuda":
         hfModel = hfModel.to(device)
     
     hfTokenizer = AutoTokenizer.from_pretrained(model_checkpoint)
 
     modelHelper = model_type_to_implementation[model_type]
```

### Comparing `helmet-1.0.2/src/helmet/explainers/gradients.py` & `helmet-1.0.3/src/helmet/explainers/gradients.py`

 * *Files identical despite different names*

### Comparing `helmet-1.0.2/src/helmet/explainers/perturbation.py` & `helmet-1.0.3/src/helmet/explainers/perturbation.py`

 * *Files identical despite different names*

### Comparing `helmet-1.0.2/src/helmet/model/base_lm.py` & `helmet-1.0.3/src/helmet/model/base_lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import torch
-import numpy as np
+from abc import ABC, abstractmethod
 from datetime import datetime
 
-from abc import ABC, abstractmethod
+import numpy as np
+import torch
 
-from helmet.updater import update_app, get_run
+from helmet.updater import get_run, update_app
 from helmet.utils.types import Explanation, Input, Output, Run
- 
+
+
 class Base_LM(ABC):    
     def __init__(self, model_checkpoint: str, model, tokenizer, 
                  model_type: str, url: str, project_id:str, embeddings, device="cpu"):
         self.model = model
         self.model_checkpoint = model_checkpoint
         self.tokenizer = tokenizer
         self.platform_url = url
@@ -20,15 +21,19 @@
         self.device = device
         self.__post_init__()
     
     def __post_init__(self):
         self.reset_model()
         print("model loaded")
     
-    def _encode_text(self, text: str, **kwargs):
+    def _encode_text(self, text, **kwargs):
+        if isinstance(text, list):
+            text = self.tokenizer.apply_chat_template(text, tokenize = False, add_generation_prompt = True)
+            # token_ids = self.tokenizer.encode(prompt, add_special_tokens=False, return_tensors="pt")
+
         return self.tokenizer.encode_plus(text, return_tensors="pt", **kwargs)
 
     def _tokenize(self, text: str, **kwargs):
         t = self.tokenizer(text, return_tensors="pt", **kwargs)
         return t.to(self.device)
 
     def token_ids_to_string(self, output) -> str:
```

### Comparing `helmet-1.0.2/src/helmet/model/dec_lm.py` & `helmet-1.0.3/src/helmet/model/dec_lm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import time
+from operator import attrgetter
 from typing import Tuple
-import transformers
+
 import torch
-from operator import attrgetter
-import time
+import transformers
 
+from helmet.explainers.gradients import analyze_token, input_x_gradient
 from helmet.model.base_lm import Base_LM
+from helmet.utils.constants import ALTERNATIVES, CONTRASTIVE, SALIENCY
 from helmet.utils.types import *
-from helmet.utils.constants import ALTERNATIVES, SALIENCY, CONTRASTIVE
-from helmet.explainers.gradients import analyze_token, input_x_gradient
+
 
 class DEC_LM(Base_LM):
     def __init__(self, model_checkpoint: str, model: transformers.AutoModelForCausalLM, 
                  tokenizer: transformers.PreTrainedTokenizer, url: str, project_id: str, model_config: dict = {}, device="cpu"):
         self.model_type = "dec"
         self.model_config = model_config
 
@@ -22,28 +24,28 @@
             assert embeddings is not None, AssertionError(f"embeddings {model_config['embeddings']} not found in model")
         except Exception as e:
             print(e)
             raise KeyError("embeddings must be specified in model_config")
 
         super().__init__(model_checkpoint, model, tokenizer, self.model_type, url, project_id, embeddings, device)
     
-    def forward(self, inputs, max_new_tokens, **kwargs) -> Tuple[list, AlternativesExplanation]:
-        inputs["input_ids"] = inputs["input_ids"].to_device(self.device)
-        inputs["attention_mask"] = inputs["attention_mask"].to_device(self.device)
+    def forward(self, inputs, generation_args, **kwargs) -> Tuple[list, AlternativesExplanation]:
+        inputs["input_ids"] = self.to_device(inputs["input_ids"])
+        inputs["attention_mask"] = self.to_device(inputs["attention_mask"])
 
         input_len = len(inputs["input_ids"][0])
         amount_potentials = 5
 
         output = self.model.generate(
             input_ids=inputs["input_ids"], 
             attention_mask=inputs["attention_mask"],
-            use_cache=True, 
-            max_new_tokens=max_new_tokens,
-            return_dict_in_generate=True, 
-            output_scores=True # this gets the scores, while logits are unprocessed.
+            return_dict_in_generate=True,
+            output_scores=True, # this gets the scores, while logits are unprocessed.
+            **generation_args,
+            **kwargs
         )
         alternatives_per_token = []
         for i in range(len(output.scores)):
             scores = output.scores[i]
             top_k = scores.topk(amount_potentials, dim=1)
             top_k_scores = top_k.values.detach().flatten().tolist()
             top_k_indices = top_k.indices
@@ -105,20 +107,18 @@
         explanation = ContrastiveExplanation(contrastive_input=alternative_output_str, attributions=gradients)
         run.explanations.append(explanation)
 
         self.update_run(run)
 
         return explanation
 
-    def predict(self, prompt, generate_explanations=False, groundtruth=None, *args, **kwargs):
+    def predict(self, prompt, generation_args, generate_explanations=False, groundtruth=None, *args, **kwargs):
         start = time.time()
-        eos_token = False
-        max_tokens = kwargs.get("max_new_tokens", 10)
         input = self._encode_text(prompt)
-        output_token_ids, alternatives = self.forward(input, max_new_tokens=max_tokens)
+        output_token_ids, alternatives = self.forward(input, generation_args)
         output_str: str = self.token_ids_to_string(output_token_ids)
 
         # if generate_explanations:
         #     explanation_type = kwargs.get("explanation_type", None)
         #     assert explanation_type is not None, AssertionError("explanation_type must be specified if generate_explanations=True")
             
         #     explanation: Explanation = self.explain(input, output_token_ids, explanation_type)
```

### Comparing `helmet-1.0.2/src/helmet/updater.py` & `helmet-1.0.3/src/helmet/updater.py`

 * *Files identical despite different names*

### Comparing `helmet-1.0.2/src/helmet/utils/types.py` & `helmet-1.0.3/src/helmet/utils/types.py`

 * *Files identical despite different names*

### Comparing `helmet-1.0.2/PKG-INFO` & `helmet-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helmet
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Author: Jeroen
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

