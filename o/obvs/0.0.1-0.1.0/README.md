# Comparing `tmp/obvs-0.0.1.tar.gz` & `tmp/obvs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obvs-0.0.1.tar", max compression
+gzip compressed data, was "obvs-0.1.0.tar", max compression
```

## Comparing `obvs-0.0.1.tar` & `obvs-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2024-04-25 05:37:40.008891 obvs-0.0.1/LICENSE
--rw-r--r--   0        0        0       83 2024-02-29 04:23:57.449418 obvs-0.0.1/obvs/__init__.py
--rw-r--r--   0        0        0    17710 2024-04-25 05:54:16.193289 obvs-0.0.1/obvs/lenses.py
--rw-r--r--   0        0        0     1493 2024-04-25 05:54:16.193553 obvs-0.0.1/obvs/logging.py
--rw-r--r--   0        0        0     4542 2024-04-25 05:54:16.193772 obvs-0.0.1/obvs/metrics.py
--rw-r--r--   0        0        0    15905 2024-04-25 05:54:16.193934 obvs-0.0.1/obvs/patchscope.py
--rw-r--r--   0        0        0    10149 2024-04-25 05:54:16.194228 obvs-0.0.1/obvs/patchscope_base.py
--rw-r--r--   0        0        0     3679 2024-04-25 05:54:16.194362 obvs-0.0.1/obvs/vis.py
--rw-r--r--   0        0        0     2799 2024-04-25 05:54:16.196076 obvs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 obvs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-27 03:25:59.294279 obvs-0.1.0/LICENSE
+-rw-r--r--   0        0        0       83 2024-02-29 04:23:57.449418 obvs-0.1.0/obvs/__init__.py
+-rw-r--r--   0        0        0    19237 2024-04-26 22:23:36.259612 obvs-0.1.0/obvs/lenses.py
+-rw-r--r--   0        0        0     1493 2024-04-25 05:54:16.193553 obvs-0.1.0/obvs/logging.py
+-rw-r--r--   0        0        0     4698 2024-04-26 22:23:36.259861 obvs-0.1.0/obvs/metrics.py
+-rw-r--r--   0        0        0    15905 2024-04-25 05:54:16.193934 obvs-0.1.0/obvs/patchscope.py
+-rw-r--r--   0        0        0    10149 2024-04-25 05:54:16.194228 obvs-0.1.0/obvs/patchscope_base.py
+-rw-r--r--   0        0        0     3679 2024-04-25 05:54:16.194362 obvs-0.1.0/obvs/vis.py
+-rw-r--r--   0        0        0     2992 2024-04-27 03:39:08.117520 obvs-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 obvs-0.1.0/PKG-INFO
```

### Comparing `obvs-0.0.1/LICENSE` & `obvs-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `obvs-0.0.1/obvs/lenses.py` & `obvs-0.1.0/obvs/lenses.py`

 * *Files 7% similar despite different names*

