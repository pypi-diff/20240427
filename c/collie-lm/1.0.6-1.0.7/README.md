# Comparing `tmp/collie-lm-1.0.6.tar.gz` & `tmp/collie_lm-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collie-lm-1.0.6.tar", last modified: Tue Mar  5 11:59:53 2024, max compression
+gzip compressed data, was "collie_lm-1.0.7.tar", last modified: Sat Apr 27 14:42:23 2024, max compression
```

## Comparing `collie-lm-1.0.6.tar` & `collie_lm-1.0.7.tar`

### file list

```diff
@@ -1,136 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.493724 collie-lm-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-05 11:59:43.000000 collie-lm-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-05 11:59:53.493724 collie-lm-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-03-05 11:59:43.000000 collie-lm-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.473724 collie-lm-1.0.6/collie/
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.473724 collie-lm-1.0.6/collie/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/callbacks/callback_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/callbacks/checkpoint_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/callbacks/has_monitor_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/callbacks/load_best_model_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    12378 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/callbacks/topk_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/callbacks/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.477724 collie-lm-1.0.6/collie/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20799 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/controller/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/controller/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    44074 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/controller/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/controller/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.477724 collie-lm-1.0.6/collie/data/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/data/batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.477724 collie-lm-1.0.6/collie/driver/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/driver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.477724 collie-lm-1.0.6/collie/driver/io/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/driver/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/driver/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/driver/io/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/driver/io/petrel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.477724 collie-lm-1.0.6/collie/log/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/log/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/log/highlighter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/log/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/log/print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.481724 collie-lm-1.0.6/collie/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12371 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/metrics/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/metrics/classify_f1_pre_rec_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/metrics/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/metrics/ppl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/metrics/rouge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.481724 collie-lm-1.0.6/collie/models/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35768 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.481724 collie-lm-1.0.6/collie/models/chatglm/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/chatglm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51812 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/chatglm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.481724 collie-lm-1.0.6/collie/models/chatglm2/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/chatglm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60707 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/chatglm2/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.481724 collie-lm-1.0.6/collie/models/internlm/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/internlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33771 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/internlm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.481724 collie-lm-1.0.6/collie/models/internlm2/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/internlm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/internlm2/configuration_internlm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    68586 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/internlm2/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.481724 collie-lm-1.0.6/collie/models/llama/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/llama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34948 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/llama/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.481724 collie-lm-1.0.6/collie/models/moss/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/moss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32025 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/moss/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.485724 collie-lm-1.0.6/collie/models/moss_moon/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/moss_moon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26944 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/moss_moon/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/moss_moon/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31684 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.485724 collie-lm-1.0.6/collie/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/optim/adalomo.py
--rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/optim/lomo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/optim/sophiag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.485724 collie-lm-1.0.6/collie/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28431 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/utils/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    24739 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/utils/metric_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/utils/padder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/utils/peft_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    45963 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/utils/pipeline_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/utils/rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/utils/seq_len_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    26973 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.485724 collie-lm-1.0.6/collie_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.489724 collie-lm-1.0.6/collie_cli/bullet/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/bullet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/bullet/charDef.py
--rw-r--r--   0 runner    (1001) docker     (127)    25857 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/bullet/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/bullet/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/bullet/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/bullet/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/bullet/keyhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/bullet/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/bullet/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/collie_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9865 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-05 11:59:43.000000 collie-lm-1.0.6/collie_cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.493724 collie-lm-1.0.6/collie_lm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-05 11:59:53.000000 collie-lm-1.0.6/collie_lm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-03-05 11:59:53.000000 collie-lm-1.0.6/collie_lm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 11:59:53.000000 collie-lm-1.0.6/collie_lm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-05 11:59:53.000000 collie-lm-1.0.6/collie_lm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-05 11:59:53.000000 collie-lm-1.0.6/collie_lm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-05 11:59:53.000000 collie-lm-1.0.6/collie_lm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 11:59:53.493724 collie-lm-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-05 11:59:43.000000 collie-lm-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.489724 collie-lm-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.489724 collie-lm-1.0.6/tests/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/callbacks/_test_checkpoint_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/callbacks/_test_load_best_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/callbacks/test_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.489724 collie-lm-1.0.6/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/helpers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:53.493724 collie-lm-1.0.6/tests/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/trainer/_test_checkpoint_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/trainer/_test_trainer_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/trainer/_test_trainer_metric_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-03-05 11:59:43.000000 collie-lm-1.0.6/tests/trainer/test_trainer_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.245554 collie_lm-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 14:42:14.000000 collie_lm-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-27 14:42:23.245554 collie_lm-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11921 2024-04-27 14:42:14.000000 collie_lm-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.225554 collie_lm-1.0.7/collie/
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.229554 collie_lm-1.0.7/collie/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/callbacks/callback_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/callbacks/checkpoint_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/callbacks/has_monitor_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/callbacks/load_best_model_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12378 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/callbacks/topk_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/callbacks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10648 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.229554 collie_lm-1.0.7/collie/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20799 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/controller/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/controller/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43793 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/controller/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/controller/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.229554 collie_lm-1.0.7/collie/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/data/batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20605 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/data/template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.229554 collie_lm-1.0.7/collie/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/driver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.229554 collie_lm-1.0.7/collie/driver/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/driver/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/driver/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/driver/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/driver/io/petrel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.229554 collie_lm-1.0.7/collie/log/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/log/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/log/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/log/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/log/print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.233554 collie_lm-1.0.7/collie/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12371 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/metrics/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/metrics/classify_f1_pre_rec_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/metrics/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/metrics/ppl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/metrics/rouge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.233554 collie_lm-1.0.7/collie/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35768 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.233554 collie_lm-1.0.7/collie/models/chatglm/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/chatglm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51812 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/chatglm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.233554 collie_lm-1.0.7/collie/models/chatglm2/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/chatglm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60707 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/chatglm2/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.233554 collie_lm-1.0.7/collie/models/internlm/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/internlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33771 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/internlm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.233554 collie_lm-1.0.7/collie/models/internlm2/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/internlm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/internlm2/configuration_internlm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69001 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/internlm2/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.233554 collie_lm-1.0.7/collie/models/llama/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/llama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34948 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/llama/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.237554 collie_lm-1.0.7/collie/models/moss/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/moss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32025 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/moss/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.237554 collie_lm-1.0.7/collie/models/moss_moon/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/moss_moon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26944 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/moss_moon/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/moss_moon/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31818 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.237554 collie_lm-1.0.7/collie/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/optim/adalomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/optim/lomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/optim/sophiag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.237554 collie_lm-1.0.7/collie/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28431 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/utils/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24765 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/utils/metric_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/utils/padder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/utils/peft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38835 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/utils/pipeline_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/utils/rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/utils/seq_len_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26973 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.241554 collie_lm-1.0.7/collie_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.241554 collie_lm-1.0.7/collie_cli/bullet/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/bullet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/bullet/charDef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25857 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/bullet/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/bullet/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/bullet/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/bullet/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/bullet/keyhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/bullet/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/bullet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/collie_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9865 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-27 14:42:14.000000 collie_lm-1.0.7/collie_cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.245554 collie_lm-1.0.7/collie_lm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-27 14:42:23.000000 collie_lm-1.0.7/collie_lm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-27 14:42:23.000000 collie_lm-1.0.7/collie_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:42:23.000000 collie_lm-1.0.7/collie_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-27 14:42:23.000000 collie_lm-1.0.7/collie_lm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 14:42:23.000000 collie_lm-1.0.7/collie_lm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 14:42:23.000000 collie_lm-1.0.7/collie_lm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 14:42:23.245554 collie_lm-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-27 14:42:14.000000 collie_lm-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.241554 collie_lm-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.245554 collie_lm-1.0.7/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/callbacks/_test_checkpoint_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/callbacks/_test_load_best_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/callbacks/test_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.245554 collie_lm-1.0.7/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/helpers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:23.245554 collie_lm-1.0.7/tests/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/trainer/_test_checkpoint_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/trainer/_test_trainer_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/trainer/_test_trainer_metric_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/trainer/test_trainer_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-27 14:42:14.000000 collie_lm-1.0.7/tests/trainer/test_trainer_peft_save.py
```

### Comparing `collie-lm-1.0.6/LICENSE` & `collie_lm-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/PKG-INFO` & `collie_lm-1.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collie-lm
-Version: 1.0.6
+Version: 1.0.7
 Summary: CoLLiE: Collaborative Training of Large Language Models in an Efficient Way
 Author: OpenLMLab
 Author-email: yanhang@pjlab.org.cn
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: deepspeed>=0.10.0
 Requires-Dist: tqdm
@@ -22,7 +22,8 @@
 Requires-Dist: wandb
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: accelerate>=0.20.3
 Requires-Dist: bitsandbytes>=0.41.0
 Requires-Dist: scipy
 Requires-Dist: rich>=13.3.5
+Requires-Dist: safetensors
```

### Comparing `collie-lm-1.0.6/README.md` & `collie_lm-1.0.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -76,43 +76,18 @@
   <summary>完整特性</summary>
   <div align="center">
       <img src="docs/assets/images/features.svg" width="800px">
   </div>
 </details>
 
 ## CoLLiE支持的模型
