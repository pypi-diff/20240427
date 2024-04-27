# Comparing `tmp/DLStudio-2.4.3.tar.gz` & `tmp/DLStudio-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLStudio-2.4.3.tar", last modified: Sat Mar 23 22:01:59 2024, max compression
+gzip compressed data, was "DLStudio-2.4.8.tar", last modified: Sat Apr 27 21:46:25 2024, max compression
```

## Comparing `DLStudio-2.4.3.tar` & `DLStudio-2.4.8.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.131379 DLStudio-2.4.3/
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/AdversarialLearning/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    91504 2024-03-23 16:57:24.000000 DLStudio-2.4.3/AdversarialLearning/AdversarialLearning.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      609 2023-12-06 04:36:12.000000 DLStudio-2.4.3/AdversarialLearning/__init__.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/DLStudio/
--rwxr-xr-x   0 kak       (1000) kak       (1000)   345101 2024-03-23 21:33:31.000000 DLStudio-2.4.3/DLStudio/DLStudio.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      555 2023-12-06 04:36:12.000000 DLStudio-2.4.3/DLStudio/__init__.py
--rw-rw-r--   0 kak       (1000) kak       (1000)   307785 2024-03-23 21:55:56.000000 DLStudio-2.4.3/DLStudio-2.4.3.html
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/DLStudio.egg-info/
--rwxr-xr-x   0 kak       (1000) kak       (1000)     2108 2024-03-23 22:01:59.000000 DLStudio-2.4.3/DLStudio.egg-info/PKG-INFO
--rwxr-xr-x   0 kak       (1000) kak       (1000)     2166 2024-03-23 22:01:59.000000 DLStudio-2.4.3/DLStudio.egg-info/SOURCES.txt
--rwxr-xr-x   0 kak       (1000) kak       (1000)        1 2024-03-23 22:01:59.000000 DLStudio-2.4.3/DLStudio.egg-info/dependency_links.txt
--rwxr-xr-x   0 kak       (1000) kak       (1000)      108 2024-03-23 22:01:59.000000 DLStudio-2.4.3/DLStudio.egg-info/top_level.txt
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/DataPrediction/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    34515 2024-03-23 16:58:20.000000 DLStudio-2.4.3/DataPrediction/DataPrediction.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      584 2023-12-06 04:36:12.000000 DLStudio-2.4.3/DataPrediction/__init__.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/Examples/
--rw-r--r--   0 kak       (1000) kak       (1000)      516 2023-12-06 04:36:23.000000 DLStudio-2.4.3/Examples/README
--rw-r--r--   0 kak       (1000) kak       (1000)     2372 2024-02-17 00:32:47.000000 DLStudio-2.4.3/Examples/custom_data_loading.py
--rw-r--r--   0 kak       (1000) kak       (1000)     4822 2024-02-17 00:35:53.000000 DLStudio-2.4.3/Examples/noisy_object_detection_and_localization.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3518 2024-02-19 18:49:38.000000 DLStudio-2.4.3/Examples/object_detection_and_localization.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3513 2024-03-16 11:10:34.000000 DLStudio-2.4.3/Examples/object_detection_and_localization_iou.py
--rw-r--r--   0 kak       (1000) kak       (1000)     1900 2023-12-06 04:36:23.000000 DLStudio-2.4.3/Examples/playing_with_cifar10.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2179 2023-12-06 04:36:23.000000 DLStudio-2.4.3/Examples/playing_with_reconfig.py
--rw-r--r--   0 kak       (1000) kak       (1000)     1652 2023-12-06 04:36:23.000000 DLStudio-2.4.3/Examples/playing_with_sequential.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2161 2024-02-17 00:29:28.000000 DLStudio-2.4.3/Examples/playing_with_skip_connections.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3067 2024-03-17 20:04:07.000000 DLStudio-2.4.3/Examples/semantic_segmentation.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2939 2023-12-06 04:36:23.000000 DLStudio-2.4.3/Examples/text_classification_with_GRU.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3070 2023-12-06 04:36:23.000000 DLStudio-2.4.3/Examples/text_classification_with_GRU_word2vec.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2770 2023-12-06 04:36:23.000000 DLStudio-2.4.3/Examples/text_classification_with_TEXTnet.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3139 2023-12-06 04:36:23.000000 DLStudio-2.4.3/Examples/text_classification_with_TEXTnetOrder2.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3172 2023-12-06 04:36:23.000000 DLStudio-2.4.3/Examples/text_classification_with_TEXTnetOrder2_word2vec.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3084 2023-12-06 04:36:23.000000 DLStudio-2.4.3/Examples/text_classification_with_TEXTnet_word2vec.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/ExamplesAdversarialLearning/
--rwxr-xr-x   0 kak       (1000) kak       (1000)     3140 2023-12-06 04:36:12.000000 DLStudio-2.4.3/ExamplesAdversarialLearning/README
--rw-r--r--   0 kak       (1000) kak       (1000)     4755 2024-03-23 17:28:17.000000 DLStudio-2.4.3/ExamplesAdversarialLearning/dcgan_DG1.py
--rw-r--r--   0 kak       (1000) kak       (1000)     5181 2023-12-06 04:36:12.000000 DLStudio-2.4.3/ExamplesAdversarialLearning/dcgan_DG2.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3969 2023-12-06 04:36:12.000000 DLStudio-2.4.3/ExamplesAdversarialLearning/wgan_CG1.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3756 2023-12-06 04:36:12.000000 DLStudio-2.4.3/ExamplesAdversarialLearning/wgan_with_gp_CG2.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/ExamplesDataPrediction/
--rwxr-xr-x   0 kak       (1000) kak       (1000)     3497 2023-12-06 04:36:25.000000 DLStudio-2.4.3/ExamplesDataPrediction/power_load_prediction_with_pmGRU.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/ExamplesDiffusion/
--rw-r--r--   0 kak       (1000) kak       (1000)     3450 2024-03-20 04:39:10.000000 DLStudio-2.4.3/ExamplesDiffusion/GenerateNewImageSamples.py
--rw-rw-r--   0 kak       (1000) kak       (1000)     5361 2024-03-16 14:36:21.000000 DLStudio-2.4.3/ExamplesDiffusion/README
--rw-r--r--   0 kak       (1000) kak       (1000)     3201 2024-03-23 21:29:29.000000 DLStudio-2.4.3/ExamplesDiffusion/RunCodeForDiffusion.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2442 2024-03-23 17:07:15.000000 DLStudio-2.4.3/ExamplesDiffusion/VisualizeSamples.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/ExamplesMetricLearning/
--rw-r--r--   0 kak       (1000) kak       (1000)     2436 2023-12-06 04:36:23.000000 DLStudio-2.4.3/ExamplesMetricLearning/example_for_pairwise_contrastive_loss.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2182 2023-12-06 04:36:23.000000 DLStudio-2.4.3/ExamplesMetricLearning/example_for_triplet_loss.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/ExamplesSeq2SeqLearning/
--rwxr-xr-x   0 kak       (1000) kak       (1000)     2804 2023-12-06 04:36:11.000000 DLStudio-2.4.3/ExamplesSeq2SeqLearning/seq2seq_with_learnable_embeddings.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)     3826 2023-12-06 04:36:11.000000 DLStudio-2.4.3/ExamplesSeq2SeqLearning/seq2seq_with_pretrained_embeddings.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/ExamplesTransformers/
--rwxr-xr-x   0 kak       (1000) kak       (1000)     4936 2023-12-06 04:36:11.000000 DLStudio-2.4.3/ExamplesTransformers/seq2seq_with_transformerFG.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)     4702 2023-12-06 04:36:11.000000 DLStudio-2.4.3/ExamplesTransformers/seq2seq_with_transformerPreLN.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)     3822 2023-12-06 04:36:11.000000 DLStudio-2.4.3/ExamplesTransformers/upgrade_model.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/GenerativeDiffusion/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    66183 2024-03-23 21:30:36.000000 DLStudio-2.4.3/GenerativeDiffusion/GenerativeDiffusion.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      854 2024-03-09 18:01:26.000000 DLStudio-2.4.3/GenerativeDiffusion/__init__.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2588 2024-03-17 19:54:26.000000 DLStudio-2.4.3/MANIFEST.in
--rw-r--r--   0 kak       (1000) kak       (1000)     1120 2023-12-06 04:36:12.000000 DLStudio-2.4.3/Makefile
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/MetricLearning/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    39646 2024-03-23 16:59:38.000000 DLStudio-2.4.3/MetricLearning/MetricLearning.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      584 2023-12-06 04:36:25.000000 DLStudio-2.4.3/MetricLearning/__init__.py
--rw-rw-r--   0 kak       (1000) kak       (1000)     2108 2024-03-23 22:01:59.131379 DLStudio-2.4.3/PKG-INFO
--rw-r--r--   0 kak       (1000) kak       (1000)     1032 2023-12-06 04:36:12.000000 DLStudio-2.4.3/README
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.127379 DLStudio-2.4.3/Seq2SeqLearning/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    80634 2024-03-23 17:01:20.000000 DLStudio-2.4.3/Seq2SeqLearning/Seq2SeqLearning.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      589 2023-12-06 04:36:12.000000 DLStudio-2.4.3/Seq2SeqLearning/__init__.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.131379 DLStudio-2.4.3/TestDLStudio/
--rwxr-xr-x   0 kak       (1000) kak       (1000)   345101 2024-03-23 21:37:12.000000 DLStudio-2.4.3/TestDLStudio/DLStudio.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      585 2023-12-06 04:36:23.000000 DLStudio-2.4.3/TestDLStudio/Test.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      828 2023-12-06 04:36:23.000000 DLStudio-2.4.3/TestDLStudio/TestInstanceCreation.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-03-23 22:01:59.131379 DLStudio-2.4.3/Transformers/
--rwxr-xr-x   0 kak       (1000) kak       (1000)   163326 2024-03-23 16:59:11.000000 DLStudio-2.4.3/Transformers/Transformers.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      496 2023-12-06 04:36:23.000000 DLStudio-2.4.3/Transformers/__init__.py
--rw-rw-r--   0 kak       (1000) kak       (1000)       38 2024-03-23 22:01:59.131379 DLStudio-2.4.3/setup.cfg
--rwxr-xr-x   0 kak       (1000) kak       (1000)     2428 2024-03-17 19:54:06.000000 DLStudio-2.4.3/setup.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.680817 DLStudio-2.4.8/AdversarialLearning/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)    91752 2024-04-27 18:19:47.000000 DLStudio-2.4.8/AdversarialLearning/AdversarialLearning.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      609 2023-12-06 04:36:12.000000 DLStudio-2.4.8/AdversarialLearning/__init__.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.680817 DLStudio-2.4.8/DLStudio/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)   346678 2024-04-27 20:57:17.000000 DLStudio-2.4.8/DLStudio/DLStudio.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      555 2023-12-06 04:36:12.000000 DLStudio-2.4.8/DLStudio/__init__.py
+-rw-rw-r--   0 kak       (1000) kak       (1000)   312388 2024-04-27 21:32:24.000000 DLStudio-2.4.8/DLStudio-2.4.8.html
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.680817 DLStudio-2.4.8/DLStudio.egg-info/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     2108 2024-04-27 21:46:25.000000 DLStudio-2.4.8/DLStudio.egg-info/PKG-INFO
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     2281 2024-04-27 21:46:25.000000 DLStudio-2.4.8/DLStudio.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kak       (1000) kak       (1000)        1 2024-04-27 21:46:25.000000 DLStudio-2.4.8/DLStudio.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      108 2024-04-27 21:46:25.000000 DLStudio-2.4.8/DLStudio.egg-info/top_level.txt
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/DataPrediction/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)    34515 2024-04-27 18:21:48.000000 DLStudio-2.4.8/DataPrediction/DataPrediction.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      584 2023-12-06 04:36:12.000000 DLStudio-2.4.8/DataPrediction/__init__.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/Examples/
+-rw-r--r--   0 kak       (1000) kak       (1000)      516 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/README
+-rw-r--r--   0 kak       (1000) kak       (1000)     2372 2024-02-17 00:32:47.000000 DLStudio-2.4.8/Examples/custom_data_loading.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     4822 2024-02-17 00:35:53.000000 DLStudio-2.4.8/Examples/noisy_object_detection_and_localization.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3518 2024-02-19 18:49:38.000000 DLStudio-2.4.8/Examples/object_detection_and_localization.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3513 2024-03-16 11:10:34.000000 DLStudio-2.4.8/Examples/object_detection_and_localization_iou.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     1900 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/playing_with_cifar10.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2179 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/playing_with_reconfig.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     1652 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/playing_with_sequential.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2161 2024-02-17 00:29:28.000000 DLStudio-2.4.8/Examples/playing_with_skip_connections.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3067 2024-03-17 20:04:07.000000 DLStudio-2.4.8/Examples/semantic_segmentation.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2939 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/text_classification_with_GRU.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3070 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/text_classification_with_GRU_word2vec.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2770 2024-03-26 13:53:50.000000 DLStudio-2.4.8/Examples/text_classification_with_TEXTnet.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3139 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/text_classification_with_TEXTnetOrder2.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3172 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/text_classification_with_TEXTnetOrder2_word2vec.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3084 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/text_classification_with_TEXTnet_word2vec.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesAdversarialLearning/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     3140 2023-12-06 04:36:12.000000 DLStudio-2.4.8/ExamplesAdversarialLearning/README
+-rw-r--r--   0 kak       (1000) kak       (1000)     4755 2024-03-23 17:28:17.000000 DLStudio-2.4.8/ExamplesAdversarialLearning/dcgan_DG1.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     5181 2023-12-06 04:36:12.000000 DLStudio-2.4.8/ExamplesAdversarialLearning/dcgan_DG2.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3969 2023-12-06 04:36:12.000000 DLStudio-2.4.8/ExamplesAdversarialLearning/wgan_CG1.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3756 2023-12-06 04:36:12.000000 DLStudio-2.4.8/ExamplesAdversarialLearning/wgan_with_gp_CG2.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesDataPrediction/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     3497 2023-12-06 04:36:25.000000 DLStudio-2.4.8/ExamplesDataPrediction/power_load_prediction_with_pmGRU.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesDiffusion/
+-rw-r--r--   0 kak       (1000) kak       (1000)     3450 2024-03-20 04:39:10.000000 DLStudio-2.4.8/ExamplesDiffusion/GenerateNewImageSamples.py
+-rw-rw-r--   0 kak       (1000) kak       (1000)     5361 2024-03-16 14:36:21.000000 DLStudio-2.4.8/ExamplesDiffusion/README
+-rw-r--r--   0 kak       (1000) kak       (1000)     3201 2024-03-23 21:29:29.000000 DLStudio-2.4.8/ExamplesDiffusion/RunCodeForDiffusion.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2442 2024-03-23 17:07:15.000000 DLStudio-2.4.8/ExamplesDiffusion/VisualizeSamples.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesMetricLearning/
+-rw-r--r--   0 kak       (1000) kak       (1000)     2436 2023-12-06 04:36:23.000000 DLStudio-2.4.8/ExamplesMetricLearning/example_for_pairwise_contrastive_loss.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2182 2023-12-06 04:36:23.000000 DLStudio-2.4.8/ExamplesMetricLearning/example_for_triplet_loss.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesSeq2SeqLearning/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     2804 2023-12-06 04:36:11.000000 DLStudio-2.4.8/ExamplesSeq2SeqLearning/seq2seq_with_learnable_embeddings.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     3826 2023-12-06 04:36:11.000000 DLStudio-2.4.8/ExamplesSeq2SeqLearning/seq2seq_with_pretrained_embeddings.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesTransformers/
+-rw-r--r--   0 kak       (1000) kak       (1000)     2451 2024-04-27 20:50:21.000000 DLStudio-2.4.8/ExamplesTransformers/image_recog_with_visTransformer.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     5080 2024-04-27 14:48:55.000000 DLStudio-2.4.8/ExamplesTransformers/seq2seq_with_transformerFG.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     4840 2024-04-27 14:49:07.000000 DLStudio-2.4.8/ExamplesTransformers/seq2seq_with_transformerPreLN.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2909 2024-04-26 03:59:11.000000 DLStudio-2.4.8/ExamplesTransformers/test_checkpoint_for_visTransformer.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3822 2023-12-06 04:36:11.000000 DLStudio-2.4.8/ExamplesTransformers/upgrade_model.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/GenerativeDiffusion/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)    66182 2024-04-27 18:25:02.000000 DLStudio-2.4.8/GenerativeDiffusion/GenerativeDiffusion.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      854 2024-03-09 18:01:26.000000 DLStudio-2.4.8/GenerativeDiffusion/__init__.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2548 2024-04-27 21:04:33.000000 DLStudio-2.4.8/MANIFEST.in
+-rw-r--r--   0 kak       (1000) kak       (1000)     1120 2023-12-06 04:36:12.000000 DLStudio-2.4.8/Makefile
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/MetricLearning/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)    39645 2024-04-27 18:24:24.000000 DLStudio-2.4.8/MetricLearning/MetricLearning.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      584 2023-12-06 04:36:25.000000 DLStudio-2.4.8/MetricLearning/__init__.py
+-rw-rw-r--   0 kak       (1000) kak       (1000)     2108 2024-04-27 21:46:25.684817 DLStudio-2.4.8/PKG-INFO
+-rw-r--r--   0 kak       (1000) kak       (1000)     1032 2023-12-06 04:36:12.000000 DLStudio-2.4.8/README
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/Seq2SeqLearning/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)    80633 2024-04-27 18:20:35.000000 DLStudio-2.4.8/Seq2SeqLearning/Seq2SeqLearning.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      589 2023-12-06 04:36:12.000000 DLStudio-2.4.8/Seq2SeqLearning/__init__.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/TestDLStudio/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)   346678 2024-04-27 21:02:42.000000 DLStudio-2.4.8/TestDLStudio/DLStudio.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      585 2023-12-06 04:36:23.000000 DLStudio-2.4.8/TestDLStudio/Test.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      828 2023-12-06 04:36:23.000000 DLStudio-2.4.8/TestDLStudio/TestInstanceCreation.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/Transformers/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)   191880 2024-04-27 18:23:27.000000 DLStudio-2.4.8/Transformers/Transformers.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      553 2024-03-28 13:14:29.000000 DLStudio-2.4.8/Transformers/__init__.py
+-rw-rw-r--   0 kak       (1000) kak       (1000)       38 2024-04-27 21:46:25.684817 DLStudio-2.4.8/setup.cfg
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     2428 2024-04-27 06:52:24.000000 DLStudio-2.4.8/setup.py
```

### Comparing `DLStudio-2.4.3/AdversarialLearning/AdversarialLearning.py` & `DLStudio-2.4.8/AdversarialLearning/AdversarialLearning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.3'
+__version__   = '2.4.8'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-March-23'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html'
+__date__      = '2024-April-27'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
 __doc__ = '''
 
 
   You are looking at the AdversarialLearning co-class file in the DLStudio platform.
@@ -991,31 +991,34 @@
                     ##  that does not exist in the computational graph. That is, the call shown below first 
                     ##  makes a copy of the 'fakes' tensor and then removes it from the computational graph. 
                     ##  The original 'fakes' tensor continues to remain in the computational graph.  This ploy 
                     ##  ensures that a subsequent call to backward() in the 3rd statement below would only
                     ##  update the netD weights.
                     output = netD(fakes.detach()).view(-1)    
                     lossD_for_fakes = criterion(output, label)    
-                    ##  At this point, we do not care if the following call also calculates the gradients
-                    ##  wrt the Discriminator weights since we are going to next iteration with 'netD.zero_grad()':
                     lossD_for_fakes.backward()          
+                    ##  The following is just for displaying the losses:
                     lossD = lossD_for_reals + lossD_for_fakes    
                     d_losses_per_print_cycle.append(lossD)  
                     ##  Only the Discriminator weights are incremented:
                     optimizerD.step()  
 
                     ##  Minimization Part of the Min-Max Objective of Eq. (3):
                     ##
-                    ##  That brings to the min part of the max-min optimization described in Eq. (3) the doc 
+                    ##  That brings us to the min part of the max-min optimization described in Eq. (3) the doc 
                     ##  section at the beginning of this file.  The min part requires that we minimize 
                     ##  "1 - D(G(z))" which, since D is constrained to lie in the interval (0,1), requires that 
                     ##  we maximize D(G(z)).  We accomplish that by applying the Discriminator to the output 
                     ##  of the Generator and use 1 as the target for each image:
                     netG.zero_grad()   
                     label.fill_(real_label)  
+                    ##  The following forward prop will compute the partials wrt the discriminator params also, but
+                    ##  they will never get used for updating param vals for two reasons: (1) We call "step()" on 
+                    ##  just optimizerG as shown later below; and (2) We call "netD.zero_grad()" at the beginning of 
+                    ##  each training cycle.
                     output = netD(fakes).view(-1)   
                     lossG = criterion(output, label)          
                     g_losses_per_print_cycle.append(lossG) 
                     lossG.backward()    
                     ##  Only the Generator parameters are incremented:
                     optimizerG.step() 
                     if i % 100 == 99:
```

### Comparing `DLStudio-2.4.3/AdversarialLearning/__init__.py` & `DLStudio-2.4.8/AdversarialLearning/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/DLStudio/DLStudio.py` & `DLStudio-2.4.8/DLStudio/DLStudio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.3'
+__version__   = '2.4.8'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-March-23'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html'
+__date__      = '2024-April-27'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
 
 __doc__ = '''
 
 DLStudio.py
@@ -18,27 +18,37 @@
 
 Date: ''' + __date__ + '''
 
 
 @tag_changes
 CHANGE LOG:
 
+  Version 2.4.8:
+
+    In this version, I have made two important changes to the Transformers module
+    in DLStudio: (1) The Transformers module now includes a new class that I have
+    named visTransformer that works like the famous Vision Transformer (ViT)
+    proposed by Dosovitskiy et al. And (2) I have made changes to the QKV code for
+    the calculation of self and cross attention in all of the Transformer classes
+    in the module. The attention calculations should now execute faster, which is
+    a very important consideration in any transformer based learning.
+
   Version 2.4.3:
 
     The diffusion modeling part of the code should now accept training images of
     any size.  Previously it was limited to images of size 64x64.  Note that this
     change is not as significant as you might think because, under the hood, the
     actual input image size is changed to the size 64x64 for diffusion modeling.
     So this change is more for your convenience than anything else.  I have also
     improved the image visualization code in the ExamplesDiffusion directory. The
     new implementation of the script VisualizeSamples.py automatically generates a
     collage of the images generated from noise by the script
-    GenerateNewImageSamples.py.  Other changes include a minor clean-up of the
-    main doc page for GenerativeDiffusion module and of a couple of the functions
-    in the module.
+    GenerateNewImageSamples.py.  Other changes include minor clean-up of the main
+    doc page for GenerativeDiffusion module and of a couple of the functions in
+    the module.
 
   Version 2.4.2:
 
     DLStudio now includes a new module devoted to data modeling with diffusion.
     This module, named GenerativeDiffusion, is a co-class of DLStudio.  That is,
     GenerativeDiffusion resides at the same level of software abstraction as the
     main DLStudio class in the platform.  See the README in the new
@@ -1002,54 +1012,73 @@
     dataset used in this example.  See the "For Data Prediction" part of the "The
     Datasets Included" section of the doc page for that.
 
 
 @tag2_transformers
     TRANSFORMERS
 
-    The goal of Transformer based learning is the same that of Seq2SeqLearning
-    described earlier in this Introduction except that now you completely forgo
-    recurrence. That is, you only use the mechanism of attention to translate
-    sentences from a source language into sentences in the target language. For
-    such applications, you need two forms of attention: self-attention and
-    cross-attention.  Self-attention refers to the intra-sentence relationships
-    between the words and cross-attention refers to the inter-sentence
-    relationships between the words in a pair of sentences, one in the source
-    language and the other in the target language. I have explained these concepts
-    in great detail in the doc sections of the inner classes in the Transformers
-    class.  In particular, I have explained the concept of the "dot-product"
-    attention in which each word puts out three things: a Query Vector Q, a Key
-    Vector K, and a Value Vector V. By taking the dot-product of the Query Vector
-    Q of a word with the Key Vector K for all the words in a sentence, the neural
-    network gets a measure of the extent to which each word in a sentence is
-    important to every other word.  These dot-product values are then used as
-    weights on the Value Vectors, V, for the individual words.  Cross attention
-    works in a similar manner, except that now you take the dot-products of the Q
-    vectors in the target-language sentence with the K vectors in the
+    For Seq2SeqLearning learning, the goal of a Transformer based implementation
+    is the same as described earlier in this Introduction except that now you
+    completely forgo recurrence. That is, you only use the mechanism of attention
+    to translate sentences from a source language into sentences in the target
+    language. For such applications, you need two forms of attention:
+    self-attention and cross-attention.  Self-attention refers to the
+    intra-sentence relationships between the words and cross-attention refers to
+    the inter-sentence relationships between the words in a pair of sentences, one
+    in the source language and the other in the target language. I have explained
+    these concepts in great detail in the doc sections of the inner classes in the
+    Transformers class.  In particular, I have explained the concept of the
+    "dot-product" attention in which each word puts out three things: a Query
+    Vector Q, a Key Vector K, and a Value Vector V. By taking the dot-product of
+    the Query Vector Q of a word with the Key Vector K for all the words in a
+    sentence, the neural network gets a measure of the extent to which each word
+    in a sentence is important to every other word.  These dot-product values are
+    then used as weights on the Value Vectors, V, for the individual words.  Cross
+    attention works in a similar manner, except that now you take the dot-products
+    of the Q vectors in the target-language sentence with the K vectors in the
     corresponding source-language sentence for producing the weight vectors that
     tell us how to weight the source-language Value Vectors vis-a-vis the words in
     the target language.
 
-    You will see two different implementations of the transformer architecture in
+    In addition to their use in Seq2SeqLearning learning, transformers are now
+    also used widely in computer vision applications. As a nod to their adoption
+    in the learning required for solving CV problems, I have created a new class
+    named visTransformer in the Transformers module of DLStudio.  The transformer
+    part of the logic in a visTransformer is identical to what it is in a
+    transformer class for Seq2SeqLearning learning.  That logic kicks in after you
+    have divided an image into patches and you represent each patch by an
+    embedding vector --- in exactly the same as when you represent a word or a
+    token in a sentence by an embedding vector.
+
+    You will see three different implementations of the transformer architecture in
     the Transformers co-class of DLStudio:
 
           TransformerFG
-    and
+
           TransformerPreLN
 
-    with the "FG" suffix standing for "First Generation" and the "PreLN" suffix
-    for "Pre LayerNorm". TransformerFG is my implementation of the transformer
-    architecture proposed in the famous paper by Vaswani et al.  and
-    TransformerPreLN my implementation of the same architecture but with the
-    modification suggested by Xiong et al. for more stable learning.  Since, the
-    modification is small from an architectural standpoint, I could have combined
-    both transformer types in the same implementation with some conditional logic
-    to account for the differences.  However, I have chosen to keep them separate
-    mostly for educational purposes.  Further details on these implementations are
-    in the documentation blocks in the Transformers co-class.
+          visTransformer
+
+    The "FG" suffix TransformerFG stands for "First Generation"; the "PreLN"
+    suffix in TransformerPreLN for "Pre LayerNorm"; and, finally, the name
+    visTransformer stands for "Vision Transformer."  
+
+    TransformerFG is my implementation of the transformer architecture proposed in
+    the famous paper by Vaswani et al.  and TransformerPreLN my implementation of
+    the same architecture but with the modification suggested by Xiong et al. for
+    more stable learning.  Since, the modification is small from an architectural
+    standpoint, I could have combined both transformer types in the same
+    implementation with some conditional logic to account for the differences.
+    However, I have chosen to keep them separate mostly for educational purposes.
+    Further details on these implementations are in the documentation blocks in
+    the Transformers co-class.  
+
+    The visTransformer implementation is based on the paper "An Image is Worth
+    16x16 Words: Transformers for Image Recognition at Scale'' by Dosovitskiy et
+    al.
  
     If you want to use my code for learning the main ideas related to how to
     create purely attention based networks, your starting point for that should be
     the following scripts in the ExamplesTransformers directory of the DLStudio
     distribution:
 
         seq2seq_with_transformerFG.py
@@ -1061,14 +1090,24 @@
 
     that contains 90,000 pairs of English-Spanish sentences with the maximum
     number of words in each sentence limited to 8 words.  For processing by the
     attention networks, each sentence is enclosed in <SOS> and <EOS> tokens, with
     the former standing for "Start of Sentence" and the latter for "End of
     Sentence".
 
+    And if you wish to use visTransformer for solving image recognition problems
+    with a transformer based implementation, your starting point should be
+    the following scripts in the same ExamplesTransformers directory that was
+    mentioned above:
+
+          image_recog_with_visTransformer.py
+          test_checkpoint_for_visTransformer.py 
+
+    Both these script use the CIFAR10 dataset for demonstrating image recognition.
+
 
 @tag2_metriclearning
     METRIC LEARNING
 
     The main idea of metric learning is to learn a mapping from the images to
     their embedding vector representations in such a way that the embeddings for
     what are supposed to be similar images are pulled together and those for
@@ -1653,35 +1692,43 @@
 
 
 @tag_coclass5
     ============
     Transformers
     ============
 
-    The code in this co-class of DLStudio consists two slightly different
-    implementations of the transformer architecture: TransformerFG and
-    TransformerPreLN.  TransformerFG is my implementation of the architecture as
-    conceptualized in the famous paper "Attention is All You Need" by Vaswani et
-    el.  And TransformerPreLN is my implementation of the original idea along with
-    the modifications suggested by Xiong et al. in their paper "On Layer
-    Normalization in the Transformer Architecture" for more stable learning.  The
-    two versions of transformers differ in only one respect: The placement of the
-    LayerNorm in relation to the architectural components related to attention and
-    the feedforward network.  Literally, the difference is small, yet its
-    consequences on the stability of learning significant.
-
-    The fundamentals of how the attention works in both TransformerFG and
-    TransformerPreLN are exactly the same.  For self-attention, you associate a
-    Query Vector Q_i and a Key Vector K_i with each word w_i in a sentence.  For a
-    given w_i, the dot product of its Q_i with the K_j vectors for all the other
-    words w_j is a measure of how related w_i is to each w_j with regard to what's
-    needed for the translation of a source sentence into the target sentence.  One
-    more vector you associate with each word w_i is the Value Vector V_i.  The
-    value vectors for the words in a sentence are weighted by the output of the
-    activation nn.LogSoftmax applied to the dot-products.
+    The code in this module of DLStudio consists of three different
+    implementations of the transformer architecture: (1) TransformerFG, (2)
+    TransformerPreLN, and (3) visTransformer.  The first two of these are meant
+    for seq2seq learning, as in language translation, and the last is for solving
+    the problem of image recognition.
+
+    TransformerFG is my implementation of the architecture as conceptualized in
+    the famous paper "Attention is All You Need" by Vaswani et el.  And
+    TransformerPreLN is my implementation of the original idea along with the
+    modifications suggested by Xiong et al. in their paper "On Layer Normalization
+    in the Transformer Architecture" for more stable learning.  The two versions
+    of transformers differ in only one respect: The placement of the LayerNorm in
+    relation to the architectural components related to attention and the
+    feedforward network.  Literally, the difference is small, yet its consequences
+    are significant regarding the stability of learning.  Finally, visTransformer
+    is my implementation of the Vision Transformer as presented in the famou paper
+    "An Image is Worth 16x16$ Words: Transformers for Image Recognition at Scale''
+    by Dosovitskiy et al.
+
+    The fundamentals of how the attention works in all three transformer based
+    implementations in the Transformers module are exactly the same.  For
+    self-attention, you associate a Query Vector Q_i and a Key Vector K_i with
+    each word w_i in a sentence.  For a given w_i, the dot product of its Q_i with
+    the K_j vectors for all the other words w_j is a measure of how related w_i is
+    to each w_j with regard to what's needed for the translation of a source
+    sentence into the target sentence.  One more vector you associate with each
+    word w_i is the Value Vector V_i.  The value vectors for the words in a
+    sentence are weighted by the output of the activation nn.LogSoftmax applied to
+    the dot-products.
 
     The self-attention mechanism described above is half of what goes into each
     base encoder of a transformer, the other half is a feedforward network
     (FFN). The overall encoder consists of a cascade of these base encoders.  In
     my implementation, I have referred to the overall encoder as the
     MasterEncoder.  The MasterDecoder also consists of a cascade of base decoders.
     A base decoder is similar to a base encoder except for there being a layer of
@@ -1701,24 +1748,32 @@
     the self-attention layer and residual connection wraps around both.
     Similarly, LayerNorm is applied to the input to FFN and the residual
     connection wraps around both.  Similar considerations applied to the decoder
     side, except we now also have a layer of cross-attention interposed between
     the self-attention and FFN.
    
     As I mentioned in the Introduction, your main entry point for experimenting
-    with the transformer code in DLStudio are the following two scripts in the
-    ExamplesTransformers directory of the distribution:
+    with the seq2seq based transformer code in DLStudio are the following two
+    scripts in the ExamplesTransformers directory of the distribution:
 
         seq2seq_with_transformerFG.py
         seq2seq_with_transformerPreLN.py
 
     However, before you can run these scripts, you would need to download the
     training dataset used in these examples.  See the "For Transformers" part of
     the "The Datasets Included" section of this doc page for that.
 
+    And your main entry point for experimenting with image recognition by playing
+    with the visTransformer class are the scripts:
+
+          image_recog_with_visTransformer.py
+          test_checkpoint_for_visTransformer.py 
+
+    Both these script use the CIFAR10 dataset for demonstrating image recognition.
+
 
 @tag_coclass6
     ===================
     MetricLearning:
     ===================
 
     As mentioned in the Introduction, the main idea of metric learning is to learn
@@ -2036,38 +2091,28 @@
     a link at the top of the main DLStudio doc page.
 
 
 @tag_examples_xform
 ExamplesTransformers DIRECTORY:
 
     The ExamplesTransformers directory of the distribution contains the following
-    two scripts for experimenting with transformers:
+    four scripts for experimenting with transformers in DLStudio:
 
         seq2seq_with_transformerFG.py 
         seq2seq_with_transformerPreLN.py         
 
-    Both these scripts deal with English-to-Spanish translation in a manner
-    similar to what's demonstrated by the code in the Seq2SeqLearning co-class and
-    the example scripts associated with that co-class.
-
-    The directory also contains the following two scripts
+        image_recog_with_visTransformer.py
+        test_checkpoint_for_visTransformer.py 
 
-        test_checkpointFG.py
-        test_checkpointPreLN.py
 
-    to address the problems of training a transformer network.  As I have
-    mentioned elsewhere in this documentation, transformer training can be
-    frustrating, to say the least, and can take a very long time.  What
-    exacerbates the frustrations is that, with a wrong choice for the
-    hyperparameters, you could end with model divergence in the middle of training
-    and not know about it until the end.  [Model divergence is akin to mode
-    collapse in training a GAN.]  To deal with these problems, starting with
-    Version 2.2.7, the transformer training routines now create a checkpoint of
-    the model every 5 epochs. While the training is going on, you can evaluate the
-    checkpoints in the manner illustrated by the above two scripts.
+    The first two scripts deal with English-to-Spanish translation in a manner
+    similar to what's demonstrated by the code in the Seq2SeqLearning co-class and
+    the example scripts associated with that co-class. The last two relate to my
+    demonstration of image recognition with a transformer based implementation.  I
+    have used the CFAR10 dataset for image recognition.
 
 
 @tag_examples_metric
 ExamplesMetricLearning DIRECTORY:
 
     The ExamplesMetricLearning directory at top level of the distribution 
     contains the following scripts:
@@ -2302,15 +2347,16 @@
         ExamplesDataPrediction directory.  With that you should be able to execute
         the data prediction script in that directory.
 
 
 @tag2_dataset
     FOR TRANSFORMERS:
 
-        Download the dataset archive
+        For the seq2seq learning part of the Transformers module in DLStudio,
+        download the dataset archive
 
             en_es_corpus_for_learning_with_Transformers.tar.gz
 
         into the ExamplesTransformers directory of the DLStudio distribution.
         Next, execute the following command in that directory:
 
             tar zxvf en_es_corpus_for_learning_with_Transformers.tar.gz
@@ -2625,23 +2671,19 @@
                                   tvt.ToTensor(),
                                   tvt.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))])        
         ##  Don't need any augmentation for the test data: 
         transform_test = tvt.Compose([
                                tvt.ToTensor(),
                                tvt.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))])
         ##  Define where the training and the test datasets are located
-        train_data_loc = torchvision.datasets.CIFAR10(
-                        root=self.dataroot, train=True, download=True, transform=transform_train)
-        test_data_loc = torchvision.datasets.CIFAR10(
-                      root=self.dataroot, train=False, download=True, transform=transform_test)
+        train_data_loc = torchvision.datasets.CIFAR10( root=self.dataroot, train=True, download=True, transform=transform_train )
+        test_data_loc = torchvision.datasets.CIFAR10(  root=self.dataroot, train=False, download=True, transform=transform_test )
         ##  Now create the data loaders:
-        self.train_data_loader = torch.utils.data.DataLoader(train_data_loc, batch_size=self.batch_size, 
-                                                                     shuffle=True, num_workers=2)
-        self.test_data_loader = torch.utils.data.DataLoader(test_data_loc, batch_size=self.batch_size, 
-                                                                 shuffle=False, num_workers=2)
+        self.train_data_loader = torch.utils.data.DataLoader(train_data_loc, batch_size=self.batch_size, shuffle=True, num_workers=2)
+        self.test_data_loader = torch.utils.data.DataLoader(test_data_loc, batch_size=self.batch_size, shuffle=False, num_workers=2)
 
     def imshow(self, img):
         '''
         called by display_tensor_as_image() for displaying the image
         '''
         img = img / 2 + 0.5     # unnormalize
         npimg = img.numpy()
@@ -2705,17 +2747,15 @@
                     FILE.flush()
                     running_loss = 0.0
                     if display_images:
                         logger = logging.getLogger()
                         old_level = logger.level
                         logger.setLevel(100)
                         plt.figure(figsize=[6,3])
-
-                        plt.imshow(np.transpose(torchvision.utils.make_grid(inputs, 
-                                                            normalize=False, padding=3, pad_value=255).cpu(), (1,2,0)))
+                        plt.imshow(np.transpose(torchvision.utils.make_grid(inputs,  normalize=False, padding=3, pad_value=255).cpu(), (1,2,0)))
                         plt.show()
                         logger.setLevel(old_level)
                 loss.backward()
                 optimizer.step()
         print("\nFinished Training\n")
         self.save_model(net)
         plt.figure(figsize=(10,5))
