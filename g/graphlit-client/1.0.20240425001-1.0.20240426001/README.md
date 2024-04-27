# Comparing `tmp/graphlit_client-1.0.20240425001.tar.gz` & `tmp/graphlit_client-1.0.20240426001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-1.0.20240425001.tar", last modified: Thu Apr 25 21:56:52 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240426001.tar", last modified: Fri Apr 26 21:24:33 2024, max compression
```

## Comparing `graphlit_client-1.0.20240425001.tar` & `graphlit_client-1.0.20240426001.tar`

### file list

```diff
@@ -1,99 +1,156 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 21:56:52.549811 graphlit_client-1.0.20240425001/
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-25 21:56:52.549811 graphlit_client-1.0.20240425001/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 21:56:52.529810 graphlit_client-1.0.20240425001/graphlit/
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit/graphlit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 21:56:52.541811 graphlit_client-1.0.20240425001/graphlit_api/
--rw-r--r--   0 vsts      (1001) docker     (127)    59846 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/add_contents_to_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/async_base_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/base_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/clear_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44094 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/close_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/create_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/create_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/create_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/create_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/create_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/create_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_all_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_all_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_all_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_all_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_all_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_all_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/delete_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/disable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/disable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/enable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/enable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16949 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/extract_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/get_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/get_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7261 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/get_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/get_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/get_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/get_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4502 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/get_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/get_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/ingest_encoded_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/ingest_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/ingest_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)    69307 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/input_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/is_content_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/is_feed_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/lookup_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/lookup_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40591 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3256 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/prompt_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/prompt_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/publish_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/publish_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      750 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/publish_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/query_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/query_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/query_content_facets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8887 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/query_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/query_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/query_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4953 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/query_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/query_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/remove_contents_from_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/suggest_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/summarize_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/update_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/update_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/update_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/update_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/update_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/update_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/update_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/update_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/graphlit_api/usage.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 21:56:52.549811 graphlit_client-1.0.20240425001/graphlit_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-25 21:56:52.000000 graphlit_client-1.0.20240425001/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2899 2024-04-25 21:56:52.000000 graphlit_client-1.0.20240425001/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-25 21:56:52.000000 graphlit_client-1.0.20240425001/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-25 21:56:52.000000 graphlit_client-1.0.20240425001/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-25 21:56:52.000000 graphlit_client-1.0.20240425001/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-25 21:56:52.549811 graphlit_client-1.0.20240425001/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-25 21:56:37.000000 graphlit_client-1.0.20240425001/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 21:24:33.849019 graphlit_client-1.0.20240426001/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-26 21:24:33.849019 graphlit_client-1.0.20240426001/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 21:24:33.809019 graphlit_client-1.0.20240426001/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 21:24:33.849019 graphlit_client-1.0.20240426001/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    70176 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    72202 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      749 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_all_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16975 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      291 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7261 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      580 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      270 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      804 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      593 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      715 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4502 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/get_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    69307 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50785 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3256 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      750 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/publish_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_content_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8887 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      740 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1006 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      759 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      887 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      592 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      727 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4953 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      749 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/update_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/graphlit_api/usage.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 21:24:33.849019 graphlit_client-1.0.20240426001/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-26 21:24:33.000000 graphlit_client-1.0.20240426001/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     4643 2024-04-26 21:24:33.000000 graphlit_client-1.0.20240426001/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-26 21:24:33.000000 graphlit_client-1.0.20240426001/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-26 21:24:33.000000 graphlit_client-1.0.20240426001/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-26 21:24:33.000000 graphlit_client-1.0.20240426001/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-26 21:24:33.849019 graphlit_client-1.0.20240426001/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-26 21:24:19.000000 graphlit_client-1.0.20240426001/setup.py
```

### Comparing `graphlit_client-1.0.20240425001/LICENSE` & `graphlit_client-1.0.20240426001/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/PKG-INFO` & `graphlit_client-1.0.20240426001/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240425001
+Version: 1.0.20240426001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240425001/README.md` & `graphlit_client-1.0.20240426001/README.md`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit/graphlit.py` & `graphlit_client-1.0.20240426001/graphlit/graphlit.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/__init__.py` & `graphlit_client-1.0.20240426001/graphlit_api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,20 +7,33 @@
 )
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel, Upload
 from .clear_conversation import ClearConversation, ClearConversationClearConversation
 from .client import Client
 from .close_conversation import CloseConversation, CloseConversationCloseConversation
 from .create_alert import CreateAlert, CreateAlertCreateAlert
+from .create_category import CreateCategory, CreateCategoryCreateCategory
 from .create_collection import CreateCollection, CreateCollectionCreateCollection
 from .create_conversation import (
     CreateConversation,
     CreateConversationCreateConversation,
 )
+from .create_event import CreateEvent, CreateEventCreateEvent
 from .create_feed import CreateFeed, CreateFeedCreateFeed
+from .create_label import CreateLabel, CreateLabelCreateLabel
+from .create_observation import CreateObservation, CreateObservationCreateObservation
+from .create_organization import (
+    CreateOrganization,
+    CreateOrganizationCreateOrganization,
+)
+from .create_person import CreatePerson, CreatePersonCreatePerson
+from .create_place import CreatePlace, CreatePlaceCreatePlace
+from .create_product import CreateProduct, CreateProductCreateProduct
+from .create_repo import CreateRepo, CreateRepoCreateRepo
+from .create_software import CreateSoftware, CreateSoftwareCreateSoftware
 from .create_specification import (
     CreateSpecification,
     CreateSpecificationCreateSpecification,
 )
 from .create_workflow import (
     CreateWorkflow,
     CreateWorkflowCreateWorkflow,
@@ -66,28 +79,53 @@
     DeleteAllConversationsDeleteAllConversations,
 )
 from .delete_all_feeds import DeleteAllFeeds, DeleteAllFeedsDeleteAllFeeds
 from .delete_all_workflows import (
     DeleteAllWorkflows,
     DeleteAllWorkflowsDeleteAllWorkflows,
 )
+from .delete_categories import DeleteCategories, DeleteCategoriesDeleteCategories
+from .delete_category import DeleteCategory, DeleteCategoryDeleteCategory
 from .delete_collection import DeleteCollection, DeleteCollectionDeleteCollection
 from .delete_collections import DeleteCollections, DeleteCollectionsDeleteCollections
 from .delete_content import DeleteContent, DeleteContentDeleteContent
 from .delete_contents import DeleteContents, DeleteContentsDeleteContents
 from .delete_conversation import (
     DeleteConversation,
     DeleteConversationDeleteConversation,
 )
 from .delete_conversations import (
     DeleteConversations,
     DeleteConversationsDeleteConversations,
 )
+from .delete_event import DeleteEvent, DeleteEventDeleteEvent
+from .delete_events import DeleteEvents, DeleteEventsDeleteEvents
 from .delete_feed import DeleteFeed, DeleteFeedDeleteFeed
 from .delete_feeds import DeleteFeeds, DeleteFeedsDeleteFeeds
+from .delete_label import DeleteLabel, DeleteLabelDeleteLabel
+from .delete_labels import DeleteLabels, DeleteLabelsDeleteLabels
+from .delete_observation import DeleteObservation, DeleteObservationDeleteObservation
+from .delete_organization import (
+    DeleteOrganization,
+    DeleteOrganizationDeleteOrganization,
+)
+from .delete_organizations import (
+    DeleteOrganizations,
+    DeleteOrganizationsDeleteOrganizations,
+)
+from .delete_person import DeletePerson, DeletePersonDeletePerson
+from .delete_persons import DeletePersons, DeletePersonsDeletePersons
+from .delete_place import DeletePlace, DeletePlaceDeletePlace
+from .delete_places import DeletePlaces, DeletePlacesDeletePlaces
+from .delete_product import DeleteProduct, DeleteProductDeleteProduct
+from .delete_products import DeleteProducts, DeleteProductsDeleteProducts
+from .delete_repo import DeleteRepo, DeleteRepoDeleteRepo
+from .delete_repos import DeleteRepos, DeleteReposDeleteRepos
+from .delete_software import DeleteSoftware, DeleteSoftwareDeleteSoftware
+from .delete_softwares import DeleteSoftwares, DeleteSoftwaresDeleteSoftwares
 from .delete_specification import (
     DeleteSpecification,
     DeleteSpecificationDeleteSpecification,
 )
 from .delete_workflow import DeleteWorkflow, DeleteWorkflowDeleteWorkflow
 from .delete_workflows import DeleteWorkflows, DeleteWorkflowsDeleteWorkflows
 from .disable_alert import DisableAlert, DisableAlertDisableAlert
@@ -204,14 +242,15 @@
     GetAlertAlertIntegrationSlack,
     GetAlertAlertOwner,
     GetAlertAlertPublishing,
     GetAlertAlertPublishingElevenLabs,
     GetAlertAlertPublishSpecification,
     GetAlertAlertSummarySpecification,
 )
+from .get_category import GetCategory, GetCategoryCategory
 from .get_collection import (
     GetCollection,
     GetCollectionCollection,
     GetCollectionCollectionContents,
     GetCollectionCollectionOwner,
 )
 from .get_content import (
@@ -253,14 +292,15 @@
     GetConversationConversationFilterWorkflows,
     GetConversationConversationMessages,
     GetConversationConversationMessagesCitations,
     GetConversationConversationMessagesCitationsContent,
     GetConversationConversationOwner,
     GetConversationConversationSpecification,
 )
+from .get_event import GetEvent, GetEventEvent
 from .get_feed import (
     GetFeed,
     GetFeedFeed,
     GetFeedFeedDiscord,
     GetFeedFeedEmail,
     GetFeedFeedEmailGoogle,
     GetFeedFeedEmailMicrosoft,
@@ -282,21 +322,28 @@
     GetFeedFeedSiteS3,
     GetFeedFeedSiteSharePoint,
     GetFeedFeedSlack,
     GetFeedFeedWeb,
     GetFeedFeedWorkflow,
     GetFeedFeedYoutube,
 )
+from .get_label import GetLabel, GetLabelLabel
+from .get_organization import GetOrganization, GetOrganizationOrganization
+from .get_person import GetPerson, GetPersonPerson
+from .get_place import GetPlace, GetPlacePlace
+from .get_product import GetProduct, GetProductProduct
 from .get_project import (
     GetProject,
     GetProjectProject,
     GetProjectProjectQuota,
     GetProjectProjectSpecification,
     GetProjectProjectWorkflow,
 )
+from .get_repo import GetRepo, GetRepoRepo
+from .get_software import GetSoftware, GetSoftwareSoftware
 from .get_specification import (
     GetSpecification,
     GetSpecificationSpecification,
     GetSpecificationSpecificationAnthropic,
     GetSpecificationSpecificationAzureOpenAi,
     GetSpecificationSpecificationOpenAi,
     GetSpecificationSpecificationOwner,
@@ -532,50 +579,88 @@
 from .lookup_credits import LookupCredits, LookupCreditsLookupCredits
 from .lookup_usage import LookupUsage, LookupUsageLookupUsage
 from .operations import (
     ADD_CONTENTS_TO_COLLECTIONS_GQL,
     CLEAR_CONVERSATION_GQL,
     CLOSE_CONVERSATION_GQL,
     CREATE_ALERT_GQL,
+    CREATE_CATEGORY_GQL,
     CREATE_COLLECTION_GQL,
     CREATE_CONVERSATION_GQL,
+    CREATE_EVENT_GQL,
     CREATE_FEED_GQL,
+    CREATE_LABEL_GQL,
+    CREATE_OBSERVATION_GQL,
+    CREATE_ORGANIZATION_GQL,
+    CREATE_PERSON_GQL,
+    CREATE_PLACE_GQL,
+    CREATE_PRODUCT_GQL,
+    CREATE_REPO_GQL,
+    CREATE_SOFTWARE_GQL,
     CREATE_SPECIFICATION_GQL,
     CREATE_WORKFLOW_GQL,
     CREDITS_GQL,
     DELETE_ALERT_GQL,
     DELETE_ALERTS_GQL,
     DELETE_ALL_ALERTS_GQL,
     DELETE_ALL_COLLECTIONS_GQL,
     DELETE_ALL_CONTENTS_GQL,
     DELETE_ALL_CONVERSATIONS_GQL,
     DELETE_ALL_FEEDS_GQL,
     DELETE_ALL_WORKFLOWS_GQL,
+    DELETE_CATEGORIES_GQL,
+    DELETE_CATEGORY_GQL,
     DELETE_COLLECTION_GQL,
     DELETE_COLLECTIONS_GQL,
     DELETE_CONTENT_GQL,
     DELETE_CONTENTS_GQL,
     DELETE_CONVERSATION_GQL,
     DELETE_CONVERSATIONS_GQL,
+    DELETE_EVENT_GQL,
+    DELETE_EVENTS_GQL,
     DELETE_FEED_GQL,
     DELETE_FEEDS_GQL,
+    DELETE_LABEL_GQL,
+    DELETE_LABELS_GQL,
+    DELETE_OBSERVATION_GQL,
+    DELETE_ORGANIZATION_GQL,
+    DELETE_ORGANIZATIONS_GQL,
+    DELETE_PERSON_GQL,
+    DELETE_PERSONS_GQL,
+    DELETE_PLACE_GQL,
+    DELETE_PLACES_GQL,
+    DELETE_PRODUCT_GQL,
+    DELETE_PRODUCTS_GQL,
+    DELETE_REPO_GQL,
+    DELETE_REPOS_GQL,
+    DELETE_SOFTWARE_GQL,
+    DELETE_SOFTWARES_GQL,
     DELETE_SPECIFICATION_GQL,
     DELETE_WORKFLOW_GQL,
     DELETE_WORKFLOWS_GQL,
     DISABLE_ALERT_GQL,
     DISABLE_FEED_GQL,
     ENABLE_ALERT_GQL,
     ENABLE_FEED_GQL,
     EXTRACT_CONTENTS_GQL,
     GET_ALERT_GQL,
+    GET_CATEGORY_GQL,
     GET_COLLECTION_GQL,
     GET_CONTENT_GQL,
     GET_CONVERSATION_GQL,
+    GET_EVENT_GQL,
     GET_FEED_GQL,
+    GET_LABEL_GQL,
+    GET_ORGANIZATION_GQL,
+    GET_PERSON_GQL,
+    GET_PLACE_GQL,
+    GET_PRODUCT_GQL,
     GET_PROJECT_GQL,
+    GET_REPO_GQL,
+    GET_SOFTWARE_GQL,
     GET_SPECIFICATION_GQL,
     GET_WORKFLOW_GQL,
     INGEST_ENCODED_FILE_GQL,
     INGEST_TEXT_GQL,
     INGEST_URI_GQL,
     IS_CONTENT_DONE_GQL,
     IS_FEED_DONE_GQL,
@@ -583,30 +668,49 @@
     LOOKUP_USAGE_GQL,
     PROMPT_CONVERSATION_GQL,
     PROMPT_SPECIFICATIONS_GQL,
     PUBLISH_CONTENTS_GQL,
     PUBLISH_CONVERSATION_GQL,
     PUBLISH_TEXT_GQL,
     QUERY_ALERTS_GQL,
+    QUERY_CATEGORIES_GQL,
     QUERY_COLLECTIONS_GQL,
     QUERY_CONTENT_FACETS_GQL,
     QUERY_CONTENTS_GQL,
     QUERY_CONVERSATIONS_GQL,
+    QUERY_EVENTS_GQL,
     QUERY_FEEDS_GQL,
+    QUERY_LABELS_GQL,
+    QUERY_ORGANIZATIONS_GQL,
+    QUERY_PERSONS_GQL,
+    QUERY_PLACES_GQL,
+    QUERY_PRODUCTS_GQL,
+    QUERY_REPOS_GQL,
+    QUERY_SOFTWARE_GQL,
     QUERY_SPECIFICATIONS_GQL,
     QUERY_WORKFLOWS_GQL,
     REMOVE_CONTENTS_FROM_COLLECTION_GQL,
     SUGGEST_CONVERSATION_GQL,
     SUMMARIZE_CONTENTS_GQL,
     UPDATE_ALERT_GQL,
+    UPDATE_CATEGORY_GQL,
     UPDATE_COLLECTION_GQL,
     UPDATE_CONTENT_GQL,
     UPDATE_CONVERSATION_GQL,
+    UPDATE_EVENT_GQL,
     UPDATE_FEED_GQL,
+    UPDATE_LABEL_GQL,
+    UPDATE_OBSERVATION_GQL,
+    UPDATE_ORGANIZATION_GQL,
+    UPDATE_PERSON_GQL,
+    UPDATE_PLACE_GQL,
+    UPDATE_PRODUCT_GQL,
     UPDATE_PROJECT_GQL,
+    UPDATE_REPO_GQL,
+    UPDATE_SOFTWARE_GQL,
     UPDATE_SPECIFICATION_GQL,
     UPDATE_WORKFLOW_GQL,
     USAGE_GQL,
 )
 from .prompt_conversation import (
     PromptConversation,
     PromptConversationPromptConversation,
@@ -650,14 +754,19 @@
     QueryAlertsAlertsResultsIntegrationSlack,
     QueryAlertsAlertsResultsOwner,
     QueryAlertsAlertsResultsPublishing,
     QueryAlertsAlertsResultsPublishingElevenLabs,
     QueryAlertsAlertsResultsPublishSpecification,
     QueryAlertsAlertsResultsSummarySpecification,
 )
+from .query_categories import (
+    QueryCategories,
+    QueryCategoriesCategories,
+    QueryCategoriesCategoriesResults,
+)
 from .query_collections import (
     QueryCollections,
     QueryCollectionsCollections,
     QueryCollectionsCollectionsResults,
     QueryCollectionsCollectionsResultsContents,
     QueryCollectionsCollectionsResultsOwner,
 )
@@ -712,14 +821,15 @@
     QueryConversationsConversationsResultsFilterWorkflows,
     QueryConversationsConversationsResultsMessages,
     QueryConversationsConversationsResultsMessagesCitations,
     QueryConversationsConversationsResultsMessagesCitationsContent,
     QueryConversationsConversationsResultsOwner,
     QueryConversationsConversationsResultsSpecification,
 )
+from .query_events import QueryEvents, QueryEventsEvents, QueryEventsEventsResults
 from .query_feeds import (
     QueryFeeds,
     QueryFeedsFeeds,
     QueryFeedsFeedsResults,
     QueryFeedsFeedsResultsDiscord,
     QueryFeedsFeedsResultsEmail,
     QueryFeedsFeedsResultsEmailGoogle,
@@ -742,14 +852,33 @@
     QueryFeedsFeedsResultsSiteS3,
     QueryFeedsFeedsResultsSiteSharePoint,
     QueryFeedsFeedsResultsSlack,
     QueryFeedsFeedsResultsWeb,
     QueryFeedsFeedsResultsWorkflow,
     QueryFeedsFeedsResultsYoutube,
 )
+from .query_labels import QueryLabels, QueryLabelsLabels, QueryLabelsLabelsResults
+from .query_organizations import (
+    QueryOrganizations,
+    QueryOrganizationsOrganizations,
+    QueryOrganizationsOrganizationsResults,
+)
+from .query_persons import QueryPersons, QueryPersonsPersons, QueryPersonsPersonsResults
+from .query_places import QueryPlaces, QueryPlacesPlaces, QueryPlacesPlacesResults
+from .query_products import (
+    QueryProducts,
+    QueryProductsProducts,
+    QueryProductsProductsResults,
+)
+from .query_repos import QueryRepos, QueryReposRepos, QueryReposReposResults
+from .query_software import (
+    QuerySoftware,
+    QuerySoftwareSoftwares,
+    QuerySoftwareSoftwaresResults,
+)
 from .query_specifications import (
     QuerySpecifications,
     QuerySpecificationsSpecifications,
     QuerySpecificationsSpecificationsResults,
     QuerySpecificationsSpecificationsResultsAnthropic,
     QuerySpecificationsSpecificationsResultsAzureOpenAi,
     QuerySpecificationsSpecificationsResultsOpenAi,
@@ -807,22 +936,35 @@
     SummarizeContents,
     SummarizeContentsSummarizeContents,
     SummarizeContentsSummarizeContentsContent,
     SummarizeContentsSummarizeContentsItems,
     SummarizeContentsSummarizeContentsSpecification,
 )
 from .update_alert import UpdateAlert, UpdateAlertUpdateAlert
+from .update_category import UpdateCategory, UpdateCategoryUpdateCategory
 from .update_collection import UpdateCollection, UpdateCollectionUpdateCollection
 from .update_content import UpdateContent, UpdateContentUpdateContent
 from .update_conversation import (
     UpdateConversation,
     UpdateConversationUpdateConversation,
 )
+from .update_event import UpdateEvent, UpdateEventUpdateEvent
 from .update_feed import UpdateFeed, UpdateFeedUpdateFeed
+from .update_label import UpdateLabel, UpdateLabelUpdateLabel
+from .update_observation import UpdateObservation, UpdateObservationUpdateObservation
+from .update_organization import (
+    UpdateOrganization,
+    UpdateOrganizationUpdateOrganization,
+)
+from .update_person import UpdatePerson, UpdatePersonUpdatePerson
+from .update_place import UpdatePlace, UpdatePlaceUpdatePlace
+from .update_product import UpdateProduct, UpdateProductUpdateProduct
 from .update_project import UpdateProject, UpdateProjectUpdateProject
+from .update_repo import UpdateRepo, UpdateRepoUpdateRepo
+from .update_software import UpdateSoftware, UpdateSoftwareUpdateSoftware
 from .update_specification import (
     UpdateSpecification,
     UpdateSpecificationUpdateSpecification,
 )
 from .update_workflow import (
     UpdateWorkflow,
     UpdateWorkflowUpdateWorkflow,
@@ -890,17 +1032,27 @@
     "AzureTextExtractionPropertiesInput",
     "BaseModel",
     "BillableMetrics",
     "BoundingBoxInput",
     "CLEAR_CONVERSATION_GQL",
     "CLOSE_CONVERSATION_GQL",
     "CREATE_ALERT_GQL",
+    "CREATE_CATEGORY_GQL",
     "CREATE_COLLECTION_GQL",
     "CREATE_CONVERSATION_GQL",
+    "CREATE_EVENT_GQL",
     "CREATE_FEED_GQL",
+    "CREATE_LABEL_GQL",
+    "CREATE_OBSERVATION_GQL",
+    "CREATE_ORGANIZATION_GQL",
+    "CREATE_PERSON_GQL",
+    "CREATE_PLACE_GQL",
+    "CREATE_PRODUCT_GQL",
+    "CREATE_REPO_GQL",
+    "CREATE_SOFTWARE_GQL",
     "CREATE_SPECIFICATION_GQL",
     "CREATE_WORKFLOW_GQL",
     "CREDITS_GQL",
     "CategoryFacetInput",
     "CategoryFacetTypes",
     "CategoryFilter",
     "CategoryInput",
@@ -935,20 +1087,40 @@
     "ConversationStrategyInput",
     "ConversationStrategyTypes",
     "ConversationStrategyUpdateInput",
     "ConversationTypes",
     "ConversationUpdateInput",
     "CreateAlert",
     "CreateAlertCreateAlert",
+    "CreateCategory",
+    "CreateCategoryCreateCategory",
     "CreateCollection",
     "CreateCollectionCreateCollection",
     "CreateConversation",
     "CreateConversationCreateConversation",
+    "CreateEvent",
+    "CreateEventCreateEvent",
     "CreateFeed",
     "CreateFeedCreateFeed",
+    "CreateLabel",
+    "CreateLabelCreateLabel",
+    "CreateObservation",
+    "CreateObservationCreateObservation",
+    "CreateOrganization",
+    "CreateOrganizationCreateOrganization",
+    "CreatePerson",
+    "CreatePersonCreatePerson",
+    "CreatePlace",
+    "CreatePlaceCreatePlace",
+    "CreateProduct",
+    "CreateProductCreateProduct",
+    "CreateRepo",
+    "CreateRepoCreateRepo",
+    "CreateSoftware",
+    "CreateSoftwareCreateSoftware",
     "CreateSpecification",
     "CreateSpecificationCreateSpecification",
     "CreateWorkflow",
     "CreateWorkflowCreateWorkflow",
     "CreateWorkflowCreateWorkflowActions",
     "CreateWorkflowCreateWorkflowActionsConnector",
     "CreateWorkflowCreateWorkflowActionsConnectorSlack",
@@ -982,22 +1154,41 @@
     "DELETE_ALERT_GQL",
     "DELETE_ALL_ALERTS_GQL",
     "DELETE_ALL_COLLECTIONS_GQL",
     "DELETE_ALL_CONTENTS_GQL",
     "DELETE_ALL_CONVERSATIONS_GQL",
     "DELETE_ALL_FEEDS_GQL",
     "DELETE_ALL_WORKFLOWS_GQL",
+    "DELETE_CATEGORIES_GQL",
+    "DELETE_CATEGORY_GQL",
     "DELETE_COLLECTIONS_GQL",
     "DELETE_COLLECTION_GQL",
     "DELETE_CONTENTS_GQL",
     "DELETE_CONTENT_GQL",
     "DELETE_CONVERSATIONS_GQL",
     "DELETE_CONVERSATION_GQL",
+    "DELETE_EVENTS_GQL",
+    "DELETE_EVENT_GQL",
     "DELETE_FEEDS_GQL",
     "DELETE_FEED_GQL",
+    "DELETE_LABELS_GQL",
+    "DELETE_LABEL_GQL",
+    "DELETE_OBSERVATION_GQL",
+    "DELETE_ORGANIZATIONS_GQL",
+    "DELETE_ORGANIZATION_GQL",
+    "DELETE_PERSONS_GQL",
+    "DELETE_PERSON_GQL",
+    "DELETE_PLACES_GQL",
+    "DELETE_PLACE_GQL",
+    "DELETE_PRODUCTS_GQL",
+    "DELETE_PRODUCT_GQL",
+    "DELETE_REPOS_GQL",
+    "DELETE_REPO_GQL",
+    "DELETE_SOFTWARES_GQL",
+    "DELETE_SOFTWARE_GQL",
     "DELETE_SPECIFICATION_GQL",
     "DELETE_WORKFLOWS_GQL",
     "DELETE_WORKFLOW_GQL",
     "DISABLE_ALERT_GQL",
     "DISABLE_FEED_GQL",
     "DateRangeFilter",
     "DateRangeInput",
@@ -1015,30 +1206,68 @@
     "DeleteAllContentsDeleteAllContents",
     "DeleteAllConversations",
     "DeleteAllConversationsDeleteAllConversations",
     "DeleteAllFeeds",
     "DeleteAllFeedsDeleteAllFeeds",
     "DeleteAllWorkflows",
     "DeleteAllWorkflowsDeleteAllWorkflows",
+    "DeleteCategories",
+    "DeleteCategoriesDeleteCategories",
+    "DeleteCategory",
+    "DeleteCategoryDeleteCategory",
     "DeleteCollection",
     "DeleteCollectionDeleteCollection",
     "DeleteCollections",
     "DeleteCollectionsDeleteCollections",
     "DeleteContent",
     "DeleteContentDeleteContent",
     "DeleteContents",
     "DeleteContentsDeleteContents",
     "DeleteConversation",
     "DeleteConversationDeleteConversation",
     "DeleteConversations",
     "DeleteConversationsDeleteConversations",
+    "DeleteEvent",
+    "DeleteEventDeleteEvent",
+    "DeleteEvents",
+    "DeleteEventsDeleteEvents",
     "DeleteFeed",
     "DeleteFeedDeleteFeed",
     "DeleteFeeds",
     "DeleteFeedsDeleteFeeds",
+    "DeleteLabel",
+    "DeleteLabelDeleteLabel",
+    "DeleteLabels",
+    "DeleteLabelsDeleteLabels",
+    "DeleteObservation",
+    "DeleteObservationDeleteObservation",
+    "DeleteOrganization",
+    "DeleteOrganizationDeleteOrganization",
+    "DeleteOrganizations",
+    "DeleteOrganizationsDeleteOrganizations",
+    "DeletePerson",
+    "DeletePersonDeletePerson",
+    "DeletePersons",
+    "DeletePersonsDeletePersons",
+    "DeletePlace",
+    "DeletePlaceDeletePlace",
+    "DeletePlaces",
+    "DeletePlacesDeletePlaces",
+    "DeleteProduct",
+    "DeleteProductDeleteProduct",
+    "DeleteProducts",
+    "DeleteProductsDeleteProducts",
+    "DeleteRepo",
+    "DeleteRepoDeleteRepo",
+    "DeleteRepos",
+    "DeleteReposDeleteRepos",
+    "DeleteSoftware",
+    "DeleteSoftwareDeleteSoftware",
+    "DeleteSoftwares",
+    "DeleteSoftwaresDeleteSoftwares",
     "DeleteSpecification",
     "DeleteSpecificationDeleteSpecification",
     "DeleteWorkflow",
     "DeleteWorkflowDeleteWorkflow",
     "DeleteWorkflows",
     "DeleteWorkflowsDeleteWorkflows",
     "DeviceTypes",
@@ -1093,19 +1322,28 @@
     "FeedServiceTypes",
     "FeedTypes",
     "FeedUpdateInput",
     "FilePreparationConnectorInput",
     "FilePreparationServiceTypes",
     "FileTypes",
     "GET_ALERT_GQL",
+    "GET_CATEGORY_GQL",
     "GET_COLLECTION_GQL",
     "GET_CONTENT_GQL",
     "GET_CONVERSATION_GQL",
+    "GET_EVENT_GQL",
     "GET_FEED_GQL",
+    "GET_LABEL_GQL",
+    "GET_ORGANIZATION_GQL",
+    "GET_PERSON_GQL",
+    "GET_PLACE_GQL",
+    "GET_PRODUCT_GQL",
     "GET_PROJECT_GQL",
+    "GET_REPO_GQL",
+    "GET_SOFTWARE_GQL",
     "GET_SPECIFICATION_GQL",
     "GET_WORKFLOW_GQL",
     "GetAlert",
     "GetAlertAlert",
     "GetAlertAlertFilter",
     "GetAlertAlertFilterCollections",
     "GetAlertAlertFilterContents",
@@ -1118,14 +1356,16 @@
     "GetAlertAlertIntegration",
     "GetAlertAlertIntegrationSlack",
     "GetAlertAlertOwner",
     "GetAlertAlertPublishSpecification",
     "GetAlertAlertPublishing",
     "GetAlertAlertPublishingElevenLabs",
     "GetAlertAlertSummarySpecification",
+    "GetCategory",
+    "GetCategoryCategory",
     "GetCollection",
     "GetCollectionCollection",
     "GetCollectionCollectionContents",
     "GetCollectionCollectionOwner",
     "GetContent",
     "GetContentContent",
     "GetContentContentAudio",
@@ -1161,14 +1401,16 @@
     "GetConversationConversationFilterObservationsObservable",
     "GetConversationConversationFilterWorkflows",
     "GetConversationConversationMessages",
     "GetConversationConversationMessagesCitations",
     "GetConversationConversationMessagesCitationsContent",
     "GetConversationConversationOwner",
     "GetConversationConversationSpecification",
+    "GetEvent",
+    "GetEventEvent",
     "GetFeed",
     "GetFeedFeed",
     "GetFeedFeedDiscord",
     "GetFeedFeedEmail",
     "GetFeedFeedEmailGoogle",
     "GetFeedFeedEmailMicrosoft",
     "GetFeedFeedIssue",
@@ -1188,19 +1430,33 @@
     "GetFeedFeedSiteOneDrive",
     "GetFeedFeedSiteS3",
     "GetFeedFeedSiteSharePoint",
     "GetFeedFeedSlack",
     "GetFeedFeedWeb",
     "GetFeedFeedWorkflow",
     "GetFeedFeedYoutube",
+    "GetLabel",
+    "GetLabelLabel",
+    "GetOrganization",
+    "GetOrganizationOrganization",
+    "GetPerson",
+    "GetPersonPerson",
+    "GetPlace",
+    "GetPlacePlace",
+    "GetProduct",
+    "GetProductProduct",
     "GetProject",
     "GetProjectProject",
     "GetProjectProjectQuota",
     "GetProjectProjectSpecification",
     "GetProjectProjectWorkflow",
+    "GetRepo",
+    "GetRepoRepo",
+    "GetSoftware",
+    "GetSoftwareSoftware",
     "GetSpecification",
     "GetSpecificationSpecification",
     "GetSpecificationSpecificationAnthropic",
     "GetSpecificationSpecificationAzureOpenAi",
     "GetSpecificationSpecificationOpenAi",
     "GetSpecificationSpecificationOwner",
     "GetSpecificationSpecificationPromptStrategy",
@@ -1388,19 +1644,28 @@
     "PublishContents",
     "PublishContentsPublishContents",
     "PublishConversation",
     "PublishConversationPublishConversation",
     "PublishText",
     "PublishTextPublishText",
     "QUERY_ALERTS_GQL",
+    "QUERY_CATEGORIES_GQL",
     "QUERY_COLLECTIONS_GQL",
     "QUERY_CONTENTS_GQL",
     "QUERY_CONTENT_FACETS_GQL",
     "QUERY_CONVERSATIONS_GQL",
+    "QUERY_EVENTS_GQL",
     "QUERY_FEEDS_GQL",
+    "QUERY_LABELS_GQL",
+    "QUERY_ORGANIZATIONS_GQL",
+    "QUERY_PERSONS_GQL",
+    "QUERY_PLACES_GQL",
+    "QUERY_PRODUCTS_GQL",
+    "QUERY_REPOS_GQL",
+    "QUERY_SOFTWARE_GQL",
     "QUERY_SPECIFICATIONS_GQL",
     "QUERY_WORKFLOWS_GQL",
     "QueryAlerts",
     "QueryAlertsAlerts",
     "QueryAlertsAlertsResults",
     "QueryAlertsAlertsResultsFilter",
     "QueryAlertsAlertsResultsFilterCollections",
@@ -1414,14 +1679,17 @@
     "QueryAlertsAlertsResultsIntegration",
     "QueryAlertsAlertsResultsIntegrationSlack",
     "QueryAlertsAlertsResultsOwner",
     "QueryAlertsAlertsResultsPublishSpecification",
     "QueryAlertsAlertsResultsPublishing",
     "QueryAlertsAlertsResultsPublishingElevenLabs",
     "QueryAlertsAlertsResultsSummarySpecification",
+    "QueryCategories",
+    "QueryCategoriesCategories",
+    "QueryCategoriesCategoriesResults",
     "QueryCollections",
     "QueryCollectionsCollections",
     "QueryCollectionsCollectionsResults",
     "QueryCollectionsCollectionsResultsContents",
     "QueryCollectionsCollectionsResultsOwner",
     "QueryContentFacets",
     "QueryContentFacetsContents",
@@ -1468,14 +1736,17 @@
     "QueryConversationsConversationsResultsFilterObservationsObservable",
     "QueryConversationsConversationsResultsFilterWorkflows",
     "QueryConversationsConversationsResultsMessages",
     "QueryConversationsConversationsResultsMessagesCitations",
     "QueryConversationsConversationsResultsMessagesCitationsContent",
     "QueryConversationsConversationsResultsOwner",
     "QueryConversationsConversationsResultsSpecification",
+    "QueryEvents",
+    "QueryEventsEvents",
+    "QueryEventsEventsResults",
     "QueryFeeds",
     "QueryFeedsFeeds",
     "QueryFeedsFeedsResults",
     "QueryFeedsFeedsResultsDiscord",
     "QueryFeedsFeedsResultsEmail",
     "QueryFeedsFeedsResultsEmailGoogle",
     "QueryFeedsFeedsResultsEmailMicrosoft",
@@ -1496,14 +1767,35 @@
     "QueryFeedsFeedsResultsSiteOneDrive",
     "QueryFeedsFeedsResultsSiteS3",
     "QueryFeedsFeedsResultsSiteSharePoint",
     "QueryFeedsFeedsResultsSlack",
     "QueryFeedsFeedsResultsWeb",
     "QueryFeedsFeedsResultsWorkflow",
     "QueryFeedsFeedsResultsYoutube",
+    "QueryLabels",
+    "QueryLabelsLabels",
+    "QueryLabelsLabelsResults",
+    "QueryOrganizations",
+    "QueryOrganizationsOrganizations",
+    "QueryOrganizationsOrganizationsResults",
+    "QueryPersons",
+    "QueryPersonsPersons",
+    "QueryPersonsPersonsResults",
+    "QueryPlaces",
+    "QueryPlacesPlaces",
+    "QueryPlacesPlacesResults",
+    "QueryProducts",
+    "QueryProductsProducts",
+    "QueryProductsProductsResults",
+    "QueryRepos",
+    "QueryReposRepos",
+    "QueryReposReposResults",
+    "QuerySoftware",
+    "QuerySoftwareSoftwares",
+    "QuerySoftwareSoftwaresResults",
     "QuerySpecifications",
     "QuerySpecificationsSpecifications",
     "QuerySpecificationsSpecificationsResults",
     "QuerySpecificationsSpecificationsResultsAnthropic",
     "QuerySpecificationsSpecificationsResultsAzureOpenAi",
     "QuerySpecificationsSpecificationsResultsOpenAi",
     "QuerySpecificationsSpecificationsResultsOwner",
@@ -1603,35 +1895,65 @@
     "TextRoles",
     "TextTypes",
     "TimeIntervalTypes",
     "TimedPolicyRecurrenceTypes",
     "ToolDefinitionInput",
     "ToolDefinitionUpdateInput",
     "UPDATE_ALERT_GQL",
+    "UPDATE_CATEGORY_GQL",
     "UPDATE_COLLECTION_GQL",
     "UPDATE_CONTENT_GQL",
     "UPDATE_CONVERSATION_GQL",
+    "UPDATE_EVENT_GQL",
     "UPDATE_FEED_GQL",
+    "UPDATE_LABEL_GQL",
+    "UPDATE_OBSERVATION_GQL",
+    "UPDATE_ORGANIZATION_GQL",
+    "UPDATE_PERSON_GQL",
+    "UPDATE_PLACE_GQL",
+    "UPDATE_PRODUCT_GQL",
     "UPDATE_PROJECT_GQL",
+    "UPDATE_REPO_GQL",
+    "UPDATE_SOFTWARE_GQL",
     "UPDATE_SPECIFICATION_GQL",
     "UPDATE_WORKFLOW_GQL",
     "USAGE_GQL",
     "UnitTypes",
     "UpdateAlert",
     "UpdateAlertUpdateAlert",
+    "UpdateCategory",
+    "UpdateCategoryUpdateCategory",
     "UpdateCollection",
     "UpdateCollectionUpdateCollection",
     "UpdateContent",
     "UpdateContentUpdateContent",
     "UpdateConversation",
     "UpdateConversationUpdateConversation",
+    "UpdateEvent",
+    "UpdateEventUpdateEvent",
     "UpdateFeed",
     "UpdateFeedUpdateFeed",
+    "UpdateLabel",
+    "UpdateLabelUpdateLabel",
+    "UpdateObservation",
+    "UpdateObservationUpdateObservation",
+    "UpdateOrganization",
+    "UpdateOrganizationUpdateOrganization",
+    "UpdatePerson",
+    "UpdatePersonUpdatePerson",
+    "UpdatePlace",
+    "UpdatePlaceUpdatePlace",
+    "UpdateProduct",
+    "UpdateProductUpdateProduct",
     "UpdateProject",
     "UpdateProjectUpdateProject",
+    "UpdateRepo",
+    "UpdateRepoUpdateRepo",
+    "UpdateSoftware",
+    "UpdateSoftwareUpdateSoftware",
     "UpdateSpecification",
     "UpdateSpecificationUpdateSpecification",
     "UpdateWorkflow",
     "UpdateWorkflowUpdateWorkflow",
     "UpdateWorkflowUpdateWorkflowActions",
     "UpdateWorkflowUpdateWorkflowActionsConnector",
     "UpdateWorkflowUpdateWorkflowActionsConnectorSlack",
```

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/add_contents_to_collections.py` & `graphlit_client-1.0.20240426001/graphlit_api/add_contents_to_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/async_base_client.py` & `graphlit_client-1.0.20240426001/graphlit_api/async_base_client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/base_model.py` & `graphlit_client-1.0.20240426001/graphlit_api/base_model.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/clear_conversation.py` & `graphlit_client-1.0.20240426001/graphlit_api/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/client.py` & `graphlit_client-1.0.20240426001/graphlit_api/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,75 +5,142 @@
 
 from .add_contents_to_collections import AddContentsToCollections
 from .async_base_client import AsyncBaseClient
 from .base_model import UNSET, UnsetType
 from .clear_conversation import ClearConversation
 from .close_conversation import CloseConversation
 from .create_alert import CreateAlert