-- [MOSS-MOON](https://github.com/OpenLMLab/MOSS)
-    - [moss-moon-003-base](https://huggingface.co/fnlp/moss-moon-003-base)
-    - [moss-moon-003-sft](https://huggingface.co/fnlp/moss-moon-003-sft)
-    - [moss-moon-003-sft-plugin](https://huggingface.co/fnlp/moss-moon-003-sft-plugin)
-- [InternLM](https://github.com/InternLM/InternLM)
-    - [internlm-7b](https://huggingface.co/internlm/internlm-7b)
-    - [internlm-chat-7b](https://huggingface.co/internlm/internlm-chat-7b)
-    - [internlm-chat-7b-8k](https://huggingface.co/internlm/internlm-chat-7b-8k)
-- [LLaMA](https://github.com/facebookresearch/llama)
-    - [llama-7b-hf](https://huggingface.co/decapoda-research/llama-7b-hf)
-    - [llama-13b-hf](https://huggingface.co/decapoda-research/llama-13b-hf)
-    - [llama-30b-hf](https://huggingface.co/decapoda-research/llama-30b-hf)
-    - [llama-65b-hf](https://huggingface.co/decapoda-research/llama-65b-hf)
-- [LLaMA-2](https://github.com/facebookresearch/llama)
-    - [Llama-2-7b-hf](https://huggingface.co/meta-llama/Llama-2-7b-hf)
-    - [Llama-2-13b-hf](https://huggingface.co/meta-llama/Llama-2-13b-hf)
-    - [Llama-2-70b-hf](https://huggingface.co/meta-llama/Llama-2-70b-hf)
-    - [Llama-2-7b-chat-hf](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf)
-    - [Llama-2-13b-chat-hf](https://huggingface.co/meta-llama/Llama-2-13b-chat-hf)
-    - [Llama-2-70b-chat-hf](https://huggingface.co/meta-llama/Llama-2-70b-chat-hf)
-- [OpenLLaMA](https://github.com/openlm-research/open_llama)
-    - [open_llama_3b](https://huggingface.co/openlm-research/open_llama_3b)
-    - [open_llama_7b](https://huggingface.co/openlm-research/open_llama_7b)
-    - [open_llama_13b](https://huggingface.co/openlm-research/open_llama_13b)
-    - [open_llama_7b_v2](https://huggingface.co/openlm-research/open_llama_7b_v2)
-- [ChatGLM](https://github.com/THUDM/ChatGLM-6B)
-    - [chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
-- [ChatGLM2](https://github.com/THUDM/ChatGLM2-6B)
-    - [chatglm2-6b](https://huggingface.co/THUDM/chatglm2-6b)
+- MOSS系列：[MOSS-MOON](https://github.com/OpenMOSS/MOSS)
+- InternLM系列：[InternLM2](https://github.com/InternLM/InternLM)
+- LLaMA系列：[LLaMA](https://github.com/meta-llama/llama)、[LLaMA-2](https://github.com/meta-llama/llama)
+- ChatGLM系列：[ChatGLM](https://github.com/THUDM/ChatGLM2-6B)、[ChatGLM2](https://github.com/THUDM/ChatGLM2-6B)
 
 
 ## 评测
 
 ### 显存占用
 使用张量并行测试了批量大小为 1，序列长度为 2048，梯度累计步数为 2 下显存占用情况，结果如下：
```

#### html2text {}

```diff
@@ -45,44 +45,24 @@
 - å¹¶è¡ç­ç¥ - æ°æ®å¹¶è¡ (DP) - [æµæ°´çº¿å¹¶è¡ (PP)](https://arxiv.org/
 pdf/1811.06965.pdf) - [å¼ éå¹¶è¡ (TP)](https://arxiv.org/pdf/2104.04473.pdf)
 - [é¶åä½ä¼åå¨ (ZeRO)](https://arxiv.org/pdf/1910.02054.pdf) -
 é«æå¾®è° - [LOMO](https://arxiv.org/pdf/2306.09782.pdf) - [LoRA](https://
 arxiv.org/pdf/2106.09685.pdf) - [Flash Attention](https://arxiv.org/pdf/
 2205.14135.pdf) - è®¾è®¡ä¼é - ç¨æ·åå¥½ å®æ´ç¹æ§
                        [docs/assets/images/features.svg]
-## CoLLiEæ¯æçæ¨¡å - [MOSS-MOON](https://github.com/OpenLMLab/MOSS) -
-[moss-moon-003-base](https://huggingface.co/fnlp/moss-moon-003-base) - [moss-
-moon-003-sft](https://huggingface.co/fnlp/moss-moon-003-sft) - [moss-moon-003-
-sft-plugin](https://huggingface.co/fnlp/moss-moon-003-sft-plugin) - [InternLM]
-(https://github.com/InternLM/InternLM) - [internlm-7b](https://huggingface.co/
-internlm/internlm-7b) - [internlm-chat-7b](https://huggingface.co/internlm/
-internlm-chat-7b) - [internlm-chat-7b-8k](https://huggingface.co/internlm/
-internlm-chat-7b-8k) - [LLaMA](https://github.com/facebookresearch/llama) -
-[llama-7b-hf](https://huggingface.co/decapoda-research/llama-7b-hf) - [llama-
-13b-hf](https://huggingface.co/decapoda-research/llama-13b-hf) - [llama-30b-hf]
-(https://huggingface.co/decapoda-research/llama-30b-hf) - [llama-65b-hf](https:
-//huggingface.co/decapoda-research/llama-65b-hf) - [LLaMA-2](https://
-github.com/facebookresearch/llama) - [Llama-2-7b-hf](https://huggingface.co/
-meta-llama/Llama-2-7b-hf) - [Llama-2-13b-hf](https://huggingface.co/meta-llama/
-Llama-2-13b-hf) - [Llama-2-70b-hf](https://huggingface.co/meta-llama/Llama-2-
-70b-hf) - [Llama-2-7b-chat-hf](https://huggingface.co/meta-llama/Llama-2-7b-
-chat-hf) - [Llama-2-13b-chat-hf](https://huggingface.co/meta-llama/Llama-2-13b-
-chat-hf) - [Llama-2-70b-chat-hf](https://huggingface.co/meta-llama/Llama-2-70b-
-chat-hf) - [OpenLLaMA](https://github.com/openlm-research/open_llama) -
-[open_llama_3b](https://huggingface.co/openlm-research/open_llama_3b) -
-[open_llama_7b](https://huggingface.co/openlm-research/open_llama_7b) -
-[open_llama_13b](https://huggingface.co/openlm-research/open_llama_13b) -
-[open_llama_7b_v2](https://huggingface.co/openlm-research/open_llama_7b_v2) -
-[ChatGLM](https://github.com/THUDM/ChatGLM-6B) - [chatglm-6b](https://
-huggingface.co/THUDM/chatglm-6b) - [ChatGLM2](https://github.com/THUDM/
-ChatGLM2-6B) - [chatglm2-6b](https://huggingface.co/THUDM/chatglm2-6b) ##
-è¯æµ ### æ¾å­å ç¨ ä½¿ç¨å¼ éå¹¶è¡æµè¯äºæ¹éå¤§å°ä¸º
-1ï¼åºåé¿åº¦ä¸º 2048ï¼æ¢¯åº¦ç´¯è®¡æ­¥æ°ä¸º 2
-ä¸æ¾å­å ç¨æåµï¼ç»æå¦ä¸ï¼ [docs/assets/images/mem_req.png]###
-ååé å¨ A100 å RTX-3090 ä¸æµè¯äºä¸åæ¹éå¤§å°ä¸ä½¿ç¨ Adam
+## CoLLiEæ¯æçæ¨¡å - MOSSç³»åï¼[MOSS-MOON](https://github.com/
+OpenMOSS/MOSS) - InternLMç³»åï¼[InternLM2](https://github.com/InternLM/
+InternLM) - LLaMAç³»åï¼[LLaMA](https://github.com/meta-llama/llama)ã
+[LLaMA-2](https://github.com/meta-llama/llama) - ChatGLMç³»åï¼[ChatGLM]
+(https://github.com/THUDM/ChatGLM2-6B)ã[ChatGLM2](https://github.com/THUDM/
+ChatGLM2-6B) ## è¯æµ ### æ¾å­å ç¨
+ä½¿ç¨å¼ éå¹¶è¡æµè¯äºæ¹éå¤§å°ä¸º 1ï¼åºåé¿åº¦ä¸º
+2048ï¼æ¢¯åº¦ç´¯è®¡æ­¥æ°ä¸º 2 ä¸æ¾å­å ç¨æåµï¼ç»æå¦ä¸ï¼ [docs/
+assets/images/mem_req.png]### ååé å¨ A100 å RTX-3090
+ä¸æµè¯äºä¸åæ¹éå¤§å°ä¸ä½¿ç¨ Adam
 ä¼åå¨çååéï¼ç»æå¦ä¸ï¼ [docs/assets/images/throughput.png]##
 å®è£ å¨å®è£åï¼ä½ éè¦ç¡®ä¿ï¼ * PyTorch >= 1.13 * CUDA >= 11.6 *
 Linux OS ### PyPIå®è£ ä½ å¯ä»¥ç®åå°éè¿PyPIå®è£ï¼å½ä»¤å¦ä¸ï¼
 ```bash pip install collie-lm ``` ### æºç å®è£ ```bash git clone https://
 github.com/OpenLMLab/collie python setup.py install ``` ## Dockerå®è£ ##
 ä½¿ç¨ ### å¿«éå¼å§
 ä¸é¢å°æä¾ä¸ä¸ªä½¿ç¨CoLLiEè®­ç»Mossçæ ·ä¾ï¼åæ¶ä½¿ç¨LOMOä¼åå¨ï¼å¹¶ä¸å¼å¯ZeRO3æ¥éä½æ¾å­æ¶èã
```

### Comparing `collie-lm-1.0.6/collie/__init__.py` & `collie_lm-1.0.7/collie/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .controller import Trainer, Evaluator, EvaluatorForPerplexity, \
     EvaluatorForClassfication, EvaluatorForGeneration, Server
 from .config import CollieConfig
 from .metrics import BaseMetric, DecodeMetric, AccuracyMetric, \
     PPLMetric, BleuMetric, ClassifyFPreRecMetric
 from .data import CollieDatasetForClassification, CollieBatchSampler, \
     CollieDataLoader, CollieDatasetForTraining, CollieDatasetForGeneration, \
-        CollieDatasetForPerplexity
+    CollieDatasetForPerplexity, CollieDatasetForTemplatedMultiTurnChat
 from .optim import Lomo, Lion, SophiaG, Adan
 
 __all__ = [
     # controller
     'Trainer',
     'Evaluator',
     'EvaluatorForPerplexity',
@@ -77,16 +77,16 @@
     'env',
     'setup_ds_engine',
     'zero3_load_state_dict',
     'is_zero3_enabled',
     'broadcast_tensor',
     'concat_tensor',
     'find_tensors',
-    'BaseProvider', 
-    'GradioProvider', 
+    'BaseProvider',
+    'GradioProvider',
     'BaseMonitor',
     'StepTimeMonitor',
     'TGSMonitor',
     'MemoryMonitor',
     'LossMonitor',
     'EvalMonitor',
     'LRMonitor',
@@ -96,30 +96,31 @@
     "is_static_method",
     "auto_param_call",
     "NetworkIOMonitor",
     "DiskIOMonitor",
     "CPUMemoryMonitor",
     "ColliePadder",
     "get_keys_to_not_convert",
-    
+
     # metrics
     'BaseMetric',
-    'DecodeMetric', 
-    'AccuracyMetric', 
+    'DecodeMetric',
+    'AccuracyMetric',
     'PPLMetric',
     'BleuMetric',
     'ClassifyFPreRecMetric',
-    
-    #data
-    'CollieDatasetForClassification', 
-    'CollieBatchSampler', 
-    'CollieDataLoader', 
+
+    # data
+    'CollieDatasetForClassification',
+    'CollieBatchSampler',
+    'CollieDataLoader',
     'CollieDatasetForTraining',
+    'CollieDatasetForTemplatedMultiTurnChat',
     'CollieDatasetForGeneration',
     'CollieDatasetForPerplexity',
-    
+
     # optim
     "Lomo",
     "Lion",
     "SophiaG",
     "Adan"
-]
+]
```

### Comparing `collie-lm-1.0.6/collie/callbacks/callback.py` & `collie_lm-1.0.7/collie/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/callbacks/callback_manager.py` & `collie_lm-1.0.7/collie/callbacks/callback_manager.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/callbacks/checkpoint_callback.py` & `collie_lm-1.0.7/collie/callbacks/checkpoint_callback.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/callbacks/has_monitor_callback.py` & `collie_lm-1.0.7/collie/callbacks/has_monitor_callback.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/callbacks/load_best_model_callback.py` & `collie_lm-1.0.7/collie/callbacks/load_best_model_callback.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/callbacks/topk_saver.py` & `collie_lm-1.0.7/collie/callbacks/topk_saver.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/callbacks/utils.py` & `collie_lm-1.0.7/collie/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/config.py` & `collie_lm-1.0.7/collie/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,17 +96,17 @@
     use_flash: bool = field(
         default=True, metadata={"help": "Whether to use flash attention."}
     )
     dropout: float = field(default=0.0, metadata={"help": "Dropout probability."})
     init_method: dict = field(
         default_factory=lambda: {'init_func': torch.nn.init.normal_, 'init_kwargs': {'mean': 0.0, 'std': 0.02}},
         metadata={
-        "help": "Initialization method. Possible values are 'normal', 'xavier_normal', "
-        "'xavier_uniform', 'kaiming_normal', 'kaiming_uniform', 'orthogonal', 'sparse', "
-        "'eye', 'dirac'. Default is 'torch.nn.init.normal_' with mean = 0.0 and std = 0.02."
+            "help": "Initialization method. Possible values are 'normal', 'xavier_normal', "
+                    "'xavier_uniform', 'kaiming_normal', 'kaiming_uniform', 'orthogonal', 'sparse', "
+                    "'eye', 'dirac'. Default is 'torch.nn.init.normal_' with mean = 0.0 and std = 0.02."
         }
     )
     low_cpu_mem_usage: bool = field(
         default=True,
         metadata={
             "help": "Tries to not use more than 1x model size in CPU memory (including peak memory) while loading the model."
         },
@@ -191,14 +191,18 @@
     def __str__(self) -> str:
         title = self.__class__.__name__
         r = f"{title}:\n"
         r += _repr_dict(self.__dict__, 0)
         return r
 
     def valid_config(self):
+        """
+        验证配置是否合法。
+        """
+        # sanity check
         if (
             "zero_optimization" in self.ds_config.keys()
             and "stage" in self.ds_config["zero_optimization"].keys()
             and self.ds_config["zero_optimization"]["stage"] == 3
         ):
             assert self.pp_size == 1, "Pipeline is not compatible with Zero3."
         if self.tp_size > 1:
@@ -206,14 +210,19 @@
                 self.peft_config.peft_type != PeftType.LORA
             ), "Tensor parallelism is not compatible with LoRa"
             assert (
                 not self.quantization_config.load_in_4bit
                 and not self.quantization_config.load_in_8bit
             ), "Tensor parallelism is not compatible with int8 quantization and int4 quantization"
 
+        if 'train_micro_batch_size_per_gpu' not in self.ds_config:
+            self.ds_config['train_micro_batch_size_per_gpu'] = self.train_micro_batch_size
+        if 'gradient_accumulation_steps' not in self.ds_config:
+            self.ds_config['gradient_accumulation_steps'] = self.gradient_accumulation_steps
+
 
 def load_config(path: str):
     content = {}
     if path.lower().endswith("yaml"):
         import yaml
 
         content = yaml.load(open(path, "r"), Loader=yaml.SafeLoader)
```

### Comparing `collie-lm-1.0.6/collie/controller/evaluator.py` & `collie_lm-1.0.7/collie/controller/evaluator.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/controller/server.py` & `collie_lm-1.0.7/collie/controller/server.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/controller/trainer.py` & `collie_lm-1.0.7/collie/controller/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,21 +608,15 @@
                     )
                     if env.dp_rank == 0 and env.tp_rank == 0:
                         io_driver.save(state_dict, os.path.join(path, name))
             if is_zero3_enabled(self.config):
                 self._checkpoint_epilogue()
             env.barrier()
             if env.rank == 0:
-                inference_mode = peft_config.inference_mode
-                peft_config.inference_mode = True
-                io_driver.save(
-                    json.dumps(peft_config.__dict__),
-                    os.path.join(path, "adapter_config.json"),
-                )
-                peft_config.inference_mode = inference_mode
+                peft_config.save_pretrained(output_dir)
                 if pp_save:
                     pp_merge_peft(path, name_prefix, io_driver)
 
     def load_peft(
         self,
         path: str,
         adapter_name="default",
```

### Comparing `collie-lm-1.0.6/collie/controller/utils.py` & `collie_lm-1.0.7/collie/controller/utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/data/batch_sampler.py` & `collie_lm-1.0.7/collie/data/batch_sampler.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/data/dataloader.py` & `collie_lm-1.0.7/collie/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/data/dataset.py` & `collie_lm-1.0.7/collie/data/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 import io
 import json
 import mmap
 import os
 import random
 import threading
 from functools import reduce
-from typing import Dict, List, Optional, Sequence, Tuple
+from typing import Dict, List, Optional, Sequence, Tuple, Callable
 
 import numpy as np
 import torch
 from torch.utils.data import Dataset
 from torch.utils.data.dataset import Dataset
 from transformers import PreTrainedTokenizer
 
 from collie.driver.io import FileIODriver
+from .template_utils import tokenize_conversation
 
 __all__ = [
     "CollieDatasetForTraining",
+    "CollieDatasetForTemplatedMultiTurnChat",
     "CollieDatasetForGeneration",
     "CollieDatasetForClassification",
 ]
 
 
 class _ShardContainer(list):
     def __init__(self, path, shuffle: bool = False, seed: int = 1024) -> None:
@@ -51,34 +53,34 @@
 
     def _get_mmap(self, path):
         if not hasattr(self.threadlocal, "handles"):
             with open(path, "rb") as f:
                 mm = mmap.mmap(f.fileno(), 0, access=mmap.ACCESS_READ)
                 self.threadlocal.handles = [f, mm]
                 if (
-                    path.endswith(".gz")
-                    or path.endswith(".bz")
-                    or path.endswith(".bz2")
+                        path.endswith(".gz")
+                        or path.endswith(".bz")
+                        or path.endswith(".bz2")
                 ):
                     raise NotImplementedError(
                         "Compressed files are not supported because .seek() would require "
                         "rereading the entire file, making performance too slow."
                     )
         return self.threadlocal.handles[-1]
 
     def __len__(self):
         return len(self.meta)
 
     def __getitem__(self, index):
         meta = self.meta[self.indices[index]]
         file_name: str = meta["file"]
         if (
-            self.file is None
-            or self.file_name != file_name.replace(".meta", "")
-            or (isinstance(self.file, mmap.mmap) and self.file.closed)
+                self.file is None
+                or self.file_name != file_name.replace(".meta", "")
+                or (isinstance(self.file, mmap.mmap) and self.file.closed)
         ):
             self.file_name = file_name.replace(".meta", "")
             if self.file is not None:
                 self.file.close()
             self.file = self._get_mmap(self.file_name)
         self.file.seek(meta["offset"])
         return json.loads(self.file.readline().decode())
@@ -88,22 +90,22 @@
     ids_with_special_tokens = tokenizer("a", add_special_tokens=True).input_ids
     ids_without_special_tokens = tokenizer("a", add_special_tokens=False).input_ids
     bos_length = 0
     for bos_length in range(len(ids_with_special_tokens)):
         if ids_with_special_tokens[bos_length] == ids_without_special_tokens[0]:
             break
     eos_length = (
-        len(ids_with_special_tokens) - len(ids_without_special_tokens) - bos_length
+            len(ids_with_special_tokens) - len(ids_without_special_tokens) - bos_length
     )
     return bos_length, eos_length
 
 
 class CollieDatasetForTraining(Dataset):
     """**CoLLie** 中的基本数据格式，可用于预训练、微调任务。
-    需提供的数据格式形似：
+    需提供的dataset数据格式形似：
 
     .. code-block::
 
         [
             {
                 "text": "这是prompt部分的文本",
             },
@@ -135,21 +137,21 @@
         ]
 
     当使用第二种数据格式时，只有 `output` 部分的 token 会参与 loss计算。
     当使用第二种数据格式时，`labels` 字段是可选的，如果不提供 `labels` 默认计算所有 token 的 loss
     """
 
     def __init__(
-        self,
-        dataset: Sequence[Dict],
-        tokenizer: Optional[PreTrainedTokenizer] = None,
-        add_special_tokens: bool = True,
-        shuffle: bool = False,
-        seed: int = 1024,
-        max_length: int = -1,
+            self,
+            dataset: Sequence[Dict],
+            tokenizer: Optional[PreTrainedTokenizer] = None,
+            add_special_tokens: bool = True,
+            shuffle: bool = False,
+            seed: int = 1024,
+            max_length: int = -1,
     ):
         self.dataset = dataset
         self.tokenizer = tokenizer
         self.add_special_tokens = add_special_tokens
         self.indices = list(range(len(self.dataset)))
         self.max_length = max_length
         if shuffle:
@@ -157,50 +159,54 @@
             random.shuffle(self.indices)
         if self.tokenizer is not None:
             self.bos_length, self.eos_length = _inspect_special_tokens_length(self.tokenizer)
 
     def __len__(self):
         return len(self.dataset)
 
-    def __getitem__(self, index) -> Dict:
+    def __getitem__(self, index) -> Dict or List[Dict]:
         if isinstance(index, slice):
             return self._get_slice(index)
         if index > len(self):
             raise IndexError("Index out of range.")
         index = self.indices[index]
         if self.tokenizer is None:
+            if isinstance(self.dataset[index]["tokens"], torch.Tensor):
+                self.dataset[index]["tokens"] = self.dataset[index]["tokens"].numpy().tolist()
+            if isinstance(self.dataset[index]["labels"], torch.Tensor):
+                self.dataset[index]["labels"] = self.dataset[index]["labels"].numpy().tolist()
             input_ids = self.dataset[index]["tokens"]
-            labels = self.dataset[index].get("labels", input_ids.detach().clone())
+            labels = self.dataset[index].get("labels", input_ids.copy())
             if "attention_mask" in self.dataset[index].keys():
                 attention_mask = self.dataset[index]["attention_mask"]
             else:
-                attention_mask = torch.ones_like(torch.tensor(input_ids)).cpu().tolist()
+                attention_mask = [1 for _ in range(len(input_ids))]
         else:
             if "text" in self.dataset[0].keys():
                 inputs = self.tokenizer(
                     self.dataset[index]["text"],
                     add_special_tokens=self.add_special_tokens,
                 )
                 input_ids = inputs["input_ids"]
                 labels = torch.tensor(input_ids).cpu().tolist()
                 attention_mask = inputs.get(
                     "attention_mask",
-                    torch.ones_like(torch.tensor(input_ids)).cpu().tolist(),
+                    [1 for _ in range(len(input_ids))],
                 )
             elif (
-                "input" in self.dataset[0].keys() and "output" in self.dataset[0].keys()
+                    "input" in self.dataset[0].keys() and "output" in self.dataset[0].keys()
             ):
                 inputs = self.tokenizer(
                     self.dataset[index]["input"] + self.dataset[index]["output"],
                     add_special_tokens=self.add_special_tokens,
                 )
                 input_ids = inputs["input_ids"]
                 attention_mask = inputs.get(
                     "attention_mask",
-                    torch.ones_like(torch.tensor(input_ids)).cpu().tolist(),
+                    [1 for _ in range(len(input_ids))],
                 )
                 labels = torch.tensor(input_ids)
                 target_length = len(
                     self.tokenizer(
                         self.dataset[index]["output"],
                         add_special_tokens=self.add_special_tokens,
                     ).input_ids
@@ -225,34 +231,34 @@
         result = []
         for idx in self.indices[s]:
             result.append(self[idx])
         return result
 
     @classmethod
     def from_json(
-        cls,
-        path: str,
-        tokenizer: Optional[PreTrainedTokenizer] = None,
-        shuffle: bool = False,
-        seed: int = 1024,
+            cls,
+            path: str,
+            tokenizer: Optional[PreTrainedTokenizer] = None,
+            shuffle: bool = False,
+            seed: int = 1024,
     ):
         dataset = cls(
             dataset=json.loads(FileIODriver.load(path, mode="r")),
             shuffle=shuffle,
             seed=seed,
             tokenizer=tokenizer,
         )
         return dataset
 
     @classmethod
     def from_processed(cls, path: str, shuffle: bool = False, seed: int = 1024):
         dataset = cls(dataset=_ShardContainer(path), shuffle=shuffle, seed=seed)
         return dataset
 
-    def save_propressed(self, path: str, shard_size: int = 4):
+    def save_processed(self, path: str, shard_size: int = 4):
         shard = io.BytesIO()
         shard_idx = 0
         meta = np.empty((0, 2), int)
         for i in self.indices:
             data = {"tokens": self[i]["input_ids"]}
             data.update(
                 {key: value for key, value in self[i].items() if key != "input_ids"}
@@ -273,14 +279,89 @@
                 shard_idx += 1
 
 
 class CollieDatasetForPerplexity(CollieDatasetForTraining):
     ...
 
 
+class CollieDatasetForTemplatedMultiTurnChat(CollieDatasetForTraining):
+    """**CoLLie** 中的多轮对话数据集，会根据模板进行处理
+    :param dataset: 提供的多轮对话数据，形如：
+
+    .. code-block::
+
+            [
+                {
+                    "history": [
+                        {
+                            "role": "user",
+                            "content": "这是用户的问题"
+                        },
+                        {
+                            "role": "assistant",
+                            "content": "这是助手的回答"
+                        },
+                        ...
+                    ]
+                },
+                ...
+            ]
+
+    :tokenizer: 用于处理数据的 tokenizer
+    :shuffle: 是否打乱数据
+    :seed: 随机种子
+    :max_length: 每条数据最大长度
+    :template_fn: 模板函数，为多轮对话数据添加模板
+    :add_generation_prompt: 是否添加用于生成的 prompt，训练时不需要
+    :text_field: 对话数据中文本字段的名称，默认为 `history`
+    """
+    def __init__(
+            self,
+            dataset: Sequence[Dict],
+            tokenizer: Optional[PreTrainedTokenizer],
+            shuffle: bool = False,
+            seed: int = 1024,
+            max_length: int = -1,
+            template_fn: Optional[Callable] = None,
+            add_generation_prompt: bool = False,
+            text_field: str = "history",
+    ):
+        super().__init__(
+            dataset=dataset,
+            tokenizer=tokenizer,
+            shuffle=shuffle,
+            seed=seed,
+            max_length=max_length,
+        )
+        self.template_fn = template_fn
+        self.add_generation_prompt = add_generation_prompt
+        self.text_field = text_field
+
+    def __getitem__(self, index) -> Dict:
+        if index > len(self):
+            raise IndexError("Index out of range in dataset.")
+
+        input_ids, labels, attention_mask = tokenize_conversation(
+            self.dataset[index],
+            self.tokenizer,
+            text_field=self.text_field,
+            prepare_template_fn=self.template_fn,
+            add_generation_prompt=self.add_generation_prompt,
+        )
+        if self.max_length > 0:
+            input_ids = input_ids[: self.max_length]
+            attention_mask = attention_mask[: self.max_length]
+            labels = labels[: self.max_length]
+        return {
+            "input_ids": input_ids,
+            "attention_mask": attention_mask,
+            "labels": labels,
+        }
+
+
 class CollieDatasetForGeneration(CollieDatasetForTraining):
     """**CoLLie** 中的生成数据集，主要用于数据生成或者与生成相关的检验
     须搭配 :class:`~collie.controller.evaluator.EvaluatorForGeneration` 使用。需提供的数据格式形似:
 
         .. code-block::
 
             [
@@ -298,24 +379,24 @@
         target = None
         index = self.indices[index]
         if self.tokenizer is None:
             input_ids = self.dataset[index]["tokens"]
             if "attention_mask" in self.dataset[index].keys():
                 attention_mask = self.dataset[index]["attention_mask"]
             else:
-                attention_mask = torch.ones_like(torch.tensor(input_ids).cpu().tolist())
+                attention_mask = [1 for _ in range(len(input_ids))]
             target = self.dataset[index].get("target", None)
         else:
             inputs = self.tokenizer(
                 self.dataset[index]["text"], add_special_tokens=self.add_special_tokens
             )
             input_ids = inputs["input_ids"]
             attention_mask = inputs.get(
                 "attention_mask",
-                torch.ones_like(torch.tensor(input_ids)).cpu().tolist(),
+                [1 for _ in range(len(input_ids))],
             )
             if "target" in self.dataset[index].keys():
                 if isinstance(self.dataset[index]["target"], str):
                     target = [self.tokenizer(self.dataset[index]["target"]).input_ids]
                 elif isinstance(self.dataset[index]["target"], (list, tuple, set)):
                     target = [
                         self.tokenizer(x).input_ids
@@ -347,22 +428,22 @@
                     "target": 0
                 },
                 ...
             ]
     """
 
     def __init__(
-        self,
-        dataset: Sequence[Dict],
-        tokenizer: Optional[PreTrainedTokenizer] = None,
-        add_special_tokens: bool = True,
-        shuffle: bool = False,
-        seed: int = 1024,
-        max_length: int = -1,
-        style: str = "harness",
+            self,
+            dataset: Sequence[Dict],
+            tokenizer: Optional[PreTrainedTokenizer] = None,
+            add_special_tokens: bool = True,
+            shuffle: bool = False,
+            seed: int = 1024,
+            max_length: int = -1,
+            style: str = "harness",
     ):
         super().__init__(
             dataset=dataset,
             tokenizer=tokenizer,
             add_special_tokens=add_special_tokens,
             shuffle=shuffle,
             seed=seed,
@@ -380,17 +461,17 @@
         index = self.indices[index]
         if self.tokenizer is None:
             input_ids = tuple(self.dataset[index]["tokens"])
             target = self.dataset[index]["target"]
         else:
             if self.style == "harness":
                 if (
-                    "input" in self.dataset[0].keys()
-                    and "output" in self.dataset[0].keys()
-                    and "target" in self.dataset[0].keys()
+                        "input" in self.dataset[0].keys()
+                        and "output" in self.dataset[0].keys()
+                        and "target" in self.dataset[0].keys()
                 ):
                     input_ids = []
                     attention_mask = []
                     labels = []
                     for output in self.dataset[index]["output"]:
                         inputs = self.tokenizer(
                             self.dataset[index]["input"] + output,
@@ -434,26 +515,26 @@
                     "input_ids": input_ids,
                     "attention_mask": attention_mask,
                     "labels": labels,
                     "target": target,
                 }
             elif self.style == "helm":
                 if (
-                    "input" in self.dataset[0].keys()
-                    and "output" in self.dataset[0].keys()
-                    and "target" in self.dataset[0].keys()
+                        "input" in self.dataset[0].keys()
+                        and "output" in self.dataset[0].keys()
+                        and "target" in self.dataset[0].keys()
                 ):
                     inputs = self.tokenizer(
                         self.dataset[index]["input"],
                         add_special_tokens=self.add_special_tokens,
                     )
                     input_ids = inputs["input_ids"]
                     attention_mask = inputs.get(
                         "attention_mask",
-                        torch.ones_like(torch.tensor(input_ids)).cpu().tolist(),
+                        [1 for _ in range(len(input_ids))],
                     )
                     output = tuple([option for option in self.dataset[index]["output"]])
                     target = self.dataset[index]["target"]
                 else:
                     raise ValueError(
                         "CollieDatasetForClassification must have three fields (`input`, `output` and `target`)."
                     )
```

### Comparing `collie-lm-1.0.6/collie/driver/io/base.py` & `collie_lm-1.0.7/collie/driver/io/base.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/driver/io/file.py` & `collie_lm-1.0.7/collie/driver/io/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from collie.driver.io.base import IODriver
 
 import os
 import io
 import torch
+from safetensors.torch import load_file
 import shutil
 
 class FileIODriver(IODriver):
     @staticmethod
     def load(path: str, mode: str):
         assert os.path.exists(path), f"File {path} does not exist."
         if 'b' in mode.lower():
-            return torch.load(path, map_location=torch.device('cpu'))
+            if path.endswith(".safetensors"):
+                return load_file(path, device='cpu')
+            else:
+                return torch.load(path, map_location=torch.device('cpu'))
         else:
             with open(path, 'r') as f:
                 return f.read()
 
     @staticmethod
     def load_buffer(path: str):
         assert os.path.exists(path), f"File {path} does not exist."
```

### Comparing `collie-lm-1.0.6/collie/driver/io/petrel.py` & `collie_lm-1.0.7/collie/driver/io/petrel.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/log/handler.py` & `collie_lm-1.0.7/collie/log/handler.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/log/logger.py` & `collie_lm-1.0.7/collie/log/logger.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/log/print.py` & `collie_lm-1.0.7/collie/log/print.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/metrics/accuracy.py` & `collie_lm-1.0.7/collie/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/metrics/base.py` & `collie_lm-1.0.7/collie/metrics/base.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/metrics/bleu.py` & `collie_lm-1.0.7/collie/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/metrics/classify_f1_pre_rec_metric.py` & `collie_lm-1.0.7/collie/metrics/classify_f1_pre_rec_metric.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/metrics/decode.py` & `collie_lm-1.0.7/collie/metrics/decode.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/metrics/ppl.py` & `collie_lm-1.0.7/collie/metrics/ppl.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/metrics/rouge.py` & `collie_lm-1.0.7/collie/metrics/rouge.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/models/base.py` & `collie_lm-1.0.7/collie/models/base.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/models/chatglm/model.py` & `collie_lm-1.0.7/collie/models/chatglm/model.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/models/chatglm2/model.py` & `collie_lm-1.0.7/collie/models/chatglm2/model.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/models/internlm/model.py` & `collie_lm-1.0.7/collie/models/internlm/model.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/models/internlm2/configuration_internlm2.py` & `collie_lm-1.0.7/collie/models/internlm2/configuration_internlm2.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/models/internlm2/model.py` & `collie_lm-1.0.7/collie/models/internlm2/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1395,19 +1395,27 @@
                         weights.append(weight_map["model.tok_embeddings.weight"])
                     if max(parts) - 1 in layers:
                         weights.append(weight_map["output.weight"])
                     if max(parts) - 2 in layers:
                         weights.append(weight_map["model.norm.weight"])
                 else:
                     # 如果没有 pytorch_model.bin.index.json 文件的话，那么就加载所有的权重
+                    # 优先加载 safetensors 存储的权重
                     weights = [
                         weight
                         for weight in io_driver.list(path)
-                        if weight.endswith(".bin")
+                        if weight.endswith(".safetensors")
                     ]
+                    if len(weights) == 0:
+                        # 如果没有 safetensors 文件，那么就加载 bin 文件
+                        weights = [
+                            weight
+                            for weight in io_driver.list(path)
+                            if weight.endswith(".bin")
+                        ]
                 with progress(
                     weights,
                     desc="Loading state dict",
                     total=len(weights),
                     disable=hide_progress,
                 ) as pbar:
                     for weight in pbar:
```

### Comparing `collie-lm-1.0.6/collie/models/llama/model.py` & `collie_lm-1.0.7/collie/models/llama/model.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/models/moss/model.py` & `collie_lm-1.0.7/collie/models/moss/model.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/models/moss_moon/model.py` & `collie_lm-1.0.7/collie/models/moss_moon/model.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/models/moss_moon/utils.py` & `collie_lm-1.0.7/collie/models/moss_moon/utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/models/utils.py` & `collie_lm-1.0.7/collie/models/utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/module.py` & `collie_lm-1.0.7/collie/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -513,14 +513,15 @@
 
         self.tied_comms = self._index_tied_modules()
         self._synchronize_tied_weights()
 
         self.activation_checkpoint_interval = activation_checkpoint_interval
         self.activation_checkpoint_func = activation_checkpoint_func
 
+        self.parts = [int(x) for x in self.parts]  # deepspeed版本问题，新版会使用numpy，这边要转成int才能json.dump
         os.environ["COLLIE_PP_PARTS"] = json.dumps(self.parts)
         os.environ["COLLIE_PP_RANK"] = str(self.stage_id)
         os.environ["COLLIE_DP_RANK"] = str(self._grid.data_parallel_id)
         
         PipelineGenerationMixin.__init__(self)
         
         self.inner_forward = False
```

### Comparing `collie-lm-1.0.6/collie/optim/adalomo.py` & `collie_lm-1.0.7/collie/optim/adalomo.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,19 +75,26 @@
 
         self.exp_avg_sq = {}
         self.exp_avg_sq_row = {}
         self.exp_avg_sq_col = {}
 
         # register hook function, which will be called through the backward process
         for n, p in self.model.named_parameters():
-            if len(p.ds_shape) == 1:
-                self.exp_avg_sq[n] = torch.zeros(p.ds_shape[0], dtype=torch.float32).cuda()
+            if self.zero3_enabled:
+                if len(p.ds_shape) == 1:
+                    self.exp_avg_sq[n] = torch.zeros(p.ds_shape[0], dtype=torch.float32).cuda()
+                else:
+                    self.exp_avg_sq_row[n] = torch.zeros(p.ds_shape[0], dtype=torch.float32).cuda()
+                    self.exp_avg_sq_col[n] = torch.zeros(p.ds_shape[1], dtype=torch.float32).cuda()
             else:
-                self.exp_avg_sq_row[n] = torch.zeros(p.ds_shape[0], dtype=torch.float32).cuda()
-                self.exp_avg_sq_col[n] = torch.zeros(p.ds_shape[1], dtype=torch.float32).cuda()
+                if len(p.data.shape) == 1:
+                    self.exp_avg_sq[n] = torch.zeros(p.data.shape[0], dtype=torch.float32).cuda()
+                else:
+                    self.exp_avg_sq_row[n] = torch.zeros(p.data.shape[0], dtype=torch.float32).cuda()
+                    self.exp_avg_sq_col[n] = torch.zeros(p.data.shape[1], dtype=torch.float32).cuda()
 
             if p.requires_grad:
                 p.register_hook(self.grad_func)
         defaults = dict(
             lr=lr,
             eps=eps,
             weight_decay=weight_decay,
```

### Comparing `collie-lm-1.0.6/collie/optim/adan.py` & `collie_lm-1.0.7/collie/optim/adan.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/optim/lion.py` & `collie_lm-1.0.7/collie/optim/lion.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/optim/lomo.py` & `collie_lm-1.0.7/collie/optim/lomo.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/optim/sophiag.py` & `collie_lm-1.0.7/collie/optim/sophiag.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/utils/__init__.py` & `collie_lm-1.0.7/collie/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/utils/data_provider.py` & `collie_lm-1.0.7/collie/utils/data_provider.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/utils/dist_utils.py` & `collie_lm-1.0.7/collie/utils/dist_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,15 @@
     """
     if torch.distributed.is_initialized():
         return
     if isinstance(config, str):
         config = load_config(config)
     if isinstance(config.ds_config, str):
         config.ds_config = load_config(config.ds_config)
+    config.valid_config()
     patch_bitesandbytes(config)
     patch_transformers(config)
     patch_deepspeed(config)
     patch_megatron()
     patch_peft(config)
     if "WORLD_SIZE" in os.environ.keys():
         # launch from pytorch
```

### Comparing `collie-lm-1.0.6/collie/utils/metric_wrapper.py` & `collie_lm-1.0.7/collie/utils/metric_wrapper.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/utils/monitor.py` & `collie_lm-1.0.7/collie/utils/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             config.ds_config["monitor_config"]["wandb"] = {"enabled": False}
         else:
             config.ds_config["monitor_config"]["wandb"]["job_name"] = tag
             config.ds_config["monitor_config"]["wandb"]["config"] = config
         if "csv_monitor" not in config.ds_config["monitor_config"].keys():
             config.ds_config["monitor_config"]["csv_monitor"] = {"enabled": False}
         else:
-            config.ds_config["monitor_config"]["csv_monitor"]["job_name"] = tag + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
+            config.ds_config["monitor_config"]["csv_monitor"]["job_name"] = tag + datetime.datetime.now().strftime("-%Y-%m-%d-%H-%M-%S")
         monitor = MonitorMaster(dictToObj(config.ds_config["monitor_config"]))
         config.ds_config["monitor_config"]["wandb"].pop("config", {})
         return monitor
     else:
         return DummyDeepSpeedMonitor(config.ds_config)
     
 class BaseMonitor:
@@ -215,18 +215,18 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         if 'loss' in self.item.keys() and self.item["mode"] == "train":
             self.monitor.write_events([(f"Learning Rate", self.item['lr'], self.item['global_batch_idx'])])  
         
 class _MultiMonitors:
     def __init__(self, monitors: Sequence[BaseMonitor]) -> None:
         self.monitors = monitors
-        self.item = {}
+        self.item = {"mode": "init"}
     
     def __enter__(self):
         for monitor in self.monitors:
             monitor.__enter__()
         return self.item
     
     def __exit__(self, exc_type, exc_val, exc_tb):
         for monitor in self.monitors:
             monitor.item = self.item
-            monitor.__exit__(exc_type, exc_val, exc_tb)
+            monitor.__exit__(exc_type, exc_val, exc_tb)
```

### Comparing `collie-lm-1.0.6/collie/utils/padder.py` & `collie_lm-1.0.7/collie/utils/padder.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/utils/peft_utils.py` & `collie_lm-1.0.7/collie/utils/peft_utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/utils/pipeline_engine.py` & `collie_lm-1.0.7/collie/utils/pipeline_engine.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,190 +1,35 @@
 import torch
-from torch import nn
 import torch.distributed as dist
+from deepspeed.runtime.activation_checkpointing import checkpointing as ds_checkpointing
+from deepspeed.runtime.pipe import PipelineModule, p2p, schedule
 from deepspeed.runtime.pipe.engine import PipelineEngine, _tensor_bytes
-from deepspeed.runtime.pipe import schedule, p2p, PipelineModule
 from deepspeed.runtime.utils import PartitionedTensor
-from deepspeed.runtime.activation_checkpointing import checkpointing as ds_checkpointing
-from deepspeed.runtime.engine import DeepSpeedEngine
-from deepspeed.utils.timer import ThroughputTimer
 from deepspeed.utils import logger
 from peft import PeftModel
+from torch import nn
 
-from .utils import _split_batch, auto_param_call, _split_past_key_values
-from .dist_utils import broadcast_tensor, env
 from ..module import PipelineModel
+from .dist_utils import broadcast_tensor, env
+from .utils import _split_batch, _split_past_key_values, auto_param_call
 
-def is_even(number):
-    return number % 2 == 0
 
 class ColliePipelineEngine(PipelineEngine):
     def __init__(self, has_bool_tensors=False, *args, **kwargs):
-        DeepSpeedEngine.__init__(self, *args, **kwargs)
+        super().__init__(has_bool_tensors, *args, **kwargs)
+        # 注册一些collie里需要用到的属性，deepspeed里没有
         if isinstance(self.module, PipelineModel):
             pipeline_module = self.module
         elif isinstance(self.module, PeftModel) and isinstance(self.module.get_base_model(), PipelineModel):
             pipeline_module = self.module.get_base_model()
         else:
             raise TypeError("Model must base PipelineModule.")
         # 防止被加入到 Module 的 _modules 里访问不到
         object.__setattr__(self, "pipeline_module", pipeline_module)
 
-        assert self.zero_optimization_stage() < 2, "ZeRO-2 and ZeRO-3 are incompatible with pipeline parallelism"
-
-        # We schedule the all-reduces, so disable it in super().backward()
-        self.enable_backward_allreduce = False
-        self.has_bool_tensors = has_bool_tensors
-        self.eval_return_logits = False
-        self.outputs = None
-
-        # used to disable the pipeline all-reduce when used with 1-bit Adam/1-bit LAMB
-        self.pipeline_enable_backward_allreduce = True
-
-        if self.elasticity_enabled():
-            if not self.is_elastic_model_parallel_supported():
-                assert not self.elasticity_enabled(), "Elasticity is not currently supported" \
-                " with pipeline parallelism."
-
-        # pipeline step for logging
-        self.log_batch_step_id = -1
-
-        self.micro_batch_size = self.train_micro_batch_size_per_gpu()
-        self.micro_batches = self.gradient_accumulation_steps()
-
-        # Set Grid and Communication Groups
-        self.grid = self.module._grid
-        if self.grid.get_global_rank() == 0:
-            logger.info(f'CONFIG: micro_batches={self.micro_batches} '
-                        f'micro_batch_size={self.micro_batch_size}')
-
-        self.global_rank = self.grid.get_global_rank()
-
-        assert self.dp_world_size == self.grid.data_parallel_size
-        assert self.train_batch_size() == \
-            self.micro_batch_size * self.micro_batches * self.grid.data_parallel_size
-
-        #  Set Stage Inf
-        self.num_stages = self.grid.pipe_parallel_size
-        self.stage_id = self.grid.get_stage_id()
-        self.prev_stage = self.stage_id - 1
-        self.next_stage = self.stage_id + 1
-
-        self.data_iterator = None
-        self.batch_fn = None
-
-        self._force_grad_boundary = False
-
-        self.batch_timer = ThroughputTimer(batch_size=self.train_batch_size(),
-                                           logging_fn=self.tput_log,
-                                           monitor_memory=False,
-                                           steps_per_output=self.steps_per_print())
-
-        # PipelineEngine needs to handle data loading specially due to only the first
-        # and last stages loading inputs/labels. We construct a sampler that uses
-        if self.training_data:
-            self._build_data_iter(self.training_data)
-
-        self.is_pipe_parallel = self.grid.pipe_parallel_size > 1
-        self.is_data_parallel = self.grid.data_parallel_size > 1
-        self.is_model_parallel = self.grid.model_parallel_size > 1
-
-        # Partition input/output buffers
-        # XXX temporarily disable while I revert some partition hacks.
-        self.is_pipe_partitioned = self.is_model_parallel
-        self.is_grad_partitioned = self.is_model_parallel
-
-        model_parameters = filter(lambda p: p.requires_grad, self.module.parameters())
-        num_params = sum([p.numel() for p in model_parameters])
-        unique_params = num_params
-        # Subtract tied parameters if we don't own them
-        if self.module.tied_comms:
-            tied_params = 0
-            for key, d in self.module.tied_comms.items():
-                if self.global_rank != min(d['ranks']):
-                    tied_params += sum(p.numel() for p in d['module'].parameters())
-            unique_params -= tied_params
-        params_tensor = torch.LongTensor(data=[num_params, unique_params]).to(self.device)
-        dist.all_reduce(params_tensor, group=self.grid.get_model_parallel_group())
-        params_tensor = params_tensor.tolist()
-        total_params = params_tensor[0]
-        unique_params = params_tensor[1]
-        if self.grid.data_parallel_id == 0:
-            logger.info(f'RANK={self.global_rank} '
-                        f'STAGE={self.stage_id} '
-                        f'LAYERS={self.module._local_stop - self.module._local_start} '
-                        f'[{self.module._local_start}, {self.module._local_stop}) '
-                        f'STAGE_PARAMS={num_params} ({num_params/1e6:0.3f}M) '
-                        f'TOTAL_PARAMS={total_params} ({total_params/1e6:0.3f}M) '
-                        f'UNIQUE_PARAMS={unique_params} ({unique_params/1e6:0.3f}M)')
-
-        #initialize peer-2-peer communication and allreduce groups
-        if self.is_pipe_parallel:
-            p2p.init_process_groups(self.grid)
-
-        # Pipeline buffers
-        self.num_pipe_buffers = 0
-        self.pipe_buffers = {
-            'inputs': [],  # batch input and received activations
-            'labels': [],  # labels from batch input
-            'outputs': [],  # activations
-            'output_tensors': [],  # tensor object to preserve backward graph
-        }
-        self.pipe_recv_buf = None
-        self.grad_layer = None
-
-        self.meta_buffer = None
-
-        self.first_output_send = True
-        self.first_gradient_send = True
-
-        #stores the loss for the current micro batch being processed
-        self.loss = torch.tensor(0.0).to(self.device)
-
-        #stores the loss for the entire batch
-        self.total_loss = None
-        self.agg_loss = torch.tensor(0.0, requires_grad=False).to(self.device)
-        self.dp_group_loss = torch.tensor(0.0, requires_grad=False).to(self.device)
-
-        if self._config.pipeline['activation_checkpoint_interval'] > 0:
-            self.module.activation_checkpoint_interval = self._config.pipeline['activation_checkpoint_interval']
-
-        self.module.checkpoint_parallel_write_pipeline = self._config.checkpoint_parallel_write_pipeline
-
-        if self.is_last_stage():
-            self.loss_model = self.module.loss_fn
-
-        self.has_attention_mask = self.module.__class__.__name__ == 'GPT2ModelPipe'
-        # Initialize pipeline communicators. Just send a 0.
-        if is_even(self.stage_id):
-            if not self.is_last_stage():
-                p2p.send(self.loss, self.next_stage)
-            if not self.is_first_stage():
-                p2p.recv(self.loss, self.prev_stage)
-        else:
-            if not self.is_first_stage():
-                p2p.recv(self.loss, self.prev_stage)
-            if not self.is_last_stage():
-                p2p.send(self.loss, self.next_stage)
-
-        # XXX look into timer reporting timing
-        # Initialize some timers because of early weirdness.
-        if self.wall_clock_breakdown():
-            self.timers('forward_microstep').start()
-            self.timers('forward_microstep').stop()
-            self.timers('backward_microstep').start()
-            self.timers('backward_microstep').stop()
-            self.timers('backward_inner_microstep').start()
-            self.timers('backward_inner_microstep').stop()
-            self.timers('backward_allreduce_microstep').start()
-            self.timers('backward_allreduce_microstep').stop()
-            self.timers('backward_allreduce').start()
-            self.timers('backward_allreduce').stop()
-            self.timers('step_microstep').start()
-            self.timers('step_microstep').stop()
         self.buffer_shape = None
         self.inputs_extra = {}
         self.outputs_extra = {}
 
     def reset_buffer_shape(self, batch):
         if self.buffer_shape is None:
             self.buffer_shape = {}
@@ -220,15 +65,15 @@
         batch = _split_batch(batch, self.train_micro_batch_size_per_gpu(),
                              self.gradient_accumulation_steps())
         data_iter = iter(batch)
         result = super().train_batch(data_iter)
 
         self.pipeline_module.inner_forward = False
         return result
-    
+
     def eval_batch(self, batch):
         self.pipeline_module.inner_forward = True
         self.pipeline_module.forward_type = "eval"
 
         self.reset_buffer_shape(batch)
         if self.total_loss is not None:
             total_loss = self.total_loss.detach().clone()
@@ -245,15 +90,15 @@
         # len(logits) = micro_batch_nums
         # Assume batch first
         logits = self.broadcast_logits(logits)
         self.total_loss = total_loss
 
         self.pipeline_module.inner_forward = False
         return logits
-    
+
     def generate_batch(self, batch):
         self.pipeline_module.inner_forward = True
         self.pipeline_module.forward_type = "generate"
 
         self.reset_buffer_shape(batch)
 
         if self.total_loss is not None:
@@ -307,26 +152,26 @@
         if self.is_last_stage():
             logits = self._reduce_outputs(self.fwd_outputs, reduce=None)
 
         # Restore the training iterator
         self.set_dataiterator(train_iterator)
 
         # Reset any buffers that may have been populated during the forward passes.
-        #ds_checkpointing.reset()
+        # ds_checkpointing.reset()
         self.eval_return_logits = False
-        
+
         # logits: list
         # len(logits) = micro_batch_nums
         # Assume batch first
         logits = self.broadcast_logits(logits)
         self.total_loss = total_loss
 
         self.pipeline_module.inner_forward = False
         return logits
-    
+
     def broadcast_logits(self, logits):
         src_rank = self.grid.stage_to_global(self.num_stages - 1)
         if logits is not None:
             assert isinstance(logits, list), type(logits)
             assert isinstance(logits[0], dict), type(logits[0])
             _logits = {}
             for key in logits[0].keys():
@@ -383,15 +228,15 @@
                 meta=self.inputs_extra["_meta"],
                 local_part=self.inputs_extra["_local_data"],
                 group=self.grid.get_slice_parallel_group()
             )
             inputs[self.inputs_extra["_grad_key"]] = part_input.full()
             inputs[self.inputs_extra["_grad_key"]].requires_grad = True
             # skip mask
-            #inputs[1].requires_grad = True
+            # inputs[1].requires_grad = True
             part_input = None
             if isinstance(inputs, dict):
                 self.pipe_buffers['inputs'][buffer_id] = {k:v for k, v in inputs.items()}
             else:
                 self.pipe_buffers['inputs'][buffer_id] = inputs
 
         # Zero out the gradients each time we use the tensor because only the data in
@@ -408,16 +253,16 @@
         if self.module.training:
             _grad_key = None
             for key, value in outputs.items():
                 if value.requires_grad:
                     assert _grad_key is None, "More than one tensors requires grad."
                     if self.is_pipe_partitioned and not self.is_last_stage():
                         part = PartitionedTensor(tensor=value, group=self.grid.get_slice_parallel_group())
-                    # Clear the large output data, but save the computation graph
-                    # TODO 这里源代码没有.to，但现在必须加.to否则会无法send
+                        # Clear the large output data, but save the computation graph
+                        # TODO 这里源代码没有.to，但现在必须加.to否则会无法send
                         value.data = torch.zeros(1).to(self.device)
                         self.pipe_buffers['output_tensors'][buffer_id] = value
                         self.outputs_extra["_meta"] = part.to_meta()
                         self.outputs_extra["_local_data"] = part.data()
                     _grad_key = key
             assert _grad_key is not None, "None of the outputs has grad!"
             self.outputs_extra["_grad_key"] = _grad_key
@@ -450,15 +295,15 @@
                 self.fwd_outputs.append(self.loss.detach())
 
                 if self.total_loss is None:
                     self.total_loss = torch.zeros_like(self.loss)
                 self.total_loss += self.loss.detach()
             elif isinstance(self.loss, dict):
                 self.fwd_outputs.append({k:v.detach() for k, v in self.loss.items()})
-                
+
                 if self.total_loss is None:
                     self.total_loss = {k:torch.zeros_like(l) for k, l in self.loss.items()}
                 for k, l in self.loss.items():
                     self.total_loss[k] += l.detach()
             else:
                 self.fwd_outputs.append([l.detach() for l in self.loss])
 
@@ -539,15 +384,15 @@
             self.timers('backward_microstep').stop()
 
         self.mem_status('AFTER BWD')
 
     def _exec_load_micro_batch(self, buffer_id):
         if self.wall_clock_breakdown():
             self.timers('batch_input').start()
-            
+
         batch = self._next_batch() # {"input_ids": torch.Tensor, "labels": torch.Tensor}
         # batch = self._next_batch() # (inputs, labels)
 
         # if self.is_first_stage():
         #     loaded = {}
         #     for key, tensor in batch[0].items():
         #         assert torch.is_tensor(tensor)
@@ -567,15 +412,15 @@
         #         for key, tensor in batch[1].items():
         #             assert torch.is_tensor(tensor)
         #             tensor = tensor.to(self.device).detach()
         #             loaded[key] = tensor
         #     else:
         #         raise NotImplementedError
         #     self.pipe_buffers['labels'][buffer_id] = loaded
-        
+
         if self.is_first_stage() or self.is_last_stage():
             loaded = {}
             for key, tensor in batch.items():
                 assert torch.is_tensor(tensor)
                 mine = tensor.clone().detach().to(self.device)
                 mine.requires_grad = mine.is_floating_point()
                 loaded[key] = mine
@@ -660,15 +505,15 @@
                 recv_shapes_and_dtypes.append((recv_shape.tolist(), recv_dtype))
 
             buffers = self._allocate_buffers(recv_shapes_and_dtypes, num_buffers=1)[0]
             # Convert to tuples if requested.
             if recv_type == 2:
                 buffers = tuple(buffers)
             return buffers
-        
+
         elif recv_type == 3:
             # dict
             count_tensor = torch.LongTensor(data=[0]).to(self.device)
             p2p.recv(count_tensor, send_stage)
             num_tensors = count_tensor.item()
             recv_dict = {}
             for idx in range(num_tensors):
@@ -743,15 +588,15 @@
 
     def _exec_send_grads(self, buffer_id):
         if self.wall_clock_breakdown():
             self.timers('pipe_send_grad').start()
         inputs = self.pipe_buffers['inputs'][buffer_id]
 
         # Partition the gradient
-        
+
         if self.is_grad_partitioned:
             part = None
             _grad_key = None
             for key, value in inputs.items():
                 if value.grad is not None:
                     # TODO 在 collie 里我们暂时限定 dict 里只有一个 tensor 是有梯度的
                     assert part is None, "More than one tensors have grad."
@@ -837,15 +682,15 @@
 
             # NCCL does not like to send torch.BoolTensor types, so un-cast the
             # attention mask
             # TODO 如何处理
             # if self.has_attention_mask or self.has_bool_tensors:
             #     recvd[-1] = recvd[-1].bool()
             for key, buffer in recvd.items():
-                    buffer.requires_grad = self.module.training and \
+                buffer.requires_grad = self.module.training and \
                         (key == self.inputs_extra["_grad_key"])
         if isinstance(recvd, dict):
             self.pipe_buffers['inputs'][buffer_id] = {k:v for k, v in recvd.items()}
         else:
             self.pipe_buffers['inputs'][buffer_id] = recvd
 
         if self.wall_clock_breakdown():
@@ -901,15 +746,15 @@
             self.timers('pipe_recv_grad').stop()
 
     def _exec_optimizer_step(self, lr_kwargs=None):
         return super()._exec_optimizer_step(lr_kwargs)
 
     def _exec_reduce_grads(self):
         return super()._exec_reduce_grads()
-    
+
     def _exec_reduce_tied_grads(self):
         return super()._exec_reduce_tied_grads()
 
     _INSTRUCTION_MAP = {
         schedule.OptimizerStep: _exec_optimizer_step,
         schedule.ReduceGrads: _exec_reduce_grads,
         schedule.ReduceTiedGrads: _exec_reduce_tied_grads,
@@ -966,25 +811,25 @@
         else:
             scaled_loss = prescaled_loss
             if self.warn_unscaled_loss:
                 logger.warning(f"DeepSpeed unable to scale loss because of type: {type(prescaled_loss)}")
                 self.warn_unscaled_loss = False
 
         return scaled_loss
-    
+
     def _reduce_outputs(self, outputs, reduce='avg', reduce_dp=True):
         if reduce is None:
             return outputs
 
         if reduce.lower() == 'avg':
             # first sum over all microbatches
             if torch.is_tensor(outputs[0]):
                 reduced = sum(outputs)
             elif isinstance(outputs[0], dict):
-                # list of dict 
+                # list of dict
                 reduced = {k:torch.zeros_like[o] for k, o in outputs[0].items()}
                 for idx, out in enumerate(outputs):
                     for key, o in out.items():
                         reduced[key] += o
             else:
                 # TODO 这里是源代码。是不是不太对？
                 assert isinstance(outputs, (list, tuple))
```

### Comparing `collie-lm-1.0.6/collie/utils/rich_progress.py` & `collie_lm-1.0.7/collie/utils/rich_progress.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/utils/seq_len_to_mask.py` & `collie_lm-1.0.7/collie/utils/seq_len_to_mask.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie/utils/utils.py` & `collie_lm-1.0.7/collie/utils/utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie_cli/bullet/charDef.py` & `collie_lm-1.0.7/collie_cli/bullet/charDef.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie_cli/bullet/client.py` & `collie_lm-1.0.7/collie_cli/bullet/client.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie_cli/bullet/colors.py` & `collie_lm-1.0.7/collie_cli/bullet/colors.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie_cli/bullet/cursor.py` & `collie_lm-1.0.7/collie_cli/bullet/cursor.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie_cli/bullet/keyhandler.py` & `collie_lm-1.0.7/collie_cli/bullet/keyhandler.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie_cli/bullet/styles.py` & `collie_lm-1.0.7/collie_cli/bullet/styles.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie_cli/bullet/utils.py` & `collie_lm-1.0.7/collie_cli/bullet/utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie_cli/collie_cli.py` & `collie_lm-1.0.7/collie_cli/collie_cli.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie_cli/config.py` & `collie_lm-1.0.7/collie_cli/config.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie_cli/run.py` & `collie_lm-1.0.7/collie_cli/run.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/collie_lm.egg-info/PKG-INFO` & `collie_lm-1.0.7/collie_lm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collie-lm
-Version: 1.0.6
+Version: 1.0.7
 Summary: CoLLiE: Collaborative Training of Large Language Models in an Efficient Way
 Author: OpenLMLab
 Author-email: yanhang@pjlab.org.cn
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: deepspeed>=0.10.0
 Requires-Dist: tqdm
@@ -22,7 +22,8 @@
 Requires-Dist: wandb
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: accelerate>=0.20.3
 Requires-Dist: bitsandbytes>=0.41.0
 Requires-Dist: scipy
 Requires-Dist: rich>=13.3.5
+Requires-Dist: safetensors
```

### Comparing `collie-lm-1.0.6/collie_lm.egg-info/SOURCES.txt` & `collie_lm-1.0.7/collie_lm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 collie/controller/server.py
 collie/controller/trainer.py
 collie/controller/utils.py
 collie/data/__init__.py
 collie/data/batch_sampler.py
 collie/data/dataloader.py
 collie/data/dataset.py
+collie/data/template_utils.py
 collie/driver/__init__.py
 collie/driver/io/__init__.py
 collie/driver/io/base.py
 collie/driver/io/file.py
 collie/driver/io/petrel.py
 collie/log/__init__.py
 collie/log/handler.py
@@ -101,8 +102,9 @@
 tests/callbacks/test_callbacks.py
 tests/helpers/__init__.py
 tests/helpers/utils.py
 tests/trainer/__init__.py
 tests/trainer/_test_checkpoint_zero.py
 tests/trainer/_test_trainer_metric.py
 tests/trainer/_test_trainer_metric_evaluator.py
-tests/trainer/test_trainer_checkpoint.py
+tests/trainer/test_trainer_checkpoint.py
+tests/trainer/test_trainer_peft_save.py
```

### Comparing `collie-lm-1.0.6/setup.py` & `collie_lm-1.0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("requirements.txt", encoding="utf-8") as f:
     reqs = f.read()
 
 setup(
     name="collie-lm",
-    version="1.0.6",
+    version="1.0.7",
     description="CoLLiE: Collaborative Training of Large Language Models in an Efficient Way",
     author="OpenLMLab",
     author_email="yanhang@pjlab.org.cn",
     packages=find_packages(),
     install_requires=reqs.splitlines(),
     python_requires=">=3.8",
     entry_points={
```

### Comparing `collie-lm-1.0.6/tests/callbacks/_test_checkpoint_callback.py` & `collie_lm-1.0.7/tests/callbacks/_test_checkpoint_callback.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/tests/callbacks/_test_load_best_callback.py` & `collie_lm-1.0.7/tests/callbacks/_test_load_best_callback.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/tests/callbacks/test_callbacks.py` & `collie_lm-1.0.7/tests/callbacks/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/tests/helpers/utils.py` & `collie_lm-1.0.7/tests/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/tests/trainer/_test_checkpoint_zero.py` & `collie_lm-1.0.7/tests/trainer/_test_checkpoint_zero.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/tests/trainer/_test_trainer_metric.py` & `collie_lm-1.0.7/tests/trainer/_test_trainer_metric.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/tests/trainer/_test_trainer_metric_evaluator.py` & `collie_lm-1.0.7/tests/trainer/_test_trainer_metric_evaluator.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.6/tests/trainer/test_trainer_checkpoint.py` & `collie_lm-1.0.7/tests/trainer/test_trainer_checkpoint.py`

 * *Files identical despite different names*

