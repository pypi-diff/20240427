# Comparing `tmp/datadreamer-0.1.4.tar.gz` & `tmp/datadreamer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadreamer-0.1.4.tar", last modified: Mon Apr  8 20:01:26 2024, max compression
+gzip compressed data, was "datadreamer-0.1.5.tar", last modified: Sat Apr 27 17:50:50 2024, max compression
```

## Comparing `datadreamer-0.1.4.tar` & `datadreamer-0.1.5.tar`

### file list

```diff
@@ -1,61 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-08 20:01:21.000000 datadreamer-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28298 2024-04-08 20:01:26.160206 datadreamer-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-08 20:01:21.000000 datadreamer-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.152206 datadreamer-0.1.4/datadreamer/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.156206 datadreamer-0.1.4/datadreamer/dataset_annotation/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/dataset_annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/dataset_annotation/clip_annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/dataset_annotation/image_annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/dataset_annotation/owlv2_annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/dataset_annotation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.156206 datadreamer-0.1.4/datadreamer/image_generation/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/clip_image_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/sdxl_image_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/sdxl_lightning_image_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/sdxl_turbo_image_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.156206 datadreamer-0.1.4/datadreamer/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/pipelines/generate_dataset_from_scratch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.156206 datadreamer-0.1.4/datadreamer/prompt_generation/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/lm_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/lm_synonym_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/simple_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/synonym_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/tinyllama_lm_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/wordnet_synonym_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.156206 datadreamer-0.1.4/datadreamer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/utils/convert_dataset_to_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/utils/nms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/datadreamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28298 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-08 20:01:21.000000 datadreamer-0.1.4/examples/image_annotation_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-08 20:01:21.000000 datadreamer-0.1.4/examples/image_generation_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-08 20:01:21.000000 datadreamer-0.1.4/examples/measure_batched_prompt_gen_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 20:01:21.000000 datadreamer-0.1.4/examples/prompt_generation_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-08 20:01:21.000000 datadreamer-0.1.4/examples/visualize_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-08 20:01:21.000000 datadreamer-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-08 20:01:21.000000 datadreamer-0.1.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-08 20:01:21.000000 datadreamer-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:01:26.160206 datadreamer-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.152206 datadreamer-0.1.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)    33852 2024-04-08 20:01:21.000000 datadreamer-0.1.4/tests/integration/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/tests/unittests/
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-08 20:01:21.000000 datadreamer-0.1.4/tests/unittests/test_annotators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-08 20:01:21.000000 datadreamer-0.1.4/tests/unittests/test_image_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-08 20:01:21.000000 datadreamer-0.1.4/tests/unittests/test_prompt_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-08 20:01:21.000000 datadreamer-0.1.4/tools/autogenerate_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.788124 datadreamer-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-27 17:50:46.000000 datadreamer-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    29093 2024-04-27 17:50:50.788124 datadreamer-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-04-27 17:50:46.000000 datadreamer-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.780125 datadreamer-0.1.5/datadreamer/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.780125 datadreamer-0.1.5/datadreamer/dataset_annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/dataset_annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/dataset_annotation/clip_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/dataset_annotation/image_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/dataset_annotation/owlv2_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/dataset_annotation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.784124 datadreamer-0.1.5/datadreamer/image_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/image_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/image_generation/clip_image_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/image_generation/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/image_generation/sdxl_image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/image_generation/sdxl_lightning_image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/image_generation/sdxl_turbo_image_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.784124 datadreamer-0.1.5/datadreamer/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18816 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/pipelines/generate_dataset_from_scratch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.784124 datadreamer-0.1.5/datadreamer/prompt_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/prompt_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/prompt_generation/lm_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/prompt_generation/lm_synonym_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/prompt_generation/prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/prompt_generation/simple_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/prompt_generation/synonym_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/prompt_generation/tinyllama_lm_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/prompt_generation/wordnet_synonym_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.788124 datadreamer-0.1.5/datadreamer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/utils/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/utils/coco_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/utils/convert_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/utils/luxonis_dataset_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/utils/merge_raw_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/utils/nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/utils/single_label_cls_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-04-27 17:50:46.000000 datadreamer-0.1.5/datadreamer/utils/yolo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.788124 datadreamer-0.1.5/datadreamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29093 2024-04-27 17:50:50.000000 datadreamer-0.1.5/datadreamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-27 17:50:50.000000 datadreamer-0.1.5/datadreamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:50:50.000000 datadreamer-0.1.5/datadreamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-27 17:50:50.000000 datadreamer-0.1.5/datadreamer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-27 17:50:50.000000 datadreamer-0.1.5/datadreamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-27 17:50:50.000000 datadreamer-0.1.5/datadreamer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.788124 datadreamer-0.1.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-27 17:50:46.000000 datadreamer-0.1.5/examples/image_annotation_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-27 17:50:46.000000 datadreamer-0.1.5/examples/image_generation_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-27 17:50:46.000000 datadreamer-0.1.5/examples/measure_batched_prompt_gen_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-27 17:50:46.000000 datadreamer-0.1.5/examples/prompt_generation_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-27 17:50:46.000000 datadreamer-0.1.5/examples/visualize_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-27 17:50:46.000000 datadreamer-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-27 17:50:46.000000 datadreamer-0.1.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-27 17:50:46.000000 datadreamer-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 17:50:50.788124 datadreamer-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.776124 datadreamer-0.1.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.788124 datadreamer-0.1.5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)    36877 2024-04-27 17:50:46.000000 datadreamer-0.1.5/tests/integration/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.788124 datadreamer-0.1.5/tests/unittests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-27 17:50:46.000000 datadreamer-0.1.5/tests/unittests/test_annotators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-27 17:50:46.000000 datadreamer-0.1.5/tests/unittests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-27 17:50:46.000000 datadreamer-0.1.5/tests/unittests/test_image_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-27 17:50:46.000000 datadreamer-0.1.5/tests/unittests/test_prompt_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:50.788124 datadreamer-0.1.5/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-27 17:50:46.000000 datadreamer-0.1.5/tools/autogenerate_requirements.py
```

### Comparing `datadreamer-0.1.4/LICENSE` & `datadreamer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/PKG-INFO` & `datadreamer-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadreamer
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for dataset generation and knowledge extraction from foundation computer vision models.
 Maintainer-email: Luxonis <support@luxonis.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -228,14 +228,16 @@
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: matplotlib>=3.6.0
 Requires-Dist: opencv-python>=4.7.0
 Requires-Dist: accelerate>=0.25.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: bitsandbytes>=0.42.0
 Requires-Dist: nltk>=3.8.1
+Requires-Dist: luxonis-ml[all]>=0.1.0
+Requires-Dist: python-box>=7.1.1
 Provides-Extra: dev
 Requires-Dist: pre-commit>=3.2.1; extra == "dev"
 Requires-Dist: toml>=0.10.2; extra == "dev"
 
 # DataDreamer
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
@@ -372,48 +374,57 @@
 
 Run the following command in your terminal to use the script:
 
 ```bash
 datadreamer --save_dir <directory> --class_names <objects> --prompts_number <number> [additional options]
 ```
 