```diff
@@ -303,14 +303,43 @@
                 cell_annotations=top_preds,
                 title="Top predicted token and its logit",
             )
         if file_name:
             fig.write_html(f'{file_name.replace(".html", "")}.html')
         return fig
 
+    def compute_surprisal_at_position(self):
+        """
+        Compute the surprisal for a specific position across all layers.
+        """
+        if "logits" not in self.data:
+            raise ValueError("Logits data not found. Please run the lens first.")
+
+        # Assuming target_token_ids is known and corresponds to the actual token ID at target_position
+        # For this example, we assume a single target token ID for simplicity.
+        # In a real scenario, this would be dynamic or calculated based on input sequence.
+        target_token_id = (
+            self.target_token_id
+        )  # This should be set or calculated based on your specific use case.
+        target_position = self.target_token_position
+        logits_at_position = self.data["logits"][
+            :,
+            target_position,
+            :,
+        ]  # Shape: (n_layers, d_vocab)
+        probabilities_at_position = torch.softmax(torch.tensor(logits_at_position), dim=-1)
+
+        # Probability of the actual next token at the given position, for all layers
+        actual_token_probabilities = probabilities_at_position[:, target_token_id]
+
+        # Surprisal calculation: negative log probability
+        surprisals = -torch.log(actual_token_probabilities)
+
+        return surprisals.numpy()  # Convert to numpy array for convenience
+
 
 class PatchscopeLogitLens(BaseLogitLens):
     """Implementation of logit-lens in patchscope framework.
     The logit-lens is defined in the patchscope framework as follows:
     S = T   (source prompt = target prompt)
     M = M*  (source model = target model)
     l* = L* (target layer = last layer)
@@ -330,15 +359,15 @@
         layers (list[int]): Indices of Transformer Layers for which the lens should be applied
         """
 
         super().__init__(model, prompt, device, layers, substring)
         self.data["logits"] = torch.zeros(
             len(self.layers),
             len(self.substring_tokens),
-            self.patchscope.tokenizer.vocab_size,
+            self.patchscope.source_model.lm_head.out_features,  # not vocab size, as gpt-j embedding dimension different to tokenizer vocab size
         )
 
     def run(self, position: int):
         """Run the logit lens for each layer in layers, for a specific position in the prompt.
 
         Args:
             position (int): Position in the prompt for which the lens should be applied
@@ -382,18 +411,19 @@
             layers (list[int]): Indices of Transformer Layers for which the lens should be applied
         """
 
         # get starting position and tokens of substring
         start_pos, substring_tokens = self.patchscope.source_position_tokens(substring)
 
         # initialize tensor for logits
+
         self.data["logits"] = torch.zeros(
             len(layers),
             len(substring_tokens),
-            self.patchscope.tokenizer.vocab_size,
+            self.patchscope.source_model.lm_head.out_features,  # not vocab size, as gpt-j embedding dimension different to tokenizer vocab size
         )
 
         # loop over all layers
         for i, layer in enumerate(layers):
             # with one forward pass, we can get the logits of every position
             with self.patchscope.source_model.trace(self.patchscope.source.prompt) as _:
                 # get the appropriate sub-module and block from source_model
```

### Comparing `obvs-0.0.1/obvs/logging.py` & `obvs-0.1.0/obvs/logging.py`

 * *Files identical despite different names*