+from .create_category import CreateCategory
 from .create_collection import CreateCollection
 from .create_conversation import CreateConversation
+from .create_event import CreateEvent
 from .create_feed import CreateFeed
+from .create_label import CreateLabel
+from .create_observation import CreateObservation
+from .create_organization import CreateOrganization
+from .create_person import CreatePerson
+from .create_place import CreatePlace
+from .create_product import CreateProduct
+from .create_repo import CreateRepo
+from .create_software import CreateSoftware
 from .create_specification import CreateSpecification
 from .create_workflow import CreateWorkflow
 from .credits import Credits
 from .delete_alert import DeleteAlert
 from .delete_alerts import DeleteAlerts
 from .delete_all_alerts import DeleteAllAlerts
 from .delete_all_collections import DeleteAllCollections
 from .delete_all_contents import DeleteAllContents
 from .delete_all_conversations import DeleteAllConversations
 from .delete_all_feeds import DeleteAllFeeds
 from .delete_all_workflows import DeleteAllWorkflows
+from .delete_categories import DeleteCategories
+from .delete_category import DeleteCategory
 from .delete_collection import DeleteCollection
 from .delete_collections import DeleteCollections
 from .delete_content import DeleteContent
 from .delete_contents import DeleteContents
 from .delete_conversation import DeleteConversation
 from .delete_conversations import DeleteConversations