@@ -2807,32 +2847,29 @@
         with torch.no_grad():
             for i,data in enumerate(self.test_data_loader):
                 ##  data is set to the images and the labels for one batch at a time:
                 images, labels = data
                 images = images.to(self.device)
                 labels = labels.to(self.device)
                 if i % 1000 == 999:
-                    print("\n\n[i=%d:] Ground Truth:     " % (i+1) + ' '.join('%5s' % self.class_labels[labels[j]] 
-                                                                   for j in range(self.batch_size)))
+                    print("\n\n[i=%d:] Ground Truth:     " % (i+1) + ' '.join('%5s' % self.class_labels[labels[j]] for j in range(self.batch_size)))
                 outputs = net(images)
                 ##  max() returns two things: the max value and its index in the 10 element
                 ##  output vector.  We are only interested in the index --- since that is 
                 ##  essentially the predicted class label:
                 _, predicted = torch.max(outputs.data, 1)#
 #                if display_images and i % 1000 == 999:
                 if i % 1000 == 999:
-                    print("[i=%d:] Predicted Labels: " % (i+1) + ' '.join('%5s' % self.class_labels[predicted[j]]
-                                                              for j in range(self.batch_size)))
+                    print("[i=%d:] Predicted Labels: " % (i+1) + ' '.join('%5s' % self.class_labels[predicted[j]] for j in range(self.batch_size)))
                     logger = logging.getLogger()
                     old_level = logger.level
                     if display_images:
                         logger.setLevel(100)
                         plt.figure(figsize=[6,3])
-                        plt.imshow(np.transpose(torchvision.utils.make_grid(images,
-                                                      normalize=False, padding=3, pad_value=255).cpu(), (1,2,0)))
+                        plt.imshow(np.transpose(torchvision.utils.make_grid(images, normalize=False, padding=3, pad_value=255).cpu(), (1,2,0)))
                         plt.show()
                         logger.setLevel(old_level)
                 for label,prediction in zip(labels,predicted):
                         confusion_matrix[label][prediction] += 1
                 total += labels.size(0)
                 correct += (predicted == labels).sum().item()
                 ##  comp is a list of size batch_size of "True" and "False" vals
@@ -3088,32 +3125,32 @@
         networks are difficult to train because of the vanishing gradients problem.
         What that means is that as the depth of network increases, the loss gradients
         calculated for the early layers become more and more muted, which suppresses
         the learning of the parameters in those layers.  An important mitigation
         strategy for addressing this problem consists of creating a CNN using blocks
         with skip connections.
 
-        With the code shown in this inner class of the module, you can now experiment
-        with skip connections in a CNN to see how a deep network with this feature
-        might improve the classification results.  As you will see in the code shown
-        below, the network that allows you to construct a CNN with skip connections
-        is named BMEnet.  As shown in the script playing_with_skip_connections.py in
-        the Examples directory of the distribution, you can easily create a CNN with
-        arbitrary depth just by using the "depth" constructor option for the BMEnet
-        class.  The basic block of the network constructed by BMEnet is called
-        SkipBlock which, very much like the BasicBlock in ResNet-18, has a couple of
-        convolutional layers whose output is combined with the input to the block.
-    
-        Note that the value given to the "depth" constructor option for the BMEnet
-        class does NOT translate directly into the actual depth of the CNN. [Again,
-        see the script playing_with_skip_connections.py in the Examples directory for
-        how to use this option.] The value of "depth" is translated into how many
-        "same input and output channels" and the "same input and output sizes"
-        instances of SkipBlock to use between successive instances of downsampling
-        and channel-doubling instances of SkipBlock.
+        With the code shown in this inner class of the module, you can now experiment with
+        skip connections in a CNN to see how a deep network with this feature might improve
+        the classification results.  As you will see in the code shown below, the network
+        that allows you to construct a CNN with skip connections is named BMEnet.  As shown
+        in the script playing_with_skip_connections.py in the Examples directory of the
+        distribution, you can easily create a CNN with arbitrary depth just by using the
+        "depth" constructor option for the BMEnet class.  The basic block of the network
+        constructed by BMEnet is called SkipBlock which, very much like the BasicBlock in
+        ResNet-18, has a couple of convolutional layers whose output is combined with the
+        input to the block.
+    
+        Note that the value given to the "depth" constructor option for the BMEnet class
+        does NOT translate directly into the actual depth of the CNN. [Again, see the script
+        playing_with_skip_connections.py in the Examples directory for how to use this
+        option.] The value of "depth" is translated into how many "same input and output
+        channels" and the "same input and output sizes" instances of SkipBlock to use
+        between successive instances of downsampling and channel-doubling instances of
+        SkipBlock.
  
         Class Path: DLStudio -> BMEnet
         """
         def __init__(self, dl_studio, skip_connections=True, depth=8):
             super(DLStudio.BMEnet, self).__init__()
             self.dl_studio = dl_studio
             self.depth = depth
@@ -3215,40 +3252,39 @@
 
 
     ###%%%
     ########################################################################################
     #################  Start Definition of Inner Class CustomDataLoading  ##################
 
     class CustomDataLoading(nn.Module):             
-        """This is a testbed for experimenting with a completely grounds-up attempt at
-        designing a custom data loader.  Ordinarily, if the basic format of how the
-        dataset is stored is similar to one of the datasets that the Torchvision
-        module knows about, you can go ahead and use that for your own dataset.  At
-        worst, you may need to carry out some light customizations depending on the
-        number of classes involved, etc.
-
-        However, if the underlying dataset is stored in a manner that does not look
-        like anything in Torchvision, you have no choice but to supply yourself all
-        of the data loading infrastructure.  That is what this inner class of the 
-        DLStudio module is all about.
-
-        The custom data loading exercise here is related to a dataset called
-        PurdueShapes5 that contains 32x32 images of binary shapes belonging to the
-        following five classes:
+        """
+        This is a testbed for experimenting with a completely grounds-up attempt at
+        designing a custom data loader.  Ordinarily, if the basic format of how the dataset
+        is stored is similar to one of the datasets that the Torchvision module knows about,
+        you can go ahead and use that for your own dataset.  At worst, you may need to carry
+        out some light customizations depending on the number of classes involved, etc.
+
+        However, if the underlying dataset is stored in a manner that does not look like
+        anything in Torchvision, you have no choice but to supply yourself all of the data
+        loading infrastructure.  That is what this inner class of the DLStudio module is all
+        about.
+
+        The custom data loading exercise here is related to a dataset called PurdueShapes5
+        that contains 32x32 images of binary shapes belonging to the following five classes:
 
                        1.  rectangle
                        2.  triangle
                        3.  disk
                        4.  oval
                        5.  star
 
-        The dataset was generated by randomizing the sizes and the orientations
-        of these five patterns.  Since the patterns are rotated with a very simple
-        non-interpolating transform, just the act of random rotations can introduce
-        boundary and even interior noise in the patterns.
+        The dataset was generated by randomizing the sizes and the orientations of these
+        five patterns.  Since the patterns are rotated with a very simple non-interpolating
+        transform, just the act of random rotations can introduce boundary and even interior
+        noise in the patterns.
 
         Each 32x32 image is stored in the dataset as the following list:
 
                            [R, G, B, Bbox, Label]
         where
                 R     :   is a 1024 element list of the values for the red component
                           of the color at all the pixels
@@ -3258,30 +3294,30 @@
                 G     :   the same as above but for the blue component of the color
 
                 Bbox  :   a list like [x1,y1,x2,y2] that defines the bounding box 
                           for the object in the image
            
                 Label :   the shape of the object
 
-        I serialize the dataset with Python's pickle module and then compress it with 
-        the gzip module.  
+        I serialize the dataset with Python's pickle module and then compress it with the
+        gzip module.
 
-        You will find the following dataset directories in the "data" subdirectory
-        of Examples in the DLStudio distro:
+        You will find the following dataset directories in the "data" subdirectory of
+        Examples in the DLStudio distro:
 
                PurdueShapes5-10000-train.gz
                PurdueShapes5-1000-test.gz
                PurdueShapes5-20-train.gz
                PurdueShapes5-20-test.gz               
 
-        The number that follows the main name string "PurdueShapes5-" is for the 
-        number of images in the dataset.  
+        The number that follows the main name string "PurdueShapes5-" is for the number of
+        images in the dataset.
 
-        You will find the last two datasets, with 20 images each, useful for debugging
-        your logic for object detection and bounding-box regression.
+        You will find the last two datasets, with 20 images each, useful for debugging your
+        logic for object detection and bounding-box regression.
 
         Class Path:   DLStudio  ->  CustomDataLoading
         """     
         def __init__(self, dl_studio, dataserver_train=None, dataserver_test=None, dataset_file_train=None, dataset_file_test=None):
             super(DLStudio.CustomDataLoading, self).__init__()
             self.dl_studio = dl_studio
             self.dataserver_train = dataserver_train
@@ -3549,29 +3585,29 @@
     ###%%%
     ########################################################################################
     ###################  Start Definition of Inner Class DetectAndLocalize  ################
 
     class DetectAndLocalize(nn.Module):             
         """
         The purpose of this inner class is to focus on object detection in images --- as
-        opposed to image classification.  Most people would say that object detection
-        is a more challenging problem than image classification because, in general,
-        the former also requires localization.  The simplest interpretation of what
-        is meant by localization is that the code that carries out object detection
-        must also output a bounding-box rectangle for the object that was detected.
-
-        You will find in this inner class some examples of LOADnet classes meant
-        for solving the object detection and localization problem.  The acronym
-        "LOAD" in "LOADnet" stands for
+        opposed to image classification.  Most people would say that object detection is a
+        more challenging problem than image classification because, in general, the former
+        also requires localization.  The simplest interpretation of what is meant by
+        localization is that the code that carries out object detection must also output a
+        bounding-box rectangle for the object that was detected.
+
+        You will find in this inner class some examples of LOADnet classes meant for solving
+        the object detection and localization problem.  The acronym "LOAD" in "LOADnet"
+        stands for
 
                     "LOcalization And Detection"
 
-        The different network examples included here are LOADnet1, LOADnet2, and
-        LOADnet3.  For now, only pay attention to LOADnet2 since that's the class I
-        have worked with the most for the 1.0.7 distribution.
+        The different network examples included here are LOADnet1, LOADnet2, and LOADnet3.
+        For now, only pay attention to LOADnet2 since that's the class I have worked with
+        the most for the 1.0.7 distribution.
 
         Class Path:   DLStudio  ->  DetectAndLocalize
         """
         def __init__(self, dl_studio, dataserver_train=None, dataserver_test=None, dataset_file_train=None, dataset_file_test=None):
             super(DLStudio.DetectAndLocalize, self).__init__()
             self.dl_studio = dl_studio
             self.dataserver_train = dataserver_train
@@ -3758,34 +3794,29 @@
                         out = out + torch.cat((identity, identity), dim=1)
                 return out
 
 
 
         class LOADnet1(nn.Module):
             """
-            The acronym 'LOAD' stands for 'LOcalization And Detection'.
-            LOADnet1 only uses fully-connected layers for the regression
+            The acronym 'LOAD' stands for 'LOcalization And Detection'.  LOADnet1 only
+            uses fully-connected layers for the regression
 
             Class Path:   DLStudio  ->  DetectAndLocalize  ->  LOADnet1
             """
             def __init__(self, skip_connections=True, depth=32):
                 super(DLStudio.DetectAndLocalize.LOADnet1, self).__init__()
                 self.pool_count = 3
                 self.depth = depth // 2
                 self.conv = nn.Conv2d(3, 64, 3, padding=1)
-                self.skip64 = DLStudio.DetectAndLocalize.SkipBlock3(64, 64, 
-                                                           skip_connections=skip_connections)
-                self.skip64ds = DLStudio.DetectAndLocalize.SkipBlock3(64, 64, 
-                                           downsample=True, skip_connections=skip_connections)
-                self.skip64to128 = DLStudio.DetectAndLocalize.SkipBlock3(64, 128, 
-                                                            skip_connections=skip_connections )
-                self.skip128 = DLStudio.DetectAndLocalize.SkipBlock3(128, 128, 
-                                                             skip_connections=skip_connections)
-                self.skip128ds = DLStudio.DetectAndLocalize.SkipBlock3(128,128,
-                                            downsample=True, skip_connections=skip_connections)
+                self.skip64 = DLStudio.DetectAndLocalize.SkipBlock3(64, 64, skip_connections=skip_connections)
+                self.skip64ds = DLStudio.DetectAndLocalize.SkipBlock3(64, 64, downsample=True, skip_connections=skip_connections)
+                self.skip64to128 = DLStudio.DetectAndLocalize.SkipBlock3(64, 128, skip_connections=skip_connections )
+                self.skip128 = DLStudio.DetectAndLocalize.SkipBlock3(128, 128, skip_connections=skip_connections)
+                self.skip128ds = DLStudio.DetectAndLocalize.SkipBlock3(128,128, downsample=True, skip_connections=skip_connections)
                 self.fc1 =  nn.Linear(128 * (32 // 2**self.pool_count)**2, 1000)
                 self.fc2 =  nn.Linear(1000, 5)
                 self.fc3 =  nn.Linear(32768, 1000)
                 self.fc4 =  nn.Linear(1000, 4)
 
             def forward(self, x):
                 x = nn.MaxPool2d(2,2)(nn.functional.relu(self.conv(x)))          
@@ -3808,16 +3839,16 @@
                 x2 =  x.view( x.shape[0], - 1 )
                 x2 = nn.functional.relu(self.fc3(x2))
                 x2 = self.fc4(x2)
                 return x1,x2
 
         class LOADnet2(nn.Module):
             """
-            The acronym 'LOAD' stands for 'LOcalization And Detection'.
-            LOADnet2 uses both convo and linear layers for regression
+            The acronym 'LOAD' stands for 'LOcalization And Detection'.  LOADnet2 uses
+            both convo and linear layers for regression
 
             Class Path:   DLStudio  ->  DetectAndLocalize  ->  LOADnet2
             """ 
             def __init__(self, skip_connections=True, depth=8):
                 super(DLStudio.DetectAndLocalize.LOADnet2, self).__init__()
                 if depth not in [8,10,12,14,16]:
                     sys.exit("LOADnet2 has only been tested for 'depth' values 8, 10, 12, 14, and 16")
@@ -3884,18 +3915,19 @@
                 x2 = x2.view( x.shape[0], - 1 )
                 x2 = self.fc_seqn(x2)
                 return x1,x2
 
 
         class LOADnet3(nn.Module):
             """
-            The acronym 'LOAD' stands for 'LOcalization And Detection'.
-            LOADnet3 uses both convo and linear layers for regression
+            The acronym 'LOAD' stands for 'LOcalization And Detection'.  LOADnet3 uses
+            both convo and linear layers for regression
 
             Class Path:   DLStudio  ->  DetectAndLocalize  ->  LOADnet3
+
             """ 
             def __init__(self, skip_connections=True, depth=8):
                 super(DLStudio.DetectAndLocalize.LOADnet3, self).__init__()
                 if depth not in [4, 8, 16]:
                     sys.exit("LOADnet2 has been tested for 'depth' for only 4, 8, and 16")
                 self.depth = depth // 4
                 self.conv = nn.Conv2d(3, 64, 3, padding=1)
@@ -4479,158 +4511,152 @@
         This version of DLStudio also comes with a new dataset, PurdueShapes5MultiObject,
         for experimenting with mUnet.  Each image in this dataset contains a random number
         of selections from five different shapes, with the shapes being randomly scaled,
         oriented, and located in each image.  The five different shapes are: rectangle,
         triangle, disk, oval, and star.
 
            Class Path:   DLStudio  ->  SemanticSegmentation
-
         """
         def __init__(self, dl_studio, max_num_objects, dataserver_train=None, dataserver_test=None, dataset_file_train=None, dataset_file_test=None):
             super(DLStudio.SemanticSegmentation, self).__init__()
             self.dl_studio = dl_studio
             self.max_num_objects = max_num_objects
             self.dataserver_train = dataserver_train
             self.dataserver_test = dataserver_test
 
 
         class PurdueShapes5MultiObjectDataset(torch.utils.data.Dataset):
             """
             The very first thing to note is that the images in the dataset
-            PurdueShapes5MultiObjectDataset are of size 64x64.  Each image has a
-            random number (up to five) of the objects drawn from the following five
-            shapes: rectangle, triangle, disk, oval, and star.  Each shape is
-            randomized with respect to all its parameters, including those for its
-            scale and location in the image.
-
-            Each image in the dataset is represented by two data objects, one a list
-            and the other a dictionary. The list data objects consists of the
-            following items:
+            PurdueShapes5MultiObjectDataset are of size 64x64.  Each image has a random
+            number (up to five) of the objects drawn from the following five shapes:
+            rectangle, triangle, disk, oval, and star.  Each shape is randomized with
+            respect to all its parameters, including those for its scale and location in the
+            image.
+
+            Each image in the dataset is represented by two data objects, one a list and the
+            other a dictionary. The list data objects consists of the following items:
 
                 [R, G, B, mask_array, mask_val_to_bbox_map]                                   ## (A)
             
             and the other data object is a dictionary that is set to:
             
                 label_map = {'rectangle':50, 
                              'triangle' :100, 
                              'disk'     :150, 
                              'oval'     :200, 
                              'star'     :250}                                                 ## (B)
             
-            Note that that second data object for each image is the same, as shown
-            above.
+            Note that that second data object for each image is the same, as shown above.
 
-            In the rest of this comment block, I'll explain in greater detail the
-            elements of the list in line (A) above.
+            In the rest of this comment block, I'll explain in greater detail the elements
+            of the list in line (A) above.
 
             
             R,G,B:
             ------
 
-            Each of these is a 4096-element array whose elements store the
-            corresponding color values at each of the 4096 pixels in a 64x64 image.
-            That is, R is a list of 4096 integers, each between 0 and 255, for the
-            value of the red component of the color at each pixel. Similarly, for G
-            and B.
+            Each of these is a 4096-element array whose elements store the corresponding
+            color values at each of the 4096 pixels in a 64x64 image.  That is, R is a list
+            of 4096 integers, each between 0 and 255, for the value of the red component of
+            the color at each pixel. Similarly, for G and B.
             
 
             mask_array:
             ----------
 
-            The fourth item in the list shown in line (A) above is for the mask which is
-            a numpy array of shape:
+            The fourth item in the list shown in line (A) above is for the mask which is a
+            numpy array of shape:
             
                            (5, 64, 64)
             
             It is initialized by the command:
             
                  mask_array = np.zeros((5,64,64), dtype=np.uint8)
             
-            In essence, the mask_array consists of five planes, each of size 64x64.
-            Each plane of the mask array represents an object type according to the
-            following shape_index
+            In essence, the mask_array consists of five planes, each of size 64x64.  Each
+            plane of the mask array represents an object type according to the following
+            shape_index
             
                     shape_index = (label_map[shape] - 50) // 50
             
             where the label_map is as shown in line (B) above.  In other words, the
             shape_index values for the different shapes are:
             
                      rectangle:  0
                       triangle:  1
                           disk:  2
                           oval:  3
                           star:  4
             
-            Therefore, the first layer (of index 0) of the mask is where the pixel
-            values of 50 are stored at all those pixels that belong to the rectangle
-            shapes.  Similarly, the second mask layer (of index 1) is where the pixel
-            values of 100 are stored at all those pixel coordinates that belong to
-            the triangle shapes in an image; and so on.
+            Therefore, the first layer (of index 0) of the mask is where the pixel values of
+            50 are stored at all those pixels that belong to the rectangle shapes.
+            Similarly, the second mask layer (of index 1) is where the pixel values of 100
+            are stored at all those pixel coordinates that belong to the triangle shapes in
+            an image; and so on.
             
-            It is in the manner described above that we define five different masks
-            for an image in the dataset.  Each mask is for a different shape and the
-            pixel values at the nonzero pixels in each mask layer are keyed to the
-            shapes also.
+            It is in the manner described above that we define five different masks for an
+            image in the dataset.  Each mask is for a different shape and the pixel values
+            at the nonzero pixels in each mask layer are keyed to the shapes also.
             
-            A reader is likely to wonder as to the need for this redundancy in the
-            dataset representation of the shapes in each image.  Such a reader is
-            likely to ask: Why can't we just use the binary values 1s and 0s in each
-            mask layer where the corresponding pixels are in the image?  Setting
-            these mask values to 50, 100, etc., was done merely for convenience.  I
-            went with the intuition that the learning needed for multi-object
-            segmentation would become easier if each shape was represented by a
-            different pixels value in the corresponding mask. So I went ahead
-            incorporated that in the dataset generation program itself.
-
-            The mask values for the shapes are not to be confused with the actual RGB
-            values of the pixels that belong to the shapes. The RGB values at the
-            pixels in a shape are randomly generated.  Yes, all the pixels in a shape
-            instance in an image have the same RGB values (but that value has nothing
-            to do with the values given to the mask pixels for that shape).
+            A reader is likely to wonder as to the need for this redundancy in the dataset
+            representation of the shapes in each image.  Such a reader is likely to ask: Why
+            can't we just use the binary values 1s and 0s in each mask layer where the
+            corresponding pixels are in the image?  Setting these mask values to 50, 100,
+            etc., was done merely for convenience.  I went with the intuition that the
+            learning needed for multi-object segmentation would become easier if each shape
+            was represented by a different pixels value in the corresponding mask. So I went
+            ahead incorporated that in the dataset generation program itself.
+
+            The mask values for the shapes are not to be confused with the actual RGB values
+            of the pixels that belong to the shapes. The RGB values at the pixels in a shape
+            are randomly generated.  Yes, all the pixels in a shape instance in an image
+            have the same RGB values (but that value has nothing to do with the values given
+            to the mask pixels for that shape).
             
             
             mask_val_to_bbox_map:
             --------------------
                    
-            The fifth item in the list in line (A) above is a dictionary that tells us
-            what bounding-box rectangle to associate with each shape in the image.  To
-            illustrate what this dictionary looks like, assume that an image contains
-            only one rectangle and only one disk, the dictionary in this case will look
-            like:
+            The fifth item in the list in line (A) above is a dictionary that tells us what
+            bounding-box rectangle to associate with each shape in the image.  To illustrate
+            what this dictionary looks like, assume that an image contains only one
+            rectangle and only one disk, the dictionary in this case will look like:
             
                 mask values to bbox mappings:  {200: [], 
                                                 250: [], 
                                                 100: [], 
                                                  50: [[56, 20, 63, 25]], 
                                                 150: [[37, 41, 55, 59]]}
             
-            Should there happen to be two rectangles in the same image, the dictionary
-            would then be like:
+            Should there happen to be two rectangles in the same image, the dictionary would
+            then be like:
             
                 mask values to bbox mappings:  {200: [], 
                                                 250: [], 
                                                 100: [], 
                                                  50: [[56, 20, 63, 25], [18, 16, 32, 36]], 
                                                 150: [[37, 41, 55, 59]]}
             
-            Therefore, it is not a problem even if all the objects in an image are of
-            the same type.  Remember, the object that are selected for an image are
-            shown randomly from the different shapes.  By the way, an entry like '[56,
-            20, 63, 25]' for the bounding box means that the upper-left corner of the
-            BBox for the 'rectangle' shape is at (56,20) and the lower-right corner of
-            the same is at the pixel coordinates (63,25).
+            Therefore, it is not a problem even if all the objects in an image are of the
+            same type.  Remember, the object that are selected for an image are shown
+            randomly from the different shapes.  By the way, an entry like '[56, 20, 63,
+            25]' for the bounding box means that the upper-left corner of the BBox for the
+            'rectangle' shape is at (56,20) and the lower-right corner of the same is at the
+            pixel coordinates (63,25).
             
             As far as the BBox quadruples are concerned, in the definition
             
                     [min_x,min_y,max_x,max_y]
             
             note that x is the horizontal coordinate, increasing to the right on your
             screen, and y is the vertical coordinate increasing downwards.
 
             Class Path:   DLStudio  ->  SemanticSegmentation  ->  PurdueShapes5MultiObjectDataset
+
             """
             def __init__(self, dl_studio, segmenter, train_or_test, dataset_file):
                 super(DLStudio.SemanticSegmentation.PurdueShapes5MultiObjectDataset, self).__init__()
                 max_num_objects = segmenter.max_num_objects
                 if train_or_test == 'train' and dataset_file == "PurdueShapes5MultiObject-10000-train.gz":
                     if os.path.exists("torch_saved_PurdueShapes5MultiObject-10000_dataset.pt") and \
                               os.path.exists("torch_saved_PurdueShapes5MultiObject_label_map.pt"):
@@ -5224,26 +5250,26 @@
             def init_hidden(self):
                 hidden = torch.zeros(1, self.hidden_size)
                 return hidden
 
 
         class TEXTnetOrder2(nn.Module):
             """
-            In this variant of the TEXTnet network, the value of hidden as used at
-            each time step also includes its value at the previous time step.  This 
-            fact, not directly apparent by the definition of the class shown below, 
-            is made possible by the last parameter, cell, in the header of forward().  
-            All you can see here, at the end of forward(), is that the value of cell 
-            goes through a linear layer and through a sigmoid nonlinearity. By the way, 
-            since the sigmoid saturates at 0 and 1, it can act like a switch. Later 
-            when I use this class in the training function, you will see the cell
-            values being used in such a manner that the hidden state at each time
-            step is mixed with the hidden state at the previous time step.
+            In this variant of the TEXTnet network, the value of hidden as used at each
+            time step also includes its value at the previous time step.  This fact, not
+            directly apparent by the definition of the class shown below, is made possible
+            by the last parameter, cell, in the header of forward().  As you can see below,
+            at the end of forward(), the value of the cell goes through a linear layer
+            and through a sigmoid nonlinearity. By the way, since the sigmoid saturates at 0
+            and 1, it can act like a switch. Later when I use this class in the training
+            function, you will see the cell values being used in such a manner that the
+            hidden state at each time step is mixed with the hidden state at the previous
+            time step, but only to the extent allowed by the switching action of the Sigmoid.
 