+or using a `.yaml` config file
+
+```bash
+datadreamer --config <path-to-config>
+```
+
 <a name="main-parameters"></a>
 
 ### 🎯 Main Parameters
 
 - `--save_dir` (required): Path to the directory for saving generated images and annotations.
 - `--class_names` (required): Space-separated list of object names for image generation and annotation. Example: `person moon robot`.
 - `--prompts_number` (optional): Number of prompts to generate for each object. Defaults to `10`.
 - `--annotate_only` (optional): Only annotate the images without generating new ones, prompt and image generator will be skipped. Defaults to `False`.
 
 <a name="additional-parameters"></a>
 
 ### 🔧 Additional Parameters
 
 - `--task`: Choose between detection and classification. Default is `detection`.
+- `--dataset_format`: Format of the dataset. Defaults to `raw`. Supported values: `raw`, `yolo`, `coco`, `luxonis-dataset`, `cls-single`.
+- `--split_ratios`: Split ratios for train, validation, and test sets. Defaults to `[0.8, 0.1, 0.1]`.
 - `--num_objects_range`: Range of objects in a prompt. Default is 1 to 3.
 - `--prompt_generator`: Choose between `simple`, `lm` (language model) and `tiny` (tiny LM). Default is `simple`.
 - `--image_generator`: Choose image generator, e.g., `sdxl`, `sdxl-turbo` or `sdxl-lightning`. Default is `sdxl-turbo`.
 - `--image_annotator`: Specify the image annotator, like `owlv2` for object detection or `clip` for image classification. Default is `owlv2`.
 - `--conf_threshold`: Confidence threshold for annotation. Default is `0.15`.
 - `--annotation_iou_threshold`: Intersection over Union (IoU) threshold for annotation. Default is `0.2`.
 - `--prompt_prefix`: Prefix to add to every image generation prompt. Default is `""`.
 - `--prompt_suffix`: Suffix to add to every image generation prompt, e.g., for adding details like resolution. Default is `", hd, 8k, highly detailed"`.
 - `--negative_prompt`: Negative prompts to guide the generation away from certain features. Default is `"cartoon, blue skin, painting, scrispture, golden, illustration, worst quality, low quality, normal quality:2, unrealistic dream, low resolution,  static, sd character, low quality, low resolution, greyscale, monochrome, nose, cropped, lowres, jpeg artifacts, deformed iris, deformed pupils, bad eyes, semi-realistic worst quality, bad lips, deformed mouth, deformed face, deformed fingers, bad anatomy"`.
-- `--use_tta`: Toggle test time augmentation for object detection. Default is `True`.
+- `--use_tta`: Toggle test time augmentation for object detection. Default is `False`.
 - `--synonym_generator`: Enhance class names with synonyms. Default is `none`. Other options are `llm`, `wordnet`.
 - `--use_image_tester`: Use image tester for image generation. Default is `False`.
 - `--image_tester_patience`: Patience level for image tester. Default is `1`.
 - `--lm_quantization`: Quantization to use for Mistral language model. Choose between `none` and `4bit`. Default is `none`.
 - `--annotator_size`: Size of the annotator model to use. Choose between `base` and `large`. Default is `base`.
 - `--batch_size_prompt`: Batch size for prompt generation. Default is 64.
-- `--batch_size_annotation`: Batch size for annotation. Default is `8`.
+- `--batch_size_annotation`: Batch size for annotation. Default is `1`.
 - `--batch_size_image`: Batch size for image generation. Default is `1`.
 - `--device`: Choose between `cuda` and `cpu`. Default is `cuda`.
 - `--seed`: Set a random seed for image and prompt generation. Default is `42`.
+- `--config`: A path to an optional `.yaml` config file specifying the pipeline's arguments.
 
 <a name="available-models"></a>
 
 ### 🤖 Available Models
 
 | Model Category    | Model Names                                                                           | Description/Notes                       |
 | ----------------- | ------------------------------------------------------------------------------------- | --------------------------------------- |
@@ -430,16 +441,24 @@
 
 ### 💡 Example
 
 ```bash
 datadreamer --save_dir path/to/save_directory --class_names person moon robot --prompts_number 20 --prompt_generator simple --num_objects_range 1 3 --image_generator sdxl-turbo
 ```
 
+or using a `.yaml` config file (if arguments are provided with the config file in the command, they will override the ones in the config file):
+
+```bash
+datadreamer --save_dir path/to/save_directory --config configs/det_config.yaml
+```
+
 This command generates images for the specified objects, saving them and their annotations in the given directory. The script allows customization of the generation process through various parameters, adapting to different needs and hardware configurations.
 
+See `/configs` folder for some examples of the `.yaml` config files.
+
 <a name="output"></a>
 
 ### 📦 Output
 
 The dataset comprises two primary components: images and their corresponding annotations, stored as JSON files.
 
 ```bash
```

### Comparing `datadreamer-0.1.4/README.md` & `datadreamer-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -134,48 +134,57 @@
 
 Run the following command in your terminal to use the script:
 
 ```bash
 datadreamer --save_dir <directory> --class_names <objects> --prompts_number <number> [additional options]
 ```
 
+or using a `.yaml` config file
+
+```bash
+datadreamer --config <path-to-config>
+```
+
 <a name="main-parameters"></a>
 
 ### 🎯 Main Parameters
 
 - `--save_dir` (required): Path to the directory for saving generated images and annotations.
 - `--class_names` (required): Space-separated list of object names for image generation and annotation. Example: `person moon robot`.
 - `--prompts_number` (optional): Number of prompts to generate for each object. Defaults to `10`.
 - `--annotate_only` (optional): Only annotate the images without generating new ones, prompt and image generator will be skipped. Defaults to `False`.
 
 <a name="additional-parameters"></a>
 
 ### 🔧 Additional Parameters
 
 - `--task`: Choose between detection and classification. Default is `detection`.
+- `--dataset_format`: Format of the dataset. Defaults to `raw`. Supported values: `raw`, `yolo`, `coco`, `luxonis-dataset`, `cls-single`.
+- `--split_ratios`: Split ratios for train, validation, and test sets. Defaults to `[0.8, 0.1, 0.1]`.
 - `--num_objects_range`: Range of objects in a prompt. Default is 1 to 3.
 - `--prompt_generator`: Choose between `simple`, `lm` (language model) and `tiny` (tiny LM). Default is `simple`.
 - `--image_generator`: Choose image generator, e.g., `sdxl`, `sdxl-turbo` or `sdxl-lightning`. Default is `sdxl-turbo`.
 - `--image_annotator`: Specify the image annotator, like `owlv2` for object detection or `clip` for image classification. Default is `owlv2`.
 - `--conf_threshold`: Confidence threshold for annotation. Default is `0.15`.
 - `--annotation_iou_threshold`: Intersection over Union (IoU) threshold for annotation. Default is `0.2`.
 - `--prompt_prefix`: Prefix to add to every image generation prompt. Default is `""`.
 - `--prompt_suffix`: Suffix to add to every image generation prompt, e.g., for adding details like resolution. Default is `", hd, 8k, highly detailed"`.
 - `--negative_prompt`: Negative prompts to guide the generation away from certain features. Default is `"cartoon, blue skin, painting, scrispture, golden, illustration, worst quality, low quality, normal quality:2, unrealistic dream, low resolution,  static, sd character, low quality, low resolution, greyscale, monochrome, nose, cropped, lowres, jpeg artifacts, deformed iris, deformed pupils, bad eyes, semi-realistic worst quality, bad lips, deformed mouth, deformed face, deformed fingers, bad anatomy"`.
