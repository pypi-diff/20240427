# Comparing `tmp/llmtuner-0.6.3.tar.gz` & `tmp/llmtuner-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmtuner-0.6.3.tar", last modified: Sun Apr 21 15:13:38 2024, max compression
+gzip compressed data, was "llmtuner-0.7.0.tar", last modified: Sat Apr 27 19:49:59 2024, max compression
```

## Comparing `llmtuner-0.6.3.tar` & `llmtuner-0.7.0.tar`

### file list

```diff
@@ -1,121 +1,131 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:38.024641 llmtuner-0.6.3/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2024-04-21 15:12:38.000000 llmtuner-0.6.3/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    34527 2024-04-21 15:13:37.988640 llmtuner-0.6.3/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    31899 2024-04-21 15:12:38.000000 llmtuner-0.6.3/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      641 2024-04-21 15:12:38.000000 llmtuner-0.6.3/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2024-04-21 15:13:38.024641 llmtuner-0.6.3/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2596 2024-04-21 15:12:39.000000 llmtuner-0.6.3/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:32.364621 llmtuner-0.6.3/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:32.552622 llmtuner-0.6.3/src/llmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      389 2024-04-21 15:12:37.000000 llmtuner-0.6.3/src/llmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:32.880623 llmtuner-0.6.3/src/llmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       55 2024-04-21 15:12:28.000000 llmtuner-0.6.3/src/llmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8717 2024-04-21 15:12:28.000000 llmtuner-0.6.3/src/llmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3127 2024-04-21 15:12:28.000000 llmtuner-0.6.3/src/llmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:33.148624 llmtuner-0.6.3/src/llmtuner/chat/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      110 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/chat/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1770 2024-04-21 15:12:28.000000 llmtuner-0.6.3/src/llmtuner/chat/base_engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3334 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/chat/chat_model.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    10056 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/chat/hf_engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5840 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/chat/vllm_engine.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:33.584625 llmtuner-0.6.3/src/llmtuner/data/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      377 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/data/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5505 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/data/aligner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2140 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/data/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6528 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/data/formatter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7364 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/data/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4989 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/data/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11328 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/data/preprocess.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    30113 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/data/template.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3698 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/data/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:33.692626 llmtuner-0.6.3/src/llmtuner/eval/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       59 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/eval/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5763 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/eval/evaluator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2419 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/eval/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:34.232627 llmtuner-0.6.3/src/llmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6495 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    34840 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1117 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7450 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1314 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/packages.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:34.468628 llmtuner-0.6.3/src/llmtuner/extras/patches/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/patches/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8841 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/patches/llama_patch.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1824 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/ploting.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:34.884630 llmtuner-0.6.3/src/llmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      494 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3871 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1462 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/hparams/evaluation_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    12586 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1915 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7468 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/hparams/model_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    14439 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/hparams/parser.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:35.380632 llmtuner-0.6.3/src/llmtuner/model/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      229 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/model/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7992 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/model/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5786 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/model/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    18372 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/model/patcher.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6956 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/model/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:35.520632 llmtuner-0.6.3/src/llmtuner/train/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/train/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:35.664632 llmtuner-0.6.3/src/llmtuner/train/dpo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/dpo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7577 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/dpo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3090 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/dpo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:35.792633 llmtuner-0.6.3/src/llmtuner/train/orpo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/orpo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5763 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/orpo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2654 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/orpo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:36.032634 llmtuner-0.6.3/src/llmtuner/train/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    20807 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2380 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2634 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:36.240634 llmtuner-0.6.3/src/llmtuner/train/pt/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/pt/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1348 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/pt/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2439 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/pt/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:36.452635 llmtuner-0.6.3/src/llmtuner/train/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      267 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5318 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3041 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:36.840637 llmtuner-0.6.3/src/llmtuner/train/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2247 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5314 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4300 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/sft/workflow.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3914 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/train/tuner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    16450 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/train/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:37.216638 llmtuner-0.6.3/src/llmtuner/webui/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       95 2024-04-21 15:12:37.000000 llmtuner-0.6.3/src/llmtuner/webui/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4956 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/chatter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4881 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/common.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:37.648639 llmtuner-0.6.3/src/llmtuner/webui/components/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      362 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/components/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2103 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/components/chatbot.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/components/data.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2776 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/components/eval.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3753 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/components/export.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1356 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/components/infer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2395 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/components/top.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     9927 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/components/train.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      567 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/css.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2695 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2600 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/interface.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    42316 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/locales.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2004 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/manager.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15689 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/runner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3313 2024-04-21 15:12:37.000000 llmtuner-0.6.3/src/llmtuner/webui/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:32.780622 llmtuner-0.6.3/src/llmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    34527 2024-04-21 15:13:30.000000 llmtuner-0.6.3/src/llmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3047 2024-04-21 15:13:31.000000 llmtuner-0.6.3/src/llmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2024-04-21 15:13:30.000000 llmtuner-0.6.3/src/llmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      586 2024-04-21 15:13:30.000000 llmtuner-0.6.3/src/llmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2024-04-21 15:13:30.000000 llmtuner-0.6.3/src/llmtuner.egg-info/top_level.txt
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:37.952640 llmtuner-0.6.3/tests/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2311 2024-04-21 15:12:37.000000 llmtuner-0.6.3/tests/test_attn.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1691 2024-04-21 15:12:37.000000 llmtuner-0.6.3/tests/test_galore.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      933 2024-04-21 15:12:37.000000 llmtuner-0.6.3/tests/test_throughput.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2566 2024-04-21 15:12:37.000000 llmtuner-0.6.3/tests/test_toolcall.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:58.951033 llmtuner-0.7.0/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2024-04-27 19:49:37.000000 llmtuner-0.7.0/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    36078 2024-04-27 19:49:58.915033 llmtuner-0.7.0/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    33563 2024-04-27 19:49:37.000000 llmtuner-0.7.0/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      641 2024-04-27 19:49:37.000000 llmtuner-0.7.0/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2024-04-27 19:49:58.951033 llmtuner-0.7.0/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2529 2024-04-27 19:49:38.000000 llmtuner-0.7.0/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:53.827016 llmtuner-0.7.0/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:53.999016 llmtuner-0.7.0/src/llmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      389 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:54.391018 llmtuner-0.7.0/src/llmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       55 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8717 2024-04-27 19:49:24.000000 llmtuner-0.7.0/src/llmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3127 2024-04-27 19:49:24.000000 llmtuner-0.7.0/src/llmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:54.631018 llmtuner-0.7.0/src/llmtuner/chat/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      110 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/chat/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1896 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/chat/base_engine.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3578 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/chat/chat_model.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11272 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/chat/hf_engine.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8237 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/chat/vllm_engine.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:54.995020 llmtuner-0.7.0/src/llmtuner/data/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      377 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6621 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/data/aligner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2140 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6528 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/formatter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7451 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5033 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    13825 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/preprocess.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    32979 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/template.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3698 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:55.207020 llmtuner-0.7.0/src/llmtuner/eval/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       59 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/eval/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5776 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/eval/evaluator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2419 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/eval/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:55.443021 llmtuner-0.7.0/src/llmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6495 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    40195 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1117 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7450 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1662 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/packages.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1824 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/ploting.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:55.691022 llmtuner-0.7.0/src/llmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      494 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3882 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1462 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/evaluation_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    12586 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1917 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8174 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/model_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15072 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/parser.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:55.859023 llmtuner-0.7.0/src/llmtuner/model/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      294 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8911 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/model/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6222 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5551 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/patcher.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:56.459025 llmtuner-0.7.0/src/llmtuner/model/utils/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1998 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/attention.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4028 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/checkpointing.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2344 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/embedding.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    13800 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/longlora.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3061 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      832 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/mod.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2063 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/moe.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6262 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/quantization.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1711 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/rope.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2886 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/unsloth.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2311 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/valuehead.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      887 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/visual.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:56.595025 llmtuner-0.7.0/src/llmtuner/train/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:56.771026 llmtuner-0.7.0/src/llmtuner/train/dpo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/dpo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7577 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/dpo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3152 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/dpo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:56.907026 llmtuner-0.7.0/src/llmtuner/train/orpo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/orpo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5763 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/orpo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2717 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/orpo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:57.195027 llmtuner-0.7.0/src/llmtuner/train/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    20807 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2380 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2696 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:57.339028 llmtuner-0.7.0/src/llmtuner/train/pt/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/pt/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1348 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/pt/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2501 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/pt/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:57.531028 llmtuner-0.7.0/src/llmtuner/train/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      267 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5318 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3103 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:57.679029 llmtuner-0.7.0/src/llmtuner/train/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2247 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5314 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4479 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/sft/workflow.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3927 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/tuner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    16575 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:58.179031 llmtuner-0.7.0/src/llmtuner/webui/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       95 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5235 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/webui/chatter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4986 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/common.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:58.731032 llmtuner-0.7.0/src/llmtuner/webui/components/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      362 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/components/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2389 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/chatbot.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/data.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2776 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/eval.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4218 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/export.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1566 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/infer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2605 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/top.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     9925 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/components/train.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      567 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/css.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2757 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/engine.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2563 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/interface.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    43606 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/locales.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2055 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/manager.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15827 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/runner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3313 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:54.255017 llmtuner-0.7.0/src/llmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    36078 2024-04-27 19:49:52.000000 llmtuner-0.7.0/src/llmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3408 2024-04-27 19:49:52.000000 llmtuner-0.7.0/src/llmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2024-04-27 19:49:52.000000 llmtuner-0.7.0/src/llmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      541 2024-04-27 19:49:52.000000 llmtuner-0.7.0/src/llmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2024-04-27 19:49:52.000000 llmtuner-0.7.0/src/llmtuner.egg-info/top_level.txt
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:58.883033 llmtuner-0.7.0/tests/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2311 2024-04-27 19:49:36.000000 llmtuner-0.7.0/tests/test_attn.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1691 2024-04-27 19:49:36.000000 llmtuner-0.7.0/tests/test_galore.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      933 2024-04-27 19:49:36.000000 llmtuner-0.7.0/tests/test_throughput.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2566 2024-04-27 19:49:36.000000 llmtuner-0.7.0/tests/test_toolcall.py
```

### Comparing `llmtuner-0.6.3/LICENSE` & `llmtuner-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/PKG-INFO` & `llmtuner-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.6.3
+Version: 0.7.0
 Summary: Easy-to-use LLM fine-tuning framework
 Home-page: https://github.com/hiyouga/LLaMA-Factory
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -35,29 +35,27 @@
 Requires-Dist: protobuf
 Requires-Dist: uvicorn
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: sse-starlette
 Requires-Dist: matplotlib
 Requires-Dist: fire
+Requires-Dist: packaging
 Provides-Extra: deepspeed
 Requires-Dist: deepspeed>=0.10.0; extra == "deepspeed"
 Provides-Extra: metrics
 Requires-Dist: nltk; extra == "metrics"
 Requires-Dist: jieba; extra == "metrics"
 Requires-Dist: rouge-chinese; extra == "metrics"
-Provides-Extra: unsloth
-Requires-Dist: torch==2.2.0; extra == "unsloth"
-Requires-Dist: unsloth[cu121-ampere-torch220]; extra == "unsloth"
 Provides-Extra: galore
 Requires-Dist: galore-torch; extra == "galore"
 Provides-Extra: badam
 Requires-Dist: badam; extra == "badam"
 Provides-Extra: vllm
-Requires-Dist: vllm>=0.3.3; extra == "vllm"
+Requires-Dist: vllm>=0.4.0; extra == "vllm"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes>=0.39.0; extra == "bitsandbytes"
 Provides-Extra: gptq
 Requires-Dist: optimum>=1.16.0; extra == "gptq"
 Requires-Dist: auto-gptq>=0.5.0; extra == "gptq"
 Provides-Extra: awq
 Requires-Dist: autoawq; extra == "awq"