-            Class Path:  DLStudio -> TextClassification -> EXTnetOrder2
+            Class Path:  DLStudio -> TextClassification -> TEXTnetOrder2
             """
             def __init__(self, input_size, hidden_size, output_size):
                 super(DLStudio.TextClassification.TEXTnetOrder2, self).__init__()
                 self.input_size = input_size
                 self.hidden_size = hidden_size
                 self.output_size = output_size
                 self.combined_to_hidden = nn.Linear(input_size + 2*hidden_size, hidden_size)
@@ -5334,15 +5360,16 @@
                     input = torch.zeros(1,review_tensor.shape[2])
                     input = input.to(self.dl_studio.device)
                     for k in range(review_tensor.shape[1]):
                         input[0,:] = review_tensor[0,k]
                         output, hidden = net(input, hidden)
                     loss = criterion(output, torch.argmax(sentiment,1))
                     running_loss += loss.item()
-                    loss.backward(retain_graph=True)        
+#                    loss.backward(retain_graph=True)        
+                    loss.backward()        
                     optimizer.step()
                     if i % 200 == 199:    
                         avg_loss = running_loss / float(200)
                         training_loss_tally.append(avg_loss)
                         current_time = time.perf_counter()
                         time_elapsed = current_time-start_time
                         print("[epoch:%d  iter:%4d  elapsed_time: %4d secs]     loss: %.5f" % (epoch+1,i+1, time_elapsed,avg_loss))
```

### Comparing `DLStudio-2.4.3/DLStudio/__init__.py` & `DLStudio-2.4.8/DLStudio/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/DLStudio-2.4.3.html` & `DLStudio-2.4.8/DLStudio-2.4.8.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
 <html>
 <head>
 <title>
-DLStudio-2.4.3.html
+DLStudio-2.4.8.html
 </title>
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
 <style type="text/css">
 p.morelinespace {
     line-height: 130%;
     font-weight: bold;
 }
@@ -21,32 +21,32 @@
 </style>
 </head>
 
 <body>  
 <hr class="myhr1">
 <div style="color:blue; font-size:300%">  
   <strong>DLStudio</strong></div>
-<div style="color:blue; font-size:150%"> Version 2.4.3, &nbsp; 2024-March-23<br>
+<div style="color:blue; font-size:150%"> Version 2.4.8, &nbsp; 2024-April-27<br>
 <font="-1">A software platform for teaching the Deep Learning class at Purdue University</font><br>
 </div>
 <hr class="myhr1">
 <br>
 <div style="font-size:125%; line-height:130%; font-weight: bold">
 DLStudio.py<br>
-Version:&nbsp;&nbsp;2.4.3<br>
+Version:&nbsp;&nbsp;2.4.8<br>
 Author:&nbsp;&nbsp;Avinash&nbsp;Kak&nbsp;(kak@purdue.edu)<br>
-Date:&nbsp;&nbsp;2024-March-23<br>
+Date:&nbsp;&nbsp;2024-April-27<br>
 </div>
 <br>
 <table>
 <tr>
 <th style="text-align:left vertical-align:top">
 <div style="font-size:125%">
-<b>Download Version 2.4.3:</b>&nbsp;&nbsp;&nbsp;&nbsp;    
-<a HREF="https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.tar.gz?download">gztar</a> 
+<b>Download Version 2.4.8:</b>&nbsp;&nbsp;&nbsp;&nbsp;    
+<a HREF="https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.tar.gz?download">gztar</a> 
 </div>
 <br>
 <br>
 <br>
 </th>
 <td style="text-align:center vertical-align:top padding:0">
 <div style="text-align:center">
@@ -74,27 +74,27 @@
 </div>
 </div>
 </td>
 </tr>
 <tr>
 <td>
 <div style="color:red">
-<a HREF="DLStudio-2.4.3_CodeOnly.html">View the main module code file in your browser</a> 
+<a HREF="DLStudio-2.4.8_CodeOnly.html">View the main module code file in your browser</a> 
 &nbsp;<br>
-<a HREF="AdversarialLearning-2.4.3_CodeOnly.html">View the Adversarial Learning code file in your browser</a>&nbsp;
+<a HREF="AdversarialLearning-2.4.8_CodeOnly.html">View the Adversarial Learning code file in your browser</a>&nbsp;
 &nbsp;<br>
-<a HREF="Seq2SeqLearning-2.4.3_CodeOnly.html">View the Seq2Seq Learning code file in your browser</a>
+<a HREF="Seq2SeqLearning-2.4.8_CodeOnly.html">View the Seq2Seq Learning code file in your browser</a>
 &nbsp;<br>
-<a HREF="DataPrediction-2.4.3_CodeOnly.html">View the Data Prediction code file in your browser</a>&nbsp;
+<a HREF="DataPrediction-2.4.8_CodeOnly.html">View the Data Prediction code file in your browser</a>&nbsp;
 &nbsp;<br>
-<a HREF="Transformers-2.4.3_CodeOnly.html">View the Transformers code file in your browser</a>&nbsp;
+<a HREF="Transformers-2.4.8_CodeOnly.html">View the Transformers code file in your browser</a>&nbsp;
 &nbsp;<br>
-<a HREF="MetricLearning-2.4.3_CodeOnly.html">View the Metric Learning code file in your browser</a>&nbsp;
+<a HREF="MetricLearning-2.4.8_CodeOnly.html">View the Metric Learning code file in your browser</a>&nbsp;
 &nbsp;<br>
-<a HREF="GenerativeDiffusion-2.4.3_CodeOnly.html">View the Generative Diffusion code file in your browser</a>&nbsp;<br> 
+<a HREF="GenerativeDiffusion-2.4.8_CodeOnly.html">View the Generative Diffusion code file in your browser</a>&nbsp;<br> 
 &nbsp;<br>
 <a HREF="datasets_for_DLStudio.tar.gz">Download the image datasets for the main DLStudio module</a> 
 &nbsp;<br>
 <a HREF="datasets_for_AdversarialNetworks.tar.gz">Download the image datasets for adversarial learning and diffusion</a> 
 &nbsp;<br>
 <a HREF="text_datasets_for_DLStudio.tar.gz">Download the datasets for text classification</a> 
 &nbsp;<br>
@@ -113,31 +113,40 @@
 <br>
 <br>
 <span style="color:red; font-size:150%"><strong>CONTENTS:</strong></span>
 <br>
 <br>
 <div style="font-size:100%; line-height:180%; font-weight: bold">
 
-
 <a href=#100>CHANGE&nbsp;LOG</a><br><a href=#101>INTRODUCTION</a><br><a href=#102>&nbsp;&nbsp;&nbsp;&nbsp;SKIP&nbsp;CONNECTIONS</a><br><a href=#103>&nbsp;&nbsp;&nbsp;&nbsp;OBJECT&nbsp;DETECTION&nbsp;AND&nbsp;LOCALIZATION</a><br><a href=#104>&nbsp;&nbsp;&nbsp;&nbsp;NOISY&nbsp;OBJECT&nbsp;DETECTION&nbsp;AND&nbsp;LOCALIZATION</a><br><a href=#105>&nbsp;&nbsp;&nbsp;&nbsp;IoU&nbsp;REGRESSION&nbsp;FOR&nbsp;OBJECT&nbsp;DETECTION&nbsp;AND&nbsp;LOCALIZATION</a><br><a href=#106>&nbsp;&nbsp;&nbsp;&nbsp;SEMANTIC&nbsp;SEGMENTATION</a><br><a href=#107>&nbsp;&nbsp;&nbsp;&nbsp;TEXT&nbsp;CLASSIFICATION</a><br><a href=#108>&nbsp;&nbsp;&nbsp;&nbsp;DATA&nbsp;MODELING&nbsp;WITH&nbsp;ADVERSARIAL&nbsp;LEARNING</a><br><a href=#109>&nbsp;&nbsp;&nbsp;&nbsp;DATA&nbsp;MODELING&nbsp;WITH&nbsp;DIFFUSION</a><br><a href=#110>&nbsp;&nbsp;&nbsp;&nbsp;SEQUENCE-TO-SEQUENCE&nbsp;LEARNING&nbsp;WITH&nbsp;ATTENTION</a><br><a href=#111>&nbsp;&nbsp;&nbsp;&nbsp;DATA&nbsp;PREDICTION</a><br><a href=#112>&nbsp;&nbsp;&nbsp;&nbsp;TRANSFORMERS</a><br><a href=#113>&nbsp;&nbsp;&nbsp;&nbsp;METRIC&nbsp;LEARNING</a><br><a href=#114>INSTALLATION</a><br><a href=#115>USAGE</a><br><a href=#116>CONSTRUCTOR&nbsp;PARAMETERS</a><br><a href=#117>PUBLIC&nbsp;METHODS</a><br><a href=#118>THE&nbsp;MAIN&nbsp;INNER&nbsp;CLASSES&nbsp;OF&nbsp;THE&nbsp;DLStudio&nbsp;CLASS</a><br><a href=#119>CO-CLASSES&nbsp;IN&nbsp;THE&nbsp;DLStudio&nbsp;PLATFORM</a><br><a href=#120>Examples&nbsp;DIRECTORY</a><br><a href=#121>ExamplesAdversarialLearning&nbsp;DIRECTORY</a><br><a href=#122>ExamplesDiffusion&nbsp;DIRECTORY</a><br><a href=#123>ExamplesSeq2SeqLearning&nbsp;DIRECTORY</a><br><a href=#124>ExamplesDataPrediction&nbsp;DIRECTORY</a><br><a href=#125>ExamplesTransformers&nbsp;DIRECTORY</a><br><a href=#126>ExamplesMetricLearning&nbsp;DIRECTORY</a><br><a href=#127>THE&nbsp;DATASETS&nbsp;INCLUDED</a><br><a href=#128>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;THE&nbsp;MAIN&nbsp;DLStudio&nbsp;MODULE</a><br><a href=#129>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;Seq2Seq&nbsp;LEARNING</a><br><a href=#130>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;ADVERSARIAL&nbsp;LEARNING&nbsp;AND&nbsp;DIFFUSION</a><br><a href=#131>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;DATA&nbsp;PREDICTION</a><br><a href=#132>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;TRANSFORMERS</a><br><a href=#133>BUGS</a><br><a href=#134>ACKNOWLEDGMENTS</a><br><a href=#135>ABOUT&nbsp;THE&nbsp;AUTHOR</a><br><a href=#136>COPYRIGHT</a><br><br></div>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong><a id="100">CHANGE LOG</a></strong></span><br>&nbsp;<br>
+&nbsp;&nbsp;Version&nbsp;2.4.8:<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;In&nbsp;this&nbsp;version,&nbsp;I&nbsp;have&nbsp;made&nbsp;two&nbsp;important&nbsp;changes&nbsp;to&nbsp;the&nbsp;Transformers&nbsp;module<br>
+&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;DLStudio:&nbsp;(1)&nbsp;The&nbsp;Transformers&nbsp;module&nbsp;now&nbsp;includes&nbsp;a&nbsp;new&nbsp;class&nbsp;that&nbsp;I&nbsp;have<br>
+&nbsp;&nbsp;&nbsp;&nbsp;named&nbsp;visTransformer&nbsp;that&nbsp;works&nbsp;like&nbsp;the&nbsp;famous&nbsp;Vision&nbsp;Transformer&nbsp;(ViT)<br>
+&nbsp;&nbsp;&nbsp;&nbsp;proposed&nbsp;by&nbsp;Dosovitskiy&nbsp;et&nbsp;al.&nbsp;And&nbsp;(2)&nbsp;I&nbsp;have&nbsp;made&nbsp;changes&nbsp;to&nbsp;the&nbsp;QKV&nbsp;code&nbsp;for<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;calculation&nbsp;of&nbsp;self&nbsp;and&nbsp;cross&nbsp;attention&nbsp;in&nbsp;all&nbsp;of&nbsp;the&nbsp;Transformer&nbsp;classes<br>
+&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;module.&nbsp;The&nbsp;attention&nbsp;calculations&nbsp;should&nbsp;now&nbsp;execute&nbsp;faster,&nbsp;which&nbsp;is<br>
+&nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;very&nbsp;important&nbsp;consideration&nbsp;in&nbsp;any&nbsp;transformer&nbsp;based&nbsp;learning.<br>
+&nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.4.3:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;diffusion&nbsp;modeling&nbsp;part&nbsp;of&nbsp;the&nbsp;code&nbsp;should&nbsp;now&nbsp;accept&nbsp;training&nbsp;images&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;any&nbsp;size.&nbsp;&nbsp;Previously&nbsp;it&nbsp;was&nbsp;limited&nbsp;to&nbsp;images&nbsp;of&nbsp;size&nbsp;64x64.&nbsp;&nbsp;Note&nbsp;that&nbsp;this<br>
 &nbsp;&nbsp;&nbsp;&nbsp;change&nbsp;is&nbsp;not&nbsp;as&nbsp;significant&nbsp;as&nbsp;you&nbsp;might&nbsp;think&nbsp;because,&nbsp;under&nbsp;the&nbsp;hood,&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;actual&nbsp;input&nbsp;image&nbsp;size&nbsp;is&nbsp;changed&nbsp;to&nbsp;the&nbsp;size&nbsp;64x64&nbsp;for&nbsp;diffusion&nbsp;modeling.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;So&nbsp;this&nbsp;change&nbsp;is&nbsp;more&nbsp;for&nbsp;your&nbsp;convenience&nbsp;than&nbsp;anything&nbsp;else.&nbsp;&nbsp;I&nbsp;have&nbsp;also<br>
 &nbsp;&nbsp;&nbsp;&nbsp;improved&nbsp;the&nbsp;image&nbsp;visualization&nbsp;code&nbsp;in&nbsp;the&nbsp;ExamplesDiffusion&nbsp;directory.&nbsp;The<br>
 &nbsp;&nbsp;&nbsp;&nbsp;new&nbsp;implementation&nbsp;of&nbsp;the&nbsp;script&nbsp;VisualizeSamples.py&nbsp;automatically&nbsp;generates&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;collage&nbsp;of&nbsp;the&nbsp;images&nbsp;generated&nbsp;from&nbsp;noise&nbsp;by&nbsp;the&nbsp;script<br>
-&nbsp;&nbsp;&nbsp;&nbsp;GenerateNewImageSamples.py.&nbsp;&nbsp;Other&nbsp;changes&nbsp;include&nbsp;a&nbsp;minor&nbsp;clean-up&nbsp;of&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;main&nbsp;doc&nbsp;page&nbsp;for&nbsp;GenerativeDiffusion&nbsp;module&nbsp;and&nbsp;of&nbsp;a&nbsp;couple&nbsp;of&nbsp;the&nbsp;functions<br>
-&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;module.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;GenerateNewImageSamples.py.&nbsp;&nbsp;Other&nbsp;changes&nbsp;include&nbsp;minor&nbsp;clean-up&nbsp;of&nbsp;the&nbsp;main<br>
+&nbsp;&nbsp;&nbsp;&nbsp;doc&nbsp;page&nbsp;for&nbsp;GenerativeDiffusion&nbsp;module&nbsp;and&nbsp;of&nbsp;a&nbsp;couple&nbsp;of&nbsp;the&nbsp;functions&nbsp;in<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;module.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.4.2:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;DLStudio&nbsp;now&nbsp;includes&nbsp;a&nbsp;new&nbsp;module&nbsp;devoted&nbsp;to&nbsp;data&nbsp;modeling&nbsp;with&nbsp;diffusion.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;module,&nbsp;named&nbsp;GenerativeDiffusion,&nbsp;is&nbsp;a&nbsp;co-class&nbsp;of&nbsp;DLStudio.&nbsp;&nbsp;That&nbsp;is,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;GenerativeDiffusion&nbsp;resides&nbsp;at&nbsp;the&nbsp;same&nbsp;level&nbsp;of&nbsp;software&nbsp;abstraction&nbsp;as&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;main&nbsp;DLStudio&nbsp;class&nbsp;in&nbsp;the&nbsp;platform.&nbsp;&nbsp;See&nbsp;the&nbsp;README&nbsp;in&nbsp;the&nbsp;new<br>
@@ -1077,54 +1086,73 @@
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Before&nbsp;you&nbsp;can&nbsp;run&nbsp;this&nbsp;script,&nbsp;you&nbsp;would&nbsp;need&nbsp;to&nbsp;download&nbsp;the&nbsp;training<br>
 &nbsp;&nbsp;&nbsp;&nbsp;dataset&nbsp;used&nbsp;in&nbsp;this&nbsp;example.&nbsp;&nbsp;See&nbsp;the&nbsp;"For&nbsp;Data&nbsp;Prediction"&nbsp;part&nbsp;of&nbsp;the&nbsp;"The<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Datasets&nbsp;Included"&nbsp;section&nbsp;of&nbsp;the&nbsp;doc&nbsp;page&nbsp;for&nbsp;that.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:blue; font-size:100%"><strong>&nbsp;&nbsp;<a id="112">    TRANSFORMERS</a></strong></span><br>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;goal&nbsp;of&nbsp;Transformer&nbsp;based&nbsp;learning&nbsp;is&nbsp;the&nbsp;same&nbsp;that&nbsp;of&nbsp;Seq2SeqLearning<br>
-&nbsp;&nbsp;&nbsp;&nbsp;described&nbsp;earlier&nbsp;in&nbsp;this&nbsp;Introduction&nbsp;except&nbsp;that&nbsp;now&nbsp;you&nbsp;completely&nbsp;forgo<br>
-&nbsp;&nbsp;&nbsp;&nbsp;recurrence.&nbsp;That&nbsp;is,&nbsp;you&nbsp;only&nbsp;use&nbsp;the&nbsp;mechanism&nbsp;of&nbsp;attention&nbsp;to&nbsp;translate<br>
-&nbsp;&nbsp;&nbsp;&nbsp;sentences&nbsp;from&nbsp;a&nbsp;source&nbsp;language&nbsp;into&nbsp;sentences&nbsp;in&nbsp;the&nbsp;target&nbsp;language.&nbsp;For<br>
-&nbsp;&nbsp;&nbsp;&nbsp;such&nbsp;applications,&nbsp;you&nbsp;need&nbsp;two&nbsp;forms&nbsp;of&nbsp;attention:&nbsp;self-attention&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;cross-attention.&nbsp;&nbsp;Self-attention&nbsp;refers&nbsp;to&nbsp;the&nbsp;intra-sentence&nbsp;relationships<br>
-&nbsp;&nbsp;&nbsp;&nbsp;between&nbsp;the&nbsp;words&nbsp;and&nbsp;cross-attention&nbsp;refers&nbsp;to&nbsp;the&nbsp;inter-sentence<br>
-&nbsp;&nbsp;&nbsp;&nbsp;relationships&nbsp;between&nbsp;the&nbsp;words&nbsp;in&nbsp;a&nbsp;pair&nbsp;of&nbsp;sentences,&nbsp;one&nbsp;in&nbsp;the&nbsp;source<br>
-&nbsp;&nbsp;&nbsp;&nbsp;language&nbsp;and&nbsp;the&nbsp;other&nbsp;in&nbsp;the&nbsp;target&nbsp;language.&nbsp;I&nbsp;have&nbsp;explained&nbsp;these&nbsp;concepts<br>
-&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;great&nbsp;detail&nbsp;in&nbsp;the&nbsp;doc&nbsp;sections&nbsp;of&nbsp;the&nbsp;inner&nbsp;classes&nbsp;in&nbsp;the&nbsp;Transformers<br>
-&nbsp;&nbsp;&nbsp;&nbsp;class.&nbsp;&nbsp;In&nbsp;particular,&nbsp;I&nbsp;have&nbsp;explained&nbsp;the&nbsp;concept&nbsp;of&nbsp;the&nbsp;"dot-product"<br>
-&nbsp;&nbsp;&nbsp;&nbsp;attention&nbsp;in&nbsp;which&nbsp;each&nbsp;word&nbsp;puts&nbsp;out&nbsp;three&nbsp;things:&nbsp;a&nbsp;Query&nbsp;Vector&nbsp;Q,&nbsp;a&nbsp;Key<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Vector&nbsp;K,&nbsp;and&nbsp;a&nbsp;Value&nbsp;Vector&nbsp;V.&nbsp;By&nbsp;taking&nbsp;the&nbsp;dot-product&nbsp;of&nbsp;the&nbsp;Query&nbsp;Vector<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Q&nbsp;of&nbsp;a&nbsp;word&nbsp;with&nbsp;the&nbsp;Key&nbsp;Vector&nbsp;K&nbsp;for&nbsp;all&nbsp;the&nbsp;words&nbsp;in&nbsp;a&nbsp;sentence,&nbsp;the&nbsp;neural<br>
-&nbsp;&nbsp;&nbsp;&nbsp;network&nbsp;gets&nbsp;a&nbsp;measure&nbsp;of&nbsp;the&nbsp;extent&nbsp;to&nbsp;which&nbsp;each&nbsp;word&nbsp;in&nbsp;a&nbsp;sentence&nbsp;is<br>
-&nbsp;&nbsp;&nbsp;&nbsp;important&nbsp;to&nbsp;every&nbsp;other&nbsp;word.&nbsp;&nbsp;These&nbsp;dot-product&nbsp;values&nbsp;are&nbsp;then&nbsp;used&nbsp;as<br>
-&nbsp;&nbsp;&nbsp;&nbsp;weights&nbsp;on&nbsp;the&nbsp;Value&nbsp;Vectors,&nbsp;V,&nbsp;for&nbsp;the&nbsp;individual&nbsp;words.&nbsp;&nbsp;Cross&nbsp;attention<br>
-&nbsp;&nbsp;&nbsp;&nbsp;works&nbsp;in&nbsp;a&nbsp;similar&nbsp;manner,&nbsp;except&nbsp;that&nbsp;now&nbsp;you&nbsp;take&nbsp;the&nbsp;dot-products&nbsp;of&nbsp;the&nbsp;Q<br>
-&nbsp;&nbsp;&nbsp;&nbsp;vectors&nbsp;in&nbsp;the&nbsp;target-language&nbsp;sentence&nbsp;with&nbsp;the&nbsp;K&nbsp;vectors&nbsp;in&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;For&nbsp;Seq2SeqLearning&nbsp;learning,&nbsp;the&nbsp;goal&nbsp;of&nbsp;a&nbsp;Transformer&nbsp;based&nbsp;implementation<br>
+&nbsp;&nbsp;&nbsp;&nbsp;is&nbsp;the&nbsp;same&nbsp;as&nbsp;described&nbsp;earlier&nbsp;in&nbsp;this&nbsp;Introduction&nbsp;except&nbsp;that&nbsp;now&nbsp;you<br>
+&nbsp;&nbsp;&nbsp;&nbsp;completely&nbsp;forgo&nbsp;recurrence.&nbsp;That&nbsp;is,&nbsp;you&nbsp;only&nbsp;use&nbsp;the&nbsp;mechanism&nbsp;of&nbsp;attention<br>
+&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;translate&nbsp;sentences&nbsp;from&nbsp;a&nbsp;source&nbsp;language&nbsp;into&nbsp;sentences&nbsp;in&nbsp;the&nbsp;target<br>
+&nbsp;&nbsp;&nbsp;&nbsp;language.&nbsp;For&nbsp;such&nbsp;applications,&nbsp;you&nbsp;need&nbsp;two&nbsp;forms&nbsp;of&nbsp;attention:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;self-attention&nbsp;and&nbsp;cross-attention.&nbsp;&nbsp;Self-attention&nbsp;refers&nbsp;to&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;intra-sentence&nbsp;relationships&nbsp;between&nbsp;the&nbsp;words&nbsp;and&nbsp;cross-attention&nbsp;refers&nbsp;to<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;inter-sentence&nbsp;relationships&nbsp;between&nbsp;the&nbsp;words&nbsp;in&nbsp;a&nbsp;pair&nbsp;of&nbsp;sentences,&nbsp;one<br>
+&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;source&nbsp;language&nbsp;and&nbsp;the&nbsp;other&nbsp;in&nbsp;the&nbsp;target&nbsp;language.&nbsp;I&nbsp;have&nbsp;explained<br>
+&nbsp;&nbsp;&nbsp;&nbsp;these&nbsp;concepts&nbsp;in&nbsp;great&nbsp;detail&nbsp;in&nbsp;the&nbsp;doc&nbsp;sections&nbsp;of&nbsp;the&nbsp;inner&nbsp;classes&nbsp;in&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Transformers&nbsp;class.&nbsp;&nbsp;In&nbsp;particular,&nbsp;I&nbsp;have&nbsp;explained&nbsp;the&nbsp;concept&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;"dot-product"&nbsp;attention&nbsp;in&nbsp;which&nbsp;each&nbsp;word&nbsp;puts&nbsp;out&nbsp;three&nbsp;things:&nbsp;a&nbsp;Query<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Vector&nbsp;Q,&nbsp;a&nbsp;Key&nbsp;Vector&nbsp;K,&nbsp;and&nbsp;a&nbsp;Value&nbsp;Vector&nbsp;V.&nbsp;By&nbsp;taking&nbsp;the&nbsp;dot-product&nbsp;of<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;Query&nbsp;Vector&nbsp;Q&nbsp;of&nbsp;a&nbsp;word&nbsp;with&nbsp;the&nbsp;Key&nbsp;Vector&nbsp;K&nbsp;for&nbsp;all&nbsp;the&nbsp;words&nbsp;in&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;sentence,&nbsp;the&nbsp;neural&nbsp;network&nbsp;gets&nbsp;a&nbsp;measure&nbsp;of&nbsp;the&nbsp;extent&nbsp;to&nbsp;which&nbsp;each&nbsp;word<br>
+&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;a&nbsp;sentence&nbsp;is&nbsp;important&nbsp;to&nbsp;every&nbsp;other&nbsp;word.&nbsp;&nbsp;These&nbsp;dot-product&nbsp;values&nbsp;are<br>
+&nbsp;&nbsp;&nbsp;&nbsp;then&nbsp;used&nbsp;as&nbsp;weights&nbsp;on&nbsp;the&nbsp;Value&nbsp;Vectors,&nbsp;V,&nbsp;for&nbsp;the&nbsp;individual&nbsp;words.&nbsp;&nbsp;Cross<br>
+&nbsp;&nbsp;&nbsp;&nbsp;attention&nbsp;works&nbsp;in&nbsp;a&nbsp;similar&nbsp;manner,&nbsp;except&nbsp;that&nbsp;now&nbsp;you&nbsp;take&nbsp;the&nbsp;dot-products<br>
+&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;the&nbsp;Q&nbsp;vectors&nbsp;in&nbsp;the&nbsp;target-language&nbsp;sentence&nbsp;with&nbsp;the&nbsp;K&nbsp;vectors&nbsp;in&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;corresponding&nbsp;source-language&nbsp;sentence&nbsp;for&nbsp;producing&nbsp;the&nbsp;weight&nbsp;vectors&nbsp;that<br>
 &nbsp;&nbsp;&nbsp;&nbsp;tell&nbsp;us&nbsp;how&nbsp;to&nbsp;weight&nbsp;the&nbsp;source-language&nbsp;Value&nbsp;Vectors&nbsp;vis-a-vis&nbsp;the&nbsp;words&nbsp;in<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;target&nbsp;language.<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;You&nbsp;will&nbsp;see&nbsp;two&nbsp;different&nbsp;implementations&nbsp;of&nbsp;the&nbsp;transformer&nbsp;architecture&nbsp;in<br>
+&nbsp;&nbsp;&nbsp;&nbsp;In&nbsp;addition&nbsp;to&nbsp;their&nbsp;use&nbsp;in&nbsp;Seq2SeqLearning&nbsp;learning,&nbsp;transformers&nbsp;are&nbsp;now<br>
+&nbsp;&nbsp;&nbsp;&nbsp;also&nbsp;used&nbsp;widely&nbsp;in&nbsp;computer&nbsp;vision&nbsp;applications.&nbsp;As&nbsp;a&nbsp;nod&nbsp;to&nbsp;their&nbsp;adoption<br>
+&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;learning&nbsp;required&nbsp;for&nbsp;solving&nbsp;CV&nbsp;problems,&nbsp;I&nbsp;have&nbsp;created&nbsp;a&nbsp;new&nbsp;class<br>
+&nbsp;&nbsp;&nbsp;&nbsp;named&nbsp;visTransformer&nbsp;in&nbsp;the&nbsp;Transformers&nbsp;module&nbsp;of&nbsp;DLStudio.&nbsp;&nbsp;The&nbsp;transformer<br>
+&nbsp;&nbsp;&nbsp;&nbsp;part&nbsp;of&nbsp;the&nbsp;logic&nbsp;in&nbsp;a&nbsp;visTransformer&nbsp;is&nbsp;identical&nbsp;to&nbsp;what&nbsp;it&nbsp;is&nbsp;in&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;transformer&nbsp;class&nbsp;for&nbsp;Seq2SeqLearning&nbsp;learning.&nbsp;&nbsp;That&nbsp;logic&nbsp;kicks&nbsp;in&nbsp;after&nbsp;you<br>
+&nbsp;&nbsp;&nbsp;&nbsp;have&nbsp;divided&nbsp;an&nbsp;image&nbsp;into&nbsp;patches&nbsp;and&nbsp;you&nbsp;represent&nbsp;each&nbsp;patch&nbsp;by&nbsp;an<br>
+&nbsp;&nbsp;&nbsp;&nbsp;embedding&nbsp;vector&nbsp;---&nbsp;in&nbsp;exactly&nbsp;the&nbsp;same&nbsp;as&nbsp;when&nbsp;you&nbsp;represent&nbsp;a&nbsp;word&nbsp;or&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;token&nbsp;in&nbsp;a&nbsp;sentence&nbsp;by&nbsp;an&nbsp;embedding&nbsp;vector.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;You&nbsp;will&nbsp;see&nbsp;three&nbsp;different&nbsp;implementations&nbsp;of&nbsp;the&nbsp;transformer&nbsp;architecture&nbsp;in<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;Transformers&nbsp;co-class&nbsp;of&nbsp;DLStudio:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TransformerFG<br>
-&nbsp;&nbsp;&nbsp;&nbsp;and<br>
+&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TransformerPreLN<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;the&nbsp;"FG"&nbsp;suffix&nbsp;standing&nbsp;for&nbsp;"First&nbsp;Generation"&nbsp;and&nbsp;the&nbsp;"PreLN"&nbsp;suffix<br>
-&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;"Pre&nbsp;LayerNorm".&nbsp;TransformerFG&nbsp;is&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;transformer<br>
-&nbsp;&nbsp;&nbsp;&nbsp;architecture&nbsp;proposed&nbsp;in&nbsp;the&nbsp;famous&nbsp;paper&nbsp;by&nbsp;Vaswani&nbsp;et&nbsp;al.&nbsp;&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;TransformerPreLN&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;same&nbsp;architecture&nbsp;but&nbsp;with&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;modification&nbsp;suggested&nbsp;by&nbsp;Xiong&nbsp;et&nbsp;al.&nbsp;for&nbsp;more&nbsp;stable&nbsp;learning.&nbsp;&nbsp;Since,&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;modification&nbsp;is&nbsp;small&nbsp;from&nbsp;an&nbsp;architectural&nbsp;standpoint,&nbsp;I&nbsp;could&nbsp;have&nbsp;combined<br>
-&nbsp;&nbsp;&nbsp;&nbsp;both&nbsp;transformer&nbsp;types&nbsp;in&nbsp;the&nbsp;same&nbsp;implementation&nbsp;with&nbsp;some&nbsp;conditional&nbsp;logic<br>
-&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;account&nbsp;for&nbsp;the&nbsp;differences.&nbsp;&nbsp;However,&nbsp;I&nbsp;have&nbsp;chosen&nbsp;to&nbsp;keep&nbsp;them&nbsp;separate<br>
-&nbsp;&nbsp;&nbsp;&nbsp;mostly&nbsp;for&nbsp;educational&nbsp;purposes.&nbsp;&nbsp;Further&nbsp;details&nbsp;on&nbsp;these&nbsp;implementations&nbsp;are<br>
-&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;documentation&nbsp;blocks&nbsp;in&nbsp;the&nbsp;Transformers&nbsp;co-class.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;visTransformer<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;"FG"&nbsp;suffix&nbsp;TransformerFG&nbsp;stands&nbsp;for&nbsp;"First&nbsp;Generation";&nbsp;the&nbsp;"PreLN"<br>
+&nbsp;&nbsp;&nbsp;&nbsp;suffix&nbsp;in&nbsp;TransformerPreLN&nbsp;for&nbsp;"Pre&nbsp;LayerNorm";&nbsp;and,&nbsp;finally,&nbsp;the&nbsp;name<br>
+&nbsp;&nbsp;&nbsp;&nbsp;visTransformer&nbsp;stands&nbsp;for&nbsp;"Vision&nbsp;Transformer."&nbsp;&nbsp;<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;TransformerFG&nbsp;is&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;transformer&nbsp;architecture&nbsp;proposed&nbsp;in<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;famous&nbsp;paper&nbsp;by&nbsp;Vaswani&nbsp;et&nbsp;al.&nbsp;&nbsp;and&nbsp;TransformerPreLN&nbsp;my&nbsp;implementation&nbsp;of<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;same&nbsp;architecture&nbsp;but&nbsp;with&nbsp;the&nbsp;modification&nbsp;suggested&nbsp;by&nbsp;Xiong&nbsp;et&nbsp;al.&nbsp;for<br>
+&nbsp;&nbsp;&nbsp;&nbsp;more&nbsp;stable&nbsp;learning.&nbsp;&nbsp;Since,&nbsp;the&nbsp;modification&nbsp;is&nbsp;small&nbsp;from&nbsp;an&nbsp;architectural<br>
+&nbsp;&nbsp;&nbsp;&nbsp;standpoint,&nbsp;I&nbsp;could&nbsp;have&nbsp;combined&nbsp;both&nbsp;transformer&nbsp;types&nbsp;in&nbsp;the&nbsp;same<br>
+&nbsp;&nbsp;&nbsp;&nbsp;implementation&nbsp;with&nbsp;some&nbsp;conditional&nbsp;logic&nbsp;to&nbsp;account&nbsp;for&nbsp;the&nbsp;differences.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;However,&nbsp;I&nbsp;have&nbsp;chosen&nbsp;to&nbsp;keep&nbsp;them&nbsp;separate&nbsp;mostly&nbsp;for&nbsp;educational&nbsp;purposes.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Further&nbsp;details&nbsp;on&nbsp;these&nbsp;implementations&nbsp;are&nbsp;in&nbsp;the&nbsp;documentation&nbsp;blocks&nbsp;in<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;Transformers&nbsp;co-class.&nbsp;&nbsp;<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;visTransformer&nbsp;implementation&nbsp;is&nbsp;based&nbsp;on&nbsp;the&nbsp;paper&nbsp;"An&nbsp;Image&nbsp;is&nbsp;Worth<br>
+&nbsp;&nbsp;&nbsp;&nbsp;16x16&nbsp;Words:&nbsp;Transformers&nbsp;for&nbsp;Image&nbsp;Recognition&nbsp;at&nbsp;Scale''&nbsp;by&nbsp;Dosovitskiy&nbsp;et<br>
+&nbsp;&nbsp;&nbsp;&nbsp;al.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;want&nbsp;to&nbsp;use&nbsp;my&nbsp;code&nbsp;for&nbsp;learning&nbsp;the&nbsp;main&nbsp;ideas&nbsp;related&nbsp;to&nbsp;how&nbsp;to<br>
 &nbsp;&nbsp;&nbsp;&nbsp;create&nbsp;purely&nbsp;attention&nbsp;based&nbsp;networks,&nbsp;your&nbsp;starting&nbsp;point&nbsp;for&nbsp;that&nbsp;should&nbsp;be<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;following&nbsp;scripts&nbsp;in&nbsp;the&nbsp;ExamplesTransformers&nbsp;directory&nbsp;of&nbsp;the&nbsp;DLStudio<br>
 &nbsp;&nbsp;&nbsp;&nbsp;distribution:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;seq2seq_with_transformerFG.py<br>
@@ -1136,14 +1164,24 @@
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;contains&nbsp;90,000&nbsp;pairs&nbsp;of&nbsp;English-Spanish&nbsp;sentences&nbsp;with&nbsp;the&nbsp;maximum<br>
 &nbsp;&nbsp;&nbsp;&nbsp;number&nbsp;of&nbsp;words&nbsp;in&nbsp;each&nbsp;sentence&nbsp;limited&nbsp;to&nbsp;8&nbsp;words.&nbsp;&nbsp;For&nbsp;processing&nbsp;by&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;attention&nbsp;networks,&nbsp;each&nbsp;sentence&nbsp;is&nbsp;enclosed&nbsp;in&nbsp;&lt;SOS&gt;&nbsp;and&nbsp;&lt;EOS&gt;&nbsp;tokens,&nbsp;with<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;former&nbsp;standing&nbsp;for&nbsp;"Start&nbsp;of&nbsp;Sentence"&nbsp;and&nbsp;the&nbsp;latter&nbsp;for&nbsp;"End&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Sentence".<br>
 &nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;And&nbsp;if&nbsp;you&nbsp;wish&nbsp;to&nbsp;use&nbsp;visTransformer&nbsp;for&nbsp;solving&nbsp;image&nbsp;recognition&nbsp;problems<br>
+&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;a&nbsp;transformer&nbsp;based&nbsp;implementation,&nbsp;your&nbsp;starting&nbsp;point&nbsp;should&nbsp;be<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;following&nbsp;scripts&nbsp;in&nbsp;the&nbsp;same&nbsp;ExamplesTransformers&nbsp;directory&nbsp;that&nbsp;was<br>
+&nbsp;&nbsp;&nbsp;&nbsp;mentioned&nbsp;above:<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image_recog_with_visTransformer.py<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;test_checkpoint_for_visTransformer.py&nbsp;<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Both&nbsp;these&nbsp;script&nbsp;use&nbsp;the&nbsp;CIFAR10&nbsp;dataset&nbsp;for&nbsp;demonstrating&nbsp;image&nbsp;recognition.<br>
+&nbsp;<br>
 &nbsp;<br>
 <span style="color:blue; font-size:100%"><strong>&nbsp;&nbsp;<a id="113">    METRIC LEARNING</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;main&nbsp;idea&nbsp;of&nbsp;metric&nbsp;learning&nbsp;is&nbsp;to&nbsp;learn&nbsp;a&nbsp;mapping&nbsp;from&nbsp;the&nbsp;images&nbsp;to<br>
 &nbsp;&nbsp;&nbsp;&nbsp;their&nbsp;embedding&nbsp;vector&nbsp;representations&nbsp;in&nbsp;such&nbsp;a&nbsp;way&nbsp;that&nbsp;the&nbsp;embeddings&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;what&nbsp;are&nbsp;supposed&nbsp;to&nbsp;be&nbsp;similar&nbsp;images&nbsp;are&nbsp;pulled&nbsp;together&nbsp;and&nbsp;those&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;dissimilar&nbsp;images&nbsp;are&nbsp;pulled&nbsp;as&nbsp;far&nbsp;apart&nbsp;as&nbsp;possible.&nbsp;&nbsp;After&nbsp;such&nbsp;a&nbsp;mapping<br>
 &nbsp;&nbsp;&nbsp;&nbsp;function&nbsp;is&nbsp;learned,&nbsp;you&nbsp;can&nbsp;take&nbsp;a&nbsp;query&nbsp;image&nbsp;(whose&nbsp;class&nbsp;label&nbsp;is&nbsp;not<br>
@@ -1704,35 +1742,43 @@
 &nbsp;&nbsp;&nbsp;&nbsp;training&nbsp;dataset&nbsp;used&nbsp;in&nbsp;this&nbsp;example.&nbsp;&nbsp;See&nbsp;the&nbsp;"For&nbsp;Data&nbsp;Prediction"&nbsp;part&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;"The&nbsp;Datasets&nbsp;Included"&nbsp;section&nbsp;of&nbsp;the&nbsp;doc&nbsp;page&nbsp;for&nbsp;that.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong>    </strong></span><br>&nbsp;&nbsp;&nbsp;&nbsp;Transformers<br>
 &nbsp;&nbsp;&nbsp;&nbsp;============<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;code&nbsp;in&nbsp;this&nbsp;co-class&nbsp;of&nbsp;DLStudio&nbsp;consists&nbsp;two&nbsp;slightly&nbsp;different<br>
-&nbsp;&nbsp;&nbsp;&nbsp;implementations&nbsp;of&nbsp;the&nbsp;transformer&nbsp;architecture:&nbsp;TransformerFG&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;TransformerPreLN.&nbsp;&nbsp;TransformerFG&nbsp;is&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;architecture&nbsp;as<br>
-&nbsp;&nbsp;&nbsp;&nbsp;conceptualized&nbsp;in&nbsp;the&nbsp;famous&nbsp;paper&nbsp;"Attention&nbsp;is&nbsp;All&nbsp;You&nbsp;Need"&nbsp;by&nbsp;Vaswani&nbsp;et<br>
-&nbsp;&nbsp;&nbsp;&nbsp;el.&nbsp;&nbsp;And&nbsp;TransformerPreLN&nbsp;is&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;original&nbsp;idea&nbsp;along&nbsp;with<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;modifications&nbsp;suggested&nbsp;by&nbsp;Xiong&nbsp;et&nbsp;al.&nbsp;in&nbsp;their&nbsp;paper&nbsp;"On&nbsp;Layer<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Normalization&nbsp;in&nbsp;the&nbsp;Transformer&nbsp;Architecture"&nbsp;for&nbsp;more&nbsp;stable&nbsp;learning.&nbsp;&nbsp;The<br>
-&nbsp;&nbsp;&nbsp;&nbsp;two&nbsp;versions&nbsp;of&nbsp;transformers&nbsp;differ&nbsp;in&nbsp;only&nbsp;one&nbsp;respect:&nbsp;The&nbsp;placement&nbsp;of&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;LayerNorm&nbsp;in&nbsp;relation&nbsp;to&nbsp;the&nbsp;architectural&nbsp;components&nbsp;related&nbsp;to&nbsp;attention&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;feedforward&nbsp;network.&nbsp;&nbsp;Literally,&nbsp;the&nbsp;difference&nbsp;is&nbsp;small,&nbsp;yet&nbsp;its<br>
-&nbsp;&nbsp;&nbsp;&nbsp;consequences&nbsp;on&nbsp;the&nbsp;stability&nbsp;of&nbsp;learning&nbsp;significant.<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;fundamentals&nbsp;of&nbsp;how&nbsp;the&nbsp;attention&nbsp;works&nbsp;in&nbsp;both&nbsp;TransformerFG&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;TransformerPreLN&nbsp;are&nbsp;exactly&nbsp;the&nbsp;same.&nbsp;&nbsp;For&nbsp;self-attention,&nbsp;you&nbsp;associate&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Query&nbsp;Vector&nbsp;Q_i&nbsp;and&nbsp;a&nbsp;Key&nbsp;Vector&nbsp;K_i&nbsp;with&nbsp;each&nbsp;word&nbsp;w_i&nbsp;in&nbsp;a&nbsp;sentence.&nbsp;&nbsp;For&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;given&nbsp;w_i,&nbsp;the&nbsp;dot&nbsp;product&nbsp;of&nbsp;its&nbsp;Q_i&nbsp;with&nbsp;the&nbsp;K_j&nbsp;vectors&nbsp;for&nbsp;all&nbsp;the&nbsp;other<br>
-&nbsp;&nbsp;&nbsp;&nbsp;words&nbsp;w_j&nbsp;is&nbsp;a&nbsp;measure&nbsp;of&nbsp;how&nbsp;related&nbsp;w_i&nbsp;is&nbsp;to&nbsp;each&nbsp;w_j&nbsp;with&nbsp;regard&nbsp;to&nbsp;what's<br>
-&nbsp;&nbsp;&nbsp;&nbsp;needed&nbsp;for&nbsp;the&nbsp;translation&nbsp;of&nbsp;a&nbsp;source&nbsp;sentence&nbsp;into&nbsp;the&nbsp;target&nbsp;sentence.&nbsp;&nbsp;One<br>
-&nbsp;&nbsp;&nbsp;&nbsp;more&nbsp;vector&nbsp;you&nbsp;associate&nbsp;with&nbsp;each&nbsp;word&nbsp;w_i&nbsp;is&nbsp;the&nbsp;Value&nbsp;Vector&nbsp;V_i.&nbsp;&nbsp;The<br>
-&nbsp;&nbsp;&nbsp;&nbsp;value&nbsp;vectors&nbsp;for&nbsp;the&nbsp;words&nbsp;in&nbsp;a&nbsp;sentence&nbsp;are&nbsp;weighted&nbsp;by&nbsp;the&nbsp;output&nbsp;of&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;activation&nbsp;nn.LogSoftmax&nbsp;applied&nbsp;to&nbsp;the&nbsp;dot-products.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;code&nbsp;in&nbsp;this&nbsp;module&nbsp;of&nbsp;DLStudio&nbsp;consists&nbsp;of&nbsp;three&nbsp;different<br>
+&nbsp;&nbsp;&nbsp;&nbsp;implementations&nbsp;of&nbsp;the&nbsp;transformer&nbsp;architecture:&nbsp;(1)&nbsp;TransformerFG,&nbsp;(2)<br>
+&nbsp;&nbsp;&nbsp;&nbsp;TransformerPreLN,&nbsp;and&nbsp;(3)&nbsp;visTransformer.&nbsp;&nbsp;The&nbsp;first&nbsp;two&nbsp;of&nbsp;these&nbsp;are&nbsp;meant<br>
+&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;seq2seq&nbsp;learning,&nbsp;as&nbsp;in&nbsp;language&nbsp;translation,&nbsp;and&nbsp;the&nbsp;last&nbsp;is&nbsp;for&nbsp;solving<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;problem&nbsp;of&nbsp;image&nbsp;recognition.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;TransformerFG&nbsp;is&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;architecture&nbsp;as&nbsp;conceptualized&nbsp;in<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;famous&nbsp;paper&nbsp;"Attention&nbsp;is&nbsp;All&nbsp;You&nbsp;Need"&nbsp;by&nbsp;Vaswani&nbsp;et&nbsp;el.&nbsp;&nbsp;And<br>
+&nbsp;&nbsp;&nbsp;&nbsp;TransformerPreLN&nbsp;is&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;original&nbsp;idea&nbsp;along&nbsp;with&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;modifications&nbsp;suggested&nbsp;by&nbsp;Xiong&nbsp;et&nbsp;al.&nbsp;in&nbsp;their&nbsp;paper&nbsp;"On&nbsp;Layer&nbsp;Normalization<br>
+&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;Transformer&nbsp;Architecture"&nbsp;for&nbsp;more&nbsp;stable&nbsp;learning.&nbsp;&nbsp;The&nbsp;two&nbsp;versions<br>
+&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;transformers&nbsp;differ&nbsp;in&nbsp;only&nbsp;one&nbsp;respect:&nbsp;The&nbsp;placement&nbsp;of&nbsp;the&nbsp;LayerNorm&nbsp;in<br>
+&nbsp;&nbsp;&nbsp;&nbsp;relation&nbsp;to&nbsp;the&nbsp;architectural&nbsp;components&nbsp;related&nbsp;to&nbsp;attention&nbsp;and&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;feedforward&nbsp;network.&nbsp;&nbsp;Literally,&nbsp;the&nbsp;difference&nbsp;is&nbsp;small,&nbsp;yet&nbsp;its&nbsp;consequences<br>
+&nbsp;&nbsp;&nbsp;&nbsp;are&nbsp;significant&nbsp;regarding&nbsp;the&nbsp;stability&nbsp;of&nbsp;learning.&nbsp;&nbsp;Finally,&nbsp;visTransformer<br>
+&nbsp;&nbsp;&nbsp;&nbsp;is&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;Vision&nbsp;Transformer&nbsp;as&nbsp;presented&nbsp;in&nbsp;the&nbsp;famou&nbsp;paper<br>
+&nbsp;&nbsp;&nbsp;&nbsp;"An&nbsp;Image&nbsp;is&nbsp;Worth&nbsp;16x16$&nbsp;Words:&nbsp;Transformers&nbsp;for&nbsp;Image&nbsp;Recognition&nbsp;at&nbsp;Scale''<br>
+&nbsp;&nbsp;&nbsp;&nbsp;by&nbsp;Dosovitskiy&nbsp;et&nbsp;al.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;fundamentals&nbsp;of&nbsp;how&nbsp;the&nbsp;attention&nbsp;works&nbsp;in&nbsp;all&nbsp;three&nbsp;transformer&nbsp;based<br>
+&nbsp;&nbsp;&nbsp;&nbsp;implementations&nbsp;in&nbsp;the&nbsp;Transformers&nbsp;module&nbsp;are&nbsp;exactly&nbsp;the&nbsp;same.&nbsp;&nbsp;For<br>
+&nbsp;&nbsp;&nbsp;&nbsp;self-attention,&nbsp;you&nbsp;associate&nbsp;a&nbsp;Query&nbsp;Vector&nbsp;Q_i&nbsp;and&nbsp;a&nbsp;Key&nbsp;Vector&nbsp;K_i&nbsp;with<br>
+&nbsp;&nbsp;&nbsp;&nbsp;each&nbsp;word&nbsp;w_i&nbsp;in&nbsp;a&nbsp;sentence.&nbsp;&nbsp;For&nbsp;a&nbsp;given&nbsp;w_i,&nbsp;the&nbsp;dot&nbsp;product&nbsp;of&nbsp;its&nbsp;Q_i&nbsp;with<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;K_j&nbsp;vectors&nbsp;for&nbsp;all&nbsp;the&nbsp;other&nbsp;words&nbsp;w_j&nbsp;is&nbsp;a&nbsp;measure&nbsp;of&nbsp;how&nbsp;related&nbsp;w_i&nbsp;is<br>
+&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;each&nbsp;w_j&nbsp;with&nbsp;regard&nbsp;to&nbsp;what's&nbsp;needed&nbsp;for&nbsp;the&nbsp;translation&nbsp;of&nbsp;a&nbsp;source<br>
+&nbsp;&nbsp;&nbsp;&nbsp;sentence&nbsp;into&nbsp;the&nbsp;target&nbsp;sentence.&nbsp;&nbsp;One&nbsp;more&nbsp;vector&nbsp;you&nbsp;associate&nbsp;with&nbsp;each<br>
+&nbsp;&nbsp;&nbsp;&nbsp;word&nbsp;w_i&nbsp;is&nbsp;the&nbsp;Value&nbsp;Vector&nbsp;V_i.&nbsp;&nbsp;The&nbsp;value&nbsp;vectors&nbsp;for&nbsp;the&nbsp;words&nbsp;in&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;sentence&nbsp;are&nbsp;weighted&nbsp;by&nbsp;the&nbsp;output&nbsp;of&nbsp;the&nbsp;activation&nbsp;nn.LogSoftmax&nbsp;applied&nbsp;to<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;dot-products.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;self-attention&nbsp;mechanism&nbsp;described&nbsp;above&nbsp;is&nbsp;half&nbsp;of&nbsp;what&nbsp;goes&nbsp;into&nbsp;each<br>
 &nbsp;&nbsp;&nbsp;&nbsp;base&nbsp;encoder&nbsp;of&nbsp;a&nbsp;transformer,&nbsp;the&nbsp;other&nbsp;half&nbsp;is&nbsp;a&nbsp;feedforward&nbsp;network<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(FFN).&nbsp;The&nbsp;overall&nbsp;encoder&nbsp;consists&nbsp;of&nbsp;a&nbsp;cascade&nbsp;of&nbsp;these&nbsp;base&nbsp;encoders.&nbsp;&nbsp;In<br>
 &nbsp;&nbsp;&nbsp;&nbsp;my&nbsp;implementation,&nbsp;I&nbsp;have&nbsp;referred&nbsp;to&nbsp;the&nbsp;overall&nbsp;encoder&nbsp;as&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;MasterEncoder.&nbsp;&nbsp;The&nbsp;MasterDecoder&nbsp;also&nbsp;consists&nbsp;of&nbsp;a&nbsp;cascade&nbsp;of&nbsp;base&nbsp;decoders.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;A&nbsp;base&nbsp;decoder&nbsp;is&nbsp;similar&nbsp;to&nbsp;a&nbsp;base&nbsp;encoder&nbsp;except&nbsp;for&nbsp;there&nbsp;being&nbsp;a&nbsp;layer&nbsp;of<br>
@@ -1752,24 +1798,32 @@
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;self-attention&nbsp;layer&nbsp;and&nbsp;residual&nbsp;connection&nbsp;wraps&nbsp;around&nbsp;both.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Similarly,&nbsp;LayerNorm&nbsp;is&nbsp;applied&nbsp;to&nbsp;the&nbsp;input&nbsp;to&nbsp;FFN&nbsp;and&nbsp;the&nbsp;residual<br>
 &nbsp;&nbsp;&nbsp;&nbsp;connection&nbsp;wraps&nbsp;around&nbsp;both.&nbsp;&nbsp;Similar&nbsp;considerations&nbsp;applied&nbsp;to&nbsp;the&nbsp;decoder<br>
 &nbsp;&nbsp;&nbsp;&nbsp;side,&nbsp;except&nbsp;we&nbsp;now&nbsp;also&nbsp;have&nbsp;a&nbsp;layer&nbsp;of&nbsp;cross-attention&nbsp;interposed&nbsp;between<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;self-attention&nbsp;and&nbsp;FFN.<br>
 &nbsp;&nbsp;&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;As&nbsp;I&nbsp;mentioned&nbsp;in&nbsp;the&nbsp;Introduction,&nbsp;your&nbsp;main&nbsp;entry&nbsp;point&nbsp;for&nbsp;experimenting<br>
-&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;the&nbsp;transformer&nbsp;code&nbsp;in&nbsp;DLStudio&nbsp;are&nbsp;the&nbsp;following&nbsp;two&nbsp;scripts&nbsp;in&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;ExamplesTransformers&nbsp;directory&nbsp;of&nbsp;the&nbsp;distribution:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;the&nbsp;seq2seq&nbsp;based&nbsp;transformer&nbsp;code&nbsp;in&nbsp;DLStudio&nbsp;are&nbsp;the&nbsp;following&nbsp;two<br>
+&nbsp;&nbsp;&nbsp;&nbsp;scripts&nbsp;in&nbsp;the&nbsp;ExamplesTransformers&nbsp;directory&nbsp;of&nbsp;the&nbsp;distribution:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;seq2seq_with_transformerFG.py<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;seq2seq_with_transformerPreLN.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;However,&nbsp;before&nbsp;you&nbsp;can&nbsp;run&nbsp;these&nbsp;scripts,&nbsp;you&nbsp;would&nbsp;need&nbsp;to&nbsp;download&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;training&nbsp;dataset&nbsp;used&nbsp;in&nbsp;these&nbsp;examples.&nbsp;&nbsp;See&nbsp;the&nbsp;"For&nbsp;Transformers"&nbsp;part&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;"The&nbsp;Datasets&nbsp;Included"&nbsp;section&nbsp;of&nbsp;this&nbsp;doc&nbsp;page&nbsp;for&nbsp;that.<br>
 &nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;And&nbsp;your&nbsp;main&nbsp;entry&nbsp;point&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;image&nbsp;recognition&nbsp;by&nbsp;playing<br>
+&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;the&nbsp;visTransformer&nbsp;class&nbsp;are&nbsp;the&nbsp;scripts:<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image_recog_with_visTransformer.py<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;test_checkpoint_for_visTransformer.py&nbsp;<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Both&nbsp;these&nbsp;script&nbsp;use&nbsp;the&nbsp;CIFAR10&nbsp;dataset&nbsp;for&nbsp;demonstrating&nbsp;image&nbsp;recognition.<br>
+&nbsp;<br>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong>    </strong></span><br>&nbsp;&nbsp;&nbsp;&nbsp;MetricLearning:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;===================<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;As&nbsp;mentioned&nbsp;in&nbsp;the&nbsp;Introduction,&nbsp;the&nbsp;main&nbsp;idea&nbsp;of&nbsp;metric&nbsp;learning&nbsp;is&nbsp;to&nbsp;learn<br>
 &nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;mapping&nbsp;from&nbsp;the&nbsp;images&nbsp;to&nbsp;their&nbsp;embedding&nbsp;vector&nbsp;representations&nbsp;in&nbsp;such&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;way&nbsp;that&nbsp;the&nbsp;embeddings&nbsp;for&nbsp;what&nbsp;are&nbsp;supposed&nbsp;to&nbsp;be&nbsp;similar&nbsp;images&nbsp;are&nbsp;pulled<br>
@@ -2073,38 +2127,28 @@
 &nbsp;&nbsp;&nbsp;&nbsp;hourly&nbsp;electric&nbsp;load&nbsp;recordings&nbsp;made&nbsp;available&nbsp;by&nbsp;several&nbsp;utilities&nbsp;in&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;east&nbsp;and&nbsp;the&nbsp;midwest&nbsp;of&nbsp;the&nbsp;United&nbsp;States.&nbsp;&nbsp;You&nbsp;can&nbsp;download&nbsp;this&nbsp;dataset&nbsp;from<br>
 &nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;link&nbsp;at&nbsp;the&nbsp;top&nbsp;of&nbsp;the&nbsp;main&nbsp;DLStudio&nbsp;doc&nbsp;page.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong><a id="125">ExamplesTransformers DIRECTORY</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;ExamplesTransformers&nbsp;directory&nbsp;of&nbsp;the&nbsp;distribution&nbsp;contains&nbsp;the&nbsp;following<br>
-&nbsp;&nbsp;&nbsp;&nbsp;two&nbsp;scripts&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;transformers:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;four&nbsp;scripts&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;transformers&nbsp;in&nbsp;DLStudio:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;seq2seq_with_transformerFG.py&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;seq2seq_with_transformerPreLN.py&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Both&nbsp;these&nbsp;scripts&nbsp;deal&nbsp;with&nbsp;English-to-Spanish&nbsp;translation&nbsp;in&nbsp;a&nbsp;manner<br>
-&nbsp;&nbsp;&nbsp;&nbsp;similar&nbsp;to&nbsp;what's&nbsp;demonstrated&nbsp;by&nbsp;the&nbsp;code&nbsp;in&nbsp;the&nbsp;Seq2SeqLearning&nbsp;co-class&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;example&nbsp;scripts&nbsp;associated&nbsp;with&nbsp;that&nbsp;co-class.<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;directory&nbsp;also&nbsp;contains&nbsp;the&nbsp;following&nbsp;two&nbsp;scripts<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image_recog_with_visTransformer.py<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;test_checkpoint_for_visTransformer.py&nbsp;<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;test_checkpointFG.py<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;test_checkpointPreLN.py<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;address&nbsp;the&nbsp;problems&nbsp;of&nbsp;training&nbsp;a&nbsp;transformer&nbsp;network.&nbsp;&nbsp;As&nbsp;I&nbsp;have<br>
-&nbsp;&nbsp;&nbsp;&nbsp;mentioned&nbsp;elsewhere&nbsp;in&nbsp;this&nbsp;documentation,&nbsp;transformer&nbsp;training&nbsp;can&nbsp;be<br>
-&nbsp;&nbsp;&nbsp;&nbsp;frustrating,&nbsp;to&nbsp;say&nbsp;the&nbsp;least,&nbsp;and&nbsp;can&nbsp;take&nbsp;a&nbsp;very&nbsp;long&nbsp;time.&nbsp;&nbsp;What<br>
-&nbsp;&nbsp;&nbsp;&nbsp;exacerbates&nbsp;the&nbsp;frustrations&nbsp;is&nbsp;that,&nbsp;with&nbsp;a&nbsp;wrong&nbsp;choice&nbsp;for&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;hyperparameters,&nbsp;you&nbsp;could&nbsp;end&nbsp;with&nbsp;model&nbsp;divergence&nbsp;in&nbsp;the&nbsp;middle&nbsp;of&nbsp;training<br>
-&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;not&nbsp;know&nbsp;about&nbsp;it&nbsp;until&nbsp;the&nbsp;end.&nbsp;&nbsp;[Model&nbsp;divergence&nbsp;is&nbsp;akin&nbsp;to&nbsp;mode<br>
-&nbsp;&nbsp;&nbsp;&nbsp;collapse&nbsp;in&nbsp;training&nbsp;a&nbsp;GAN.]&nbsp;&nbsp;To&nbsp;deal&nbsp;with&nbsp;these&nbsp;problems,&nbsp;starting&nbsp;with<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Version&nbsp;2.2.7,&nbsp;the&nbsp;transformer&nbsp;training&nbsp;routines&nbsp;now&nbsp;create&nbsp;a&nbsp;checkpoint&nbsp;of<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;model&nbsp;every&nbsp;5&nbsp;epochs.&nbsp;While&nbsp;the&nbsp;training&nbsp;is&nbsp;going&nbsp;on,&nbsp;you&nbsp;can&nbsp;evaluate&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;checkpoints&nbsp;in&nbsp;the&nbsp;manner&nbsp;illustrated&nbsp;by&nbsp;the&nbsp;above&nbsp;two&nbsp;scripts.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;first&nbsp;two&nbsp;scripts&nbsp;deal&nbsp;with&nbsp;English-to-Spanish&nbsp;translation&nbsp;in&nbsp;a&nbsp;manner<br>
+&nbsp;&nbsp;&nbsp;&nbsp;similar&nbsp;to&nbsp;what's&nbsp;demonstrated&nbsp;by&nbsp;the&nbsp;code&nbsp;in&nbsp;the&nbsp;Seq2SeqLearning&nbsp;co-class&nbsp;and<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;example&nbsp;scripts&nbsp;associated&nbsp;with&nbsp;that&nbsp;co-class.&nbsp;The&nbsp;last&nbsp;two&nbsp;relate&nbsp;to&nbsp;my<br>
+&nbsp;&nbsp;&nbsp;&nbsp;demonstration&nbsp;of&nbsp;image&nbsp;recognition&nbsp;with&nbsp;a&nbsp;transformer&nbsp;based&nbsp;implementation.&nbsp;&nbsp;I<br>
+&nbsp;&nbsp;&nbsp;&nbsp;have&nbsp;used&nbsp;the&nbsp;CFAR10&nbsp;dataset&nbsp;for&nbsp;image&nbsp;recognition.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong><a id="126">ExamplesMetricLearning DIRECTORY</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;ExamplesMetricLearning&nbsp;directory&nbsp;at&nbsp;top&nbsp;level&nbsp;of&nbsp;the&nbsp;distribution&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;contains&nbsp;the&nbsp;following&nbsp;scripts:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.&nbsp;&nbsp;example_for_pairwise_contrastive_loss.py<br>
@@ -2317,15 +2361,16 @@
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;That&nbsp;will&nbsp;create&nbsp;data&nbsp;directory&nbsp;named&nbsp;"dataPred"&nbsp;in&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ExamplesDataPrediction&nbsp;directory.&nbsp;&nbsp;With&nbsp;that&nbsp;you&nbsp;should&nbsp;be&nbsp;able&nbsp;to&nbsp;execute<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;data&nbsp;prediction&nbsp;script&nbsp;in&nbsp;that&nbsp;directory.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:blue; font-size:100%"><strong>&nbsp;&nbsp;<a id="132">    FOR TRANSFORMERS</a></strong></span><br>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Download&nbsp;the&nbsp;dataset&nbsp;archive<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;For&nbsp;the&nbsp;seq2seq&nbsp;learning&nbsp;part&nbsp;of&nbsp;the&nbsp;Transformers&nbsp;module&nbsp;in&nbsp;DLStudio,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;download&nbsp;the&nbsp;dataset&nbsp;archive<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;en_es_corpus_for_learning_with_Transformers.tar.gz<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;into&nbsp;the&nbsp;ExamplesTransformers&nbsp;directory&nbsp;of&nbsp;the&nbsp;DLStudio&nbsp;distribution.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Next,&nbsp;execute&nbsp;the&nbsp;following&nbsp;command&nbsp;in&nbsp;that&nbsp;directory:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tar&nbsp;zxvf&nbsp;en_es_corpus_for_learning_with_Transformers.tar.gz<br>
@@ -2538,61 +2583,59 @@
 networks&nbsp;are&nbsp;difficult&nbsp;to&nbsp;train&nbsp;because&nbsp;of&nbsp;the&nbsp;vanishing&nbsp;gradients&nbsp;problem.<br>
 What&nbsp;that&nbsp;means&nbsp;is&nbsp;that&nbsp;as&nbsp;the&nbsp;depth&nbsp;of&nbsp;network&nbsp;increases,&nbsp;the&nbsp;loss&nbsp;gradients<br>
 calculated&nbsp;for&nbsp;the&nbsp;early&nbsp;layers&nbsp;become&nbsp;more&nbsp;and&nbsp;more&nbsp;muted,&nbsp;which&nbsp;suppresses<br>
 the&nbsp;learning&nbsp;of&nbsp;the&nbsp;parameters&nbsp;in&nbsp;those&nbsp;layers.&nbsp;&nbsp;An&nbsp;important&nbsp;mitigation<br>
 strategy&nbsp;for&nbsp;addressing&nbsp;this&nbsp;problem&nbsp;consists&nbsp;of&nbsp;creating&nbsp;a&nbsp;CNN&nbsp;using&nbsp;blocks<br>
 with&nbsp;skip&nbsp;connections.<br>
 &nbsp;<br>
-With&nbsp;the&nbsp;code&nbsp;shown&nbsp;in&nbsp;this&nbsp;inner&nbsp;class&nbsp;of&nbsp;the&nbsp;module,&nbsp;you&nbsp;can&nbsp;now&nbsp;experiment<br>
-with&nbsp;skip&nbsp;connections&nbsp;in&nbsp;a&nbsp;CNN&nbsp;to&nbsp;see&nbsp;how&nbsp;a&nbsp;deep&nbsp;network&nbsp;with&nbsp;this&nbsp;feature<br>
-might&nbsp;improve&nbsp;the&nbsp;classification&nbsp;results.&nbsp;&nbsp;As&nbsp;you&nbsp;will&nbsp;see&nbsp;in&nbsp;the&nbsp;code&nbsp;shown<br>
-below,&nbsp;the&nbsp;network&nbsp;that&nbsp;allows&nbsp;you&nbsp;to&nbsp;construct&nbsp;a&nbsp;CNN&nbsp;with&nbsp;skip&nbsp;connections<br>
-is&nbsp;named&nbsp;BMEnet.&nbsp;&nbsp;As&nbsp;shown&nbsp;in&nbsp;the&nbsp;script&nbsp;playing_with_skip_connections.py&nbsp;in<br>
-the&nbsp;Examples&nbsp;directory&nbsp;of&nbsp;the&nbsp;distribution,&nbsp;you&nbsp;can&nbsp;easily&nbsp;create&nbsp;a&nbsp;CNN&nbsp;with<br>
-arbitrary&nbsp;depth&nbsp;just&nbsp;by&nbsp;using&nbsp;the&nbsp;"depth"&nbsp;constructor&nbsp;option&nbsp;for&nbsp;the&nbsp;BMEnet<br>
-class.&nbsp;&nbsp;The&nbsp;basic&nbsp;block&nbsp;of&nbsp;the&nbsp;network&nbsp;constructed&nbsp;by&nbsp;BMEnet&nbsp;is&nbsp;called<br>
-SkipBlock&nbsp;which,&nbsp;very&nbsp;much&nbsp;like&nbsp;the&nbsp;BasicBlock&nbsp;in&nbsp;ResNet-18,&nbsp;has&nbsp;a&nbsp;couple&nbsp;of<br>
-convolutional&nbsp;layers&nbsp;whose&nbsp;output&nbsp;is&nbsp;combined&nbsp;with&nbsp;the&nbsp;input&nbsp;to&nbsp;the&nbsp;block.<br>
-&nbsp;<br>
-Note&nbsp;that&nbsp;the&nbsp;value&nbsp;given&nbsp;to&nbsp;the&nbsp;"depth"&nbsp;constructor&nbsp;option&nbsp;for&nbsp;the&nbsp;BMEnet<br>
-class&nbsp;does&nbsp;NOT&nbsp;translate&nbsp;directly&nbsp;into&nbsp;the&nbsp;actual&nbsp;depth&nbsp;of&nbsp;the&nbsp;CNN.&nbsp;[Again,<br>
-see&nbsp;the&nbsp;script&nbsp;playing_with_skip_connections.py&nbsp;in&nbsp;the&nbsp;Examples&nbsp;directory&nbsp;for<br>
-how&nbsp;to&nbsp;use&nbsp;this&nbsp;option.]&nbsp;The&nbsp;value&nbsp;of&nbsp;"depth"&nbsp;is&nbsp;translated&nbsp;into&nbsp;how&nbsp;many<br>
-"same&nbsp;input&nbsp;and&nbsp;output&nbsp;channels"&nbsp;and&nbsp;the&nbsp;"same&nbsp;input&nbsp;and&nbsp;output&nbsp;sizes"<br>
-instances&nbsp;of&nbsp;SkipBlock&nbsp;to&nbsp;use&nbsp;between&nbsp;successive&nbsp;instances&nbsp;of&nbsp;downsampling<br>
-and&nbsp;channel-doubling&nbsp;instances&nbsp;of&nbsp;SkipBlock.<br>
+With&nbsp;the&nbsp;code&nbsp;shown&nbsp;in&nbsp;this&nbsp;inner&nbsp;class&nbsp;of&nbsp;the&nbsp;module,&nbsp;you&nbsp;can&nbsp;now&nbsp;experiment&nbsp;with<br>
+skip&nbsp;connections&nbsp;in&nbsp;a&nbsp;CNN&nbsp;to&nbsp;see&nbsp;how&nbsp;a&nbsp;deep&nbsp;network&nbsp;with&nbsp;this&nbsp;feature&nbsp;might&nbsp;improve<br>
+the&nbsp;classification&nbsp;results.&nbsp;&nbsp;As&nbsp;you&nbsp;will&nbsp;see&nbsp;in&nbsp;the&nbsp;code&nbsp;shown&nbsp;below,&nbsp;the&nbsp;network<br>
+that&nbsp;allows&nbsp;you&nbsp;to&nbsp;construct&nbsp;a&nbsp;CNN&nbsp;with&nbsp;skip&nbsp;connections&nbsp;is&nbsp;named&nbsp;BMEnet.&nbsp;&nbsp;As&nbsp;shown<br>
+in&nbsp;the&nbsp;script&nbsp;playing_with_skip_connections.py&nbsp;in&nbsp;the&nbsp;Examples&nbsp;directory&nbsp;of&nbsp;the<br>
+distribution,&nbsp;you&nbsp;can&nbsp;easily&nbsp;create&nbsp;a&nbsp;CNN&nbsp;with&nbsp;arbitrary&nbsp;depth&nbsp;just&nbsp;by&nbsp;using&nbsp;the<br>
+"depth"&nbsp;constructor&nbsp;option&nbsp;for&nbsp;the&nbsp;BMEnet&nbsp;class.&nbsp;&nbsp;The&nbsp;basic&nbsp;block&nbsp;of&nbsp;the&nbsp;network<br>
+constructed&nbsp;by&nbsp;BMEnet&nbsp;is&nbsp;called&nbsp;SkipBlock&nbsp;which,&nbsp;very&nbsp;much&nbsp;like&nbsp;the&nbsp;BasicBlock&nbsp;in<br>
+ResNet-18,&nbsp;has&nbsp;a&nbsp;couple&nbsp;of&nbsp;convolutional&nbsp;layers&nbsp;whose&nbsp;output&nbsp;is&nbsp;combined&nbsp;with&nbsp;the<br>
+input&nbsp;to&nbsp;the&nbsp;block.<br>
+&nbsp;<br>
+Note&nbsp;that&nbsp;the&nbsp;value&nbsp;given&nbsp;to&nbsp;the&nbsp;"depth"&nbsp;constructor&nbsp;option&nbsp;for&nbsp;the&nbsp;BMEnet&nbsp;class<br>
+does&nbsp;NOT&nbsp;translate&nbsp;directly&nbsp;into&nbsp;the&nbsp;actual&nbsp;depth&nbsp;of&nbsp;the&nbsp;CNN.&nbsp;[Again,&nbsp;see&nbsp;the&nbsp;script<br>
+playing_with_skip_connections.py&nbsp;in&nbsp;the&nbsp;Examples&nbsp;directory&nbsp;for&nbsp;how&nbsp;to&nbsp;use&nbsp;this<br>
+option.]&nbsp;The&nbsp;value&nbsp;of&nbsp;"depth"&nbsp;is&nbsp;translated&nbsp;into&nbsp;how&nbsp;many&nbsp;"same&nbsp;input&nbsp;and&nbsp;output<br>
+channels"&nbsp;and&nbsp;the&nbsp;"same&nbsp;input&nbsp;and&nbsp;output&nbsp;sizes"&nbsp;instances&nbsp;of&nbsp;SkipBlock&nbsp;to&nbsp;use<br>
+between&nbsp;successive&nbsp;instances&nbsp;of&nbsp;downsampling&nbsp;and&nbsp;channel-doubling&nbsp;instances&nbsp;of<br>
+SkipBlock.<br>
 &nbsp;<br>
 Class&nbsp;Path:&nbsp;DLStudio&nbsp;-&gt;&nbsp;BMEnet</tt></dl>
 
 <dl><dt><strong>CustomDataLoading</strong> = &lt;class 'DLStudio.DLStudio.CustomDataLoading'&gt;<dd><tt>This&nbsp;is&nbsp;a&nbsp;testbed&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;a&nbsp;completely&nbsp;grounds-up&nbsp;attempt&nbsp;at<br>
-designing&nbsp;a&nbsp;custom&nbsp;data&nbsp;loader.&nbsp;&nbsp;Ordinarily,&nbsp;if&nbsp;the&nbsp;basic&nbsp;format&nbsp;of&nbsp;how&nbsp;the<br>
-dataset&nbsp;is&nbsp;stored&nbsp;is&nbsp;similar&nbsp;to&nbsp;one&nbsp;of&nbsp;the&nbsp;datasets&nbsp;that&nbsp;the&nbsp;Torchvision<br>
-module&nbsp;knows&nbsp;about,&nbsp;you&nbsp;can&nbsp;go&nbsp;ahead&nbsp;and&nbsp;use&nbsp;that&nbsp;for&nbsp;your&nbsp;own&nbsp;dataset.&nbsp;&nbsp;At<br>
-worst,&nbsp;you&nbsp;may&nbsp;need&nbsp;to&nbsp;carry&nbsp;out&nbsp;some&nbsp;light&nbsp;customizations&nbsp;depending&nbsp;on&nbsp;the<br>
-number&nbsp;of&nbsp;classes&nbsp;involved,&nbsp;etc.<br>
-&nbsp;<br>
-However,&nbsp;if&nbsp;the&nbsp;underlying&nbsp;dataset&nbsp;is&nbsp;stored&nbsp;in&nbsp;a&nbsp;manner&nbsp;that&nbsp;does&nbsp;not&nbsp;look<br>
-like&nbsp;anything&nbsp;in&nbsp;Torchvision,&nbsp;you&nbsp;have&nbsp;no&nbsp;choice&nbsp;but&nbsp;to&nbsp;supply&nbsp;yourself&nbsp;all<br>
-of&nbsp;the&nbsp;data&nbsp;loading&nbsp;infrastructure.&nbsp;&nbsp;That&nbsp;is&nbsp;what&nbsp;this&nbsp;inner&nbsp;class&nbsp;of&nbsp;the&nbsp;<br>
-DLStudio&nbsp;module&nbsp;is&nbsp;all&nbsp;about.<br>
-&nbsp;<br>
-The&nbsp;custom&nbsp;data&nbsp;loading&nbsp;exercise&nbsp;here&nbsp;is&nbsp;related&nbsp;to&nbsp;a&nbsp;dataset&nbsp;called<br>
-PurdueShapes5&nbsp;that&nbsp;contains&nbsp;32x32&nbsp;images&nbsp;of&nbsp;binary&nbsp;shapes&nbsp;belonging&nbsp;to&nbsp;the<br>
-following&nbsp;five&nbsp;classes:<br>
+designing&nbsp;a&nbsp;custom&nbsp;data&nbsp;loader.&nbsp;&nbsp;Ordinarily,&nbsp;if&nbsp;the&nbsp;basic&nbsp;format&nbsp;of&nbsp;how&nbsp;the&nbsp;dataset<br>
+is&nbsp;stored&nbsp;is&nbsp;similar&nbsp;to&nbsp;one&nbsp;of&nbsp;the&nbsp;datasets&nbsp;that&nbsp;the&nbsp;Torchvision&nbsp;module&nbsp;knows&nbsp;about,<br>
+you&nbsp;can&nbsp;go&nbsp;ahead&nbsp;and&nbsp;use&nbsp;that&nbsp;for&nbsp;your&nbsp;own&nbsp;dataset.&nbsp;&nbsp;At&nbsp;worst,&nbsp;you&nbsp;may&nbsp;need&nbsp;to&nbsp;carry<br>
+out&nbsp;some&nbsp;light&nbsp;customizations&nbsp;depending&nbsp;on&nbsp;the&nbsp;number&nbsp;of&nbsp;classes&nbsp;involved,&nbsp;etc.<br>
+&nbsp;<br>
+However,&nbsp;if&nbsp;the&nbsp;underlying&nbsp;dataset&nbsp;is&nbsp;stored&nbsp;in&nbsp;a&nbsp;manner&nbsp;that&nbsp;does&nbsp;not&nbsp;look&nbsp;like<br>
+anything&nbsp;in&nbsp;Torchvision,&nbsp;you&nbsp;have&nbsp;no&nbsp;choice&nbsp;but&nbsp;to&nbsp;supply&nbsp;yourself&nbsp;all&nbsp;of&nbsp;the&nbsp;data<br>
+loading&nbsp;infrastructure.&nbsp;&nbsp;That&nbsp;is&nbsp;what&nbsp;this&nbsp;inner&nbsp;class&nbsp;of&nbsp;the&nbsp;DLStudio&nbsp;module&nbsp;is&nbsp;all<br>
+about.<br>
+&nbsp;<br>
+The&nbsp;custom&nbsp;data&nbsp;loading&nbsp;exercise&nbsp;here&nbsp;is&nbsp;related&nbsp;to&nbsp;a&nbsp;dataset&nbsp;called&nbsp;PurdueShapes5<br>
+that&nbsp;contains&nbsp;32x32&nbsp;images&nbsp;of&nbsp;binary&nbsp;shapes&nbsp;belonging&nbsp;to&nbsp;the&nbsp;following&nbsp;five&nbsp;classes:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.&nbsp;&nbsp;rectangle<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.&nbsp;&nbsp;triangle<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.&nbsp;&nbsp;disk<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.&nbsp;&nbsp;oval<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5.&nbsp;&nbsp;star<br>
 &nbsp;<br>
-The&nbsp;dataset&nbsp;was&nbsp;generated&nbsp;by&nbsp;randomizing&nbsp;the&nbsp;sizes&nbsp;and&nbsp;the&nbsp;orientations<br>
-of&nbsp;these&nbsp;five&nbsp;patterns.&nbsp;&nbsp;Since&nbsp;the&nbsp;patterns&nbsp;are&nbsp;rotated&nbsp;with&nbsp;a&nbsp;very&nbsp;simple<br>
-non-interpolating&nbsp;transform,&nbsp;just&nbsp;the&nbsp;act&nbsp;of&nbsp;random&nbsp;rotations&nbsp;can&nbsp;introduce<br>
-boundary&nbsp;and&nbsp;even&nbsp;interior&nbsp;noise&nbsp;in&nbsp;the&nbsp;patterns.<br>
+The&nbsp;dataset&nbsp;was&nbsp;generated&nbsp;by&nbsp;randomizing&nbsp;the&nbsp;sizes&nbsp;and&nbsp;the&nbsp;orientations&nbsp;of&nbsp;these<br>
+five&nbsp;patterns.&nbsp;&nbsp;Since&nbsp;the&nbsp;patterns&nbsp;are&nbsp;rotated&nbsp;with&nbsp;a&nbsp;very&nbsp;simple&nbsp;non-interpolating<br>
+transform,&nbsp;just&nbsp;the&nbsp;act&nbsp;of&nbsp;random&nbsp;rotations&nbsp;can&nbsp;introduce&nbsp;boundary&nbsp;and&nbsp;even&nbsp;interior<br>
+noise&nbsp;in&nbsp;the&nbsp;patterns.<br>
 &nbsp;<br>
 Each&nbsp;32x32&nbsp;image&nbsp;is&nbsp;stored&nbsp;in&nbsp;the&nbsp;dataset&nbsp;as&nbsp;the&nbsp;following&nbsp;list:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[R,&nbsp;G,&nbsp;B,&nbsp;Bbox,&nbsp;Label]<br>
 where<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;R&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:&nbsp;&nbsp;&nbsp;is&nbsp;a&nbsp;1024&nbsp;element&nbsp;list&nbsp;of&nbsp;the&nbsp;values&nbsp;for&nbsp;the&nbsp;red&nbsp;component<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;the&nbsp;color&nbsp;at&nbsp;all&nbsp;the&nbsp;pixels<br>
@@ -2602,49 +2645,49 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;G&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:&nbsp;&nbsp;&nbsp;the&nbsp;same&nbsp;as&nbsp;above&nbsp;but&nbsp;for&nbsp;the&nbsp;blue&nbsp;component&nbsp;of&nbsp;the&nbsp;color<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Bbox&nbsp;&nbsp;:&nbsp;&nbsp;&nbsp;a&nbsp;list&nbsp;like&nbsp;[x1,y1,x2,y2]&nbsp;that&nbsp;defines&nbsp;the&nbsp;bounding&nbsp;box&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;the&nbsp;object&nbsp;in&nbsp;the&nbsp;image<br>
 &nbsp;&nbsp;&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Label&nbsp;:&nbsp;&nbsp;&nbsp;the&nbsp;shape&nbsp;of&nbsp;the&nbsp;object<br>
 &nbsp;<br>
-I&nbsp;serialize&nbsp;the&nbsp;dataset&nbsp;with&nbsp;Python's&nbsp;pickle&nbsp;module&nbsp;and&nbsp;then&nbsp;compress&nbsp;it&nbsp;with&nbsp;<br>
-the&nbsp;gzip&nbsp;module.&nbsp;&nbsp;<br>
+I&nbsp;serialize&nbsp;the&nbsp;dataset&nbsp;with&nbsp;Python's&nbsp;pickle&nbsp;module&nbsp;and&nbsp;then&nbsp;compress&nbsp;it&nbsp;with&nbsp;the<br>
+gzip&nbsp;module.<br>
 &nbsp;<br>
-You&nbsp;will&nbsp;find&nbsp;the&nbsp;following&nbsp;dataset&nbsp;directories&nbsp;in&nbsp;the&nbsp;"data"&nbsp;subdirectory<br>
-of&nbsp;Examples&nbsp;in&nbsp;the&nbsp;DLStudio&nbsp;distro:<br>
+You&nbsp;will&nbsp;find&nbsp;the&nbsp;following&nbsp;dataset&nbsp;directories&nbsp;in&nbsp;the&nbsp;"data"&nbsp;subdirectory&nbsp;of<br>
+Examples&nbsp;in&nbsp;the&nbsp;DLStudio&nbsp;distro:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PurdueShapes5-10000-train.gz<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PurdueShapes5-1000-test.gz<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PurdueShapes5-20-train.gz<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PurdueShapes5-20-test.gz&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
 &nbsp;<br>
-The&nbsp;number&nbsp;that&nbsp;follows&nbsp;the&nbsp;main&nbsp;name&nbsp;string&nbsp;"PurdueShapes5-"&nbsp;is&nbsp;for&nbsp;the&nbsp;<br>
-number&nbsp;of&nbsp;images&nbsp;in&nbsp;the&nbsp;dataset.&nbsp;&nbsp;<br>
+The&nbsp;number&nbsp;that&nbsp;follows&nbsp;the&nbsp;main&nbsp;name&nbsp;string&nbsp;"PurdueShapes5-"&nbsp;is&nbsp;for&nbsp;the&nbsp;number&nbsp;of<br>
+images&nbsp;in&nbsp;the&nbsp;dataset.<br>
 &nbsp;<br>
-You&nbsp;will&nbsp;find&nbsp;the&nbsp;last&nbsp;two&nbsp;datasets,&nbsp;with&nbsp;20&nbsp;images&nbsp;each,&nbsp;useful&nbsp;for&nbsp;debugging<br>
-your&nbsp;logic&nbsp;for&nbsp;object&nbsp;detection&nbsp;and&nbsp;bounding-box&nbsp;regression.<br>
+You&nbsp;will&nbsp;find&nbsp;the&nbsp;last&nbsp;two&nbsp;datasets,&nbsp;with&nbsp;20&nbsp;images&nbsp;each,&nbsp;useful&nbsp;for&nbsp;debugging&nbsp;your<br>
+logic&nbsp;for&nbsp;object&nbsp;detection&nbsp;and&nbsp;bounding-box&nbsp;regression.<br>
 &nbsp;<br>
 Class&nbsp;Path:&nbsp;&nbsp;&nbsp;DLStudio&nbsp;&nbsp;-&gt;&nbsp;&nbsp;CustomDataLoading</tt></dl>
 
 <dl><dt><strong>DetectAndLocalize</strong> = &lt;class 'DLStudio.DLStudio.DetectAndLocalize'&gt;<dd><tt>The&nbsp;purpose&nbsp;of&nbsp;this&nbsp;inner&nbsp;class&nbsp;is&nbsp;to&nbsp;focus&nbsp;on&nbsp;object&nbsp;detection&nbsp;in&nbsp;images&nbsp;---&nbsp;as<br>
-opposed&nbsp;to&nbsp;image&nbsp;classification.&nbsp;&nbsp;Most&nbsp;people&nbsp;would&nbsp;say&nbsp;that&nbsp;object&nbsp;detection<br>
-is&nbsp;a&nbsp;more&nbsp;challenging&nbsp;problem&nbsp;than&nbsp;image&nbsp;classification&nbsp;because,&nbsp;in&nbsp;general,<br>
-the&nbsp;former&nbsp;also&nbsp;requires&nbsp;localization.&nbsp;&nbsp;The&nbsp;simplest&nbsp;interpretation&nbsp;of&nbsp;what<br>
-is&nbsp;meant&nbsp;by&nbsp;localization&nbsp;is&nbsp;that&nbsp;the&nbsp;code&nbsp;that&nbsp;carries&nbsp;out&nbsp;object&nbsp;detection<br>
-must&nbsp;also&nbsp;output&nbsp;a&nbsp;bounding-box&nbsp;rectangle&nbsp;for&nbsp;the&nbsp;object&nbsp;that&nbsp;was&nbsp;detected.<br>
-&nbsp;<br>
-You&nbsp;will&nbsp;find&nbsp;in&nbsp;this&nbsp;inner&nbsp;class&nbsp;some&nbsp;examples&nbsp;of&nbsp;LOADnet&nbsp;classes&nbsp;meant<br>
-for&nbsp;solving&nbsp;the&nbsp;object&nbsp;detection&nbsp;and&nbsp;localization&nbsp;problem.&nbsp;&nbsp;The&nbsp;acronym<br>
-"LOAD"&nbsp;in&nbsp;"LOADnet"&nbsp;stands&nbsp;for<br>
+opposed&nbsp;to&nbsp;image&nbsp;classification.&nbsp;&nbsp;Most&nbsp;people&nbsp;would&nbsp;say&nbsp;that&nbsp;object&nbsp;detection&nbsp;is&nbsp;a<br>
+more&nbsp;challenging&nbsp;problem&nbsp;than&nbsp;image&nbsp;classification&nbsp;because,&nbsp;in&nbsp;general,&nbsp;the&nbsp;former<br>
+also&nbsp;requires&nbsp;localization.&nbsp;&nbsp;The&nbsp;simplest&nbsp;interpretation&nbsp;of&nbsp;what&nbsp;is&nbsp;meant&nbsp;by<br>
+localization&nbsp;is&nbsp;that&nbsp;the&nbsp;code&nbsp;that&nbsp;carries&nbsp;out&nbsp;object&nbsp;detection&nbsp;must&nbsp;also&nbsp;output&nbsp;a<br>
+bounding-box&nbsp;rectangle&nbsp;for&nbsp;the&nbsp;object&nbsp;that&nbsp;was&nbsp;detected.<br>
+&nbsp;<br>
+You&nbsp;will&nbsp;find&nbsp;in&nbsp;this&nbsp;inner&nbsp;class&nbsp;some&nbsp;examples&nbsp;of&nbsp;LOADnet&nbsp;classes&nbsp;meant&nbsp;for&nbsp;solving<br>
+the&nbsp;object&nbsp;detection&nbsp;and&nbsp;localization&nbsp;problem.&nbsp;&nbsp;The&nbsp;acronym&nbsp;"LOAD"&nbsp;in&nbsp;"LOADnet"<br>
+stands&nbsp;for<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"LOcalization&nbsp;And&nbsp;Detection"<br>
 &nbsp;<br>
-The&nbsp;different&nbsp;network&nbsp;examples&nbsp;included&nbsp;here&nbsp;are&nbsp;LOADnet1,&nbsp;LOADnet2,&nbsp;and<br>
-LOADnet3.&nbsp;&nbsp;For&nbsp;now,&nbsp;only&nbsp;pay&nbsp;attention&nbsp;to&nbsp;LOADnet2&nbsp;since&nbsp;that's&nbsp;the&nbsp;class&nbsp;I<br>
-have&nbsp;worked&nbsp;with&nbsp;the&nbsp;most&nbsp;for&nbsp;the&nbsp;1.0.7&nbsp;distribution.<br>
+The&nbsp;different&nbsp;network&nbsp;examples&nbsp;included&nbsp;here&nbsp;are&nbsp;LOADnet1,&nbsp;LOADnet2,&nbsp;and&nbsp;LOADnet3.<br>
+For&nbsp;now,&nbsp;only&nbsp;pay&nbsp;attention&nbsp;to&nbsp;LOADnet2&nbsp;since&nbsp;that's&nbsp;the&nbsp;class&nbsp;I&nbsp;have&nbsp;worked&nbsp;with<br>
+the&nbsp;most&nbsp;for&nbsp;the&nbsp;1.0.7&nbsp;distribution.<br>
 &nbsp;<br>
 Class&nbsp;Path:&nbsp;&nbsp;&nbsp;DLStudio&nbsp;&nbsp;-&gt;&nbsp;&nbsp;DetectAndLocalize</tt></dl>
 
 <dl><dt><strong>ExperimentsWithCIFAR</strong> = &lt;class 'DLStudio.DLStudio.ExperimentsWithCIFAR'&gt;<dd><tt>Class&nbsp;Path:&nbsp;&nbsp;DLStudio&nbsp;&nbsp;-&gt;&nbsp;&nbsp;ExperimentsWithCIFAR</tt></dl>
 
 <dl><dt><strong>ExperimentsWithSequential</strong> = &lt;class 'DLStudio.DLStudio.ExperimentsWithSequential'&gt;<dd><tt>Demonstrates&nbsp;how&nbsp;to&nbsp;use&nbsp;the&nbsp;torch.nn.Sequential&nbsp;container&nbsp;class<br>
 &nbsp;<br>
@@ -2714,17 +2757,18 @@
 <tr bgcolor="#55aa55">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#ffffff" face="helvetica, arial"><big><strong>Data</strong></big></font></td></tr>
     
 <tr><td style="bgcolor:#55aa55;"></td><td>&nbsp;</td>
 <td style="width:100%;"><strong>__author__</strong> = 'Avinash Kak (kak@purdue.edu)'<br>
 <strong>__copyright__</strong> = '(C) 2024 Avinash Kak. Python Software Foundation.'<br>
-<strong>__date__</strong> = '2024-March-23'<br>
-<strong>__url__</strong> = 'https://engineering.purdue.edu/kak/distDT/DLStudio-2.4.3.html'<br>
-<strong>__version__</strong> = '2.4.3'</td></tr></table>
+<strong>__date__</strong> = '2024-April-27'<br>
+<strong>__url__</strong> = 'https://engineering.purdue.edu/kak/distDT/DLStudio-2.4.8.html'<br>
+<strong>__version__</strong> = '2.4.8'</td></tr></table>
 <table style="width:100%; border-collapse:collapse; border-spacking:0; padding:2; border:0;">
 <tr style="bgcolor:#7799ee;">
 <td style="colspan:3; vertical-align:bottom;">&nbsp;<br>
 <span style="color:#ffffff; font-family:helvetica, arial; font-size:large;"><strong>Author</strong></big></span></td></tr>
 <tr><td style="bgcolor:#7799ee;"></td><td>&nbsp;</td>
 <td style="width:100%;">Avinash&nbsp;Kak&nbsp;(kak@purdue.edu)</td></tr></table>
 </body></html>
+
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 ===============================================================================
 DDLLSSttuuddiioo
-Version 2.4.3,   2024-March-23
+Version 2.4.8,   2024-April-27
 "-1">A software platform for teaching the Deep Learning class at Purdue
 University
 
 ===============================================================================
 
 DLStudio.py
-Version:  2.4.3
+Version:  2.4.8
 Author:  Avinash Kak (kak@purdue.edu)
-Date:  2024-March-23
+Date:  2024-April-27
 
                                                  Total number of downloads (all
                                         versions) from this website:
                                         file = fopen("HowManyCounts.txt", "r")
                                         or exit("Unable to open file!"); echo
-DDoowwnnllooaadd VVeerrssiioonn 22..44..33::? ? ? ?  _gg_zz_tt_aa_rr       fgets($file); fclose($file); ?>
+DDoowwnnllooaadd VVeerrssiioonn 22..44..88::? ? ? ?  _gg_zz_tt_aa_rr       fgets($file); fclose($file); ?>
                                                     This count is automatically
                                         updated at every rotation of
                                                   the weblogs (normally once
                                         every two to four days)
                                                   Last updated:
                                         file = fopen("LastUpdated.txt", "r") or
                                         exit("Unable to open file!"); echo
@@ -93,27 +93,40 @@
 _A_C_K_N_O_W_L_E_D_G_M_E_N_T_S
 _A_B_O_U_T_ _T_H_E_ _A_U_T_H_O_R
 _C_O_P_Y_R_I_G_H_T
 
  
 CCHHAANNGGEE LLOOGG
  
+  Version 2.4.8:
+ 
+    In this version, I have made two important changes to the Transformers module
+    in DLStudio: 
+(1) The Transformers module now includes a new class that I have
+    named visTransformer that works like the famous Vision Transformer (ViT)
+    proposed by Dosovitskiy et al. And 
+(2) I have made changes to the QKV code for
+    the calculation of self and cross attention in all of the Transformer classes
+    in the module. The attention calculations should now execute faster, which is
+    a very important consideration in any transformer based learning.
+ 
   Version 2.4.3:
  
     The diffusion modeling part of the code should now accept training images of
     any size.  Previously it was limited to images of size 64x64.  Note that this
     change is not as significant as you might think because, under the hood, the
     actual input image size is changed to the size 64x64 for diffusion modeling.
     So this change is more for your convenience than anything else.  I have also
     improved the image visualization code in the ExamplesDiffusion directory. The
     new implementation of the script VisualizeSamples.py automatically generates a
     collage of the images generated from noise by the script
-    GenerateNewImageSamples.py.  Other changes include a minor clean-up of the
-    main doc page for GenerativeDiffusion module and of a couple of the functions
-    in the module.
+    GenerateNewImageSamples.py.  Other changes include minor clean-
+up of the main
+    doc page for GenerativeDiffusion module and of a couple of the functions in
+    the module.
  
   Version 2.4.2:
  
     DLStudio now includes a new module devoted to data modeling with diffusion.
     This module, named GenerativeDiffusion, is a co-
 class of DLStudio.  That is,
     GenerativeDiffusion resides at the same level of software abstraction as the
@@ -1141,58 +1154,81 @@
     Before you can run this script, you would need to download the training
     dataset used in this example.  See the "For Data Prediction" part of the "The
     Datasets Included" section of the doc page for that.
  
  
 ? ?  TTRRAANNSSFFOORRMMEERRSS
  
-    The goal of Transformer based learning is the same that of Seq2SeqLearning
-    described earlier in this Introduction except that now you completely forgo
-    recurrence. That is, you only use the mechanism of attention to translate
-    sentences from a source language into sentences in the target language. For
-    such applications, you need two forms of attention: self-attention and
-    cross-attention.  Self-attention refers to the intra-sentence relationships
-    between the words and cross-attention refers to the inter-sentence
-    relationships between the words in a pair of sentences, one in the source
-    language and the other in the target language. I have explained these concepts
-    in great detail in the doc sections of the inner classes in the Transformers
-    class.  In particular, I have explained the concept of the "dot-product"
-    attention in which each word puts out three things: a Query Vector Q, a Key
-    Vector K, and a Value Vector V. By taking the dot-
-product of the Query Vector
-    Q of a word with the Key Vector K for all the words in a sentence, the neural
-    network gets a measure of the extent to which each word in a sentence is
-    important to every other word.  These dot-product values are then used as
-    weights on the Value Vectors, V, for the individual words.  Cross attention
-    works in a similar manner, except that now you take the dot-
-products of the Q
-    vectors in the target-language sentence with the K vectors in the
+    For Seq2SeqLearning learning, the goal of a Transformer based implementation
+    is the same as described earlier in this Introduction except that now you
+    completely forgo recurrence. That is, you only use the mechanism of attention
+    to translate sentences from a source language into sentences in the target
+    language. For such applications, you need two forms of attention:
+    self-attention and cross-attention.  Self-attention refers to the
+    intra-sentence relationships between the words and cross-
+attention refers to
+    the inter-
+sentence relationships between the words in a pair of sentences, one
+    in the source language and the other in the target language. I have explained
+    these concepts in great detail in the doc sections of the inner classes in the
+    Transformers class.  In particular, I have explained the concept of the
+    "dot-product" attention in which each word puts out three things: a Query
+    Vector Q, a Key Vector K, and a Value Vector V. By taking the dot-
+product of
+    the Query Vector Q of a word with the Key Vector K for all the words in a
+    sentence, the neural network gets a measure of the extent to which each word
+    in a sentence is important to every other word.  These dot-
+product values are
+    then used as weights on the Value Vectors, V, for the individual words.  Cross
+    attention works in a similar manner, except that now you take the dot-
+products
+    of the Q vectors in the target-language sentence with the K vectors in the
     corresponding source-
 language sentence for producing the weight vectors that
     tell us how to weight the source-language Value Vectors vis-a-
 vis the words in
     the target language.
  
-    You will see two different implementations of the transformer architecture in
+    In addition to their use in Seq2SeqLearning learning, transformers are now
+    also used widely in computer vision applications. As a nod to their adoption
+    in the learning required for solving CV problems, I have created a new class
+    named visTransformer in the Transformers module of DLStudio.  The transformer
+    part of the logic in a visTransformer is identical to what it is in a
+    transformer class for Seq2SeqLearning learning.  That logic kicks in after you
+    have divided an image into patches and you represent each patch by an
+    embedding vector --- in exactly the same as when you represent a word or a
+    token in a sentence by an embedding vector.
+ 
+    You will see three different implementations of the transformer architecture in
     the Transformers co-class of DLStudio:
  
           TransformerFG
-    and
+ 
           TransformerPreLN
  
-    with the "FG" suffix standing for "First Generation" and the "PreLN" suffix
-    for "Pre LayerNorm". TransformerFG is my implementation of the transformer
-    architecture proposed in the famous paper by Vaswani et al.  and
-    TransformerPreLN my implementation of the same architecture but with the
-    modification suggested by Xiong et al. for more stable learning.  Since, the
-    modification is small from an architectural standpoint, I could have combined
-    both transformer types in the same implementation with some conditional logic
-    to account for the differences.  However, I have chosen to keep them separate
-    mostly for educational purposes.  Further details on these implementations are
-    in the documentation blocks in the Transformers co-class.
+          visTransformer
+ 
+    The "FG" suffix TransformerFG stands for "First Generation"; the "PreLN"
+    suffix in TransformerPreLN for "Pre LayerNorm"; and, finally, the name
+    visTransformer stands for "Vision Transformer."  
+ 
+    TransformerFG is my implementation of the transformer architecture proposed in
+    the famous paper by Vaswani et al.  and TransformerPreLN my implementation of
+    the same architecture but with the modification suggested by Xiong et al. for
+    more stable learning.  Since, the modification is small from an architectural
+    standpoint, I could have combined both transformer types in the same
+    implementation with some conditional logic to account for the differences.
+    However, I have chosen to keep them separate mostly for educational purposes.
+    Further details on these implementations are in the documentation blocks in
+    the Transformers co-class.  
+ 
+    The visTransformer implementation is based on the paper "An Image is Worth
+    16x16 Words:
+ Transformers for Image Recognition at Scale'' by Dosovitskiy et
+    al.
  
     If you want to use my code for learning the main ideas related to how to
     create purely attention based networks, your starting point for that should be
     the following scripts in the ExamplesTransformers directory of the DLStudio
     distribution:
  
         seq2seq_with_transformerFG.py
@@ -1204,14 +1240,24 @@
  
     that contains 90,000 pairs of English-Spanish sentences with the maximum
     number of words in each sentence limited to 8 words.  For processing by the
     attention networks, each sentence is enclosed in <SOS> and <EOS> tokens, with
     the former standing for "Start of Sentence" and the latter for "End of
     Sentence".
  
+    And if you wish to use visTransformer for solving image recognition problems
+    with a transformer based implementation, your starting point should be
+    the following scripts in the same ExamplesTransformers directory that was
+    mentioned above:
+ 
+          image_recog_with_visTransformer.py
+          test_checkpoint_for_visTransformer.py 
+ 
+    Both these script use the CIFAR10 dataset for demonstrating image recognition.
+ 
  
 ? ?  MMEETTRRIICC LLEEAARRNNIINNGG
  
     The main idea of metric learning is to learn a mapping from the images to
     their embedding vector representations in such a way that the embeddings for
     what are supposed to be similar images are pulled together and those for
     dissimilar images are pulled as far apart as possible.  After such a mapping
@@ -1826,36 +1872,45 @@
     the "The Datasets Included" section of the doc page for that.
  
  
 
     Transformers
     ============
  
-    The code in this co-class of DLStudio consists two slightly different
-    implementations of the transformer architecture: TransformerFG and
-    TransformerPreLN.  TransformerFG is my implementation of the architecture as
-    conceptualized in the famous paper "Attention is All You Need" by Vaswani et
-    el.  And TransformerPreLN is my implementation of the original idea along with
-    the modifications suggested by Xiong et al. in their paper "On Layer
-    Normalization in the Transformer Architecture" for more stable learning.  The
-    two versions of transformers differ in only one respect:
- The placement of the
-    LayerNorm in relation to the architectural components related to attention and
-    the feedforward network.  Literally, the difference is small, yet its
-    consequences on the stability of learning significant.
- 
-    The fundamentals of how the attention works in both TransformerFG and
-    TransformerPreLN are exactly the same.  For self-attention, you associate a
-    Query Vector Q_i and a Key Vector K_i with each word w_i in a sentence.  For a
-    given w_i, the dot product of its Q_i with the K_j vectors for all the other
-    words w_j is a measure of how related w_i is to each w_j with regard to what's
-    needed for the translation of a source sentence into the target sentence.  One
-    more vector you associate with each word w_i is the Value Vector V_i.  The
-    value vectors for the words in a sentence are weighted by the output of the
-    activation nn.LogSoftmax applied to the dot-products.
+    The code in this module of DLStudio consists of three different
+    implementations of the transformer architecture: (1) TransformerFG, (2)
+    TransformerPreLN, and (3) visTransformer.  The first two of these are meant
+    for seq2seq learning, as in language translation, and the last is for solving
+    the problem of image recognition.
+ 
+    TransformerFG is my implementation of the architecture as conceptualized in
+    the famous paper "Attention is All You Need" by Vaswani et el.  And
+    TransformerPreLN is my implementation of the original idea along with the
+    modifications suggested by Xiong et al. in their paper "On Layer Normalization
+    in the Transformer Architecture" for more stable learning.  The two versions
+    of transformers differ in only one respect:
+ The placement of the LayerNorm in
+    relation to the architectural components related to attention and the
+    feedforward network.  Literally, the difference is small, yet its consequences
+    are significant regarding the stability of learning.  Finally, visTransformer
+    is my implementation of the Vision Transformer as presented in the famou paper
+    "An Image is Worth 16x16$ Words:
+ Transformers for Image Recognition at Scale''
+    by Dosovitskiy et al.
+ 
+    The fundamentals of how the attention works in all three transformer based
+    implementations in the Transformers module are exactly the same.  For
+    self-attention, you associate a Query Vector Q_i and a Key Vector K_i with
+    each word w_i in a sentence.  For a given w_i, the dot product of its Q_i with
+    the K_j vectors for all the other words w_j is a measure of how related w_i is
+    to each w_j with regard to what's needed for the translation of a source
+    sentence into the target sentence.  One more vector you associate with each
+    word w_i is the Value Vector V_i.  The value vectors for the words in a
+    sentence are weighted by the output of the activation nn.LogSoftmax applied to
+    the dot-products.
  
     The self-attention mechanism described above is half of what goes into each
     base encoder of a transformer, the other half is a feedforward network
     
 (FFN). The overall encoder consists of a cascade of these base encoders.  In
     my implementation, I have referred to the overall encoder as the
     MasterEncoder.  The MasterDecoder also consists of a cascade of base decoders.
@@ -1877,24 +1932,32 @@
     the self-attention layer and residual connection wraps around both.
     Similarly, LayerNorm is applied to the input to FFN and the residual
     connection wraps around both.  Similar considerations applied to the decoder
     side, except we now also have a layer of cross-attention interposed between
     the self-attention and FFN.
    
     As I mentioned in the Introduction, your main entry point for experimenting
-    with the transformer code in DLStudio are the following two scripts in the
-    ExamplesTransformers directory of the distribution:
+    with the seq2seq based transformer code in DLStudio are the following two
+    scripts in the ExamplesTransformers directory of the distribution:
  
         seq2seq_with_transformerFG.py
         seq2seq_with_transformerPreLN.py
  
     However, before you can run these scripts, you would need to download the
     training dataset used in these examples.  See the "For Transformers" part of
     the "The Datasets Included" section of this doc page for that.
  
+    And your main entry point for experimenting with image recognition by playing
+    with the visTransformer class are the scripts:
+ 
+          image_recog_with_visTransformer.py
+          test_checkpoint_for_visTransformer.py 
+ 
+    Both these script use the CIFAR10 dataset for demonstrating image recognition.
+ 
  
 
     MetricLearning:
     ===================
  
     As mentioned in the Introduction, the main idea of metric learning is to learn
     a mapping from the images to their embedding vector representations in such a
@@ -2222,39 +2285,30 @@
     east and the midwest of the United States.  You can download this dataset from
     a link at the top of the main DLStudio doc page.
  
  
 EExxaammpplleessTTrraannssffoorrmmeerrss DDIIRREECCTTOORRYY
  
     The ExamplesTransformers directory of the distribution contains the following
-    two scripts for experimenting with transformers:
+    four scripts for experimenting with transformers in DLStudio:
  
         seq2seq_with_transformerFG.py 
         seq2seq_with_transformerPreLN.py         
  
-    Both these scripts deal with English-to-Spanish translation in a manner
-    similar to what's demonstrated by the code in the Seq2SeqLearning co-
-class and
-    the example scripts associated with that co-class.
- 
-    The directory also contains the following two scripts
+        image_recog_with_visTransformer.py
+        test_checkpoint_for_visTransformer.py 
  
-        test_checkpointFG.py
-        test_checkpointPreLN.py
  
-    to address the problems of training a transformer network.  As I have
-    mentioned elsewhere in this documentation, transformer training can be
-    frustrating, to say the least, and can take a very long time.  What
-    exacerbates the frustrations is that, with a wrong choice for the
-    hyperparameters, you could end with model divergence in the middle of training
-    and not know about it until the end.  [Model divergence is akin to mode
-    collapse in training a GAN.]  To deal with these problems, starting with
-    Version 2.2.7, the transformer training routines now create a checkpoint of
-    the model every 5 epochs. While the training is going on, you can evaluate the
-    checkpoints in the manner illustrated by the above two scripts.
+    The first two scripts deal with English-to-Spanish translation in a manner
+    similar to what's demonstrated by the code in the Seq2SeqLearning co-
+class and
+    the example scripts associated with that co-
+class. The last two relate to my
+    demonstration of image recognition with a transformer based implementation.  I
+    have used the CFAR10 dataset for image recognition.
  
  
 EExxaammpplleessMMeettrriiccLLeeaarrnniinngg DDIIRREECCTTOORRYY
  
     The ExamplesMetricLearning directory at top level of the distribution 
     contains the following scripts:
  
@@ -2483,15 +2537,16 @@
         That will create data directory named "dataPred" in the
         ExamplesDataPrediction directory.  With that you should be able to execute
         the data prediction script in that directory.
  
  
 ? ?  FFOORR TTRRAANNSSFFOORRMMEERRSS
  
-        Download the dataset archive
+        For the seq2seq learning part of the Transformers module in DLStudio,
+        download the dataset archive
  
             en_es_corpus_for_learning_with_Transformers.tar.gz
  
         into the ExamplesTransformers directory of the DLStudio distribution.
         Next, execute the following command in that directory:
  
             tar zxvf en_es_corpus_for_learning_with_Transformers.tar.gz
@@ -2676,61 +2731,59 @@
                      networks are difficult to train because of the vanishing gradients problem.
                      What that means is that as the depth of network increases, the loss gradients
                      calculated for the early layers become more and more muted, which suppresses
                      the learning of the parameters in those layers.  An important mitigation
                      strategy for addressing this problem consists of creating a CNN using blocks
                      with skip connections.
                       
-                     With the code shown in this inner class of the module, you can now experiment
-                     with skip connections in a CNN to see how a deep network with this feature
-                     might improve the classification results.  As you will see in the code shown
-                     below, the network that allows you to construct a CNN with skip connections
-                     is named BMEnet.  As shown in the script playing_with_skip_connections.py in
-                     the Examples directory of the distribution, you can easily create a CNN with
-                     arbitrary depth just by using the "depth" constructor option for the BMEnet
-                     class.  The basic block of the network constructed by BMEnet is called
-                     SkipBlock which, very much like the BasicBlock in ResNet-18, has a couple of
-                     convolutional layers whose output is combined with the input to the block.
-                      
-                     Note that the value given to the "depth" constructor option for the BMEnet
-                     class does NOT translate directly into the actual depth of the CNN. [Again,
-                     see the script playing_with_skip_connections.py in the Examples directory for
-                     how to use this option.] The value of "depth" is translated into how many
-                     "same input and output channels" and the "same input and output sizes"
-                     instances of SkipBlock to use between successive instances of downsampling
-                     and channel-doubling instances of SkipBlock.
+                     With the code shown in this inner class of the module, you can now experiment with
+                     skip connections in a CNN to see how a deep network with this feature might improve
+                     the classification results.  As you will see in the code shown below, the network
+                     that allows you to construct a CNN with skip connections is named BMEnet.  As shown
+                     in the script playing_with_skip_connections.py in the Examples directory of the
+                     distribution, you can easily create a CNN with arbitrary depth just by using the
+                     "depth" constructor option for the BMEnet class.  The basic block of the network
+                     constructed by BMEnet is called SkipBlock which, very much like the BasicBlock in
+                     ResNet-18, has a couple of convolutional layers whose output is combined with the
+                     input to the block.
+                      
+                     Note that the value given to the "depth" constructor option for the BMEnet class
+                     does NOT translate directly into the actual depth of the CNN. [Again, see the script
+                     playing_with_skip_connections.py in the Examples directory for how to use this
+                     option.] The value of "depth" is translated into how many "same input and output
+                     channels" and the "same input and output sizes" instances of SkipBlock to use
+                     between successive instances of downsampling and channel-doubling instances of
+                     SkipBlock.
                       
                      Class Path: DLStudio -> BMEnet
                  CCuussttoommDDaattaaLLooaaddiinngg = <class 'DLStudio.DLStudio.CustomDataLoading'>
                      This is a testbed for experimenting with a completely grounds-up attempt at
-                     designing a custom data loader.  Ordinarily, if the basic format of how the
-                     dataset is stored is similar to one of the datasets that the Torchvision
-                     module knows about, you can go ahead and use that for your own dataset.  At
-                     worst, you may need to carry out some light customizations depending on the
-                     number of classes involved, etc.
-                      
-                     However, if the underlying dataset is stored in a manner that does not look
-                     like anything in Torchvision, you have no choice but to supply yourself all
-                     of the data loading infrastructure.  That is what this inner class of the 
-                     DLStudio module is all about.
-                      
-                     The custom data loading exercise here is related to a dataset called
-                     PurdueShapes5 that contains 32x32 images of binary shapes belonging to the
-                     following five classes:
+                     designing a custom data loader.  Ordinarily, if the basic format of how the dataset
+                     is stored is similar to one of the datasets that the Torchvision module knows about,
+                     you can go ahead and use that for your own dataset.  At worst, you may need to carry
+                     out some light customizations depending on the number of classes involved, etc.
+                      
+                     However, if the underlying dataset is stored in a manner that does not look like
+                     anything in Torchvision, you have no choice but to supply yourself all of the data
+                     loading infrastructure.  That is what this inner class of the DLStudio module is all
+                     about.
+                      
+                     The custom data loading exercise here is related to a dataset called PurdueShapes5
+                     that contains 32x32 images of binary shapes belonging to the following five classes:
                       
                                     1.  rectangle
                                     2.  triangle
-                                    3.  disk
-                                    4.  oval
-                                    5.  star
-                      
-                     The dataset was generated by randomizing the sizes and the orientations
-                     of these five patterns.  Since the patterns are rotated with a very simple
-                     non-interpolating transform, just the act of random rotations can introduce
-                     boundary and even interior noise in the patterns.
+                                    3.  disk
+                                    4.  oval
+                                    5.  star
+                      
+                     The dataset was generated by randomizing the sizes and the orientations of these
+                     five patterns.  Since the patterns are rotated with a very simple non-interpolating
+                     transform, just the act of random rotations can introduce boundary and even interior
+                     noise in the patterns.
                       
                      Each 32x32 image is stored in the dataset as the following list:
                       
                                         [R, G, B, Bbox, Label]
                      where
                              R     :   is a 1024 element list of the values for the red component
                                        of the color at all the pixels
@@ -2740,49 +2793,49 @@
                              G     :   the same as above but for the blue component of the color
                       
                              Bbox  :   a list like [x1,y1,x2,y2] that defines the bounding box 
                                        for the object in the image
                         
                              Label :   the shape of the object
                       
-                     I serialize the dataset with Python's pickle module and then compress it with 
-                     the gzip module.  
+                     I serialize the dataset with Python's pickle module and then compress it with the
+                     gzip module.
                       
-                     You will find the following dataset directories in the "data" subdirectory
-                     of Examples in the DLStudio distro:
+                     You will find the following dataset directories in the "data" subdirectory of
+                     Examples in the DLStudio distro:
                       
                             PurdueShapes5-10000-train.gz
                             PurdueShapes5-1000-test.gz
                             PurdueShapes5-20-train.gz
                             PurdueShapes5-20-test.gz               
                       
-                     The number that follows the main name string "PurdueShapes5-" is for the 
-                     number of images in the dataset.  
+                     The number that follows the main name string "PurdueShapes5-" is for the number of
+                     images in the dataset.
                       
-                     You will find the last two datasets, with 20 images each, useful for debugging
-                     your logic for object detection and bounding-box regression.
+                     You will find the last two datasets, with 20 images each, useful for debugging your
+                     logic for object detection and bounding-box regression.
                       
                      Class Path:   DLStudio  ->  CustomDataLoading
                  DDeetteeccttAAnnddLLooccaalliizzee = <class 'DLStudio.DLStudio.DetectAndLocalize'>
                      The purpose of this inner class is to focus on object detection in images --- as
-                     opposed to image classification.  Most people would say that object detection
-                     is a more challenging problem than image classification because, in general,
-                     the former also requires localization.  The simplest interpretation of what
-                     is meant by localization is that the code that carries out object detection
-                     must also output a bounding-box rectangle for the object that was detected.
-                      
-                     You will find in this inner class some examples of LOADnet classes meant
-                     for solving the object detection and localization problem.  The acronym
-                     "LOAD" in "LOADnet" stands for
+                     opposed to image classification.  Most people would say that object detection is a
+                     more challenging problem than image classification because, in general, the former
+                     also requires localization.  The simplest interpretation of what is meant by
+                     localization is that the code that carries out object detection must also output a
+                     bounding-box rectangle for the object that was detected.
+                      
+                     You will find in this inner class some examples of LOADnet classes meant for solving
+                     the object detection and localization problem.  The acronym "LOAD" in "LOADnet"
+                     stands for
                       
                                  "LOcalization And Detection"
                       
-                     The different network examples included here are LOADnet1, LOADnet2, and
-                     LOADnet3.  For now, only pay attention to LOADnet2 since that's the class I
-                     have worked with the most for the 1.0.7 distribution.
+                     The different network examples included here are LOADnet1, LOADnet2, and LOADnet3.
+                     For now, only pay attention to LOADnet2 since that's the class I have worked with
+                     the most for the 1.0.7 distribution.
                       
                      Class Path:   DLStudio  ->  DetectAndLocalize
                  EExxppeerriimmeennttssWWiitthhCCIIFFAARR = <class 'DLStudio.DLStudio.ExperimentsWithCIFAR'>
                      Class Path:  DLStudio  ->  ExperimentsWithCIFAR
                  EExxppeerriimmeennttssWWiitthhSSeeqquueennttiiaall = <class 'DLStudio.DLStudio.ExperimentsWithSequential'>
                      Demonstrates how to use the torch.nn.Sequential container class
                       
@@ -2845,13 +2898,13 @@
                      News reports.  I access these embeddings through the popular Gensim library.
                       
                      Class Path:  DLStudio -> TextClassificationWithEmbeddings
  
 DDaattaa
    ____aauutthhoorr____ = 'Avinash Kak (kak@purdue.edu)'
    ____ccooppyyrriigghhtt____ = '(C) 2024 Avinash Kak. Python Software Foundation.'
-   ____ddaattee____ = '2024-March-23'
-   ____uurrll____ = 'https://engineering.purdue.edu/kak/distDT/DLStudio-2.4.3.html'
-   ____vveerrssiioonn____ = '2.4.3'
+   ____ddaattee____ = '2024-April-27'
+   ____uurrll____ = 'https://engineering.purdue.edu/kak/distDT/DLStudio-2.4.8.html'
+   ____vveerrssiioonn____ = '2.4.8'
  
 AAuutthhoorr
          Avinash Kak (kak@purdue.edu)
```

### Comparing `DLStudio-2.4.3/DLStudio.egg-info/PKG-INFO` & `DLStudio-2.4.8/DLStudio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: DLStudio
-Version: 2.4.3
+Version: 2.4.8
 Summary: A PyTorch based software platform for teaching the Deep Learning class at Purdue University
-Home-page: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html
+Home-page: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html
 Author: Avinash Kak
 Author-email: kak@purdue.edu
 Maintainer: Avinash Kak
 Maintainer-email: kak@purdue.edu
 License: Python Software Foundation License
-Download-URL: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.tar.gz
+Download-URL: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.tar.gz
 Keywords: PyTorch programming
 Platform: All platforms
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.10
 
 
 
 Consult the module API page at
 
-      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html
+      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html
 
 for all information related to this module, including the information about
 the latest changes to the code.  
 
 ::
 
       convo_layers_config = "1x[128,3,3,1]-MaxPool(2) 1x[16,5,5,1]-MaxPool(2)"
```

### Comparing `DLStudio-2.4.3/DLStudio.egg-info/SOURCES.txt` & `DLStudio-2.4.8/DLStudio.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DLStudio-2.4.3.html
+DLStudio-2.4.8.html
 MANIFEST.in
 Makefile
 README
 setup.py
 AdversarialLearning/AdversarialLearning.py
 AdversarialLearning/__init__.py
 DLStudio/DLStudio.py
@@ -39,16 +39,18 @@
 ExamplesDiffusion/README
 ExamplesDiffusion/RunCodeForDiffusion.py
 ExamplesDiffusion/VisualizeSamples.py
 ExamplesMetricLearning/example_for_pairwise_contrastive_loss.py
 ExamplesMetricLearning/example_for_triplet_loss.py
 ExamplesSeq2SeqLearning/seq2seq_with_learnable_embeddings.py
 ExamplesSeq2SeqLearning/seq2seq_with_pretrained_embeddings.py
+ExamplesTransformers/image_recog_with_visTransformer.py
 ExamplesTransformers/seq2seq_with_transformerFG.py
 ExamplesTransformers/seq2seq_with_transformerPreLN.py
+ExamplesTransformers/test_checkpoint_for_visTransformer.py
 ExamplesTransformers/upgrade_model.py
 GenerativeDiffusion/GenerativeDiffusion.py
 GenerativeDiffusion/__init__.py
 MetricLearning/MetricLearning.py
 MetricLearning/__init__.py
 Seq2SeqLearning/Seq2SeqLearning.py
 Seq2SeqLearning/__init__.py
```

### Comparing `DLStudio-2.4.3/DataPrediction/DataPrediction.py` & `DLStudio-2.4.8/DataPrediction/DataPrediction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.3'
+__version__   = '2.4.8'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-March-23'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html'
+__date__      = '2024-April-27'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
 __doc__ = '''
 
 
   You are looking at the DataPrediction co-class file in the DLStudio platform.
```

### Comparing `DLStudio-2.4.3/DataPrediction/__init__.py` & `DLStudio-2.4.8/DataPrediction/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/README` & `DLStudio-2.4.8/Examples/README`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/custom_data_loading.py` & `DLStudio-2.4.8/Examples/custom_data_loading.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/noisy_object_detection_and_localization.py` & `DLStudio-2.4.8/Examples/noisy_object_detection_and_localization.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/object_detection_and_localization.py` & `DLStudio-2.4.8/Examples/object_detection_and_localization.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/object_detection_and_localization_iou.py` & `DLStudio-2.4.8/Examples/object_detection_and_localization_iou.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/playing_with_cifar10.py` & `DLStudio-2.4.8/Examples/playing_with_cifar10.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/playing_with_reconfig.py` & `DLStudio-2.4.8/Examples/playing_with_reconfig.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/playing_with_sequential.py` & `DLStudio-2.4.8/Examples/playing_with_sequential.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/playing_with_skip_connections.py` & `DLStudio-2.4.8/Examples/playing_with_skip_connections.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/semantic_segmentation.py` & `DLStudio-2.4.8/Examples/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/text_classification_with_GRU.py` & `DLStudio-2.4.8/Examples/text_classification_with_GRU.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/text_classification_with_GRU_word2vec.py` & `DLStudio-2.4.8/Examples/text_classification_with_GRU_word2vec.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/text_classification_with_TEXTnet.py` & `DLStudio-2.4.8/Examples/text_classification_with_TEXTnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 
 ##  watch -d -n 0.5 nvidia-smi
 
 from DLStudio import *
 
 
-#dataroot = "/home/kak/TextDatasets/sentiment_dataset/"
-dataroot = "./data/TextDatasets/sentiment_dataset/"
+dataroot = "/home/kak/TextDatasets/sentiment_dataset/"
+#dataroot = "./data/TextDatasets/sentiment_dataset/"
 
 
 dataset_archive_train = "sentiment_dataset_train_40.tar.gz"
 #dataset_archive_train = "sentiment_dataset_train_200.tar.gz"
 
 dataset_archive_test =  "sentiment_dataset_test_40.tar.gz"
 #dataset_archive_test = "sentiment_dataset_test_200.tar.gz"
```

### Comparing `DLStudio-2.4.3/Examples/text_classification_with_TEXTnetOrder2.py` & `DLStudio-2.4.8/Examples/text_classification_with_TEXTnetOrder2.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/text_classification_with_TEXTnetOrder2_word2vec.py` & `DLStudio-2.4.8/Examples/text_classification_with_TEXTnetOrder2_word2vec.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Examples/text_classification_with_TEXTnet_word2vec.py` & `DLStudio-2.4.8/Examples/text_classification_with_TEXTnet_word2vec.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesAdversarialLearning/README` & `DLStudio-2.4.8/ExamplesAdversarialLearning/README`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesAdversarialLearning/dcgan_DG1.py` & `DLStudio-2.4.8/ExamplesAdversarialLearning/dcgan_DG1.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesAdversarialLearning/dcgan_DG2.py` & `DLStudio-2.4.8/ExamplesAdversarialLearning/dcgan_DG2.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesAdversarialLearning/wgan_CG1.py` & `DLStudio-2.4.8/ExamplesAdversarialLearning/wgan_CG1.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesAdversarialLearning/wgan_with_gp_CG2.py` & `DLStudio-2.4.8/ExamplesAdversarialLearning/wgan_with_gp_CG2.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesDataPrediction/power_load_prediction_with_pmGRU.py` & `DLStudio-2.4.8/ExamplesDataPrediction/power_load_prediction_with_pmGRU.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesDiffusion/GenerateNewImageSamples.py` & `DLStudio-2.4.8/ExamplesDiffusion/GenerateNewImageSamples.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesDiffusion/README` & `DLStudio-2.4.8/ExamplesDiffusion/README`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesDiffusion/RunCodeForDiffusion.py` & `DLStudio-2.4.8/ExamplesDiffusion/RunCodeForDiffusion.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesDiffusion/VisualizeSamples.py` & `DLStudio-2.4.8/ExamplesDiffusion/VisualizeSamples.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesMetricLearning/example_for_pairwise_contrastive_loss.py` & `DLStudio-2.4.8/ExamplesMetricLearning/example_for_pairwise_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesMetricLearning/example_for_triplet_loss.py` & `DLStudio-2.4.8/ExamplesMetricLearning/example_for_triplet_loss.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesSeq2SeqLearning/seq2seq_with_learnable_embeddings.py` & `DLStudio-2.4.8/ExamplesSeq2SeqLearning/seq2seq_with_learnable_embeddings.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesSeq2SeqLearning/seq2seq_with_pretrained_embeddings.py` & `DLStudio-2.4.8/ExamplesSeq2SeqLearning/seq2seq_with_pretrained_embeddings.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/ExamplesTransformers/seq2seq_with_transformerFG.py` & `DLStudio-2.4.8/ExamplesTransformers/seq2seq_with_transformerFG.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,32 +50,36 @@
 #dataroot = "/home/kak/TextDatasets/en_es_corpus_xformer/"
 #dataroot = "/mnt/cloudNAS3/Avi/TextDatasets/en_es_corpus_xformer/"
 
 data_archive =  "en_es_xformer_8_90000.tar.gz"
 
 max_seq_length = 10
 
-embedding_size = 256                   ## for running in RVL Cloud
+embedding_size = 256        
 #embedding_size = 128
-#embedding_size = 64                   ## for running on laptop
+#embedding_size = 64        
 
-num_basic_encoders = num_basic_decoders = num_atten_heads = 4       ## for running on RVL Cloud
-#num_basic_encoders = num_basic_decoders = num_atten_heads = 2      ## for running on laptop
+num_basic_encoders = num_basic_decoders = num_atten_heads = 4     
+#num_basic_encoders = num_basic_decoders = num_atten_heads = 2    
 
 #optimizer_params = {'beta1' : 0.9,  'beta2': 0.98,  'epsilon' : 1e-9}
 optimizer_params = {'beta1' : 0.9,  'beta2': 0.98,  'epsilon' : 1e-6}
 
 num_warmup_steps = 4000
 
 #masking = True
 masking = False
 
 dls = DLStudio(
                 dataroot = dataroot,
-                path_saved_model = {"encoder" : "./saved_encoder", "decoder" : "./saved_decoder"},
+                path_saved_model = {"encoder" : "./saved_encoder", 
+                                    "decoder" : "./saved_decoder", 
+                                    "embeddings_generator_en" : "./saved_embeddings_generator_en",
+                                    "embeddings_generator_es" : "./saved_embeddings_generator_es",
+                                   },
                 batch_size = 50,
                 use_gpu = True,
                 epochs = 40,
               )
 
 xformer = TransformerFG( 
                         dl_studio = dls,
@@ -118,12 +122,12 @@
 if masking:
     xformer.run_code_for_training_TransformerFG(dls,master_encoder,master_decoder,display_train_loss=True,
                                                                                      checkpoints_dir="checkpoints_with_masking_FG")
 else:
     xformer.run_code_for_training_TransformerFG(dls,master_encoder,master_decoder,display_train_loss=True,
                                                                                         checkpoints_dir="checkpoints_no_masking_FG")
 
-import pymsgbox
-response = pymsgbox.confirm("Finished training.  Start evaluation?")
+#import pymsgbox
+#response = pymsgbox.confirm("Finished training.  Start evaluation?")
 
-if response == "OK": 
-    xformer.run_code_for_evaluating_TransformerFG(master_encoder, master_decoder, 'myoutput.txt')
+#if response == "OK": 
+xformer.run_code_for_evaluating_TransformerFG(master_encoder, master_decoder, 'myoutput.txt')
```

### Comparing `DLStudio-2.4.3/ExamplesTransformers/seq2seq_with_transformerPreLN.py` & `DLStudio-2.4.8/ExamplesTransformers/seq2seq_with_transformerPreLN.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,36 +41,41 @@
 
 
 ##  watch -d -n 0.5 nvidia-smi
 
 from DLStudio import *
 from Transformers import *
 
+
 dataroot = "./data/"
 #dataroot = "/home/kak/TextDatasets/en_es_corpus_xformer/"
 #dataroot = "/mnt/cloudNAS3/Avi/TextDatasets/en_es_corpus_xformer/"
 
 #data_archive =  "en_es_xformer_8_10000.tar.gz"
 data_archive =  "en_es_xformer_8_90000.tar.gz"
 
 max_seq_length = 10
 
-embedding_size = 256                       ##  for running on RVL Cloud
+embedding_size = 256               
 #embedding_size = 128
-#embedding_size = 64                         ##  for running on laptop
+#embedding_size = 64               
 
-num_basic_encoders = num_basic_decoders = num_atten_heads = 4       ##  for running on RVL Cloud
-#num_basic_encoders = num_basic_decoders = num_atten_heads = 2        ##  for running on laptop
+num_basic_encoders = num_basic_decoders = num_atten_heads = 4   
+#num_basic_encoders = num_basic_decoders = num_atten_heads = 2  
 
 masking = True
 #masking = False
 
 dls = DLStudio(
                 dataroot = dataroot,
-                path_saved_model = {"encoder" : "./saved_encoder", "decoder" : "./saved_decoder"},
+                path_saved_model = {"encoder" : "./saved_encoder", 
+                                    "decoder" : "./saved_decoder", 
+                                    "embeddings_generator_en" : "./saved_embeddings_generator_en",
+                                    "embeddings_generator_es" : "./saved_embeddings_generator_es",
+                                   },
                 learning_rate =  1e-5, 
                 batch_size = 50,
                 use_gpu = True,
                 epochs = 60,
       )
 
 xformer = TransformerPreLN( 
@@ -112,14 +117,13 @@
 if masking:
     xformer.run_code_for_training_TransformerPreLN(dls,master_encoder,master_decoder,display_train_loss=True,
                                                                         checkpoints_dir="checkpoints_with_masking_PreLN")
 else:
     xformer.run_code_for_training_TransformerPreLN(dls,master_encoder,master_decoder,display_train_loss=True,
                                                                         checkpoints_dir="checkpoints_no_masking_PreLN")
 
-import pymsgbox
-
-response = pymsgbox.confirm("Finished training.  Start evaluation?")
+#import pymsgbox
+#response = pymsgbox.confirm("Finished training.  Start evaluation?")
+#if response == "OK": 
 
-if response == "OK": 
-    xformer.run_code_for_evaluating_TransformerPreLN(master_encoder, master_decoder)
+xformer.run_code_for_evaluating_TransformerPreLN(master_encoder, master_decoder)
```

### Comparing `DLStudio-2.4.3/ExamplesTransformers/upgrade_model.py` & `DLStudio-2.4.8/ExamplesTransformers/upgrade_model.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/GenerativeDiffusion/GenerativeDiffusion.py` & `DLStudio-2.4.8/GenerativeDiffusion/GenerativeDiffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.3'
+__version__   = '2.4.8'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-March-23'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html'
+__date__      = '2024-April-27'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
-
 __doc__  =  '''
 
 You are looking at the GenerativeDiffusion co-class file in the DLStudio platform.
 For the overall documentation on DLStudio, visit:
 
            https://engineering.purdue.edu/kak/distDLS/
 
@@ -1251,15 +1250,15 @@
         return x
 ##################################################   End of mUNet Class  ##################################################
 ###########################################################################################################################
 
 
 
 ###########################################################################################################################
-############################################### Start of utilty classes ###################################################
+############################################## Start of utilty functions ##################################################
 
 def timestep_embedding(timesteps, dim, max_period=10000):  
     """
     Source:  https://github.com/openai/improved-diffusion
 
     Create sinusoidal timestep embeddings.
 
