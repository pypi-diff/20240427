# Comparing `tmp/weblinx-0.2.4.tar.gz` & `tmp/weblinx-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weblinx-0.2.4.tar", last modified: Thu Apr  4 22:06:29 2024, max compression
+gzip compressed data, was "weblinx-0.3.0rc1.tar", last modified: Sat Apr 27 20:29:14 2024, max compression
```

## Comparing `weblinx-0.2.4.tar` & `weblinx-0.3.0rc1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.734953 weblinx-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-04 22:06:20.000000 weblinx-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-04 22:06:29.734953 weblinx-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-04 22:06:20.000000 weblinx-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:06:29.734953 weblinx-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-04 22:06:20.000000 weblinx-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.730954 weblinx-0.2.4/weblinx/
--rw-r--r--   0 runner    (1001) docker     (127)    47300 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.730954 weblinx-0.2.4/weblinx/_data/
--rw-r--r--   0 runner    (1001) docker     (127)    38206 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/_data/splits.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.730954 weblinx-0.2.4/weblinx/eval/
--rw-r--r--   0 runner    (1001) docker     (127)    18223 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/eval/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/eval/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.730954 weblinx-0.2.4/weblinx/processing/
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/dom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30700 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24575 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/truncation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.734953 weblinx-0.2.4/weblinx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/envs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34112 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/hydra.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/recs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/video.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 22:06:21.000000 weblinx-0.2.4/weblinx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.730954 weblinx-0.2.4/weblinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-04 22:06:29.000000 weblinx-0.2.4/weblinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-04 22:06:29.000000 weblinx-0.2.4/weblinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:06:29.000000 weblinx-0.2.4/weblinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 22:06:29.000000 weblinx-0.2.4/weblinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 22:06:29.000000 weblinx-0.2.4/weblinx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:14.954902 weblinx-0.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-27 20:29:05.000000 weblinx-0.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-27 20:29:14.954902 weblinx-0.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-27 20:29:05.000000 weblinx-0.3.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 20:29:14.954902 weblinx-0.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:14.950902 weblinx-0.3.0rc1/weblinx/
+-rw-r--r--   0 runner    (1001) docker     (127)    47300 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:14.950902 weblinx-0.3.0rc1/weblinx/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    38206 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/_data/splits.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:14.950902 weblinx-0.3.0rc1/weblinx/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)    18570 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/eval/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/eval/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:14.950902 weblinx-0.3.0rc1/weblinx/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/processing/dom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/processing/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/processing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31369 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/processing/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25236 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/processing/truncation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:14.954902 weblinx-0.3.0rc1/weblinx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/utils/envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34112 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/utils/hydra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/utils/recs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/utils/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 20:29:06.000000 weblinx-0.3.0rc1/weblinx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:14.950902 weblinx-0.3.0rc1/weblinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-27 20:29:14.000000 weblinx-0.3.0rc1/weblinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-27 20:29:14.000000 weblinx-0.3.0rc1/weblinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 20:29:14.000000 weblinx-0.3.0rc1/weblinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-27 20:29:14.000000 weblinx-0.3.0rc1/weblinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 20:29:14.000000 weblinx-0.3.0rc1/weblinx.egg-info/top_level.txt
```

### Comparing `weblinx-0.2.4/LICENSE` & `weblinx-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/setup.py` & `weblinx-0.3.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/__init__.py` & `weblinx-0.3.0rc1/weblinx/__init__.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/_data/splits.json` & `weblinx-0.3.0rc1/weblinx/_data/splits.json`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/eval/__init__.py` & `weblinx-0.3.0rc1/weblinx/eval/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,26 +129,30 @@
                 )
                 return False
 
     # If we reach this point, then the reference action is valid
     return True
 
 
-def process_model_results(replays, model_results, model_name=None, verbose=True):
+def process_model_results(replays, model_results, model_name=None, backward_compatible=False, verbose=True):
     """
     Processes the results for a model (i.e. the content of an entire results.json file output by a model).
     """
     processed_results = []
 
     if model_name is None:
         desc = "Processing results"
     else:
         desc = f"Processing results for {model_name}"
     for pred in tqdm(model_results, desc=desc, disable=not verbose):
         demo_name = pred["demo_name"]
+        # If the demo name has an underscore, then we only take the last part, 
+        # as the demos no longer have an author prefix to the name
+        if backward_compatible and "_" in demo_name:
+            demo_name = demo_name.split("_")[-1]
         turn_index = pred["turn_index"]
         replay = replays[demo_name]
         turn = replay[turn_index]
 
         # First, we get the reference action
         ref_action = extract_action_from_turn(turn)
 
@@ -397,14 +401,15 @@
     metrics=None,
     splits=None,
     future_turn_acc=1,
     res_fname="results.json",
     processed_fname="processed_results.json",
     score_fname_template="eval_scores.csv",
     split_file=default_split_file,
+    backward_compatible=True,
     check_hashes=True,
 ):
     """
     Unlike full_eval_and_save, this function will automatically load the replays and splits from the results_dir.
 
     """
     results_dir = Path(results_dir)
@@ -472,15 +477,15 @@
                 )
                 continue
 
             # process results and save scores as csv
             logger.info(f"Computing score for [{project} | {model_name} | {split}]")
             print("model_results length:", len(model_results))
             processed_results = process_model_results(
-                replays, model_results, model_name=model_name
+                replays, model_results, model_name=model_name, backward_compatible=backward_compatible
             )
             print("processed_results length:", len(processed_results))
 
             scores = run_evaluation(
                 processed_results,
                 metrics=metrics,
                 num_turns=future_turn_acc,
```

