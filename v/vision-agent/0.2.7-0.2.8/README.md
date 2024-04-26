# Comparing `tmp/vision_agent-0.2.7.tar.gz` & `tmp/vision_agent-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.2.7.tar", max compression
+gzip compressed data, was "vision_agent-0.2.8.tar", max compression
```

## Comparing `vision_agent-0.2.7.tar` & `vision_agent-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-25 17:35:32.460863 vision_agent-0.2.7/LICENSE
--rw-r--r--   0        0        0     6639 2024-04-25 17:35:32.460863 vision_agent-0.2.7/README.md
--rw-r--r--   0        0        0     2099 2024-04-25 17:35:33.044866 vision_agent-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      108 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4526 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10506 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    26024 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     7342 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0        0 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/fonts/__init__.py
--rw-r--r--   0        0        0  1594400 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     7552 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5383 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0    10539 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      413 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    43013 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7653 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/tools/video.py
--rw-r--r--   0        0        0     1792 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/type_defs.py
--rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 vision_agent-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-26 04:03:18.769806 vision_agent-0.2.8/LICENSE
+-rw-r--r--   0        0        0     6639 2024-04-26 04:03:18.769806 vision_agent-0.2.8/README.md
+-rw-r--r--   0        0        0     2099 2024-04-26 04:03:19.333807 vision_agent-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4526 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10506 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    26112 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     7342 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0        0 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/fonts/__init__.py
+-rw-r--r--   0        0        0  1594400 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     7552 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5383 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0    10539 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      413 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    43013 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7653 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     1792 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/type_defs.py
+-rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 vision_agent-0.2.8/PKG-INFO
```

### Comparing `vision_agent-0.2.7/LICENSE` & `vision_agent-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/README.md` & `vision_agent-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/pyproject.toml` & `vision_agent-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.2.7"
+version = "0.2.8"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.2.7/vision_agent/agent/agent.py` & `vision_agent-0.2.8/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/agent/easytool.py` & `vision_agent-0.2.8/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.2.8/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/agent/reflexion.py` & `vision_agent-0.2.8/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.2.8/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/agent/vision_agent.py` & `vision_agent-0.2.8/vision_agent/agent/vision_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,15 +342,17 @@
 
     for param, call_result in zip(parameters, tool_result["call_results"]):
         # Calls can fail, so we need to check if the call was successful. It can either:
         # 1. return a str or some error that's not a dictionary
         # 2. return a dictionary but not have the necessary keys
 
         if not isinstance(call_result, dict) or (
-            "bboxes" not in call_result and "heat_map" not in call_result
+            "bboxes" not in call_result
+            and "mask" not in call_result
+            and "heat_map" not in call_result
         ):
             return image_to_data
 
         # if the call was successful, then we can add the image data
         image = param["image"]
         if image not in image_to_data:
             image_to_data[image] = {
@@ -362,15 +364,16 @@
             }
 
         image_to_data[image]["bboxes"].extend(call_result.get("bboxes", []))
         image_to_data[image]["labels"].extend(call_result.get("labels", []))
         image_to_data[image]["scores"].extend(call_result.get("scores", []))
         image_to_data[image]["masks"].extend(call_result.get("masks", []))
         # only single heatmap is returned
-        image_to_data[image]["heat_map"].append(call_result.get("heat_map", []))
+        if "heat_map" in call_result:
+            image_to_data[image]["heat_map"].append(call_result["heat_map"])
         if "mask_shape" in call_result:
             image_to_data[image]["mask_shape"] = call_result["mask_shape"]
 
     return image_to_data
 
 
 def sample_n_evenly_spaced(lst: Sequence, n: int) -> Sequence:
```

### Comparing `vision_agent-0.2.7/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.2.8/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/fonts/default_font_ch_en.ttf` & `vision_agent-0.2.8/vision_agent/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/image_utils.py` & `vision_agent-0.2.8/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/llm/llm.py` & `vision_agent-0.2.8/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/lmm/lmm.py` & `vision_agent-0.2.8/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/tools/prompts.py` & `vision_agent-0.2.8/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/tools/tools.py` & `vision_agent-0.2.8/vision_agent/tools/tools.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/tools/video.py` & `vision_agent-0.2.8/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/vision_agent/type_defs.py` & `vision_agent-0.2.8/vision_agent/type_defs.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.7/PKG-INFO` & `vision_agent-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.2.7
+Version: 0.2.8
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