@@ -1298,15 +1297,15 @@
     Source:  https://github.com/openai/improved-diffusion
     Zero out the parameters of a module and return it.
     """
     for p in module.parameters():
         p.detach().zero_()
     return module
 
-################################################ End of utilty classes ####################################################
+############################################### End of utilty functions ###################################################
 ###########################################################################################################################
 
 
 
 ##______________________________    Test code follows    _________________________________
 
 if __name__ == '__main__':
```

### Comparing `DLStudio-2.4.3/GenerativeDiffusion/__init__.py` & `DLStudio-2.4.8/GenerativeDiffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/MANIFEST.in` & `DLStudio-2.4.8/MANIFEST.in`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 include MetricLearning/MetricLearning.py
 include MetricLearning/__init__.py
 GenerativeDiffusion/GenerativeDiffusion.py
 GenerativeDiffusion/__init__.py
 include setup.py
 include Makefile
 include README
-include DLStudio-2.4.3.html
+include DLStudio-2.4.8.html
 include TestDLStudio/DLStudio.py
 include TestDLStudio/TestInstanceCreation.py
 include TestDLStudio/Test.py
 include Examples/README
 include Examples/playing_with_reconfig.py
 include Examples/playing_with_sequential.py
 include Examples/playing_with_cifar10.py
@@ -42,16 +42,15 @@
 include ExamplesAdversarialLearning/wgan_CG1.py
 include ExamplesAdversarialLearning/wgan_with_gp_CG2.py
 include ExamplesSeq2SeqLearning/seq2seq_with_learnable_embeddings.py
 include ExamplesSeq2SeqLearning/seq2seq_with_pretrained_embeddings.py
 include ExamplesDataPrediction/power_load_prediction_with_pmGRU.py
 include ExamplesTransformers/seq2seq_with_transformerFG.py
 include ExamplesTransformers/seq2seq_with_transformerPreLN.py
-include ExamplesTransformers/test_checkpointFG.py
-include ExamplesTransformers/test_your_own_sentence_checkpointFG.py
-include ExamplesTransformers/test_checkpointPreLN.py
+include ExamplesTransformers/image_recog_with_visTransformer.py
+include ExamplesTransformers/test_checkpoint_for_visTransformer.py
 include ExamplesMetricLearning/example_for_pairwise_contrastive_loss.py
 include ExamplesMetricLearning/example_for_triplet_loss.py
 include ExamplesDiffusion/README
 include ExamplesDiffusion/RunCodeForDiffusion.py
 include ExamplesDiffusion/GenerateNewImageSamples.py
 include ExamplesDiffusion/VisualizeSamples.py
```

### Comparing `DLStudio-2.4.3/Makefile` & `DLStudio-2.4.8/Makefile`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/MetricLearning/MetricLearning.py` & `DLStudio-2.4.8/MetricLearning/MetricLearning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.3'
+__version__   = '2.4.8'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-March-23'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html'
+__date__      = '2024-April-27'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
-
 __doc__ = '''
 
 
   You are looking at the MetricLearning module file in the DLStudio platform.
   For the overall documentation on DLStudio, visit:
 
            https://engineering.purdue.edu/kak/distDLS/
```

### Comparing `DLStudio-2.4.3/MetricLearning/__init__.py` & `DLStudio-2.4.8/MetricLearning/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/PKG-INFO` & `DLStudio-2.4.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: DLStudio
-Version: 2.4.3
+Version: 2.4.8
 Summary: A PyTorch based software platform for teaching the Deep Learning class at Purdue University
-Home-page: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html
+Home-page: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html
 Author: Avinash Kak
 Author-email: kak@purdue.edu
 Maintainer: Avinash Kak
 Maintainer-email: kak@purdue.edu
 License: Python Software Foundation License
-Download-URL: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.tar.gz
+Download-URL: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.tar.gz
 Keywords: PyTorch programming
 Platform: All platforms
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.10
 
 
 
 Consult the module API page at
 
-      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html
+      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html
 
 for all information related to this module, including the information about
 the latest changes to the code.  
 
 ::
 
       convo_layers_config = "1x[128,3,3,1]-MaxPool(2) 1x[16,5,5,1]-MaxPool(2)"
```

### Comparing `DLStudio-2.4.3/README` & `DLStudio-2.4.8/README`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Seq2SeqLearning/Seq2SeqLearning.py` & `DLStudio-2.4.8/Seq2SeqLearning/Seq2SeqLearning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.3'
+__version__   = '2.4.8'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-March-23'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html'
+__date__      = '2024-April-27'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
-
 __doc__ = '''
 
 
   You are looking at the Seq2SeqLearning co-class file in the DLStudio platform.
   For the overall documentation on DLStudio, visit:
 
            https://engineering.purdue.edu/kak/distDLS/
```

### Comparing `DLStudio-2.4.3/Seq2SeqLearning/__init__.py` & `DLStudio-2.4.8/Seq2SeqLearning/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/TestDLStudio/DLStudio.py` & `DLStudio-2.4.8/TestDLStudio/DLStudio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.3'
+__version__   = '2.4.8'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-March-23'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html'
+__date__      = '2024-April-27'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
 
 __doc__ = '''
 
 DLStudio.py
@@ -18,27 +18,37 @@
 
 Date: ''' + __date__ + '''
 
 
 @tag_changes
 CHANGE LOG:
 
+  Version 2.4.8:
+
+    In this version, I have made two important changes to the Transformers module
+    in DLStudio: (1) The Transformers module now includes a new class that I have
+    named visTransformer that works like the famous Vision Transformer (ViT)
+    proposed by Dosovitskiy et al. And (2) I have made changes to the QKV code for
+    the calculation of self and cross attention in all of the Transformer classes
+    in the module. The attention calculations should now execute faster, which is
+    a very important consideration in any transformer based learning.
+
   Version 2.4.3:
 
     The diffusion modeling part of the code should now accept training images of
     any size.  Previously it was limited to images of size 64x64.  Note that this
     change is not as significant as you might think because, under the hood, the
     actual input image size is changed to the size 64x64 for diffusion modeling.
     So this change is more for your convenience than anything else.  I have also
     improved the image visualization code in the ExamplesDiffusion directory. The
     new implementation of the script VisualizeSamples.py automatically generates a
     collage of the images generated from noise by the script
-    GenerateNewImageSamples.py.  Other changes include a minor clean-up of the
-    main doc page for GenerativeDiffusion module and of a couple of the functions
-    in the module.
+    GenerateNewImageSamples.py.  Other changes include minor clean-up of the main
+    doc page for GenerativeDiffusion module and of a couple of the functions in
+    the module.
 
   Version 2.4.2:
 
     DLStudio now includes a new module devoted to data modeling with diffusion.
     This module, named GenerativeDiffusion, is a co-class of DLStudio.  That is,
     GenerativeDiffusion resides at the same level of software abstraction as the
     main DLStudio class in the platform.  See the README in the new
@@ -1002,54 +1012,73 @@
     dataset used in this example.  See the "For Data Prediction" part of the "The
     Datasets Included" section of the doc page for that.
 
 
 @tag2_transformers
     TRANSFORMERS
 
-    The goal of Transformer based learning is the same that of Seq2SeqLearning
-    described earlier in this Introduction except that now you completely forgo
-    recurrence. That is, you only use the mechanism of attention to translate
-    sentences from a source language into sentences in the target language. For
-    such applications, you need two forms of attention: self-attention and
-    cross-attention.  Self-attention refers to the intra-sentence relationships
-    between the words and cross-attention refers to the inter-sentence
-    relationships between the words in a pair of sentences, one in the source
-    language and the other in the target language. I have explained these concepts
-    in great detail in the doc sections of the inner classes in the Transformers
-    class.  In particular, I have explained the concept of the "dot-product"
-    attention in which each word puts out three things: a Query Vector Q, a Key
-    Vector K, and a Value Vector V. By taking the dot-product of the Query Vector
-    Q of a word with the Key Vector K for all the words in a sentence, the neural
-    network gets a measure of the extent to which each word in a sentence is
-    important to every other word.  These dot-product values are then used as
-    weights on the Value Vectors, V, for the individual words.  Cross attention
-    works in a similar manner, except that now you take the dot-products of the Q
-    vectors in the target-language sentence with the K vectors in the
+    For Seq2SeqLearning learning, the goal of a Transformer based implementation
+    is the same as described earlier in this Introduction except that now you
+    completely forgo recurrence. That is, you only use the mechanism of attention
+    to translate sentences from a source language into sentences in the target
+    language. For such applications, you need two forms of attention:
+    self-attention and cross-attention.  Self-attention refers to the
+    intra-sentence relationships between the words and cross-attention refers to
+    the inter-sentence relationships between the words in a pair of sentences, one
+    in the source language and the other in the target language. I have explained
+    these concepts in great detail in the doc sections of the inner classes in the
+    Transformers class.  In particular, I have explained the concept of the
+    "dot-product" attention in which each word puts out three things: a Query
+    Vector Q, a Key Vector K, and a Value Vector V. By taking the dot-product of
+    the Query Vector Q of a word with the Key Vector K for all the words in a
+    sentence, the neural network gets a measure of the extent to which each word
+    in a sentence is important to every other word.  These dot-product values are
+    then used as weights on the Value Vectors, V, for the individual words.  Cross
+    attention works in a similar manner, except that now you take the dot-products
+    of the Q vectors in the target-language sentence with the K vectors in the
     corresponding source-language sentence for producing the weight vectors that
     tell us how to weight the source-language Value Vectors vis-a-vis the words in
     the target language.
 
-    You will see two different implementations of the transformer architecture in
+    In addition to their use in Seq2SeqLearning learning, transformers are now
+    also used widely in computer vision applications. As a nod to their adoption
+    in the learning required for solving CV problems, I have created a new class
+    named visTransformer in the Transformers module of DLStudio.  The transformer
+    part of the logic in a visTransformer is identical to what it is in a
+    transformer class for Seq2SeqLearning learning.  That logic kicks in after you
+    have divided an image into patches and you represent each patch by an
+    embedding vector --- in exactly the same as when you represent a word or a
+    token in a sentence by an embedding vector.
+
+    You will see three different implementations of the transformer architecture in
     the Transformers co-class of DLStudio:
 
           TransformerFG
-    and
+
           TransformerPreLN
 
-    with the "FG" suffix standing for "First Generation" and the "PreLN" suffix
-    for "Pre LayerNorm". TransformerFG is my implementation of the transformer
-    architecture proposed in the famous paper by Vaswani et al.  and
-    TransformerPreLN my implementation of the same architecture but with the
-    modification suggested by Xiong et al. for more stable learning.  Since, the
-    modification is small from an architectural standpoint, I could have combined
-    both transformer types in the same implementation with some conditional logic
-    to account for the differences.  However, I have chosen to keep them separate
-    mostly for educational purposes.  Further details on these implementations are
-    in the documentation blocks in the Transformers co-class.
+          visTransformer
+
+    The "FG" suffix TransformerFG stands for "First Generation"; the "PreLN"
+    suffix in TransformerPreLN for "Pre LayerNorm"; and, finally, the name
+    visTransformer stands for "Vision Transformer."  
+
+    TransformerFG is my implementation of the transformer architecture proposed in
+    the famous paper by Vaswani et al.  and TransformerPreLN my implementation of
+    the same architecture but with the modification suggested by Xiong et al. for
+    more stable learning.  Since, the modification is small from an architectural
+    standpoint, I could have combined both transformer types in the same
+    implementation with some conditional logic to account for the differences.
+    However, I have chosen to keep them separate mostly for educational purposes.
+    Further details on these implementations are in the documentation blocks in
+    the Transformers co-class.  
+
+    The visTransformer implementation is based on the paper "An Image is Worth
+    16x16 Words: Transformers for Image Recognition at Scale'' by Dosovitskiy et
+    al.
  
     If you want to use my code for learning the main ideas related to how to
     create purely attention based networks, your starting point for that should be
     the following scripts in the ExamplesTransformers directory of the DLStudio
     distribution:
 
         seq2seq_with_transformerFG.py
@@ -1061,14 +1090,24 @@
 
     that contains 90,000 pairs of English-Spanish sentences with the maximum
     number of words in each sentence limited to 8 words.  For processing by the
     attention networks, each sentence is enclosed in <SOS> and <EOS> tokens, with
     the former standing for "Start of Sentence" and the latter for "End of
     Sentence".
 
+    And if you wish to use visTransformer for solving image recognition problems
+    with a transformer based implementation, your starting point should be
+    the following scripts in the same ExamplesTransformers directory that was
+    mentioned above:
+
+          image_recog_with_visTransformer.py
+          test_checkpoint_for_visTransformer.py 
+
+    Both these script use the CIFAR10 dataset for demonstrating image recognition.
+
 
 @tag2_metriclearning
     METRIC LEARNING
 
     The main idea of metric learning is to learn a mapping from the images to
     their embedding vector representations in such a way that the embeddings for
     what are supposed to be similar images are pulled together and those for
@@ -1653,35 +1692,43 @@
 
 
 @tag_coclass5
     ============
     Transformers
     ============
 
-    The code in this co-class of DLStudio consists two slightly different
-    implementations of the transformer architecture: TransformerFG and
-    TransformerPreLN.  TransformerFG is my implementation of the architecture as
-    conceptualized in the famous paper "Attention is All You Need" by Vaswani et
-    el.  And TransformerPreLN is my implementation of the original idea along with
-    the modifications suggested by Xiong et al. in their paper "On Layer
-    Normalization in the Transformer Architecture" for more stable learning.  The
-    two versions of transformers differ in only one respect: The placement of the
-    LayerNorm in relation to the architectural components related to attention and
-    the feedforward network.  Literally, the difference is small, yet its
-    consequences on the stability of learning significant.
-
-    The fundamentals of how the attention works in both TransformerFG and
-    TransformerPreLN are exactly the same.  For self-attention, you associate a
-    Query Vector Q_i and a Key Vector K_i with each word w_i in a sentence.  For a
-    given w_i, the dot product of its Q_i with the K_j vectors for all the other
-    words w_j is a measure of how related w_i is to each w_j with regard to what's
-    needed for the translation of a source sentence into the target sentence.  One
-    more vector you associate with each word w_i is the Value Vector V_i.  The
-    value vectors for the words in a sentence are weighted by the output of the
-    activation nn.LogSoftmax applied to the dot-products.
+    The code in this module of DLStudio consists of three different
+    implementations of the transformer architecture: (1) TransformerFG, (2)
+    TransformerPreLN, and (3) visTransformer.  The first two of these are meant
+    for seq2seq learning, as in language translation, and the last is for solving
+    the problem of image recognition.
+
+    TransformerFG is my implementation of the architecture as conceptualized in
+    the famous paper "Attention is All You Need" by Vaswani et el.  And
+    TransformerPreLN is my implementation of the original idea along with the
+    modifications suggested by Xiong et al. in their paper "On Layer Normalization
+    in the Transformer Architecture" for more stable learning.  The two versions
+    of transformers differ in only one respect: The placement of the LayerNorm in
+    relation to the architectural components related to attention and the
+    feedforward network.  Literally, the difference is small, yet its consequences
+    are significant regarding the stability of learning.  Finally, visTransformer
+    is my implementation of the Vision Transformer as presented in the famou paper
+    "An Image is Worth 16x16$ Words: Transformers for Image Recognition at Scale''
+    by Dosovitskiy et al.
+
+    The fundamentals of how the attention works in all three transformer based
+    implementations in the Transformers module are exactly the same.  For
+    self-attention, you associate a Query Vector Q_i and a Key Vector K_i with
+    each word w_i in a sentence.  For a given w_i, the dot product of its Q_i with
+    the K_j vectors for all the other words w_j is a measure of how related w_i is
+    to each w_j with regard to what's needed for the translation of a source
+    sentence into the target sentence.  One more vector you associate with each
+    word w_i is the Value Vector V_i.  The value vectors for the words in a
+    sentence are weighted by the output of the activation nn.LogSoftmax applied to
+    the dot-products.
 
     The self-attention mechanism described above is half of what goes into each
     base encoder of a transformer, the other half is a feedforward network
     (FFN). The overall encoder consists of a cascade of these base encoders.  In
     my implementation, I have referred to the overall encoder as the
     MasterEncoder.  The MasterDecoder also consists of a cascade of base decoders.
     A base decoder is similar to a base encoder except for there being a layer of
@@ -1701,24 +1748,32 @@
     the self-attention layer and residual connection wraps around both.
     Similarly, LayerNorm is applied to the input to FFN and the residual
     connection wraps around both.  Similar considerations applied to the decoder
     side, except we now also have a layer of cross-attention interposed between
     the self-attention and FFN.
    
     As I mentioned in the Introduction, your main entry point for experimenting
-    with the transformer code in DLStudio are the following two scripts in the
-    ExamplesTransformers directory of the distribution:
+    with the seq2seq based transformer code in DLStudio are the following two
+    scripts in the ExamplesTransformers directory of the distribution:
 
         seq2seq_with_transformerFG.py
         seq2seq_with_transformerPreLN.py
 
     However, before you can run these scripts, you would need to download the
     training dataset used in these examples.  See the "For Transformers" part of
     the "The Datasets Included" section of this doc page for that.
 
+    And your main entry point for experimenting with image recognition by playing
+    with the visTransformer class are the scripts:
+
+          image_recog_with_visTransformer.py
+          test_checkpoint_for_visTransformer.py 
+
+    Both these script use the CIFAR10 dataset for demonstrating image recognition.
+
 
 @tag_coclass6
     ===================
     MetricLearning:
     ===================
 
     As mentioned in the Introduction, the main idea of metric learning is to learn
@@ -2036,38 +2091,28 @@
     a link at the top of the main DLStudio doc page.
 
 
 @tag_examples_xform
 ExamplesTransformers DIRECTORY:
 
     The ExamplesTransformers directory of the distribution contains the following
-    two scripts for experimenting with transformers:
+    four scripts for experimenting with transformers in DLStudio:
 
         seq2seq_with_transformerFG.py 
         seq2seq_with_transformerPreLN.py         
 
-    Both these scripts deal with English-to-Spanish translation in a manner
-    similar to what's demonstrated by the code in the Seq2SeqLearning co-class and
-    the example scripts associated with that co-class.
-
-    The directory also contains the following two scripts
+        image_recog_with_visTransformer.py
+        test_checkpoint_for_visTransformer.py 
 
-        test_checkpointFG.py
-        test_checkpointPreLN.py
 
-    to address the problems of training a transformer network.  As I have
-    mentioned elsewhere in this documentation, transformer training can be
-    frustrating, to say the least, and can take a very long time.  What
-    exacerbates the frustrations is that, with a wrong choice for the
-    hyperparameters, you could end with model divergence in the middle of training
-    and not know about it until the end.  [Model divergence is akin to mode
-    collapse in training a GAN.]  To deal with these problems, starting with
-    Version 2.2.7, the transformer training routines now create a checkpoint of
-    the model every 5 epochs. While the training is going on, you can evaluate the
-    checkpoints in the manner illustrated by the above two scripts.
+    The first two scripts deal with English-to-Spanish translation in a manner
+    similar to what's demonstrated by the code in the Seq2SeqLearning co-class and
+    the example scripts associated with that co-class. The last two relate to my
+    demonstration of image recognition with a transformer based implementation.  I
+    have used the CFAR10 dataset for image recognition.
 
 
 @tag_examples_metric
 ExamplesMetricLearning DIRECTORY:
 
     The ExamplesMetricLearning directory at top level of the distribution 
     contains the following scripts:
@@ -2302,15 +2347,16 @@
         ExamplesDataPrediction directory.  With that you should be able to execute
         the data prediction script in that directory.
 
 
 @tag2_dataset
     FOR TRANSFORMERS:
 
-        Download the dataset archive
+        For the seq2seq learning part of the Transformers module in DLStudio,
+        download the dataset archive
 
             en_es_corpus_for_learning_with_Transformers.tar.gz
 
         into the ExamplesTransformers directory of the DLStudio distribution.
         Next, execute the following command in that directory:
 
             tar zxvf en_es_corpus_for_learning_with_Transformers.tar.gz
@@ -2625,23 +2671,19 @@
                                   tvt.ToTensor(),
                                   tvt.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))])        
         ##  Don't need any augmentation for the test data: 
         transform_test = tvt.Compose([
                                tvt.ToTensor(),
                                tvt.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))])
         ##  Define where the training and the test datasets are located
-        train_data_loc = torchvision.datasets.CIFAR10(
-                        root=self.dataroot, train=True, download=True, transform=transform_train)
-        test_data_loc = torchvision.datasets.CIFAR10(
-                      root=self.dataroot, train=False, download=True, transform=transform_test)
+        train_data_loc = torchvision.datasets.CIFAR10( root=self.dataroot, train=True, download=True, transform=transform_train )
+        test_data_loc = torchvision.datasets.CIFAR10(  root=self.dataroot, train=False, download=True, transform=transform_test )
         ##  Now create the data loaders:
-        self.train_data_loader = torch.utils.data.DataLoader(train_data_loc, batch_size=self.batch_size, 
-                                                                     shuffle=True, num_workers=2)
-        self.test_data_loader = torch.utils.data.DataLoader(test_data_loc, batch_size=self.batch_size, 
-                                                                 shuffle=False, num_workers=2)
+        self.train_data_loader = torch.utils.data.DataLoader(train_data_loc, batch_size=self.batch_size, shuffle=True, num_workers=2)
+        self.test_data_loader = torch.utils.data.DataLoader(test_data_loc, batch_size=self.batch_size, shuffle=False, num_workers=2)
 
     def imshow(self, img):
         '''
         called by display_tensor_as_image() for displaying the image
         '''
         img = img / 2 + 0.5     # unnormalize
         npimg = img.numpy()
@@ -2705,17 +2747,15 @@
                     FILE.flush()
                     running_loss = 0.0
                     if display_images:
                         logger = logging.getLogger()
                         old_level = logger.level
                         logger.setLevel(100)
                         plt.figure(figsize=[6,3])
-
-                        plt.imshow(np.transpose(torchvision.utils.make_grid(inputs, 
-                                                            normalize=False, padding=3, pad_value=255).cpu(), (1,2,0)))
+                        plt.imshow(np.transpose(torchvision.utils.make_grid(inputs,  normalize=False, padding=3, pad_value=255).cpu(), (1,2,0)))
                         plt.show()
                         logger.setLevel(old_level)
                 loss.backward()
                 optimizer.step()
         print("\nFinished Training\n")
         self.save_model(net)
         plt.figure(figsize=(10,5))
@@ -2807,32 +2847,29 @@
         with torch.no_grad():
             for i,data in enumerate(self.test_data_loader):
                 ##  data is set to the images and the labels for one batch at a time:
                 images, labels = data
                 images = images.to(self.device)
                 labels = labels.to(self.device)
                 if i % 1000 == 999:
-                    print("\n\n[i=%d:] Ground Truth:     " % (i+1) + ' '.join('%5s' % self.class_labels[labels[j]] 
-                                                                   for j in range(self.batch_size)))
+                    print("\n\n[i=%d:] Ground Truth:     " % (i+1) + ' '.join('%5s' % self.class_labels[labels[j]] for j in range(self.batch_size)))
                 outputs = net(images)
                 ##  max() returns two things: the max value and its index in the 10 element
                 ##  output vector.  We are only interested in the index --- since that is 
                 ##  essentially the predicted class label:
                 _, predicted = torch.max(outputs.data, 1)#
 #                if display_images and i % 1000 == 999:
                 if i % 1000 == 999:
-                    print("[i=%d:] Predicted Labels: " % (i+1) + ' '.join('%5s' % self.class_labels[predicted[j]]
-                                                              for j in range(self.batch_size)))
+                    print("[i=%d:] Predicted Labels: " % (i+1) + ' '.join('%5s' % self.class_labels[predicted[j]] for j in range(self.batch_size)))
                     logger = logging.getLogger()
                     old_level = logger.level
                     if display_images:
                         logger.setLevel(100)
                         plt.figure(figsize=[6,3])
-                        plt.imshow(np.transpose(torchvision.utils.make_grid(images,
-                                                      normalize=False, padding=3, pad_value=255).cpu(), (1,2,0)))
+                        plt.imshow(np.transpose(torchvision.utils.make_grid(images, normalize=False, padding=3, pad_value=255).cpu(), (1,2,0)))
                         plt.show()
                         logger.setLevel(old_level)
                 for label,prediction in zip(labels,predicted):
                         confusion_matrix[label][prediction] += 1
                 total += labels.size(0)
                 correct += (predicted == labels).sum().item()
                 ##  comp is a list of size batch_size of "True" and "False" vals
@@ -3088,32 +3125,32 @@
         networks are difficult to train because of the vanishing gradients problem.
         What that means is that as the depth of network increases, the loss gradients
         calculated for the early layers become more and more muted, which suppresses
         the learning of the parameters in those layers.  An important mitigation
         strategy for addressing this problem consists of creating a CNN using blocks
         with skip connections.
 
-        With the code shown in this inner class of the module, you can now experiment
-        with skip connections in a CNN to see how a deep network with this feature
-        might improve the classification results.  As you will see in the code shown
-        below, the network that allows you to construct a CNN with skip connections
-        is named BMEnet.  As shown in the script playing_with_skip_connections.py in
-        the Examples directory of the distribution, you can easily create a CNN with
-        arbitrary depth just by using the "depth" constructor option for the BMEnet
-        class.  The basic block of the network constructed by BMEnet is called
-        SkipBlock which, very much like the BasicBlock in ResNet-18, has a couple of
-        convolutional layers whose output is combined with the input to the block.
-    
-        Note that the value given to the "depth" constructor option for the BMEnet
-        class does NOT translate directly into the actual depth of the CNN. [Again,
-        see the script playing_with_skip_connections.py in the Examples directory for
-        how to use this option.] The value of "depth" is translated into how many
-        "same input and output channels" and the "same input and output sizes"
-        instances of SkipBlock to use between successive instances of downsampling
-        and channel-doubling instances of SkipBlock.
+        With the code shown in this inner class of the module, you can now experiment with
+        skip connections in a CNN to see how a deep network with this feature might improve
+        the classification results.  As you will see in the code shown below, the network
+        that allows you to construct a CNN with skip connections is named BMEnet.  As shown
+        in the script playing_with_skip_connections.py in the Examples directory of the
+        distribution, you can easily create a CNN with arbitrary depth just by using the
+        "depth" constructor option for the BMEnet class.  The basic block of the network
+        constructed by BMEnet is called SkipBlock which, very much like the BasicBlock in
+        ResNet-18, has a couple of convolutional layers whose output is combined with the
+        input to the block.
+    
+        Note that the value given to the "depth" constructor option for the BMEnet class
+        does NOT translate directly into the actual depth of the CNN. [Again, see the script
+        playing_with_skip_connections.py in the Examples directory for how to use this
+        option.] The value of "depth" is translated into how many "same input and output
+        channels" and the "same input and output sizes" instances of SkipBlock to use
+        between successive instances of downsampling and channel-doubling instances of
+        SkipBlock.
  
         Class Path: DLStudio -> BMEnet
         """
         def __init__(self, dl_studio, skip_connections=True, depth=8):
             super(DLStudio.BMEnet, self).__init__()
             self.dl_studio = dl_studio
             self.depth = depth