-- `--use_tta`: Toggle test time augmentation for object detection. Default is `True`.
+- `--use_tta`: Toggle test time augmentation for object detection. Default is `False`.
 - `--synonym_generator`: Enhance class names with synonyms. Default is `none`. Other options are `llm`, `wordnet`.
 - `--use_image_tester`: Use image tester for image generation. Default is `False`.
 - `--image_tester_patience`: Patience level for image tester. Default is `1`.
 - `--lm_quantization`: Quantization to use for Mistral language model. Choose between `none` and `4bit`. Default is `none`.
 - `--annotator_size`: Size of the annotator model to use. Choose between `base` and `large`. Default is `base`.
 - `--batch_size_prompt`: Batch size for prompt generation. Default is 64.
-- `--batch_size_annotation`: Batch size for annotation. Default is `8`.
+- `--batch_size_annotation`: Batch size for annotation. Default is `1`.
 - `--batch_size_image`: Batch size for image generation. Default is `1`.
 - `--device`: Choose between `cuda` and `cpu`. Default is `cuda`.
 - `--seed`: Set a random seed for image and prompt generation. Default is `42`.
+- `--config`: A path to an optional `.yaml` config file specifying the pipeline's arguments.
 
 <a name="available-models"></a>
 
 ### 🤖 Available Models
 
 | Model Category    | Model Names                                                                           | Description/Notes                       |
 | ----------------- | ------------------------------------------------------------------------------------- | --------------------------------------- |
@@ -192,16 +201,24 @@
 
 ### 💡 Example
 
 ```bash
 datadreamer --save_dir path/to/save_directory --class_names person moon robot --prompts_number 20 --prompt_generator simple --num_objects_range 1 3 --image_generator sdxl-turbo
 ```
 
+or using a `.yaml` config file (if arguments are provided with the config file in the command, they will override the ones in the config file):
+
+```bash
+datadreamer --save_dir path/to/save_directory --config configs/det_config.yaml
+```
+
 This command generates images for the specified objects, saving them and their annotations in the given directory. The script allows customization of the generation process through various parameters, adapting to different needs and hardware configurations.
 
+See `/configs` folder for some examples of the `.yaml` config files.
+
 <a name="output"></a>
 
 ### 📦 Output
 
 The dataset comprises two primary components: images and their corresponding annotations, stored as JSON files.
 
 ```bash
```

### Comparing `datadreamer-0.1.4/datadreamer/dataset_annotation/clip_annotator.py` & `datadreamer-0.1.5/datadreamer/dataset_annotation/clip_annotator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/dataset_annotation/image_annotator.py` & `datadreamer-0.1.5/datadreamer/dataset_annotation/image_annotator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/dataset_annotation/owlv2_annotator.py` & `datadreamer-0.1.5/datadreamer/dataset_annotation/owlv2_annotator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/dataset_annotation/utils.py` & `datadreamer-0.1.5/datadreamer/dataset_annotation/utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/image_generation/clip_image_tester.py` & `datadreamer-0.1.5/datadreamer/image_generation/clip_image_tester.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/image_generation/image_generator.py` & `datadreamer-0.1.5/datadreamer/image_generation/image_generator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/image_generation/sdxl_image_generator.py` & `datadreamer-0.1.5/datadreamer/image_generation/sdxl_image_generator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/image_generation/sdxl_lightning_image_generator.py` & `datadreamer-0.1.5/datadreamer/image_generation/sdxl_lightning_image_generator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/image_generation/sdxl_turbo_image_generator.py` & `datadreamer-0.1.5/datadreamer/image_generation/sdxl_turbo_image_generator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/pipelines/generate_dataset_from_scratch.py` & `datadreamer-0.1.5/datadreamer/pipelines/generate_dataset_from_scratch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import argparse
-import json
 import os