+from .delete_event import DeleteEvent
+from .delete_events import DeleteEvents
 from .delete_feed import DeleteFeed
 from .delete_feeds import DeleteFeeds
+from .delete_label import DeleteLabel
+from .delete_labels import DeleteLabels
+from .delete_observation import DeleteObservation
+from .delete_organization import DeleteOrganization
+from .delete_organizations import DeleteOrganizations
+from .delete_person import DeletePerson
+from .delete_persons import DeletePersons
+from .delete_place import DeletePlace
+from .delete_places import DeletePlaces
+from .delete_product import DeleteProduct
+from .delete_products import DeleteProducts
+from .delete_repo import DeleteRepo
+from .delete_repos import DeleteRepos
+from .delete_software import DeleteSoftware
+from .delete_softwares import DeleteSoftwares
 from .delete_specification import DeleteSpecification
 from .delete_workflow import DeleteWorkflow
 from .delete_workflows import DeleteWorkflows
 from .disable_alert import DisableAlert
 from .disable_feed import DisableFeed
 from .enable_alert import EnableAlert
 from .enable_feed import EnableFeed
 from .enums import TextTypes
 from .extract_contents import ExtractContents
 from .get_alert import GetAlert
+from .get_category import GetCategory
 from .get_collection import GetCollection
 from .get_content import GetContent
 from .get_conversation import GetConversation