@@ -3215,40 +3252,39 @@
 
 
     ###%%%
     ########################################################################################
     #################  Start Definition of Inner Class CustomDataLoading  ##################
 
     class CustomDataLoading(nn.Module):             
-        """This is a testbed for experimenting with a completely grounds-up attempt at
-        designing a custom data loader.  Ordinarily, if the basic format of how the
-        dataset is stored is similar to one of the datasets that the Torchvision
-        module knows about, you can go ahead and use that for your own dataset.  At
-        worst, you may need to carry out some light customizations depending on the
-        number of classes involved, etc.
-
-        However, if the underlying dataset is stored in a manner that does not look
-        like anything in Torchvision, you have no choice but to supply yourself all
-        of the data loading infrastructure.  That is what this inner class of the 
-        DLStudio module is all about.
-
-        The custom data loading exercise here is related to a dataset called
-        PurdueShapes5 that contains 32x32 images of binary shapes belonging to the
-        following five classes:
+        """
+        This is a testbed for experimenting with a completely grounds-up attempt at
+        designing a custom data loader.  Ordinarily, if the basic format of how the dataset
+        is stored is similar to one of the datasets that the Torchvision module knows about,
+        you can go ahead and use that for your own dataset.  At worst, you may need to carry
+        out some light customizations depending on the number of classes involved, etc.
+
+        However, if the underlying dataset is stored in a manner that does not look like
+        anything in Torchvision, you have no choice but to supply yourself all of the data
+        loading infrastructure.  That is what this inner class of the DLStudio module is all
+        about.
+
+        The custom data loading exercise here is related to a dataset called PurdueShapes5
+        that contains 32x32 images of binary shapes belonging to the following five classes:
 
                        1.  rectangle
                        2.  triangle
                        3.  disk
                        4.  oval
                        5.  star
 