### Comparing `obvs-0.0.1/obvs/metrics.py` & `obvs-0.1.0/obvs/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,16 @@
             true_token_index = torch.tensor(
                 [true_token_index],
                 dtype=torch.long,
                 device=logits.device,
             ).repeat(logits.size(0))
         elif (
             torch.is_tensor(true_token_index)
-            and true_token_index.dim() == 0
+            and true_token_index.dim()  # pylint: disable=use-implicit-booleaness-not-comparison-to-zero
+            == 0
             and len(logits.shape) == 2
         ):
             true_token_index = true_token_index.repeat(logits.size(0))
         elif len(logits.shape) == 1:
             true_token_index = torch.tensor(
                 [true_token_index],
                 dtype=torch.long,
@@ -86,15 +87,16 @@
             true_token_index = torch.tensor(
                 [true_token_index],
                 dtype=torch.long,
                 device=logits.device,
             ).repeat(logits.size(0))
         elif (
             torch.is_tensor(true_token_index)
-            and true_token_index.dim() == 0
+            and true_token_index.dim()  # pylint: disable=use-implicit-booleaness-not-comparison-to-zero
+            == 0
             and len(logits.shape) == 2
         ):
             true_token_index = true_token_index.repeat(logits.size(0))
         elif len(logits.shape) == 1:
             true_token_index = torch.tensor(
                 [true_token_index],
                 dtype=torch.long,
```

### Comparing `obvs-0.0.1/obvs/patchscope.py` & `obvs-0.1.0/obvs/patchscope.py`

 * *Files identical despite different names*

### Comparing `obvs-0.0.1/obvs/patchscope_base.py` & `obvs-0.1.0/obvs/patchscope_base.py`

 * *Files identical despite different names*

### Comparing `obvs-0.0.1/obvs/vis.py` & `obvs-0.1.0/obvs/vis.py`

 * *Files identical despite different names*

### Comparing `obvs-0.0.1/pyproject.toml` & `obvs-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 ###########
 # 📜 Poetry
 ###########
 [tool.poetry]
 name = "obvs"
-version = "0.0.1"
+version = "0.1.0"
 description = "Making Transformers Obvious"
 authors = ["Jamie Coombes <jamie@example.com>"]
 license = "MIT"
 packages = [{ include = "obvs" }]
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 # Everything below here is alphabetically sorted
 ipykernel = "^6.28.0"
-torch = "^2.2.0"
+torch = "==2.2.0"
 transformers = "^4.37.1"
 nnsight = "^0.2.11"
 tiktoken = "^0.5.2"
 plotly = "^5.18.0"
 typer = "^0.9.0"
 kaleido = "0.2.1"
 fsspec = "2023.9.2"
 ipython = "^8.22.2"
 ipdb = "^0.13.13"
 torchmetrics = "^1.3.1"
 einops = "^0.7.0"
 idna = "^3.7"
+pandas = "^2.2.2"
+datasets = "^2.18.0"
+jupyter = "^1.0.0"
+zstandard = "^0.22.0"
+nbstripout = "^0.7.1"
 
 [tool.poetry.dev-dependencies]
 # Everything below here is alphabetically sorted
 bandit = "^1.7.5"
 black = "^24.3.0"
+bump2version = "^1.0.1"
 detect-secrets = "1.2.0"
 flake8 = "5.0.4"
 flake8-bugbear = "^23.3.12"
 flake8-comprehensions = "^3.12.0"
 flake8-docstrings = "^1.7.0"
 flake8-eradicate = "^1.4.0"
 flake8-fixme = "^1.1.1"
@@ -43,18 +49,21 @@
 flake8-no-pep420 = "^2.4.0"
 flake8-print = "^5.0.0"
 flake8-return = "^1.2.0"
 flake8-simplify = "^0.20.0"
 ipdb = "^0.13.13"
 isort = "^5.12.0"
 jupyter-black = "^0.3.4"
+myst-parser = "^3.0.0"
 pip-audit = "^2.5.5"
 pre-commit = "^3.3.2"
-pylint = "^2.17.4"
+pylint = "^3.1.0"
 pytest = "^7.3.1"
+sphinx = "^7.3.7"
+sphinx-autoapi = "^3.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pyinstrument = "^4.6.2"
 huggingface-hub = { extras = ["cli"], version = "^0.20.3" }
 
 [build-system]
```

### Comparing `obvs-0.0.1/PKG-INFO` & `obvs-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: obvs
-Version: 0.0.1
+Version: 0.1.0
 Summary: Making Transformers Obvious
 License: MIT
 Author: Jamie Coombes
 Author-email: jamie@example.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: datasets (>=2.18.0,<3.0.0)
 Requires-Dist: einops (>=0.7.0,<0.8.0)
 Requires-Dist: fsspec (==2023.9.2)
 Requires-Dist: idna (>=3.7,<4.0)
 Requires-Dist: ipdb (>=0.13.13,<0.14.0)
 Requires-Dist: ipykernel (>=6.28.0,<7.0.0)
 Requires-Dist: ipython (>=8.22.2,<9.0.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: kaleido (==0.2.1)
+Requires-Dist: nbstripout (>=0.7.1,<0.8.0)
 Requires-Dist: nnsight (>=0.2.11,<0.3.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: plotly (>=5.18.0,<6.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
-Requires-Dist: torch (>=2.2.0,<3.0.0)
+Requires-Dist: torch (==2.2.0)
 Requires-Dist: torchmetrics (>=1.3.1,<2.0.0)
 Requires-Dist: transformers (>=4.37.1,<5.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: zstandard (>=0.22.0,<0.23.0)
```