### Comparing `weblinx-0.2.4/weblinx/eval/__main__.py` & `weblinx-0.3.0rc1/weblinx/eval/__main__.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/eval/metrics.py` & `weblinx-0.3.0rc1/weblinx/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/processing/__init__.py` & `weblinx-0.3.0rc1/weblinx/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/processing/dom.py` & `weblinx-0.3.0rc1/weblinx/processing/dom.py`

 * *Files 10% similar despite different names*

```diff
@@ -324,28 +324,33 @@
                 for child in node.getchildren():
                     node.addprevious(child)
                 node.getparent().remove(node)
     return new_tree
 
 
 def clean_and_prune_tree(
-    dom_tree, cands_turn, max_depth=1, max_children=5, max_sibling=2
+    dom_tree, cands_turn=None, candidate_uids=None, max_depth=1, max_children=5, max_sibling=2,
 ):
     """
     This function will clean and prune the tree based on the candidates in the cands_turn. This
     is useful for removing any elements that are not candidates, and for removing any elements
     that are not needed for the ranking model.
 
     Parameters
     ----------
     dom_tree : lxml.html.HtmlElement
         The tree to clean and prune.
 
     cands_turn : list
-        The list of candidates for the turn.
+        The list of candidates for the turn. If this is None, we are expected to pass in the
+        `candidate_uids`; otherwise an error will be raised.
+    
+    candidate_uids : list, optional
+        The list of candidate uids to keep. If this is None, we are expected to pass in the
+        `cands_turn`; otherwise an error will be raised.
 
     max_depth : int, optional
         The maximum depth to prune the tree. Defaults to 1.
 
     max_children : int, optional
         The maximum number of children to keep for each candidate. Defaults to 5.
 
@@ -356,29 +361,35 @@
     -------
     lxml.html.HtmlElement
         The cleaned and pruned tree.
 
     Raises
     ------
     ValueError
-        If cands_turn is None.
+        If cands_turn is None and candidate_uids is None. Alternatively, if both
+        cands_turn and candidate_uids are passed in, an error will be raised.
     """
-    if cands_turn is None:
+    if cands_turn is None and candidate_uids is None:
         raise ValueError(
-            "cands_turn cannot be None. The dom_tree cannot be pruned this way."
+            "cands_turn or candidate_uids must be provided. The dom_tree cannot be pruned this way."
         )
 
-    if cands_turn is not None:
-        candidate_uids = [cand["uid"] for cand in cands_turn]
-        dom_tree = prune_tree(
-            dom_tree,
-            set(candidate_uids),
-            max_depth=max_depth,
-            max_children=max_children,
-            max_sibling=max_sibling,
+    if cands_turn is not None and candidate_uids is not None:
+        raise ValueError(
+            "cands_turn and candidate_uids cannot both be provided. Please provide only one."
         )
-        remove_uid_when_not_candidate(dom_tree, candidate_uids=candidate_uids)
+    if candidate_uids is None:
+        candidate_uids = [cand["uid"] for cand in cands_turn]
+    
+    dom_tree = prune_tree(
+        dom_tree,
+        set(candidate_uids),
+        max_depth=max_depth,
+        max_children=max_children,
+        max_sibling=max_sibling,
+    )
+    remove_uid_when_not_candidate(dom_tree, candidate_uids=candidate_uids)
 
     remove_html_comments(dom_tree)
     sanitize_elem_attributes(dom_tree)
 
     return dom_tree
```

