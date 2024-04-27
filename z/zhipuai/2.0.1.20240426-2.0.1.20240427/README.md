# Comparing `tmp/zhipuai-2.0.1.20240426.tar.gz` & `tmp/zhipuai-2.0.1.20240427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhipuai-2.0.1.20240426.tar", max compression
+gzip compressed data, was "zhipuai-2.0.1.20240427.tar", max compression
```

## Comparing `zhipuai-2.0.1.20240426.tar` & `zhipuai-2.0.1.20240427.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     7371 2024-04-26 09:31:24.262524 zhipuai-2.0.1.20240426/README.md
--rw-r--r--   0        0        0     2979 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/pyproject.toml
--rw-r--r--   0        0        0      343 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/__init__.py
--rw-r--r--   0        0        0       23 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/__version__.py
--rw-r--r--   0        0        0    13562 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/_base_models.py
--rw-r--r--   0        0        0     2431 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/_client.py
--rw-r--r--   0        0        0      147 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/api_resource/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/api_resource/chat/__init__.py
--rw-r--r--   0        0        0     3230 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/api_resource/chat/async_completions.py
--rw-r--r--   0        0        0      451 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/api_resource/chat/chat.py
--rw-r--r--   0        0        0     4561 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/api_resource/chat/completions.py
--rw-r--r--   0        0        0     1694 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/api_resource/embeddings.py
--rw-r--r--   0        0        0     2463 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/api_resource/files.py
--rw-r--r--   0        0        0        0 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/api_resource/fine_tuning/__init__.py
--rw-r--r--   0        0        0      311 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/api_resource/fine_tuning/fine_tuning.py
--rw-r--r--   0        0        0     3757 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/api_resource/fine_tuning/jobs.py
--rw-r--r--   0        0        0     1885 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/api_resource/images.py
--rw-r--r--   0        0        0        0 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/__init__.py
--rw-r--r--   0        0        0      406 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_base_api.py
--rw-r--r--   0        0        0     6405 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_base_compat.py
--rw-r--r--   0        0        0     4484 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_base_type.py
--rw-r--r--   0        0        0     2038 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_errors.py
--rw-r--r--   0        0        0     1384 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_files.py
--rw-r--r--   0        0        0    13808 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_http_client.py
--rw-r--r--   0        0        0      713 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_jwt_token.py
--rw-r--r--   0        0        0     2346 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_request_opt.py
--rw-r--r--   0        0        0     3640 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_response.py
--rw-r--r--   0        0        0     4085 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_sse_client.py
--rw-r--r--   0        0        0     1451 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_utils/__init__.py
--rw-r--r--   0        0        0     3858 2024-04-26 09:31:24.266523 zhipuai-2.0.1.20240426/zhipuai/core/_utils/_typing.py
--rw-r--r--   0        0        0    11363 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/core/_utils/_utils.py
--rw-r--r--   0        0        0        0 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/chat/__init__.py
--rw-r--r--   0        0        0      557 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/chat/async_chat_completion.py
--rw-r--r--   0        0        0      885 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/chat/chat_completion.py
--rw-r--r--   0        0        0     1257 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      171 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/chat/chat_completions_create_param.py
--rw-r--r--   0        0        0      434 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/embeddings.py
--rw-r--r--   0        0        0      538 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/file_object.py
--rw-r--r--   0        0        0      244 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/fine_tuning/__init__.py
--rw-r--r--   0        0        0     1113 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0        0        0     1110 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0        0        0      339 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/fine_tuning/job_create_params.py
--rw-r--r--   0        0        0      382 2024-04-26 09:31:24.270523 zhipuai-2.0.1.20240426/zhipuai/types/image.py
--rw-r--r--   0        0        0     8067 1970-01-01 00:00:00.000000 zhipuai-2.0.1.20240426/PKG-INFO
+-rw-r--r--   0        0        0     7371 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/README.md
+-rw-r--r--   0        0        0     2979 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/pyproject.toml
+-rw-r--r--   0        0        0      343 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/__version__.py
+-rw-r--r--   0        0        0    13562 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/_base_models.py
+-rw-r--r--   0        0        0     2431 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/_client.py
+-rw-r--r--   0        0        0      147 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/__init__.py
+-rw-r--r--   0        0        0     3230 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/async_completions.py
+-rw-r--r--   0        0        0      451 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/chat.py
+-rw-r--r--   0        0        0     4789 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/completions.py
+-rw-r--r--   0        0        0     1694 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/embeddings.py
+-rw-r--r--   0        0        0     2463 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/files.py
+-rw-r--r--   0        0        0        0 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/fine_tuning/__init__.py
+-rw-r--r--   0        0        0      311 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/fine_tuning/fine_tuning.py
+-rw-r--r--   0        0        0     3757 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/fine_tuning/jobs.py
+-rw-r--r--   0        0        0     1885 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/images.py
+-rw-r--r--   0        0        0        0 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/core/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_base_api.py
+-rw-r--r--   0        0        0     6405 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_base_compat.py
+-rw-r--r--   0        0        0     4484 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_base_type.py
+-rw-r--r--   0        0        0     2038 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_errors.py
+-rw-r--r--   0        0        0     1384 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_files.py
+-rw-r--r--   0        0        0    13808 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_http_client.py
+-rw-r--r--   0        0        0      713 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_jwt_token.py
+-rw-r--r--   0        0        0     2346 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_request_opt.py
+-rw-r--r--   0        0        0     3640 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_response.py
+-rw-r--r--   0        0        0     4085 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_sse_client.py
+-rw-r--r--   0        0        0     1451 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_utils/__init__.py
+-rw-r--r--   0        0        0     3858 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_utils/_typing.py
+-rw-r--r--   0        0        0    11363 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_utils/_utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/chat/__init__.py
+-rw-r--r--   0        0        0      557 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/chat/async_chat_completion.py
+-rw-r--r--   0        0        0      885 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/chat/chat_completion.py
+-rw-r--r--   0        0        0     1257 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      171 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/chat/chat_completions_create_param.py
+-rw-r--r--   0        0        0      434 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/embeddings.py
+-rw-r--r--   0        0        0      538 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/file_object.py
+-rw-r--r--   0        0        0      244 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/__init__.py
+-rw-r--r--   0        0        0     1113 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/fine_tuning_job.py
+-rw-r--r--   0        0        0     1110 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/fine_tuning_job_event.py
+-rw-r--r--   0        0        0      339 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/job_create_params.py
+-rw-r--r--   0        0        0      382 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/image.py
+-rw-r--r--   0        0        0     8067 1970-01-01 00:00:00.000000 zhipuai-2.0.1.20240427/PKG-INFO
```

### Comparing `zhipuai-2.0.1.20240426/README.md` & `zhipuai-2.0.1.20240427/README.md`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/pyproject.toml` & `zhipuai-2.0.1.20240427/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zhipuai"
-version = "2.0.1.20240426"
+version = "2.0.1.20240427"
 description = "A SDK library for accessing big model apis from ZhipuAI"
 authors = ["Zhipu AI"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12,!=3.9.7"
 httpx = ">=0.23.0"
```