-        The dataset was generated by randomizing the sizes and the orientations
-        of these five patterns.  Since the patterns are rotated with a very simple
-        non-interpolating transform, just the act of random rotations can introduce
-        boundary and even interior noise in the patterns.
+        The dataset was generated by randomizing the sizes and the orientations of these
+        five patterns.  Since the patterns are rotated with a very simple non-interpolating
+        transform, just the act of random rotations can introduce boundary and even interior
+        noise in the patterns.
 
         Each 32x32 image is stored in the dataset as the following list:
 
                            [R, G, B, Bbox, Label]
         where
                 R     :   is a 1024 element list of the values for the red component
                           of the color at all the pixels
@@ -3258,30 +3294,30 @@
                 G     :   the same as above but for the blue component of the color
 
                 Bbox  :   a list like [x1,y1,x2,y2] that defines the bounding box 
                           for the object in the image
            
                 Label :   the shape of the object
 
-        I serialize the dataset with Python's pickle module and then compress it with 
-        the gzip module.  
+        I serialize the dataset with Python's pickle module and then compress it with the
+        gzip module.
 
-        You will find the following dataset directories in the "data" subdirectory
-        of Examples in the DLStudio distro:
+        You will find the following dataset directories in the "data" subdirectory of
+        Examples in the DLStudio distro:
 
                PurdueShapes5-10000-train.gz
                PurdueShapes5-1000-test.gz
                PurdueShapes5-20-train.gz
                PurdueShapes5-20-test.gz               
 
-        The number that follows the main name string "PurdueShapes5-" is for the 
-        number of images in the dataset.  
+        The number that follows the main name string "PurdueShapes5-" is for the number of
+        images in the dataset.
 
-        You will find the last two datasets, with 20 images each, useful for debugging
-        your logic for object detection and bounding-box regression.
+        You will find the last two datasets, with 20 images each, useful for debugging your
+        logic for object detection and bounding-box regression.
 
         Class Path:   DLStudio  ->  CustomDataLoading
         """     
         def __init__(self, dl_studio, dataserver_train=None, dataserver_test=None, dataset_file_train=None, dataset_file_test=None):
             super(DLStudio.CustomDataLoading, self).__init__()
             self.dl_studio = dl_studio
             self.dataserver_train = dataserver_train
@@ -3549,29 +3585,29 @@
     ###%%%
     ########################################################################################
     ###################  Start Definition of Inner Class DetectAndLocalize  ################
 
     class DetectAndLocalize(nn.Module):             
         """
         The purpose of this inner class is to focus on object detection in images --- as
-        opposed to image classification.  Most people would say that object detection
-        is a more challenging problem than image classification because, in general,
-        the former also requires localization.  The simplest interpretation of what
-        is meant by localization is that the code that carries out object detection
-        must also output a bounding-box rectangle for the object that was detected.
-
-        You will find in this inner class some examples of LOADnet classes meant
-        for solving the object detection and localization problem.  The acronym
-        "LOAD" in "LOADnet" stands for
+        opposed to image classification.  Most people would say that object detection is a
+        more challenging problem than image classification because, in general, the former
+        also requires localization.  The simplest interpretation of what is meant by
+        localization is that the code that carries out object detection must also output a
+        bounding-box rectangle for the object that was detected.
+
+        You will find in this inner class some examples of LOADnet classes meant for solving
+        the object detection and localization problem.  The acronym "LOAD" in "LOADnet"
+        stands for
 
                     "LOcalization And Detection"
 
-        The different network examples included here are LOADnet1, LOADnet2, and
-        LOADnet3.  For now, only pay attention to LOADnet2 since that's the class I
-        have worked with the most for the 1.0.7 distribution.
+        The different network examples included here are LOADnet1, LOADnet2, and LOADnet3.
+        For now, only pay attention to LOADnet2 since that's the class I have worked with
+        the most for the 1.0.7 distribution.
 
         Class Path:   DLStudio  ->  DetectAndLocalize
         """
         def __init__(self, dl_studio, dataserver_train=None, dataserver_test=None, dataset_file_train=None, dataset_file_test=None):
             super(DLStudio.DetectAndLocalize, self).__init__()
             self.dl_studio = dl_studio
             self.dataserver_train = dataserver_train
@@ -3758,34 +3794,29 @@
                         out = out + torch.cat((identity, identity), dim=1)
                 return out
 
 
 
         class LOADnet1(nn.Module):
             """