+import shutil
+import uuid
 
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
+from box import Box
 from PIL import Image
 from tqdm import tqdm
 
 from datadreamer.dataset_annotation import CLIPAnnotator, OWLv2Annotator
 from datadreamer.image_generation import (
     StableDiffusionImageGenerator,
     StableDiffusionLightningImageGenerator,
@@ -20,14 +22,16 @@
 from datadreamer.prompt_generation import (
     LMPromptGenerator,
     LMSynonymGenerator,
     SimplePromptGenerator,
     TinyLlamaLMPromptGenerator,
     WordNetSynonymGenerator,
 )
+from datadreamer.utils import Config, convert_dataset
+from datadreamer.utils.dataset_utils import save_annotations_to_json
 
 prompt_generators = {
     "simple": SimplePromptGenerator,
     "lm": LMPromptGenerator,
     "tiny": TinyLlamaLMPromptGenerator,
 }
 
@@ -48,185 +52,189 @@
 
 def parse_args():
     # Argument parsing
     parser = argparse.ArgumentParser(description="Generate and annotate images.")
     parser.add_argument(
         "--save_dir",
         type=str,
-        default="generated_dataset",
         help="Directory to save generated images and annotations",
     )
 
     parser.add_argument(
         "--task",
         type=str,
-        default="detection",
         choices=["detection", "classification"],
         help="Task to generate data for",
     )
 
     parser.add_argument(
         "--class_names",
         type=str,
         nargs="+",
-        default=["bear", "bicycle", "bird", "person"],
         help="List of object names for prompt generation",
     )
 
     parser.add_argument(
         "--annotate_only",
         action="store_true",
+        default=None,
         help="Only annotate the images without generating new ones, prompt and image generator will be skipped.",
     )
 
     parser.add_argument(
-        "--prompts_number", type=int, default=10, help="Number of prompts to generate"
+        "--prompts_number",
+        type=int,
+        help="Number of prompts to generate",
     )
 
     parser.add_argument(
         "--num_objects_range",
         type=int,
         nargs="+",
-        default=[1, 3],
         help="Range of number of objects in a prompt",
     )
 
     parser.add_argument(
         "--prompt_generator",
         type=str,
-        default="simple",
         choices=["simple", "lm", "tiny"],
         help="Prompt generator to use: simple or language model",
     )
     parser.add_argument(
         "--image_generator",
         type=str,
-        default="sdxl-turbo",
         choices=["sdxl", "sdxl-turbo", "sdxl-lightning"],
         help="Image generator to use",
     )
     parser.add_argument(
         "--image_annotator",
         type=str,
-        default="owlv2",
         choices=["owlv2", "clip"],
         help="Image annotator to use",
     )
 
     parser.add_argument(
+        "--dataset_format",
+        type=str,
+        choices=["raw", "yolo", "coco", "luxonis-dataset", "cls-single"],
+        help="Dataset format to use",
+    )
+    parser.add_argument(
+        "--split_ratios",
+        type=float,
+        nargs="+",
+        help="Train-validation-test split ratios (default: 0.8, 0.1, 0.1).",
+    )
+
+    parser.add_argument(
         "--synonym_generator",
         type=str,
-        default="none",
         choices=["none", "llm", "wordnet"],
         help="Image annotator to use",
     )
 
     parser.add_argument(
         "--negative_prompt",
         type=str,
-        default="cartoon, blue skin, painting, scrispture, golden, illustration, worst quality, low quality, normal quality:2, unrealistic dream, low resolution,  static, sd character, low quality, low resolution, greyscale, monochrome, nose, cropped, lowres, jpeg artifacts, deformed iris, deformed pupils, bad eyes, semi-realistic worst quality, bad lips, deformed mouth, deformed face, deformed fingers, bad anatomy",
         help="Negative prompt to guide the generation away from certain features",
     )
 
     parser.add_argument(
         "--prompt_suffix",
         type=str,
-        default=", hd, 8k, highly detailed",
         help="Suffix to add to every image generation prompt, e.g., for adding details like resolution",
     )
 
     parser.add_argument(
         "--prompt_prefix",
         type=str,
-        default="",
         help="Prefix to add to every image generation prompt",
     )
 
     parser.add_argument(
         "--conf_threshold",
         type=float,
-        default=0.15,
         help="Confidence threshold for annotation",
     )
 
     parser.add_argument(
         "--annotation_iou_threshold",
         type=float,
-        default=0.2,
         help="Intersection over Union (IoU) threshold for annotation",
     )
 
     parser.add_argument(
         "--use_tta",
-        default=False,
+        default=None,
         action="store_true",
         help="Whether to use test time augmentation for object detection",
     )
 
     parser.add_argument(
         "--use_image_tester",
-        default=False,
+        default=None,
         action="store_true",
         help="Whether to use image tester for image generation",
     )
 
     parser.add_argument(
         "--image_tester_patience",
         type=int,
-        default=1,
         help="Patience for image tester",
     )
 
     parser.add_argument(
         "--lm_quantization",
         type=str,
-        default="none",
         choices=["none", "4bit"],
         help="Quantization to use for Mistral language model",
     )
 
     parser.add_argument(
         "--annotator_size",
         type=str,
-        default="base",
         choices=["base", "large"],
         help="Size of the annotator model to use",
     )
 
     parser.add_argument(
         "--batch_size_prompt",
         type=int,
-        default=64,
         help="Batch size for prompt generation",
     )
 
     parser.add_argument(
         "--batch_size_annotation",
         type=int,
-        default=1,
         help="Batch size for annotation",
     )
 
     parser.add_argument(
         "--batch_size_image",
         type=int,
-        default=1,
         help="Batch size for image generation",
     )
 
     parser.add_argument(
         "--device",
         type=str,
-        default="cuda",
         choices=["cuda", "cpu"],
         help="Device to use",
     )
 
     parser.add_argument(
-        "--seed", type=int, default=42, help="Random seed for image generation"
+        "--config",
+        type=str,
+        help="Path to the configuration file",
+    )
+
+    parser.add_argument(
+        "--seed",
+        type=int,
+        help="Random seed for image generation",
     )
 
     return parser.parse_args()
 
 
 def check_args(args):
     # Check save_dir
@@ -238,17 +246,14 @@
 
     # Check class_names
     if not args.class_names or any(
         not isinstance(name, str) for name in args.class_names
     ):
         raise ValueError("--class_names must be a non-empty list of strings")
 
-    if args.annotate_only and not args.task == "detection":
-        raise ValueError("--annotate_only can only be used with --task=detection")
-
     # Check prompts_number
     if args.prompts_number <= 0:
         raise ValueError("--prompts_number must be a positive integer")
 
     # Check num_objects_range
     if (
         len(args.num_objects_range) != 2
@@ -315,69 +320,59 @@
         )
 
     if args.task == "classification" and args.image_annotator not in clf_annotators:
         raise ValueError(
             "--image_annotator must be one of the available annotators for classification task"
         )
 
+    # Check coorect task and dataset_format
+    if args.task == "classification" and args.dataset_format in ["coco", "yolo"]:
+        raise ValueError(
+            "--dataset_format must be one of the available dataset formats for classification task: raw, cls-single, luxonis-dataset"
+        )
+
+    if args.task == "detection" and args.dataset_format in ["cls-single"]:
+        raise ValueError(
+            "--dataset_format must be one of the available dataset formats for detection task: raw, coco, yolo, luxonis-dataset"
+        )
 
-def save_det_annotations_to_json(
-    image_paths,
-    boxes_list,
-    labels_list,
-    class_names,
-    save_dir,
-    file_name="annotations.json",
-):
-    annotations = {}
-    for image_path, bboxes, labels in zip(image_paths, boxes_list, labels_list):
-        image_name = os.path.basename(image_path)
-        annotations[image_name] = {
-            "boxes": bboxes.tolist(),
-            "labels": labels.tolist(),
-        }
-    annotations["class_names"] = class_names
-
-    # Save to JSON file
-    with open(os.path.join(save_dir, file_name), "w") as f:
-        json.dump(annotations, f, indent=4)
-
-
-def save_clf_annotations_to_json(
-    image_paths, labels_list, class_names, save_dir, file_name="annotations.json"
-):
-    annotations = {}
-    for image_path, labels in zip(image_paths, labels_list):
-        image_name = os.path.basename(image_path)
-        annotations[image_name] = {
-            "labels": labels.tolist(),
-        }
-    annotations["class_names"] = class_names
-
-    # Save to JSON file
-    with open(os.path.join(save_dir, file_name), "w") as f:
-        json.dump(annotations, f, indent=4)
+    # Check split_ratios
+    if (
+        len(args.split_ratios) != 3
+        or not all(0 <= ratio <= 1 for ratio in args.split_ratios)
+        or sum(args.split_ratios) != 1
+    ):
+        raise ValueError(
+            "--split_ratios must be a list of three floats that sum up to 1"
+        )
 
 
 def main():
     args = parse_args()
+    # Get the None args without the config
+    args_dict = {k: v for k, v in vars(args).items() if k != "config" and v is not None}
+    config = Config.get_config(args.config, args_dict)
+    args = Box(config.model_dump(exclude_none=True, by_alias=True))
+    # Check arguments
     check_args(args)
 
+    # Directories for saving images and bboxes
     save_dir = args.save_dir
+    if not args.annotate_only:
+        if os.path.exists(save_dir):
+            shutil.rmtree(save_dir)
+        os.makedirs(save_dir)
 
-    # Directories for saving images and bboxes
     bbox_dir = os.path.join(save_dir, "bboxes_visualization")
-    if not os.path.exists(save_dir):
-        os.makedirs(save_dir)
-    if not os.path.exists(bbox_dir):
-        os.makedirs(bbox_dir)
+    if os.path.exists(bbox_dir):
+        shutil.rmtree(bbox_dir)
+    os.makedirs(bbox_dir)
 
     # Save arguments
-    with open(os.path.join(save_dir, "generation_args.json"), "w") as f:
-        json.dump(vars(args), f, indent=4)
+    config.save_data(os.path.join(save_dir, "generation_args.yaml"))
 
     generated_prompts = None
     image_paths = []
 
     if not args.annotate_only:
         # Prompt generation
         prompt_generator_class = prompt_generators[args.prompt_generator]
@@ -413,15 +408,17 @@
         prompt_objects = [p[0] for p in generated_prompts]
 
         num_generated_images = 0
         for generated_images_batch in image_generator.generate_images(
             prompts, prompt_objects
         ):
             for generated_image in generated_images_batch:
-                image_path = os.path.join(save_dir, f"image_{num_generated_images}.jpg")
+                unique_id = uuid.uuid4().hex
+                unique_filename = f"image_{num_generated_images}_{unique_id}.jpg"
+                image_path = os.path.join(save_dir, unique_filename)
                 generated_image.save(image_path)
                 image_paths.append(image_path)
                 num_generated_images += 1
 
         image_generator.release(empty_cuda_cache=True)
 
     else:
@@ -438,20 +435,23 @@
         synonym_generator = synonym_generator_class(device=args.device)
         synonym_dict = synonym_generator.generate_synonyms_for_list(args.class_names)
         synonym_generator.release(empty_cuda_cache=True)
         synonym_generator.save_synonyms(
             synonym_dict, os.path.join(save_dir, "synonyms.json")
         )
 
+    boxes_list = []
+    scores_list = []
+    labels_list = []
+
     if args.task == "classification":
         # Classification annotation
         annotator_class = clf_annotators[args.image_annotator]
         annotator = annotator_class(device=args.device, size=args.annotator_size)
 
-        labels_list = []
         # Split image_paths into batches
         image_batches = [
             image_paths[i : i + args.batch_size_annotation]
             for i in range(0, len(image_paths), args.batch_size_annotation)
         ]
 
         for image_batch in tqdm(
@@ -464,32 +464,40 @@
                 images,
                 args.class_names,
                 conf_threshold=args.conf_threshold,
                 synonym_dict=synonym_dict,
             )
             labels_list.extend(batch_labels)
 
-        save_clf_annotations_to_json(
-            image_paths, labels_list, args.class_names, save_dir
+        save_annotations_to_json(
+            image_paths=image_paths,
+            labels_list=labels_list,
+            class_names=args.class_names,
+            save_dir=save_dir,
         )
+
+        if args.dataset_format == "cls-single":
+            convert_dataset.convert_dataset(
+                args.save_dir,
+                args.save_dir,
+                "cls-single",
+                args.split_ratios,
+                copy_files=False,
+                seed=args.seed,
+            )
     else:
         # Annotation
         annotator_class = det_annotators[args.image_annotator]
         annotator = annotator_class(device=args.device, size=args.annotator_size)
 
-        boxes_list = []
-        scores_list = []
-        labels_list = []
-
         # Split image_paths into batches
         image_batches = [
             image_paths[i : i + args.batch_size_annotation]
             for i in range(0, len(image_paths), args.batch_size_annotation)
         ]
-
         for i, image_batch in tqdm(
             enumerate(image_batches),
             desc="Annotating images",
             total=len(image_batches),
         ):
             images = [Image.open(image_path) for image_path in image_batch]
             boxes_batch, scores_batch, local_labels_batch = annotator.annotate_batch(
@@ -542,14 +550,50 @@
                     os.path.join(
                         bbox_dir, f"bbox_{i * args.batch_size_annotation + j}.jpg"
                     )
                 )
                 plt.close()
 
         # Save annotations as JSON files
-        save_det_annotations_to_json(
-            image_paths, boxes_list, labels_list, args.class_names, save_dir
+        save_annotations_to_json(
+            image_paths=image_paths,
+            labels_list=labels_list,
+            boxes_list=boxes_list,
+            class_names=args.class_names,
+            save_dir=save_dir,
+        )
+
+        if args.dataset_format == "yolo":
+            # Convert annotations to YOLO format
+            convert_dataset.convert_dataset(
+                args.save_dir,
+                args.save_dir,
+                "yolo",
+                args.split_ratios,
+                copy_files=False,
+                seed=args.seed,
+            )
+        # Convert annotations to COCO format
+        elif args.dataset_format == "coco":
+            convert_dataset.convert_dataset(
+                args.save_dir,
+                args.save_dir,
+                "coco",
+                args.split_ratios,
+                copy_files=False,
+                seed=args.seed,
+            )
+
+    # Convert annotations to LuxonisDataset format
+    if args.dataset_format == "luxonis-dataset":
+        convert_dataset.convert_dataset(
+            args.save_dir,
+            args.save_dir,
+            "luxonis-dataset",
+            args.split_ratios,
+            copy_files=False,
+            seed=args.seed,
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `datadreamer-0.1.4/datadreamer/prompt_generation/lm_prompt_generator.py` & `datadreamer-0.1.5/datadreamer/prompt_generation/lm_prompt_generator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/prompt_generation/lm_synonym_generator.py` & `datadreamer-0.1.5/datadreamer/prompt_generation/lm_synonym_generator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/prompt_generation/prompt_generator.py` & `datadreamer-0.1.5/datadreamer/prompt_generation/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/prompt_generation/simple_prompt_generator.py` & `datadreamer-0.1.5/datadreamer/prompt_generation/simple_prompt_generator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/prompt_generation/synonym_generator.py` & `datadreamer-0.1.5/datadreamer/prompt_generation/synonym_generator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/prompt_generation/tinyllama_lm_prompt_generator.py` & `datadreamer-0.1.5/datadreamer/prompt_generation/tinyllama_lm_prompt_generator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/prompt_generation/wordnet_synonym_generator.py` & `datadreamer-0.1.5/datadreamer/prompt_generation/wordnet_synonym_generator.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer/utils/convert_dataset_to_yolo.py` & `datadreamer-0.1.5/datadreamer/utils/yolo_converter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,157 +1,152 @@
 from __future__ import annotations
 
-import argparse
-import json
 import os
 import shutil
 
-import numpy as np
 from PIL import Image
 
+from datadreamer.utils import BaseConverter
 
-def read_annotations(annotation_path):
-    """Reads annotations from a JSON file located at the specified path.
 
-    Args:
-    - annotation_path (str): The path to the JSON file containing annotations.
+class YOLOConverter(BaseConverter):
+    """Class for converting a dataset to YOLO format.
 
-    Returns:
-    - dict: A dictionary containing the data loaded from the JSON file.
-    """
-    with open(annotation_path) as f:
-        data = json.load(f)
-    return data
-
-
-def convert_to_yolo_format(box, image_width, image_height):
-    """Converts bounding box coordinates to YOLO format.
-
-    Args:
-    - box (list of float): A list containing the bounding box coordinates [x_min, y_min, x_max, y_max].
-    - image_width (int): The width of the image.
-    - image_height (int): The height of the image.
+    Format:
 
-    Returns:
-    - list of float: A list containing the bounding box in YOLO format [x_center, y_center, width, height].
+    dataset_dir
+    ├── train
+    │   ├── images
+    │   │   ├── 0.jpg
+    │   │   ├── 1.jpg
+    │   ├── labels
+    │   │   ├── 0.txt
+    │   │   ├── 1.txt
+    ├── val
+    │   ├── images
+    │   ├── labels
+    ├── test
+    │   ├── images
+    │   ├── labels
     """
-    x_center = (box[0] + box[2]) / 2 / image_width
-    y_center = (box[1] + box[3]) / 2 / image_height
-    width = (box[2] - box[0]) / image_width
-    height = (box[3] - box[1]) / image_height
-    return [x_center, y_center, width, height]
-
-
-def process_data(data, image_dir, output_dir, split_ratio):
-    """Processes the data by dividing it into training and validation sets, and saves
-    the images and labels in YOLO format.
-
-    Args:
-    - data (dict): The dictionary containing image annotations.
-    - image_dir (str): The directory where the source images are located.
-    - output_dir (str): The base directory where the processed data will be saved.
-    - split_ratio (float): The ratio to split the data into training and validation sets.
-
-    No return value.
-    """
-    images = list(data.keys())
-    np.random.shuffle(images)
-
-    split_index = int(len(images) * split_ratio)
-    train_images = images[:split_index]
-    val_images = images[split_index:]
-
-    for dataset_type, image_set in [("train", train_images), ("val", val_images)]:
-        image_output_dir = os.path.join(output_dir, dataset_type, "images")
-        label_output_dir = os.path.join(output_dir, dataset_type, "labels")
-
-        # If the output directories already exist, replace them
-        if os.path.exists(image_output_dir):
-            shutil.rmtree(image_output_dir)
-        if os.path.exists(label_output_dir):
-            shutil.rmtree(label_output_dir)
-
-        os.makedirs(image_output_dir)
-        os.makedirs(label_output_dir)
-
-        for image_name in image_set:
-            if image_name == "class_names":
-                continue
-            # extract image name from image path
-            image_full_path = os.path.join(image_dir, image_name)
-            annotation = data[image_name]
-            image = Image.open(image_full_path)
-            image_width, image_height = image.size
-
-            label_file = os.path.join(
-                label_output_dir, os.path.splitext(image_name)[0] + ".txt"
-            )
-            with open(label_file, "w") as f:
-                for box, label in zip(annotation["boxes"], annotation["labels"]):
-                    yolo_box = convert_to_yolo_format(box, image_width, image_height)
-                    f.write(f"{label} {' '.join(map(str, yolo_box))}\n")
-
-            shutil.copy(image_full_path, os.path.join(image_output_dir, image_name))
-
-
-def create_data_yaml(root_dir, class_names):
-    """Creates a YAML file for dataset configuration, specifying paths and class names.
-
-    Args:
-    - root_dir (str): The root directory where the dataset is located.
-    - class_names (list of str): A list of class names.
-
-    No return value.
-    """
-    yaml_content = (
-        f"train: {os.path.abspath(os.path.join(root_dir, 'train'))}\n"
-        f"val: {os.path.abspath(os.path.join(root_dir, 'val'))}\n"
-        f"nc: {len(class_names)}\n"
-        f"names: {class_names}"
-    )
-    with open(os.path.join(root_dir, "data.yaml"), "w") as f:
-        f.write(yaml_content)
-
-
-def convert(dataset_dir, output_dir, train_val_split_ratio):
-    """Converts a dataset into a format suitable for training with YOLO, including
-    creating training and validation splits.
-
-    Args:
-    - dataset_dir (str): The directory where the source dataset is located.
-    - output_dir (str): The directory where the processed dataset should be saved.
-    - train_val_split_ratio (float): The ratio to split the dataset into training and validation sets.
-
-    No return value.
-    """
-    annotation_path = os.path.join(dataset_dir, "annotations.json")
-    data = read_annotations(annotation_path)
-    process_data(data, dataset_dir, output_dir, train_val_split_ratio)
-    create_data_yaml(output_dir, data["class_names"])
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description="Convert dataset to YOLO format with train-val split."
-    )
-    parser.add_argument(
-        "--save_dir", type=str, help="Directory containing the images and annotations."
-    )
-    parser.add_argument(
-        "--output_dir",
-        type=str,
-        help="Directory where the processed dataset will be saved.",
-    )
-    parser.add_argument(
-        "--split_ratio",
-        type=float,
-        default=0.8,
-        help="Train-validation split ratio (default: 0.8)",
-    )
-
-    args = parser.parse_args()
-
-    convert(args.save_dir, args.output_dir, args.split_ratio)
 
+    def __init__(self, seed=42):
+        super().__init__(seed)
 
-if __name__ == "__main__":
-    main()
+    def convert(self, dataset_dir, output_dir, split_ratios, copy_files=True):
+        """Converts a dataset into a format suitable for training with YOLO, including
+        creating training and validation splits.
+
+        Args:
+        - dataset_dir (str): The directory where the source dataset is located.
+        - output_dir (str): The directory where the processed dataset should be saved.
+        - split_ratios (list of float): The ratios to split the data into training, validation, and test sets.
+        - copy_files (bool, optional): Whether to copy the source files to the output directory, otherwise move them. Defaults to True.
+
+        No return value.
+        """
+        annotation_path = os.path.join(dataset_dir, "annotations.json")
+        data = BaseConverter.read_annotations(annotation_path)
+        self.process_data(data, dataset_dir, output_dir, split_ratios, copy_files)
+
+    def convert_to_yolo_format(self, box, image_width, image_height):
+        """Converts bounding box coordinates to YOLO format.
+
+        Args:
+        - box (list of float): A list containing the bounding box coordinates [x_min, y_min, x_max, y_max].
+        - image_width (int): The width of the image.
+        - image_height (int): The height of the image.
+
+        Returns:
+        - list of float: A list containing the bounding box in YOLO format [x_center, y_center, width, height].
+        """
+        x_center = (box[0] + box[2]) / 2 / image_width
+        y_center = (box[1] + box[3]) / 2 / image_height
+        width = (box[2] - box[0]) / image_width
+        height = (box[3] - box[1]) / image_height
+        return [x_center, y_center, width, height]
+
+    def process_data(self, data, image_dir, output_dir, split_ratios, copy_files=True):
+        """Processes the data by dividing it into training and validation sets, and
+        saves the images and labels in YOLO format.
+
+        Args:
+        - data (dict): The dictionary containing image annotations.
+        - image_dir (str): The directory where the source images are located.
+        - output_dir (str): The base directory where the processed data will be saved.
+        - split_ratios (float): The ratio to split the data into training, validation, and test sets.
+        - copy_files (bool, optional): Whether to copy the source files to the output directory, otherwise move them. Defaults to True.
+
+
+        No return value.
+        """
+        images = list(data.keys())
+        images.remove("class_names")
+
+        train_images, val_images, test_images = BaseConverter.make_splits(
+            images, split_ratios
+        )
+
+        for dataset_type, image_set in [
+            ("train", train_images),
+            ("val", val_images),
+            ("test", test_images),
+        ]:
+            image_output_dir = os.path.join(output_dir, dataset_type, "images")
+            label_output_dir = os.path.join(output_dir, dataset_type, "labels")
+
+            # If the output directories already exist, replace them
+            if os.path.exists(image_output_dir):
+                shutil.rmtree(image_output_dir)
+            if os.path.exists(label_output_dir):
+                shutil.rmtree(label_output_dir)
+
+            os.makedirs(image_output_dir)
+            os.makedirs(label_output_dir)
+
+            for image_name in image_set:
+                # extract image name from image path
+                image_full_path = os.path.join(image_dir, image_name)
+                annotation = data[image_name]
+                image = Image.open(image_full_path)
+                image_width, image_height = image.size
+
+                label_file = os.path.join(
+                    label_output_dir, os.path.splitext(image_name)[0] + ".txt"
+                )
+                with open(label_file, "w") as f:
+                    for box, label in zip(annotation["boxes"], annotation["labels"]):
+                        yolo_box = self.convert_to_yolo_format(
+                            box, image_width, image_height
+                        )
+                        f.write(f"{label} {' '.join(map(str, yolo_box))}\n")
+
+                if copy_files:
+                    shutil.copy(
+                        image_full_path, os.path.join(image_output_dir, image_name)
+                    )
+                else:
+                    shutil.move(
+                        image_full_path, os.path.join(image_output_dir, image_name)
+                    )
+
+        self.create_data_yaml(output_dir, data["class_names"])
+
+    def create_data_yaml(self, root_dir, class_names):
+        """Creates a YAML file for dataset configuration, specifying paths and class
+        names.
+
+        Args:
+        - root_dir (str): The root directory where the dataset is located.
+        - class_names (list of str): A list of class names.
+
+        No return value.
+        """
+        yaml_content = (
+            f"train: {os.path.abspath(os.path.join(root_dir, 'train'))}\n"
+            f"val: {os.path.abspath(os.path.join(root_dir, 'val'))}\n"
+            f"test: {os.path.abspath(os.path.join(root_dir, 'test'))}\n"
+            f"nc: {len(class_names)}\n"
+            f"names: {class_names}"
+        )
+        with open(os.path.join(root_dir, "data.yaml"), "w") as f:
+            f.write(yaml_content)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `datadreamer-0.1.4/datadreamer/utils/nms.py` & `datadreamer-0.1.5/datadreamer/utils/nms.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/datadreamer.egg-info/PKG-INFO` & `datadreamer-0.1.5/datadreamer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadreamer
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for dataset generation and knowledge extraction from foundation computer vision models.
 Maintainer-email: Luxonis <support@luxonis.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -228,14 +228,16 @@
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: matplotlib>=3.6.0
 Requires-Dist: opencv-python>=4.7.0
 Requires-Dist: accelerate>=0.25.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: bitsandbytes>=0.42.0
 Requires-Dist: nltk>=3.8.1
+Requires-Dist: luxonis-ml[all]>=0.1.0
+Requires-Dist: python-box>=7.1.1
 Provides-Extra: dev
 Requires-Dist: pre-commit>=3.2.1; extra == "dev"
 Requires-Dist: toml>=0.10.2; extra == "dev"
 
 # DataDreamer
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
@@ -372,48 +374,57 @@
 
 Run the following command in your terminal to use the script:
 
 ```bash
 datadreamer --save_dir <directory> --class_names <objects> --prompts_number <number> [additional options]
 ```
 
+or using a `.yaml` config file
+
+```bash
+datadreamer --config <path-to-config>
+```
+
 <a name="main-parameters"></a>
 
 ### 🎯 Main Parameters
 
 - `--save_dir` (required): Path to the directory for saving generated images and annotations.
 - `--class_names` (required): Space-separated list of object names for image generation and annotation. Example: `person moon robot`.
 - `--prompts_number` (optional): Number of prompts to generate for each object. Defaults to `10`.
 - `--annotate_only` (optional): Only annotate the images without generating new ones, prompt and image generator will be skipped. Defaults to `False`.
 
 <a name="additional-parameters"></a>
 
 ### 🔧 Additional Parameters
 
 - `--task`: Choose between detection and classification. Default is `detection`.
+- `--dataset_format`: Format of the dataset. Defaults to `raw`. Supported values: `raw`, `yolo`, `coco`, `luxonis-dataset`, `cls-single`.
+- `--split_ratios`: Split ratios for train, validation, and test sets. Defaults to `[0.8, 0.1, 0.1]`.
 - `--num_objects_range`: Range of objects in a prompt. Default is 1 to 3.
 - `--prompt_generator`: Choose between `simple`, `lm` (language model) and `tiny` (tiny LM). Default is `simple`.
 - `--image_generator`: Choose image generator, e.g., `sdxl`, `sdxl-turbo` or `sdxl-lightning`. Default is `sdxl-turbo`.
 - `--image_annotator`: Specify the image annotator, like `owlv2` for object detection or `clip` for image classification. Default is `owlv2`.
 - `--conf_threshold`: Confidence threshold for annotation. Default is `0.15`.
 - `--annotation_iou_threshold`: Intersection over Union (IoU) threshold for annotation. Default is `0.2`.
 - `--prompt_prefix`: Prefix to add to every image generation prompt. Default is `""`.
 - `--prompt_suffix`: Suffix to add to every image generation prompt, e.g., for adding details like resolution. Default is `", hd, 8k, highly detailed"`.
 - `--negative_prompt`: Negative prompts to guide the generation away from certain features. Default is `"cartoon, blue skin, painting, scrispture, golden, illustration, worst quality, low quality, normal quality:2, unrealistic dream, low resolution,  static, sd character, low quality, low resolution, greyscale, monochrome, nose, cropped, lowres, jpeg artifacts, deformed iris, deformed pupils, bad eyes, semi-realistic worst quality, bad lips, deformed mouth, deformed face, deformed fingers, bad anatomy"`.
-- `--use_tta`: Toggle test time augmentation for object detection. Default is `True`.
+- `--use_tta`: Toggle test time augmentation for object detection. Default is `False`.
 - `--synonym_generator`: Enhance class names with synonyms. Default is `none`. Other options are `llm`, `wordnet`.
 - `--use_image_tester`: Use image tester for image generation. Default is `False`.
 - `--image_tester_patience`: Patience level for image tester. Default is `1`.
 - `--lm_quantization`: Quantization to use for Mistral language model. Choose between `none` and `4bit`. Default is `none`.
 - `--annotator_size`: Size of the annotator model to use. Choose between `base` and `large`. Default is `base`.
 - `--batch_size_prompt`: Batch size for prompt generation. Default is 64.
-- `--batch_size_annotation`: Batch size for annotation. Default is `8`.
+- `--batch_size_annotation`: Batch size for annotation. Default is `1`.
 - `--batch_size_image`: Batch size for image generation. Default is `1`.
 - `--device`: Choose between `cuda` and `cpu`. Default is `cuda`.
 - `--seed`: Set a random seed for image and prompt generation. Default is `42`.
+- `--config`: A path to an optional `.yaml` config file specifying the pipeline's arguments.
 
 <a name="available-models"></a>
 
 ### 🤖 Available Models
 
 | Model Category    | Model Names                                                                           | Description/Notes                       |
 | ----------------- | ------------------------------------------------------------------------------------- | --------------------------------------- |
@@ -430,16 +441,24 @@
 
 ### 💡 Example
 
 ```bash
 datadreamer --save_dir path/to/save_directory --class_names person moon robot --prompts_number 20 --prompt_generator simple --num_objects_range 1 3 --image_generator sdxl-turbo
 ```
 
+or using a `.yaml` config file (if arguments are provided with the config file in the command, they will override the ones in the config file):
+
+```bash
+datadreamer --save_dir path/to/save_directory --config configs/det_config.yaml
+```
+
 This command generates images for the specified objects, saving them and their annotations in the given directory. The script allows customization of the generation process through various parameters, adapting to different needs and hardware configurations.
 
+See `/configs` folder for some examples of the `.yaml` config files.
+
 <a name="output"></a>
 
 ### 📦 Output
 
 The dataset comprises two primary components: images and their corresponding annotations, stored as JSON files.
 
 ```bash
```

### Comparing `datadreamer-0.1.4/datadreamer.egg-info/SOURCES.txt` & `datadreamer-0.1.5/datadreamer.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -28,19 +28,28 @@
 datadreamer/prompt_generation/lm_synonym_generator.py
 datadreamer/prompt_generation/prompt_generator.py
 datadreamer/prompt_generation/simple_prompt_generator.py
 datadreamer/prompt_generation/synonym_generator.py
 datadreamer/prompt_generation/tinyllama_lm_prompt_generator.py
 datadreamer/prompt_generation/wordnet_synonym_generator.py
 datadreamer/utils/__init__.py
-datadreamer/utils/convert_dataset_to_yolo.py
+datadreamer/utils/base_converter.py
+datadreamer/utils/coco_converter.py
+datadreamer/utils/config.py
+datadreamer/utils/convert_dataset.py
+datadreamer/utils/dataset_utils.py
+datadreamer/utils/luxonis_dataset_converter.py
+datadreamer/utils/merge_raw_datasets.py
 datadreamer/utils/nms.py
+datadreamer/utils/single_label_cls_converter.py
+datadreamer/utils/yolo_converter.py
 examples/image_annotation_example.py
 examples/image_generation_example.py
 examples/measure_batched_prompt_gen_speed.py
 examples/prompt_generation_example.py
 examples/visualize_detection_dataset.py
 tests/integration/test_pipeline.py
 tests/unittests/test_annotators.py
+tests/unittests/test_converters.py
 tests/unittests/test_image_generation.py
 tests/unittests/test_prompt_generation.py
 tools/autogenerate_requirements.py
```

### Comparing `datadreamer-0.1.4/examples/image_annotation_example.py` & `datadreamer-0.1.5/examples/image_annotation_example.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/examples/image_generation_example.py` & `datadreamer-0.1.5/examples/image_generation_example.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/examples/measure_batched_prompt_gen_speed.py` & `datadreamer-0.1.5/examples/measure_batched_prompt_gen_speed.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/examples/visualize_detection_dataset.py` & `datadreamer-0.1.5/examples/visualize_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/pyproject.toml` & `datadreamer-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datadreamer"
-version = "0.1.4"
+version = "0.1.5"
 description = "A library for dataset generation and knowledge extraction from foundation computer vision models."
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 maintainers = [{ name = "Luxonis", email = "support@luxonis.com"}]
 keywords = ["computer vision", "AI", "machine learning", "generative models"]
 dynamic = ["dependencies", "optional-dependencies"]
```

### Comparing `datadreamer-0.1.4/tests/integration/test_pipeline.py` & `datadreamer-0.1.5/tests/integration/test_pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,21 +17,31 @@
     # Run the command
     result = subprocess.run(cmd, shell=True)
     assert result.returncode == 0, "Command failed to run"
     # Check that the target folder is a folder
     assert os.path.isdir(target_folder), "Directory not created"
     files = [
         "annotations.json",
-        "generation_args.json",
-        "image_0.jpg",
+        "generation_args.yaml",
         "prompts.json",
     ]
     # Check that all the files were created
     for file in files:
         assert os.path.isfile(os.path.join(target_folder, file)), f"{file} not created"
+    # Check that an image with an unique was created
+    assert (
+        len(
+            list(
+                filter(
+                    lambda x: "image_" in x and ".jpg" in x, os.listdir(target_folder)
+                )
+            )
+        )
+        > 0
+    ), "Images not created"
     # Check that the "bboxes_visualization" folder was created
     assert os.path.isdir(
         os.path.join(target_folder, "bboxes_visualization")
     ), "bboxes_visualization directory not created"
 
 
 def _check_wrong_argument_choice(cmd: str):
@@ -1042,7 +1052,86 @@
         f"--image_annotator clip "
         f"--image_generator sdxl "
         f"--use_image_tester "
         f"--device cuda"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
+
+
+# =========================================================
+# TEST WITH CONFIG FILE
+# =========================================================
+@pytest.mark.skipif(
+    total_memory < 16 or total_disk_space < 35,
+    reason="Test requires at least 16GB of RAM and 35GB of HDD",
+)
+def test_cpu_simple_sdxl_turbo_config_detection_pipeline():
+    # Define target folder
+    target_folder = "data/data-det-cpu-simple-sdxl-turbo-config/"
+    # Define the command to run the datadreamer
+    cmd = (
+        f"datadreamer --save_dir {target_folder} "
+        f"--num_objects_range 1 2 "
+        f"--config ./sample_config.yaml "
+        f"--device cpu"
+    )
+    # Check the run of the pipeline
+    _check_detection_pipeline(cmd, target_folder)
+
+
+@pytest.mark.skipif(
+    not torch.cuda.is_available() or total_memory < 16 or total_disk_space < 35,
+    reason="Test requires GPU, at least 16GB of RAM and 35GB of HDD",
+)
+def test_cuda_simple_sdxl_turbo_config_detection_pipeline():
+    # Define target folder
+    target_folder = "data/data-det-cuda-simple-sdxl-turbo-config/"
+    # Define the command to run the datadreamer
+    cmd = (
+        f"datadreamer --save_dir {target_folder} "
+        f"--num_objects_range 1 2 "
+        f"--config ./sample_config.yaml "
+        f"--device cuda"
+    )
+    # Check the run of the pipeline
+    _check_detection_pipeline(cmd, target_folder)
+
+
+@pytest.mark.skipif(
+    total_memory < 16 or total_disk_space < 35,
+    reason="Test requires at least 16GB of RAM and 35GB of HDD",
+)
+def test_cpu_simple_sdxl_turbo_config_classification_pipeline():
+    # Define target folder
+    target_folder = "data/data-cls-cpu-simple-sdxl-turbo-config/"
+    # Define the command to run the datadreamer
+    cmd = (
+        f"datadreamer --task classification "
+        f"--save_dir {target_folder} "
+        f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
+        f"--config ./sample_config.yaml "
+        f"--device cpu"
+    )
+    # Check the run of the pipeline
+    _check_detection_pipeline(cmd, target_folder)
+
+
+@pytest.mark.skipif(
+    not torch.cuda.is_available() or total_memory < 16 or total_disk_space < 35,
+    reason="Test requires GPU, at least 16GB of RAM and 35GB of HDD",
+)
+def test_cuda_simple_sdxl_turbo_config_classification_pipeline():
+    # Define target folder
+    target_folder = "data/data-cls-cuda-simple-sdxl-turbo-config/"
+    # Define the command to run the datadreamer
+    cmd = (
+        f"datadreamer --task classification "
+        f"--save_dir {target_folder} "
+        f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
+        f"--config ./sample_config.yaml "
+        f"--device cuda"
+    )
+    # Check the run of the pipeline
+    _check_detection_pipeline(cmd, target_folder)
```

### Comparing `datadreamer-0.1.4/tests/unittests/test_annotators.py` & `datadreamer-0.1.5/tests/unittests/test_annotators.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/tests/unittests/test_image_generation.py` & `datadreamer-0.1.5/tests/unittests/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/tests/unittests/test_prompt_generation.py` & `datadreamer-0.1.5/tests/unittests/test_prompt_generation.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.4/tools/autogenerate_requirements.py` & `datadreamer-0.1.5/tools/autogenerate_requirements.py`

 * *Files identical despite different names*

