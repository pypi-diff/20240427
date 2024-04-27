# Comparing `tmp/taskingai-0.2.1.tar.gz` & `tmp/taskingai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskingai-0.2.1.tar", last modified: Wed Mar 13 12:59:07 2024, max compression
+gzip compressed data, was "taskingai-0.2.2.tar", last modified: Fri Apr 26 13:17:36 2024, max compression
```

## Comparing `taskingai-0.2.1.tar` & `taskingai-0.2.2.tar`

### file list

```diff
@@ -1,207 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.843003 taskingai-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-13 12:56:46.000000 taskingai-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-03-13 12:59:07.843003 taskingai-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-03-13 12:56:46.000000 taskingai-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-13 12:56:46.000000 taskingai-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 12:59:07.843003 taskingai-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-13 12:56:46.000000 taskingai-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.807003 taskingai-0.2.1/taskingai/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.807003 taskingai-0.2.1/taskingai/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/assistant/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/assistant/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/assistant/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.811003 taskingai-0.2.1/taskingai/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23799 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.815003 taskingai-0.2.1/taskingai/client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_bulk_create_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_create_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_create_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_create_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_create_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_create_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_create_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_delete_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_delete_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_delete_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_delete_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_delete_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_delete_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_delete_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_generate_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_get_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_get_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_get_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_get_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_get_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_get_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_list_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_list_assistants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_list_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_list_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_list_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_list_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_list_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_query_collection_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_run_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_update_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_update_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_update_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_update_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_update_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_update_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/apis/api_update_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.815003 taskingai-0.2.1/taskingai/client/models/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.823003 taskingai-0.2.1/taskingai/client/models/entities/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/action_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/action_authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/action_body_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/action_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/action_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/assistant_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/assistant_memory_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_assistant_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_finish_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_function_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_function_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_function_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_function_parameters_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_system_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_completion_user_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chat_memory_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/message_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/message_content.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/message_generation_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/message_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/record_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/retrieval_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/retrieval_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/retrieval_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/retrieval_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/sort_order_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/text_embedding_input_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/text_embedding_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/text_splitter_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/tool_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/entities/tool_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.839003 taskingai-0.2.1/taskingai/client/models/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/action_bulk_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/action_bulk_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/action_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/action_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/action_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/action_run_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/action_run_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/action_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/action_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/assistant_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/assistant_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/assistant_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/assistant_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/assistant_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/assistant_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/assistant_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/base_data_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/base_empty_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chat_completion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chat_completion_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chat_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chat_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chat_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chat_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chat_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chat_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chat_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chunk_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chunk_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chunk_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chunk_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chunk_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chunk_query_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chunk_query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chunk_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/chunk_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/collection_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/collection_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/collection_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/collection_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/collection_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/collection_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/collection_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/message_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/message_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/message_generate_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/message_generate_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/message_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/message_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/message_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/message_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/message_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/record_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/record_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/record_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/record_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/record_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/record_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/record_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/text_embedding_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/models/schemas/text_embedding_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17738 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.839003 taskingai-0.2.1/taskingai/client/stream_apis/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/stream_apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/stream_apis/stream_api_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/stream_apis/stream_api_message_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.839003 taskingai-0.2.1/taskingai/inference/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/inference/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/inference/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.839003 taskingai-0.2.1/taskingai/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/retrieval/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/retrieval/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/retrieval/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/retrieval/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.839003 taskingai-0.2.1/taskingai/tool/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-03-13 12:56:46.000000 taskingai-0.2.1/taskingai/tool/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:59:07.839003 taskingai-0.2.1/taskingai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-03-13 12:59:07.000000 taskingai-0.2.1/taskingai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-03-13 12:59:07.000000 taskingai-0.2.1/taskingai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:59:07.000000 taskingai-0.2.1/taskingai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-13 12:59:07.000000 taskingai-0.2.1/taskingai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-13 12:59:07.000000 taskingai-0.2.1/taskingai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.416963 taskingai-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 13:14:19.000000 taskingai-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-26 13:17:36.416963 taskingai-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-26 13:14:19.000000 taskingai-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-26 13:14:19.000000 taskingai-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:17:36.416963 taskingai-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-26 13:14:19.000000 taskingai-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.388963 taskingai-0.2.2/taskingai/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.388963 taskingai-0.2.2/taskingai/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/assistant/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/assistant/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/assistant/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.392963 taskingai-0.2.2/taskingai/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22868 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.396963 taskingai-0.2.2/taskingai/client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_bulk_create_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_create_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_create_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_create_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_create_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_create_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_create_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_delete_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_delete_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_delete_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_delete_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_delete_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_delete_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_delete_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_generate_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_get_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_get_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_get_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_get_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_get_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_list_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_list_assistants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_list_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_list_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_list_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_list_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_list_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_query_collection_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_run_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_update_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_update_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_update_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_update_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_update_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_update_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/apis/api_update_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.396963 taskingai-0.2.2/taskingai/client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.404963 taskingai-0.2.2/taskingai/client/models/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/action_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/action_authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/action_body_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/action_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/action_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/assistant_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/assistant_memory_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_assistant_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_finish_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_function_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_function_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_function_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_function_parameters_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_system_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_completion_user_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chat_memory_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/file_id_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/message_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/message_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/message_generation_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/message_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/record_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/retrieval_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/retrieval_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/retrieval_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/retrieval_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/sort_order_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/text_embedding_input_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/text_embedding_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/text_splitter_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/tool_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/tool_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/entities/upload_file_purpose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.416963 taskingai-0.2.2/taskingai/client/models/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/action_bulk_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/action_bulk_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/action_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/action_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/action_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/action_run_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/action_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/action_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/action_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/assistant_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/assistant_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/assistant_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/assistant_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/assistant_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/assistant_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/assistant_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/base_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/base_empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chat_completion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chat_completion_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chat_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chat_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chat_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chat_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chat_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chat_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chat_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chunk_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chunk_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chunk_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chunk_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chunk_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chunk_query_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chunk_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chunk_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/chunk_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/collection_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/collection_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/collection_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/collection_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/collection_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/collection_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/collection_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/message_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/message_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/message_generate_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/message_generate_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/message_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/message_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/message_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/message_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/message_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/record_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/record_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/record_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/record_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/record_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/record_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/record_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/text_embedding_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/text_embedding_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/models/schemas/upload_file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19459 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.416963 taskingai-0.2.2/taskingai/client/stream_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/stream_apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/stream_apis/stream_api_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/stream_apis/stream_api_message_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.416963 taskingai-0.2.2/taskingai/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.416963 taskingai-0.2.2/taskingai/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/inference/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/inference/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.416963 taskingai-0.2.2/taskingai/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/retrieval/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/retrieval/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11072 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/retrieval/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/retrieval/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.416963 taskingai-0.2.2/taskingai/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-04-26 13:14:19.000000 taskingai-0.2.2/taskingai/tool/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:17:36.416963 taskingai-0.2.2/taskingai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-26 13:17:36.000000 taskingai-0.2.2/taskingai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-26 13:17:36.000000 taskingai-0.2.2/taskingai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:17:36.000000 taskingai-0.2.2/taskingai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-26 13:17:36.000000 taskingai-0.2.2/taskingai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 13:17:36.000000 taskingai-0.2.2/taskingai.egg-info/top_level.txt
```

### Comparing `taskingai-0.2.1/pyproject.toml` & `taskingai-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/setup.py` & `taskingai-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/assistant/assistant.py` & `taskingai-0.2.2/taskingai/assistant/assistant.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from typing import Optional, List, Dict
+from typing import Any, Optional, List, Dict, Union
 from taskingai.client.models import *
 from taskingai.client.apis import *
 
 __all__ = [
     "Assistant",
     "AssistantTool",
     "AssistantRetrieval",
     "AssistantToolType",
+    "ToolRef",
+    "ToolType",
+    "RetrievalRef",
+    "RetrievalType",
+    "RetrievalConfig",
+    "RetrievalMethod",
     "AssistantRetrievalType",
     "get_assistant",
     "list_assistants",
     "create_assistant",
     "update_assistant",
     "delete_assistant",
     "a_get_assistant",
@@ -23,15 +29,38 @@
 AssistantTool = ToolRef
 AssistantRetrieval = RetrievalRef
 AssistantToolType = ToolType
 AssistantRetrievalType = RetrievalType
 DEFAULT_RETRIEVAL_CONFIG = RetrievalConfig(top_k=3, method=RetrievalMethod.USER_MESSAGE)
 
 
+def _get_assistant_dict_params(
+    memory: Optional[Union[AssistantMemory, Dict[str, Any]]] = None,
+    tools: Optional[List[Union[AssistantTool, Dict[str, Any]]]] = None,
+    retrievals: Optional[List[Union[AssistantRetrieval, Dict[str, Any]]]] = None,
+    retrieval_configs: Optional[Union[RetrievalConfig, Dict[str, Any]]] = None,
+):
+    memory = memory if isinstance(memory, AssistantMemory) else (AssistantMemory(**memory) if memory else None)
+    tools = [tool if isinstance(tool, AssistantTool) else AssistantTool(**tool) for tool in (tools or [])] or None
+    retrievals = [
+        retrieval if isinstance(retrieval, AssistantRetrieval) else AssistantRetrieval(**retrieval)
+        for retrieval in (retrievals or [])
+    ] or None
+    retrieval_configs = (
+        retrieval_configs
+        if isinstance(retrieval_configs, RetrievalConfig)
+        else RetrievalConfig(**retrieval_configs)
+        if retrieval_configs
+        else None
+    )
+    return memory, tools, retrievals, retrieval_configs
+
+
 def list_assistants(
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Assistant]:
     """
     List assistants.
@@ -55,21 +84,22 @@
     )
     response: AssistantListResponse = api_list_assistants(payload)
     assistants: List[Assistant] = response.data
     return assistants
 
 
 async def a_list_assistants(
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Assistant]:
     """
-    List assistants.
+    List assistants in async mode.
 
     :param order: The order of the assistants. It can be "asc" or "desc".
     :param limit: The maximum number of assistants to return.
     :param after: The cursor to get the next page of assistants.
     :param before: The cursor to get the previous page of assistants.
     :return: The list of assistants.
     """
@@ -107,37 +137,42 @@
     """
 
     response: AssistantGetResponse = await async_api_get_assistant(assistant_id=assistant_id)
     return response.data
 
 
 def create_assistant(
+    *,
     model_id: str,
-    memory: AssistantMemory,
+    memory: Union[AssistantMemory, Dict[str, Any]],
     name: Optional[str] = None,
     description: Optional[str] = None,
     system_prompt_template: Optional[List[str]] = None,
-    tools: Optional[List[AssistantTool]] = None,
-    retrievals: Optional[List[AssistantRetrieval]] = None,
-    retrieval_configs: Optional[RetrievalConfig] = None,
+    tools: Optional[List[Union[AssistantTool, Dict[str, Any]]]] = None,
+    retrievals: Optional[List[Union[AssistantRetrieval, Dict[str, Any]]]] = None,
+    retrieval_configs: Optional[Union[RetrievalConfig, Dict[str, Any]]] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Assistant:
     """
     Create an assistant.
 
     :param model_id: The ID of an available chat completion model in your project.
     :param memory: The assistant memory.
     :param name: The assistant name.
     :param description: The assistant description.
     :param system_prompt_template: A list of system prompt chunks where prompt variables are wrapped by curly brackets, e.g. {{variable}}.
     :param tools: The assistant tools.
     :param retrievals: The assistant retrievals.
+    :param retrieval_configs: The assistant retrieval configurations.
     :param metadata: The assistant metadata. It can store up to 16 key-value pairs where each key's length is less than 64 and value's length is less than 512.
     :return: The created assistant object.
     """
+    memory, tools, retrievals, retrieval_configs = _get_assistant_dict_params(
+        memory=memory, tools=tools, retrievals=retrievals, retrieval_configs=retrieval_configs
+    )
 
     body = AssistantCreateRequest(
         model_id=model_id,
         name=name or "",
         description=description or "",
         memory=memory,
         system_prompt_template=system_prompt_template or [],
@@ -147,37 +182,42 @@
         metadata=metadata or {},
     )
     response: AssistantCreateResponse = api_create_assistant(payload=body)
     return response.data
 
 
 async def a_create_assistant(
+    *,
     model_id: str,
-    memory: AssistantMemory,
+    memory: Union[AssistantMemory, Dict[str, Any]],
     name: Optional[str] = None,
     description: Optional[str] = None,
     system_prompt_template: Optional[List[str]] = None,
-    tools: Optional[List[AssistantTool]] = None,
-    retrievals: Optional[List[AssistantRetrieval]] = None,
-    retrieval_configs: Optional[RetrievalConfig] = None,
+    tools: Optional[List[Union[AssistantTool, Dict[str, Any]]]] = None,
+    retrievals: Optional[List[Union[AssistantRetrieval, Dict[str, Any]]]] = None,
+    retrieval_configs: Optional[Union[RetrievalConfig, Dict[str, Any]]] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Assistant:
     """
     Create an assistant in async mode.
 
     :param model_id: The ID of an available chat completion model in your project.
     :param memory: The assistant memory.
     :param name: The assistant name.
     :param description: The assistant description.
     :param system_prompt_template: A list of system prompt chunks where prompt variables are wrapped by curly brackets, e.g. {{variable}}.
     :param tools: The assistant tools.
     :param retrievals: The assistant retrievals.
+    :param retrieval_configs: The assistant retrieval configurations.
     :param metadata: The assistant metadata. It can store up to 16 key-value pairs where each key's length is less than 64 and value's length is less than 512.
     :return: The created assistant object.
     """
+    memory, tools, retrievals, retrieval_configs = _get_assistant_dict_params(
+        memory=memory, tools=tools, retrievals=retrievals, retrieval_configs=retrieval_configs
+    )
 
     body = AssistantCreateRequest(
         model_id=model_id,
         name=name or "",
         description=description or "",
         memory=memory,
         system_prompt_template=system_prompt_template or [],
@@ -188,39 +228,45 @@
     )
     response: AssistantCreateResponse = await async_api_create_assistant(payload=body)
     return response.data
 
 
 def update_assistant(
     assistant_id: str,
+    *,
     model_id: Optional[str] = None,
     name: Optional[str] = None,
     description: Optional[str] = None,
     system_prompt_template: Optional[List[str]] = None,
-    memory: Optional[AssistantMemory] = None,
-    tools: Optional[List[AssistantTool]] = None,
-    retrievals: Optional[List[AssistantRetrieval]] = None,
-    retrieval_configs: Optional[RetrievalConfig] = None,
+    memory: Optional[Union[AssistantMemory, Dict[str, Any]]] = None,
+    tools: Optional[List[Union[AssistantTool, Dict[str, Any]]]] = None,
+    retrievals: Optional[List[Union[AssistantRetrieval, Dict[str, Any]]]] = None,
+    retrieval_configs: Optional[Union[RetrievalConfig, Dict[str, Any]]] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Assistant:
     """
     Update an assistant.
 
     :param assistant_id: The ID of the assistant.
     :param model_id: The ID of an available chat completion model in your project.
     :param name: The assistant name.
     :param description: The assistant description.
     :param system_prompt_template: A list of system prompt chunks where prompt variables are wrapped by curly brackets, e.g. {{variable}}.
     :param memory: The assistant memory.
     :param tools: The assistant tools.
     :param retrievals: The assistant retrievals.
+    :param retrieval_configs: The assistant retrieval configurations.
     :param metadata: The assistant metadata. It can store up to 16 key-value pairs where each key's length is less than 64 and value's length is less than 512.
     :return: The updated assistant object.
     """
 
+    memory, tools, retrievals, retrieval_configs = _get_assistant_dict_params(
+        memory=memory, tools=tools, retrievals=retrievals, retrieval_configs=retrieval_configs
+    )
+
     body = AssistantUpdateRequest(
         model_id=model_id,
         name=name,
         description=description,
         memory=memory,
         system_prompt_template=system_prompt_template,
         tools=tools,
@@ -230,39 +276,45 @@
     )
     response: AssistantUpdateResponse = api_update_assistant(assistant_id=assistant_id, payload=body)
     return response.data
 
 
 async def a_update_assistant(
     assistant_id: str,
+    *,
     model_id: Optional[str] = None,
     name: Optional[str] = None,
     description: Optional[str] = None,
     system_prompt_template: Optional[List[str]] = None,
-    memory: Optional[AssistantMemory] = None,
-    tools: Optional[List[AssistantTool]] = None,
-    retrievals: Optional[List[AssistantRetrieval]] = None,
-    retrieval_configs: Optional[RetrievalConfig] = None,
+    memory: Optional[Union[AssistantMemory, Dict[str, Any]]] = None,
+    tools: Optional[List[Union[AssistantTool, Dict[str, Any]]]] = None,
+    retrievals: Optional[List[Union[AssistantRetrieval, Dict[str, Any]]]] = None,
+    retrieval_configs: Optional[Union[RetrievalConfig, Dict[str, Any]]] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Assistant:
     """
     Update an assistant in async mode.
 
     :param assistant_id: The ID of the assistant.
     :param model_id: The ID of an available chat completion model in your project.
     :param name: The assistant name.
     :param description: The assistant description.
     :param system_prompt_template: A list of system prompt chunks where prompt variables are wrapped by curly brackets, e.g. {{variable}}.
     :param memory: The assistant memory.
     :param tools: The assistant tools.
     :param retrievals: The assistant retrievals.
+    :param retrieval_configs: The assistant retrieval configurations.
     :param metadata: The assistant metadata. It can store up to 16 key-value pairs where each key's length is less than 64 and value's length is less than 512.
     :return: The updated assistant object.
     """
 
+    memory, tools, retrievals, retrieval_configs = _get_assistant_dict_params(
+        memory=memory, tools=tools, retrievals=retrievals, retrieval_configs=retrieval_configs
+    )
+
     body = AssistantUpdateRequest(
         model_id=model_id,
         name=name,
         description=description,
         memory=memory,
         system_prompt_template=system_prompt_template,
         tools=tools,
```

### Comparing `taskingai-0.2.1/taskingai/assistant/chat.py` & `taskingai-0.2.2/taskingai/assistant/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "a_update_chat",
     "a_delete_chat",
 ]
 
 
 def list_chats(
     assistant_id: str,
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Chat]:
     """
     List chats.
@@ -49,14 +50,15 @@
         payload=payload,
     )
     return response.data
 
 
 async def a_list_chats(
     assistant_id: str,
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Chat]:
     """
     List chats in async mode.
@@ -112,86 +114,102 @@
         chat_id=chat_id,
     )
     return response.data
 
 
 def create_chat(
     assistant_id: str,
+    *,
+    name: Optional[str] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Chat:
     """
     Create a chat.
 
     :param assistant_id: The ID of the assistant.
+    :param name: The name of the chat.
     :param metadata: The chat metadata. It can store up to 16 key-value pairs where each key's length is less than 64 and value's length is less than 512.
     :return: The created chat object.
     """
 
     body = ChatCreateRequest(
+        name=name or "",
         metadata=metadata or {},
     )
     response: ChatCreateResponse = api_create_chat(assistant_id=assistant_id, payload=body)
     return response.data
 
 
 async def a_create_chat(
     assistant_id: str,
+    *,
+    name: Optional[str] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Chat:
     """
     Create a chat in async mode.
 
     :param assistant_id: The ID of the assistant.
+    :param name: The name of the chat.
     :param metadata: The chat metadata. It can store up to 16 key-value pairs where each key's length is less than 64 and value's length is less than 512.
     :return: The created chat object.
     """
 
     body = ChatCreateRequest(
+        name=name or "",
         metadata=metadata or {},
     )
     response: ChatCreateResponse = await async_api_create_chat(assistant_id=assistant_id, payload=body)
     return response.data
 
 
 def update_chat(
     assistant_id: str,
     chat_id: str,
-    metadata: Dict[str, str],
+    *,
+    name: Optional[str] = None,
+    metadata: Optional[Dict[str, str]] = None,
 ) -> Chat:
     """
     Update a chat.
 
     :param assistant_id: The ID of the assistant.
     :param chat_id: The ID of the chat.
+    :param name: The name of the chat.
     :param metadata: The assistant metadata. It can store up to 16 key-value pairs where each key's length is less than 64 and value's length is less than 512.
     :return: The updated chat object.
     """
 
     body = ChatUpdateRequest(
+        name=name,
         metadata=metadata,
     )
     response: ChatUpdateResponse = api_update_chat(assistant_id=assistant_id, chat_id=chat_id, payload=body)
     return response.data
 
 
 async def a_update_chat(
     assistant_id: str,
     chat_id: str,
-    metadata: Dict[str, str],
+    *,
+    name: Optional[str] = None,
+    metadata: Optional[Dict[str, str]] = None,
 ) -> Chat:
     """
     Update a chat in async mode.
 
     :param assistant_id: The ID of the assistant.
     :param chat_id: The ID of the chat.
+    :param name: The name of the chat.
     :param metadata: The assistant metadata. It can store up to 16 key-value pairs where each key's length is less than 64 and value's length is less than 512.
     :return: The updated chat object.
     """
 
     body = ChatUpdateRequest(
+        name=name,
         metadata=metadata,
     )
     response: ChatUpdateResponse = await async_api_update_chat(assistant_id=assistant_id, chat_id=chat_id, payload=body)
     return response.data
 
 
 def delete_chat(
```

### Comparing `taskingai-0.2.1/taskingai/assistant/memory.py` & `taskingai-0.2.2/taskingai/assistant/memory.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/assistant/message.py` & `taskingai-0.2.2/taskingai/assistant/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "a_generate_message",
 ]
 
 
 def list_messages(
     assistant_id: str,
     chat_id: str,
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Message]:
     """
     List messages.
@@ -57,14 +58,15 @@
     )
     return response.data
 
 
 async def a_list_messages(
     assistant_id: str,
     chat_id: str,
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Message]:
     """
     List messages in async mode.
@@ -128,14 +130,15 @@
     )
     return response.data
 
 
 def create_message(
     assistant_id: str,
     chat_id: str,
+    *,
     text: str,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Message:
     """
     Create a message.
 
     :param assistant_id: The ID of the assistant.
@@ -153,14 +156,15 @@
     response: MessageCreateResponse = api_create_message(assistant_id=assistant_id, chat_id=chat_id, payload=body)
     return response.data
 
 
 async def a_create_message(
     assistant_id: str,
     chat_id: str,
+    *,
     text: str,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Message:
     """
     Create a message in async mode.
 
     :param assistant_id: The ID of the assistant.
@@ -181,20 +185,22 @@
     return response.data
 
 
 def update_message(
     assistant_id: str,
     chat_id: str,
     message_id: str,
+    *,
     metadata: Dict[str, str],
 ) -> Message:
     """
     Update a message.
 
     :param assistant_id: The ID of the assistant.
+    :param chat_id: The ID of the chat.
     :param message_id: The ID of the message.
     :param metadata: The assistant metadata. It can store up to 16 key-value pairs where each key's length is less than 64 and value's length is less than 512.
     :return: The updated message object.
     """
 
     body = MessageUpdateRequest(
         metadata=metadata or {},
@@ -205,20 +211,22 @@
     return response.data
 
 
 async def a_update_message(
     assistant_id: str,
     chat_id: str,
     message_id: str,
+    *,
     metadata: Dict[str, str],
 ) -> Message:
     """
     Update a message in async mode.
 
     :param assistant_id: The ID of the assistant.
+    :param chat_id: The ID of the chat.
     :param message_id: The ID of the message.
     :param metadata: The assistant metadata. It can store up to 16 key-value pairs where each key's length is less than 64 and value's length is less than 512.
     :return: The updated message object.
     """
 
     body = MessageUpdateRequest(
         metadata=metadata or {},
@@ -228,14 +236,15 @@
     )
     return response.data
 
 
 def generate_message(
     assistant_id: str,
     chat_id: str,
+    *,
     system_prompt_variables: Optional[Dict] = None,
     stream: bool = False,
 ) -> Union[Message, Stream]:
     """
     Generate a message.
 
     :param assistant_id: The ID of the assistant.
@@ -263,14 +272,15 @@
         )
         return response
 
 
 async def a_generate_message(
     assistant_id: str,
     chat_id: str,
+    *,
     system_prompt_variables: Optional[Dict] = None,
     stream: bool = False,
 ) -> Union[Message, AsyncStream]:
     """
     Generate a message in async mode.
 
     :param assistant_id: The ID of the assistant.
```

### Comparing `taskingai-0.2.1/taskingai/client/api_client.py` & `taskingai-0.2.2/taskingai/client/api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
     OpenAPI spec version: 0.1.0
 """
 from __future__ import absolute_import
 
 import datetime
 import json
-import mimetypes
 import os
 import re
 import tempfile
 from typing import Type
 
 # python 2 and python 3 compatibility library
 import six
@@ -97,40 +96,14 @@
         try:
             data = json.loads(response.data)
         except ValueError:
             data = response.data
 
         return response_type(**data)
 
-    def prepare_post_parameters(self, post_params=None, files=None):
-        """Builds form parameters.
-
-        :param post_params: Normal form parameters.
-        :param files: File parameters.
-        :return: Form parameters with files.
-        """
-        params = []
-
-        if post_params:
-            params = post_params
-
-        if files:
-            for k, v in six.iteritems(files):
-                if not v:
-                    continue
-                file_names = v if type(v) is list else [v]
-                for n in file_names:
-                    with open(n, "rb") as f:
-                        filename = os.path.basename(f.name)
-                        filedata = f.read()
-                        mimetype = mimetypes.guess_type(filename)[0] or "application/octet-stream"
-                        params.append(tuple([k, tuple([filename, filedata, mimetype])]))
-
-        return params
-
     def select_header_accept(self, accepts):
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
         :return: Accept (e.g. application/json).
         """
         if not accepts:
@@ -248,18 +221,14 @@
 
         # path parameters
         if path_params:
             for k, v in path_params.items():
                 # specified safe chars, encode everything
                 resource_path = resource_path.replace("{%s}" % k, quote(str(v), safe=config.safe_chars_for_path_param))
 
-        # post parameters
-        if post_params or files:
-            post_params = self.prepare_post_parameters(post_params, files)
-
         # auth setting
         self.update_params_for_auth(header_params, query_params, auth_settings)
 
         # body
 
         # request url
         url = self.configuration.host + resource_path
@@ -268,14 +237,15 @@
         response_data = self.request(
             method,
             url,
             stream=stream,
             query_params=query_params,
             headers=header_params,
             post_params=post_params,
+            files=files,
             body=body,
             _preload_content=_preload_content,
             _request_timeout=_request_timeout,
         )
 
         if stream:
             return response_data
@@ -363,14 +333,15 @@
         self,
         method,
         url,
         stream=False,
         query_params=None,
         headers=None,
         post_params=None,
+        files=None,
         body=None,
         _preload_content=True,
         _request_timeout=None,
     ):
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
             return self.rest_client.GET(
@@ -404,36 +375,39 @@
         elif method == "POST":
             return self.rest_client.POST(
                 url,
                 stream=stream,
                 query_params=query_params,
                 headers=headers,
                 post_params=post_params,
+                files=files,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout,
                 body=body,
             )
         elif method == "PUT":
             return self.rest_client.PUT(
                 url,
                 stream=stream,
                 query_params=query_params,
                 headers=headers,
                 post_params=post_params,
+                files=files,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout,
                 body=body,
             )
         elif method == "PATCH":
             return self.rest_client.PATCH(
                 url,
                 stream=stream,
                 query_params=query_params,
                 headers=headers,
                 post_params=post_params,
+                files=files,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout,
                 body=body,
             )
         elif method == "DELETE":
             return self.rest_client.DELETE(
                 url,
@@ -485,18 +459,14 @@
 
         # path parameters
         if path_params:
             for k, v in path_params.items():
                 # specified safe chars, encode everything
                 resource_path = resource_path.replace("{%s}" % k, quote(str(v), safe=config.safe_chars_for_path_param))
 
-        # post parameters
-        if post_params or files:
-            post_params = self.prepare_post_parameters(post_params, files)
-
         # auth setting
         self.update_params_for_auth(header_params, query_params, auth_settings)
 
         # body
 
         # request url
         url = self.configuration.host + resource_path
@@ -505,14 +475,15 @@
         response_data = await self.request(
             method,
             url,
             stream=stream,
             query_params=query_params,
             headers=header_params,
             post_params=post_params,
+            files=files,
             body=body,
             _preload_content=_preload_content,
             _request_timeout=_request_timeout,
         )
 
         if stream:
             return response_data
@@ -597,14 +568,15 @@
         self,
         method,
         url,
         stream,
         query_params=None,
         headers=None,
         post_params=None,
+        files=None,
         body=None,
         _preload_content=True,
         _request_timeout=None,
     ):
         """Makes the HTTP request using the asynchronous RESTClient."""
         if method == "GET":
             return await self.rest_client.GET(
@@ -638,36 +610,39 @@
         elif method == "POST":
             return await self.rest_client.POST(
                 url,
                 stream=stream,
                 query_params=query_params,
                 headers=headers,
                 post_params=post_params,
+                files=files,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout,
                 body=body,
             )
         elif method == "PUT":
             return await self.rest_client.PUT(
                 url,
                 stream=stream,
                 query_params=query_params,
                 headers=headers,
                 post_params=post_params,
+                files=files,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout,
                 body=body,
             )
         elif method == "PATCH":
             return await self.rest_client.PATCH(
                 url,
                 stream=stream,
                 query_params=query_params,
                 headers=headers,
                 post_params=post_params,
+                files=files,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout,
                 body=body,
             )
         elif method == "DELETE":
             return await self.rest_client.DELETE(
                 url,
```

### Comparing `taskingai-0.2.1/taskingai/client/apis/__init__.py` & `taskingai-0.2.2/taskingai/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_bulk_create_actions.py` & `taskingai-0.2.2/taskingai/client/apis/api_bulk_create_actions.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_chat_completion.py` & `taskingai-0.2.2/taskingai/client/apis/api_chat_completion.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_create_assistant.py` & `taskingai-0.2.2/taskingai/client/apis/api_create_assistant.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_create_chat.py` & `taskingai-0.2.2/taskingai/client/apis/api_create_chat.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_create_chunk.py` & `taskingai-0.2.2/taskingai/client/apis/api_create_chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_create_collection.py` & `taskingai-0.2.2/taskingai/client/apis/api_create_collection.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_create_message.py` & `taskingai-0.2.2/taskingai/client/apis/api_create_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_create_record.py` & `taskingai-0.2.2/taskingai/client/apis/api_create_record.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_delete_action.py` & `taskingai-0.2.2/taskingai/client/apis/api_delete_action.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_delete_assistant.py` & `taskingai-0.2.2/taskingai/client/apis/api_delete_assistant.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_delete_chat.py` & `taskingai-0.2.2/taskingai/client/apis/api_delete_chat.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_delete_chunk.py` & `taskingai-0.2.2/taskingai/client/apis/api_delete_chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_delete_collection.py` & `taskingai-0.2.2/taskingai/client/apis/api_delete_collection.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_delete_message.py` & `taskingai-0.2.2/taskingai/client/apis/api_delete_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_delete_record.py` & `taskingai-0.2.2/taskingai/client/apis/api_delete_record.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_generate_message.py` & `taskingai-0.2.2/taskingai/client/apis/api_generate_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_get_action.py` & `taskingai-0.2.2/taskingai/client/apis/api_get_action.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_get_assistant.py` & `taskingai-0.2.2/taskingai/client/apis/api_get_assistant.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_get_chat.py` & `taskingai-0.2.2/taskingai/client/apis/api_get_chat.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_get_chunk.py` & `taskingai-0.2.2/taskingai/client/apis/api_get_chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_get_collection.py` & `taskingai-0.2.2/taskingai/client/apis/api_get_collection.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_get_message.py` & `taskingai-0.2.2/taskingai/client/apis/api_get_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_get_record.py` & `taskingai-0.2.2/taskingai/client/apis/api_get_record.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_list_actions.py` & `taskingai-0.2.2/taskingai/client/apis/api_list_actions.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_list_assistants.py` & `taskingai-0.2.2/taskingai/client/apis/api_list_assistants.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_list_chats.py` & `taskingai-0.2.2/taskingai/client/apis/api_list_chats.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_list_chunks.py` & `taskingai-0.2.2/taskingai/client/apis/api_list_chunks.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_list_collections.py` & `taskingai-0.2.2/taskingai/client/apis/api_list_collections.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_list_messages.py` & `taskingai-0.2.2/taskingai/client/apis/api_list_messages.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_list_records.py` & `taskingai-0.2.2/taskingai/client/apis/api_list_records.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_query_collection_chunks.py` & `taskingai-0.2.2/taskingai/client/apis/api_query_collection_chunks.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_run_action.py` & `taskingai-0.2.2/taskingai/client/apis/api_run_action.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_text_embedding.py` & `taskingai-0.2.2/taskingai/client/apis/api_text_embedding.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_update_action.py` & `taskingai-0.2.2/taskingai/client/apis/api_update_action.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_update_assistant.py` & `taskingai-0.2.2/taskingai/client/apis/api_update_assistant.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_update_chat.py` & `taskingai-0.2.2/taskingai/client/apis/api_update_chat.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_update_chunk.py` & `taskingai-0.2.2/taskingai/client/apis/api_update_chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_update_collection.py` & `taskingai-0.2.2/taskingai/client/apis/api_update_collection.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_update_message.py` & `taskingai-0.2.2/taskingai/client/apis/api_update_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/apis/api_update_record.py` & `taskingai-0.2.2/taskingai/client/apis/api_update_record.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/configuration.py` & `taskingai-0.2.2/taskingai/client/configuration.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/error_handling.py` & `taskingai-0.2.2/taskingai/client/error_handling.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/exceptions.py` & `taskingai-0.2.2/taskingai/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/__init__.py` & `taskingai-0.2.2/taskingai/client/models/entities/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from .chat_completion_role import *
 from .chat_completion_system_message import *
 from .chat_completion_user_message import *
 from .chat_memory import *
 from .chat_memory_message import *
 from .chunk import *
 from .collection import *
+from .file_id_data import *
 from .message import *
 from .message_chunk import *
 from .message_content import *
 from .message_generation_log import *
 from .message_role import *
 from .record import *
 from .record_type import *
@@ -53,7 +54,8 @@
 from .status import *
 from .text_embedding_input_type import *
 from .text_embedding_output import *
 from .text_splitter import *
 from .text_splitter_type import *
 from .tool_ref import *
 from .tool_type import *
+from .upload_file_purpose import *
```

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/action.py` & `taskingai-0.2.2/taskingai/client/models/entities/action.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,16 +27,12 @@
 class Action(BaseModel):
     action_id: str = Field(..., min_length=20, max_length=30)
     name: str = Field(..., min_length=1, max_length=128)
     operation_id: str = Field(...)
     description: str = Field(..., min_length=1, max_length=512)
     url: str = Field(...)
     method: ActionMethod = Field(...)
-    path_param_schema: Optional[Dict[str, ActionParam]] = Field(None)
-    query_param_schema: Optional[Dict[str, ActionParam]] = Field(None)
     body_type: ActionBodyType = Field(...)
-    body_param_schema: Optional[Dict[str, ActionParam]] = Field(None)
-    function_def: ChatCompletionFunction = Field(...)
     openapi_schema: Dict[str, Any] = Field(...)
     authentication: ActionAuthentication = Field(...)
     updated_timestamp: int = Field(..., ge=0)
     created_timestamp: int = Field(..., ge=0)
```

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/action_authentication.py` & `taskingai-0.2.2/taskingai/client/models/entities/action_authentication.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/assistant.py` & `taskingai-0.2.2/taskingai/client/models/entities/assistant.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/assistant_memory.py` & `taskingai-0.2.2/taskingai/client/models/entities/assistant_memory.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chat.py` & `taskingai-0.2.2/taskingai/client/models/entities/chat.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,10 +17,11 @@
 
 __all__ = ["Chat"]
 
 
 class Chat(BaseModel):
     chat_id: str = Field(..., min_length=20, max_length=30)
     assistant_id: str = Field(..., min_length=20, max_length=30)
+    name: str = Field("", min_length=0, max_length=127)
     metadata: Dict[str, str] = Field({}, min_length=0, max_length=16)
     updated_timestamp: int = Field(..., ge=0)
     created_timestamp: int = Field(..., ge=0)
```

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chat_completion.py` & `taskingai-0.2.2/taskingai/client/models/entities/chat_completion.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chat_completion_assistant_message.py` & `taskingai-0.2.2/taskingai/client/models/entities/chat_completion_assistant_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chat_completion_chunk.py` & `taskingai-0.2.2/taskingai/client/models/entities/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chat_completion_function.py` & `taskingai-0.2.2/taskingai/client/models/entities/chat_completion_function.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chat_completion_function_message.py` & `taskingai-0.2.2/taskingai/client/models/entities/chat_completion_function_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chat_completion_function_parameters.py` & `taskingai-0.2.2/taskingai/client/models/entities/chat_completion_function_parameters.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chat_completion_function_parameters_property.py` & `taskingai-0.2.2/taskingai/client/models/entities/chat_completion_function_parameters_property.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chat_completion_system_message.py` & `taskingai-0.2.2/taskingai/client/models/entities/chat_completion_system_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chat_completion_user_message.py` & `taskingai-0.2.2/taskingai/client/models/entities/chat_completion_user_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chat_memory.py` & `taskingai-0.2.2/taskingai/client/models/entities/chat_memory.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/chunk.py` & `taskingai-0.2.2/taskingai/client/models/entities/chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/collection.py` & `taskingai-0.2.2/taskingai/client/models/entities/collection.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/message.py` & `taskingai-0.2.2/taskingai/client/models/entities/message.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 
 Author: James Yao
 Organization: TaskingAI
 License: Apache 2.0
 """
 
 from pydantic import BaseModel, Field
-from typing import Dict
+from typing import List, Dict
 from .message_content import MessageContent
 
 __all__ = ["Message"]
 
 
 class Message(BaseModel):
     message_id: str = Field(..., min_length=20, max_length=30)
     chat_id: str = Field(..., min_length=20, max_length=30)
     assistant_id: str = Field(None, min_length=20, max_length=30)
     role: str = Field(..., min_length=1, max_length=20)
     content: MessageContent = Field(...)
     metadata: Dict[str, str] = Field({}, min_length=0, max_length=16)
+    logs: List[Dict] = Field([])
     updated_timestamp: int = Field(..., ge=0)
     created_timestamp: int = Field(..., ge=0)
```

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/message_generation_log.py` & `taskingai-0.2.2/taskingai/client/models/entities/message_generation_log.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/record.py` & `taskingai-0.2.2/taskingai/client/models/entities/record.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/retrieval_config.py` & `taskingai-0.2.2/taskingai/client/models/entities/retrieval_config.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/entities/text_splitter.py` & `taskingai-0.2.2/taskingai/client/models/entities/text_splitter.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/__init__.py` & `taskingai-0.2.2/taskingai/client/models/schemas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,7 +68,8 @@
 from .record_get_response import *
 from .record_list_request import *
 from .record_list_response import *
 from .record_update_request import *
 from .record_update_response import *
 from .text_embedding_request import *
 from .text_embedding_response import *
+from .upload_file_response import *
```

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/action_bulk_create_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/action_bulk_create_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/action_list_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/action_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/action_list_response.py` & `taskingai-0.2.2/taskingai/client/models/schemas/action_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/action_update_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/action_update_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/assistant_create_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/assistant_create_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/assistant_list_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/assistant_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/assistant_list_response.py` & `taskingai-0.2.2/taskingai/client/models/schemas/assistant_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/assistant_update_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/assistant_update_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/chat_completion_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/chat_completion_request.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 Author: James Yao
 Organization: TaskingAI
 License: Apache 2.0
 """
 
 from pydantic import BaseModel, Field
 from typing import Optional, List, Dict, Union
-from ..entities.chat_completion_assistant_message import ChatCompletionAssistantMessage
+from ..entities.chat_completion_function_message import ChatCompletionFunctionMessage
 from ..entities.chat_completion_system_message import ChatCompletionSystemMessage
 from ..entities.chat_completion_user_message import ChatCompletionUserMessage
-from ..entities.chat_completion_function_message import ChatCompletionFunctionMessage
+from ..entities.chat_completion_assistant_message import ChatCompletionAssistantMessage
 from ..entities.chat_completion_function import ChatCompletionFunction
 
 __all__ = ["ChatCompletionRequest"]
 
 
 class ChatCompletionRequest(BaseModel):
     model_id: str = Field(..., min_length=8, max_length=8)
```

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/chat_list_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/chat_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/chat_list_response.py` & `taskingai-0.2.2/taskingai/client/models/schemas/chat_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/chunk_list_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/chunk_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/chunk_list_response.py` & `taskingai-0.2.2/taskingai/client/models/schemas/chunk_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/chunk_query_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/chunk_query_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/collection_create_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/collection_create_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/collection_list_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/collection_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/collection_list_response.py` & `taskingai-0.2.2/taskingai/client/models/schemas/collection_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/collection_update_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/collection_update_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/message_create_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/message_create_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/message_generate_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/message_generate_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/message_list_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/message_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/message_list_response.py` & `taskingai-0.2.2/taskingai/client/models/schemas/message_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/record_create_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/record_create_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 
 Author: James Yao
 Organization: TaskingAI
 License: Apache 2.0
 """
 
 from pydantic import BaseModel, Field
-from typing import Dict
+from typing import Optional, Dict
 from ..entities.record_type import RecordType
 from ..entities.text_splitter import TextSplitter
 
 __all__ = ["RecordCreateRequest"]
 
 
 class RecordCreateRequest(BaseModel):
     type: RecordType = Field("text")
+    file_id: Optional[str] = Field(None, min_length=1, max_length=256)
+    url: Optional[str] = Field(None, min_length=1, max_length=2048)
     title: str = Field("", min_length=0, max_length=256)
-    content: str = Field(..., min_length=1, max_length=32768)
+    content: Optional[str] = Field(None, min_length=1, max_length=32768)
     text_splitter: TextSplitter = Field(...)
     metadata: Dict[str, str] = Field({}, min_length=0, max_length=16)
```

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/record_list_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/record_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/record_list_response.py` & `taskingai-0.2.2/taskingai/client/models/schemas/record_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/record_update_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/record_update_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,11 +17,13 @@
 from ..entities.text_splitter import TextSplitter
 
 __all__ = ["RecordUpdateRequest"]
 
 
 class RecordUpdateRequest(BaseModel):
     type: Optional[RecordType] = Field(None)
+    file_id: Optional[str] = Field(None, min_length=1, max_length=256)
+    url: Optional[str] = Field(None, min_length=1, max_length=2048)
     title: Optional[str] = Field(None, min_length=0, max_length=256)
     content: Optional[str] = Field(None, min_length=1, max_length=32768)
     text_splitter: Optional[TextSplitter] = Field(None)
     metadata: Optional[Dict[str, str]] = Field(None, min_length=0, max_length=16)
```

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/text_embedding_request.py` & `taskingai-0.2.2/taskingai/client/models/schemas/text_embedding_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/models/schemas/text_embedding_response.py` & `taskingai-0.2.2/taskingai/client/models/schemas/text_embedding_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/stream.py` & `taskingai-0.2.2/taskingai/client/stream.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/stream_apis/stream_api_chat_completion.py` & `taskingai-0.2.2/taskingai/client/stream_apis/stream_api_chat_completion.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/stream_apis/stream_api_message_generation.py` & `taskingai-0.2.2/taskingai/client/stream_apis/stream_api_message_generation.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/client/utils.py` & `taskingai-0.2.2/taskingai/client/utils.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/config.py` & `taskingai-0.2.2/taskingai/config.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/exceptions.py` & `taskingai-0.2.2/taskingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/inference/text_embedding.py` & `taskingai-0.2.2/taskingai/inference/text_embedding.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.1/taskingai/retrieval/chunk.py` & `taskingai-0.2.2/taskingai/retrieval/chunk.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     "query_chunks",
     "a_query_chunks",
 ]
 
 
 def list_chunks(
     collection_id: str,
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Chunk]:
     """
     List chunks.
@@ -50,14 +51,15 @@
     )
     response: ChunkListResponse = api_list_chunks(collection_id=collection_id, payload=payload)
     return response.data
 
 
 async def a_list_chunks(
     collection_id: str,
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Chunk]:
     """
     List chunks in async mode.
@@ -111,14 +113,15 @@
         chunk_id=chunk_id,
     )
     return response.data
 
 
 def create_chunk(
     collection_id: str,
+    *,
     content: str,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Chunk:
     """
     Create a chunk.
 
     :param collection_id: The ID of the collection.
@@ -133,14 +136,15 @@
     )
     response: ChunkCreateResponse = api_create_chunk(collection_id=collection_id, payload=body)
     return response.data
 
 
 async def a_create_chunk(
     collection_id: str,
+    *,
     content: str,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Chunk:
     """
     Create a chunk in async mode.
 
     :param collection_id: The ID of the collection.
@@ -156,14 +160,15 @@
     response: ChunkCreateResponse = await async_api_create_chunk(collection_id=collection_id, payload=body)
     return response.data
 
 
 def update_chunk(
     collection_id: str,
     chunk_id: str,
+    *,
     content: Optional[str] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Chunk:
     """
     Update a chunk.
 
     :param collection_id: The ID of the collection.
@@ -181,14 +186,15 @@
     response: ChunkUpdateResponse = api_update_chunk(collection_id=collection_id, chunk_id=chunk_id, payload=body)
     return response.data
 
 
 async def a_update_chunk(
     collection_id: str,
     chunk_id: str,
+    *,
     content: Optional[str] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Chunk:
     """
     Update a chunk in async mode.
 
     :param collection_id: The ID of the collection.
@@ -235,14 +241,15 @@
     """
 
     await async_api_delete_chunk(collection_id=collection_id, chunk_id=chunk_id)
 
 
 def query_chunks(
     collection_id: str,
+    *,
     query_text: str,
     top_k: int = 3,
     max_tokens: Optional[int] = None,
 ) -> List[Chunk]:
     """
     Query chunks in a collection.
     :param collection_id: The ID of the collection.
@@ -262,14 +269,15 @@
         payload=body,
     )
     return response.data
 
 
 async def a_query_chunks(
     collection_id: str,
+    *,
     query_text: str,
     top_k: int = 3,
     max_tokens: Optional[int] = None,
 ) -> List[Chunk]:
     """
     Query chunks in a collection.
     :param collection_id: The ID of the collection.
```

### Comparing `taskingai-0.2.1/taskingai/retrieval/collection.py` & `taskingai-0.2.2/taskingai/retrieval/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "a_create_collection",
     "a_update_collection",
     "a_delete_collection",
 ]
 
 
 def list_collections(
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Collection]:
     """
     List collections.
@@ -45,14 +46,15 @@
         before=before,
     )
     response: CollectionListResponse = api_list_collections(payload=payload)
     return response.data
 
 
 async def a_list_collections(
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Collection]:
     """
     List collections.
@@ -97,14 +99,15 @@
     """
 
     response: CollectionGetResponse = await async_api_get_collection(collection_id=collection_id)
     return response.data
 
 
 def create_collection(
+    *,
     embedding_model_id: str,
     capacity: int = 1000,
     name: Optional[str] = None,
     description: Optional[str] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Collection:
     """
@@ -126,14 +129,15 @@
         metadata=metadata or {},
     )
     response: CollectionCreateResponse = api_create_collection(payload=body)
     return response.data
 
 
 async def a_create_collection(
+    *,
     embedding_model_id: str,
     capacity: int = 1000,
     name: Optional[str] = None,
     description: Optional[str] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Collection:
     """
@@ -157,14 +161,15 @@
     )
     response: CollectionCreateResponse = await async_api_create_collection(payload=body)
     return response.data
 
 
 def update_collection(
     collection_id: str,
+    *,
     name: Optional[str] = None,
     description: Optional[str] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Collection:
     """
     Update a collection.
 
@@ -181,14 +186,15 @@
     )
     response: CollectionUpdateResponse = api_update_collection(collection_id=collection_id, payload=body)
     return response.data
 
 
 async def a_update_collection(
     collection_id: str,
+    *,
     name: Optional[str] = None,
     description: Optional[str] = None,
     metadata: Optional[Dict[str, str]] = None,
 ) -> Collection:
     """
     Update a collection in async mode.
```

### Comparing `taskingai-0.2.1/taskingai/tool/action.py` & `taskingai-0.2.2/taskingai/tool/action.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, List, Dict
+from typing import Any, Optional, List, Dict, Union
 
 from taskingai.client.models import *
 from taskingai.client.apis import *
 
 
 __all__ = [
     "Action",
@@ -20,14 +20,15 @@
     "a_update_action",
     "a_delete_action",
     "a_run_action",
 ]
 
 
 def list_actions(
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Action]:
     """
     List actions.
@@ -49,14 +50,15 @@
         before=before,
     )
     response: ActionListResponse = api_list_actions(payload=payload)
     return response.data
 
 
 async def a_list_actions(
+    *,
     order: str = "desc",
     limit: int = 20,
     after: Optional[str] = None,
     before: Optional[str] = None,
 ) -> List[Action]:
     """
     List actions in async mode.
@@ -100,95 +102,115 @@
     """
 
     response: ActionGetResponse = await async_api_get_action(action_id=action_id)
     return response.data
 
 
 def bulk_create_actions(
+    *,
     openapi_schema: Dict,
-    authentication: Optional[ActionAuthentication] = None,
+    authentication: Optional[Union[ActionAuthentication, Dict[str, Any]]] = None,
 ) -> List[Action]:
     """
     Create actions from an OpenAPI schema.
 
     :param openapi_schema: The action schema is compliant with the OpenAPI Specification. If there are multiple paths and methods in the openapi_schema, the service will create multiple actions whose openapi_schema only has exactly one path and one method
     :param authentication: The action API authentication.
     :return: The created action object.
     """
 
-    if authentication is None:
-        authentication = ActionAuthentication(
-            type=ActionAuthenticationType.NONE,
-        )
+    authentication = (
+        authentication
+        if isinstance(authentication, ActionAuthentication)
+        else ActionAuthentication(**(authentication or ActionAuthentication(type=ActionAuthenticationType.NONE)))
+    )
+
     body = ActionBulkCreateRequest(
         openapi_schema=openapi_schema,
         authentication=authentication,
     )
     response: ActionBulkCreateResponse = api_bulk_create_actions(payload=body)
     return response.data
 
 
 async def a_bulk_create_actions(
+    *,
     openapi_schema: Dict,
-    authentication: Optional[ActionAuthentication] = None,
+    authentication: Optional[Union[ActionAuthentication, Dict[str, Any]]] = None,
 ) -> List[Action]:
     """
     Create actions from an OpenAPI schema in async mode.
 
     :param openapi_schema: The action schema is compliant with the OpenAPI Specification. If there are multiple paths and methods in the openapi_schema, the service will create multiple actions whose openapi_schema only has exactly one path and one method
     :param authentication: The action API authentication.
     :return: The created action object.
     """
 
-    if authentication is None:
-        authentication = ActionAuthentication(
-            type=ActionAuthenticationType.NONE,
-        )
+    authentication = (
+        authentication
+        if isinstance(authentication, ActionAuthentication)
+        else ActionAuthentication(**(authentication or ActionAuthentication(type=ActionAuthenticationType.NONE)))
+    )
+
     body = ActionBulkCreateRequest(
         openapi_schema=openapi_schema,
         authentication=authentication,
     )
     response: ActionBulkCreateResponse = await async_api_bulk_create_actions(payload=body)
     return response.data
 
 
 def update_action(
     action_id: str,
+    *,
     openapi_schema: Optional[Dict] = None,
-    authentication: Optional[ActionAuthentication] = None,
+    authentication: Optional[Union[ActionAuthentication, Dict[str, Any]]] = None,
 ) -> Action:
     """
     Update an action.
 
     :param action_id: The ID of the action.
     :param openapi_schema: The action schema, which is compliant with the OpenAPI Specification. It should only have exactly one path and one method.
     :param authentication: The action API authentication.
     :return: The updated action object.
     """
+    if authentication:
+        authentication = (
+            authentication
+            if isinstance(authentication, ActionAuthentication)
+            else ActionAuthentication(**authentication)
+        )
     body = ActionUpdateRequest(
         openapi_schema=openapi_schema,
         authentication=authentication,
     )
     response: ActionUpdateResponse = api_update_action(action_id=action_id, payload=body)
     return response.data
 
 
 async def a_update_action(
     action_id: str,
+    *,
     openapi_schema: Optional[Dict] = None,
-    authentication: Optional[ActionAuthentication] = None,
+    authentication: Optional[Union[ActionAuthentication, Dict[str, Any]]] = None,
 ) -> Action:
     """
     Update an action in async mode.
 
     :param action_id: The ID of the action.
     :param openapi_schema: The action schema, which is compliant with the OpenAPI Specification. It should only have exactly one path and one method.
     :param authentication: The action API authentication.
     :return: The updated action object.
     """
+    if authentication:
+        authentication = (
+            authentication
+            if isinstance(authentication, ActionAuthentication)
+            else ActionAuthentication(**authentication)
+        )
     body = ActionUpdateRequest(
         openapi_schema=openapi_schema,
         authentication=authentication,
     )
     response: ActionUpdateResponse = await async_api_update_action(action_id=action_id, payload=body)
     return response.data
 
@@ -211,14 +233,15 @@
     """
 
     await async_api_delete_action(action_id=action_id)
 
 
 def run_action(
     action_id: str,
+    *,
     parameters: Dict,
 ) -> Dict:
     """
     Run an action.
 
     :param action_id: The ID of the action.
     :param parameters: The action parameters.
@@ -231,14 +254,15 @@
     response: ActionRunResponse = api_run_action(action_id=action_id, payload=body)
     result = response.data
     return result
 
 
 async def a_run_action(
     action_id: str,
+    *,
     parameters: Dict,
 ) -> Dict:
     """
     Run an action in async mode.
 
     :param action_id: The ID of the action.
     :param parameters: The action parameters.
```

### Comparing `taskingai-0.2.1/taskingai.egg-info/SOURCES.txt` & `taskingai-0.2.2/taskingai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 taskingai/client/models/entities/chat_completion_role.py
 taskingai/client/models/entities/chat_completion_system_message.py
 taskingai/client/models/entities/chat_completion_user_message.py
 taskingai/client/models/entities/chat_memory.py
 taskingai/client/models/entities/chat_memory_message.py
 taskingai/client/models/entities/chunk.py
 taskingai/client/models/entities/collection.py
+taskingai/client/models/entities/file_id_data.py
 taskingai/client/models/entities/message.py
 taskingai/client/models/entities/message_chunk.py
 taskingai/client/models/entities/message_content.py
 taskingai/client/models/entities/message_generation_log.py
 taskingai/client/models/entities/message_role.py
 taskingai/client/models/entities/record.py
 taskingai/client/models/entities/record_type.py
@@ -111,14 +112,15 @@
 taskingai/client/models/entities/status.py
 taskingai/client/models/entities/text_embedding_input_type.py
 taskingai/client/models/entities/text_embedding_output.py
 taskingai/client/models/entities/text_splitter.py
 taskingai/client/models/entities/text_splitter_type.py
 taskingai/client/models/entities/tool_ref.py
 taskingai/client/models/entities/tool_type.py
+taskingai/client/models/entities/upload_file_purpose.py
 taskingai/client/models/schemas/__init__.py
 taskingai/client/models/schemas/action_bulk_create_request.py
 taskingai/client/models/schemas/action_bulk_create_response.py
 taskingai/client/models/schemas/action_get_response.py
 taskingai/client/models/schemas/action_list_request.py
 taskingai/client/models/schemas/action_list_response.py
 taskingai/client/models/schemas/action_run_request.py
@@ -173,17 +175,20 @@
 taskingai/client/models/schemas/record_get_response.py
 taskingai/client/models/schemas/record_list_request.py
 taskingai/client/models/schemas/record_list_response.py
 taskingai/client/models/schemas/record_update_request.py
 taskingai/client/models/schemas/record_update_response.py
 taskingai/client/models/schemas/text_embedding_request.py
 taskingai/client/models/schemas/text_embedding_response.py
+taskingai/client/models/schemas/upload_file_response.py
 taskingai/client/stream_apis/__init__.py
 taskingai/client/stream_apis/stream_api_chat_completion.py
 taskingai/client/stream_apis/stream_api_message_generation.py
+taskingai/file/__init__.py
+taskingai/file/file.py
 taskingai/inference/__init__.py
 taskingai/inference/chat_completion.py
 taskingai/inference/text_embedding.py
 taskingai/retrieval/__init__.py
 taskingai/retrieval/chunk.py
 taskingai/retrieval/collection.py
 taskingai/retrieval/record.py
```