-            The acronym 'LOAD' stands for 'LOcalization And Detection'.
-            LOADnet1 only uses fully-connected layers for the regression
+            The acronym 'LOAD' stands for 'LOcalization And Detection'.  LOADnet1 only
+            uses fully-connected layers for the regression
 
             Class Path:   DLStudio  ->  DetectAndLocalize  ->  LOADnet1
             """
             def __init__(self, skip_connections=True, depth=32):
                 super(DLStudio.DetectAndLocalize.LOADnet1, self).__init__()
                 self.pool_count = 3
                 self.depth = depth // 2
                 self.conv = nn.Conv2d(3, 64, 3, padding=1)
-                self.skip64 = DLStudio.DetectAndLocalize.SkipBlock3(64, 64, 
-                                                           skip_connections=skip_connections)
-                self.skip64ds = DLStudio.DetectAndLocalize.SkipBlock3(64, 64, 
-                                           downsample=True, skip_connections=skip_connections)
-                self.skip64to128 = DLStudio.DetectAndLocalize.SkipBlock3(64, 128, 
-                                                            skip_connections=skip_connections )
-                self.skip128 = DLStudio.DetectAndLocalize.SkipBlock3(128, 128, 
-                                                             skip_connections=skip_connections)
-                self.skip128ds = DLStudio.DetectAndLocalize.SkipBlock3(128,128,
-                                            downsample=True, skip_connections=skip_connections)
+                self.skip64 = DLStudio.DetectAndLocalize.SkipBlock3(64, 64, skip_connections=skip_connections)
+                self.skip64ds = DLStudio.DetectAndLocalize.SkipBlock3(64, 64, downsample=True, skip_connections=skip_connections)
+                self.skip64to128 = DLStudio.DetectAndLocalize.SkipBlock3(64, 128, skip_connections=skip_connections )
+                self.skip128 = DLStudio.DetectAndLocalize.SkipBlock3(128, 128, skip_connections=skip_connections)
+                self.skip128ds = DLStudio.DetectAndLocalize.SkipBlock3(128,128, downsample=True, skip_connections=skip_connections)
                 self.fc1 =  nn.Linear(128 * (32 // 2**self.pool_count)**2, 1000)
                 self.fc2 =  nn.Linear(1000, 5)
                 self.fc3 =  nn.Linear(32768, 1000)
                 self.fc4 =  nn.Linear(1000, 4)
 
             def forward(self, x):
                 x = nn.MaxPool2d(2,2)(nn.functional.relu(self.conv(x)))          
@@ -3808,16 +3839,16 @@
                 x2 =  x.view( x.shape[0], - 1 )
                 x2 = nn.functional.relu(self.fc3(x2))
                 x2 = self.fc4(x2)
                 return x1,x2
 
         class LOADnet2(nn.Module):
             """
-            The acronym 'LOAD' stands for 'LOcalization And Detection'.
-            LOADnet2 uses both convo and linear layers for regression
+            The acronym 'LOAD' stands for 'LOcalization And Detection'.  LOADnet2 uses
+            both convo and linear layers for regression
 
             Class Path:   DLStudio  ->  DetectAndLocalize  ->  LOADnet2
             """ 
             def __init__(self, skip_connections=True, depth=8):
                 super(DLStudio.DetectAndLocalize.LOADnet2, self).__init__()
                 if depth not in [8,10,12,14,16]:
                     sys.exit("LOADnet2 has only been tested for 'depth' values 8, 10, 12, 14, and 16")
@@ -3884,18 +3915,19 @@
                 x2 = x2.view( x.shape[0], - 1 )
                 x2 = self.fc_seqn(x2)
                 return x1,x2
 
 
         class LOADnet3(nn.Module):
             """
-            The acronym 'LOAD' stands for 'LOcalization And Detection'.
-            LOADnet3 uses both convo and linear layers for regression
+            The acronym 'LOAD' stands for 'LOcalization And Detection'.  LOADnet3 uses
+            both convo and linear layers for regression
 
             Class Path:   DLStudio  ->  DetectAndLocalize  ->  LOADnet3
+
             """ 
             def __init__(self, skip_connections=True, depth=8):
                 super(DLStudio.DetectAndLocalize.LOADnet3, self).__init__()
                 if depth not in [4, 8, 16]:
                     sys.exit("LOADnet2 has been tested for 'depth' for only 4, 8, and 16")
                 self.depth = depth // 4
                 self.conv = nn.Conv2d(3, 64, 3, padding=1)
@@ -4479,158 +4511,152 @@
         This version of DLStudio also comes with a new dataset, PurdueShapes5MultiObject,
         for experimenting with mUnet.  Each image in this dataset contains a random number
         of selections from five different shapes, with the shapes being randomly scaled,
         oriented, and located in each image.  The five different shapes are: rectangle,
         triangle, disk, oval, and star.
 
            Class Path:   DLStudio  ->  SemanticSegmentation
-
         """
         def __init__(self, dl_studio, max_num_objects, dataserver_train=None, dataserver_test=None, dataset_file_train=None, dataset_file_test=None):
             super(DLStudio.SemanticSegmentation, self).__init__()
             self.dl_studio = dl_studio
             self.max_num_objects = max_num_objects
             self.dataserver_train = dataserver_train
             self.dataserver_test = dataserver_test
 
 
         class PurdueShapes5MultiObjectDataset(torch.utils.data.Dataset):
             """
             The very first thing to note is that the images in the dataset
-            PurdueShapes5MultiObjectDataset are of size 64x64.  Each image has a
-            random number (up to five) of the objects drawn from the following five
-            shapes: rectangle, triangle, disk, oval, and star.  Each shape is
-            randomized with respect to all its parameters, including those for its
-            scale and location in the image.
-
-            Each image in the dataset is represented by two data objects, one a list
-            and the other a dictionary. The list data objects consists of the
-            following items:
+            PurdueShapes5MultiObjectDataset are of size 64x64.  Each image has a random
+            number (up to five) of the objects drawn from the following five shapes:
+            rectangle, triangle, disk, oval, and star.  Each shape is randomized with
+            respect to all its parameters, including those for its scale and location in the
+            image.
+
+            Each image in the dataset is represented by two data objects, one a list and the
+            other a dictionary. The list data objects consists of the following items:
 
                 [R, G, B, mask_array, mask_val_to_bbox_map]                                   ## (A)
             
             and the other data object is a dictionary that is set to:
             
                 label_map = {'rectangle':50, 
                              'triangle' :100, 
                              'disk'     :150, 
                              'oval'     :200, 
                              'star'     :250}                                                 ## (B)
             
-            Note that that second data object for each image is the same, as shown
-            above.
+            Note that that second data object for each image is the same, as shown above.
 
-            In the rest of this comment block, I'll explain in greater detail the
-            elements of the list in line (A) above.
+            In the rest of this comment block, I'll explain in greater detail the elements
+            of the list in line (A) above.
 
             
             R,G,B:
             ------
 
-            Each of these is a 4096-element array whose elements store the
-            corresponding color values at each of the 4096 pixels in a 64x64 image.
-            That is, R is a list of 4096 integers, each between 0 and 255, for the
-            value of the red component of the color at each pixel. Similarly, for G
-            and B.
+            Each of these is a 4096-element array whose elements store the corresponding
+            color values at each of the 4096 pixels in a 64x64 image.  That is, R is a list
+            of 4096 integers, each between 0 and 255, for the value of the red component of
+            the color at each pixel. Similarly, for G and B.
             
 
             mask_array:
             ----------
 
-            The fourth item in the list shown in line (A) above is for the mask which is
-            a numpy array of shape:
+            The fourth item in the list shown in line (A) above is for the mask which is a
+            numpy array of shape:
             
                            (5, 64, 64)
             
             It is initialized by the command:
             
                  mask_array = np.zeros((5,64,64), dtype=np.uint8)
             
-            In essence, the mask_array consists of five planes, each of size 64x64.
-            Each plane of the mask array represents an object type according to the
-            following shape_index
+            In essence, the mask_array consists of five planes, each of size 64x64.  Each
+            plane of the mask array represents an object type according to the following
+            shape_index
             
                     shape_index = (label_map[shape] - 50) // 50
             
             where the label_map is as shown in line (B) above.  In other words, the
             shape_index values for the different shapes are:
             
                      rectangle:  0
                       triangle:  1
                           disk:  2
                           oval:  3
                           star:  4
             
-            Therefore, the first layer (of index 0) of the mask is where the pixel
-            values of 50 are stored at all those pixels that belong to the rectangle
-            shapes.  Similarly, the second mask layer (of index 1) is where the pixel
-            values of 100 are stored at all those pixel coordinates that belong to
-            the triangle shapes in an image; and so on.
+            Therefore, the first layer (of index 0) of the mask is where the pixel values of
+            50 are stored at all those pixels that belong to the rectangle shapes.
+            Similarly, the second mask layer (of index 1) is where the pixel values of 100
+            are stored at all those pixel coordinates that belong to the triangle shapes in
+            an image; and so on.
             
-            It is in the manner described above that we define five different masks
-            for an image in the dataset.  Each mask is for a different shape and the
-            pixel values at the nonzero pixels in each mask layer are keyed to the
-            shapes also.
+            It is in the manner described above that we define five different masks for an
+            image in the dataset.  Each mask is for a different shape and the pixel values
+            at the nonzero pixels in each mask layer are keyed to the shapes also.
             
-            A reader is likely to wonder as to the need for this redundancy in the
-            dataset representation of the shapes in each image.  Such a reader is
-            likely to ask: Why can't we just use the binary values 1s and 0s in each
-            mask layer where the corresponding pixels are in the image?  Setting
-            these mask values to 50, 100, etc., was done merely for convenience.  I
-            went with the intuition that the learning needed for multi-object
-            segmentation would become easier if each shape was represented by a
-            different pixels value in the corresponding mask. So I went ahead
-            incorporated that in the dataset generation program itself.
-
-            The mask values for the shapes are not to be confused with the actual RGB
-            values of the pixels that belong to the shapes. The RGB values at the
-            pixels in a shape are randomly generated.  Yes, all the pixels in a shape
-            instance in an image have the same RGB values (but that value has nothing
-            to do with the values given to the mask pixels for that shape).
+            A reader is likely to wonder as to the need for this redundancy in the dataset
+            representation of the shapes in each image.  Such a reader is likely to ask: Why
+            can't we just use the binary values 1s and 0s in each mask layer where the
+            corresponding pixels are in the image?  Setting these mask values to 50, 100,
+            etc., was done merely for convenience.  I went with the intuition that the
+            learning needed for multi-object segmentation would become easier if each shape
+            was represented by a different pixels value in the corresponding mask. So I went
+            ahead incorporated that in the dataset generation program itself.
+
+            The mask values for the shapes are not to be confused with the actual RGB values
+            of the pixels that belong to the shapes. The RGB values at the pixels in a shape
+            are randomly generated.  Yes, all the pixels in a shape instance in an image
+            have the same RGB values (but that value has nothing to do with the values given
+            to the mask pixels for that shape).
             
             
             mask_val_to_bbox_map:
             --------------------
                    
-            The fifth item in the list in line (A) above is a dictionary that tells us
-            what bounding-box rectangle to associate with each shape in the image.  To
-            illustrate what this dictionary looks like, assume that an image contains
-            only one rectangle and only one disk, the dictionary in this case will look
-            like:
+            The fifth item in the list in line (A) above is a dictionary that tells us what
+            bounding-box rectangle to associate with each shape in the image.  To illustrate
+            what this dictionary looks like, assume that an image contains only one
+            rectangle and only one disk, the dictionary in this case will look like:
             
                 mask values to bbox mappings:  {200: [], 
                                                 250: [], 
                                                 100: [], 
                                                  50: [[56, 20, 63, 25]], 
                                                 150: [[37, 41, 55, 59]]}
             
-            Should there happen to be two rectangles in the same image, the dictionary
-            would then be like:
+            Should there happen to be two rectangles in the same image, the dictionary would
+            then be like:
             
                 mask values to bbox mappings:  {200: [], 
                                                 250: [], 
                                                 100: [], 
                                                  50: [[56, 20, 63, 25], [18, 16, 32, 36]], 
                                                 150: [[37, 41, 55, 59]]}
             
-            Therefore, it is not a problem even if all the objects in an image are of
-            the same type.  Remember, the object that are selected for an image are
-            shown randomly from the different shapes.  By the way, an entry like '[56,
-            20, 63, 25]' for the bounding box means that the upper-left corner of the
-            BBox for the 'rectangle' shape is at (56,20) and the lower-right corner of
-            the same is at the pixel coordinates (63,25).
+            Therefore, it is not a problem even if all the objects in an image are of the
+            same type.  Remember, the object that are selected for an image are shown
+            randomly from the different shapes.  By the way, an entry like '[56, 20, 63,
+            25]' for the bounding box means that the upper-left corner of the BBox for the
+            'rectangle' shape is at (56,20) and the lower-right corner of the same is at the
+            pixel coordinates (63,25).
             
             As far as the BBox quadruples are concerned, in the definition
             
                     [min_x,min_y,max_x,max_y]
             
             note that x is the horizontal coordinate, increasing to the right on your
             screen, and y is the vertical coordinate increasing downwards.
 
             Class Path:   DLStudio  ->  SemanticSegmentation  ->  PurdueShapes5MultiObjectDataset
+
             """
             def __init__(self, dl_studio, segmenter, train_or_test, dataset_file):
                 super(DLStudio.SemanticSegmentation.PurdueShapes5MultiObjectDataset, self).__init__()
                 max_num_objects = segmenter.max_num_objects
                 if train_or_test == 'train' and dataset_file == "PurdueShapes5MultiObject-10000-train.gz":
                     if os.path.exists("torch_saved_PurdueShapes5MultiObject-10000_dataset.pt") and \
                               os.path.exists("torch_saved_PurdueShapes5MultiObject_label_map.pt"):
@@ -5224,26 +5250,26 @@
             def init_hidden(self):
                 hidden = torch.zeros(1, self.hidden_size)
                 return hidden
 
 
         class TEXTnetOrder2(nn.Module):
             """
-            In this variant of the TEXTnet network, the value of hidden as used at
-            each time step also includes its value at the previous time step.  This 
-            fact, not directly apparent by the definition of the class shown below, 
-            is made possible by the last parameter, cell, in the header of forward().  
-            All you can see here, at the end of forward(), is that the value of cell 
-            goes through a linear layer and through a sigmoid nonlinearity. By the way, 
-            since the sigmoid saturates at 0 and 1, it can act like a switch. Later 
-            when I use this class in the training function, you will see the cell
-            values being used in such a manner that the hidden state at each time
-            step is mixed with the hidden state at the previous time step.
+            In this variant of the TEXTnet network, the value of hidden as used at each
+            time step also includes its value at the previous time step.  This fact, not
+            directly apparent by the definition of the class shown below, is made possible
+            by the last parameter, cell, in the header of forward().  As you can see below,
+            at the end of forward(), the value of the cell goes through a linear layer
+            and through a sigmoid nonlinearity. By the way, since the sigmoid saturates at 0
+            and 1, it can act like a switch. Later when I use this class in the training
+            function, you will see the cell values being used in such a manner that the
+            hidden state at each time step is mixed with the hidden state at the previous
+            time step, but only to the extent allowed by the switching action of the Sigmoid.
 
-            Class Path:  DLStudio -> TextClassification -> EXTnetOrder2
+            Class Path:  DLStudio -> TextClassification -> TEXTnetOrder2
             """
             def __init__(self, input_size, hidden_size, output_size):
                 super(DLStudio.TextClassification.TEXTnetOrder2, self).__init__()
                 self.input_size = input_size
                 self.hidden_size = hidden_size
                 self.output_size = output_size
                 self.combined_to_hidden = nn.Linear(input_size + 2*hidden_size, hidden_size)
@@ -5334,15 +5360,16 @@
                     input = torch.zeros(1,review_tensor.shape[2])
                     input = input.to(self.dl_studio.device)
                     for k in range(review_tensor.shape[1]):
                         input[0,:] = review_tensor[0,k]
                         output, hidden = net(input, hidden)
                     loss = criterion(output, torch.argmax(sentiment,1))
                     running_loss += loss.item()
-                    loss.backward(retain_graph=True)        
+#                    loss.backward(retain_graph=True)        
+                    loss.backward()        
                     optimizer.step()
                     if i % 200 == 199:    
                         avg_loss = running_loss / float(200)
                         training_loss_tally.append(avg_loss)
                         current_time = time.perf_counter()
                         time_elapsed = current_time-start_time
                         print("[epoch:%d  iter:%4d  elapsed_time: %4d secs]     loss: %.5f" % (epoch+1,i+1, time_elapsed,avg_loss))
```

### Comparing `DLStudio-2.4.3/TestDLStudio/Test.py` & `DLStudio-2.4.8/TestDLStudio/Test.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/TestDLStudio/TestInstanceCreation.py` & `DLStudio-2.4.8/TestDLStudio/TestInstanceCreation.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.3/Transformers/Transformers.py` & `DLStudio-2.4.8/Transformers/Transformers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.3'
+__version__   = '2.4.8'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-March-23'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html'
+__date__      = '2024-April-27'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
 
 __doc__ = '''
 
 
@@ -16,33 +16,40 @@
 
            https://engineering.purdue.edu/kak/distDLS/
 
 
 
 TRANSFORMERS:
 
-    There are two different kinds of transformers in this file:
+    There are three different transformer based implementations in this file:
 
          TransformerFG                 [FG stands for "First Generation"]
 
          TransformerPreLN              [PreLN stands for "Pre Layer Norm"]
- 
-    The very small difference between the two has important consequences with
-    regard to how fast and how stably the learning takes place in the two
-    implementations.  I could have easily combined the two implementations with a
-    small number of conditional statements to account for the differences, however
-    I have chosen to keep them separate in order to make it easier for the two to
-    evolve separately and to be used differently for educational purposes.
+
+         visTransformer                [stands for Vision Transformer]
+
+    Although the first two are very similar, the difference between the two has
+    important consequences with regard to how fast and how stably the learning
+    takes place in the two implementations.  I could have easily combined the two
+    implementations with a small number of conditional statements to account for
+    the differences.  However I have chosen to keep them separate in order to make
+    it easier for the two to evolve separately and to be used differently for
+    educational purposes.  The third, visTransformer, is meant for solving image
+    recognition problems with transformers.
 
     The TransformerFG implementation is based on the transformers as first
     envisioned in the seminal paper "Attention is All You Need" by Vaswani et el.
     And, the network code in TransformerPreLN incorporates the modifications
     suggested by "On Layer Normalization in the Transformer Architecture" by Xiong
     et al.  Both these papers are now so well known that just entering their title
     in a Google search window will take you directly to their PDFs at arxiv.org.
+    The visTransformer implementation is based on the paper "An Image is Worth
+    16x16 Words: Transformers for Image Recognition at Scale'' by Dosovitskiy et
+    al.
 
     The sequence-to-sequence problem addressed in both TransformerFG and
     TransformerPreLN is the English-to-Spanish translation problem, which is the
     same problem as in the Seq2SeqLearning co-class in the DLStudio module.  The
     seq2seq learning in the Seq2SeqLearning class was based on using recurrence
     along with the notion of attention.  Recurrence was used to generate a time
     evolution of the hidden state as a sentence was scanned left-to-right and
@@ -87,14 +94,22 @@
     The following two scripts in the ExamplesTransformers directory of the
     distribution are your main entry points for experimenting with the
     Transformers code:
 
         seq2seq_with_transformerFG.py
         seq2seq_with_transformerPreLN.py
 
+    For the image recognition class visTransformer, I'll use the CIFAR-10 datasete
+    that you are alrady very familiar with.  The following two scripts in the same
+    ExamplesTransformers directory as mentioned above are your main entry points
+    for playing with the vision related Transformer code in DLStudio:
+
+        image_recog_with_visTransformer.py  
+        test_checkpoint_for_visTransformer.py
+
 
 
 REGARDING THE DIFFICULTY OF TRAINING A TRANSFORMER NETWORK:
 
     Transformers, in general, are difficult to train and that's especially the
     case with TransformerFG. Using the same learning rate throughout the training
     process either results in excessively slow learning if the learning-rate is
@@ -119,77 +134,53 @@
     rate linearly with the iteration index.  Note that the more stable
     TransformerPreLN does NOT require a learning-rate warm-up --- because that
     transformer is inherently more stable. The price you pay for that stability is
     the slower convergence of the model.  In my own rather informal and
     unscientific comparisons, the performance I get with about 20 epochs of
     TransformerFG takes more than 60 epochs with TransformerPreLN.
 
-    To cope with the challenges of training a transformer, starting with Version
-    2.2.7, DLStudio provides you with the tools you need so that you can be more
-    productive during the training phase. Now when you train a model, the training
-    function spits out a checkpoint for the model every 5 epochs. Additionally,
-    now you also have the functions for checking the performance of the
-    checkpoints. The performance check can be as simple as looking at the
-    translated sentences vis-a-vis their targets for a random selection of
-    sentence pairs from the data.  When real learning is taking place, you will
-    see longer and longer fragments of the translated sentences corresponding to
-    the target sentences. On the other hand, when you have model divergence, the
-    translated sentences will appear to be gibberish.  A future version of
-    DLStudio will also print out the BLEU score for the checkpoints.
-
-    The following scripts in the ExamplesTransformers directory of the distro show
-    how to check the performance of the checkpoints:
- 
-        test_checkpointFG.py
-        test_checkpointPreLN.py
-
-    These scripts call the following function in the code in this file for showing
-    you how a particular checkpoint is performing:
-
-        run_code_for_evaluating_checkpoint()
-
-    I have defined this function separately in the TransformerFG and TransformerPreLN 
-    classes.
-
 @endofdocs
 '''
 
 
 from DLStudio import DLStudio
 
 import sys,os,os.path
 import torch
 import torch.nn as nn
 import torch.optim as optim
+import torchvision
+import torchvision.transforms as tvt
 import numpy as np
 import math
 import random
 import matplotlib.pyplot as plt
 import matplotlib.animation as animation
 import time
 import glob                                                                                                           
 import gzip
 import pickle
 
+"""
 import signal
-
 def sigchld_sig_handler( signum, frame ):                                                                       
-    print("shutting down the training session --- chile processes")
+    print("shutting down the training session --- child processes")
     os.wait()                                                                                                   
-                                                                                                                       
 def interrupt_sig_handler( signum, frame ):    
     print("shutting down the training session --- main process")
     os.kill( os.getpid(), signal.SIGKILL )                                                                          
-                                                                                                                       
 signal.signal( signal.SIGINT,  interrupt_sig_handler )                                                          
 signal.signal( signal.SIGCHLD, sigchld_sig_handler ) 
+"""
 
 
 ###%%%
-##################################  Start Definition of Inner Class TransformerFG  ####################################
+#######################################################################################################################
+####################################  Start Definition of Class TransformerFG  #######################################
+#######################################################################################################################
 
 class TransformerFG(nn.Module):             
     """
     TransformerFG stands for "Transformer First Generation".
 
     The goal of this class is to serve as an instructional aid in understanding the basic 
     concepts of attention-based learning with neural networks --- as laid out in the 
@@ -602,32 +593,29 @@
 
         """
         def __init__(self, dl_studio, max_seq_length, qkv_size, num_atten_heads):
             super(TransformerFG.AttentionHead, self).__init__()
             self.dl_studio = dl_studio
             self.qkv_size = qkv_size
             self.max_seq_length = max_seq_length
-            self.WQ =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (B)
-            self.WK =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (C)
-            self.WV =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (D)
+            self.WQ =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (B)
+            self.WK =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (C)
+            self.WV =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (D)
             self.softmax = nn.Softmax(dim=1)                                                                           ## (E)
 
         def forward(self, sent_embed_slice):           ## sent_embed_slice == sentence_embedding_slice                 ## (F)
-            Q = self.WQ( sent_embed_slice.reshape(sent_embed_slice.shape[0],-1).float() )                              ## (G)
-            K = self.WK( sent_embed_slice.reshape(sent_embed_slice.shape[0],-1).float() )                              ## (H)
-            V = self.WV( sent_embed_slice.reshape(sent_embed_slice.shape[0],-1).float() )                              ## (I)
-            Q = Q.view(sent_embed_slice.shape[0], self.max_seq_length, self.qkv_size)                                  ## (J)
-            K = K.view(sent_embed_slice.shape[0], self.max_seq_length, self.qkv_size)                                  ## (K)
-            V = V.view(sent_embed_slice.shape[0], self.max_seq_length, self.qkv_size)                                  ## (L)
-            A = K.transpose(2,1)                                                                                       ## (M)
-            QK_dot_prod = Q @ A                                                                                        ## (N)
-            rowwise_softmax_normalizations = self.softmax( QK_dot_prod )                                               ## (O)
-            Z = rowwise_softmax_normalizations @ V                                                                     ## (P)
-            coeff = 1.0/torch.sqrt(torch.tensor([self.qkv_size]).float()).to(self.dl_studio.device)                    ## (Q)
-            Z = coeff * Z                                                                                              ## (R)
+            Q = self.WQ( sent_embed_slice )                                                                            ## (G)
+            K = self.WK( sent_embed_slice )                                                                            ## (H)
+            V = self.WV( sent_embed_slice )                                                                            ## (I)
+            A = K.transpose(2,1)                                                                                       ## (J)
+            QK_dot_prod = Q @ A                                                                                        ## (K)
+            rowwise_softmax_normalizations = self.softmax( QK_dot_prod )                                               ## (L)
+            Z = rowwise_softmax_normalizations @ V                                                                     ## (M)
+            coeff = 1.0/torch.sqrt(torch.tensor([self.qkv_size]).float()).to(self.dl_studio.device)                    ## (N)
+            Z = coeff * Z                                                                                              ## (O)
             return Z
 
 
     ###%%%
     ##################################  Cross Attention Code for TransformerFG  #######################################
 
     class CrossAttention(nn.Module):
@@ -704,32 +692,30 @@
         ClassPath:  TransformerFG  ->   CrossAttention
         """  
         def __init__(self, dl_studio, max_seq_length, qkv_size, num_atten_heads):
             super(TransformerFG.CrossAttentionHead, self).__init__()
             self.dl_studio = dl_studio
             self.qkv_size = qkv_size
             self.max_seq_length = max_seq_length
-            self.WQ =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (B)
-            self.WK =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (C)
-            self.WV =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (D)
+            self.WQ =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (B)
+            self.WK =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (C)
+            self.WV =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (D)
             self.softmax = nn.Softmax(dim=1)                                                                           ## (E)
 
         def forward(self, basic_decoder_slice, final_encoder_slice):                                                   ## (F)
-            Q = self.WQ( basic_decoder_slice.reshape(final_encoder_slice.shape[0],-1).float() )                        ## (G)
-            K = self.WK( final_encoder_slice.reshape(final_encoder_slice.shape[0],-1).float() )                        ## (H)
-            V = self.WV( final_encoder_slice.reshape(final_encoder_slice.shape[0],-1).float() )                        ## (I)
-            Q = Q.view(final_encoder_slice.shape[0], self.max_seq_length, self.qkv_size)                               ## (J)
-            K = K.view(final_encoder_slice.shape[0], self.max_seq_length, self.qkv_size)                               ## (K)
-            V = V.view(final_encoder_slice.shape[0], self.max_seq_length, self.qkv_size)                               ## (L)
-            A = K.transpose(2,1)                                                                                       ## (M)
-            QK_dot_prod = Q @ A                                                                                        ## (N)
-            rowwise_softmax_normalizations = self.softmax( QK_dot_prod )                                               ## (O)
-            Z = rowwise_softmax_normalizations @ V                                                                     ## (P)
-            coeff = 1.0/torch.sqrt(torch.tensor([self.qkv_size]).float()).to(self.dl_studio.device)                    ## (Q)
-            Z = coeff * Z                                                                                              ## (R)
+            Q = self.WQ( basic_decoder_slice )                                                                         ## (G)
+            K = self.WK( final_encoder_slice )                                                                         ## (H)
+            V = self.WV( final_encoder_slice )                                                                         ## (I)
+
+            A = K.transpose(2,1)                                                                                       ## (J)
+            QK_dot_prod = Q @ A                                                                                        ## (K)
+            rowwise_softmax_normalizations = self.softmax( QK_dot_prod )                                               ## (L)
+            Z = rowwise_softmax_normalizations @ V                                                                     ## (M)
+            coeff = 1.0/torch.sqrt(torch.tensor([self.qkv_size]).float()).to(self.dl_studio.device)                    ## (N)
+            Z = coeff * Z                                                                                              ## (O)
             return Z
 
 
 
     ###%%%
     ###################################   Basic Decoder Code for TransformerFG ########################################
 
@@ -866,27 +852,35 @@
         "Save the trained encoder to a disk file"       
         torch.save(encoder.state_dict(), self.dl_studio.path_saved_model["encoder"])
 
     def save_decoder(self, decoder):
         "Save the trained decoder to a disk file"       
         torch.save(decoder.state_dict(), self.dl_studio.path_saved_model["decoder"])
 
+    def save_embeddings_generator_en(self, embeddings_generator_en):
+        torch.save(embeddings_generator_en.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_en"])
+
+    def save_embeddings_generator_es(self, embeddings_generator_es):
+        torch.save(embeddings_generator_es.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_es"])
+
     def save_checkpoint_encoder(self, encoder, dir_name, epoch_index):
         "Save the encoder checkpoint"       
         # if os.path.exists(dir_name + "/encoder_" + str(epoch_index - 1)):              
         #    os.remove(dir_name + "/encoder_" + str(epoch_index - 1))
         torch.save(encoder.state_dict(), dir_name + "/encoder_" + str(epoch_index))
 
     def save_checkpoint_decoder(self, decoder, dir_name, epoch_index):
         "Save the decoder checkpoint"       
         # if os.path.exists(dir_name + "/decoder_" + str(epoch_index - 1)):              
         #    os.remove(dir_name + "/decoder_" + str(epoch_index - 1))
         torch.save(decoder.state_dict(), dir_name + "/decoder_" + str(epoch_index))
 
 
+
+
     def run_code_for_training_TransformerFG(self, dls, master_encoder, master_decoder, display_train_loss=False, 
                                                                                                 checkpoints_dir='checkpoints'):
         """
         A particular feature of TransformerFG is how it is trained. Training a transformer as 
         conceptualized in the paper by Vaswani et al. requires a carefully designed warm-up stage 
         at the beginning in which you start with a very small learning rate that is gradually 
         increased to a set maximum value in a specific number of training iterations.  The 
@@ -1007,33 +1001,38 @@
                 running_loss += loss_normed
                 if iter % 200 == 199:    
                     avg_loss = running_loss / float(200)
                     training_loss_tally.append(avg_loss)
                     running_loss = 0.0
                     current_time = time.perf_counter()
                     time_elapsed = current_time-start_time
-                    print("[epoch:%2d  iter:%4d  elapsed_time: %4d secs]     loss: %.4f" % (epoch,iter+1,time_elapsed,avg_loss)) 
+                    print("[epoch:%2d/%d  iter:%4d  elapsed_time: %4d secs]     loss: %.4f" % (epoch+1,self.dl_studio.epochs,iter+1,time_elapsed,avg_loss)) 
                     accum_times.append(current_time-start_time)
             ##  At the beginning of the training session, the designated checkpoint_dir has already been flushed
             if self.save_checkpoints and  (epoch + 1) % 5 == 0:
                 self.save_checkpoint_encoder(master_encoder, checkpoints_dir, epoch)
                 self.save_checkpoint_decoder(master_decoder, checkpoints_dir, epoch)
+                self.save_embeddings_generator_en(embeddings_generator_en, checkpoints_dir, epoch)
+                self.save_embeddings_generator_es(embeddings_generator_es, checkpoints_dir, epoch)
                 print("Checkpoint saved at the end of epoch %d" % (epoch))
         print("\nFinished Training\n")
         self.save_encoder(master_encoder)       
         self.save_decoder(master_decoder)       
+        self.save_embeddings_generator_en(embeddings_generator_en)       
+        self.save_embeddings_generator_es(embeddings_generator_es)       
         if display_train_loss:
             plt.figure(figsize=(10,5))
-            plt.title("Training Loss vs. Iterations")
+            plt.title("FG Training Loss vs. Iterations")
             plt.plot(training_loss_tally)
             plt.xlabel("iterations")
             plt.ylabel("training loss")
-            plt.legend()
-            plt.savefig("training_loss.png")
-            plt.show()
+            plt.legend(["Plot of loss versus iterations"], fontsize="x-large")
+            plt.savefig("training_loss_FG.png")
+#            plt.show()
+
 
 
     def run_code_for_evaluating_TransformerFG(self, master_encoder, master_decoder, result_file=None):
         """
         The main difference between the training code shown in the previous function and the
         evaluation code shown here is with regard to the input to MasterDecoder and how we
         process its output. As shown in the previous function, for the training loop, the
@@ -1051,23 +1050,26 @@
         predicted log probabilities (logprob) over the target vocabulary for every word 
         position in the target language; and (2) for each target-language word position, 
         the word_vocab_index at which the logprob is maximum.  The loss calculation in
         the training code was based on the former.  ON the other hand, as shown in line (H)
         below, it is the latter that lets us do the the translations in the target words
         in line (I).
         """
-        if result_file is not None:
-            FILE = open(result_file, 'w')
         master_encoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['encoder']))
         master_decoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['decoder']))
+        embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size)
+        embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size)
+        embeddings_generator_en.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_en']))
+        embeddings_generator_es.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_es']))
         master_encoder.to(self.dl_studio.device)
         master_decoder.to(self.dl_studio.device)     
-        embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size).to(self.dl_studio.device)
-        embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size).to(self.dl_studio.device)
+        embeddings_generator_en.to(self.dl_studio.device)
+        embeddings_generator_es.to(self.dl_studio.device)        
         self.debug = False
+        FILE = open("translations_with_FG_" + str(self.dl_studio.epochs) + ".txt", 'w')
         with torch.no_grad():
             for iter in range(20):
                 starter_stub_for_translation = ['SOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS']      ## (A)
                 batched_pairs = random.sample(self.training_corpus, 1)                                                     ## (B)
                 source_sentences = [pair[0] for pair in batched_pairs]
                 target_sentences = [pair[1] for pair in batched_pairs]
                 if self.debug:
@@ -1085,17 +1087,17 @@
                 _, predicted_word_index_values = master_decoder(starter_stub_tensor, master_encoder_output)                ## (H)
                 predicted_word_index_values = predicted_word_index_values[0].unsqueeze(1)
                 decoded_words = [self.es_index_2_word[predicted_word_index_values[di].item()] 
                                                                         for di in range(self.max_seq_length)]              ## (I)
                 output_sentence = " ".join(decoded_words)                                                                 
                 print("\n\n\nThe input sentence pair: ", source_sentences, target_sentences)                             
                 print("\nThe translation produced by TransformerFG: ", output_sentence)
-                if result_file is not None:
-                    FILE.write("\n\n\nThe input sentence pair: %s   %s" %  (source_sentences, target_sentences))
-                    FILE.write("\nThe translation produced by TransformerFG:  %s" % output_sentence)
+                FILE.write("\n\n\nThe input sentence pair: %s    %s" % (source_sentences, target_sentences))
+                FILE.write("\nThe translation produced by TransformerPreLN:  %s" % output_sentence)
+
 
 
     def run_code_for_evaluating_checkpoint(self, master_encoder, master_decoder, checkpoints_dir, checkpoint_index, result_file=None):
         """
         Training transformer networks has always been difficulty and that's the case even with 
         learning-rate warm-up and other mitigating strategies.  DLStudio provides you with 
         checkpoints for making transformer training a little bit less frustrated.  While you are 
@@ -1269,22 +1271,24 @@
         def _update_learning_rate(self):
             ''' Learning rate scheduling per step '''
             self.n_steps += 1
             lr = self.lr_mul * self._get_lr_scale()
             for param_group in self._optimizer.param_groups:
                 param_group['lr'] = lr
 
-################################  END Definition of Inner Class TransformerFG  END  #################################
+###################################  END Definition of Class TransformerFG  END  ####################################
 #####################################################################################################################
 #####################################################################################################################
 
 
 
 ###%%%
-###############################  Start Definition of Inner Class TransformerPreLN  ##################################
+#####################################################################################################################
+##################################  Start Definition of Class TransformerPreLN  #####################################
+#####################################################################################################################
 class TransformerPreLN(nn.Module):             
     """
     TransformerPreLN stands for "Transformer Pre Layer Norm".
 
     As with the TransformerFG class, the goal of TransformerPreLN is to serve as an 
     instructional aid in understanding the basic concepts of attention-based learning with
     neural networks.
@@ -1539,15 +1543,15 @@
             div_term =  1.0 / (100.0 ** ( 2.0 * torch.arange(0, self.embedding_size, 2) / float(self.embedding_size) ))
             position_encodings[:, :, 0::2] =  torch.sin(word_positions * div_term)                                     ## (F)
             position_encodings[:, :, 1::2] =  torch.cos(word_positions * div_term)                                     ## (G)
             return sentence_tensor + position_encodings
 
 
     ###%%%
-    #####################################   Encoder Code TransformerPreLN  ###############################################
+    #####################################   Encoder Code in TransformerPreLN  ############################################
 
     class MasterEncoder(nn.Module):
         """
         The purpose of the MasterEncoder is to invoke a stack of BasicEncoder instances on a
         source-language sentence tensor. The output of each BasicEncoder is fed as input to the 
         next BasicEncoder in the cascade, as illustrated in the loop in Line B below.  The stack
         of BasicEncoder instances is constructed in Line A.
@@ -1613,15 +1617,15 @@
             basic_encoder_out = basic_encoder_out.view(sentence_tensor.shape[0], self.max_seq_length, self.embedding_size ) 
             basic_encoder_out =  basic_encoder_out  + input_for_FFN
             return basic_encoder_out
 
 
 
     ###%%%
-    ####################################  Self Attention Code TransformerPreLN ###########################################
+    ####################################  Self Attention Code in TransformerPreLN ########################################
 
     class SelfAttention(nn.Module):
         """
         As described in the doc section of the BasicEncoder class, in each BasicEncoder you have 
         a layer of SelfAttention followed by a Fully-Connected layer.  The SelfAttention layer 
         concatenates the outputs from all AttentionHead instances and presents that concatenated 
         output as its own output. If the input sentence consists of W words at most and if the 