+from .get_event import GetEvent
 from .get_feed import GetFeed
+from .get_label import GetLabel
+from .get_organization import GetOrganization
+from .get_person import GetPerson
+from .get_place import GetPlace
+from .get_product import GetProduct
 from .get_project import GetProject
+from .get_repo import GetRepo
+from .get_software import GetSoftware
 from .get_specification import GetSpecification
 from .get_workflow import GetWorkflow
 from .ingest_encoded_file import IngestEncodedFile
 from .ingest_text import IngestText
 from .ingest_uri import IngestUri
 from .input_types import (
     AlertFilter,
     AlertInput,
     AlertUpdateInput,
+    CategoryFilter,
+    CategoryInput,
+    CategoryUpdateInput,
     CollectionFilter,
     CollectionInput,
     CollectionUpdateInput,
     ContentFacetInput,
     ContentFilter,
     ContentPublishingConnectorInput,
     ContentUpdateInput,
     ConversationFilter,
     ConversationInput,
     ConversationUpdateInput,
     EntityReferenceInput,
+    EventFilter,
+    EventInput,
+    EventUpdateInput,
     FeedFilter,
     FeedInput,
     FeedUpdateInput,
+    LabelFilter,
+    LabelInput,
+    LabelUpdateInput,
+    ObservationInput,
+    ObservationUpdateInput,
+    OrganizationFilter,
+    OrganizationInput,
+    OrganizationUpdateInput,
+    PersonFilter,
+    PersonInput,
+    PersonUpdateInput,
+    PlaceFilter,
+    PlaceInput,
+    PlaceUpdateInput,
+    ProductFilter,
+    ProductInput,
+    ProductUpdateInput,
     ProjectUpdateInput,
+    RepoFilter,
+    RepoInput,
+    RepoUpdateInput,
+    SoftwareFilter,
+    SoftwareInput,
+    SoftwareUpdateInput,
     SpecificationFilter,
     SpecificationInput,
     SpecificationUpdateInput,
     SummarizationStrategyInput,
     WorkflowFilter,
     WorkflowInput,
     WorkflowUpdateInput,
@@ -83,50 +150,88 @@
 from .lookup_credits import LookupCredits
 from .lookup_usage import LookupUsage
 from .operations import (
     ADD_CONTENTS_TO_COLLECTIONS_GQL,
     CLEAR_CONVERSATION_GQL,
     CLOSE_CONVERSATION_GQL,
     CREATE_ALERT_GQL,
+    CREATE_CATEGORY_GQL,
     CREATE_COLLECTION_GQL,
     CREATE_CONVERSATION_GQL,
+    CREATE_EVENT_GQL,
     CREATE_FEED_GQL,
+    CREATE_LABEL_GQL,
+    CREATE_OBSERVATION_GQL,
+    CREATE_ORGANIZATION_GQL,
+    CREATE_PERSON_GQL,
+    CREATE_PLACE_GQL,
+    CREATE_PRODUCT_GQL,
+    CREATE_REPO_GQL,
+    CREATE_SOFTWARE_GQL,
     CREATE_SPECIFICATION_GQL,
     CREATE_WORKFLOW_GQL,
     CREDITS_GQL,
     DELETE_ALERT_GQL,
     DELETE_ALERTS_GQL,
     DELETE_ALL_ALERTS_GQL,
     DELETE_ALL_COLLECTIONS_GQL,
     DELETE_ALL_CONTENTS_GQL,
     DELETE_ALL_CONVERSATIONS_GQL,
     DELETE_ALL_FEEDS_GQL,
     DELETE_ALL_WORKFLOWS_GQL,
+    DELETE_CATEGORIES_GQL,
+    DELETE_CATEGORY_GQL,
     DELETE_COLLECTION_GQL,
     DELETE_COLLECTIONS_GQL,
     DELETE_CONTENT_GQL,
     DELETE_CONTENTS_GQL,
     DELETE_CONVERSATION_GQL,
     DELETE_CONVERSATIONS_GQL,
+    DELETE_EVENT_GQL,
+    DELETE_EVENTS_GQL,
     DELETE_FEED_GQL,
     DELETE_FEEDS_GQL,
+    DELETE_LABEL_GQL,
+    DELETE_LABELS_GQL,
+    DELETE_OBSERVATION_GQL,
+    DELETE_ORGANIZATION_GQL,
+    DELETE_ORGANIZATIONS_GQL,
+    DELETE_PERSON_GQL,
+    DELETE_PERSONS_GQL,
+    DELETE_PLACE_GQL,
+    DELETE_PLACES_GQL,
+    DELETE_PRODUCT_GQL,
+    DELETE_PRODUCTS_GQL,
+    DELETE_REPO_GQL,
+    DELETE_REPOS_GQL,
+    DELETE_SOFTWARE_GQL,
+    DELETE_SOFTWARES_GQL,
     DELETE_SPECIFICATION_GQL,
     DELETE_WORKFLOW_GQL,
     DELETE_WORKFLOWS_GQL,
     DISABLE_ALERT_GQL,
     DISABLE_FEED_GQL,
     ENABLE_ALERT_GQL,
     ENABLE_FEED_GQL,
     EXTRACT_CONTENTS_GQL,
     GET_ALERT_GQL,
+    GET_CATEGORY_GQL,
     GET_COLLECTION_GQL,
     GET_CONTENT_GQL,
     GET_CONVERSATION_GQL,
+    GET_EVENT_GQL,
     GET_FEED_GQL,
+    GET_LABEL_GQL,
+    GET_ORGANIZATION_GQL,
+    GET_PERSON_GQL,
+    GET_PLACE_GQL,
+    GET_PRODUCT_GQL,
     GET_PROJECT_GQL,
+    GET_REPO_GQL,
+    GET_SOFTWARE_GQL,
     GET_SPECIFICATION_GQL,
     GET_WORKFLOW_GQL,
     INGEST_ENCODED_FILE_GQL,
     INGEST_TEXT_GQL,
     INGEST_URI_GQL,
     IS_CONTENT_DONE_GQL,
     IS_FEED_DONE_GQL,
@@ -134,56 +239,94 @@
     LOOKUP_USAGE_GQL,
     PROMPT_CONVERSATION_GQL,
     PROMPT_SPECIFICATIONS_GQL,
     PUBLISH_CONTENTS_GQL,
     PUBLISH_CONVERSATION_GQL,
     PUBLISH_TEXT_GQL,
     QUERY_ALERTS_GQL,
+    QUERY_CATEGORIES_GQL,
     QUERY_COLLECTIONS_GQL,
     QUERY_CONTENT_FACETS_GQL,
     QUERY_CONTENTS_GQL,
     QUERY_CONVERSATIONS_GQL,
+    QUERY_EVENTS_GQL,
     QUERY_FEEDS_GQL,
+    QUERY_LABELS_GQL,
+    QUERY_ORGANIZATIONS_GQL,
+    QUERY_PERSONS_GQL,
+    QUERY_PLACES_GQL,
+    QUERY_PRODUCTS_GQL,
+    QUERY_REPOS_GQL,
+    QUERY_SOFTWARE_GQL,
     QUERY_SPECIFICATIONS_GQL,
     QUERY_WORKFLOWS_GQL,
     REMOVE_CONTENTS_FROM_COLLECTION_GQL,
     SUGGEST_CONVERSATION_GQL,
     SUMMARIZE_CONTENTS_GQL,
     UPDATE_ALERT_GQL,
+    UPDATE_CATEGORY_GQL,
     UPDATE_COLLECTION_GQL,
     UPDATE_CONTENT_GQL,
     UPDATE_CONVERSATION_GQL,
+    UPDATE_EVENT_GQL,
     UPDATE_FEED_GQL,
+    UPDATE_LABEL_GQL,
+    UPDATE_OBSERVATION_GQL,
+    UPDATE_ORGANIZATION_GQL,
+    UPDATE_PERSON_GQL,
+    UPDATE_PLACE_GQL,
+    UPDATE_PRODUCT_GQL,
     UPDATE_PROJECT_GQL,
+    UPDATE_REPO_GQL,
+    UPDATE_SOFTWARE_GQL,
     UPDATE_SPECIFICATION_GQL,
     UPDATE_WORKFLOW_GQL,
     USAGE_GQL,
 )
 from .prompt_conversation import PromptConversation
 from .prompt_specifications import PromptSpecifications
 from .publish_contents import PublishContents
 from .publish_conversation import PublishConversation
 from .publish_text import PublishText
 from .query_alerts import QueryAlerts
+from .query_categories import QueryCategories
 from .query_collections import QueryCollections
 from .query_content_facets import QueryContentFacets
 from .query_contents import QueryContents
 from .query_conversations import QueryConversations
+from .query_events import QueryEvents
 from .query_feeds import QueryFeeds
+from .query_labels import QueryLabels
+from .query_organizations import QueryOrganizations
+from .query_persons import QueryPersons
+from .query_places import QueryPlaces
+from .query_products import QueryProducts
+from .query_repos import QueryRepos
+from .query_software import QuerySoftware
 from .query_specifications import QuerySpecifications
 from .query_workflows import QueryWorkflows
 from .remove_contents_from_collection import RemoveContentsFromCollection
 from .suggest_conversation import SuggestConversation
 from .summarize_contents import SummarizeContents
 from .update_alert import UpdateAlert
+from .update_category import UpdateCategory
 from .update_collection import UpdateCollection
 from .update_content import UpdateContent
 from .update_conversation import UpdateConversation
+from .update_event import UpdateEvent
 from .update_feed import UpdateFeed
+from .update_label import UpdateLabel
+from .update_observation import UpdateObservation
+from .update_organization import UpdateOrganization
+from .update_person import UpdatePerson
+from .update_place import UpdatePlace
+from .update_product import UpdateProduct
 from .update_project import UpdateProject
+from .update_repo import UpdateRepo
+from .update_software import UpdateSoftware
 from .update_specification import UpdateSpecification
 from .update_workflow import UpdateWorkflow
 from .usage import Usage
 
 
 def gql(q: str) -> str:
     return q
@@ -292,14 +435,88 @@
             operation_name="UpdateAlert",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateAlert.model_validate(data)
 
+    async def create_category(
+        self, category: CategoryInput, **kwargs: Any
+    ) -> CreateCategory:
+        variables: Dict[str, object] = {"category": category}
+        response = await self.execute(
+            query=CREATE_CATEGORY_GQL,
+            operation_name="CreateCategory",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CreateCategory.model_validate(data)
+
+    async def delete_categories(
+        self, ids: List[str], **kwargs: Any
+    ) -> DeleteCategories:
+        variables: Dict[str, object] = {"ids": ids}
+        response = await self.execute(
+            query=DELETE_CATEGORIES_GQL,
+            operation_name="DeleteCategories",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteCategories.model_validate(data)
+
+    async def delete_category(self, id: str, **kwargs: Any) -> DeleteCategory:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=DELETE_CATEGORY_GQL,
+            operation_name="DeleteCategory",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteCategory.model_validate(data)
+
+    async def get_category(self, id: str, **kwargs: Any) -> GetCategory:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=GET_CATEGORY_GQL,
+            operation_name="GetCategory",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return GetCategory.model_validate(data)
+
+    async def query_categories(
+        self, filter: CategoryFilter, **kwargs: Any
+    ) -> QueryCategories:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=QUERY_CATEGORIES_GQL,
+            operation_name="QueryCategories",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryCategories.model_validate(data)
+
+    async def update_category(
+        self, category: CategoryUpdateInput, **kwargs: Any
+    ) -> UpdateCategory:
+        variables: Dict[str, object] = {"category": category}
+        response = await self.execute(
+            query=UPDATE_CATEGORY_GQL,
+            operation_name="UpdateCategory",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return UpdateCategory.model_validate(data)
+
     async def add_contents_to_collections(
         self,
         contents: List[EntityReferenceInput],
         collections: List[EntityReferenceInput],
         **kwargs: Any
     ) -> AddContentsToCollections:
         variables: Dict[str, object] = {
@@ -894,14 +1111,80 @@
             operation_name="UpdateConversation",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateConversation.model_validate(data)
 
+    async def create_event(self, event: EventInput, **kwargs: Any) -> CreateEvent:
+        variables: Dict[str, object] = {"event": event}
+        response = await self.execute(
+            query=CREATE_EVENT_GQL,
+            operation_name="CreateEvent",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CreateEvent.model_validate(data)
+
+    async def delete_event(self, id: str, **kwargs: Any) -> DeleteEvent:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=DELETE_EVENT_GQL,
+            operation_name="DeleteEvent",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteEvent.model_validate(data)
+
+    async def delete_events(self, ids: List[str], **kwargs: Any) -> DeleteEvents:
+        variables: Dict[str, object] = {"ids": ids}
+        response = await self.execute(
+            query=DELETE_EVENTS_GQL,
+            operation_name="DeleteEvents",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteEvents.model_validate(data)
+
+    async def get_event(self, id: str, **kwargs: Any) -> GetEvent:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=GET_EVENT_GQL,
+            operation_name="GetEvent",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return GetEvent.model_validate(data)
+
+    async def query_events(self, filter: EventFilter, **kwargs: Any) -> QueryEvents:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=QUERY_EVENTS_GQL,
+            operation_name="QueryEvents",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryEvents.model_validate(data)
+
+    async def update_event(self, event: EventUpdateInput, **kwargs: Any) -> UpdateEvent:
+        variables: Dict[str, object] = {"event": event}
+        response = await self.execute(
+            query=UPDATE_EVENT_GQL,
+            operation_name="UpdateEvent",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return UpdateEvent.model_validate(data)
+
     async def create_feed(
         self,
         feed: FeedInput,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
     ) -> CreateFeed:
         variables: Dict[str, object] = {"feed": feed, "correlationId": correlation_id}
@@ -1008,14 +1291,397 @@
             operation_name="UpdateFeed",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateFeed.model_validate(data)
 
+    async def create_label(self, label: LabelInput, **kwargs: Any) -> CreateLabel:
+        variables: Dict[str, object] = {"label": label}
+        response = await self.execute(
+            query=CREATE_LABEL_GQL,
+            operation_name="CreateLabel",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CreateLabel.model_validate(data)
+
+    async def delete_label(self, id: str, **kwargs: Any) -> DeleteLabel:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=DELETE_LABEL_GQL,
+            operation_name="DeleteLabel",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteLabel.model_validate(data)
+
+    async def delete_labels(self, ids: List[str], **kwargs: Any) -> DeleteLabels:
+        variables: Dict[str, object] = {"ids": ids}
+        response = await self.execute(
+            query=DELETE_LABELS_GQL,
+            operation_name="DeleteLabels",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteLabels.model_validate(data)
+
+    async def get_label(self, id: str, **kwargs: Any) -> GetLabel:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=GET_LABEL_GQL,
+            operation_name="GetLabel",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return GetLabel.model_validate(data)
+
+    async def query_labels(self, filter: LabelFilter, **kwargs: Any) -> QueryLabels:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=QUERY_LABELS_GQL,
+            operation_name="QueryLabels",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryLabels.model_validate(data)
+
+    async def update_label(self, label: LabelUpdateInput, **kwargs: Any) -> UpdateLabel:
+        variables: Dict[str, object] = {"label": label}
+        response = await self.execute(
+            query=UPDATE_LABEL_GQL,
+            operation_name="UpdateLabel",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return UpdateLabel.model_validate(data)
+
+    async def create_observation(
+        self, observation: ObservationInput, **kwargs: Any
+    ) -> CreateObservation:
+        variables: Dict[str, object] = {"observation": observation}
+        response = await self.execute(
+            query=CREATE_OBSERVATION_GQL,
+            operation_name="CreateObservation",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CreateObservation.model_validate(data)
+
+    async def delete_observation(self, id: str, **kwargs: Any) -> DeleteObservation:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=DELETE_OBSERVATION_GQL,
+            operation_name="DeleteObservation",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteObservation.model_validate(data)
+
+    async def update_observation(
+        self, observation: ObservationUpdateInput, **kwargs: Any
+    ) -> UpdateObservation:
+        variables: Dict[str, object] = {"observation": observation}
+        response = await self.execute(
+            query=UPDATE_OBSERVATION_GQL,
+            operation_name="UpdateObservation",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return UpdateObservation.model_validate(data)
+
+    async def create_organization(
+        self, organization: OrganizationInput, **kwargs: Any
+    ) -> CreateOrganization:
+        variables: Dict[str, object] = {"organization": organization}
+        response = await self.execute(
+            query=CREATE_ORGANIZATION_GQL,
+            operation_name="CreateOrganization",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CreateOrganization.model_validate(data)
+
+    async def delete_organization(self, id: str, **kwargs: Any) -> DeleteOrganization:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=DELETE_ORGANIZATION_GQL,
+            operation_name="DeleteOrganization",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteOrganization.model_validate(data)
+
+    async def delete_organizations(
+        self, ids: List[str], **kwargs: Any
+    ) -> DeleteOrganizations:
+        variables: Dict[str, object] = {"ids": ids}
+        response = await self.execute(
+            query=DELETE_ORGANIZATIONS_GQL,
+            operation_name="DeleteOrganizations",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteOrganizations.model_validate(data)
+
+    async def get_organization(self, id: str, **kwargs: Any) -> GetOrganization:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=GET_ORGANIZATION_GQL,
+            operation_name="GetOrganization",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return GetOrganization.model_validate(data)
+
+    async def query_organizations(
+        self, filter: OrganizationFilter, **kwargs: Any
+    ) -> QueryOrganizations:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=QUERY_ORGANIZATIONS_GQL,
+            operation_name="QueryOrganizations",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryOrganizations.model_validate(data)
+
+    async def update_organization(
+        self, organization: OrganizationUpdateInput, **kwargs: Any
+    ) -> UpdateOrganization:
+        variables: Dict[str, object] = {"organization": organization}
+        response = await self.execute(
+            query=UPDATE_ORGANIZATION_GQL,
+            operation_name="UpdateOrganization",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return UpdateOrganization.model_validate(data)
+
+    async def create_person(self, person: PersonInput, **kwargs: Any) -> CreatePerson:
+        variables: Dict[str, object] = {"person": person}
+        response = await self.execute(
+            query=CREATE_PERSON_GQL,
+            operation_name="CreatePerson",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CreatePerson.model_validate(data)
+
+    async def delete_person(self, id: str, **kwargs: Any) -> DeletePerson:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=DELETE_PERSON_GQL,
+            operation_name="DeletePerson",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeletePerson.model_validate(data)
+
+    async def delete_persons(self, ids: List[str], **kwargs: Any) -> DeletePersons:
+        variables: Dict[str, object] = {"ids": ids}
+        response = await self.execute(
+            query=DELETE_PERSONS_GQL,
+            operation_name="DeletePersons",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeletePersons.model_validate(data)
+
+    async def get_person(self, id: str, **kwargs: Any) -> GetPerson:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=GET_PERSON_GQL,
+            operation_name="GetPerson",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return GetPerson.model_validate(data)
+
+    async def query_persons(self, filter: PersonFilter, **kwargs: Any) -> QueryPersons:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=QUERY_PERSONS_GQL,
+            operation_name="QueryPersons",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryPersons.model_validate(data)
+
+    async def update_person(
+        self, person: PersonUpdateInput, **kwargs: Any
+    ) -> UpdatePerson:
+        variables: Dict[str, object] = {"person": person}
+        response = await self.execute(
+            query=UPDATE_PERSON_GQL,
+            operation_name="UpdatePerson",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return UpdatePerson.model_validate(data)
+
+    async def create_place(self, place: PlaceInput, **kwargs: Any) -> CreatePlace:
+        variables: Dict[str, object] = {"place": place}
+        response = await self.execute(
+            query=CREATE_PLACE_GQL,
+            operation_name="CreatePlace",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CreatePlace.model_validate(data)
+
+    async def delete_place(self, id: str, **kwargs: Any) -> DeletePlace:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=DELETE_PLACE_GQL,
+            operation_name="DeletePlace",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeletePlace.model_validate(data)
+
+    async def delete_places(self, ids: List[str], **kwargs: Any) -> DeletePlaces:
+        variables: Dict[str, object] = {"ids": ids}
+        response = await self.execute(
+            query=DELETE_PLACES_GQL,
+            operation_name="DeletePlaces",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeletePlaces.model_validate(data)
+
+    async def get_place(self, id: str, **kwargs: Any) -> GetPlace:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=GET_PLACE_GQL,
+            operation_name="GetPlace",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return GetPlace.model_validate(data)
+
+    async def query_places(self, filter: PlaceFilter, **kwargs: Any) -> QueryPlaces:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=QUERY_PLACES_GQL,
+            operation_name="QueryPlaces",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryPlaces.model_validate(data)
+
+    async def update_place(self, place: PlaceUpdateInput, **kwargs: Any) -> UpdatePlace:
+        variables: Dict[str, object] = {"place": place}
+        response = await self.execute(
+            query=UPDATE_PLACE_GQL,
+            operation_name="UpdatePlace",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return UpdatePlace.model_validate(data)
+
+    async def create_product(
+        self, product: ProductInput, **kwargs: Any
+    ) -> CreateProduct:
+        variables: Dict[str, object] = {"product": product}
+        response = await self.execute(
+            query=CREATE_PRODUCT_GQL,
+            operation_name="CreateProduct",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CreateProduct.model_validate(data)
+
+    async def delete_product(self, id: str, **kwargs: Any) -> DeleteProduct:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=DELETE_PRODUCT_GQL,
+            operation_name="DeleteProduct",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteProduct.model_validate(data)
+
+    async def delete_products(self, ids: List[str], **kwargs: Any) -> DeleteProducts:
+        variables: Dict[str, object] = {"ids": ids}
+        response = await self.execute(
+            query=DELETE_PRODUCTS_GQL,
+            operation_name="DeleteProducts",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteProducts.model_validate(data)
+
+    async def get_product(self, id: str, **kwargs: Any) -> GetProduct:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=GET_PRODUCT_GQL,
+            operation_name="GetProduct",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return GetProduct.model_validate(data)
+
+    async def query_products(
+        self, filter: ProductFilter, **kwargs: Any
+    ) -> QueryProducts:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=QUERY_PRODUCTS_GQL,
+            operation_name="QueryProducts",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryProducts.model_validate(data)
+
+    async def update_product(
+        self, product: ProductUpdateInput, **kwargs: Any
+    ) -> UpdateProduct:
+        variables: Dict[str, object] = {"product": product}
+        response = await self.execute(
+            query=UPDATE_PRODUCT_GQL,
+            operation_name="UpdateProduct",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return UpdateProduct.model_validate(data)
+
     async def credits(self, start_date: Any, duration: Any, **kwargs: Any) -> Credits:
         variables: Dict[str, object] = {"startDate": start_date, "duration": duration}
         response = await self.execute(
             query=CREDITS_GQL, operation_name="Credits", variables=variables, **kwargs
         )
         data = self.get_data(response)
         return Credits.model_validate(data)
@@ -1070,14 +1736,149 @@
         variables: Dict[str, object] = {"startDate": start_date, "duration": duration}
         response = await self.execute(
             query=USAGE_GQL, operation_name="Usage", variables=variables, **kwargs
         )
         data = self.get_data(response)
         return Usage.model_validate(data)
 
+    async def create_repo(self, repo: RepoInput, **kwargs: Any) -> CreateRepo:
+        variables: Dict[str, object] = {"repo": repo}
+        response = await self.execute(
+            query=CREATE_REPO_GQL,
+            operation_name="CreateRepo",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CreateRepo.model_validate(data)
+
+    async def delete_repo(self, id: str, **kwargs: Any) -> DeleteRepo:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=DELETE_REPO_GQL,
+            operation_name="DeleteRepo",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteRepo.model_validate(data)
+
+    async def delete_repos(self, ids: List[str], **kwargs: Any) -> DeleteRepos:
+        variables: Dict[str, object] = {"ids": ids}
+        response = await self.execute(
+            query=DELETE_REPOS_GQL,
+            operation_name="DeleteRepos",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteRepos.model_validate(data)
+
+    async def get_repo(self, id: str, **kwargs: Any) -> GetRepo:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=GET_REPO_GQL, operation_name="GetRepo", variables=variables, **kwargs
+        )
+        data = self.get_data(response)
+        return GetRepo.model_validate(data)
+
+    async def query_repos(self, filter: RepoFilter, **kwargs: Any) -> QueryRepos:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=QUERY_REPOS_GQL,
+            operation_name="QueryRepos",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryRepos.model_validate(data)
+
+    async def update_repo(self, repo: RepoUpdateInput, **kwargs: Any) -> UpdateRepo:
+        variables: Dict[str, object] = {"repo": repo}
+        response = await self.execute(
+            query=UPDATE_REPO_GQL,
+            operation_name="UpdateRepo",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return UpdateRepo.model_validate(data)
+
+    async def create_software(
+        self, software: SoftwareInput, **kwargs: Any
+    ) -> CreateSoftware:
+        variables: Dict[str, object] = {"software": software}
+        response = await self.execute(
+            query=CREATE_SOFTWARE_GQL,
+            operation_name="CreateSoftware",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CreateSoftware.model_validate(data)
+
+    async def delete_software(self, id: str, **kwargs: Any) -> DeleteSoftware:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=DELETE_SOFTWARE_GQL,
+            operation_name="DeleteSoftware",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteSoftware.model_validate(data)
+
+    async def delete_softwares(self, ids: List[str], **kwargs: Any) -> DeleteSoftwares:
+        variables: Dict[str, object] = {"ids": ids}
+        response = await self.execute(
+            query=DELETE_SOFTWARES_GQL,
+            operation_name="DeleteSoftwares",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteSoftwares.model_validate(data)
+
+    async def get_software(self, id: str, **kwargs: Any) -> GetSoftware:
+        variables: Dict[str, object] = {"id": id}
+        response = await self.execute(
+            query=GET_SOFTWARE_GQL,
+            operation_name="GetSoftware",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return GetSoftware.model_validate(data)
+
+    async def query_software(
+        self, filter: SoftwareFilter, **kwargs: Any
+    ) -> QuerySoftware:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=QUERY_SOFTWARE_GQL,
+            operation_name="QuerySoftware",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QuerySoftware.model_validate(data)
+
+    async def update_software(
+        self, software: SoftwareUpdateInput, **kwargs: Any
+    ) -> UpdateSoftware:
+        variables: Dict[str, object] = {"software": software}
+        response = await self.execute(
+            query=UPDATE_SOFTWARE_GQL,
+            operation_name="UpdateSoftware",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return UpdateSoftware.model_validate(data)
+
     async def create_specification(
         self, specification: SpecificationInput, **kwargs: Any
     ) -> CreateSpecification:
         variables: Dict[str, object] = {"specification": specification}
         response = await self.execute(
             query=CREATE_SPECIFICATION_GQL,
             operation_name="CreateSpecification",
```

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/close_conversation.py` & `graphlit_client-1.0.20240426001/graphlit_api/close_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/create_collection.py` & `graphlit_client-1.0.20240426001/graphlit_api/create_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/create_conversation.py` & `graphlit_client-1.0.20240426001/graphlit_api/create_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/create_specification.py` & `graphlit_client-1.0.20240426001/graphlit_api/create_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/create_workflow.py` & `graphlit_client-1.0.20240426001/graphlit_api/create_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/credits.py` & `graphlit_client-1.0.20240426001/graphlit_api/credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/delete_all_conversations.py` & `graphlit_client-1.0.20240426001/graphlit_api/delete_all_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/enums.py` & `graphlit_client-1.0.20240426001/graphlit_api/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,14 +568,15 @@
     FOOTNOTE = "FOOTNOTE"
     CODE = "CODE"
     LIST_ITEM = "LIST_ITEM"
     HEADING1 = "HEADING1"
     HEADING2 = "HEADING2"
     HEADING3 = "HEADING3"
     HEADING4 = "HEADING4"
+    HEADING5 = "HEADING5"
     TABLE_COLUMN_HEADER = "TABLE_COLUMN_HEADER"
     TABLE_ROW_HEADER = "TABLE_ROW_HEADER"
     TABLE_CORNER_HEADER = "TABLE_CORNER_HEADER"
     TABLE_CELL = "TABLE_CELL"
     TABLE_CAPTION = "TABLE_CAPTION"
     TABLE = "TABLE"
     COLUMN_HEADER = "COLUMN_HEADER"
```

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/exceptions.py` & `graphlit_client-1.0.20240426001/graphlit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/extract_contents.py` & `graphlit_client-1.0.20240426001/graphlit_api/extract_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/get_alert.py` & `graphlit_client-1.0.20240426001/graphlit_api/get_alert.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/get_collection.py` & `graphlit_client-1.0.20240426001/graphlit_api/get_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/get_content.py` & `graphlit_client-1.0.20240426001/graphlit_api/get_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/get_conversation.py` & `graphlit_client-1.0.20240426001/graphlit_api/get_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/get_feed.py` & `graphlit_client-1.0.20240426001/graphlit_api/get_feed.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/get_project.py` & `graphlit_client-1.0.20240426001/graphlit_api/get_project.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/get_specification.py` & `graphlit_client-1.0.20240426001/graphlit_api/get_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/get_workflow.py` & `graphlit_client-1.0.20240426001/graphlit_api/get_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/ingest_encoded_file.py` & `graphlit_client-1.0.20240426001/graphlit_api/ingest_encoded_file.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/ingest_text.py` & `graphlit_client-1.0.20240426001/graphlit_api/ingest_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/ingest_uri.py` & `graphlit_client-1.0.20240426001/graphlit_api/ingest_uri.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/input_types.py` & `graphlit_client-1.0.20240426001/graphlit_api/input_types.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/lookup_credits.py` & `graphlit_client-1.0.20240426001/graphlit_api/lookup_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/lookup_usage.py` & `graphlit_client-1.0.20240426001/graphlit_api/lookup_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/operations.py` & `graphlit_client-1.0.20240426001/graphlit_api/operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,50 +2,88 @@
 # Source: ./documents
 
 __all__ = [
     "ADD_CONTENTS_TO_COLLECTIONS_GQL",
     "CLEAR_CONVERSATION_GQL",
     "CLOSE_CONVERSATION_GQL",
     "CREATE_ALERT_GQL",
+    "CREATE_CATEGORY_GQL",
     "CREATE_COLLECTION_GQL",
     "CREATE_CONVERSATION_GQL",
+    "CREATE_EVENT_GQL",
     "CREATE_FEED_GQL",
+    "CREATE_LABEL_GQL",
+    "CREATE_OBSERVATION_GQL",
+    "CREATE_ORGANIZATION_GQL",
+    "CREATE_PERSON_GQL",
+    "CREATE_PLACE_GQL",
+    "CREATE_PRODUCT_GQL",
+    "CREATE_REPO_GQL",
+    "CREATE_SOFTWARE_GQL",
     "CREATE_SPECIFICATION_GQL",
     "CREATE_WORKFLOW_GQL",
     "CREDITS_GQL",
     "DELETE_ALERTS_GQL",
     "DELETE_ALERT_GQL",
     "DELETE_ALL_ALERTS_GQL",
     "DELETE_ALL_COLLECTIONS_GQL",
     "DELETE_ALL_CONTENTS_GQL",
     "DELETE_ALL_CONVERSATIONS_GQL",
     "DELETE_ALL_FEEDS_GQL",
     "DELETE_ALL_WORKFLOWS_GQL",
+    "DELETE_CATEGORIES_GQL",
+    "DELETE_CATEGORY_GQL",
     "DELETE_COLLECTIONS_GQL",
     "DELETE_COLLECTION_GQL",
     "DELETE_CONTENTS_GQL",
     "DELETE_CONTENT_GQL",
     "DELETE_CONVERSATIONS_GQL",
     "DELETE_CONVERSATION_GQL",
+    "DELETE_EVENTS_GQL",
+    "DELETE_EVENT_GQL",
     "DELETE_FEEDS_GQL",
     "DELETE_FEED_GQL",
+    "DELETE_LABELS_GQL",
+    "DELETE_LABEL_GQL",
+    "DELETE_OBSERVATION_GQL",
+    "DELETE_ORGANIZATIONS_GQL",
+    "DELETE_ORGANIZATION_GQL",
+    "DELETE_PERSONS_GQL",
+    "DELETE_PERSON_GQL",
+    "DELETE_PLACES_GQL",
+    "DELETE_PLACE_GQL",
+    "DELETE_PRODUCTS_GQL",
+    "DELETE_PRODUCT_GQL",
+    "DELETE_REPOS_GQL",
+    "DELETE_REPO_GQL",
+    "DELETE_SOFTWARES_GQL",
+    "DELETE_SOFTWARE_GQL",
     "DELETE_SPECIFICATION_GQL",
     "DELETE_WORKFLOWS_GQL",
     "DELETE_WORKFLOW_GQL",
     "DISABLE_ALERT_GQL",
     "DISABLE_FEED_GQL",
     "ENABLE_ALERT_GQL",
     "ENABLE_FEED_GQL",
     "EXTRACT_CONTENTS_GQL",
     "GET_ALERT_GQL",
+    "GET_CATEGORY_GQL",
     "GET_COLLECTION_GQL",
     "GET_CONTENT_GQL",
     "GET_CONVERSATION_GQL",
+    "GET_EVENT_GQL",
     "GET_FEED_GQL",
+    "GET_LABEL_GQL",
+    "GET_ORGANIZATION_GQL",
+    "GET_PERSON_GQL",
+    "GET_PLACE_GQL",
+    "GET_PRODUCT_GQL",
     "GET_PROJECT_GQL",
+    "GET_REPO_GQL",
+    "GET_SOFTWARE_GQL",
     "GET_SPECIFICATION_GQL",
     "GET_WORKFLOW_GQL",
     "INGEST_ENCODED_FILE_GQL",
     "INGEST_TEXT_GQL",
     "INGEST_URI_GQL",
     "IS_CONTENT_DONE_GQL",
     "IS_FEED_DONE_GQL",
@@ -53,30 +91,49 @@
     "LOOKUP_USAGE_GQL",
     "PROMPT_CONVERSATION_GQL",
     "PROMPT_SPECIFICATIONS_GQL",
     "PUBLISH_CONTENTS_GQL",
     "PUBLISH_CONVERSATION_GQL",
     "PUBLISH_TEXT_GQL",
     "QUERY_ALERTS_GQL",
+    "QUERY_CATEGORIES_GQL",
     "QUERY_COLLECTIONS_GQL",
     "QUERY_CONTENTS_GQL",
     "QUERY_CONTENT_FACETS_GQL",
     "QUERY_CONVERSATIONS_GQL",
+    "QUERY_EVENTS_GQL",
     "QUERY_FEEDS_GQL",
+    "QUERY_LABELS_GQL",
+    "QUERY_ORGANIZATIONS_GQL",
+    "QUERY_PERSONS_GQL",
+    "QUERY_PLACES_GQL",
+    "QUERY_PRODUCTS_GQL",
+    "QUERY_REPOS_GQL",
+    "QUERY_SOFTWARE_GQL",
     "QUERY_SPECIFICATIONS_GQL",
     "QUERY_WORKFLOWS_GQL",
     "REMOVE_CONTENTS_FROM_COLLECTION_GQL",
     "SUGGEST_CONVERSATION_GQL",
     "SUMMARIZE_CONTENTS_GQL",
     "UPDATE_ALERT_GQL",
+    "UPDATE_CATEGORY_GQL",
     "UPDATE_COLLECTION_GQL",
     "UPDATE_CONTENT_GQL",
     "UPDATE_CONVERSATION_GQL",
+    "UPDATE_EVENT_GQL",
     "UPDATE_FEED_GQL",
+    "UPDATE_LABEL_GQL",
+    "UPDATE_OBSERVATION_GQL",
+    "UPDATE_ORGANIZATION_GQL",
+    "UPDATE_PERSON_GQL",
+    "UPDATE_PLACE_GQL",
+    "UPDATE_PRODUCT_GQL",
     "UPDATE_PROJECT_GQL",
+    "UPDATE_REPO_GQL",
+    "UPDATE_SOFTWARE_GQL",
     "UPDATE_SPECIFICATION_GQL",
     "UPDATE_WORKFLOW_GQL",
     "USAGE_GQL",
 ]
 
 CREATE_ALERT_GQL = """
 mutation CreateAlert($alert: AlertInput!, $correlationId: String) {
@@ -285,14 +342,70 @@
     name
     state
     type
   }
 }
 """
 
+CREATE_CATEGORY_GQL = """
+mutation CreateCategory($category: CategoryInput!) {
+  createCategory(category: $category) {
+    id
+    name
+  }
+}
+"""
+
+DELETE_CATEGORIES_GQL = """
+mutation DeleteCategories($ids: [ID!]!) {
+  deleteCategories(ids: $ids) {
+    id
+    state
+  }
+}
+"""
+
+DELETE_CATEGORY_GQL = """
+mutation DeleteCategory($id: ID!) {
+  deleteCategory(id: $id) {
+    id
+    state
+  }
+}
+"""
+
+GET_CATEGORY_GQL = """
+query GetCategory($id: ID!) {
+  category(id: $id) {
+    id
+    name
+  }
+}
+"""
+
+QUERY_CATEGORIES_GQL = """
+query QueryCategories($filter: CategoryFilter!) {
+  categories(filter: $filter) {
+    results {
+      id
+      name
+    }
+  }
+}
+"""
+
+UPDATE_CATEGORY_GQL = """
+mutation UpdateCategory($category: CategoryUpdateInput!) {
+  updateCategory(category: $category) {
+    id
+    name
+  }
+}
+"""
+
 ADD_CONTENTS_TO_COLLECTIONS_GQL = """
 mutation AddContentsToCollections($contents: [EntityReferenceInput!]!, $collections: [EntityReferenceInput!]!) {
   addContentsToCollections(contents: $contents, collections: $collections) {
     id
     name
     state
     type
@@ -1297,14 +1410,80 @@
     name
     state
     type
   }
 }
 """
 
+CREATE_EVENT_GQL = """
+mutation CreateEvent($event: EventInput!) {
+  createEvent(event: $event) {
+    id
+    name
+  }
+}
+"""
+
+DELETE_EVENT_GQL = """
+mutation DeleteEvent($id: ID!) {
+  deleteEvent(id: $id) {
+    id
+    state
+  }
+}
+"""
+
+DELETE_EVENTS_GQL = """
+mutation DeleteEvents($ids: [ID!]!) {
+  deleteEvents(ids: $ids) {
+    id
+    state
+  }
+}
+"""
+
+GET_EVENT_GQL = """
+query GetEvent($id: ID!) {
+  event(id: $id) {
+    id
+    name
+    alternateNames
+    creationDate
+    startDate
+    endDate
+    price
+  }
+}
+"""
+
+QUERY_EVENTS_GQL = """
+query QueryEvents($filter: EventFilter!) {
+  events(filter: $filter) {
+    results {
+      id
+      name
+      alternateNames
+      creationDate
+      startDate
+      endDate
+      price
+    }
+  }
+}
+"""
+
+UPDATE_EVENT_GQL = """
+mutation UpdateEvent($event: EventUpdateInput!) {
+  updateEvent(event: $event) {
+    id
+    name
+  }
+}
+"""
+
 CREATE_FEED_GQL = """
 mutation CreateFeed($feed: FeedInput!, $correlationId: String) {
   createFeed(feed: $feed, correlationId: $correlationId) {
     id
     name
     state
     type
@@ -1668,14 +1847,381 @@
     name
     state
     type
   }
 }
 """
 
+CREATE_LABEL_GQL = """
+mutation CreateLabel($label: LabelInput!) {
+  createLabel(label: $label) {
+    id
+    name
+  }
+}
+"""
+
+DELETE_LABEL_GQL = """
+mutation DeleteLabel($id: ID!) {
+  deleteLabel(id: $id) {
+    id
+    state
+  }
+}
+"""
+
+DELETE_LABELS_GQL = """
+mutation DeleteLabels($ids: [ID!]!) {
+  deleteLabels(ids: $ids) {
+    id
+    state
+  }
+}
+"""
+
+GET_LABEL_GQL = """
+query GetLabel($id: ID!) {
+  label(id: $id) {
+    id
+    name
+  }
+}
+"""
+
+QUERY_LABELS_GQL = """
+query QueryLabels($filter: LabelFilter!) {
+  labels(filter: $filter) {
+    results {
+      id
+      name
+    }
+  }
+}
+"""
+
+UPDATE_LABEL_GQL = """
+mutation UpdateLabel($label: LabelUpdateInput!) {
+  updateLabel(label: $label) {
+    id
+    name
+  }
+}
+"""
+
+CREATE_OBSERVATION_GQL = """
+mutation CreateObservation($observation: ObservationInput!) {
+  createObservation(observation: $observation) {
+    id
+    state
+  }
+}
+"""
+
+DELETE_OBSERVATION_GQL = """
+mutation DeleteObservation($id: ID!) {
+  deleteObservation(id: $id) {
+    id
+    state
+  }
+}
+"""
+
+UPDATE_OBSERVATION_GQL = """
+mutation UpdateObservation($observation: ObservationUpdateInput!) {
+  updateObservation(observation: $observation) {
+    id
+    state
+  }
+}
+"""
+
+CREATE_ORGANIZATION_GQL = """
+mutation CreateOrganization($organization: OrganizationInput!) {
+  createOrganization(organization: $organization) {
+    id
+    name
+    foundingDate
+    industries
+    revenue
+    revenueCurrency
+    investment
+    investmentCurrency
+  }
+}
+"""
+
+DELETE_ORGANIZATION_GQL = """
+mutation DeleteOrganization($id: ID!) {
+  deleteOrganization(id: $id) {
+    id
+    state
+  }
+}
+"""
+
+DELETE_ORGANIZATIONS_GQL = """
+mutation DeleteOrganizations($ids: [ID!]!) {
+  deleteOrganizations(ids: $ids) {
+    id
+    state
+  }
+}
+"""
+
+GET_ORGANIZATION_GQL = """
+query GetOrganization($id: ID!) {
+  organization(id: $id) {
+    id
+    name
+    alternateNames
+    creationDate
+    foundingDate
+    industries
+    revenue
+    revenueCurrency
+    investment
+    investmentCurrency
+  }
+}
+"""
+
+QUERY_ORGANIZATIONS_GQL = """
+query QueryOrganizations($filter: OrganizationFilter!) {
+  organizations(filter: $filter) {
+    results {
+      id
+      name
+      alternateNames
+      creationDate
+      foundingDate
+      industries
+      revenue
+      revenueCurrency
+      investment
+      investmentCurrency
+    }
+  }
+}
+"""
+
+UPDATE_ORGANIZATION_GQL = """
+mutation UpdateOrganization($organization: OrganizationUpdateInput!) {
+  updateOrganization(organization: $organization) {
+    id
+    name
+    foundingDate
+    industries
+    revenue
+    revenueCurrency
+    investment
+    investmentCurrency
+  }
+}
+"""
+
+CREATE_PERSON_GQL = """
+mutation CreatePerson($person: PersonInput!) {
+  createPerson(person: $person) {
+    id
+    name
+  }
+}
+"""
+
+DELETE_PERSON_GQL = """
+mutation DeletePerson($id: ID!) {
+  deletePerson(id: $id) {
+    id
+    state
+  }
+}
+"""
+
+DELETE_PERSONS_GQL = """
+mutation DeletePersons($ids: [ID!]!) {
+  deletePersons(ids: $ids) {
+    id
+    state
+  }
+}
+"""
+
+GET_PERSON_GQL = """
+query GetPerson($id: ID!) {
+  person(id: $id) {
+    id
+    name
+    alternateNames
+    creationDate
+    email
+    givenName
+    familyName
+  }
+}
+"""
+
+QUERY_PERSONS_GQL = """
+query QueryPersons($filter: PersonFilter!) {
+  persons(filter: $filter) {
+    results {
+      id
+      name
+      alternateNames
+      creationDate
+      email
+      givenName
+      familyName
+    }
+  }
+}
+"""
+
+UPDATE_PERSON_GQL = """
+mutation UpdatePerson($person: PersonUpdateInput!) {
+  updatePerson(person: $person) {
+    id
+    name
+  }
+}
+"""
+
+CREATE_PLACE_GQL = """
+mutation CreatePlace($place: PlaceInput!) {
+  createPlace(place: $place) {
+    id
+    name
+  }
+}
+"""
+
+DELETE_PLACE_GQL = """
+mutation DeletePlace($id: ID!) {
+  deletePlace(id: $id) {
+    id
+    state
+  }
+}
+"""
+
+DELETE_PLACES_GQL = """
+mutation DeletePlaces($ids: [ID!]!) {
+  deletePlaces(ids: $ids) {
+    id
+    state
+  }
+}
+"""
+
+GET_PLACE_GQL = """
+query GetPlace($id: ID!) {
+  place(id: $id) {
+    id
+    name
+    alternateNames
+    creationDate
+  }
+}
+"""
+
+QUERY_PLACES_GQL = """
+query QueryPlaces($filter: PlaceFilter!) {
+  places(filter: $filter) {
+    results {
+      id
+      name
+      alternateNames
+      creationDate
+    }
+  }
+}
+"""
+
+UPDATE_PLACE_GQL = """
+mutation UpdatePlace($place: PlaceUpdateInput!) {
+  updatePlace(place: $place) {
+    id
+    name
+  }
+}
+"""
+
+CREATE_PRODUCT_GQL = """
+mutation CreateProduct($product: ProductInput!) {
+  createProduct(product: $product) {
+    id
+    name
+  }
+}
+"""
+
+DELETE_PRODUCT_GQL = """
+mutation DeleteProduct($id: ID!) {
+  deleteProduct(id: $id) {
+    id
+    state
+  }
+}
+"""
+
+DELETE_PRODUCTS_GQL = """
+mutation DeleteProducts($ids: [ID!]!) {
+  deleteProducts(ids: $ids) {
+    id
+    state
+  }
+}
+"""
+
+GET_PRODUCT_GQL = """
+query GetProduct($id: ID!) {
+  product(id: $id) {
+    id
+    name
+    alternateNames
+    creationDate
+    manufacturer
+    model
+    brand
+    upc
+    sku
+    releaseDate
+    productionDate
+  }
+}
+"""
+
+QUERY_PRODUCTS_GQL = """
+query QueryProducts($filter: ProductFilter!) {
+  products(filter: $filter) {
+    results {
+      id
+      name
+      alternateNames
+      creationDate
+      manufacturer
+      model
+      brand
+      upc
+      sku
+      releaseDate
+      productionDate
+    }
+  }
+}
+"""
+
+UPDATE_PRODUCT_GQL = """
+mutation UpdateProduct($product: ProductUpdateInput!) {
+  updateProduct(product: $product) {
+    id
+    name
+  }
+}
+"""
+
 CREDITS_GQL = """
 query Credits($startDate: DateTime!, $duration: TimeSpan!) {
   credits(startDate: $startDate, duration: $duration) {
     correlationId
     ownerId
     credits
     storageRatio
@@ -1812,14 +2358,138 @@
     request
     variables
     response
   }
 }
 """
 
+CREATE_REPO_GQL = """
+mutation CreateRepo($repo: RepoInput!) {
+  createRepo(repo: $repo) {
+    id
+    name
+  }
+}
+"""
+
+DELETE_REPO_GQL = """
+mutation DeleteRepo($id: ID!) {
+  deleteRepo(id: $id) {
+    id
+    state
+  }
+}
+"""
+
+DELETE_REPOS_GQL = """
+mutation DeleteRepos($ids: [ID!]!) {
+  deleteRepos(ids: $ids) {
+    id
+    state
+  }
+}
+"""
+
+GET_REPO_GQL = """
+query GetRepo($id: ID!) {
+  repo(id: $id) {
+    id
+    name
+    alternateNames
+    creationDate
+  }
+}
+"""
+
+QUERY_REPOS_GQL = """
+query QueryRepos($filter: RepoFilter!) {
+  repos(filter: $filter) {
+    results {
+      id
+      name
+      alternateNames
+      creationDate
+    }
+  }
+}
+"""
+
+UPDATE_REPO_GQL = """
+mutation UpdateRepo($repo: RepoUpdateInput!) {
+  updateRepo(repo: $repo) {
+    id
+    name
+  }
+}
+"""
+
+CREATE_SOFTWARE_GQL = """
+mutation CreateSoftware($software: SoftwareInput!) {
+  createSoftware(software: $software) {
+    id
+    name
+  }
+}
+"""
+
+DELETE_SOFTWARE_GQL = """
+mutation DeleteSoftware($id: ID!) {
+  deleteSoftware(id: $id) {
+    id
+    state
+  }
+}
+"""
+
+DELETE_SOFTWARES_GQL = """
+mutation DeleteSoftwares($ids: [ID!]!) {
+  deleteSoftwares(ids: $ids) {
+    id
+    state
+  }
+}
+"""
+
+GET_SOFTWARE_GQL = """
+query GetSoftware($id: ID!) {
+  software(id: $id) {
+    id
+    name
+    alternateNames
+    creationDate
+    releaseDate
+    developer
+  }
+}
+"""
+
+QUERY_SOFTWARE_GQL = """
+query QuerySoftware($filter: SoftwareFilter!) {
+  softwares(filter: $filter) {
+    results {
+      id
+      name
+      alternateNames
+      creationDate
+      releaseDate
+      developer
+    }
+  }
+}
+"""
+
+UPDATE_SOFTWARE_GQL = """
+mutation UpdateSoftware($software: SoftwareUpdateInput!) {
+  updateSoftware(software: $software) {
+    id
+    name
+  }
+}
+"""
+
 CREATE_SPECIFICATION_GQL = """
 mutation CreateSpecification($specification: SpecificationInput!) {
   createSpecification(specification: $specification) {
     id
     name
     state
     type
```

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/prompt_conversation.py` & `graphlit_client-1.0.20240426001/graphlit_api/prompt_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/prompt_specifications.py` & `graphlit_client-1.0.20240426001/graphlit_api/prompt_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/publish_contents.py` & `graphlit_client-1.0.20240426001/graphlit_api/publish_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/publish_conversation.py` & `graphlit_client-1.0.20240426001/graphlit_api/publish_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/publish_text.py` & `graphlit_client-1.0.20240426001/graphlit_api/publish_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/query_alerts.py` & `graphlit_client-1.0.20240426001/graphlit_api/query_alerts.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/query_collections.py` & `graphlit_client-1.0.20240426001/graphlit_api/query_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/query_content_facets.py` & `graphlit_client-1.0.20240426001/graphlit_api/query_content_facets.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/query_contents.py` & `graphlit_client-1.0.20240426001/graphlit_api/query_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/query_conversations.py` & `graphlit_client-1.0.20240426001/graphlit_api/query_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/query_feeds.py` & `graphlit_client-1.0.20240426001/graphlit_api/query_feeds.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/query_specifications.py` & `graphlit_client-1.0.20240426001/graphlit_api/query_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/query_workflows.py` & `graphlit_client-1.0.20240426001/graphlit_api/query_workflows.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/remove_contents_from_collection.py` & `graphlit_client-1.0.20240426001/graphlit_api/remove_contents_from_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/summarize_contents.py` & `graphlit_client-1.0.20240426001/graphlit_api/summarize_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/update_collection.py` & `graphlit_client-1.0.20240426001/graphlit_api/update_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/update_content.py` & `graphlit_client-1.0.20240426001/graphlit_api/update_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/update_conversation.py` & `graphlit_client-1.0.20240426001/graphlit_api/update_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/update_specification.py` & `graphlit_client-1.0.20240426001/graphlit_api/update_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/update_workflow.py` & `graphlit_client-1.0.20240426001/graphlit_api/update_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_api/usage.py` & `graphlit_client-1.0.20240426001/graphlit_api/usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240425001/graphlit_client.egg-info/PKG-INFO` & `graphlit_client-1.0.20240426001/graphlit_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240425001
+Version: 1.0.20240426001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240425001/setup.py` & `graphlit_client-1.0.20240426001/setup.py`

 * *Files identical despite different names*

