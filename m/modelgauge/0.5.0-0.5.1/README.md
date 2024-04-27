# Comparing `tmp/modelgauge-0.5.0.tar.gz` & `tmp/modelgauge-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelgauge-0.5.0.tar", max compression
+gzip compressed data, was "modelgauge-0.5.1.tar", max compression
```

## Comparing `modelgauge-0.5.0.tar` & `modelgauge-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    10174 2024-04-10 19:55:36.512596 modelgauge-0.5.0/LICENSE.md
--rw-r--r--   0        0        0     1443 2024-04-15 22:05:52.195001 modelgauge-0.5.0/README.md
--rw-r--r--   0        0        0     2709 2024-04-11 19:30:18.209705 modelgauge-0.5.0/modelgauge/aggregations.py
--rw-r--r--   0        0        0      385 2024-04-12 19:02:51.769903 modelgauge-0.5.0/modelgauge/annotation.py
--rw-r--r--   0        0        0     1151 2024-04-12 19:02:51.769903 modelgauge-0.5.0/modelgauge/annotator.py
--rw-r--r--   0        0        0      429 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/annotators/README.md
--rw-r--r--   0        0        0     2529 2024-04-12 17:44:37.230043 modelgauge-0.5.0/modelgauge/base_test.py
--rw-r--r--   0        0        0     4079 2024-04-15 15:41:46.097692 modelgauge-0.5.0/modelgauge/caching.py
--rw-r--r--   0        0        0      986 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/command_line.py
--rw-r--r--   0        0        0      842 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/concurrency.py
--rw-r--r--   0        0        0     3049 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/config.py
--rw-r--r--   0        0        0      389 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/config_templates/secrets.toml
--rw-r--r--   0        0        0     1913 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/data_packing.py
--rw-r--r--   0        0        0     6856 2024-04-12 17:44:37.230043 modelgauge-0.5.0/modelgauge/dependency_helper.py
--rw-r--r--   0        0        0     3284 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/dependency_injection.py
--rw-r--r--   0        0        0     2137 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/external_data.py
--rw-r--r--   0        0        0     2378 2024-04-12 17:44:37.230043 modelgauge-0.5.0/modelgauge/general.py
--rw-r--r--   0        0        0     3902 2024-04-12 18:58:03.642894 modelgauge-0.5.0/modelgauge/instance_factory.py
--rw-r--r--   0        0        0     1330 2024-04-12 17:44:37.230043 modelgauge-0.5.0/modelgauge/load_plugins.py
--rw-r--r--   0        0        0     7485 2024-04-12 19:21:15.899936 modelgauge-0.5.0/modelgauge/main.py
--rw-r--r--   0        0        0     5278 2024-04-11 19:30:18.211705 modelgauge-0.5.0/modelgauge/multiple_choice_questions.py
--rw-r--r--   0        0        0      570 2024-04-11 19:30:18.211705 modelgauge-0.5.0/modelgauge/not_implemented.py
--rw-r--r--   0        0        0     1808 2024-04-11 19:30:18.211705 modelgauge-0.5.0/modelgauge/prompt.py
--rw-r--r--   0        0        0      539 2024-04-11 19:30:18.211705 modelgauge-0.5.0/modelgauge/prompt_formatting.py
--rw-r--r--   0        0        0     1083 2024-04-11 19:30:18.211705 modelgauge-0.5.0/modelgauge/record_init.py
--rw-r--r--   0        0        0     1282 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/records.py
--rw-r--r--   0        0        0      420 2024-04-11 19:30:18.213705 modelgauge-0.5.0/modelgauge/runners/README.md
--rw-r--r--   0        0        0     4799 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/secret_values.py
--rw-r--r--   0        0        0     6587 2024-04-12 19:02:51.769903 modelgauge-0.5.0/modelgauge/simple_test_runner.py
--rw-r--r--   0        0        0     4132 2024-04-12 19:02:51.770903 modelgauge-0.5.0/modelgauge/single_turn_prompt_response.py
--rw-r--r--   0        0        0     3011 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/sut.py
--rw-r--r--   0        0        0      803 2024-04-11 19:30:18.213705 modelgauge-0.5.0/modelgauge/sut_capabilities.py
--rw-r--r--   0        0        0     1511 2024-04-11 19:30:18.213705 modelgauge-0.5.0/modelgauge/sut_capabilities_verification.py
--rw-r--r--   0        0        0     3888 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/sut_decorator.py
--rw-r--r--   0        0        0      170 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/sut_registry.py
--rw-r--r--   0        0        0      411 2024-04-11 19:30:18.214705 modelgauge-0.5.0/modelgauge/suts/README.md
--rw-r--r--   0        0        0     5253 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/test_decorator.py
--rw-r--r--   0        0        0      188 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/test_registry.py
--rw-r--r--   0        0        0      414 2024-04-11 19:30:18.214705 modelgauge-0.5.0/modelgauge/tests/README.md
--rw-r--r--   0        0        0        4 2024-04-11 19:30:18.214705 modelgauge-0.5.0/modelgauge/tests/specifications/README.md
--rw-r--r--   0        0        0      151 2024-04-11 19:30:18.214705 modelgauge-0.5.0/modelgauge/tracked_object.py
--rw-r--r--   0        0        0     2476 2024-04-12 17:05:04.055970 modelgauge-0.5.0/modelgauge/typed_data.py
--rw-r--r--   0        0        0     3967 2024-04-15 22:05:52.198001 modelgauge-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3867 1970-01-01 00:00:00.000000 modelgauge-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    10174 2024-01-24 05:01:49.700992 modelgauge-0.5.1/LICENSE.md
+-rw-r--r--   0        0        0     1443 2024-04-16 00:43:12.304082 modelgauge-0.5.1/README.md
+-rw-r--r--   0        0        0     2709 2024-04-11 20:18:56.149725 modelgauge-0.5.1/modelgauge/aggregations.py
+-rw-r--r--   0        0        0      385 2024-04-11 20:18:56.149778 modelgauge-0.5.1/modelgauge/annotation.py
+-rw-r--r--   0        0        0     1151 2024-04-12 19:00:09.919779 modelgauge-0.5.1/modelgauge/annotator.py
+-rw-r--r--   0        0        0      429 2024-04-11 20:18:56.149914 modelgauge-0.5.1/modelgauge/annotators/README.md
+-rw-r--r--   0        0        0     2529 2024-04-12 19:00:09.920030 modelgauge-0.5.1/modelgauge/base_test.py
+-rw-r--r--   0        0        0     4079 2024-04-16 00:43:12.307534 modelgauge-0.5.1/modelgauge/caching.py
+-rw-r--r--   0        0        0      986 2024-04-11 20:18:56.150110 modelgauge-0.5.1/modelgauge/command_line.py
+-rw-r--r--   0        0        0      842 2024-04-11 20:18:56.150168 modelgauge-0.5.1/modelgauge/concurrency.py
+-rw-r--r--   0        0        0     3049 2024-04-11 20:18:56.150233 modelgauge-0.5.1/modelgauge/config.py
+-rw-r--r--   0        0        0      389 2024-04-11 20:18:56.150591 modelgauge-0.5.1/modelgauge/config_templates/secrets.toml
+-rw-r--r--   0        0        0     1913 2024-04-11 20:18:56.150656 modelgauge-0.5.1/modelgauge/data_packing.py
+-rw-r--r--   0        0        0     6856 2024-04-12 19:00:09.921774 modelgauge-0.5.1/modelgauge/dependency_helper.py
+-rw-r--r--   0        0        0     3284 2024-04-11 20:18:56.150803 modelgauge-0.5.1/modelgauge/dependency_injection.py
+-rw-r--r--   0        0        0     2137 2024-04-11 20:18:56.150871 modelgauge-0.5.1/modelgauge/external_data.py
+-rw-r--r--   0        0        0     2378 2024-04-12 19:00:09.921947 modelgauge-0.5.1/modelgauge/general.py
+-rw-r--r--   0        0        0     3902 2024-04-12 19:00:09.922138 modelgauge-0.5.1/modelgauge/instance_factory.py
+-rw-r--r--   0        0        0     1330 2024-04-12 19:00:09.922344 modelgauge-0.5.1/modelgauge/load_plugins.py
+-rw-r--r--   0        0        0     7485 2024-04-12 19:22:28.597463 modelgauge-0.5.1/modelgauge/main.py
+-rw-r--r--   0        0        0     5278 2024-04-11 20:18:56.151936 modelgauge-0.5.1/modelgauge/multiple_choice_questions.py
+-rw-r--r--   0        0        0      570 2024-04-11 20:18:56.152637 modelgauge-0.5.1/modelgauge/not_implemented.py
+-rw-r--r--   0        0        0     1808 2024-04-11 20:18:56.152948 modelgauge-0.5.1/modelgauge/prompt.py
+-rw-r--r--   0        0        0      539 2024-04-11 20:18:56.153010 modelgauge-0.5.1/modelgauge/prompt_formatting.py
+-rw-r--r--   0        0        0     1083 2024-04-11 20:18:56.153072 modelgauge-0.5.1/modelgauge/record_init.py
+-rw-r--r--   0        0        0     1282 2024-04-12 19:00:09.923035 modelgauge-0.5.1/modelgauge/records.py
+-rw-r--r--   0        0        0      420 2024-04-11 20:18:56.153219 modelgauge-0.5.1/modelgauge/runners/README.md
+-rw-r--r--   0        0        0     4799 2024-04-12 19:00:09.923328 modelgauge-0.5.1/modelgauge/secret_values.py
+-rw-r--r--   0        0        0     6587 2024-04-11 20:18:56.153351 modelgauge-0.5.1/modelgauge/simple_test_runner.py
+-rw-r--r--   0        0        0     4132 2024-04-12 19:00:09.923655 modelgauge-0.5.1/modelgauge/single_turn_prompt_response.py
+-rw-r--r--   0        0        0     3011 2024-04-12 19:00:09.923926 modelgauge-0.5.1/modelgauge/sut.py
+-rw-r--r--   0        0        0      803 2024-04-11 20:18:56.153535 modelgauge-0.5.1/modelgauge/sut_capabilities.py
+-rw-r--r--   0        0        0     1511 2024-04-11 20:18:56.153601 modelgauge-0.5.1/modelgauge/sut_capabilities_verification.py
+-rw-r--r--   0        0        0     3888 2024-04-12 19:00:09.924712 modelgauge-0.5.1/modelgauge/sut_decorator.py
+-rw-r--r--   0        0        0      170 2024-04-12 19:00:09.925183 modelgauge-0.5.1/modelgauge/sut_registry.py
+-rw-r--r--   0        0        0      411 2024-04-11 20:18:56.153842 modelgauge-0.5.1/modelgauge/suts/README.md
+-rw-r--r--   0        0        0     5253 2024-04-12 19:00:09.925984 modelgauge-0.5.1/modelgauge/test_decorator.py
+-rw-r--r--   0        0        0      188 2024-04-12 19:00:09.931759 modelgauge-0.5.1/modelgauge/test_registry.py
+-rw-r--r--   0        0        0      414 2024-04-11 20:18:56.154045 modelgauge-0.5.1/modelgauge/tests/README.md
+-rw-r--r--   0        0        0        4 2024-04-11 20:18:56.154145 modelgauge-0.5.1/modelgauge/tests/specifications/README.md
+-rw-r--r--   0        0        0      151 2024-04-11 20:18:56.155650 modelgauge-0.5.1/modelgauge/tracked_object.py
+-rw-r--r--   0        0        0     2476 2024-04-12 16:02:38.454990 modelgauge-0.5.1/modelgauge/typed_data.py
+-rw-r--r--   0        0        0     3967 2024-04-26 20:44:20.513993 modelgauge-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3867 1970-01-01 00:00:00.000000 modelgauge-0.5.1/PKG-INFO
```

### Comparing `modelgauge-0.5.0/LICENSE.md` & `modelgauge-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/README.md` & `modelgauge-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/aggregations.py` & `modelgauge-0.5.1/modelgauge/aggregations.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/annotator.py` & `modelgauge-0.5.1/modelgauge/annotator.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/base_test.py` & `modelgauge-0.5.1/modelgauge/base_test.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/caching.py` & `modelgauge-0.5.1/modelgauge/caching.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/command_line.py` & `modelgauge-0.5.1/modelgauge/command_line.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/concurrency.py` & `modelgauge-0.5.1/modelgauge/concurrency.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/config.py` & `modelgauge-0.5.1/modelgauge/config.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/data_packing.py` & `modelgauge-0.5.1/modelgauge/data_packing.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/dependency_helper.py` & `modelgauge-0.5.1/modelgauge/dependency_helper.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/dependency_injection.py` & `modelgauge-0.5.1/modelgauge/dependency_injection.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/external_data.py` & `modelgauge-0.5.1/modelgauge/external_data.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/general.py` & `modelgauge-0.5.1/modelgauge/general.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/instance_factory.py` & `modelgauge-0.5.1/modelgauge/instance_factory.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/load_plugins.py` & `modelgauge-0.5.1/modelgauge/load_plugins.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/main.py` & `modelgauge-0.5.1/modelgauge/main.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/multiple_choice_questions.py` & `modelgauge-0.5.1/modelgauge/multiple_choice_questions.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/not_implemented.py` & `modelgauge-0.5.1/modelgauge/not_implemented.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/prompt.py` & `modelgauge-0.5.1/modelgauge/prompt.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/prompt_formatting.py` & `modelgauge-0.5.1/modelgauge/prompt_formatting.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/record_init.py` & `modelgauge-0.5.1/modelgauge/record_init.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/records.py` & `modelgauge-0.5.1/modelgauge/records.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/secret_values.py` & `modelgauge-0.5.1/modelgauge/secret_values.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/simple_test_runner.py` & `modelgauge-0.5.1/modelgauge/simple_test_runner.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/single_turn_prompt_response.py` & `modelgauge-0.5.1/modelgauge/single_turn_prompt_response.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/sut.py` & `modelgauge-0.5.1/modelgauge/sut.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/sut_capabilities.py` & `modelgauge-0.5.1/modelgauge/sut_capabilities.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/sut_capabilities_verification.py` & `modelgauge-0.5.1/modelgauge/sut_capabilities_verification.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/sut_decorator.py` & `modelgauge-0.5.1/modelgauge/sut_decorator.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/test_decorator.py` & `modelgauge-0.5.1/modelgauge/test_decorator.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/modelgauge/typed_data.py` & `modelgauge-0.5.1/modelgauge/typed_data.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.5.0/pyproject.toml` & `modelgauge-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelgauge"
-version = "0.5.0"
+version = "0.5.1"
 description = "Automatically and uniformly measure the behavior of many AI Systems."
 license = "Apache-2.0"
 authors = ["MLCommons AI Safety <ai-safety-engineering@mlcommons.org>"]
 readme = "README.md"
 repository = "https://github.com/mlcommons/modelgauge"
 keywords = [
     "AI",
```

### Comparing `modelgauge-0.5.0/PKG-INFO` & `modelgauge-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelgauge
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automatically and uniformly measure the behavior of many AI Systems.
 Home-page: https://github.com/mlcommons/modelgauge
 License: Apache-2.0
 Keywords: AI,GenAI,LLM,NLP,evaluate,measure,quality,testing,prompt,safety,compare,artificial,intelligence,Large,Language,Models
 Author: MLCommons AI Safety
 Author-email: ai-safety-engineering@mlcommons.org
 Requires-Python: >=3.10,<4.0
```