### Comparing `zhipuai-2.0.1.20240426/zhipuai/_base_models.py` & `zhipuai-2.0.1.20240427/zhipuai/_base_models.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/_client.py` & `zhipuai-2.0.1.20240427/zhipuai/_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/api_resource/chat/async_completions.py` & `zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/async_completions.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/api_resource/chat/completions.py` & `zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/completions.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,33 +46,37 @@
     ) -> Completion | StreamResponse[ChatCompletionChunk]:
         _cast_type = Completion
         _stream_cls = StreamResponse[ChatCompletionChunk]
         if disable_strict_validation:
             _cast_type = object
             _stream_cls = StreamResponse[object]
 
-        if temperature:
+        print(f"temperature:{temperature}")
+        print(f"top_p:{top_p}")
+        if temperature is not None and temperature != NOT_GIVEN:
 
             if temperature <= 0:
                 do_sample = False
                 temperature = 0.01
                 logger.warning("取值范围是：(0.0, 1.0) 开区间，do_sample重写为:false（参数top_p temperture不生效）")
             if temperature >= 1:
                 do_sample = False
                 temperature = 0.99
                 logger.warning("取值范围是：(0.0, 1.0) 开区间，do_sample重写为:false（参数top_p temperture不生效）")
-        if top_p:
+        if top_p is not None and top_p != NOT_GIVEN:
 
             if top_p >= 1:
                 top_p = 0.99
                 logger.warning("取值范围是：(0.0, 1.0) 开区间，不能等于 0 或 1")
             if top_p <= 0:
                 top_p = 0.01
                 logger.warning("取值范围是：(0.0, 1.0) 开区间，不能等于 0 或 1")
 
+        print(f"temperature:{temperature}")
+        print(f"top_p:{top_p}")
         if isinstance(messages, List):
             for item in messages:
                 if item.get('content'):
                     item['content'] = self._drop_prefix_image_data(item['content'])
 
         return self._post(
             "/chat/completions",
```

### Comparing `zhipuai-2.0.1.20240426/zhipuai/api_resource/embeddings.py` & `zhipuai-2.0.1.20240427/zhipuai/api_resource/embeddings.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/api_resource/files.py` & `zhipuai-2.0.1.20240427/zhipuai/api_resource/files.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/api_resource/fine_tuning/jobs.py` & `zhipuai-2.0.1.20240427/zhipuai/api_resource/fine_tuning/jobs.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/api_resource/images.py` & `zhipuai-2.0.1.20240427/zhipuai/api_resource/images.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_base_compat.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_base_compat.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_base_type.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_base_type.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_errors.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_errors.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_files.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_files.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_http_client.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_http_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_jwt_token.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_jwt_token.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_request_opt.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_request_opt.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_response.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_response.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_sse_client.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_sse_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_utils/__init__.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_utils/_typing.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/core/_utils/_utils.py` & `zhipuai-2.0.1.20240427/zhipuai/core/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/types/chat/async_chat_completion.py` & `zhipuai-2.0.1.20240427/zhipuai/types/chat/async_chat_completion.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/types/chat/chat_completion.py` & `zhipuai-2.0.1.20240427/zhipuai/types/chat/chat_completion.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/types/chat/chat_completion_chunk.py` & `zhipuai-2.0.1.20240427/zhipuai/types/chat/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/types/file_object.py` & `zhipuai-2.0.1.20240427/zhipuai/types/file_object.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/types/fine_tuning/fine_tuning_job.py` & `zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/zhipuai/types/fine_tuning/fine_tuning_job_event.py` & `zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/fine_tuning_job_event.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240426/PKG-INFO` & `zhipuai-2.0.1.20240427/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhipuai
-Version: 2.0.1.20240426
+Version: 2.0.1.20240427
 Summary: A SDK library for accessing big model apis from ZhipuAI
 Author: Zhipu AI
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.12.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