@@ -1766,38 +1770,35 @@
         ClassPath:  TransformerPreLN   ->   AttentionHead
         """
         def __init__(self, dl_studio, max_seq_length, qkv_size, num_atten_heads):
             super(TransformerPreLN.AttentionHead, self).__init__()
             self.dl_studio = dl_studio
             self.qkv_size = qkv_size
             self.max_seq_length = max_seq_length
-            self.WQ =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (B)
-            self.WK =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (C)
-            self.WV =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (D)
+            self.WQ =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (B)
+            self.WK =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (C)
+            self.WV =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (D)
             self.softmax = nn.Softmax(dim=1)                                                                           ## (E)
 
-        def forward(self, sentence_portion):                                                                           ## (F)
-            Q = self.WQ( sentence_portion.reshape(sentence_portion.shape[0],-1).float() )                              ## (G)
-            K = self.WK( sentence_portion.reshape(sentence_portion.shape[0],-1).float() )                              ## (H)
-            V = self.WV( sentence_portion.reshape(sentence_portion.shape[0],-1).float() )                              ## (I)
-            Q = Q.view(sentence_portion.shape[0], self.max_seq_length, self.qkv_size)                                  ## (J)
-            K = K.view(sentence_portion.shape[0], self.max_seq_length, self.qkv_size)                                  ## (K)
-            V = V.view(sentence_portion.shape[0], self.max_seq_length, self.qkv_size)                                  ## (L)
-            A = K.transpose(2,1)                                                                                       ## (M)
-            QK_dot_prod = Q @ A                                                                                        ## (N)
-            rowwise_softmax_normalizations = self.softmax( QK_dot_prod )                                               ## (O)
-            Z = rowwise_softmax_normalizations @ V                                                                     ## (P)
+        def forward(self, sent_embed_slice):                                                                           ## (F)
+            Q = self.WQ( sent_embed_slice )                                                                            ## (G)
+            K = self.WK( sent_embed_slice )                                                                            ## (H)
+            V = self.WV( sent_embed_slice )                                                                            ## (I)
+            A = K.transpose(2,1)                                                                                       ## (J)
+            QK_dot_prod = Q @ A                                                                                        ## (K)
+            rowwise_softmax_normalizations = self.softmax( QK_dot_prod )                                               ## (L)
+            Z = rowwise_softmax_normalizations @ V                                                                     ## (M)
             ## torch.tensor creates a new tensor that needs to be moved to GPU
-            coeff = 1.0/torch.sqrt(torch.tensor([self.qkv_size]).float()).to(self.dl_studio.device)                    ## (Q)
-            Z = coeff * Z                                                                                              ## (R)
+            coeff = 1.0/torch.sqrt(torch.tensor([self.qkv_size]).float()).to(self.dl_studio.device)                    ## (N)
+            Z = coeff * Z                                                                                              ## (O)
             return Z
 
 
     ###%%%
-    ####################################  Cross Attention Code TransformerPreLN  #########################################
+    ####################################  Cross Attention Code in TransformerPreLN  ######################################
 
     class CrossAttention(nn.Module):
         """
         To understand the implementation of cross attention, a good starting point would be to 
         go through the documentation section provided for the SelfAttention and AttentionHead
         classes.  Whereas self-attention consists of taking dot products the query vectors for
         the individual words in a sentence with the key vectors for all the words in order to
@@ -1852,33 +1853,30 @@
 
     class CrossAttentionHead(nn.Module):
         def __init__(self, dl_studio, max_seq_length, qkv_size, num_atten_heads):
             super(TransformerPreLN.CrossAttentionHead, self).__init__()
             self.dl_studio = dl_studio
             self.qkv_size = qkv_size
             self.max_seq_length = max_seq_length
-            self.WQ =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (B)
-            self.WK =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (C)
-            self.WV =  nn.Linear( max_seq_length * self.qkv_size, max_seq_length * self.qkv_size )                     ## (D)
+            self.WQ =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (B)
+            self.WK =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (C)
+            self.WV =  nn.Linear( self.qkv_size, self.qkv_size )                                                       ## (D)
             self.softmax = nn.Softmax(dim=1)                                                                           ## (E)
 
-        def forward(self, basic_decoder_portion, final_encoder_portion):                                               ## (F)
-            Q = self.WQ( basic_decoder_portion.reshape(final_encoder_portion.shape[0],-1).float() )                    ## (G)
-            K = self.WK( final_encoder_portion.reshape(final_encoder_portion.shape[0],-1).float() )                    ## (H)
-            V = self.WV( final_encoder_portion.reshape(final_encoder_portion.shape[0],-1).float() )                    ## (I)
-            Q = Q.view(final_encoder_portion.shape[0], self.max_seq_length, self.qkv_size)                             ## (J)
-            K = K.view(final_encoder_portion.shape[0], self.max_seq_length, self.qkv_size)                             ## (K)
-            V = V.view(final_encoder_portion.shape[0], self.max_seq_length, self.qkv_size)                             ## (L)
-            A = K.transpose(2,1)                                                                                       ## (M)
-            QK_dot_prod = Q @ A                                                                                        ## (N)
-            rowwise_softmax_normalizations = self.softmax( QK_dot_prod )                                               ## (O)
-            Z = rowwise_softmax_normalizations @ V                                                                     ## (P)
+        def forward(self, basic_decoder_slice, final_encoder_slice):                                                   ## (F)
+            Q = self.WQ( basic_decoder_slice )                                                                         ## (G)
+            K = self.WK( final_encoder_slice )                                                                         ## (H)
+            V = self.WV( final_encoder_slice )                                                                         ## (I)
+            A = K.transpose(2,1)                                                                                       ## (J)
+            QK_dot_prod = Q @ A                                                                                        ## (K)
+            rowwise_softmax_normalizations = self.softmax( QK_dot_prod )                                               ## (L)
+            Z = rowwise_softmax_normalizations @ V                                                                     ## (M)
             ## torch.tensor creates a new tensor that needs to be moved to GPU
-            coeff = 1.0/torch.sqrt(torch.tensor([self.qkv_size]).float()).to(self.dl_studio.device)                    ## (Q)
-            Z = coeff * Z                                                                                              ## (R)
+            coeff = 1.0/torch.sqrt(torch.tensor([self.qkv_size]).float()).to(self.dl_studio.device)                    ## (N)
+            Z = coeff * Z                                                                                              ## (O)
             return Z
 
 
     ###%%%
     #######################################   Decoder Code TransformerPreLN ##############################################
 
     class BasicDecoderWithMasking(nn.Module):
@@ -2006,14 +2004,20 @@
         "Save the trained encoder to a disk file"       
         torch.save(encoder.state_dict(), self.dl_studio.path_saved_model["encoder"])
 
     def save_decoder(self, decoder):
         "Save the trained decoder to a disk file"       
         torch.save(decoder.state_dict(), self.dl_studio.path_saved_model["decoder"])
 
+    def save_embeddings_generator_en(self, embeddings_generator_en):
+        torch.save(embeddings_generator_en.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_en"])
+
+    def save_embeddings_generator_es(self, embeddings_generator_es):
+        torch.save(embeddings_generator_es.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_es"])
+
     def save_checkpoint_encoder(self, encoder, dir_name, epoch_index):
         "Save the encoder checkpoint"       
         # if os.path.exists(dir_name + "/encoder_" + str(epoch_index - 1)):              
         #    os.remove(dir_name + "/encoder_" + str(epoch_index - 1))
         torch.save(encoder.state_dict(), dir_name + "/encoder_" + str(epoch_index))
 
     def save_checkpoint_decoder(self, decoder, dir_name, epoch_index):
@@ -2124,32 +2128,35 @@
                 running_loss += loss_normed                                                                                  ## (X)
                 if iter % 200 == 199:         
                     avg_loss = running_loss / float(200)
                     training_loss_tally.append(avg_loss)
                     running_loss = 0.0
                     current_time = time.perf_counter()
                     time_elapsed = current_time-start_time
-                    print("[epoch:%2d  iter:%4d  elapsed_time: %4d secs]     loss: %.4f" % (epoch, iter+1, time_elapsed,avg_loss))
+                    print("[epoch:%2d/%d  iter:%4d  elapsed_time: %4d secs]     loss: %.4f" % (epoch+1,self.dl_studio.epochs,iter+1, time_elapsed,avg_loss))
                     accum_times.append(current_time-start_time)
             ##  At the beginning of the training session, the designated checkpoint_dir has already been flushed
-            if self.save_checkpoints and  (epoch + 1) % 5 == 0:                            ## will save at epochs 4, 9, 14, 19, etc
-                self.save_checkpoint_encoder(master_encoder, checkpoints_dir, epoch)
-                self.save_checkpoint_decoder(master_decoder, checkpoints_dir, epoch)
+            if self.save_checkpoints and  (epoch + 1) % 5 == 0:                      
+                self.save_checkpoint_encoder(master_encoder, checkpoints_dir, epoch+1)
+                self.save_checkpoint_decoder(master_decoder, checkpoints_dir, epoch+1)
                 print("Checkpoint saved at the end of epoch %d" % (epoch))
         print("\nFinished Training\n")
         self.save_encoder(master_encoder)       
         self.save_decoder(master_decoder)       
+        self.save_embeddings_generator_en(embeddings_generator_en)       
+        self.save_embeddings_generator_es(embeddings_generator_es)       
         if display_train_loss:
             plt.figure(figsize=(10,5))
-            plt.title("Training Loss vs. Iterations")
+            plt.title("PreLN Training Loss vs. Iterations")
             plt.plot(training_loss_tally)
             plt.xlabel("iterations")
             plt.ylabel("training loss")
-            plt.legend()
-            plt.savefig("training_loss.png")
+#            plt.legend()
+            plt.legend(["Plot of loss versus iterations"], fontsize="x-large")
+            plt.savefig("training_loss_PreLN.png")
             plt.show()
 
     def run_code_for_evaluating_TransformerPreLN(self, master_encoder, master_decoder):
         """
         The main difference between the training code shown in the previous function and the
         evaluation code shown here is with regard to the input to MasterDecoder and how we process 
         its output. As shown in the previous function, for the training loop, the input to 
@@ -2167,19 +2174,24 @@
         (2) for each target-language word position, the word_vocab_index at which the logprob is 
         maximum.  The loss calculation in the training code was based on the former.  ON the other 
         hand, as shown in line (H) below, it is the latter that lets us do the the translations in 
         the target words in line (I).
         """
         master_encoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['encoder']))
         master_decoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['decoder']))
+        embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size)
+        embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size)
+        embeddings_generator_en.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_en']))
+        embeddings_generator_es.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_es']))
         master_encoder.to(self.dl_studio.device)
         master_decoder.to(self.dl_studio.device)     
-        embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size).to(self.dl_studio.device)
-        embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size).to(self.dl_studio.device)
+        embeddings_generator_en.to(self.dl_studio.device)
+        embeddings_generator_es.to(self.dl_studio.device)        
         self.debug = False
+        FILE = open("translations_with_PreLN_" + str(self.dl_studio.epochs) + ".txt", 'w')
         with torch.no_grad():
             for iter in range(20):
                 starter_stub_for_translation = ['SOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS']      ## (A)
                 batched_pairs = random.sample(self.training_corpus, 1)                                                     ## (B)
                 source_sentences = [pair[0] for pair in batched_pairs]
                 target_sentences = [pair[1] for pair in batched_pairs]
                 if self.debug:
@@ -2197,14 +2209,16 @@
                 _, predicted_word_index_values = master_decoder(starter_stub_tensor, master_encoder_output)                ## (H)
                 predicted_word_index_values = predicted_word_index_values[0].unsqueeze(1)
                 decoded_words = [self.es_index_2_word[predicted_word_index_values[di].item()] 
                                                                         for di in range(self.max_seq_length)]              ## (I)
                 output_sentence = " ".join(decoded_words)                                                                 
                 print("\n\n\nThe input sentence pair: ", source_sentences, target_sentences)                             
                 print("\nThe translation produced by TransformerPreLN: ", output_sentence)
+                FILE.write("\n\n\nThe input sentence pair: %s    %s" % (source_sentences, target_sentences))
+                FILE.write("\nThe translation produced by TransformerPreLN:  %s" % output_sentence)
 
 
     def run_code_for_evaluating_checkpoint(self, master_encoder, master_decoder, checkpoints_dir, checkpoint_index, result_file=None):
         """
         Training transformer networks has always been difficulty and that's the case even with 
         learning-rate warm-up and other mitigating strategies.  DLStudio provides you with 
         checkpoints for making transformer training a little bit less frustrated.  While you are 
@@ -2309,19 +2323,499 @@
         _, predicted_word_index_values = master_decoder(starter_stub_tensor, master_encoder_output)              
         predicted_word_index_values = predicted_word_index_values[0].unsqueeze(1)
         decoded_words = [self.es_index_2_word[predicted_word_index_values[di].item()] for di in range(self.max_seq_length)]    
         output_sentence = " ".join(decoded_words)                                                                 
         print("\nThe translation produced by TransformerPreLN: ", output_sentence)
         return output_sentence
 
-################################  END Definition of Inner Class TransformerPreLN  ###################################
+##################################  END Definition of Class TransformerPreLN  #######################################
 #####################################################################################################################
 #####################################################################################################################
 
 
+
+###%%%
+#####################################################################################################################
+####################################  Start Definition of Class visTransformer  #####################################
+#####################################################################################################################
+
+class visTransformer(nn.Module):             
+    """
+    visTransformer stands for "Transformer for Vision Applications"
+
+    ClassPath:  visTransformer
+    """
+    def __init__(self, dl_studio, patch_size, embedding_size, num_basic_encoders, num_atten_heads, save_checkpoints=True, checkpoint_freq=10):
+        super(visTransformer, self).__init__()
+        self.dl_studio = dl_studio
+        self.batch_size = dl_studio.batch_size
+        self.learning_rate = dl_studio.learning_rate
+        self.train_data_loader =  None                       ## will be set when you call vlt.load_cifar_10_dataset()
+        self.test_data_loader = None                         ## will be set when you call vlt.load_cifar_10_dataset()
+        self.num_patches_in_image =  (dl_studio.image_size[0] // patch_size[0] ) * (dl_studio.image_size[1] // patch_size[1] )
+        self.checkpoint_freq = checkpoint_freq
+        self.patch_size  =  patch_size
+        self.patch_dimen = (patch_size[0] * patch_size[1]) * 3
+        self.embedding_size = embedding_size
+        self.num_basic_encoders = num_basic_encoders
+        self.num_atten_heads = num_atten_heads
+        self.save_checkpoints = save_checkpoints
+        self.max_seq_length = self.num_patches_in_image + 1
+        self.master_encoder = visTransformer.MasterEncoder(dl_studio, self, num_basic_encoders, num_atten_heads)
+        self.fc =  nn.Sequential( 
+                                  nn.Dropout(p=0.1),
+                                  nn.Linear(embedding_size, 512),
+                                  nn.ReLU(inplace=True),
+                                  nn.Linear(512, len(dl_studio.class_labels)),
+                                )
+        self.class_token = nn.Parameter(torch.randn((1, 1, embedding_size))).cuda()
+
+    def forward(self, x):
+        class_token = self.class_token.expand(x.shape[0], -1, -1)
+        x = torch.cat((class_token, x), dim=1)
+        x = self.master_encoder(x)
+        predicted_class_tokens = x[:,0]
+        output = self.fc(predicted_class_tokens)
+        return output
+
+
+
+    class PatchEmbeddingGenerator(nn.Module):
+        """
+        See Slide 89 of my Week 14 lecture on Transformers for a visualization of the patches
+        in the input image and their representation by embedding vectors.
+
+        ClassPath:  VisTransformer   ->   PatchEmbeddingGenerator
+        """
+        def __init__(self, vis_xformer):
+            super(visTransformer.PatchEmbeddingGenerator, self).__init__()
+            self.num_patches_in_image = vis_xformer.num_patches_in_image
+            self.patch_dimen = vis_xformer.patch_dimen                           ## (num_ of_pixels) * (3_color_channels)
+            self.embedding_size = vis_xformer.embedding_size                                             
+            self.embed = nn.Linear(self.patch_dimen, self.embedding_size)                         
+            self.positional_encodings = nn.Parameter(torch.randn((1, self.num_patches_in_image, self.embedding_size)))
+    
+        def forward(self, x):                                                                
+            x = x.reshape(x.shape[0], -1, self.patch_dimen).cuda()    
+            patch_embeddings = self.embed(x)
+            position_coded_embeddings = patch_embeddings  +  self.positional_encodings
+            return position_coded_embeddings
+
+
+    ###%%%
+    ###################################   Encoder Code for visTransformer  #############################################
+
+    class MasterEncoder(nn.Module):
+        """
+        See the doc string for the same class for the TransformerFG implementation
+
+        ClassPath:  visTransformer   ->   MasterEncoder
+        """
+        def __init__(self, dls, xformer, num_basic_encoders, num_atten_heads):
+            super(visTransformer.MasterEncoder, self).__init__()
+            self.max_seq_length = xformer.max_seq_length
+            self.basic_encoder_arr = nn.ModuleList( [xformer.BasicEncoder(dls, xformer,
+                                                      num_atten_heads) for _ in range(num_basic_encoders)] )        
+        def forward(self, sentence_tensor):
+            out_tensor = sentence_tensor
+            for i in range(len(self.basic_encoder_arr)):                                                            
+                out_tensor = self.basic_encoder_arr[i](out_tensor)
+            return out_tensor
+
+
+    class BasicEncoder(nn.Module):
+        """
+        See the doc string for the same class for the TransformerFG implementation
+
+        ClassPath:  visTransformer  ->   BasicEncoder
+        """
+        def __init__(self, dls, xformer, num_atten_heads):
+            super(visTransformer.BasicEncoder, self).__init__()
+            self.dls = dls
+            self.embedding_size = xformer.embedding_size                                             
+            self.max_seq_length = xformer.max_seq_length
+            self.num_atten_heads = num_atten_heads
+            self.self_attention_layer = xformer.SelfAttention(dls, xformer, num_atten_heads)                         
+            self.norm1 = nn.LayerNorm(self.embedding_size)                                                           
+            ## What follows are the linear layers for the FFN (Feed Forward Network) part of a BasicEncoder
+            self.W1 =  nn.Linear( self.max_seq_length * self.embedding_size, self.max_seq_length * 2 * self.embedding_size )
+            self.W2 =  nn.Linear( self.max_seq_length * 2 * self.embedding_size, self.max_seq_length * self.embedding_size ) 
+            self.norm2 = nn.LayerNorm(self.embedding_size)                                                           
+
+        def forward(self, sentence_tensor):
+            sentence_tensor = sentence_tensor.float()
+            self_atten_out = self.self_attention_layer(sentence_tensor).to(self.dls.device)                          
+            normed_atten_out = self.norm1(self_atten_out + sentence_tensor)                                          
+            basic_encoder_out =  nn.ReLU()(self.W1( normed_atten_out.view(sentence_tensor.shape[0],-1) ))            
+            basic_encoder_out =  self.W2( basic_encoder_out )                                                        
+            basic_encoder_out = basic_encoder_out.view(sentence_tensor.shape[0], self.max_seq_length, self.embedding_size ) 
+            ## for the residual connection and layer norm for FC layer:
+            basic_encoder_out =  self.norm2(basic_encoder_out  + normed_atten_out)                                   
+            return basic_encoder_out
+
+
+
+    ###%%%
+    ##################################  Self Attention Code for visTransformer #########################################
+
+    class SelfAttention(nn.Module):
+        """
+        See the doc string for the same class for the TransformerFG implementation
+
+        ClassPath:  visTransformer  ->   SelfAttention
+        """
+        def __init__(self, dls, xformer, num_atten_heads):
+            super(visTransformer.SelfAttention, self).__init__()
+            self.dl_studio = dls
+            self.max_seq_length = xformer.max_seq_length                                                     
+            self.embedding_size = xformer.embedding_size
+            self.num_atten_heads = num_atten_heads
+            self.qkv_size = self.embedding_size // num_atten_heads
+            self.attention_heads_arr = nn.ModuleList( [xformer.AttentionHead(dls, self.max_seq_length, 
+                                    self.qkv_size, num_atten_heads)  for _ in range(num_atten_heads)] )               
+
+        def forward(self, sentence_tensor):                                                                           
+            concat_out_from_atten_heads = torch.zeros( sentence_tensor.shape[0], self.max_seq_length, 
+                                                                  self.num_atten_heads * self.qkv_size).float()
+            for i in range(self.num_atten_heads):                                                                     
+                sentence_embed_slice = sentence_tensor[:, :, i * self.qkv_size : (i+1) * self.qkv_size]
+                concat_out_from_atten_heads[:, :, i * self.qkv_size : (i+1) * self.qkv_size] =          \
+                                                               self.attention_heads_arr[i](sentence_embed_slice)   
+            return concat_out_from_atten_heads
+
+
+    class AttentionHead(nn.Module):
+        """
+        See the doc string for the same class in the TransformerFG implementation
+
+        ClassPath:  visTransformer   ->   AttentionHead
+        """
+        def __init__(self, dl_studio, max_seq_length, qkv_size, num_atten_heads):
+            super(visTransformer.AttentionHead, self).__init__()
+            self.dl_studio = dl_studio
+            self.qkv_size = qkv_size
+            self.max_seq_length = max_seq_length
+            self.WQ =  nn.Linear( self.qkv_size, self.qkv_size, bias=False )               
+            self.WK =  nn.Linear( self.qkv_size, self.qkv_size, bias=False )               
+            self.WV =  nn.Linear( self.qkv_size, self.qkv_size, bias=False )               
+            self.softmax = nn.Softmax(dim=1)                                                                     
+
+        def forward(self, sent_embed_slice):           ## sent_embed_slice == sentence_embedding_slice           
+            Q = self.WQ( sent_embed_slice )
+            K = self.WK( sent_embed_slice )
+            V = self.WV( sent_embed_slice )
+            A = K.transpose(2,1)                                                                                 
+            QK_dot_prod = Q @ A                                                                                  
+            rowwise_softmax_normalizations = self.softmax( QK_dot_prod )                                         
+            Z = rowwise_softmax_normalizations @ V                                                               
+            coeff = 1.0/torch.sqrt(torch.tensor([self.qkv_size]).float()).to(self.dl_studio.device)              
+            Z = coeff * Z                                                                                        
+            return Z
+
+
+
+    ###%%%
+    ##############################  Training and Evaluation for visTransformer  ########################################
+
+    def save_visTran(self, networks):
+        "Save the trained visTran model to a disk file"       
+        for i,net in enumerate(networks):
+            torch.save(net.state_dict(), self.dl_studio.path_saved_model + "_" + str(i))
+
+    def save_checkpoint_visTran(self, networks, dir_name, epoch_index):
+        "Save the visTransformer checkpoint"       
+        for i,net in enumerate(networks):
+            torch.save(net.state_dict(), dir_name + "/checkpoint_" + str(i) + "_for_epoch_" + str(epoch_index))
+
+    def load_cifar_10_dataset(self):       
+        '''
+        For the doc string, see the same method in the main DLStudio module file 
+        '''
+        ##   But then the call to Normalize() changes the range to -1.0-1.0 float vals.
+        transform = tvt.Compose([tvt.ToTensor(),
+                                 tvt.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))])    ## accuracy: 51%
+        ##  Define where the training and the test datasets are located:
+        train_data_loc = torchvision.datasets.CIFAR10(root=self.dl_studio.dataroot, train=True, download=True, transform=transform)
+        test_data_loc = torchvision.datasets.CIFAR10(root=self.dl_studio.dataroot, train=False, download=True, transform=transform)
+        ##  Now create the data loaders:
+        self.train_data_loader = torch.utils.data.DataLoader(train_data_loc,batch_size=self.batch_size, shuffle=True, num_workers=2)
+        self.test_data_loader = torch.utils.data.DataLoader(test_data_loc,batch_size=self.batch_size, shuffle=False, num_workers=1)
+
+
+
+    def run_code_for_training_visTransformer(self, dls, vis_transformer, display_train_loss=False, checkpoint_dir='checkpoints'):
+        """
+        The training of visTransformer is based on the code shown earlier in the TransformerFG
+        class.
+        """
+        if os.path.exists(checkpoint_dir):  
+            """
+            For the visTransformer script in ExamplesTransformers, checkpoint_dir is "checkpoints_visTrans"
+            """
+            files = glob.glob(checkpoint_dir + "/*")
+            for file in files: 
+                if os.path.isfile(file): 
+                    os.remove(file) 
+                else: 
+                    files = glob.glob(file + "/*") 
+                    list(map(lambda x: os.remove(x), files)) 
+        else: 
+            os.mkdir(checkpoint_dir)   
+
+        vis_encoder_network = self.to(self.dl_studio.device)
+        optimizer = torch.optim.Adam(vis_encoder_network.parameters(), lr = self.learning_rate, betas = (0.9, 0.99))
+        patch_embedding_generator = self.PatchEmbeddingGenerator( self )
+        patch_embedding_generator.to(self.dl_studio.device)
+        criterion = nn.CrossEntropyLoss()                                                                                       
+        accum_times = []
+        start_time = time.perf_counter()
+        training_loss_tally = []
+        self.debug = False
+        print("")
+        batch_size = self.dl_studio.batch_size
+        print("\n\n batch_size: ", batch_size)
+        print("\n\n number of batches in the dataset: ", len(self.train_data_loader))
+
+        for epoch in range(self.dl_studio.epochs):                                                              
+            print("")
+            running_loss = 0.0
+            for i, data in enumerate(self.train_data_loader):                                    
+                input_images, labels = data     
+                if input_images.shape[0] != self.batch_size: break
+                input_images.to(self.dl_studio.device)
+                labels.to(self.dl_studio.device)
+                patch_sequences = input_images.unfold(2, self.patch_size[0], self.patch_size[1]).unfold(3, self.patch_size[0], self.patch_size[1])
+                patch_sequence_embeddings = patch_embedding_generator( patch_sequences )
+                vis_encoder_network.zero_grad()
+                encoder_output = vis_encoder_network( patch_sequence_embeddings )
+                loss  =  criterion( encoder_output, labels.cuda() )
+                loss.backward()                                                                                        
+                optimizer.step()
+                running_loss += loss
+                if i % 200 == 199:    
+                    avg_loss = running_loss / float(200)
+                    training_loss_tally.append(avg_loss.item())
+                    running_loss = 0.0
+                    current_time = time.perf_counter()
+                    time_elapsed = current_time-start_time
+                    print("[epoch:%2d/%2d  i:%4d  elapsed_time: %4d secs]     loss: %.4f" % (epoch+1, self.dl_studio.epochs, i+1,time_elapsed,avg_loss)) 
+                    accum_times.append(current_time-start_time)
+            ##  At the beginning of the training session, the designated checkpoint_dir has already been flushed
+            if self.save_checkpoints and  (epoch + 1) % self.checkpoint_freq == 0:
+                self.save_checkpoint_visTran( (vis_encoder_network, patch_embedding_generator), checkpoint_dir, epoch+1)
+                print("\nCheckpoint saved at the end of epoch %d" % (epoch+1))
+        print("\nFinished Training\n")
+        self.save_visTran( (vis_encoder_network, patch_embedding_generator) )
+        if display_train_loss:
+            plt.figure(figsize=(10,5))
+            plt.title("Training Loss vs. Iterations")
+            plt.plot(training_loss_tally)
+            plt.xlabel("iterations")
+            plt.ylabel("training loss")
+            plt.legend(["Plot of loss versus iterations"], fontsize="x-large")
+            plt.savefig("training_loss.png")
+            plt.show()
+
+
+    def run_code_for_evaluating_visTransformer(self):
+        class_labels = self.dl_studio.class_labels
+        filename_for_results = "classification_results_" + str(self.dl_studio.epochs) + ".txt"
+        FILE = open(filename_for_results, 'w')
+        correct = 0
+        total = 0
+        confusion_matrix = torch.zeros(len(class_labels), len(class_labels))
+        class_correct = [0] * len(class_labels)
+        class_total = [0] * len(class_labels)
+        patch_embedding_generator = self.PatchEmbeddingGenerator( self )
+        patch_embedding_generator.load_state_dict(torch.load(self.dl_studio.path_saved_model + "_1"))
+        patch_embedding_generator.to(self.dl_studio.device)
+        encoder_network = self
+        encoder_network.load_state_dict(torch.load(self.dl_studio.path_saved_model  + "_0"))
+        encoder_network.to(self.dl_studio.device)
+        debug = False
+        with torch.no_grad():
+            for i, data in enumerate(self.test_data_loader):                                    
+                if i > 999: break
+                if debug:
+                    print("\n\n\n=========Showing results for test batch %d===============" % i)
+                test_images, labels = data     
+                if test_images.shape[0] != self.batch_size: break
+                if debug:
+                    logger.setLevel(100)
+                    plt.figure(figsize=[6,3])
+                    plt.imshow(np.transpose(torchvision.utils.make_grid(input_images, normalize=False, padding=3, pad_value=255).cpu(), (1,2,0)))
+                    plt.show()
+                    logger.setLevel(old_level)
+                test_images.to(self.dl_studio.device)
+                labels.to(self.dl_studio.device)
+                patch_sequences = test_images.unfold(2, self.patch_size[0], self.patch_size[1]).unfold(3, self.patch_size[0], self.patch_size[1]) 
+                patch_sequence_embeddings = patch_embedding_generator( patch_sequences )
+                encoder_output = encoder_network( patch_sequence_embeddings )
+                _, predicted = torch.max(encoder_output.data, 1)
+                predicted = predicted.tolist()
+                if debug:
+                    print("\npredicted_class_labels: ")
+                    print(predicted)             
+                symbolic_name_prediction = [class_labels[index] for index in predicted]
+                symbolic_name_gt = [class_labels[index] for index in labels]
+                if debug:
+                    print("\nimage labels ground truth: ", symbolic_name_gt)
+                    print("\npredicted_test_image_class_label: ", symbolic_name_prediction)
+                for label,prediction in zip(labels, predicted):
+                    confusion_matrix[label][prediction] += 1
+                total += labels.shape[0]
+                labels = labels.tolist()
+                comp =  torch.LongTensor(predicted) == torch.LongTensor(labels)
+                correct += comp.sum().item()
+                for j in range(self.batch_size):
+                    label = labels[j]
+                    class_correct[label] += comp[j].item()
+                    class_total[label] += 1 
+        print("\n\nPRESENTING OVERALL CLASSIFICATION ACCURACY STATS:\n\n")
+        for j in range(len(class_labels)):
+            print('Prediction accuracy for %5s : %2d %%' % (class_labels[j], 100 * class_correct[j] / class_total[j]))
+            FILE.write('\n\nPrediction accuracy for %5s : %2d %%\n' % (class_labels[j], 100 * class_correct[j] / class_total[j]))
+        print("\n\n\nOverall accuracy of the network on the test images: %d %%" % (100 * correct / float(total)))
+        FILE.write("\n\n\nOverall accuracy of the network on the test images: %d %%\n" % (100 * correct / float(total)))
+        print("\n\nDisplaying the confusion matrix:\n")
+        FILE.write("\n\nDisplaying the confusion matrix:\n\n")
+        out_str = "         "
+        for j in range(len(class_labels)):  out_str +=  "%7s" % class_labels[j]   
+        print(out_str + "\n")
+        FILE.write(out_str + "\n\n")
+        for i,label in enumerate(class_labels):
+            out_percents = [100 * confusion_matrix[i,j] / float(class_total[i]) for j in range(len(class_labels))]
+            out_percents = ["%.2f" % item.item() for item in out_percents]
+            out_str = "%6s:  " % class_labels[i]
+            for j in range(len(class_labels)): out_str +=  "%7s" % out_percents[j]
+            print(out_str)
+            FILE.write(out_str + "\n")
+        FILE.close()        
+
+
+    def run_code_for_evaluating_checkpoint(self, encoder_network, checkpoints_dir):
+        """
+        Training transformer networks has always been difficulty and that's the case even with 
+        learning-rate warm-up and other mitigating strategies.  DLStudio provides you with 
+        checkpoints for making transformer training a little bit less frustrated.  While you are 
+        training a transformer, a checkpoint for the model is created every 5 epochs. The checkpoint
+        consists of two models, one for the encoder and the other for the decoder.  For example, after
+        5 epochs of training, the consists of the following models:
+
+                   visTrans_4
+
+        where '4' is index of the epoch at the end of which the checkpoint was created.  The
+        directory in which the checkpoint is deposited in one of the arguments when this function
+        is invoked in your script.
+
+        Subsequently, to see if any learning at all is going on, you can invoke this function and it 
+        will print out the English-to-Spanish translation for a set of randomly selected sentences 
+        from the corpus.  Let's say you want to test whether the checkpoint after 5 epochs of training
+        is any good, you could execute the script "test_checkpointFG.py" in the ExamplesTransformers
+        directory and that script will call this function.  The call syntax for the script is
+
+                python3  test_checkpoint_for_visTransformer.py  checkpoints_visTrans  4
+
+        where checkpoints_visTrans is the name of the local directory for the checkpoints
+        and where the argument 4 says that you want to use the models stored away at the end
+        of the epoch indexed 4.  In particular the above script will reload the following two
+        checkpoints:
+
+                checkpoint_0_for_epoch_4  
+        and
+                checkpoint_1_for_epoch_4
+
+        where the first is for the network model and the second for the patch embedding generator.
+        """
+        if len( sys.argv ) != 3:
+            sys.exit("\n\nYou perhaps forgot to specify which checkpoint you want to use.\n\n")
+        else:
+            checkpoint_index = int(sys.argv[2])
+        print("\n\nSHOWING RESULTS FOR THE CHECKPOINT AT EPOCH: %d\n\n" % checkpoint_index)
+        class_labels = self.dl_studio.class_labels
+        filename_for_results = "classification_results_checkpoint_" + str(checkpoint_index) + ".txt"
+        FILE = open(filename_for_results, 'w')
+        correct = 0
+        total = 0
+        confusion_matrix = torch.zeros(len(class_labels), len(class_labels))
+        class_correct = [0] * len(class_labels)
+        class_total = [0] * len(class_labels)
+        patch_embedding_generator = self.PatchEmbeddingGenerator( self )
+        patch_embedding_generator.load_state_dict(torch.load(checkpoints_dir + "/checkpoint_1_for_epoch_" + str(checkpoint_index) ))
+        patch_embedding_generator.to(self.dl_studio.device)
+        encoder_network.load_state_dict(torch.load(checkpoints_dir + "/checkpoint_0_for_epoch_" + str(checkpoint_index) ))
+        encoder_network.to(self.dl_studio.device)
+        debug = False
+        with torch.no_grad():
+            for i, data in enumerate(self.test_data_loader):                                    
+                if i > 999: break
+                if debug:
+                    print("\n\n\n=========Showing results for test image %d===============" % i)
+                test_images, labels = data     
+                if test_images.shape[0] != self.batch_size: break
+                if debug:
+                    logger.setLevel(100)
+                    plt.figure(figsize=[6,3])
+                    plt.imshow(np.transpose(torchvision.utils.make_grid(input_images, normalize=False, padding=3, pad_value=255).cpu(), (1,2,0)))
+                    plt.show()
+                    logger.setLevel(old_level)
+                test_images.to(self.dl_studio.device)
+                labels.to(self.dl_studio.device)
+                patch_sequences = test_images.unfold(2, self.patch_size[0], self.patch_size[1]).unfold(3, self.patch_size[0], self.patch_size[1]) 
+                patch_sequence_embeddings = patch_embedding_generator( patch_sequences )
+                encoder_output = encoder_network( patch_sequence_embeddings )
+                _, predicted = torch.max(encoder_output.data, 1)
+                predicted = predicted.tolist()
+                if debug:
+                    print("\npredicted_class_labels: ")
+                    print(predicted)             
+                symbolic_name_prediction = [class_labels[index] for index in predicted]
+                symbolic_name_gt = [class_labels[index] for index in labels]
+                if debug:
+                    print("\nimage labels ground truth: ", symbolic_name_gt)
+                    print("\npredicted_test_image_class_label: ", symbolic_name_prediction)
+                for label,prediction in zip(labels, predicted):
+                    confusion_matrix[label][prediction] += 1
+                total += labels.shape[0]
+                labels = labels.tolist()
+                comp =  torch.LongTensor(predicted) == torch.LongTensor(labels)
+                correct += comp.sum().item()
+                for j in range(self.batch_size):
+                    label = labels[j]
+                    class_correct[label] += comp[j].item()
+                    class_total[label] += 1 
+        print("\n\nPRESENTING OVERALL CLASSIFICATION ACCURACY STATS:\n\n")
+        for j in range(len(class_labels)):
+            print('Prediction accuracy for %5s : %2d %%' % (class_labels[j], 100 * class_correct[j] / class_total[j]))
+            FILE.write('\n\nPrediction accuracy for %5s : %2d %%\n' % (class_labels[j], 100 * class_correct[j] / class_total[j]))
+        print("\n\n\nOverall accuracy of the network on the test images: %d %%" % (100 * correct / float(total)))
+        FILE.write("\n\n\nOverall accuracy of the network on the test images: %d %%\n" % (100 * correct / float(total)))
+        print("\n\nDisplaying the confusion matrix:\n")
+        FILE.write("\n\nDisplaying the confusion matrix:\n\n")
+        out_str = "         "
+        for j in range(len(class_labels)):  out_str +=  "%7s" % class_labels[j]   
+        print(out_str + "\n")
+        FILE.write(out_str + "\n\n")
+        for i,label in enumerate(class_labels):
+            out_percents = [100 * confusion_matrix[i,j] / float(class_total[i]) for j in range(len(class_labels))]
+            out_percents = ["%.2f" % item.item() for item in out_percents]
+            out_str = "%6s:  " % class_labels[i]
+            for j in range(len(class_labels)): out_str +=  "%7s" % out_percents[j]
+            print(out_str)
+            FILE.write(out_str + "\n")
+        FILE.close()        
+
+
+##################################  END Definition of Class visTransformer  END  ####################################
+#####################################################################################################################
+#####################################################################################################################
+
+
+
+
 #_______________________  End of Transformers Class Definition __________________________
 
 #______________________________    Test code follows    _________________________________
 
 if __name__ == '__main__': 
     pass
```

### Comparing `DLStudio-2.4.3/setup.py` & `DLStudio-2.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 
 ### setup.py
 
 from setuptools import setup, find_packages
 import sys, os
 
 setup(name='DLStudio',
-      version='2.4.3',
+      version='2.4.8',
       author='Avinash Kak',
       author_email='kak@purdue.edu',
       maintainer='Avinash Kak',
       maintainer_email='kak@purdue.edu',
-      url='https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html',
-      download_url='https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.tar.gz',
+      url='https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html',
+      download_url='https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.tar.gz',
       description='A PyTorch based software platform for teaching the Deep Learning class at Purdue University',
       long_description='''
 
 Consult the module API page at
 
-      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.3.html
+      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html
 
 for all information related to this module, including the information about
 the latest changes to the code.  
 
 ::
 
       convo_layers_config = "1x[128,3,3,1]-MaxPool(2) 1x[16,5,5,1]-MaxPool(2)"
```