### Comparing `weblinx-0.2.4/weblinx/processing/intent.py` & `weblinx-0.3.0rc1/weblinx/processing/intent.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/processing/outputs.py` & `weblinx-0.3.0rc1/weblinx/processing/outputs.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/processing/prompt.py` & `weblinx-0.3.0rc1/weblinx/processing/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,17 +349,21 @@
     that are used as context for the current turn. The reason we have a num_prev_turns parameter
     is because we want to limit the number of turns we look at, as the last num_prev_turns turns
     can be displayed by another function, such as `format_prev_turns`, separate from this.
 
     This output of this function should be used by format_utterances to display the utterances.
     """
     start_index = max(0, turn.index - num_prev_turns)
-    instructor_chat_turns = replay.filter_turns(
+    lambda_func = (
         lambda turn: turn.get("speaker") == speaker and turn.index < start_index
     )
+    if isinstance(replay, list):
+        instructor_chat_turns = list(filter(lambda_func, replay))
+    else:
+        instructor_chat_turns = replay.filter_turns(lambda_func)
     return instructor_chat_turns
 
 
 def multi_attempt_format_prev_turns_truncated(
     replay: "Replay",
     turn: "Turn",
     format_intent,
@@ -611,14 +615,15 @@
         return None
 
 
 def select_turns_and_candidates_for_prompts(
     demos,
     candidates=None,
     num_candidates=20,
+    remove_turns_without_elements=True,
 ):
     """
     This will select the turns that will be used for building the prompts. It first filters
     turns based on the intents that will be predicted, whether the turn has a validated
     screenshot, and if it's a chat turn, then whether the speaker is not the navigator.
     Then, we will select the candidates for each turn, and if we cannot find any candidates
     for a given turn, then we will find the previous turn that has candidates.
@@ -631,14 +636,17 @@
     candidates : dict, optional
         The candidates for all turns, as a dictionary of lists. If None, then the candidates
         will not be used. Defaults to None.
 
     num_candidates : int, optional
         The number of candidates to select for each turn. Defaults to 20.
 
+    remove_turns_without_elements : bool, optional
+        Whether to remove turns that do not have elements. Defaults to True.
+
     Returns
     -------
     list
         A list of dictionaries, where each dictionary contains the following keys:
         - replay: The replay for the turn
         - turn: The turn to use for the prompt
         - cands_turn: The candidates for the turn, or None if no candidates are found
@@ -659,14 +667,23 @@
         )
         turns = filter_turns(
             turns,
             lambda turn: not (
                 turn.type == "chat" and turn.get("speaker") != "navigator"
             ),
         )
+        # Remove click and textinput turns where element is None
+        if remove_turns_without_elements:
+            turns = filter_turns(
+                turns,
+                lambda turn: not (
+                    turn.intent in ("click", "change", "textinput", "submit")
+                    and turn.element is None
+                ),
+            )
 
         for i, turn in enumerate(turns):
             if candidates is None:
                 cands_turn = None
             else:
                 cands_turn = select_candidates_for_turn(
                     candidates, turn, num_candidates=num_candidates
```

### Comparing `weblinx-0.2.4/weblinx/processing/truncation.py` & `weblinx-0.3.0rc1/weblinx/processing/truncation.py`

 * *Files 2% similar despite different names*

```diff
@@ -526,14 +526,33 @@
     for k, v in elem_dict.items():
         if remove_empty and v in [None, ""]:
             continue
         element_str += f"\n[[{k}]] {v}"
 
     return element_str
 
+def convert_elem_dict_to_str_dmr(elem_dict: dict):
+    """
+    Convert an element dictionary to a string.
+    """
+    elem_dict = deepcopy(elem_dict)
+
+    element_str = f"[[tag]] {elem_dict.pop('tag')}\n"
+    element_str += f"[[xpath]] {elem_dict.pop('xpath')}\n"
+    element_str += f"[[text]] {elem_dict.pop('text')}\n"
+    element_str += f"[[bbox]] {elem_dict.pop('bbox')}\n"
+    element_str += f"[[attributes]] {elem_dict.pop('attributes')}\n"
+    element_str += f"[[children]] {elem_dict.pop('children')}"
+
+    # for other keys, we just add them to the end
+
+    for k, v in elem_dict.items():
+        element_str += f"\n[[{k}]] {v}"
+
+    return element_str
 
 def truncate_cands_turn(
     cands_turn: list,
     tokenizer: "PreTrainedTokenizer",
     num_tokens_to_remove: int,
     protected_elem_keys=("tag", "bbox"),
     copy: bool = True,
```

### Comparing `weblinx-0.2.4/weblinx/utils/__init__.py` & `weblinx-0.3.0rc1/weblinx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/utils/envs.py` & `weblinx-0.3.0rc1/weblinx/utils/envs.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/utils/format.py` & `weblinx-0.3.0rc1/weblinx/utils/format.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/utils/html.py` & `weblinx-0.3.0rc1/weblinx/utils/html.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/utils/hydra.py` & `weblinx-0.3.0rc1/weblinx/utils/hydra.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/utils/recs.py` & `weblinx-0.3.0rc1/weblinx/utils/recs.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/utils/url.py` & `weblinx-0.3.0rc1/weblinx/utils/url.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx/utils/video.py` & `weblinx-0.3.0rc1/weblinx/utils/video.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.4/weblinx.egg-info/SOURCES.txt` & `weblinx-0.3.0rc1/weblinx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