@@ -112,16 +110,16 @@
 - [Projects using LLaMA Factory](#projects-using-llama-factory)
 - [License](#license)
 - [Citation](#citation)
 - [Acknowledgement](#acknowledgement)
 
 ## Features
 
-- **Various models**: LLaMA, Mistral, Mixtral-MoE, Qwen, Yi, Gemma, Baichuan, ChatGLM, Phi, etc.
-- **Integrated methods**: (Continuous) pre-training, supervised fine-tuning, reward modeling, PPO, DPO and ORPO.
+- **Various models**: LLaMA, LLaVA, Mistral, Mixtral-MoE, Qwen, Yi, Gemma, Baichuan, ChatGLM, Phi, etc.
+- **Integrated methods**: (Continuous) pre-training, (multimodal) supervised fine-tuning, reward modeling, PPO, DPO and ORPO.
 - **Scalable resources**: 32-bit full-tuning, 16-bit freeze-tuning, 16-bit LoRA and 2/4/8-bit QLoRA via AQLM/AWQ/GPTQ/LLM.int8.
 - **Advanced algorithms**: GaLore, BAdam, DoRA, LongLoRA, LLaMA Pro, Mixture-of-Depths, LoRA+, LoftQ and Agent tuning.
 - **Practical tricks**: FlashAttention-2, Unsloth, RoPE scaling, NEFTune and rsLoRA.
 - **Experiment monitors**: LlamaBoard, TensorBoard, Wandb, MLflow, etc.
 - **Faster inference**: OpenAI-style API, Gradio UI and CLI with vLLM worker.
 
 ## Benchmark
@@ -137,17 +135,19 @@
 - **GPU Memory**: Peak GPU memory usage in 4-bit quantized training. (bs=1, cutoff_len=1024)
 - We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA Factory's LoRA tuning.
 
 </details>
 
 ## Changelog
 
-[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
+[24/04/26] We supported fine-tuning the **LLaVA-1.5** multimodal LLMs. See `examples/lora_single_gpu/sft_mllm.sh` for usage.
+
+[24/04/22] We provided a **[Colab notebook](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)** for fine-tuning the Llama-3 model on a free T4 GPU. Two Llama-3-derived models fine-tuned using LLaMA Factory are available at Hugging Face, check [Llama3-8B-Chinese-Chat](https://huggingface.co/shenzhi-wang/Llama3-8B-Chinese-Chat) and [Llama3-Chinese](https://huggingface.co/zhichen/Llama3-Chinese) for details.
 
-[24/04/19] We supported **Meta Llama 3** model series.
+[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
 
 [24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See `examples/extras/badam` for usage.
 
 [24/04/16] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s long-sequence training (Llama-2-7B-56k within 24GB). It achieves **117%** speed and **50%** memory compared with FlashAttention-2, more benchmarks can be found in [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison).
 
 <details><summary>Full Changelog</summary>
 
@@ -179,15 +179,15 @@
 
 [23/10/21] We supported **[NEFTune](https://arxiv.org/abs/2310.05914)** trick for fine-tuning. Try `--neftune_noise_alpha` argument to activate NEFTune, e.g., `--neftune_noise_alpha 5`.
 
 [23/09/27] We supported **$S^2$-Attn** proposed by [LongLoRA](https://github.com/dvlab-research/LongLoRA) for the LLaMA models. Try `--shift_attn` argument to enable shift short attention.
 
 [23/09/23] We integrated MMLU, C-Eval and CMMLU benchmarks in this repo. See [this example](#evaluation) to evaluate your models.
 
-[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `--flash_attn` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
+[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `--flash_attn fa2` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
 
 [23/08/12] We supported **RoPE scaling** to extend the context length of the LLaMA models. Try `--rope_scaling linear` argument in training and `--rope_scaling dynamic` argument at inference to extrapolate the position embeddings.
 
 [23/08/11] We supported **[DPO training](https://arxiv.org/abs/2305.18290)** for instruction-tuned models. See [this example](#dpo-training) to train your models.
 
 [23/07/31] We supported **dataset streaming**. Try `--streaming` and `--max_steps 10000` arguments to load your dataset in streaming mode.
 
@@ -203,42 +203,46 @@
 
 [23/06/03] We supported quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized models.
 
 </details>
 
 ## Supported Models
 
-| Model                                                    | Model size                  | Default module    | Template  |
-| -------------------------------------------------------- | --------------------------- | ----------------- | --------- |
-| [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                      | W_pack            | baichuan2 |
-| [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                          | query_key_value   | chatglm3  |
-| [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                    | q_proj,v_proj     | cohere    |
-| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                  | q_proj,v_proj     | deepseek  |
-| [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                 | query_key_value   | falcon    |
-| [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                       | q_proj,v_proj     | gemma     |
-| [InternLM2](https://huggingface.co/internlm)             | 7B/20B                      | wqkv              | intern2   |
-| [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B              | q_proj,v_proj     | -         |
-| [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                  | q_proj,v_proj     | llama2    |
-| [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                      | q_proj,v_proj     | llama3    |
-| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B/8x22B               | q_proj,v_proj     | mistral   |
-| [OLMo](https://huggingface.co/allenai)                   | 1B/7B                       | att_proj          | olmo      |
-| [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                   | q_proj,v_proj     | -         |
-| [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B             | c_attn            | qwen      |
-| [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B | q_proj,v_proj     | qwen      |
-| [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                   | q_proj,v_proj     | -         |
-| [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                  | q_proj,v_proj     | xverse    |
-| [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                   | q_proj,v_proj     | yi        |
-| [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                 | q_proj,v_proj     | yuan      |
+| Model                                                    | Model size                       | Default module    | Template  |
+| -------------------------------------------------------- | -------------------------------- | ----------------- | --------- |
+| [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                           | W_pack            | baichuan2 |
+| [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
+| [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
+| [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                               | query_key_value   | chatglm3  |
+| [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                         | q_proj,v_proj     | cohere    |
+| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                       | q_proj,v_proj     | deepseek  |
+| [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                      | query_key_value   | falcon    |
+| [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                            | q_proj,v_proj     | gemma     |
+| [InternLM2](https://huggingface.co/internlm)             | 7B/20B                           | wqkv              | intern2   |
+| [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B                   | q_proj,v_proj     | -         |
+| [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                       | q_proj,v_proj     | llama2    |
+| [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                           | q_proj,v_proj     | llama3    |
+| [LLaVA-1.5](https://huggingface.co/llava-hf)             | 7B/13B                           | q_proj,v_proj     | vicuna    |
+| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B/8x22B                    | q_proj,v_proj     | mistral   |
+| [OLMo](https://huggingface.co/allenai)                   | 1B/7B                            | q_proj,v_proj     | -         |
+| [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                        | q_proj,v_proj     | -         |
+| [Phi-3](https://huggingface.co/microsoft)                | 3.8B                             | qkv_proj          | phi       |
+| [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B                  | c_attn            | qwen      |
+| [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B/110B | q_proj,v_proj     | qwen      |
+| [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                        | q_proj,v_proj     | -         |
+| [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                       | q_proj,v_proj     | xverse    |
+| [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                        | q_proj,v_proj     | yi        |
+| [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                      | q_proj,v_proj     | yuan      |
 
 > [!NOTE]
-> **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules.
+> **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules for better convergence.
 >
-> For the "base" models, the `--template` argument can be chosen from `default`, `alpaca`, `vicuna` etc. But make sure to use the **corresponding template** for the "chat" models.
+> For the "base" models, the `--template` argument can be chosen from `default`, `alpaca`, `vicuna` etc. But make sure to use the **corresponding template** for the "instruct/chat" models.
+>
+> Remember to use the **SAME** template in training and inference.
 
 Please refer to [constants.py](src/llmtuner/extras/constants.py) for a full list of models we supported.
 
 You also can add a custom chat template to [template.py](src/llmtuner/data/template.py).
 
 ## Supported Training Approaches
 
@@ -301,14 +305,15 @@
 - [ShareGPT4 (en&zh)](https://huggingface.co/datasets/shibing624/sharegpt_gpt4)
 - [UltraChat 200k (en)](https://huggingface.co/datasets/HuggingFaceH4/ultrachat_200k)
 - [AgentInstruct (en)](https://huggingface.co/datasets/THUDM/AgentInstruct)
 - [LMSYS Chat 1M (en)](https://huggingface.co/datasets/lmsys/lmsys-chat-1m)
 - [Evol Instruct V2 (en)](https://huggingface.co/datasets/WizardLM/WizardLM_evol_instruct_V2_196k)
 - [Glaive Function Calling V2 (en)](https://huggingface.co/datasets/glaiveai/glaive-function-calling-v2)
 - [Cosmopedia (en)](https://huggingface.co/datasets/HuggingFaceTB/cosmopedia)
+- [LLaVA mixed (en&zh)](https://huggingface.co/datasets/BUAADreamer/llava-en-zh-300k)
 - [Open Assistant (de)](https://huggingface.co/datasets/mayflowergmbh/oasst_de)
 - [Dolly 15k (de)](https://huggingface.co/datasets/mayflowergmbh/dolly-15k_de)
 - [Alpaca GPT4 (de)](https://huggingface.co/datasets/mayflowergmbh/alpaca-gpt4_de)
 - [OpenSchnabeltier (de)](https://huggingface.co/datasets/mayflowergmbh/openschnabeltier_de)
 - [Evol Instruct (de)](https://huggingface.co/datasets/mayflowergmbh/evol-instruct_de)
 - [Dolphin (de)](https://huggingface.co/datasets/mayflowergmbh/dolphin_de)
 - [Booksum (de)](https://huggingface.co/datasets/mayflowergmbh/booksum_de)
@@ -320,15 +325,15 @@
 <details><summary>Preference datasets</summary>
 
 - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
 - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 - [Orca DPO (en)](https://huggingface.co/datasets/Intel/orca_dpo_pairs)
 - [Nectar (en)](https://huggingface.co/datasets/berkeley-nest/Nectar)
-- [DPO mix (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
+- [DPO mixed (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
 - [Orca DPO (de)](https://huggingface.co/datasets/mayflowergmbh/intel_orca_dpo_pairs_de)
 
 </details>
 
 Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
@@ -355,23 +360,23 @@
 | bitsandbytes | 0.39.0  | 0.43.0    |
 | flash-attn   | 2.3.0   | 2.5.6     |
 
 ### Hardware Requirement
 
 \* *estimated*
 
-| Method            | Bits |   7B  |  13B  |  30B  |   70B  |  8x7B |  8x22B |
-| ----------------- | ---- | ----- | ----- | ----- | ------ | ----- | ------ |
-| Full              | AMP  | 120GB | 240GB | 600GB | 1200GB | 900GB | 2400GB |
-| Full              |  16  |  60GB | 120GB | 300GB |  600GB | 400GB | 1200GB |
-| Freeze            |  16  |  20GB |  40GB |  80GB |  200GB | 160GB |  400GB |
-| LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB | 120GB |  320GB |
-| QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  60GB |  160GB |
-| QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |  30GB |   96GB |
-| QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |  18GB |   48GB |
+| Method            | Bits |   7B  |  13B  |  30B  |   70B  |  110B  |  8x7B |  8x22B |
+| ----------------- | ---- | ----- | ----- | ----- | ------ | ------ | ----- | ------ |
+| Full              | AMP  | 120GB | 240GB | 600GB | 1200GB | 2000GB | 900GB | 2400GB |
+| Full              |  16  |  60GB | 120GB | 300GB |  600GB |  900GB | 400GB | 1200GB |
+| Freeze            |  16  |  20GB |  40GB |  80GB |  200GB |  360GB | 160GB |  400GB |
+| LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB |  240GB | 120GB |  320GB |
+| QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  140GB |  60GB |  160GB |
+| QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |   72GB |  30GB |   96GB |
+| QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |   48GB |  18GB |   48GB |
 
 ## Getting Started
 
 ### Data Preparation
 
 Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
 
@@ -384,41 +389,51 @@
 git clone https://github.com/hiyouga/LLaMA-Factory.git
 conda create -n llama_factory python=3.10
 conda activate llama_factory
 cd LLaMA-Factory
 pip install -e .[metrics]
 ```
 
-Extra dependencies available: deepspeed, metrics, unsloth, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
+Extra dependencies available: deepspeed, metrics, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
 
 <details><summary>For Windows users</summary>
 
 If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
 
 ```bash
 pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.2.post2-py3-none-win_amd64.whl
 ```
 
 To enable FlashAttention-2 on the Windows platform, you need to install the precompiled `flash-attn` library, which supports CUDA 12.1 to 12.2. Please download the corresponding version from [flash-attention](https://github.com/bdashore3/flash-attention/releases) based on your requirements.
 
 </details>
 
-### LLaMA Board GUI
+### Train with LLaMA Board GUI (powered by [Gradio](https://github.com/gradio-app/gradio))
 
 > [!IMPORTANT]
 > LLaMA Board GUI only supports training on a single GPU, please use [CLI](#command-line-interface) for distributed training.
 
 #### Use local environment
 
 ```bash
 export CUDA_VISIBLE_DEVICES=0 # `set CUDA_VISIBLE_DEVICES=0` for Windows
 export GRADIO_SERVER_PORT=7860 # `set GRADIO_SERVER_PORT=7860` for Windows
 python src/train_web.py # or python -m llmtuner.webui.interface
 ```
 
+<details><summary>For Alibaba Cloud users</summary>
+
+If you encountered display problems in LLaMA Board on Alibaba Cloud, try using the following command to set environment variables before starting LLaMA Board:
+
+```bash
+export GRADIO_ROOT_PATH=/${JUPYTER_NAME}/proxy/7860/
+```
+
+</details>
+
 #### Use Docker
 
 ```bash
 docker build -f ./Dockerfile -t llama-factory:latest .
 docker run --gpus=all \
     -v ./hf_cache:/root/.cache/huggingface/ \
     -v ./data:/app/data \
@@ -440,39 +455,39 @@
 
 - hf_cache: Utilize Hugging Face cache on the host machine. Reassignable if a cache already exists in a different directory.
 - data: Place datasets on this dir of the host machine so that they can be selected on LLaMA Board GUI.
 - output: Set export dir to this location so that the merged result can be accessed directly on the host machine.
 
 </details>
 
-### Command Line Interface
+### Train with Command Line Interface
 
 See [examples/README.md](examples/README.md) for usage.
 
 Use `python src/train_bash.py -h` to display arguments description.
 
 ### Deploy with OpenAI-style API and vLLM
 
 ```bash
 CUDA_VISIBLE_DEVICES=0,1 API_PORT=8000 python src/api_demo.py \
-    --model_name_or_path mistralai/Mistral-7B-Instruct-v0.2 \
-    --template mistral \
+    --model_name_or_path meta-llama/Meta-Llama-3-8B-Instruct \
+    --template llama3 \
     --infer_backend vllm \
     --vllm_enforce_eager
 ```
 
-### Use ModelScope Hub
+### Download from ModelScope Hub
 
 If you have trouble with downloading models and datasets from Hugging Face, you can use ModelScope.
 
 ```bash
 export USE_MODELSCOPE_HUB=1 # `set USE_MODELSCOPE_HUB=1` for Windows
 ```
 
-Train the model by specifying a model ID of the ModelScope Hub as the `--model_name_or_path`. You can find a full list of model IDs at [ModelScope Hub](https://modelscope.cn/models), e.g., `modelscope/Llama-2-7b-ms`.
+Train the model by specifying a model ID of the ModelScope Hub as the `--model_name_or_path`. You can find a full list of model IDs at [ModelScope Hub](https://modelscope.cn/models), e.g., `LLM-Research/Meta-Llama-3-8B-Instruct`.
 
 ## Projects using LLaMA Factory
 
 If you have a project that should be incorporated, please contact via email or create a pull request.
 
 <details><summary>Click to show</summary>
 
@@ -513,15 +528,15 @@
 
 </details>
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
-Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
+Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2/LLaVA-1.5](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Phi-3](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/LICENSE) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
 @article{zheng2024llamafactory,
```

### Comparing `llmtuner-0.6.3/README.md` & `llmtuner-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 - [Projects using LLaMA Factory](#projects-using-llama-factory)
 - [License](#license)
 - [Citation](#citation)
 - [Acknowledgement](#acknowledgement)
 
 ## Features
 
-- **Various models**: LLaMA, Mistral, Mixtral-MoE, Qwen, Yi, Gemma, Baichuan, ChatGLM, Phi, etc.
-- **Integrated methods**: (Continuous) pre-training, supervised fine-tuning, reward modeling, PPO, DPO and ORPO.
+- **Various models**: LLaMA, LLaVA, Mistral, Mixtral-MoE, Qwen, Yi, Gemma, Baichuan, ChatGLM, Phi, etc.
+- **Integrated methods**: (Continuous) pre-training, (multimodal) supervised fine-tuning, reward modeling, PPO, DPO and ORPO.
 - **Scalable resources**: 32-bit full-tuning, 16-bit freeze-tuning, 16-bit LoRA and 2/4/8-bit QLoRA via AQLM/AWQ/GPTQ/LLM.int8.
 - **Advanced algorithms**: GaLore, BAdam, DoRA, LongLoRA, LLaMA Pro, Mixture-of-Depths, LoRA+, LoftQ and Agent tuning.
 - **Practical tricks**: FlashAttention-2, Unsloth, RoPE scaling, NEFTune and rsLoRA.
 - **Experiment monitors**: LlamaBoard, TensorBoard, Wandb, MLflow, etc.
 - **Faster inference**: OpenAI-style API, Gradio UI and CLI with vLLM worker.
 
 ## Benchmark
@@ -64,17 +64,19 @@
 - **GPU Memory**: Peak GPU memory usage in 4-bit quantized training. (bs=1, cutoff_len=1024)
 - We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA Factory's LoRA tuning.
 
 </details>
 
 ## Changelog
 
-[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
+[24/04/26] We supported fine-tuning the **LLaVA-1.5** multimodal LLMs. See `examples/lora_single_gpu/sft_mllm.sh` for usage.
+
+[24/04/22] We provided a **[Colab notebook](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)** for fine-tuning the Llama-3 model on a free T4 GPU. Two Llama-3-derived models fine-tuned using LLaMA Factory are available at Hugging Face, check [Llama3-8B-Chinese-Chat](https://huggingface.co/shenzhi-wang/Llama3-8B-Chinese-Chat) and [Llama3-Chinese](https://huggingface.co/zhichen/Llama3-Chinese) for details.
 
-[24/04/19] We supported **Meta Llama 3** model series.
+[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
 
 [24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See `examples/extras/badam` for usage.
 
 [24/04/16] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s long-sequence training (Llama-2-7B-56k within 24GB). It achieves **117%** speed and **50%** memory compared with FlashAttention-2, more benchmarks can be found in [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison).
 
 <details><summary>Full Changelog</summary>
 
@@ -106,15 +108,15 @@
 
 [23/10/21] We supported **[NEFTune](https://arxiv.org/abs/2310.05914)** trick for fine-tuning. Try `--neftune_noise_alpha` argument to activate NEFTune, e.g., `--neftune_noise_alpha 5`.
 
 [23/09/27] We supported **$S^2$-Attn** proposed by [LongLoRA](https://github.com/dvlab-research/LongLoRA) for the LLaMA models. Try `--shift_attn` argument to enable shift short attention.
 
 [23/09/23] We integrated MMLU, C-Eval and CMMLU benchmarks in this repo. See [this example](#evaluation) to evaluate your models.
 
-[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `--flash_attn` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
+[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `--flash_attn fa2` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
 
 [23/08/12] We supported **RoPE scaling** to extend the context length of the LLaMA models. Try `--rope_scaling linear` argument in training and `--rope_scaling dynamic` argument at inference to extrapolate the position embeddings.
 
 [23/08/11] We supported **[DPO training](https://arxiv.org/abs/2305.18290)** for instruction-tuned models. See [this example](#dpo-training) to train your models.
 
 [23/07/31] We supported **dataset streaming**. Try `--streaming` and `--max_steps 10000` arguments to load your dataset in streaming mode.
 
@@ -130,42 +132,46 @@
 
 [23/06/03] We supported quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized models.
 
 </details>
 
 ## Supported Models
 
-| Model                                                    | Model size                  | Default module    | Template  |
-| -------------------------------------------------------- | --------------------------- | ----------------- | --------- |
-| [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                      | W_pack            | baichuan2 |
-| [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                          | query_key_value   | chatglm3  |
-| [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                    | q_proj,v_proj     | cohere    |
-| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                  | q_proj,v_proj     | deepseek  |
-| [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                 | query_key_value   | falcon    |
-| [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                       | q_proj,v_proj     | gemma     |
-| [InternLM2](https://huggingface.co/internlm)             | 7B/20B                      | wqkv              | intern2   |
-| [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B              | q_proj,v_proj     | -         |
-| [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                  | q_proj,v_proj     | llama2    |
-| [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                      | q_proj,v_proj     | llama3    |
-| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B/8x22B               | q_proj,v_proj     | mistral   |
-| [OLMo](https://huggingface.co/allenai)                   | 1B/7B                       | att_proj          | olmo      |
-| [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                   | q_proj,v_proj     | -         |
-| [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B             | c_attn            | qwen      |
-| [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B | q_proj,v_proj     | qwen      |
-| [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                   | q_proj,v_proj     | -         |
-| [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                  | q_proj,v_proj     | xverse    |
-| [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                   | q_proj,v_proj     | yi        |
-| [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                 | q_proj,v_proj     | yuan      |
+| Model                                                    | Model size                       | Default module    | Template  |
+| -------------------------------------------------------- | -------------------------------- | ----------------- | --------- |
+| [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                           | W_pack            | baichuan2 |
+| [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
+| [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
+| [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                               | query_key_value   | chatglm3  |
+| [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                         | q_proj,v_proj     | cohere    |
+| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                       | q_proj,v_proj     | deepseek  |
+| [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                      | query_key_value   | falcon    |
+| [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                            | q_proj,v_proj     | gemma     |
+| [InternLM2](https://huggingface.co/internlm)             | 7B/20B                           | wqkv              | intern2   |
+| [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B                   | q_proj,v_proj     | -         |
+| [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                       | q_proj,v_proj     | llama2    |
+| [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                           | q_proj,v_proj     | llama3    |
+| [LLaVA-1.5](https://huggingface.co/llava-hf)             | 7B/13B                           | q_proj,v_proj     | vicuna    |
+| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B/8x22B                    | q_proj,v_proj     | mistral   |
+| [OLMo](https://huggingface.co/allenai)                   | 1B/7B                            | q_proj,v_proj     | -         |
+| [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                        | q_proj,v_proj     | -         |
+| [Phi-3](https://huggingface.co/microsoft)                | 3.8B                             | qkv_proj          | phi       |
+| [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B                  | c_attn            | qwen      |
+| [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B/110B | q_proj,v_proj     | qwen      |
+| [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                        | q_proj,v_proj     | -         |
+| [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                       | q_proj,v_proj     | xverse    |
+| [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                        | q_proj,v_proj     | yi        |
+| [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                      | q_proj,v_proj     | yuan      |
 
 > [!NOTE]
-> **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules.
+> **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules for better convergence.
 >
-> For the "base" models, the `--template` argument can be chosen from `default`, `alpaca`, `vicuna` etc. But make sure to use the **corresponding template** for the "chat" models.
+> For the "base" models, the `--template` argument can be chosen from `default`, `alpaca`, `vicuna` etc. But make sure to use the **corresponding template** for the "instruct/chat" models.
+>
+> Remember to use the **SAME** template in training and inference.
 
 Please refer to [constants.py](src/llmtuner/extras/constants.py) for a full list of models we supported.
 
 You also can add a custom chat template to [template.py](src/llmtuner/data/template.py).
 
 ## Supported Training Approaches
 
@@ -228,14 +234,15 @@
 - [ShareGPT4 (en&zh)](https://huggingface.co/datasets/shibing624/sharegpt_gpt4)
 - [UltraChat 200k (en)](https://huggingface.co/datasets/HuggingFaceH4/ultrachat_200k)
 - [AgentInstruct (en)](https://huggingface.co/datasets/THUDM/AgentInstruct)
 - [LMSYS Chat 1M (en)](https://huggingface.co/datasets/lmsys/lmsys-chat-1m)
 - [Evol Instruct V2 (en)](https://huggingface.co/datasets/WizardLM/WizardLM_evol_instruct_V2_196k)
 - [Glaive Function Calling V2 (en)](https://huggingface.co/datasets/glaiveai/glaive-function-calling-v2)
 - [Cosmopedia (en)](https://huggingface.co/datasets/HuggingFaceTB/cosmopedia)
+- [LLaVA mixed (en&zh)](https://huggingface.co/datasets/BUAADreamer/llava-en-zh-300k)
 - [Open Assistant (de)](https://huggingface.co/datasets/mayflowergmbh/oasst_de)
 - [Dolly 15k (de)](https://huggingface.co/datasets/mayflowergmbh/dolly-15k_de)
 - [Alpaca GPT4 (de)](https://huggingface.co/datasets/mayflowergmbh/alpaca-gpt4_de)
 - [OpenSchnabeltier (de)](https://huggingface.co/datasets/mayflowergmbh/openschnabeltier_de)
 - [Evol Instruct (de)](https://huggingface.co/datasets/mayflowergmbh/evol-instruct_de)
 - [Dolphin (de)](https://huggingface.co/datasets/mayflowergmbh/dolphin_de)
 - [Booksum (de)](https://huggingface.co/datasets/mayflowergmbh/booksum_de)
@@ -247,15 +254,15 @@
 <details><summary>Preference datasets</summary>
 
 - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
 - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 - [Orca DPO (en)](https://huggingface.co/datasets/Intel/orca_dpo_pairs)
 - [Nectar (en)](https://huggingface.co/datasets/berkeley-nest/Nectar)
-- [DPO mix (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
+- [DPO mixed (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
 - [Orca DPO (de)](https://huggingface.co/datasets/mayflowergmbh/intel_orca_dpo_pairs_de)
 
 </details>
 
 Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
@@ -282,23 +289,23 @@
 | bitsandbytes | 0.39.0  | 0.43.0    |
 | flash-attn   | 2.3.0   | 2.5.6     |
 
 ### Hardware Requirement
 
 \* *estimated*
 
-| Method            | Bits |   7B  |  13B  |  30B  |   70B  |  8x7B |  8x22B |
-| ----------------- | ---- | ----- | ----- | ----- | ------ | ----- | ------ |
-| Full              | AMP  | 120GB | 240GB | 600GB | 1200GB | 900GB | 2400GB |
-| Full              |  16  |  60GB | 120GB | 300GB |  600GB | 400GB | 1200GB |
-| Freeze            |  16  |  20GB |  40GB |  80GB |  200GB | 160GB |  400GB |
-| LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB | 120GB |  320GB |
-| QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  60GB |  160GB |
-| QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |  30GB |   96GB |
-| QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |  18GB |   48GB |
+| Method            | Bits |   7B  |  13B  |  30B  |   70B  |  110B  |  8x7B |  8x22B |
+| ----------------- | ---- | ----- | ----- | ----- | ------ | ------ | ----- | ------ |
+| Full              | AMP  | 120GB | 240GB | 600GB | 1200GB | 2000GB | 900GB | 2400GB |
+| Full              |  16  |  60GB | 120GB | 300GB |  600GB |  900GB | 400GB | 1200GB |
+| Freeze            |  16  |  20GB |  40GB |  80GB |  200GB |  360GB | 160GB |  400GB |
+| LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB |  240GB | 120GB |  320GB |
+| QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  140GB |  60GB |  160GB |
+| QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |   72GB |  30GB |   96GB |
+| QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |   48GB |  18GB |   48GB |
 
 ## Getting Started
 
 ### Data Preparation
 
 Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
 
@@ -311,41 +318,51 @@
 git clone https://github.com/hiyouga/LLaMA-Factory.git
 conda create -n llama_factory python=3.10
 conda activate llama_factory
 cd LLaMA-Factory
 pip install -e .[metrics]
 ```
 
-Extra dependencies available: deepspeed, metrics, unsloth, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
+Extra dependencies available: deepspeed, metrics, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
 
 <details><summary>For Windows users</summary>
 
 If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
 
 ```bash
 pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.2.post2-py3-none-win_amd64.whl
 ```
 
 To enable FlashAttention-2 on the Windows platform, you need to install the precompiled `flash-attn` library, which supports CUDA 12.1 to 12.2. Please download the corresponding version from [flash-attention](https://github.com/bdashore3/flash-attention/releases) based on your requirements.
 
 </details>
 
-### LLaMA Board GUI
+### Train with LLaMA Board GUI (powered by [Gradio](https://github.com/gradio-app/gradio))
 
 > [!IMPORTANT]
 > LLaMA Board GUI only supports training on a single GPU, please use [CLI](#command-line-interface) for distributed training.
 
 #### Use local environment
 
 ```bash
 export CUDA_VISIBLE_DEVICES=0 # `set CUDA_VISIBLE_DEVICES=0` for Windows
 export GRADIO_SERVER_PORT=7860 # `set GRADIO_SERVER_PORT=7860` for Windows
 python src/train_web.py # or python -m llmtuner.webui.interface
 ```
 
+<details><summary>For Alibaba Cloud users</summary>
+
+If you encountered display problems in LLaMA Board on Alibaba Cloud, try using the following command to set environment variables before starting LLaMA Board:
+
+```bash
+export GRADIO_ROOT_PATH=/${JUPYTER_NAME}/proxy/7860/
+```
+
+</details>
+
 #### Use Docker
 
 ```bash
 docker build -f ./Dockerfile -t llama-factory:latest .
 docker run --gpus=all \
     -v ./hf_cache:/root/.cache/huggingface/ \
     -v ./data:/app/data \
@@ -367,39 +384,39 @@
 
 - hf_cache: Utilize Hugging Face cache on the host machine. Reassignable if a cache already exists in a different directory.
 - data: Place datasets on this dir of the host machine so that they can be selected on LLaMA Board GUI.
 - output: Set export dir to this location so that the merged result can be accessed directly on the host machine.
 
 </details>
 
-### Command Line Interface
+### Train with Command Line Interface
 
 See [examples/README.md](examples/README.md) for usage.
 
 Use `python src/train_bash.py -h` to display arguments description.
 
 ### Deploy with OpenAI-style API and vLLM
 
 ```bash
 CUDA_VISIBLE_DEVICES=0,1 API_PORT=8000 python src/api_demo.py \
-    --model_name_or_path mistralai/Mistral-7B-Instruct-v0.2 \
-    --template mistral \
+    --model_name_or_path meta-llama/Meta-Llama-3-8B-Instruct \
+    --template llama3 \
     --infer_backend vllm \
     --vllm_enforce_eager
 ```
 
-### Use ModelScope Hub
+### Download from ModelScope Hub
 
 If you have trouble with downloading models and datasets from Hugging Face, you can use ModelScope.
 
 ```bash
 export USE_MODELSCOPE_HUB=1 # `set USE_MODELSCOPE_HUB=1` for Windows
 ```
 
-Train the model by specifying a model ID of the ModelScope Hub as the `--model_name_or_path`. You can find a full list of model IDs at [ModelScope Hub](https://modelscope.cn/models), e.g., `modelscope/Llama-2-7b-ms`.
+Train the model by specifying a model ID of the ModelScope Hub as the `--model_name_or_path`. You can find a full list of model IDs at [ModelScope Hub](https://modelscope.cn/models), e.g., `LLM-Research/Meta-Llama-3-8B-Instruct`.
 
 ## Projects using LLaMA Factory
 
 If you have a project that should be incorporated, please contact via email or create a pull request.
 
 <details><summary>Click to show</summary>
 
@@ -440,15 +457,15 @@
 
 </details>
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
-Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
+Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2/LLaVA-1.5](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Phi-3](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/LICENSE) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
 @article{zheng2024llamafactory,
```

### Comparing `llmtuner-0.6.3/pyproject.toml` & `llmtuner-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/setup.py` & `llmtuner-0.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,17 @@
         lines = [line.strip() for line in file_content.strip().split("\n") if not line.startswith("#")]
         return lines
 
 
 extra_require = {
     "deepspeed": ["deepspeed>=0.10.0"],
     "metrics": ["nltk", "jieba", "rouge-chinese"],
-    "unsloth": ["torch==2.2.0", "unsloth[cu121-ampere-torch220]"],
     "galore": ["galore-torch"],
     "badam": ["badam"],
-    "vllm": ["vllm>=0.3.3"],
+    "vllm": ["vllm>=0.4.0"],
     "bitsandbytes": ["bitsandbytes>=0.39.0"],
     "gptq": ["optimum>=1.16.0", "auto-gptq>=0.5.0"],
     "awq": ["autoawq"],
     "aqlm": ["aqlm[gpu]>=1.1.0"],
     "qwen": ["tiktoken", "transformers_stream_generator"],
     "modelscope": ["modelscope"],
     "quality": ["ruff"],
```

### Comparing `llmtuner-0.6.3/src/llmtuner/api/app.py` & `llmtuner-0.7.0/src/llmtuner/api/app.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/api/protocol.py` & `llmtuner-0.7.0/src/llmtuner/api/protocol.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/chat/base_engine.py` & `llmtuner-0.7.0/src/llmtuner/chat/base_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Literal, Optional, Sequence, Union
 
 
 if TYPE_CHECKING:
+    from numpy.typing import NDArray
     from transformers import PreTrainedModel, PreTrainedTokenizer
     from vllm import AsyncLLMEngine
 
     from ..data import Template
     from ..hparams import DataArguments, FinetuningArguments, GeneratingArguments, ModelArguments
 
 
@@ -42,23 +43,25 @@
 
     @abstractmethod
     async def chat(
         self,
         messages: Sequence[Dict[str, str]],
         system: Optional[str] = None,
         tools: Optional[str] = None,
+        image: Optional["NDArray"] = None,
         **input_kwargs,
     ) -> List["Response"]: ...
 
     @abstractmethod
     async def stream_chat(
         self,
         messages: Sequence[Dict[str, str]],
         system: Optional[str] = None,
         tools: Optional[str] = None,
+        image: Optional["NDArray"] = None,
         **input_kwargs,
     ) -> AsyncGenerator[str, None]: ...
 
     @abstractmethod
     async def get_scores(
         self,
         batch_input: List[str],
```

### Comparing `llmtuner-0.6.3/src/llmtuner/chat/chat_model.py` & `llmtuner-0.7.0/src/llmtuner/chat/chat_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from ..hparams import get_infer_args
 from .hf_engine import HuggingfaceEngine
 from .vllm_engine import VllmEngine
 
 
 if TYPE_CHECKING:
+    from numpy.typing import NDArray
+
     from .base_engine import BaseEngine, Response
 
 
 def _start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
     asyncio.set_event_loop(loop)
     loop.run_forever()
 
@@ -32,51 +34,55 @@
         asyncio.run_coroutine_threadsafe(self.engine.start(), self._loop)
 
     def chat(
         self,
         messages: Sequence[Dict[str, str]],
         system: Optional[str] = None,
         tools: Optional[str] = None,
+        image: Optional["NDArray"] = None,
         **input_kwargs,
     ) -> List["Response"]:
-        task = asyncio.run_coroutine_threadsafe(self.achat(messages, system, tools, **input_kwargs), self._loop)
+        task = asyncio.run_coroutine_threadsafe(self.achat(messages, system, tools, image, **input_kwargs), self._loop)
         return task.result()
 
     async def achat(
         self,
         messages: Sequence[Dict[str, str]],
         system: Optional[str] = None,
         tools: Optional[str] = None,
+        image: Optional["NDArray"] = None,
         **input_kwargs,
     ) -> List["Response"]:
-        return await self.engine.chat(messages, system, tools, **input_kwargs)
+        return await self.engine.chat(messages, system, tools, image, **input_kwargs)
 
     def stream_chat(
         self,
         messages: Sequence[Dict[str, str]],
         system: Optional[str] = None,
         tools: Optional[str] = None,
+        image: Optional["NDArray"] = None,
         **input_kwargs,
     ) -> Generator[str, None, None]:
-        generator = self.astream_chat(messages, system, tools, **input_kwargs)
+        generator = self.astream_chat(messages, system, tools, image, **input_kwargs)
         while True:
             try:
                 task = asyncio.run_coroutine_threadsafe(generator.__anext__(), self._loop)
                 yield task.result()
             except StopAsyncIteration:
                 break
 
     async def astream_chat(
         self,
         messages: Sequence[Dict[str, str]],
         system: Optional[str] = None,
         tools: Optional[str] = None,
+        image: Optional["NDArray"] = None,
         **input_kwargs,
     ) -> AsyncGenerator[str, None]:
-        async for new_token in self.engine.stream_chat(messages, system, tools, **input_kwargs):
+        async for new_token in self.engine.stream_chat(messages, system, tools, image, **input_kwargs):
             yield new_token
 
     def get_scores(
         self,
         batch_input: List[str],
         **input_kwargs,
     ) -> List[float]:
```

### Comparing `llmtuner-0.6.3/src/llmtuner/chat/hf_engine.py` & `llmtuner-0.7.0/src/llmtuner/chat/hf_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from ..data import get_template_and_fix_tokenizer
 from ..extras.misc import get_logits_processor
 from ..model import load_model, load_tokenizer
 from .base_engine import BaseEngine, Response
 
 
 if TYPE_CHECKING:
-    from transformers import PreTrainedModel, PreTrainedTokenizer
+    from numpy.typing import NDArray
+    from transformers import PreTrainedModel, PreTrainedTokenizer, ProcessorMixin
+    from transformers.image_processing_utils import BaseImageProcessor
     from trl import PreTrainedModelWrapper
 
     from ..data import Template
     from ..hparams import DataArguments, FinetuningArguments, GeneratingArguments, ModelArguments
 
 
 class HuggingfaceEngine(BaseEngine):
@@ -26,33 +28,40 @@
         self,
         model_args: "ModelArguments",
         data_args: "DataArguments",
         finetuning_args: "FinetuningArguments",
         generating_args: "GeneratingArguments",
     ) -> None:
         self.can_generate = finetuning_args.stage == "sft"
-        self.tokenizer = load_tokenizer(model_args)
+        tokenizer_module = load_tokenizer(model_args)
+        self.tokenizer = tokenizer_module["tokenizer"]
+        self.processor = tokenizer_module["processor"]
         self.tokenizer.padding_side = "left" if self.can_generate else "right"
         self.template = get_template_and_fix_tokenizer(self.tokenizer, data_args.template)
         self.model = load_model(
             self.tokenizer, model_args, finetuning_args, is_trainable=False, add_valuehead=(not self.can_generate)
         )  # must after fixing tokenizer to resize vocab
         self.generating_args = generating_args.to_dict()
 
     @staticmethod
     def _process_args(
         model: "PreTrainedModel",
         tokenizer: "PreTrainedTokenizer",
+        processor: Optional["ProcessorMixin"],
         template: "Template",
         generating_args: Dict[str, Any],
         messages: Sequence[Dict[str, str]],
         system: Optional[str] = None,
         tools: Optional[str] = None,
+        image: Optional["NDArray"] = None,
         input_kwargs: Optional[Dict[str, Any]] = {},
     ) -> Tuple[Dict[str, Any], int]:
+        if processor is not None and image is not None and "<image>" not in messages[0]["content"]:
+            messages[0]["content"] = "<image>" + messages[0]["content"]
+
         paired_messages = messages + [{"role": "assistant", "content": ""}]
         prompt_ids, _ = template.encode_oneturn(
             tokenizer=tokenizer, messages=paired_messages, system=system, tools=tools
         )
         prompt_length = len(prompt_ids)
         inputs = torch.tensor([prompt_ids], device=model.device)
 
@@ -91,30 +100,37 @@
 
         gen_kwargs = dict(
             inputs=inputs,
             generation_config=GenerationConfig(**generating_args),
             logits_processor=get_logits_processor(),
         )
 
+        if processor is not None and image is not None:
+            image_processor: "BaseImageProcessor" = getattr(processor, "image_processor")
+            pixel_values: "torch.Tensor" = image_processor(image, return_tensors="pt")["pixel_values"]
+            gen_kwargs["pixel_values"] = pixel_values.to(model.device)
+
         return gen_kwargs, prompt_length
 
     @staticmethod
     @torch.inference_mode()
     def _chat(
         model: "PreTrainedModel",
         tokenizer: "PreTrainedTokenizer",
+        processor: Optional["ProcessorMixin"],
         template: "Template",
         generating_args: Dict[str, Any],
         messages: Sequence[Dict[str, str]],
         system: Optional[str] = None,
         tools: Optional[str] = None,
+        image: Optional["NDArray"] = None,
         input_kwargs: Optional[Dict[str, Any]] = {},
     ) -> List["Response"]:
         gen_kwargs, prompt_length = HuggingfaceEngine._process_args(
-            model, tokenizer, template, generating_args, messages, system, tools, input_kwargs
+            model, tokenizer, processor, template, generating_args, messages, system, tools, image, input_kwargs
         )
         generate_output = model.generate(**gen_kwargs)
         response_ids = generate_output[:, prompt_length:]
         response = tokenizer.batch_decode(response_ids, skip_special_tokens=True, clean_up_tokenization_spaces=True)
         results = []
         for i in range(len(response)):
             eos_index = (response_ids[i] == tokenizer.eos_token_id).nonzero()
@@ -131,23 +147,25 @@
         return results
 
     @staticmethod
     @torch.inference_mode()
     def _stream_chat(
         model: "PreTrainedModel",
         tokenizer: "PreTrainedTokenizer",
+        processor: Optional["ProcessorMixin"],
         template: "Template",
         generating_args: Dict[str, Any],
         messages: Sequence[Dict[str, str]],
         system: Optional[str] = None,
         tools: Optional[str] = None,
+        image: Optional["NDArray"] = None,
         input_kwargs: Optional[Dict[str, Any]] = {},
     ) -> Callable[[], str]:
         gen_kwargs, _ = HuggingfaceEngine._process_args(
-            model, tokenizer, template, generating_args, messages, system, tools, input_kwargs
+            model, tokenizer, processor, template, generating_args, messages, system, tools, image, input_kwargs
         )
         streamer = TextIteratorStreamer(tokenizer, skip_prompt=True, skip_special_tokens=True)
         gen_kwargs["streamer"] = streamer
         thread = Thread(target=model.generate, kwargs=gen_kwargs, daemon=True)
         thread.start()
 
         def stream():
@@ -195,53 +213,59 @@
         self._semaphore = asyncio.Semaphore(int(os.environ.get("MAX_CONCURRENT", 1)))
 
     async def chat(
         self,
         messages: Sequence[Dict[str, str]],
         system: Optional[str] = None,
         tools: Optional[str] = None,
+        image: Optional["NDArray"] = None,
         **input_kwargs,
     ) -> List["Response"]:
         if not self.can_generate:
             raise ValueError("The current model does not support `chat`.")
 
         loop = asyncio.get_running_loop()
         input_args = (
             self.model,
             self.tokenizer,
+            self.processor,
             self.template,
             self.generating_args,
             messages,
             system,
             tools,
+            image,
             input_kwargs,
         )
         async with self._semaphore:
             with concurrent.futures.ThreadPoolExecutor() as pool:
                 return await loop.run_in_executor(pool, self._chat, *input_args)
 
     async def stream_chat(
         self,
         messages: Sequence[Dict[str, str]],
         system: Optional[str] = None,
         tools: Optional[str] = None,
+        image: Optional["NDArray"] = None,
         **input_kwargs,
     ) -> AsyncGenerator[str, None]:
         if not self.can_generate:
             raise ValueError("The current model does not support `stream_chat`.")
 
         loop = asyncio.get_running_loop()
         input_args = (
             self.model,
             self.tokenizer,
+            self.processor,
             self.template,
             self.generating_args,
             messages,
             system,
             tools,
+            image,
             input_kwargs,
         )
         async with self._semaphore:
             with concurrent.futures.ThreadPoolExecutor() as pool:
                 stream = self._stream_chat(*input_args)
                 while True:
                     try:
```

### Comparing `llmtuner-0.6.3/src/llmtuner/data/aligner.py` & `llmtuner-0.7.0/src/llmtuner/data/aligner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from functools import partial
 from typing import TYPE_CHECKING, Any, Dict, List, Union
 
 from datasets import Features
 
 from .utils import Role
 
@@ -9,16 +10,31 @@
 if TYPE_CHECKING:
     from datasets import Dataset, IterableDataset
 
     from ..hparams import DataArguments
     from .parser import DatasetAttr
 
 
-def convert_alpaca(examples: Dict[str, List[Any]], dataset_attr: "DatasetAttr") -> Dict[str, List[Any]]:
-    outputs = {"prompt": [], "response": [], "system": [], "tools": []}
+def _convert_images(images: List[Any], dataset_attr: "DatasetAttr", data_args: "DataArguments") -> List[Any]:
+    outputs = []
+    if dataset_attr.load_from in ["script", "file"]:
+        for image in images:
+            if isinstance(image, str) and os.path.isfile(os.path.join(data_args.dataset_dir, image)):
+                outputs.append(os.path.join(data_args.dataset_dir, image))
+            else:
+                outputs.append(image)
+
+    return outputs
+
+
+def convert_alpaca(
+    examples: Dict[str, List[Any]], dataset_attr: "DatasetAttr", data_args: "DataArguments"
+) -> Dict[str, List[Any]]:
+    outputs = {"prompt": [], "response": [], "system": [], "tools": [], "images": []}
+    convert_images = partial(_convert_images, dataset_attr=dataset_attr, data_args=data_args)
     for i in range(len(examples[dataset_attr.prompt])):
         prompt = []
         if dataset_attr.history and isinstance(examples[dataset_attr.history][i], list):
             for old_prompt, old_response in examples[dataset_attr.history][i]:
                 prompt.append({"role": Role.USER.value, "content": old_prompt})
                 prompt.append({"role": Role.ASSISTANT.value, "content": old_response})
 
@@ -40,20 +56,24 @@
         else:
             response = []
 
         outputs["prompt"].append(prompt)
         outputs["response"].append(response)
         outputs["system"].append(examples[dataset_attr.system][i] if dataset_attr.system else "")
         outputs["tools"].append("")
+        outputs["images"].append(convert_images(examples[dataset_attr.images][i]) if dataset_attr.images else [])
 
     return outputs
 
 
-def convert_sharegpt(examples: Dict[str, List[Any]], dataset_attr: "DatasetAttr") -> Dict[str, List[Any]]:
-    outputs = {"prompt": [], "response": [], "system": [], "tools": []}
+def convert_sharegpt(
+    examples: Dict[str, List[Any]], dataset_attr: "DatasetAttr", data_args: "DataArguments"
+) -> Dict[str, List[Any]]:
+    outputs = {"prompt": [], "response": [], "system": [], "tools": [], "images": []}
+    convert_images = partial(_convert_images, dataset_attr=dataset_attr, data_args=data_args)
     tag_mapping = {
         dataset_attr.user_tag: Role.USER.value,
         dataset_attr.assistant_tag: Role.ASSISTANT.value,
         dataset_attr.observation_tag: Role.OBSERVATION.value,
         dataset_attr.function_tag: Role.FUNCTION.value,
         dataset_attr.system_tag: Role.SYSTEM.value,
     }
@@ -80,44 +100,47 @@
                 {"role": tag_mapping[message[dataset_attr.role_tag]], "content": message[dataset_attr.content_tag]}
             )
 
         outputs["prompt"].append(aligned_messages[:-1])
         outputs["response"].append(aligned_messages[-1:])
         outputs["system"].append(system)
         outputs["tools"].append(examples[dataset_attr.tools][i] if dataset_attr.tools else "")
+        outputs["images"].append(convert_images(examples[dataset_attr.images][i]) if dataset_attr.images else [])
 
     return outputs
 
 
 def align_dataset(
     dataset: Union["Dataset", "IterableDataset"], dataset_attr: "DatasetAttr", data_args: "DataArguments"
 ) -> Union["Dataset", "IterableDataset"]:
     r"""
     Aligned dataset:
         prompt: [{"role": "user", "content": "..."}] * (2T - 1)
         response: [{"role": "assistant", "content": "..."}] * N (N > 1 for ranking dataset)
         system: "..."
-        tools: "..."
+        tools: "...",
+        images: [],
     """
     if dataset_attr.formatting == "alpaca":
-        convert_func = partial(convert_alpaca, dataset_attr=dataset_attr)
+        convert_func = partial(convert_alpaca, dataset_attr=dataset_attr, data_args=data_args)
     else:
-        convert_func = partial(convert_sharegpt, dataset_attr=dataset_attr)
+        convert_func = partial(convert_sharegpt, dataset_attr=dataset_attr, data_args=data_args)
 
     column_names = list(next(iter(dataset)).keys())
     features = Features.from_dict(
         {
             "prompt": [
                 {"role": {"dtype": "string", "_type": "Value"}, "content": {"dtype": "string", "_type": "Value"}}
             ],
             "response": [
                 {"role": {"dtype": "string", "_type": "Value"}, "content": {"dtype": "string", "_type": "Value"}}
             ],
             "system": {"dtype": "string", "_type": "Value"},
             "tools": {"dtype": "string", "_type": "Value"},
+            "images": [{"_type": "Image"}],
         }
     )
     kwargs = {}
     if not data_args.streaming:
         kwargs = dict(
             num_proc=data_args.preprocessing_num_workers,
             load_from_cache_file=(not data_args.overwrite_cache),
```

### Comparing `llmtuner-0.6.3/src/llmtuner/data/collator.py` & `llmtuner-0.7.0/src/llmtuner/data/collator.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/data/formatter.py` & `llmtuner-0.7.0/src/llmtuner/data/formatter.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/data/loader.py` & `llmtuner-0.7.0/src/llmtuner/data/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 import os
-from typing import TYPE_CHECKING, Literal, Union
+from typing import TYPE_CHECKING, Literal, Optional, Union
 
 from datasets import load_dataset, load_from_disk
 
 from ..extras.constants import FILEEXT2TYPE
 from ..extras.logging import get_logger
 from ..extras.misc import has_tokenized_data
 from .aligner import align_dataset
@@ -12,15 +12,15 @@
 from .preprocess import get_preprocess_and_print_func
 from .template import get_template_and_fix_tokenizer
 from .utils import checksum, merge_dataset
 
 
 if TYPE_CHECKING:
     from datasets import Dataset, IterableDataset
-    from transformers import Seq2SeqTrainingArguments
+    from transformers import ProcessorMixin, Seq2SeqTrainingArguments
     from transformers.tokenization_utils import PreTrainedTokenizer
 
     from ..hparams import DataArguments, ModelArguments
     from .parser import DatasetAttr
 
 
 logger = get_logger(__name__)
@@ -111,19 +111,20 @@
         num_samples = min(data_args.max_samples, len(dataset))
         dataset = dataset.select(range(num_samples))
 
     return align_dataset(dataset, dataset_attr, data_args)
 
 
 def get_dataset(
-    tokenizer: "PreTrainedTokenizer",
     model_args: "ModelArguments",
     data_args: "DataArguments",
     training_args: "Seq2SeqTrainingArguments",
     stage: Literal["pt", "sft", "rm", "ppo"],
+    tokenizer: "PreTrainedTokenizer",
+    processor: Optional["ProcessorMixin"] = None,
 ) -> Union["Dataset", "IterableDataset"]:
     template = get_template_and_fix_tokenizer(tokenizer, data_args.template)
     if data_args.train_on_prompt and template.efficient_eos:
         raise ValueError("Current template does not support `train_on_prompt`.")
 
     # Load tokenized dataset
     if data_args.tokenized_path is not None:
@@ -145,15 +146,15 @@
                 raise ValueError("The dataset is not applicable in the current training stage.")
 
             all_datasets.append(load_single_dataset(dataset_attr, model_args, data_args))
         dataset = merge_dataset(all_datasets, data_args, training_args)
 
     with training_args.main_process_first(desc="pre-process dataset"):
         preprocess_func, print_function = get_preprocess_and_print_func(
-            tokenizer, template, data_args, training_args, stage
+            data_args, training_args, stage, template, tokenizer, processor
         )
         column_names = list(next(iter(dataset)).keys())
         kwargs = {}
         if not data_args.streaming:
             kwargs = dict(
                 num_proc=data_args.preprocessing_num_workers,
                 load_from_cache_file=(not data_args.overwrite_cache),
```

### Comparing `llmtuner-0.6.3/src/llmtuner/data/parser.py` & `llmtuner-0.7.0/src/llmtuner/data/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     file_sha1: Optional[str] = None
     subset: Optional[str] = None
     folder: Optional[str] = None
     ranking: bool = False
     formatting: Literal["alpaca", "sharegpt"] = "alpaca"
     """ columns """
     system: Optional[str] = None
+    images: Optional[str] = None
     """ columns for the alpaca format """
     prompt: Optional[str] = "instruction"
     query: Optional[str] = "input"
     response: Optional[str] = "output"
     history: Optional[str] = None
     """ columns for the sharegpt format """
     messages: Optional[str] = "conversations"
@@ -101,15 +102,15 @@
         dataset_attr.set_attr("file_sha1", dataset_info[name])
         dataset_attr.set_attr("subset", dataset_info[name])
         dataset_attr.set_attr("folder", dataset_info[name])
         dataset_attr.set_attr("ranking", dataset_info[name], default=False)
         dataset_attr.set_attr("formatting", dataset_info[name], default="alpaca")
 
         if "columns" in dataset_info[name]:
-            column_names = ["system"]
+            column_names = ["system", "images"]
             if dataset_attr.formatting == "alpaca":
                 column_names.extend(["prompt", "query", "response", "history"])
             else:
                 column_names.extend(["messages", "tools"])
 
             for column_name in column_names:
                 dataset_attr.set_attr(column_name, dataset_info[name]["columns"])
```

### Comparing `llmtuner-0.6.3/src/llmtuner/data/template.py` & `llmtuner-0.7.0/src/llmtuner/data/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -499,24 +499,26 @@
 )
 
 
 _register_template(
     name="chatml",
     format_user=StringFormatter(slots=["<|im_start|>user\n{{content}}<|im_end|>\n<|im_start|>assistant\n"]),
     format_system=StringFormatter(slots=["<|im_start|>system\n{{content}}<|im_end|>\n"]),
+    format_observation=StringFormatter(slots=["<|im_start|>tool\n{{content}}<|im_end|>\n<|im_start|>assistant\n"]),
     format_separator=EmptyFormatter(slots=["\n"]),
     stop_words=["<|im_end|>", "<|im_start|>"],
     replace_eos=True,
 )
 
 
 _register_template(
     name="chatml_de",
     format_user=StringFormatter(slots=["<|im_start|>user\n{{content}}<|im_end|>\n<|im_start|>assistant\n"]),
     format_system=StringFormatter(slots=["<|im_start|>system\n{{content}}<|im_end|>\n"]),
+    format_observation=StringFormatter(slots=["<|im_start|>tool\n{{content}}<|im_end|>\n<|im_start|>assistant\n"]),
     format_separator=EmptyFormatter(slots=["\n"]),
     default_system="Du bist ein freundlicher und hilfsbereiter KI-Assistent.",
     stop_words=["<|im_end|>", "<|im_start|>"],
     replace_eos=True,
 )
 
 
@@ -547,14 +549,40 @@
     format_user=StringFormatter(slots=["<用户>{{content}}<AI>"]),
     format_system=StringFormatter(slots=[{"bos_token"}, "{{content}}"]),
     force_system=True,
 )
 
 
 _register_template(
+    name="dbrx",
+    format_user=StringFormatter(slots=["<|im_start|>user\n{{content}}<|im_end|>\n<|im_start|>assistant\n"]),
+    format_system=StringFormatter(slots=["<|im_start|>system\n{{content}}<|im_end|>\n"]),
+    format_observation=StringFormatter(slots=["<|im_start|>tool\n{{content}}<|im_end|>\n<|im_start|>assistant\n"]),
+    format_separator=EmptyFormatter(slots=["\n"]),
+    default_system=(
+        "You are DBRX, created by Databricks. You were last updated in December 2023. "
+        "You answer questions based on information available up to that point.\n"
+        "YOU PROVIDE SHORT RESPONSES TO SHORT QUESTIONS OR STATEMENTS, but provide thorough "
+        "responses to more complex and open-ended questions.\nYou assist with various tasks, "
+        "from writing to coding (using markdown for code blocks — remember to use ``` with "
+        "code, JSON, and tables).\n(You do not have real-time data access or code execution "
+        "capabilities. You avoid stereotyping and provide balanced perspectives on "
+        "controversial topics. You do not provide song lyrics, poems, or news articles and "
+        "do not divulge details of your training data.)\nThis is your system prompt, "
+        "guiding your responses. Do not reference it, just respond to the user. If you find "
+        "yourself talking about this message, stop. You should be responding appropriately "
+        "and usually that means not mentioning this.\nYOU DO NOT MENTION ANY OF THIS INFORMATION "
+        "ABOUT YOURSELF UNLESS THE INFORMATION IS DIRECTLY PERTINENT TO THE USER'S QUERY."
+    ),
+    stop_words=["<|im_end|>"],
+    replace_eos=True,
+)
+
+
+_register_template(
     name="deepseek",
     format_user=StringFormatter(slots=["User: {{content}}\n\nAssistant:"]),
     format_system=StringFormatter(slots=[{"bos_token"}, "{{content}}"]),
     force_system=True,
 )
 
 
@@ -604,14 +632,17 @@
 )
 
 
 _register_template(
     name="gemma",
     format_user=StringFormatter(slots=["<start_of_turn>user\n{{content}}<end_of_turn>\n<start_of_turn>model\n"]),
     format_system=StringFormatter(slots=[{"bos_token"}, "{{content}}"]),
+    format_observation=StringFormatter(
+        slots=["<start_of_turn>tool\n{{content}}<end_of_turn>\n<start_of_turn>model\n"]
+    ),
     format_separator=EmptyFormatter(slots=["<end_of_turn>\n"]),
     efficient_eos=True,
     force_system=True,
 )
 
 
 _register_template(
@@ -674,14 +705,22 @@
                 "<|start_header_id|>assistant<|end_header_id|>\n\n"
             )
         ]
     ),
     format_system=StringFormatter(
         slots=[{"bos_token"}, "<|start_header_id|>system<|end_header_id|>\n\n{{content}}<|eot_id|>"]
     ),
+    format_observation=StringFormatter(
+        slots=[
+            (
+                "<|start_header_id|>tool<|end_header_id|>\n\n{{content}}<|eot_id|>"
+                "<|start_header_id|>assistant<|end_header_id|>\n\n"
+            )
+        ]
+    ),
     default_system="You are a helpful assistant.",
     stop_words=["<|eot_id|>"],
     replace_eos=True,
 )
 
 
 _register_template(
@@ -715,17 +754,30 @@
     format_user=StringFormatter(slots=["Human: {{content}}\n\nAssistant: ", {"eos_token"}]),
     format_system=StringFormatter(slots=[{"bos_token"}, "{{content}}"]),
     force_system=True,
 )
 
 
 _register_template(
+    name="phi",
+    format_user=StringFormatter(slots=["<|user|>\n{{content}}<|end|>\n<|assistant|>\n"]),
+    format_system=StringFormatter(slots=[{"bos_token"}, "<|system|>\n{{content}}<|end|>\n"]),
+    format_observation=StringFormatter(slots=["<|function_output|>\n{{content}}<|end|>\n<|assistant|>\n"]),
+    format_separator=EmptyFormatter(slots=["\n"]),
+    default_system="You are a helpful AI assistant.",
+    stop_words=["<|end|>"],
+    replace_eos=True,
+)
+
+
+_register_template(
     name="qwen",
     format_user=StringFormatter(slots=["<|im_start|>user\n{{content}}<|im_end|>\n<|im_start|>assistant\n"]),
     format_system=StringFormatter(slots=["<|im_start|>system\n{{content}}<|im_end|>\n"]),
+    format_observation=StringFormatter(slots=["<|im_start|>tool\n{{content}}<|im_end|>\n<|im_start|>assistant\n"]),
     format_separator=EmptyFormatter(slots=["\n"]),
     default_system="You are a helpful assistant.",
     stop_words=["<|im_end|>"],
     replace_eos=True,
 )
 
 
@@ -814,15 +866,15 @@
 
 
 _register_template(
     name="zephyr",
     format_user=StringFormatter(slots=["<|user|>\n{{content}}", {"eos_token"}, "<|assistant|>"]),
     format_assistant=StringFormatter(slots=["\n{{content}}", {"eos_token"}]),
     format_system=StringFormatter(slots=["<|system|>\n{{content}}", {"eos_token"}]),
-    default_system="You are a friendly chatbot who always responds in the style of a pirate",
+    default_system="You are Zephyr, a helpful assistant.",
 )
 
 
 _register_template(
     name="ziya",
     format_user=StringFormatter(slots=["<human>:{{content}}\n<bot>:"]),
     format_separator=EmptyFormatter(slots=["\n"]),
```

### Comparing `llmtuner-0.6.3/src/llmtuner/data/utils.py` & `llmtuner-0.7.0/src/llmtuner/data/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 
 def split_dataset(
     dataset: Union["Dataset", "IterableDataset"], data_args: "DataArguments", training_args: "Seq2SeqTrainingArguments"
 ) -> Dict[str, "Dataset"]:
     if training_args.do_train:
         if data_args.val_size > 1e-6:  # Split the dataset
             if data_args.streaming:
+                dataset = dataset.shuffle(buffer_size=data_args.buffer_size, seed=training_args.seed)
                 val_set = dataset.take(int(data_args.val_size))
                 train_set = dataset.skip(int(data_args.val_size))
-                dataset = dataset.shuffle(buffer_size=data_args.buffer_size, seed=training_args.seed)
                 return {"train_dataset": train_set, "eval_dataset": val_set}
             else:
                 val_size = int(data_args.val_size) if data_args.val_size > 1 else data_args.val_size
                 dataset = dataset.train_test_split(test_size=val_size, seed=training_args.seed)
                 return {"train_dataset": dataset["train"], "eval_dataset": dataset["test"]}
         else:
             if data_args.streaming:
```

### Comparing `llmtuner-0.6.3/src/llmtuner/eval/evaluator.py` & `llmtuner-0.7.0/src/llmtuner/eval/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ..model import load_model, load_tokenizer
 from .template import get_eval_template
 
 
 class Evaluator:
     def __init__(self, args: Optional[Dict[str, Any]] = None) -> None:
         self.model_args, self.data_args, self.eval_args, finetuning_args = get_eval_args(args)
-        self.tokenizer = load_tokenizer(self.model_args)
+        self.tokenizer = load_tokenizer(self.model_args)["tokenizer"]
         self.tokenizer.padding_side = "right"  # avoid overflow issue in batched inference for llama2
         self.template = get_template_and_fix_tokenizer(self.tokenizer, self.data_args.template)
         self.model = load_model(self.tokenizer, self.model_args, finetuning_args)
         self.eval_template = get_eval_template(self.eval_args.lang)
         self.choice_inputs = [
             self.tokenizer.encode(self.eval_template.prefix + ch, add_special_tokens=False)[-1] for ch in CHOICES
         ]
```

### Comparing `llmtuner-0.6.3/src/llmtuner/eval/template.py` & `llmtuner-0.7.0/src/llmtuner/eval/template.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/extras/callbacks.py` & `llmtuner-0.7.0/src/llmtuner/extras/callbacks.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/extras/constants.py` & `llmtuner-0.7.0/src/llmtuner/extras/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 LAYERNORM_NAMES = {"norm", "ln"}
 
 LOG_FILE_NAME = "trainer_log.jsonl"
 
 METHODS = ["full", "freeze", "lora"]
 
+MLLM_LIST = ["LLaVA1.5"]
+
 MOD_SUPPORTED_MODELS = ["bloom", "falcon", "gemma", "llama", "mistral", "mixtral", "phi", "starcoder2"]
 
 PEFT_METHODS = ["lora"]
 
 SUBJECTS = ["Average", "STEM", "Social Sciences", "Humanities", "Other"]
 
 SUPPORTED_MODELS = OrderedDict()
@@ -43,14 +45,16 @@
     "DPO": "dpo",
     "ORPO": "orpo",
     "Pre-Training": "pt",
 }
 
 STAGES_USE_PAIR_DATA = ["rm", "dpo", "orpo"]
 
+SUPPORTED_CLASS_FOR_S2ATTN = ["llama"]
+
 V_HEAD_WEIGHTS_NAME = "value_head.bin"
 
 V_HEAD_SAFE_WEIGHTS_NAME = "value_head.safetensors"
 
 
 class DownloadSource(str, Enum):
     DEFAULT = "hf"
@@ -264,14 +268,30 @@
     },
     template="cohere",
 )
 
 
 register_model_group(
     models={
+        "DBRX-132B-Base": {
+            DownloadSource.DEFAULT: "databricks/dbrx-base",
+            DownloadSource.MODELSCOPE: "AI-ModelScope/dbrx-base",
+        },
+        "DBRX-132B-Chat": {
+            DownloadSource.DEFAULT: "databricks/dbrx-instruct",
+            DownloadSource.MODELSCOPE: "AI-ModelScope/dbrx-instruct",
+        },
+    },
+    module="Wqkv",
+    template="dbrx",
+)
+
+
+register_model_group(
+    models={
         "DeepSeek-LLM-7B-Base": {
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-llm-7b-base",
             DownloadSource.MODELSCOPE: "deepseek-ai/deepseek-llm-7b-base",
         },
         "DeepSeek-LLM-67B-Base": {
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-llm-67b-base",
             DownloadSource.MODELSCOPE: "deepseek-ai/deepseek-llm-67b-base",
@@ -282,17 +302,19 @@
         },
         "DeepSeek-LLM-67B-Chat": {
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-llm-67b-chat",
             DownloadSource.MODELSCOPE: "deepseek-ai/deepseek-llm-67b-chat",
         },
         "DeepSeek-Math-7B-Base": {
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-math-7b-base",
+            DownloadSource.MODELSCOPE: "deepseek-ai/deepseek-math-7b-base",
         },
         "DeepSeek-Math-7B-Chat": {
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-math-7b-instruct",
+            DownloadSource.MODELSCOPE: "deepseek-ai/deepseek-math-7b-instruct",
         },
         "DeepSeek-MoE-16B-Base": {
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-moe-16b-base",
             DownloadSource.MODELSCOPE: "deepseek-ai/deepseek-moe-16b-base",
         },
         "DeepSeek-MoE-16B-Chat": {
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-moe-16b-chat",
@@ -449,14 +471,24 @@
     module="wqkv",
     template="intern2",
 )
 
 
 register_model_group(
     models={
+        "Jambda-v0.1": {
+            DownloadSource.DEFAULT: "ai21labs/Jamba-v0.1",
+            DownloadSource.MODELSCOPE: "AI-ModelScope/Jamba-v0.1",
+        }
+    },
+)
+
+
+register_model_group(
+    models={
         "LingoWhale-8B": {
             DownloadSource.DEFAULT: "deeplang-ai/LingoWhale-8B",
             DownloadSource.MODELSCOPE: "DeepLang/LingoWhale-8B",
         }
     },
     module="qkv_proj",
 )
@@ -536,14 +568,27 @@
     },
     template="llama3",
 )
 
 
 register_model_group(
     models={
+        "LLaVA1.5-7B-Chat": {
+            DownloadSource.DEFAULT: "llava-hf/llava-1.5-7b-hf",
+        },
+        "LLaVA1.5-13B-Chat": {
+            DownloadSource.DEFAULT: "llava-hf/llava-1.5-13b-hf",
+        },
+    },
+    template="vicuna",
+)
+
+
+register_model_group(
+    models={
         "Mistral-7B-v0.1": {
             DownloadSource.DEFAULT: "mistralai/Mistral-7B-v0.1",
             DownloadSource.MODELSCOPE: "AI-ModelScope/Mistral-7B-v0.1",
         },
         "Mistral-7B-v0.1-Chat": {
             DownloadSource.DEFAULT: "mistralai/Mistral-7B-Instruct-v0.1",
             DownloadSource.MODELSCOPE: "AI-ModelScope/Mistral-7B-Instruct-v0.1",
@@ -569,46 +614,44 @@
         },
         "Mixtral-8x7B-v0.1-Chat": {
             DownloadSource.DEFAULT: "mistralai/Mixtral-8x7B-Instruct-v0.1",
             DownloadSource.MODELSCOPE: "AI-ModelScope/Mixtral-8x7B-Instruct-v0.1",
         },
         "Mixtral-8x22B-v0.1": {
             DownloadSource.DEFAULT: "mistralai/Mixtral-8x22B-v0.1",
+            DownloadSource.MODELSCOPE: "AI-ModelScope/Mixtral-8x22B-v0.1",
         },
         "Mixtral-8x22B-v0.1-Chat": {
             DownloadSource.DEFAULT: "mistralai/Mixtral-8x22B-Instruct-v0.1",
         },
     },
     template="mistral",
 )
 
 
 register_model_group(
     models={
         "OLMo-1B": {
-            DownloadSource.DEFAULT: "allenai/OLMo-1B",
+            DownloadSource.DEFAULT: "allenai/OLMo-1B-hf",
         },
         "OLMo-7B": {
-            DownloadSource.DEFAULT: "allenai/OLMo-7B",
-            DownloadSource.MODELSCOPE: "AI-ModelScope/OLMo-7B",
+            DownloadSource.DEFAULT: "allenai/OLMo-7B-hf",
         },
-        "OLMo-7B-Chat": {
-            DownloadSource.DEFAULT: "allenai/OLMo-7B-Instruct",
+        "OLMo-1.7-7B": {
+            DownloadSource.DEFAULT: "allenai/OLMo-1.7-7B-hf",
         },
     },
-    module="att_proj",
-    template="olmo",
 )
 
 
 register_model_group(
     models={
         "OpenChat3.5-7B-Chat": {
             DownloadSource.DEFAULT: "openchat/openchat-3.5-0106",
-            DownloadSource.MODELSCOPE: "myxiongmodel/openchat_3.5",
+            DownloadSource.MODELSCOPE: "xcwzxcwz/openchat-3.5-0106",
         }
     },
     template="openchat",
 )
 
 
 register_model_group(
@@ -650,14 +693,30 @@
         },
     }
 )
 
 
 register_model_group(
     models={
+        "Phi3-3.8B-4k-Chat": {
+            DownloadSource.DEFAULT: "microsoft/Phi-3-mini-4k-instruct",
+            DownloadSource.DEFAULT: "LLM-Research/Phi-3-mini-4k-instruct",
+        },
+        "Phi3-3.8B-128k-Chat": {
+            DownloadSource.DEFAULT: "microsoft/Phi-3-mini-128k-instruct",
+            DownloadSource.DEFAULT: "LLM-Research/Phi-3-mini-128k-instruct",
+        },
+    },
+    module="qkv_proj",
+    template="phi",
+)
+
+
+register_model_group(
+    models={
         "Qwen-1.8B": {
             DownloadSource.DEFAULT: "Qwen/Qwen-1_8B",
             DownloadSource.MODELSCOPE: "qwen/Qwen-1_8B",
         },
         "Qwen-7B": {
             DownloadSource.DEFAULT: "Qwen/Qwen-7B",
             DownloadSource.MODELSCOPE: "qwen/Qwen-7B",
@@ -750,14 +809,18 @@
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-32B",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-32B",
         },
         "Qwen1.5-72B": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-72B",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-72B",
         },
+        "Qwen1.5-110B": {
+            DownloadSource.DEFAULT: "Qwen/Qwen1.5-110B",
+            DownloadSource.MODELSCOPE: "qwen/Qwen1.5-110B",
+        },
         "Qwen1.5-MoE-A2.7B": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-MoE-A2.7B",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-MoE-A2.7B",
         },
         "Qwen1.5-Code-7B": {
             DownloadSource.DEFAULT: "Qwen/CodeQwen1.5-7B",
             DownloadSource.MODELSCOPE: "qwen/CodeQwen1.5-7B",
@@ -786,14 +849,18 @@
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-32B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-32B-Chat",
         },
         "Qwen1.5-72B-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-72B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-72B-Chat",
         },
+        "Qwen1.5-110B-Chat": {
+            DownloadSource.DEFAULT: "Qwen/Qwen1.5-110B-Chat",
+            DownloadSource.MODELSCOPE: "qwen/Qwen1.5-110B-Chat",
+        },
         "Qwen1.5-MoE-A2.7B-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-MoE-A2.7B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-MoE-A2.7B-Chat",
         },
         "Qwen1.5-Code-7B-Chat": {
             DownloadSource.DEFAULT: "Qwen/CodeQwen1.5-7B-Chat",
             DownloadSource.MODELSCOPE: "qwen/CodeQwen1.5-7B-Chat",
@@ -846,14 +913,18 @@
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-72B-Chat-GPTQ-Int8",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-72B-Chat-GPTQ-Int8",
         },
         "Qwen1.5-72B-int4-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-72B-Chat-AWQ",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-72B-Chat-AWQ",
         },
+        "Qwen1.5-110B-int4-Chat": {
+            DownloadSource.DEFAULT: "Qwen/Qwen1.5-110B-Chat-AWQ",
+            DownloadSource.MODELSCOPE: "qwen/Qwen1.5-110B-Chat-AWQ",
+        },
         "Qwen1.5-MoE-A2.7B-int4-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4",
         },
         "Qwen1.5-Code-7B-int4-Chat": {
             DownloadSource.DEFAULT: "Qwen/CodeQwen1.5-7B-Chat-AWQ",
             DownloadSource.MODELSCOPE: "qwen/CodeQwen1.5-7B-Chat-AWQ",
@@ -887,20 +958,23 @@
 )
 
 
 register_model_group(
     models={
         "StarCoder2-3B": {
             DownloadSource.DEFAULT: "bigcode/starcoder2-3b",
+            DownloadSource.MODELSCOPE: "AI-ModelScope/starcoder2-3b",
         },
         "StarCoder2-7B": {
             DownloadSource.DEFAULT: "bigcode/starcoder2-7b",
+            DownloadSource.MODELSCOPE: "AI-ModelScope/starcoder2-7b",
         },
         "StarCoder2-15B": {
             DownloadSource.DEFAULT: "bigcode/starcoder2-15b",
+            DownloadSource.MODELSCOPE: "AI-ModelScope/starcoder2-15b",
         },
     }
 )
 
 
 register_model_group(
     models={
@@ -915,25 +989,61 @@
     },
     template="vicuna",
 )
 
 
 register_model_group(
     models={
+        "XuanYuan-6B": {
+            DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan-6B",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan-6B",
+        },
         "XuanYuan-70B": {
             DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan-70B",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan-70B",
+        },
+        "XuanYuan-2-70B": {
+            DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan2-70B",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan2-70B",
+        },
+        "XuanYuan-6B-Chat": {
+            DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan-6B-Chat",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan-6B-Chat",
         },
         "XuanYuan-70B-Chat": {
             DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan-70B-Chat",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan-70B-Chat",
+        },
+        "XuanYuan-2-70B-Chat": {
+            DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan2-70B-Chat",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan2-70B-Chat",
+        },
+        "XuanYuan-6B-int8-Chat": {
+            DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan-6B-Chat-8bit",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan-6B-Chat-8bit",
+        },
+        "XuanYuan-6B-int4-Chat": {
+            DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan-6B-Chat-4bit",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan-6B-Chat-4bit",
         },
         "XuanYuan-70B-int8-Chat": {
             DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan-70B-Chat-8bit",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan-70B-Chat-8bit",
         },
         "XuanYuan-70B-int4-Chat": {
             DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan-70B-Chat-4bit",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan-70B-Chat-4bit",
+        },
+        "XuanYuan-2-70B-int8-Chat": {
+            DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan2-70B-Chat-8bit",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan2-70B-Chat-8bit",
+        },
+        "XuanYuan-2-70B-int4-Chat": {
+            DownloadSource.DEFAULT: "Duxiaoman-DI/XuanYuan2-70B-Chat-4bit",
+            DownloadSource.MODELSCOPE: "Duxiaoman-DI/XuanYuan2-70B-Chat-4bit",
         },
     },
     template="xuanyuan",
 )
 
 
 register_model_group(
@@ -962,14 +1072,38 @@
             DownloadSource.DEFAULT: "xverse/XVERSE-13B-Chat",
             DownloadSource.MODELSCOPE: "xverse/XVERSE-13B-Chat",
         },
         "XVERSE-65B-Chat": {
             DownloadSource.DEFAULT: "xverse/XVERSE-65B-Chat",
             DownloadSource.MODELSCOPE: "xverse/XVERSE-65B-Chat",
         },
+        "XVERSE-MoE-A4.2B": {
+            DownloadSource.DEFAULT: "xverse/XVERSE-MoE-A4.2B",
+            DownloadSource.MODELSCOPE: "xverse/XVERSE-MoE-A4.2B",
+        },
+        "XVERSE-7B-int8-Chat": {
+            DownloadSource.DEFAULT: "xverse/XVERSE-7B-Chat-GPTQ-Int8",
+            DownloadSource.MODELSCOPE: "xverse/XVERSE-7B-Chat-GPTQ-Int8",
+        },
+        "XVERSE-7B-int4-Chat": {
+            DownloadSource.DEFAULT: "xverse/XVERSE-7B-Chat-GPTQ-Int4",
+            DownloadSource.MODELSCOPE: "xverse/XVERSE-7B-Chat-GPTQ-Int4",
+        },
+        "XVERSE-13B-int8-Chat": {
+            DownloadSource.DEFAULT: "xverse/XVERSE-13B-Chat-GPTQ-Int8",
+            DownloadSource.MODELSCOPE: "xverse/XVERSE-13B-Chat-GPTQ-Int8",
+        },
+        "XVERSE-13B-int4-Chat": {
+            DownloadSource.DEFAULT: "xverse/XVERSE-13B-Chat-GPTQ-Int4",
+            DownloadSource.MODELSCOPE: "xverse/XVERSE-13B-Chat-GPTQ-Int4",
+        },
+        "XVERSE-65B-int4-Chat": {
+            DownloadSource.DEFAULT: "xverse/XVERSE-65B-Chat-GPTQ-Int4",
+            DownloadSource.MODELSCOPE: "xverse/XVERSE-65B-Chat-GPTQ-Int4",
+        },
     },
     template="xverse",
 )
 
 
 register_model_group(
     models={
@@ -1054,10 +1188,13 @@
             DownloadSource.DEFAULT: "HuggingFaceH4/zephyr-7b-alpha",
             DownloadSource.MODELSCOPE: "AI-ModelScope/zephyr-7b-alpha",
         },
         "Zephyr-7B-Beta-Chat": {
             DownloadSource.DEFAULT: "HuggingFaceH4/zephyr-7b-beta",
             DownloadSource.MODELSCOPE: "modelscope/zephyr-7b-beta",
         },
+        "Zephyr-141B-ORPO-Chat": {
+            DownloadSource.DEFAULT: "HuggingFaceH4/zephyr-orpo-141b-A35b-v0.1",
+        },
     },
     template="zephyr",
 )
```

### Comparing `llmtuner-0.6.3/src/llmtuner/extras/logging.py` & `llmtuner-0.7.0/src/llmtuner/extras/logging.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/extras/misc.py` & `llmtuner-0.7.0/src/llmtuner/extras/misc.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/extras/packages.py` & `llmtuner-0.7.0/src/llmtuner/extras/packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import importlib.metadata
 import importlib.util
+from typing import TYPE_CHECKING
+
+from packaging import version
+
+
+if TYPE_CHECKING:
+    from packaging.version import Version
 
 
 def _is_package_available(name: str) -> bool:
     return importlib.util.find_spec(name) is not None
 
 
-def _get_package_version(name: str) -> str:
+def _get_package_version(name: str) -> "Version":
     try:
-        return importlib.metadata.version(name)
+        return version.parse(importlib.metadata.version(name))
     except Exception:
-        return "0.0.0"
+        return version.parse("0.0.0")
 
 
 def is_fastapi_availble():
     return _is_package_available("fastapi")
 
 
 def is_flash_attn2_available():
-    return _is_package_available("flash_attn") and _get_package_version("flash_attn").startswith("2")
+    return _is_package_available("flash_attn") and _get_package_version("flash_attn") > version.parse("2.0.0")
 
 
 def is_galore_available():
     return _is_package_available("galore_torch")
 
 
 def is_gradio_available():
@@ -37,22 +44,30 @@
     return _is_package_available("matplotlib")
 
 
 def is_nltk_available():
     return _is_package_available("nltk")
 
 
+def is_pillow_available():
+    return _is_package_available("PIL")
+
+
 def is_requests_available():
     return _is_package_available("requests")
 
 
 def is_rouge_available():
     return _is_package_available("rouge_chinese")
 
 
+def is_sdpa_available():
+    return _get_package_version("torch") > version.parse("2.1.1")
+
+
 def is_starlette_available():
     return _is_package_available("sse_starlette")
 
 
 def is_uvicorn_available():
     return _is_package_available("uvicorn")
```

### Comparing `llmtuner-0.6.3/src/llmtuner/extras/patches/llama_patch.py` & `llmtuner-0.7.0/src/llmtuner/model/utils/longlora.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 import math
-from typing import Optional, Tuple
+from typing import TYPE_CHECKING, Optional, Tuple
 
 import torch
 import torch.nn as nn
 from transformers.models.llama.modeling_llama import (
     Cache,
     LlamaAttention,
     LlamaFlashAttention2,
+    LlamaSdpaAttention,
     apply_rotary_pos_emb,
     repeat_kv,
 )
 from transformers.utils import logging
 from transformers.utils.versions import require_version
 
+from ...extras.constants import SUPPORTED_CLASS_FOR_S2ATTN
+
+
+if TYPE_CHECKING:
+    from transformers import PretrainedConfig
+
+    from ...hparams import ModelArguments
+
 
 logger = logging.get_logger(__name__)
 
 
 # Modified from:
-# https://github.com/huggingface/transformers/blob/v4.39.1/src/transformers/models/llama/modeling_llama.py
-def llama_torch_attn_forward(
+# https://github.com/huggingface/transformers/blob/v4.40.0/src/transformers/models/llama/modeling_llama.py
+def llama_attention_forward(
     self: "LlamaAttention",
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
     past_key_value: Optional["Cache"] = None,
     output_attentions: bool = False,
     cache_position: Optional[torch.LongTensor] = None,
@@ -35,18 +44,19 @@
     key_states = self.k_proj(hidden_states)
     value_states = self.v_proj(hidden_states)
 
     query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
     key_states = key_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
     value_states = value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
 
-    past_key_value = getattr(self, "past_key_value", past_key_value)
     cos, sin = self.rotary_emb(value_states, position_ids)
     query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin)
 
+    past_key_value = getattr(self, "past_key_value", past_key_value)
+
     if past_key_value is not None:
         cache_kwargs = {"sin": sin, "cos": cos, "cache_position": cache_position}
         key_states, value_states = past_key_value.update(key_states, value_states, self.layer_idx, cache_kwargs)
 
     key_states = repeat_kv(key_states, self.num_key_value_groups)
     value_states = repeat_kv(value_states, self.num_key_value_groups)
 
@@ -65,16 +75,17 @@
 
         query_states, key_states, value_states = shift(query_states), shift(key_states), shift(value_states)
         if attention_mask is not None:
             attention_mask = attention_mask[:, :, :groupsz, :groupsz].repeat(num_groups, 1, 1, 1)
 
     attn_weights = torch.matmul(query_states, key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
 
-    if attention_mask is not None:
-        attn_weights = attn_weights + attention_mask
+    if attention_mask is not None:  # no matter the length, we just slice it
+        causal_mask = attention_mask[:, :, :, : key_states.shape[-2]]
+        attn_weights = attn_weights + causal_mask
 
     # upcast attention to fp32
     attn_weights = nn.functional.softmax(attn_weights, dim=-1, dtype=torch.float32).to(query_states.dtype)
     attn_weights = nn.functional.dropout(attn_weights, p=self.attention_dropout, training=self.training)
     attn_output = torch.matmul(attn_weights, value_states)  # (bsz, :, seq_len, :) or (bsz*n_group, :, groupsz, :)
     attn_output = attn_output.transpose(1, 2).contiguous()
 
@@ -93,16 +104,16 @@
     if not output_attentions:
         attn_weights = None
 
     return attn_output, attn_weights, past_key_value
 
 
 # Modified from:
-# https://github.com/huggingface/transformers/blob/v4.39.1/src/transformers/models/llama/modeling_llama.py
-def llama_flash_attn_forward(
+# https://github.com/huggingface/transformers/blob/v4.40.0/src/transformers/models/llama/modeling_llama.py
+def llama_flash_attention_2_forward(
     self: "LlamaFlashAttention2",
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
     past_key_value: Optional["Cache"] = None,
     output_attentions: bool = False,
     cache_position: Optional[torch.LongTensor] = None,
@@ -113,15 +124,14 @@
 
     bsz, q_len, _ = hidden_states.size()
 
     query_states = self.q_proj(hidden_states)
     key_states = self.k_proj(hidden_states)
     value_states = self.v_proj(hidden_states)
 
-    # FlashAttention requires the input to have the shape (bsz, seq_len, n_heads, head_dim)
     query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
     key_states = key_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
     value_states = value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
 
     cos, sin = self.rotary_emb(value_states, position_ids)
     query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin)
 
@@ -130,17 +140,18 @@
     if past_key_value is not None:
         cache_kwargs = {"sin": sin, "cos": cos, "cache_position": cache_position}
         key_states, value_states = past_key_value.update(key_states, value_states, self.layer_idx, cache_kwargs)
 
     key_states = repeat_kv(key_states, self.num_key_value_groups)
     value_states = repeat_kv(value_states, self.num_key_value_groups)
 
-    query_states = query_states.transpose(1, 2)  # (bsz, seq_len, n_heads, head_dim)
-    key_states = key_states.transpose(1, 2)  # (bsz, seq_len, n_heads, head_dim)
-    value_states = value_states.transpose(1, 2)  # (bsz, seq_len, n_heads, head_dim)
+    # FlashAttention requires the input to have the shape (bsz, seq_len, n_heads, head_dim)
+    query_states = query_states.transpose(1, 2)
+    key_states = key_states.transpose(1, 2)
+    value_states = value_states.transpose(1, 2)
 
     dropout_rate = self.attention_dropout if self.training else 0.0
 
     input_dtype = query_states.dtype
     if input_dtype == torch.float32:
         if torch.is_autocast_enabled():
             target_dtype = torch.get_autocast_gpu_dtype()
@@ -188,11 +199,119 @@
 
     if not output_attentions:
         attn_weights = None
 
     return attn_output, attn_weights, past_key_value
 
 
-def apply_llama_patch() -> None:
-    require_version("transformers==4.39.3", "To fix: pip install transformers==4.39.3")
-    LlamaAttention.forward = llama_torch_attn_forward
-    LlamaFlashAttention2.forward = llama_flash_attn_forward
+# Modified from:
+# https://github.com/huggingface/transformers/blob/v4.40.0/src/transformers/models/llama/modeling_llama.py
+def llama_sdpa_attention_forward(
+    self: "LlamaSdpaAttention",
+    hidden_states: torch.Tensor,
+    attention_mask: Optional[torch.Tensor] = None,
+    position_ids: Optional[torch.LongTensor] = None,
+    past_key_value: Optional["Cache"] = None,
+    output_attentions: bool = False,
+    cache_position: Optional[torch.LongTensor] = None,
+    **kwargs,
+) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
+    if output_attentions:
+        logger.warning_once("SDPA does not support `output_attentions=True`. Falling back to the vanilla attention")
+        return llama_attention_forward(
+            self,
+            hidden_states=hidden_states,
+            attention_mask=attention_mask,
+            position_ids=position_ids,
+            past_key_value=past_key_value,
+            output_attentions=output_attentions,
+            cache_position=cache_position,
+            **kwargs,
+        )
+
+    bsz, q_len, _ = hidden_states.size()
+
+    query_states = self.q_proj(hidden_states)
+    key_states = self.k_proj(hidden_states)
+    value_states = self.v_proj(hidden_states)
+
+    query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+    key_states = key_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
+    value_states = value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
+
+    cos, sin = self.rotary_emb(value_states, position_ids)
+    query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin)
+
+    if past_key_value is not None:
+        cache_kwargs = {"sin": sin, "cos": cos, "cache_position": cache_position}
+        key_states, value_states = past_key_value.update(key_states, value_states, self.layer_idx, cache_kwargs)
+
+    key_states = repeat_kv(key_states, self.num_key_value_groups)
+    value_states = repeat_kv(value_states, self.num_key_value_groups)
+
+    if getattr(self.config, "group_size_ratio", None) and self.training:  # shift
+        groupsz = int(q_len * getattr(self.config, "group_size_ratio"))
+        assert q_len % groupsz == 0, "q_len {} should be divisible by group size {}.".format(q_len, groupsz)
+        num_groups = q_len // groupsz
+
+        def shift(state: torch.Tensor) -> torch.Tensor:
+            state = state.transpose(1, 2)  # output: (bsz, seq_len, n_heads, head_dim)
+            state = torch.cat(
+                (state[:, :, : self.num_heads // 2], state[:, :, self.num_heads // 2 :].roll(-groupsz // 2, dims=1)),
+                dim=2,
+            )
+            return state.reshape(bsz * num_groups, groupsz, self.num_heads, self.head_dim).transpose(1, 2)
+
+        query_states, key_states, value_states = shift(query_states), shift(key_states), shift(value_states)
+        if attention_mask is not None:
+            attention_mask = attention_mask[:, :, :groupsz, :groupsz].repeat(num_groups, 1, 1, 1)
+
+    causal_mask = attention_mask
+    if attention_mask is not None:
+        causal_mask = causal_mask[:, :, :, :groupsz]
+
+    query_states = query_states.contiguous()
+    key_states = key_states.contiguous()
+    value_states = value_states.contiguous()
+
+    attn_output = torch.nn.functional.scaled_dot_product_attention(
+        query_states,
+        key_states,
+        value_states,
+        attn_mask=causal_mask,
+        dropout_p=self.attention_dropout if self.training else 0.0,
+        is_causal=causal_mask is None and q_len > 1,
+    )
+    attn_output = attn_output.transpose(1, 2).contiguous()
+
+    if getattr(self.config, "group_size_ratio", None) and self.training:  # shift back
+        attn_output.reshape(bsz, q_len, self.num_heads, self.head_dim)
+        attn_output = torch.cat(
+            (
+                attn_output[:, :, : self.num_heads // 2],
+                attn_output[:, :, self.num_heads // 2 :].roll(groupsz // 2, dims=1),
+            )
+        )
+
+    attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
+    attn_output = self.o_proj(attn_output)
+
+    return attn_output, None, past_key_value
+
+
+def _apply_llama_patch() -> None:
+    require_version("transformers==4.40.0", "To fix: pip install transformers==4.40.0")
+    LlamaAttention.forward = llama_attention_forward
+    LlamaFlashAttention2.forward = llama_flash_attention_2_forward
+    LlamaSdpaAttention.forward = llama_sdpa_attention_forward
+
+
+def configure_longlora(config: "PretrainedConfig", model_args: "ModelArguments", is_trainable: bool) -> None:
+    if not is_trainable or not model_args.shift_attn:
+        return
+
+    if getattr(config, "model_type", None) in SUPPORTED_CLASS_FOR_S2ATTN:
+        setattr(config, "group_size_ratio", 0.25)
+        _apply_llama_patch()
+        logger.info("Using shift short attention with group_size_ratio=1/4.")
+    else:
+        logger.warning("Current model does not support shift short attention.")
```

### Comparing `llmtuner-0.6.3/src/llmtuner/extras/ploting.py` & `llmtuner-0.7.0/src/llmtuner/extras/ploting.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/hparams/data_args.py` & `llmtuner-0.7.0/src/llmtuner/hparams/data_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,19 +22,19 @@
     )
     split: str = field(
         default="train",
         metadata={"help": "Which dataset split to use for training and evaluation."},
     )
     cutoff_len: int = field(
         default=1024,
-        metadata={"help": "The cutoff length of the model inputs after tokenization."},
+        metadata={"help": "The cutoff length of the tokenized inputs in the dataset."},
     )
     reserved_label_len: int = field(
         default=1,
-        metadata={"help": "The minimum cutoff length reserved for label after tokenization."},
+        metadata={"help": "The minimum cutoff length reserved for the tokenized labels in the dataset."},
     )
     train_on_prompt: bool = field(
         default=False,
         metadata={"help": "Whether to disable the mask on the prompt or not."},
     )
     streaming: bool = field(
         default=False,
```

### Comparing `llmtuner-0.6.3/src/llmtuner/hparams/evaluation_args.py` & `llmtuner-0.7.0/src/llmtuner/hparams/evaluation_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/hparams/finetuning_args.py` & `llmtuner-0.7.0/src/llmtuner/hparams/finetuning_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/hparams/generating_args.py` & `llmtuner-0.7.0/src/llmtuner/hparams/generating_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         metadata={"help": "The number of highest probability vocabulary tokens to keep for top-k filtering."},
     )
     num_beams: int = field(
         default=1,
         metadata={"help": "Number of beams for beam search. 1 means no beam search."},
     )
     max_length: int = field(
-        default=512,
+        default=1024,
         metadata={"help": "The maximum length the generated tokens can have. It can be overridden by max_new_tokens."},
     )
     max_new_tokens: int = field(
-        default=512,
+        default=1024,
         metadata={"help": "The maximum numbers of tokens to generate, ignoring the number of tokens in the prompt."},
     )
     repetition_penalty: float = field(
         default=1.0,
         metadata={"help": "The parameter for repetition penalty. 1.0 means no penalty."},
     )
     length_penalty: float = field(
```

### Comparing `llmtuner-0.6.3/src/llmtuner/hparams/model_args.py` & `llmtuner-0.7.0/src/llmtuner/hparams/model_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,29 @@
         metadata={"help": "Path to the adapter weight or identifier from huggingface.co/models."},
     )
     cache_dir: Optional[str] = field(
         default=None,
         metadata={"help": "Where to store the pre-trained models downloaded from huggingface.co or modelscope.cn."},
     )
     use_fast_tokenizer: bool = field(
-        default=False,
+        default=True,
         metadata={"help": "Whether or not to use one of the fast tokenizer (backed by the tokenizers library)."},
     )
     resize_vocab: bool = field(
         default=False,
         metadata={"help": "Whether or not to resize the tokenizer vocab and the embedding layers."},
     )
     split_special_tokens: bool = field(
         default=False,
         metadata={"help": "Whether or not the special tokens should be split during the tokenization process."},
     )
+    new_special_tokens: Optional[str] = field(
+        default=None,
+        metadata={"help": "Special tokens to be added into the tokenizer."},
+    )
     model_revision: str = field(
         default="main",
         metadata={"help": "The specific model version to use (can be a branch name, tag name or commit id)."},
     )
     low_cpu_mem_usage: bool = field(
         default=True,
         metadata={"help": "Whether or not to use memory-efficient model loading."},
@@ -57,30 +61,34 @@
         default=None,
         metadata={"help": "Device map used to infer the 4-bit quantized model, needs bitsandbytes>=0.43.0."},
     )
     rope_scaling: Optional[Literal["linear", "dynamic"]] = field(
         default=None,
         metadata={"help": "Which scaling strategy should be adopted for the RoPE embeddings."},
     )
-    flash_attn: bool = field(
-        default=False,
-        metadata={"help": "Enable FlashAttention for faster training."},
+    flash_attn: Literal["off", "sdpa", "fa2", "auto"] = field(
+        default="auto",
+        metadata={"help": "Enable FlashAttention for faster training and inference."},
     )
     shift_attn: bool = field(
         default=False,
         metadata={"help": "Enable shift short attention (S^2-Attn) proposed by LongLoRA."},
     )
     mixture_of_depths: Optional[Literal["convert", "load"]] = field(
         default=None,
         metadata={"help": "Convert the model to mixture-of-depths (MoD) or load the MoD model."},
     )
     use_unsloth: bool = field(
         default=False,
         metadata={"help": "Whether or not to use unsloth's optimization for the LoRA training."},
     )
+    visual_inputs: bool = field(
+        default=False,
+        metadata={"help": "Whethor or not to use multimodal LLM that accepts visual inputs."},
+    )
     moe_aux_loss_coef: Optional[float] = field(
         default=None,
         metadata={"help": "Coefficient of the auxiliary router loss in mixture-of-experts model."},
     )
     disable_gradient_checkpointing: bool = field(
         default=False,
         metadata={"help": "Whether or not to disable gradient checkpointing."},
@@ -131,15 +139,15 @@
     )
     export_size: int = field(
         default=1,
         metadata={"help": "The file shard size (in GB) of the exported model."},
     )
     export_device: str = field(
         default="cpu",
-        metadata={"help": "The device used in model export."},
+        metadata={"help": "The device used in model export, use cuda to avoid addmm errors."},
     )
     export_quantization_bit: Optional[int] = field(
         default=None,
         metadata={"help": "The number of bits to quantize the exported model."},
     )
     export_quantization_dataset: Optional[str] = field(
         default=None,
@@ -170,17 +178,23 @@
         self.compute_dtype = None
         self.device_map = None
         self.model_max_length = None
 
         if self.split_special_tokens and self.use_fast_tokenizer:
             raise ValueError("`split_special_tokens` is only supported for slow tokenizers.")
 
+        if self.visual_inputs and self.use_unsloth:
+            raise ValueError("Unsloth does not support MLLM yet. Stay tuned.")
+
         if self.adapter_name_or_path is not None:  # support merging multiple lora weights
             self.adapter_name_or_path = [path.strip() for path in self.adapter_name_or_path.split(",")]
 
+        if self.new_special_tokens is not None:  # support multiple special tokens
+            self.new_special_tokens = [token.strip() for token in self.new_special_tokens.split(",")]
+
         assert self.quantization_bit in [None, 8, 4], "We only accept 4-bit or 8-bit quantization."
         assert self.export_quantization_bit in [None, 8, 4, 3, 2], "We only accept 2/3/4/8-bit quantization."
 
         if self.export_quantization_bit is not None and self.export_quantization_dataset is None:
             raise ValueError("Quantization dataset is necessary for exporting.")
 
     def to_dict(self) -> Dict[str, Any]:
```

### Comparing `llmtuner-0.6.3/src/llmtuner/hparams/parser.py` & `llmtuner-0.7.0/src/llmtuner/hparams/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,17 @@
     if model_args.adapter_name_or_path is not None and finetuning_args.finetuning_type != "lora":
         raise ValueError("Adapter is only valid for the LoRA method.")
 
     if model_args.quantization_bit is not None:
         if finetuning_args.finetuning_type != "lora":
             raise ValueError("Quantization is only compatible with the LoRA method.")
 
+        if model_args.resize_vocab:
+            raise ValueError("Cannot resize embedding layers of a quantized model.")
+
         if model_args.adapter_name_or_path is not None and finetuning_args.create_new_adapter:
             raise ValueError("Cannot create new adapter upon a quantized model.")
 
         if model_args.adapter_name_or_path is not None and len(model_args.adapter_name_or_path) != 1:
             raise ValueError("Quantized model only accepts a single adapter. Merge them first.")
 
 
@@ -82,22 +85,25 @@
     if model_args.use_unsloth:
         require_version("unsloth", "Please install unsloth: https://github.com/unslothai/unsloth")
 
     if model_args.mixture_of_depths is not None:
         require_version("mixture-of-depth>=1.1.6", "To fix: pip install mixture-of-depth>=1.1.6")
 
     if model_args.infer_backend == "vllm":
-        require_version("vllm>=0.3.3", "To fix: pip install vllm>=0.3.3")
+        require_version("vllm>=0.4.0", "To fix: pip install vllm>=0.4.0")
 
     if finetuning_args.use_galore:
         require_version("galore_torch", "To fix: pip install galore_torch")
 
     if finetuning_args.use_badam:
         require_version("badam", "To fix: pip install badam")
 
+    if finetuning_args.plot_loss:
+        require_version("matplotlib", "To fix: pip install matplotlib")
+
     if training_args is not None and training_args.predict_with_generate:
         require_version("jieba", "To fix: pip install jieba")
         require_version("nltk", "To fix: pip install nltk")
         require_version("rouge_chinese", "To fix: pip install rouge-chinese")
 
 
 def _parse_train_args(args: Optional[Dict[str, Any]] = None) -> _TRAIN_CLS:
@@ -186,24 +192,28 @@
 
     if (finetuning_args.use_galore or finetuning_args.use_badam) and training_args.deepspeed is not None:
         raise ValueError("GaLore and BAdam are incompatible with DeepSpeed yet.")
 
     if model_args.infer_backend == "vllm":
         raise ValueError("vLLM backend is only available for API, CLI and Web.")
 
+    if model_args.visual_inputs and data_args.packing:
+        raise ValueError("Cannot use packing in MLLM fine-tuning.")
+
     _verify_model_args(model_args, finetuning_args)
     _check_extra_dependencies(model_args, finetuning_args, training_args)
 
     if (
         training_args.do_train
         and finetuning_args.finetuning_type == "lora"
+        and model_args.quantization_bit is None
         and model_args.resize_vocab
         and finetuning_args.additional_target is None
     ):
-        logger.warning("Add token embeddings to `additional_target` to make the added tokens trainable.")
+        logger.warning("Remember to add embedding layers to `additional_target` to make the added tokens trainable.")
 
     if training_args.do_train and model_args.quantization_bit is not None and (not model_args.upcast_layernorm):
         logger.warning("We recommend enable `upcast_layernorm` in quantized training.")
 
     if training_args.do_train and (not training_args.fp16) and (not training_args.bf16):
         logger.warning("We recommend enable mixed precision training.")
 
@@ -297,23 +307,26 @@
     if data_args.template is None:
         raise ValueError("Please specify which `template` to use.")
 
     if model_args.infer_backend == "vllm":
         if finetuning_args.stage != "sft":
             raise ValueError("vLLM engine only supports auto-regressive models.")
 
-        if model_args.adapter_name_or_path is not None:
-            raise ValueError("vLLM engine does not support LoRA adapters. Merge them first.")
-
         if model_args.quantization_bit is not None:
-            raise ValueError("vLLM engine does not support quantization.")
+            raise ValueError("vLLM engine does not support bnb quantization (GPTQ and AWQ are supported).")
 
         if model_args.rope_scaling is not None:
             raise ValueError("vLLM engine does not support RoPE scaling.")
 
+        if model_args.adapter_name_or_path is not None and len(model_args.adapter_name_or_path) != 1:
+            raise ValueError("vLLM only accepts a single adapter. Merge them first.")
+
+    if finetuning_args.stage == "rm" and model_args.visual_inputs:
+        raise ValueError("Reward server does not support MLLM yet. Stay tuned.")
+
     _verify_model_args(model_args, finetuning_args)
     _check_extra_dependencies(model_args, finetuning_args)
 
     if model_args.export_dir is not None:
         model_args.device_map = {"": torch.device(model_args.export_device)}
     else:
         model_args.device_map = "auto"
```

### Comparing `llmtuner-0.6.3/src/llmtuner/model/adapter.py` & `llmtuner-0.7.0/src/llmtuner/model/adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from typing import TYPE_CHECKING
 
 import torch
 from peft import LoraConfig, LoraModel, PeftModel, TaskType, get_peft_model
 from transformers.integrations import is_deepspeed_zero3_enabled
 
 from ..extras.logging import get_logger
-from .utils import QuantizationMethod, find_all_linear_modules, find_expanded_modules
+from .utils.misc import find_all_linear_modules, find_expanded_modules
+from .utils.quantization import QuantizationMethod
+from .utils.unsloth import get_unsloth_peft_model, load_unsloth_peft_model
 
 
 if TYPE_CHECKING:
-    from transformers.modeling_utils import PreTrainedModel
+    from transformers import PretrainedConfig, PreTrainedModel
 
     from ..hparams import FinetuningArguments, ModelArguments
 
 
 logger = get_logger(__name__)
 
 
 def init_adapter(
-    model: "PreTrainedModel", model_args: "ModelArguments", finetuning_args: "FinetuningArguments", is_trainable: bool
+    config: "PretrainedConfig",
+    model: "PreTrainedModel",
+    model_args: "ModelArguments",
+    finetuning_args: "FinetuningArguments",
+    is_trainable: bool,
 ) -> "PreTrainedModel":
     r"""
     Initializes the adapters.
 
     Support full-parameter, freeze and LoRA training.
 
     Note that the trainable parameters must be cast to float32.
@@ -101,14 +107,18 @@
                 assert len(model_args.adapter_name_or_path) == 1, "Quantized model only accepts a single adapter."
                 is_mergeable = False
 
             if is_deepspeed_zero3_enabled():
                 assert len(model_args.adapter_name_or_path) == 1, "Cannot use multiple adapters in DeepSpeed ZeRO-3."
                 is_mergeable = False
 
+            if model_args.use_unsloth:
+                assert len(model_args.adapter_name_or_path) == 1, "Unsloth model only accepts a single adapter."
+                is_mergeable = False
+
             if (is_trainable and not finetuning_args.create_new_adapter) or (not is_mergeable):
                 adapter_to_merge = model_args.adapter_name_or_path[:-1]
                 adapter_to_resume = model_args.adapter_name_or_path[-1]
             else:
                 adapter_to_merge = model_args.adapter_name_or_path
 
             for adapter in adapter_to_merge:
@@ -117,17 +127,23 @@
                 )
                 model = model.merge_and_unload()
 
             if len(adapter_to_merge) > 0:
                 logger.info("Merged {} adapter(s).".format(len(adapter_to_merge)))
 
             if adapter_to_resume is not None:  # resume lora training
-                model = PeftModel.from_pretrained(
-                    model, adapter_to_resume, is_trainable=is_trainable, offload_folder=model_args.offload_folder
-                )
+                if model_args.use_unsloth:
+                    model = load_unsloth_peft_model(config, model_args, is_trainable=is_trainable)
+                else:
+                    model = PeftModel.from_pretrained(
+                        model,
+                        adapter_to_resume,
+                        is_trainable=is_trainable,
+                        offload_folder=model_args.offload_folder,
+                    )
 
         if is_trainable and adapter_to_resume is None:  # create new lora weights while training
             if len(finetuning_args.lora_target) == 1 and finetuning_args.lora_target[0] == "all":
                 target_modules = find_all_linear_modules(model)
             else:
                 target_modules = finetuning_args.lora_target
 
@@ -137,32 +153,36 @@
             if (
                 finetuning_args.use_dora
                 and getattr(model, "quantization_method", None) is not None
                 and getattr(model, "quantization_method", None) != QuantizationMethod.BITS_AND_BYTES
             ):
                 raise ValueError("DoRA is not compatible with PTQ-quantized models.")
 
+            if model_args.resize_vocab and finetuning_args.additional_target is None:
+                input_embeddings = model.get_input_embeddings()
+                output_embeddings = model.get_output_embeddings()
+                module_names = set()
+                for name, module in model.named_modules():
+                    if module in [input_embeddings, output_embeddings]:
+                        module_names.add(name.split(".")[-1])
+
+                finetuning_args.additional_target = module_names
+                logger.warning("Vocab has been resized, add {} to trainable params.".format(",".join(module_names)))
+
             peft_kwargs = {
                 "r": finetuning_args.lora_rank,
                 "target_modules": target_modules,
                 "lora_alpha": finetuning_args.lora_alpha,
                 "lora_dropout": finetuning_args.lora_dropout,
                 "use_rslora": finetuning_args.use_rslora,
                 "modules_to_save": finetuning_args.additional_target,
             }
 
             if model_args.use_unsloth:
-                from unsloth import FastLanguageModel  # type: ignore
-
-                unsloth_peft_kwargs = {
-                    "model": model,
-                    "max_seq_length": model_args.model_max_length,
-                    "use_gradient_checkpointing": "unsloth",
-                }
-                model = FastLanguageModel.get_peft_model(**peft_kwargs, **unsloth_peft_kwargs)
+                model = get_unsloth_peft_model(model, model_args, peft_kwargs)
             else:
                 lora_config = LoraConfig(
                     task_type=TaskType.CAUSAL_LM,
                     inference_mode=False,
                     use_dora=finetuning_args.use_dora,
                     **peft_kwargs,
                 )
```

### Comparing `llmtuner-0.6.3/src/llmtuner/model/loader.py` & `llmtuner-0.7.0/src/llmtuner/model/loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,54 @@
-from typing import TYPE_CHECKING, Any, Dict
+from typing import TYPE_CHECKING, Any, Dict, Optional, TypedDict
 
-from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
+from transformers import AutoConfig, AutoModelForCausalLM, AutoModelForVision2Seq, AutoProcessor, AutoTokenizer
 from trl import AutoModelForCausalLMWithValueHead
 
-from ..extras.constants import MOD_SUPPORTED_MODELS
 from ..extras.logging import get_logger
-from ..extras.misc import count_parameters, get_current_device, try_download_model_from_ms
+from ..extras.misc import count_parameters, try_download_model_from_ms
 from .adapter import init_adapter
 from .patcher import patch_config, patch_model, patch_tokenizer, patch_valuehead_model
-from .utils import load_valuehead_params, register_autoclass
+from .utils.misc import register_autoclass
+from .utils.mod import convert_pretrained_model_to_mod, load_mod_pretrained_model
+from .utils.unsloth import load_unsloth_pretrained_model
+from .utils.valuehead import load_valuehead_params
 
 
 if TYPE_CHECKING:
-    from transformers import PreTrainedModel, PreTrainedTokenizer
+    from transformers import PretrainedConfig, PreTrainedModel, PreTrainedTokenizer, ProcessorMixin
 
     from ..hparams import FinetuningArguments, ModelArguments
 
 
 logger = get_logger(__name__)
 
 
+class TokenizerModule(TypedDict):
+    tokenizer: "PreTrainedTokenizer"
+    processor: Optional["ProcessorMixin"]
+
+
 def _get_init_kwargs(model_args: "ModelArguments") -> Dict[str, Any]:
+    r"""
+    Gets arguments to load config/tokenizer/model.
+
+    Note: including inplace operation of model_args.
+    """
     model_args.model_name_or_path = try_download_model_from_ms(model_args)
     return {
         "trust_remote_code": True,
         "cache_dir": model_args.cache_dir,
         "revision": model_args.model_revision,
         "token": model_args.hf_hub_token,
     }
 
 
-def load_tokenizer(model_args: "ModelArguments") -> "PreTrainedTokenizer":
+def load_tokenizer(model_args: "ModelArguments") -> "TokenizerModule":
     r"""
-    Loads pretrained tokenizer. Must before load_model.
+    Loads pretrained tokenizer.
 
     Note: including inplace operation of model_args.
     """
     init_kwargs = _get_init_kwargs(model_args)
     try:
         tokenizer = AutoTokenizer.from_pretrained(
             model_args.model_name_or_path,
@@ -49,81 +61,84 @@
         tokenizer = AutoTokenizer.from_pretrained(
             model_args.model_name_or_path,
             use_fast=True,
             padding_side="right",
             **init_kwargs,
         )
 
+    if model_args.new_special_tokens is not None:
+        num_added_tokens = tokenizer.add_special_tokens(
+            dict(additional_special_tokens=model_args.new_special_tokens),
+            replace_additional_special_tokens=False,
+        )
+        logger.info("Add {} to special tokens.".format(",".join(model_args.new_special_tokens)))
+        if num_added_tokens > 0 and not model_args.resize_vocab:
+            model_args.resize_vocab = True
+            logger.warning("New tokens have been added, changed `resize_vocab` to True.")
+
     patch_tokenizer(tokenizer)
-    return tokenizer
+
+    if model_args.visual_inputs:
+        processor = AutoProcessor.from_pretrained(model_args.model_name_or_path, **init_kwargs)
+        setattr(processor, "tokenizer", tokenizer)
+    else:
+        processor = None
+
+    return {"tokenizer": tokenizer, "processor": processor}
+
+
+def load_config(model_args: "ModelArguments") -> "PretrainedConfig":
+    r"""
+    Loads model config.
+    """
+    init_kwargs = _get_init_kwargs(model_args)
+    return AutoConfig.from_pretrained(model_args.model_name_or_path, **init_kwargs)
 
 
 def load_model(
     tokenizer: "PreTrainedTokenizer",
     model_args: "ModelArguments",
     finetuning_args: "FinetuningArguments",
     is_trainable: bool = False,
     add_valuehead: bool = False,
 ) -> "PreTrainedModel":
     r"""
-    Loads pretrained model. Must after load_tokenizer.
+    Loads pretrained model.
     """
     init_kwargs = _get_init_kwargs(model_args)
-    config = AutoConfig.from_pretrained(model_args.model_name_or_path, **init_kwargs)
-    patch_config(config, tokenizer, model_args, init_kwargs, is_trainable)
+    config = load_config(model_args)
+    patch_config(config, tokenizer, model_args, init_kwargs, is_trainable, add_valuehead)
 
     model = None
-    if is_trainable and model_args.use_unsloth:
-        from unsloth import FastLanguageModel  # type: ignore
-
-        unsloth_kwargs = {
-            "model_name": model_args.model_name_or_path,
-            "max_seq_length": model_args.model_max_length,
-            "dtype": model_args.compute_dtype,
-            "load_in_4bit": model_args.quantization_bit == 4,
-            "token": model_args.hf_hub_token,
-            "device_map": {"": get_current_device()},
-            "rope_scaling": getattr(config, "rope_scaling", None),
-            "fix_tokenizer": False,
-            "trust_remote_code": True,
-        }
-        try:
-            model, _ = FastLanguageModel.from_pretrained(**unsloth_kwargs)
-        except NotImplementedError:
-            logger.warning("Unsloth does not support model type {}.".format(getattr(config, "model_type", None)))
-            model_args.use_unsloth = False
-
-        if model_args.adapter_name_or_path:
-            model_args.adapter_name_or_path = None
-            logger.warning("Unsloth does not support loading adapters.")
+    lazy_load = False
+    if model_args.use_unsloth:
+        if model_args.adapter_name_or_path is not None:
+            lazy_load = True
+        elif is_trainable:
+            model = load_unsloth_pretrained_model(config, model_args)
 
-    if model is None:
+    if model is None and not lazy_load:
         init_kwargs["config"] = config
         init_kwargs["pretrained_model_name_or_path"] = model_args.model_name_or_path
 
         if model_args.mixture_of_depths == "load":
-            from MoD import AutoMoDModelForCausalLM
-
-            model = AutoMoDModelForCausalLM.from_pretrained(**init_kwargs)
+            model = load_mod_pretrained_model(**init_kwargs)
+        elif model_args.visual_inputs:
+            model = AutoModelForVision2Seq.from_pretrained(**init_kwargs)
         else:
             model = AutoModelForCausalLM.from_pretrained(**init_kwargs)
 
         if model_args.mixture_of_depths == "convert":
-            from MoD import apply_mod_to_hf
-
-            if getattr(config, "model_type", None) not in MOD_SUPPORTED_MODELS:
-                raise ValueError("Current model is not supported by mixture-of-depth.")
-
-            model = apply_mod_to_hf(model)
-            model = model.to(model_args.compute_dtype)
+            model = convert_pretrained_model_to_mod(model, config, model_args)
 
-    patch_model(model, tokenizer, model_args, is_trainable)
-    register_autoclass(config, model, tokenizer)
+    if not lazy_load:
+        patch_model(model, tokenizer, model_args, is_trainable, add_valuehead)
+        register_autoclass(config, model, tokenizer)
 
-    model = init_adapter(model, model_args, finetuning_args, is_trainable)
+    model = init_adapter(config, model, model_args, finetuning_args, is_trainable)
 
     if add_valuehead:
         model = AutoModelForCausalLMWithValueHead.from_pretrained(model)
         patch_valuehead_model(model)
 
         if model_args.adapter_name_or_path is not None:
             vhead_path = model_args.adapter_name_or_path[-1]
```

### Comparing `llmtuner-0.6.3/src/llmtuner/train/dpo/trainer.py` & `llmtuner-0.7.0/src/llmtuner/train/dpo/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/train/dpo/workflow.py` & `llmtuner-0.7.0/src/llmtuner/train/dpo/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 def run_dpo(
     model_args: "ModelArguments",
     data_args: "DataArguments",
     training_args: "Seq2SeqTrainingArguments",
     finetuning_args: "FinetuningArguments",
     callbacks: Optional[List["TrainerCallback"]] = None,
 ):
-    tokenizer = load_tokenizer(model_args)
-    dataset = get_dataset(tokenizer, model_args, data_args, training_args, stage="rm")
+    tokenizer_module = load_tokenizer(model_args)
+    tokenizer = tokenizer_module["tokenizer"]
+    dataset = get_dataset(model_args, data_args, training_args, stage="rm", **tokenizer_module)
     model = load_model(tokenizer, model_args, finetuning_args, training_args.do_train)
 
     data_collator = PairwiseDataCollatorWithPadding(
         tokenizer=tokenizer,
         pad_to_multiple_of=8,
         label_pad_token_id=IGNORE_INDEX if data_args.ignore_pad_token_for_loss else tokenizer.pad_token_id,
     )
```

### Comparing `llmtuner-0.6.3/src/llmtuner/train/orpo/trainer.py` & `llmtuner-0.7.0/src/llmtuner/train/orpo/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/train/orpo/workflow.py` & `llmtuner-0.7.0/src/llmtuner/train/orpo/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 def run_orpo(
     model_args: "ModelArguments",
     data_args: "DataArguments",
     training_args: "Seq2SeqTrainingArguments",
     finetuning_args: "FinetuningArguments",
     callbacks: Optional[List["TrainerCallback"]] = None,
 ):
-    tokenizer = load_tokenizer(model_args)
-    dataset = get_dataset(tokenizer, model_args, data_args, training_args, stage="rm")
+    tokenizer_module = load_tokenizer(model_args)
+    tokenizer = tokenizer_module["tokenizer"]
+    dataset = get_dataset(model_args, data_args, training_args, stage="rm", **tokenizer_module)
     model = load_model(tokenizer, model_args, finetuning_args, training_args.do_train)
 
     data_collator = PairwiseDataCollatorWithPadding(
         tokenizer=tokenizer,
         pad_to_multiple_of=8,
         label_pad_token_id=IGNORE_INDEX if data_args.ignore_pad_token_for_loss else tokenizer.pad_token_id,
     )
```

### Comparing `llmtuner-0.6.3/src/llmtuner/train/ppo/trainer.py` & `llmtuner-0.7.0/src/llmtuner/train/ppo/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/train/ppo/utils.py` & `llmtuner-0.7.0/src/llmtuner/train/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/train/ppo/workflow.py` & `llmtuner-0.7.0/src/llmtuner/train/ppo/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,17 @@
     model_args: "ModelArguments",
     data_args: "DataArguments",
     training_args: "Seq2SeqTrainingArguments",
     finetuning_args: "FinetuningArguments",
     generating_args: "GeneratingArguments",
     callbacks: Optional[List["TrainerCallback"]] = None,
 ):
-    tokenizer = load_tokenizer(model_args)
-    dataset = get_dataset(tokenizer, model_args, data_args, training_args, stage="ppo")
+    tokenizer_module = load_tokenizer(model_args)
+    tokenizer = tokenizer_module["tokenizer"]
+    dataset = get_dataset(model_args, data_args, training_args, stage="ppo", **tokenizer_module)
     model = load_model(tokenizer, model_args, finetuning_args, training_args.do_train, add_valuehead=True)
 
     tokenizer.padding_side = "left"  # use left-padding in generation while using right-padding in training
     data_collator = DataCollatorWithPadding(tokenizer=tokenizer)
 
     # Create reference model and reward model
     ref_model = create_ref_model(model_args, finetuning_args, add_valuehead=True)
```

### Comparing `llmtuner-0.6.3/src/llmtuner/train/pt/trainer.py` & `llmtuner-0.7.0/src/llmtuner/train/pt/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/train/pt/workflow.py` & `llmtuner-0.7.0/src/llmtuner/train/pt/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 def run_pt(
     model_args: "ModelArguments",
     data_args: "DataArguments",
     training_args: "Seq2SeqTrainingArguments",
     finetuning_args: "FinetuningArguments",
     callbacks: Optional[List["TrainerCallback"]] = None,
 ):
-    tokenizer = load_tokenizer(model_args)
-    dataset = get_dataset(tokenizer, model_args, data_args, training_args, stage="pt")
+    tokenizer_module = load_tokenizer(model_args)
+    tokenizer = tokenizer_module["tokenizer"]
+    dataset = get_dataset(model_args, data_args, training_args, stage="pt", **tokenizer_module)
     model = load_model(tokenizer, model_args, finetuning_args, training_args.do_train)
     data_collator = DataCollatorForLanguageModeling(tokenizer=tokenizer, mlm=False)
 
     # Initialize our Trainer
     trainer = CustomTrainer(
         model=model,
         args=training_args,
```

### Comparing `llmtuner-0.6.3/src/llmtuner/train/rm/trainer.py` & `llmtuner-0.7.0/src/llmtuner/train/rm/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/train/rm/workflow.py` & `llmtuner-0.7.0/src/llmtuner/train/rm/workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 def run_rm(
     model_args: "ModelArguments",
     data_args: "DataArguments",
     training_args: "Seq2SeqTrainingArguments",
     finetuning_args: "FinetuningArguments",
     callbacks: Optional[List["TrainerCallback"]] = None,
 ):
-    tokenizer = load_tokenizer(model_args)
-    dataset = get_dataset(tokenizer, model_args, data_args, training_args, stage="rm")
+    tokenizer_module = load_tokenizer(model_args)
+    tokenizer = tokenizer_module["tokenizer"]
+    dataset = get_dataset(model_args, data_args, training_args, stage="rm", **tokenizer_module)
     model = load_model(tokenizer, model_args, finetuning_args, training_args.do_train, add_valuehead=True)
     data_collator = PairwiseDataCollatorWithPadding(tokenizer, pad_to_multiple_of=8)
 
     # Update arguments
     training_args.remove_unused_columns = False  # important for pairwise dataset
 
     # Initialize our Trainer
```

### Comparing `llmtuner-0.6.3/src/llmtuner/train/sft/metric.py` & `llmtuner-0.7.0/src/llmtuner/train/sft/metric.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/train/sft/trainer.py` & `llmtuner-0.7.0/src/llmtuner/train/sft/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/train/sft/workflow.py` & `llmtuner-0.7.0/src/llmtuner/train/sft/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
     model_args: "ModelArguments",
     data_args: "DataArguments",
     training_args: "Seq2SeqTrainingArguments",
     finetuning_args: "FinetuningArguments",
     generating_args: "GeneratingArguments",
     callbacks: Optional[List["TrainerCallback"]] = None,
 ):
-    tokenizer = load_tokenizer(model_args)
-    dataset = get_dataset(tokenizer, model_args, data_args, training_args, stage="sft")
+    tokenizer_module = load_tokenizer(model_args)
+    tokenizer = tokenizer_module["tokenizer"]
+    dataset = get_dataset(model_args, data_args, training_args, stage="sft", **tokenizer_module)
     model = load_model(tokenizer, model_args, finetuning_args, training_args.do_train)
 
     if training_args.predict_with_generate:
         tokenizer.padding_side = "left"  # use left-padding in generation
 
     if getattr(model, "is_quantized", False) and not training_args.do_train:
         setattr(model, "_hf_peft_config_loaded", True)  # hack here: make model compatible with prediction
@@ -43,14 +44,15 @@
         pad_to_multiple_of=8 if tokenizer.padding_side == "right" else None,  # for shift short attention
         label_pad_token_id=IGNORE_INDEX if data_args.ignore_pad_token_for_loss else tokenizer.pad_token_id,
     )
 
     # Override the decoding parameters of Seq2SeqTrainer
     training_args.generation_max_length = training_args.generation_max_length or data_args.cutoff_len
     training_args.generation_num_beams = data_args.eval_num_beams or training_args.generation_num_beams
+    training_args.remove_unused_columns = False if model_args.visual_inputs else training_args.remove_unused_columns
 
     # Initialize our Trainer
     trainer = CustomSeq2SeqTrainer(
         model=model,
         args=training_args,
         finetuning_args=finetuning_args,
         tokenizer=tokenizer,
```

### Comparing `llmtuner-0.6.3/src/llmtuner/train/tuner.py` & `llmtuner-0.7.0/src/llmtuner/train/tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     if model_args.export_dir is None:
         raise ValueError("Please specify `export_dir` to save model.")
 
     if model_args.adapter_name_or_path is not None and model_args.export_quantization_bit is not None:
         raise ValueError("Please merge adapters before quantizing the model.")
 
-    tokenizer = load_tokenizer(model_args)
+    tokenizer = load_tokenizer(model_args)["tokenizer"]
     get_template_and_fix_tokenizer(tokenizer, data_args.template)
     model = load_model(tokenizer, model_args, finetuning_args)  # must after fixing tokenizer to resize vocab
 
     if getattr(model, "quantization_method", None) and model_args.adapter_name_or_path is not None:
         raise ValueError("Cannot merge adapters to a quantized model.")
 
     if not isinstance(model, PreTrainedModel):
```

### Comparing `llmtuner-0.6.3/src/llmtuner/train/utils.py` & `llmtuner-0.7.0/src/llmtuner/train/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,17 @@
         "tasks": "text-generation",
         "finetuned_from": model_args.model_name_or_path,
         "tags": ["llama-factory", finetuning_args.finetuning_type],
     }
     if data_args.dataset is not None:
         kwargs["dataset"] = [dataset.strip() for dataset in data_args.dataset.split(",")]
 
+    if model_args.use_unsloth:
+        kwargs["tags"] = kwargs["tags"] + ["unsloth"]
+
     if not training_args.do_train:
         pass
     elif training_args.push_to_hub:
         trainer.push_to_hub(**kwargs)
     else:
         trainer.create_model_card(license="other", **kwargs)  # prevent from connecting to hub
 
@@ -84,24 +87,24 @@
                 model_name_or_path=finetuning_args.ref_model,
                 adapter_name_or_path=finetuning_args.ref_model_adapters,
                 quantization_bit=finetuning_args.ref_model_quantization_bit,
             )
         )
         ref_model_args = ModelArguments(**ref_model_args_dict)
         ref_finetuning_args = FinetuningArguments(finetuning_type="lora")
-        tokenizer = load_tokenizer(ref_model_args)
+        tokenizer = load_tokenizer(ref_model_args)["tokenizer"]
         ref_model = load_model(
             tokenizer, ref_model_args, ref_finetuning_args, is_trainable=False, add_valuehead=add_valuehead
         )
         logger.info("Created reference model from {}".format(finetuning_args.ref_model))
     else:
         if finetuning_args.finetuning_type == "lora":
             ref_model = None
         else:
-            tokenizer = load_tokenizer(model_args)
+            tokenizer = load_tokenizer(model_args)["tokenizer"]
             ref_model = load_model(
                 tokenizer, model_args, finetuning_args, is_trainable=False, add_valuehead=add_valuehead
             )
             logger.info("Created reference model from the model itself.")
 
     return ref_model
 
@@ -140,15 +143,15 @@
                 model_name_or_path=finetuning_args.reward_model,
                 adapter_name_or_path=finetuning_args.reward_model_adapters,
                 quantization_bit=finetuning_args.reward_model_quantization_bit,
             )
         )
         reward_model_args = ModelArguments(**reward_model_args_dict)
         reward_finetuning_args = FinetuningArguments(finetuning_type="lora")
-        tokenizer = load_tokenizer(reward_model_args)
+        tokenizer = load_tokenizer(reward_model_args)["tokenizer"]
         reward_model = load_model(
             tokenizer, reward_model_args, reward_finetuning_args, is_trainable=False, add_valuehead=True
         )
         logger.info("Loaded full weights of reward model from {}".format(finetuning_args.reward_model))
         logger.warning("Please ensure the ppo model and reward model share SAME tokenizer and vocabulary.")
         return reward_model
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/chatter.py` & `llmtuner-0.7.0/src/llmtuner/webui/chatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
 import os
 from typing import TYPE_CHECKING, Dict, Generator, List, Optional, Sequence, Tuple
 
+from numpy.typing import NDArray
+
 from ..chat import ChatModel
 from ..data import Role
 from ..extras.misc import torch_gc
 from ..extras.packages import is_gradio_available
 from .common import get_save_dir
 from .locales import ALERTS
 
@@ -27,15 +29,18 @@
 
         if not lazy_init:  # read arguments from command line
             super().__init__()
 
         if demo_mode and os.environ.get("DEMO_MODEL") and os.environ.get("DEMO_TEMPLATE"):  # load demo model
             model_name_or_path = os.environ.get("DEMO_MODEL")
             template = os.environ.get("DEMO_TEMPLATE")
-            super().__init__(dict(model_name_or_path=model_name_or_path, template=template))
+            infer_backend = os.environ.get("DEMO_BACKEND", "huggingface")
+            super().__init__(
+                dict(model_name_or_path=model_name_or_path, template=template, infer_backend=infer_backend)
+            )
 
     @property
     def loaded(self) -> bool:
         return self.engine is not None
 
     def load_model(self, data) -> Generator[str, None, None]:
         get = lambda elem_id: data[self.manager.get_elem_by_id(elem_id)]
@@ -68,16 +73,17 @@
         yield ALERTS["info_loading"][lang]
         args = dict(
             model_name_or_path=get("top.model_path"),
             adapter_name_or_path=adapter_name_or_path,
             finetuning_type=get("top.finetuning_type"),
             quantization_bit=int(get("top.quantization_bit")) if get("top.quantization_bit") in ["8", "4"] else None,
             template=get("top.template"),
-            flash_attn=(get("top.booster") == "flash_attn"),
+            flash_attn="fa2" if get("top.booster") == "flashattn2" else "auto",
             use_unsloth=(get("top.booster") == "unsloth"),
+            visual_inputs=get("top.visual_inputs"),
             rope_scaling=get("top.rope_scaling") if get("top.rope_scaling") in ["linear", "dynamic"] else None,
             infer_backend=get("infer.infer_backend"),
         )
         super().__init__(args)
 
         yield ALERTS["info_loaded"][lang]
 
@@ -105,22 +111,23 @@
 
     def stream(
         self,
         chatbot: List[List[Optional[str]]],
         messages: Sequence[Dict[str, str]],
         system: str,
         tools: str,
+        image: Optional[NDArray],
         max_new_tokens: int,
         top_p: float,
         temperature: float,
     ) -> Generator[Tuple[List[List[Optional[str]]], List[Dict[str, str]]], None, None]:
         chatbot[-1][1] = ""
         response = ""
         for new_text in self.stream_chat(
-            messages, system, tools, max_new_tokens=max_new_tokens, top_p=top_p, temperature=temperature
+            messages, system, tools, image, max_new_tokens=max_new_tokens, top_p=top_p, temperature=temperature
         ):
             response += new_text
             if tools:
                 result = self.engine.template.format_tools.extract(response)
             else:
                 result = response
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/common.py` & `llmtuner-0.7.0/src/llmtuner/webui/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from peft.utils import SAFETENSORS_WEIGHTS_NAME, WEIGHTS_NAME
 
 from ..extras.constants import (
     DATA_CONFIG,
     DEFAULT_MODULE,
     DEFAULT_TEMPLATE,
+    MLLM_LIST,
     PEFT_METHODS,
     STAGES_USE_PAIR_DATA,
     SUPPORTED_MODELS,
     TRAINING_STAGES,
     DownloadSource,
 )
 from ..extras.misc import use_modelscope
@@ -101,14 +102,18 @@
 
 def get_template(model_name: str) -> str:
     if model_name and model_name.endswith("Chat") and get_prefix(model_name) in DEFAULT_TEMPLATE:
         return DEFAULT_TEMPLATE[get_prefix(model_name)]
     return "default"
 
 
+def get_visual(model_name: str) -> bool:
+    return get_prefix(model_name) in MLLM_LIST
+
+
 def list_adapters(model_name: str, finetuning_type: str) -> "gr.Dropdown":
     if finetuning_type not in PEFT_METHODS:
         return gr.Dropdown(value=[], choices=[], interactive=False)
 
     adapters = []
     if model_name and finetuning_type == "lora":
         save_dir = get_save_dir(model_name, finetuning_type)
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/components/chatbot.py` & `llmtuner-0.7.0/src/llmtuner/webui/components/chatbot.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,23 +13,29 @@
     from gradio.components import Component
 
     from ..engine import Engine
 
 
 def create_chat_box(
     engine: "Engine", visible: bool = False
-) -> Tuple["gr.Column", "Component", "Component", Dict[str, "Component"]]:
+) -> Tuple["Component", "Component", Dict[str, "Component"]]:
     with gr.Column(visible=visible) as chat_box:
         chatbot = gr.Chatbot(show_copy_button=True)
         messages = gr.State([])
         with gr.Row():
             with gr.Column(scale=4):
-                role = gr.Dropdown(choices=[Role.USER.value, Role.OBSERVATION.value], value=Role.USER.value)
-                system = gr.Textbox(show_label=False)
-                tools = gr.Textbox(show_label=False, lines=2)
+                with gr.Row():
+                    with gr.Column():
+                        role = gr.Dropdown(choices=[Role.USER.value, Role.OBSERVATION.value], value=Role.USER.value)
+                        system = gr.Textbox(show_label=False)
+                        tools = gr.Textbox(show_label=False, lines=3)
+
+                    with gr.Column() as image_box:
+                        image = gr.Image(sources=["upload"], type="numpy")
+
                 query = gr.Textbox(show_label=False, lines=8)
                 submit_btn = gr.Button(variant="primary")
 
             with gr.Column(scale=1):
                 max_new_tokens = gr.Slider(8, 4096, value=512, step=1)
                 top_p = gr.Slider(0.01, 1.0, value=0.7, step=0.01)
                 temperature = gr.Slider(0.01, 1.5, value=0.95, step=0.01)
@@ -39,27 +45,29 @@
 
     submit_btn.click(
         engine.chatter.append,
         [chatbot, messages, role, query],
         [chatbot, messages, query],
     ).then(
         engine.chatter.stream,
-        [chatbot, messages, system, tools, max_new_tokens, top_p, temperature],
+        [chatbot, messages, system, tools, image, max_new_tokens, top_p, temperature],
         [chatbot, messages],
     )
     clear_btn.click(lambda: ([], []), outputs=[chatbot, messages])
 
     return (
-        chat_box,
         chatbot,
         messages,
         dict(
+            chat_box=chat_box,
             role=role,
             system=system,
             tools=tools,
+            image_box=image_box,
+            image=image,
             query=query,
             submit_btn=submit_btn,
             max_new_tokens=max_new_tokens,
             top_p=top_p,
             temperature=temperature,
             clear_btn=clear_btn,
         ),
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/components/data.py` & `llmtuner-0.7.0/src/llmtuner/webui/components/data.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/components/eval.py` & `llmtuner-0.7.0/src/llmtuner/webui/components/eval.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/components/export.py` & `llmtuner-0.7.0/src/llmtuner/webui/components/export.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import TYPE_CHECKING, Dict, Generator, List
 
+from ...extras.misc import torch_gc
 from ...extras.packages import is_gradio_available
 from ...train import export_model
 from ..common import get_save_dir
 from ..locales import ALERTS
 
 
 if is_gradio_available():
@@ -22,17 +23,19 @@
 def save_model(
     lang: str,
     model_name: str,
     model_path: str,
     adapter_path: List[str],
     finetuning_type: str,
     template: str,
-    max_shard_size: int,
+    visual_inputs: bool,
+    export_size: int,
     export_quantization_bit: int,
     export_quantization_dataset: str,
+    export_device: str,
     export_legacy_format: bool,
     export_dir: str,
     export_hub_model_id: str,
 ) -> Generator[str, None, None]:
     error = ""
     if not model_name:
         error = ALERTS["err_no_model"][lang]
@@ -40,14 +43,16 @@
         error = ALERTS["err_no_path"][lang]
     elif not export_dir:
         error = ALERTS["err_no_export_dir"][lang]
     elif export_quantization_bit in GPTQ_BITS and not export_quantization_dataset:
         error = ALERTS["err_no_dataset"][lang]
     elif export_quantization_bit not in GPTQ_BITS and not adapter_path:
         error = ALERTS["err_no_adapter"][lang]
+    elif export_quantization_bit in GPTQ_BITS and adapter_path:
+        error = ALERTS["err_gptq_lora"][lang]
 
     if error:
         gr.Warning(error)
         yield error
         return
 
     if adapter_path:
@@ -58,32 +63,36 @@
         adapter_name_or_path = None
 
     args = dict(
         model_name_or_path=model_path,
         adapter_name_or_path=adapter_name_or_path,
         finetuning_type=finetuning_type,
         template=template,
+        visual_inputs=visual_inputs,
         export_dir=export_dir,
         export_hub_model_id=export_hub_model_id or None,
-        export_size=max_shard_size,
+        export_size=export_size,
         export_quantization_bit=int(export_quantization_bit) if export_quantization_bit in GPTQ_BITS else None,
         export_quantization_dataset=export_quantization_dataset,
+        export_device=export_device,
         export_legacy_format=export_legacy_format,
     )
 
     yield ALERTS["info_exporting"][lang]
     export_model(args)
+    torch_gc()
     yield ALERTS["info_exported"][lang]
 
 
 def create_export_tab(engine: "Engine") -> Dict[str, "Component"]:
     with gr.Row():
-        max_shard_size = gr.Slider(value=1, minimum=1, maximum=100, step=1)
+        export_size = gr.Slider(value=1, minimum=1, maximum=100, step=1)
         export_quantization_bit = gr.Dropdown(choices=["none", "8", "4", "3", "2"], value="none")
         export_quantization_dataset = gr.Textbox(value="data/c4_demo.json")
+        export_device = gr.Radio(choices=["cpu", "cuda"], value="cpu")
         export_legacy_format = gr.Checkbox()
 
     with gr.Row():
         export_dir = gr.Textbox()
         export_hub_model_id = gr.Textbox()
 
     export_btn = gr.Button()
@@ -94,27 +103,30 @@
         [
             engine.manager.get_elem_by_id("top.lang"),
             engine.manager.get_elem_by_id("top.model_name"),
             engine.manager.get_elem_by_id("top.model_path"),
             engine.manager.get_elem_by_id("top.adapter_path"),
             engine.manager.get_elem_by_id("top.finetuning_type"),
             engine.manager.get_elem_by_id("top.template"),
-            max_shard_size,
+            engine.manager.get_elem_by_id("top.visual_inputs"),
+            export_size,
             export_quantization_bit,
             export_quantization_dataset,
+            export_device,
             export_legacy_format,
             export_dir,
             export_hub_model_id,
         ],
         [info_box],
     )
 
     return dict(
-        max_shard_size=max_shard_size,
+        export_size=export_size,
         export_quantization_bit=export_quantization_bit,
         export_quantization_dataset=export_quantization_dataset,
+        export_device=export_device,
         export_legacy_format=export_legacy_format,
         export_dir=export_dir,
         export_hub_model_id=export_hub_model_id,
         export_btn=export_btn,
         info_box=info_box,
     )
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/components/infer.py` & `llmtuner-0.7.0/src/llmtuner/webui/components/infer.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,19 +24,25 @@
         unload_btn = gr.Button()
 
     info_box = gr.Textbox(show_label=False, interactive=False)
 
     input_elems.update({infer_backend})
     elem_dict.update(dict(infer_backend=infer_backend, load_btn=load_btn, unload_btn=unload_btn, info_box=info_box))
 
-    chat_box, chatbot, messages, chat_elems = create_chat_box(engine, visible=False)
-    elem_dict.update(dict(chat_box=chat_box, **chat_elems))
+    chatbot, messages, chat_elems = create_chat_box(engine, visible=False)
+    elem_dict.update(chat_elems)
 
     load_btn.click(engine.chatter.load_model, input_elems, [info_box]).then(
-        lambda: gr.Column(visible=engine.chatter.loaded), outputs=[chat_box]
+        lambda: gr.Column(visible=engine.chatter.loaded), outputs=[chat_elems["chat_box"]]
     )
 
     unload_btn.click(engine.chatter.unload_model, input_elems, [info_box]).then(
         lambda: ([], []), outputs=[chatbot, messages]
-    ).then(lambda: gr.Column(visible=engine.chatter.loaded), outputs=[chat_box])
+    ).then(lambda: gr.Column(visible=engine.chatter.loaded), outputs=[chat_elems["chat_box"]])
+
+    engine.manager.get_elem_by_id("top.visual_inputs").change(
+        lambda enabled: gr.Column(visible=enabled),
+        [engine.manager.get_elem_by_id("top.visual_inputs")],
+        [chat_elems["image_box"]],
+    )
 
     return elem_dict
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/components/top.py` & `llmtuner-0.7.0/src/llmtuner/webui/components/top.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING, Dict
 
 from ...data import templates
 from ...extras.constants import METHODS, SUPPORTED_MODELS
 from ...extras.packages import is_gradio_available
-from ..common import get_model_path, get_template, list_adapters, save_config
+from ..common import get_model_path, get_template, get_visual, list_adapters, save_config
 from ..utils import can_quantize
 
 
 if is_gradio_available():
     import gradio as gr
 
 
@@ -26,22 +26,25 @@
     with gr.Row():
         finetuning_type = gr.Dropdown(choices=METHODS, value="lora", scale=1)
         adapter_path = gr.Dropdown(multiselect=True, allow_custom_value=True, scale=5)
         refresh_btn = gr.Button(scale=1)
 
     with gr.Accordion(open=False) as advanced_tab:
         with gr.Row():
-            quantization_bit = gr.Dropdown(choices=["none", "8", "4"], value="none")
-            template = gr.Dropdown(choices=list(templates.keys()), value="default")
-            rope_scaling = gr.Radio(choices=["none", "linear", "dynamic"], value="none")
-            booster = gr.Radio(choices=["none", "flashattn", "unsloth"], value="none")
+            quantization_bit = gr.Dropdown(choices=["none", "8", "4"], value="none", scale=2)
+            template = gr.Dropdown(choices=list(templates.keys()), value="default", scale=2)
+            rope_scaling = gr.Radio(choices=["none", "linear", "dynamic"], value="none", scale=3)
+            booster = gr.Radio(choices=["none", "flashattn2", "unsloth"], value="none", scale=3)
+            visual_inputs = gr.Checkbox(scale=1)
 
     model_name.change(list_adapters, [model_name, finetuning_type], [adapter_path], queue=False).then(
         get_model_path, [model_name], [model_path], queue=False
-    ).then(get_template, [model_name], [template], queue=False)  # do not save config since the below line will save
+    ).then(get_template, [model_name], [template], queue=False).then(
+        get_visual, [model_name], [visual_inputs], queue=False
+    )  # do not save config since the below line will save
 
     model_path.change(save_config, inputs=[lang, model_name, model_path], queue=False)
 
     finetuning_type.change(list_adapters, [model_name, finetuning_type], [adapter_path], queue=False).then(
         can_quantize, [finetuning_type], [quantization_bit], queue=False
     )
 
@@ -55,8 +58,9 @@
         adapter_path=adapter_path,
         refresh_btn=refresh_btn,
         advanced_tab=advanced_tab,
         quantization_bit=quantization_bit,
         template=template,
         rope_scaling=rope_scaling,
         booster=booster,
+        visual_inputs=visual_inputs,
     )
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/components/train.py` & `llmtuner-0.7.0/src/llmtuner/webui/components/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         )
     )
 
     with gr.Accordion(open=False) as lora_tab:
         with gr.Row():
             lora_rank = gr.Slider(value=8, minimum=1, maximum=1024, step=1)
             lora_alpha = gr.Slider(value=16, minimum=1, maximum=2048, step=1)
-            lora_dropout = gr.Slider(value=0.1, minimum=0, maximum=1, step=0.01)
+            lora_dropout = gr.Slider(value=0, minimum=0, maximum=1, step=0.01)
             loraplus_lr_ratio = gr.Slider(value=0, minimum=0, maximum=64, step=0.01)
             create_new_adapter = gr.Checkbox()
 
         with gr.Row():
             with gr.Column(scale=1):
                 use_rslora = gr.Checkbox()
                 use_dora = gr.Checkbox()
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/css.py` & `llmtuner-0.7.0/src/llmtuner/webui/css.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/engine.py` & `llmtuner-0.7.0/src/llmtuner/webui/engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
         if not self.pure_chat:
             init_dict["train.dataset"] = {"choices": list_dataset().choices}
             init_dict["eval.dataset"] = {"choices": list_dataset().choices}
             init_dict["train.output_dir"] = {"value": "train_{}".format(get_time())}
             init_dict["train.config_path"] = {"value": "{}.json".format(get_time())}
             init_dict["eval.output_dir"] = {"value": "eval_{}".format(get_time())}
+            init_dict["infer.image_box"] = {"visible": False}
 
             if user_config.get("last_model", None):
                 init_dict["top.model_name"] = {"value": user_config["last_model"]}
                 init_dict["top.model_path"] = {"value": get_model_path(user_config["last_model"])}
 
         yield self._update_component(init_dict)
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/interface.py` & `llmtuner-0.7.0/src/llmtuner/webui/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 def create_web_demo() -> gr.Blocks:
     engine = Engine(pure_chat=True)
 
     with gr.Blocks(title="Web Demo", css=CSS) as demo:
         lang = gr.Dropdown(choices=["en", "zh"])
         engine.manager.add_elems("top", dict(lang=lang))
 
-        chat_box, _, _, chat_elems = create_chat_box(engine, visible=True)
-        engine.manager.add_elems("infer", dict(chat_box=chat_box, **chat_elems))
+        _, _, chat_elems = create_chat_box(engine, visible=True)
+        engine.manager.add_elems("infer", chat_elems)
 
         demo.load(engine.resume, outputs=engine.manager.get_elem_list(), concurrency_limit=None)
         lang.change(engine.change_lang, [lang], engine.manager.get_elem_list(), queue=False)
         lang.input(save_config, inputs=[lang], queue=False)
 
     return demo
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/locales.py` & `llmtuner-0.7.0/src/llmtuner/webui/locales.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,25 @@
         "ru": {
             "label": "Ускоритель",
         },
         "zh": {
             "label": "加速方式",
         },
     },
+    "visual_inputs": {
+        "en": {
+            "label": "Visual inputs",
+        },
+        "ru": {
+            "label": "визуальные входы",
+        },
+        "zh": {
+            "label": "图像输入",
+        },
+    },
     "training_stage": {
         "en": {
             "label": "Stage",
             "info": "The stage to perform in training.",
         },
         "ru": {
             "label": "Этап",
@@ -1069,14 +1080,25 @@
         "ru": {
             "placeholder": "Инструменты (по желанию)",
         },
         "zh": {
             "placeholder": "工具列表（非必填）",
         },
     },
+    "image": {
+        "en": {
+            "label": "Image (optional)",
+        },
+        "ru": {
+            "label": "Изображение (по желанию)",
+        },
+        "zh": {
+            "label": "图像（非必填）",
+        },
+    },
     "query": {
         "en": {
             "placeholder": "Input...",
         },
         "ru": {
             "placeholder": "Ввод...",
         },
@@ -1146,15 +1168,15 @@
         "ru": {
             "value": "Очистить историю",
         },
         "zh": {
             "value": "清空历史",
         },
     },
-    "max_shard_size": {
+    "export_size": {
         "en": {
             "label": "Max shard size (GB)",
             "info": "The maximum size for a model file.",
         },
         "ru": {
             "label": "Максимальный размер фрагмента (ГБ)",
             "info": "Максимальный размер файла модели.",
@@ -1188,14 +1210,28 @@
             "info": "Набор данных калибровки, используемый для квантования.",
         },
         "zh": {
             "label": "导出量化数据集",
             "info": "量化过程中使用的校准数据集。",
         },
     },
+    "export_device": {
+        "en": {
+            "label": "Export device",
+            "info": "Which device should be used to export model.",
+        },
+        "ru": {
+            "label": "Экспорт устройство",
+            "info": "Какое устройство следует использовать для экспорта модели.",
+        },
+        "zh": {
+            "label": "导出设备",
+            "info": "导出模型使用的设备类型。",
+        },
+    },
     "export_legacy_format": {
         "en": {
             "label": "Export legacy format",
             "info": "Do not use safetensors to save the model.",
         },
         "ru": {
             "label": "Экспорт в устаревший формат",
@@ -1283,15 +1319,20 @@
         "en": "Please select a reward model.",
         "ru": "Пожалуйста, выберите модель вознаграждения.",
         "zh": "请选择奖励模型。",
     },
     "err_no_export_dir": {
         "en": "Please provide export dir.",
         "ru": "Пожалуйста, укажите каталог для экспорта.",
-        "zh": "请填写导出目录",
+        "zh": "请填写导出目录。",
+    },
+    "err_gptq_lora": {
+        "en": "Please merge adapters before quantizing the model.",
+        "ru": "Пожалуйста, объедините адаптеры перед квантованием модели.",
+        "zh": "量化模型前请先合并适配器。",
     },
     "err_failed": {
         "en": "Failed.",
         "ru": "Ошибка.",
         "zh": "训练出错。",
     },
     "err_demo": {
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/manager.py` & `llmtuner-0.7.0/src/llmtuner/webui/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,8 +56,9 @@
             self._id_to_elem["top.model_path"],
             self._id_to_elem["top.finetuning_type"],
             self._id_to_elem["top.adapter_path"],
             self._id_to_elem["top.quantization_bit"],
             self._id_to_elem["top.template"],
             self._id_to_elem["top.rope_scaling"],
             self._id_to_elem["top.booster"],
+            self._id_to_elem["top.visual_inputs"],
         }
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/runner.py` & `llmtuner-0.7.0/src/llmtuner/webui/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         if not model_name:
             return ALERTS["err_no_model"][lang]
 
         if not model_path:
             return ALERTS["err_no_path"][lang]
 
-        if len(dataset) == 0:
+        if not dataset:
             return ALERTS["err_no_dataset"][lang]
 
         if not from_preview and self.demo_mode:
             return ALERTS["err_demo"][lang]
 
         if not from_preview and get_device_count() > 1:
             return ALERTS["err_device_count"][lang]
@@ -118,16 +118,17 @@
             model_name_or_path=get("top.model_path"),
             adapter_name_or_path=adapter_name_or_path,
             cache_dir=user_config.get("cache_dir", None),
             finetuning_type=get("top.finetuning_type"),
             quantization_bit=int(get("top.quantization_bit")) if get("top.quantization_bit") in ["8", "4"] else None,
             template=get("top.template"),
             rope_scaling=get("top.rope_scaling") if get("top.rope_scaling") in ["linear", "dynamic"] else None,
-            flash_attn=(get("top.booster") == "flashattn"),
+            flash_attn="fa2" if get("top.booster") == "flashattn2" else "auto",
             use_unsloth=(get("top.booster") == "unsloth"),
+            visual_inputs=get("top.visual_inputs"),
             dataset_dir=get("train.dataset_dir"),
             dataset=",".join(get("train.dataset")),
             cutoff_len=get("train.cutoff_len"),
             learning_rate=float(get("train.learning_rate")),
             num_train_epochs=float(get("train.num_train_epochs")),
             max_samples=int(get("train.max_samples")),
             per_device_train_batch_size=get("train.batch_size"),
@@ -218,16 +219,17 @@
             model_name_or_path=get("top.model_path"),
             adapter_name_or_path=adapter_name_or_path,
             cache_dir=user_config.get("cache_dir", None),
             finetuning_type=get("top.finetuning_type"),
             quantization_bit=int(get("top.quantization_bit")) if get("top.quantization_bit") in ["8", "4"] else None,
             template=get("top.template"),
             rope_scaling=get("top.rope_scaling") if get("top.rope_scaling") in ["linear", "dynamic"] else None,
-            flash_attn=(get("top.booster") == "flashattn"),
+            flash_attn="fa2" if get("top.booster") == "flashattn2" else "auto",
             use_unsloth=(get("top.booster") == "unsloth"),
+            visual_inputs=get("top.visual_inputs"),
             dataset_dir=get("eval.dataset_dir"),
             dataset=",".join(get("eval.dataset")),
             cutoff_len=get("eval.cutoff_len"),
             max_samples=int(get("eval.max_samples")),
             per_device_eval_batch_size=get("eval.batch_size"),
             predict_with_generate=True,
             max_new_tokens=get("eval.max_new_tokens"),
```

### Comparing `llmtuner-0.6.3/src/llmtuner/webui/utils.py` & `llmtuner-0.7.0/src/llmtuner/webui/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/src/llmtuner.egg-info/PKG-INFO` & `llmtuner-0.7.0/src/llmtuner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.6.3
+Version: 0.7.0
 Summary: Easy-to-use LLM fine-tuning framework
 Home-page: https://github.com/hiyouga/LLaMA-Factory
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -35,29 +35,27 @@
 Requires-Dist: protobuf
 Requires-Dist: uvicorn
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: sse-starlette
 Requires-Dist: matplotlib
 Requires-Dist: fire
+Requires-Dist: packaging
 Provides-Extra: deepspeed
 Requires-Dist: deepspeed>=0.10.0; extra == "deepspeed"
 Provides-Extra: metrics
 Requires-Dist: nltk; extra == "metrics"
 Requires-Dist: jieba; extra == "metrics"
 Requires-Dist: rouge-chinese; extra == "metrics"
-Provides-Extra: unsloth
-Requires-Dist: torch==2.2.0; extra == "unsloth"
-Requires-Dist: unsloth[cu121-ampere-torch220]; extra == "unsloth"
 Provides-Extra: galore
 Requires-Dist: galore-torch; extra == "galore"
 Provides-Extra: badam
 Requires-Dist: badam; extra == "badam"
 Provides-Extra: vllm
-Requires-Dist: vllm>=0.3.3; extra == "vllm"
+Requires-Dist: vllm>=0.4.0; extra == "vllm"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes>=0.39.0; extra == "bitsandbytes"
 Provides-Extra: gptq
 Requires-Dist: optimum>=1.16.0; extra == "gptq"
 Requires-Dist: auto-gptq>=0.5.0; extra == "gptq"
 Provides-Extra: awq
 Requires-Dist: autoawq; extra == "awq"
@@ -112,16 +110,16 @@
 - [Projects using LLaMA Factory](#projects-using-llama-factory)
 - [License](#license)
 - [Citation](#citation)
 - [Acknowledgement](#acknowledgement)
 
 ## Features
 
-- **Various models**: LLaMA, Mistral, Mixtral-MoE, Qwen, Yi, Gemma, Baichuan, ChatGLM, Phi, etc.
-- **Integrated methods**: (Continuous) pre-training, supervised fine-tuning, reward modeling, PPO, DPO and ORPO.
+- **Various models**: LLaMA, LLaVA, Mistral, Mixtral-MoE, Qwen, Yi, Gemma, Baichuan, ChatGLM, Phi, etc.
+- **Integrated methods**: (Continuous) pre-training, (multimodal) supervised fine-tuning, reward modeling, PPO, DPO and ORPO.
 - **Scalable resources**: 32-bit full-tuning, 16-bit freeze-tuning, 16-bit LoRA and 2/4/8-bit QLoRA via AQLM/AWQ/GPTQ/LLM.int8.
 - **Advanced algorithms**: GaLore, BAdam, DoRA, LongLoRA, LLaMA Pro, Mixture-of-Depths, LoRA+, LoftQ and Agent tuning.
 - **Practical tricks**: FlashAttention-2, Unsloth, RoPE scaling, NEFTune and rsLoRA.
 - **Experiment monitors**: LlamaBoard, TensorBoard, Wandb, MLflow, etc.
 - **Faster inference**: OpenAI-style API, Gradio UI and CLI with vLLM worker.
 
 ## Benchmark
@@ -137,17 +135,19 @@
 - **GPU Memory**: Peak GPU memory usage in 4-bit quantized training. (bs=1, cutoff_len=1024)
 - We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA Factory's LoRA tuning.
 
 </details>
 
 ## Changelog
 
-[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
+[24/04/26] We supported fine-tuning the **LLaVA-1.5** multimodal LLMs. See `examples/lora_single_gpu/sft_mllm.sh` for usage.
+
+[24/04/22] We provided a **[Colab notebook](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)** for fine-tuning the Llama-3 model on a free T4 GPU. Two Llama-3-derived models fine-tuned using LLaMA Factory are available at Hugging Face, check [Llama3-8B-Chinese-Chat](https://huggingface.co/shenzhi-wang/Llama3-8B-Chinese-Chat) and [Llama3-Chinese](https://huggingface.co/zhichen/Llama3-Chinese) for details.
 
-[24/04/19] We supported **Meta Llama 3** model series.
+[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
 
 [24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See `examples/extras/badam` for usage.
 
 [24/04/16] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s long-sequence training (Llama-2-7B-56k within 24GB). It achieves **117%** speed and **50%** memory compared with FlashAttention-2, more benchmarks can be found in [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison).
 
 <details><summary>Full Changelog</summary>
 
@@ -179,15 +179,15 @@
 
 [23/10/21] We supported **[NEFTune](https://arxiv.org/abs/2310.05914)** trick for fine-tuning. Try `--neftune_noise_alpha` argument to activate NEFTune, e.g., `--neftune_noise_alpha 5`.
 
 [23/09/27] We supported **$S^2$-Attn** proposed by [LongLoRA](https://github.com/dvlab-research/LongLoRA) for the LLaMA models. Try `--shift_attn` argument to enable shift short attention.
 
 [23/09/23] We integrated MMLU, C-Eval and CMMLU benchmarks in this repo. See [this example](#evaluation) to evaluate your models.
 
-[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `--flash_attn` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
+[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `--flash_attn fa2` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
 
 [23/08/12] We supported **RoPE scaling** to extend the context length of the LLaMA models. Try `--rope_scaling linear` argument in training and `--rope_scaling dynamic` argument at inference to extrapolate the position embeddings.
 
 [23/08/11] We supported **[DPO training](https://arxiv.org/abs/2305.18290)** for instruction-tuned models. See [this example](#dpo-training) to train your models.
 
 [23/07/31] We supported **dataset streaming**. Try `--streaming` and `--max_steps 10000` arguments to load your dataset in streaming mode.
 
@@ -203,42 +203,46 @@
 
 [23/06/03] We supported quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized models.
 
 </details>
 
 ## Supported Models
 
-| Model                                                    | Model size                  | Default module    | Template  |
-| -------------------------------------------------------- | --------------------------- | ----------------- | --------- |
-| [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                      | W_pack            | baichuan2 |
-| [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                          | query_key_value   | chatglm3  |
-| [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                    | q_proj,v_proj     | cohere    |
-| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                  | q_proj,v_proj     | deepseek  |
-| [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                 | query_key_value   | falcon    |
-| [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                       | q_proj,v_proj     | gemma     |
-| [InternLM2](https://huggingface.co/internlm)             | 7B/20B                      | wqkv              | intern2   |
-| [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B              | q_proj,v_proj     | -         |
-| [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                  | q_proj,v_proj     | llama2    |
-| [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                      | q_proj,v_proj     | llama3    |
-| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B/8x22B               | q_proj,v_proj     | mistral   |
-| [OLMo](https://huggingface.co/allenai)                   | 1B/7B                       | att_proj          | olmo      |
-| [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                   | q_proj,v_proj     | -         |
-| [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B             | c_attn            | qwen      |
-| [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B | q_proj,v_proj     | qwen      |
-| [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                   | q_proj,v_proj     | -         |
-| [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                  | q_proj,v_proj     | xverse    |
-| [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                   | q_proj,v_proj     | yi        |
-| [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                 | q_proj,v_proj     | yuan      |
+| Model                                                    | Model size                       | Default module    | Template  |
+| -------------------------------------------------------- | -------------------------------- | ----------------- | --------- |
+| [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                           | W_pack            | baichuan2 |
+| [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
+| [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
+| [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                               | query_key_value   | chatglm3  |
+| [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                         | q_proj,v_proj     | cohere    |
+| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                       | q_proj,v_proj     | deepseek  |
+| [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                      | query_key_value   | falcon    |
+| [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                            | q_proj,v_proj     | gemma     |
+| [InternLM2](https://huggingface.co/internlm)             | 7B/20B                           | wqkv              | intern2   |
+| [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B                   | q_proj,v_proj     | -         |
+| [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                       | q_proj,v_proj     | llama2    |
+| [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                           | q_proj,v_proj     | llama3    |
+| [LLaVA-1.5](https://huggingface.co/llava-hf)             | 7B/13B                           | q_proj,v_proj     | vicuna    |
+| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B/8x22B                    | q_proj,v_proj     | mistral   |
+| [OLMo](https://huggingface.co/allenai)                   | 1B/7B                            | q_proj,v_proj     | -         |
+| [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                        | q_proj,v_proj     | -         |
+| [Phi-3](https://huggingface.co/microsoft)                | 3.8B                             | qkv_proj          | phi       |
+| [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B                  | c_attn            | qwen      |
+| [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B/110B | q_proj,v_proj     | qwen      |
+| [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                        | q_proj,v_proj     | -         |
+| [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                       | q_proj,v_proj     | xverse    |
+| [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                        | q_proj,v_proj     | yi        |
+| [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                      | q_proj,v_proj     | yuan      |
 
 > [!NOTE]
-> **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules.
+> **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules for better convergence.
 >
-> For the "base" models, the `--template` argument can be chosen from `default`, `alpaca`, `vicuna` etc. But make sure to use the **corresponding template** for the "chat" models.
+> For the "base" models, the `--template` argument can be chosen from `default`, `alpaca`, `vicuna` etc. But make sure to use the **corresponding template** for the "instruct/chat" models.
+>
+> Remember to use the **SAME** template in training and inference.
 
 Please refer to [constants.py](src/llmtuner/extras/constants.py) for a full list of models we supported.
 
 You also can add a custom chat template to [template.py](src/llmtuner/data/template.py).
 
 ## Supported Training Approaches
 
@@ -301,14 +305,15 @@
 - [ShareGPT4 (en&zh)](https://huggingface.co/datasets/shibing624/sharegpt_gpt4)
 - [UltraChat 200k (en)](https://huggingface.co/datasets/HuggingFaceH4/ultrachat_200k)
 - [AgentInstruct (en)](https://huggingface.co/datasets/THUDM/AgentInstruct)
 - [LMSYS Chat 1M (en)](https://huggingface.co/datasets/lmsys/lmsys-chat-1m)
 - [Evol Instruct V2 (en)](https://huggingface.co/datasets/WizardLM/WizardLM_evol_instruct_V2_196k)
 - [Glaive Function Calling V2 (en)](https://huggingface.co/datasets/glaiveai/glaive-function-calling-v2)
 - [Cosmopedia (en)](https://huggingface.co/datasets/HuggingFaceTB/cosmopedia)
+- [LLaVA mixed (en&zh)](https://huggingface.co/datasets/BUAADreamer/llava-en-zh-300k)
 - [Open Assistant (de)](https://huggingface.co/datasets/mayflowergmbh/oasst_de)
 - [Dolly 15k (de)](https://huggingface.co/datasets/mayflowergmbh/dolly-15k_de)
 - [Alpaca GPT4 (de)](https://huggingface.co/datasets/mayflowergmbh/alpaca-gpt4_de)
 - [OpenSchnabeltier (de)](https://huggingface.co/datasets/mayflowergmbh/openschnabeltier_de)
 - [Evol Instruct (de)](https://huggingface.co/datasets/mayflowergmbh/evol-instruct_de)
 - [Dolphin (de)](https://huggingface.co/datasets/mayflowergmbh/dolphin_de)
 - [Booksum (de)](https://huggingface.co/datasets/mayflowergmbh/booksum_de)
@@ -320,15 +325,15 @@
 <details><summary>Preference datasets</summary>
 
 - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
 - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 - [Orca DPO (en)](https://huggingface.co/datasets/Intel/orca_dpo_pairs)
 - [Nectar (en)](https://huggingface.co/datasets/berkeley-nest/Nectar)
-- [DPO mix (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
+- [DPO mixed (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
 - [Orca DPO (de)](https://huggingface.co/datasets/mayflowergmbh/intel_orca_dpo_pairs_de)
 
 </details>
 
 Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
@@ -355,23 +360,23 @@
 | bitsandbytes | 0.39.0  | 0.43.0    |
 | flash-attn   | 2.3.0   | 2.5.6     |
 
 ### Hardware Requirement
 
 \* *estimated*
 
-| Method            | Bits |   7B  |  13B  |  30B  |   70B  |  8x7B |  8x22B |
-| ----------------- | ---- | ----- | ----- | ----- | ------ | ----- | ------ |
-| Full              | AMP  | 120GB | 240GB | 600GB | 1200GB | 900GB | 2400GB |
-| Full              |  16  |  60GB | 120GB | 300GB |  600GB | 400GB | 1200GB |
-| Freeze            |  16  |  20GB |  40GB |  80GB |  200GB | 160GB |  400GB |
-| LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB | 120GB |  320GB |
-| QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  60GB |  160GB |
-| QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |  30GB |   96GB |
-| QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |  18GB |   48GB |
+| Method            | Bits |   7B  |  13B  |  30B  |   70B  |  110B  |  8x7B |  8x22B |
+| ----------------- | ---- | ----- | ----- | ----- | ------ | ------ | ----- | ------ |
+| Full              | AMP  | 120GB | 240GB | 600GB | 1200GB | 2000GB | 900GB | 2400GB |
+| Full              |  16  |  60GB | 120GB | 300GB |  600GB |  900GB | 400GB | 1200GB |
+| Freeze            |  16  |  20GB |  40GB |  80GB |  200GB |  360GB | 160GB |  400GB |
+| LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB |  240GB | 120GB |  320GB |
+| QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  140GB |  60GB |  160GB |
+| QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |   72GB |  30GB |   96GB |
+| QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |   48GB |  18GB |   48GB |
 
 ## Getting Started
 
 ### Data Preparation
 
 Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
 
@@ -384,41 +389,51 @@
 git clone https://github.com/hiyouga/LLaMA-Factory.git
 conda create -n llama_factory python=3.10
 conda activate llama_factory
 cd LLaMA-Factory
 pip install -e .[metrics]
 ```
 
-Extra dependencies available: deepspeed, metrics, unsloth, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
+Extra dependencies available: deepspeed, metrics, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
 
 <details><summary>For Windows users</summary>
 
 If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
 
 ```bash
 pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.2.post2-py3-none-win_amd64.whl
 ```
 
 To enable FlashAttention-2 on the Windows platform, you need to install the precompiled `flash-attn` library, which supports CUDA 12.1 to 12.2. Please download the corresponding version from [flash-attention](https://github.com/bdashore3/flash-attention/releases) based on your requirements.
 
 </details>
 
-### LLaMA Board GUI
+### Train with LLaMA Board GUI (powered by [Gradio](https://github.com/gradio-app/gradio))
 
 > [!IMPORTANT]
 > LLaMA Board GUI only supports training on a single GPU, please use [CLI](#command-line-interface) for distributed training.
 
 #### Use local environment
 
 ```bash
 export CUDA_VISIBLE_DEVICES=0 # `set CUDA_VISIBLE_DEVICES=0` for Windows
 export GRADIO_SERVER_PORT=7860 # `set GRADIO_SERVER_PORT=7860` for Windows
 python src/train_web.py # or python -m llmtuner.webui.interface
 ```
 
+<details><summary>For Alibaba Cloud users</summary>
+
+If you encountered display problems in LLaMA Board on Alibaba Cloud, try using the following command to set environment variables before starting LLaMA Board:
+
+```bash
+export GRADIO_ROOT_PATH=/${JUPYTER_NAME}/proxy/7860/
+```
+
+</details>
+
 #### Use Docker
 
 ```bash
 docker build -f ./Dockerfile -t llama-factory:latest .
 docker run --gpus=all \
     -v ./hf_cache:/root/.cache/huggingface/ \
     -v ./data:/app/data \
@@ -440,39 +455,39 @@
 
 - hf_cache: Utilize Hugging Face cache on the host machine. Reassignable if a cache already exists in a different directory.
 - data: Place datasets on this dir of the host machine so that they can be selected on LLaMA Board GUI.
 - output: Set export dir to this location so that the merged result can be accessed directly on the host machine.
 
 </details>
 
-### Command Line Interface
+### Train with Command Line Interface
 
 See [examples/README.md](examples/README.md) for usage.
 
 Use `python src/train_bash.py -h` to display arguments description.
 
 ### Deploy with OpenAI-style API and vLLM
 
 ```bash
 CUDA_VISIBLE_DEVICES=0,1 API_PORT=8000 python src/api_demo.py \
-    --model_name_or_path mistralai/Mistral-7B-Instruct-v0.2 \
-    --template mistral \
+    --model_name_or_path meta-llama/Meta-Llama-3-8B-Instruct \
+    --template llama3 \
     --infer_backend vllm \
     --vllm_enforce_eager
 ```
 
-### Use ModelScope Hub
+### Download from ModelScope Hub
 
 If you have trouble with downloading models and datasets from Hugging Face, you can use ModelScope.
 
 ```bash
 export USE_MODELSCOPE_HUB=1 # `set USE_MODELSCOPE_HUB=1` for Windows
 ```
 
-Train the model by specifying a model ID of the ModelScope Hub as the `--model_name_or_path`. You can find a full list of model IDs at [ModelScope Hub](https://modelscope.cn/models), e.g., `modelscope/Llama-2-7b-ms`.
+Train the model by specifying a model ID of the ModelScope Hub as the `--model_name_or_path`. You can find a full list of model IDs at [ModelScope Hub](https://modelscope.cn/models), e.g., `LLM-Research/Meta-Llama-3-8B-Instruct`.
 
 ## Projects using LLaMA Factory
 
 If you have a project that should be incorporated, please contact via email or create a pull request.
 
 <details><summary>Click to show</summary>
 
@@ -513,15 +528,15 @@
 
 </details>
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
-Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
+Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2/LLaVA-1.5](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Phi-3](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/LICENSE) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
 @article{zheng2024llamafactory,
```

### Comparing `llmtuner-0.6.3/src/llmtuner.egg-info/SOURCES.txt` & `llmtuner-0.7.0/src/llmtuner.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -31,28 +31,38 @@
 src/llmtuner/extras/__init__.py
 src/llmtuner/extras/callbacks.py
 src/llmtuner/extras/constants.py
 src/llmtuner/extras/logging.py
 src/llmtuner/extras/misc.py
 src/llmtuner/extras/packages.py
 src/llmtuner/extras/ploting.py
-src/llmtuner/extras/patches/__init__.py
-src/llmtuner/extras/patches/llama_patch.py
 src/llmtuner/hparams/__init__.py
 src/llmtuner/hparams/data_args.py
 src/llmtuner/hparams/evaluation_args.py
 src/llmtuner/hparams/finetuning_args.py
 src/llmtuner/hparams/generating_args.py
 src/llmtuner/hparams/model_args.py
 src/llmtuner/hparams/parser.py
 src/llmtuner/model/__init__.py
 src/llmtuner/model/adapter.py
 src/llmtuner/model/loader.py
 src/llmtuner/model/patcher.py
-src/llmtuner/model/utils.py
+src/llmtuner/model/utils/__init__.py
+src/llmtuner/model/utils/attention.py
+src/llmtuner/model/utils/checkpointing.py
+src/llmtuner/model/utils/embedding.py
+src/llmtuner/model/utils/longlora.py
+src/llmtuner/model/utils/misc.py
+src/llmtuner/model/utils/mod.py
+src/llmtuner/model/utils/moe.py
+src/llmtuner/model/utils/quantization.py
+src/llmtuner/model/utils/rope.py
+src/llmtuner/model/utils/unsloth.py
+src/llmtuner/model/utils/valuehead.py
+src/llmtuner/model/utils/visual.py
 src/llmtuner/train/__init__.py
 src/llmtuner/train/tuner.py
 src/llmtuner/train/utils.py
 src/llmtuner/train/dpo/__init__.py
 src/llmtuner/train/dpo/trainer.py
 src/llmtuner/train/dpo/workflow.py
 src/llmtuner/train/orpo/__init__.py
```

### Comparing `llmtuner-0.6.3/tests/test_attn.py` & `llmtuner-0.7.0/tests/test_attn.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/tests/test_galore.py` & `llmtuner-0.7.0/tests/test_galore.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/tests/test_throughput.py` & `llmtuner-0.7.0/tests/test_throughput.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.3/tests/test_toolcall.py` & `llmtuner-0.7.0/tests/test_toolcall.py`

 * *Files identical despite different names*

