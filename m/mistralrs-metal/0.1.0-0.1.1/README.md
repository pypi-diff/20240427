# Comparing `tmp/mistralrs_metal-0.1.0.tar.gz` & `tmp/mistralrs_metal-0.1.1.tar.gz`

## Comparing `mistralrs_metal-0.1.0.tar` & `mistralrs_metal-0.1.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0     1000     1000     1809 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.0/mistralrs-core/Cargo.toml
--rw-r--r--   0     1000     1000        0 2024-04-26 16:25:02.000000 mistralrs_metal-0.1.0/mistralrs-core/README.md
--rw-r--r--   0     1000     1000      133 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.0/mistralrs-core/src/aici/README.md
--rw-r--r--   0     1000     1000     6551 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.0/mistralrs-core/src/aici/bintokens.rs
--rw-r--r--   0     1000     1000      320 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.0/mistralrs-core/src/aici/bytes.rs
--rw-r--r--   0     1000     1000    15114 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.0/mistralrs-core/src/aici/cfg.rs
--rw-r--r--   0     1000     1000     9819 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.0/mistralrs-core/src/aici/lex.rs
--rw-r--r--   0     1000     1000      179 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.0/mistralrs-core/src/aici/mod.rs
--rw-r--r--   0     1000     1000     2447 2024-04-19 18:01:00.000000 mistralrs_metal-0.1.0/mistralrs-core/src/aici/recognizer.rs
--rw-r--r--   0     1000     1000     1696 2024-04-12 01:34:41.000000 mistralrs_metal-0.1.0/mistralrs-core/src/aici/rx.rs
--rw-r--r--   0     1000     1000     3094 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.0/mistralrs-core/src/aici/svob.rs
--rw-r--r--   0     1000     1000    17311 2024-04-19 18:01:00.000000 mistralrs_metal-0.1.0/mistralrs-core/src/aici/toktree.rs
--rw-r--r--   0     1000     1000     2935 2024-04-25 14:28:35.000000 mistralrs_metal-0.1.0/mistralrs-core/src/device_map.rs
--rw-r--r--   0     1000     1000    30518 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.0/mistralrs-core/src/engine/mod.rs
--rw-r--r--   0     1000     1000     7286 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.0/mistralrs-core/src/layers.rs
--rw-r--r--   0     1000     1000     7646 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.0/mistralrs-core/src/lib.rs
--rw-r--r--   0     1000     1000     8310 2024-04-25 00:00:52.000000 mistralrs_metal-0.1.0/mistralrs-core/src/model_loader.rs
--rw-r--r--   0     1000     1000    10703 2024-04-27 09:46:04.000000 mistralrs_metal-0.1.0/mistralrs-core/src/model_selected.rs
--rw-r--r--   0     1000     1000    15669 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/models/gemma.rs
--rw-r--r--   0     1000     1000    14022 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/models/llama.rs
--rw-r--r--   0     1000     1000    15585 2024-04-27 09:51:16.000000 mistralrs_metal-0.1.0/mistralrs-core/src/models/mistral.rs
--rw-r--r--   0     1000     1000    20102 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/models/mixtral.rs
--rw-r--r--   0     1000     1000     2620 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.0/mistralrs-core/src/models/mod.rs
--rw-r--r--   0     1000     1000    14708 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/models/phi2.rs
--rw-r--r--   0     1000     1000    14527 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/models/phi3.rs
--rw-r--r--   0     1000     1000    19588 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.0/mistralrs-core/src/models/quantized_llama.rs
--rw-r--r--   0     1000     1000    10095 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.0/mistralrs-core/src/models/quantized_phi2.rs
--rw-r--r--   0     1000     1000    15130 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/models/qwen2.rs
--rw-r--r--   0     1000     1000     4424 2024-04-25 23:09:22.000000 mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/chat_template.rs
--rw-r--r--   0     1000     1000    14978 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/ggml.rs
--rw-r--r--   0     1000     1000    17012 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/gguf.rs
--rw-r--r--   0     1000     1000    19303 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/loaders.rs
--rw-r--r--   0     1000     1000     9048 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/macros.rs
--rw-r--r--   0     1000     1000    32323 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/mod.rs
--rw-r--r--   0     1000     1000    12875 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/normal.rs
--rw-r--r--   0     1000     1000     6358 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.0/mistralrs-core/src/prefix_cacher.rs
--rw-r--r--   0     1000     1000     1241 2024-04-26 13:13:55.000000 mistralrs_metal-0.1.0/mistralrs-core/src/request.rs
--rw-r--r--   0     1000     1000     3848 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.0/mistralrs-core/src/response.rs
--rw-r--r--   0     1000     1000    10578 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.0/mistralrs-core/src/sampler.rs
--rw-r--r--   0     1000     1000     7286 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.0/mistralrs-core/src/scheduler.rs
--rw-r--r--   0     1000     1000    15888 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.0/mistralrs-core/src/sequence.rs
--rw-r--r--   0     1000     1000     7016 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.0/mistralrs-core/src/utils/mod.rs
--rw-r--r--   0     1000     1000     1154 2024-04-09 21:45:17.000000 mistralrs_metal-0.1.0/mistralrs-core/src/utils/tokens.rs
--rw-r--r--   0     1000     1000     4799 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.0/mistralrs-core/src/utils/varbuilder_utils.rs
--rw-r--r--   0     1000     1000    11049 2024-04-06 02:02:23.000000 mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/classifier.rs
--rw-r--r--   0     1000     1000     1544 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/config.rs
--rw-r--r--   0     1000     1000    24214 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/gemma.rs
--rw-r--r--   0     1000     1000    21882 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/llama.rs
--rw-r--r--   0     1000     1000    23588 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/mistral.rs
--rw-r--r--   0     1000     1000    28628 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/mixtral.rs
--rw-r--r--   0     1000     1000     4181 2024-04-25 18:24:04.000000 mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/mod.rs
--rw-r--r--   0     1000     1000    22218 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/phi2.rs
--rw-r--r--   0     1000     1000    21111 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/phi3.rs
--rw-r--r--   0     1000     1000    34138 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/quantized_llama.rs
--rw-r--r--   0     1000     1000      794 2024-04-26 00:59:23.000000 mistralrs_metal-0.1.0/mistralrs-lora/Cargo.toml
--rw-r--r--   0     1000     1000        0 2024-04-26 16:25:02.000000 mistralrs_metal-0.1.0/mistralrs-lora/README.md
--rw-r--r--   0     1000     1000     2395 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.0/mistralrs-lora/src/layer.rs
--rw-r--r--   0     1000     1000     5657 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.0/mistralrs-lora/src/lib.rs
--rw-r--r--   0     1000     1000     9437 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.0/mistralrs-lora/src/loralinear.rs
--rw-r--r--   0     1000     1000     9937 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.0/mistralrs-lora/src/qloralinear.rs
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/Cargo.toml
--rw-r--r--   0     1000     1000      686 2024-03-08 12:45:25.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/.gitignore
--rw-r--r--   0     1000     1000     3516 2024-04-27 09:46:04.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/API.md
--rw-r--r--   0     1000     1000      819 2024-04-27 10:12:38.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/Cargo_template.toml
--rw-r--r--   0     1000     1000     3755 2024-04-27 10:12:38.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/README.md
--rw-r--r--   0     1000     1000     8231 2024-04-27 02:02:03.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/mistralrs.pyi
--rw-r--r--   0     1000     1000      530 2024-04-27 10:24:09.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/pyproject_template.toml
--rw-r--r--   0     1000     1000    28363 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/src/lib.rs
--rw-r--r--   0     1000     1000      397 2024-04-25 14:28:35.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/src/message.rs
--rw-r--r--   0     1000     1000     1590 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/src/stream.rs
--rw-r--r--   0     1000     1000     3058 2024-04-25 00:00:52.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/src/which.rs
--rwxr-xr-x   0     1000     1000     2045 2024-04-27 10:24:55.000000 mistralrs_metal-0.1.0/mistralrs-pyo3/upload.py
--rw-r--r--   0     1000     1000    97009 2024-04-27 10:11:43.000000 mistralrs_metal-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 mistralrs_metal-0.1.0/Cargo.toml
--rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 mistralrs_metal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4451 1970-01-01 00:00:00.000000 mistralrs_metal-0.1.0/PKG-INFO
+-rw-r--r--   0     1000     1000      794 2024-04-26 00:59:23.000000 mistralrs_metal-0.1.1/mistralrs-lora/Cargo.toml
+-rw-r--r--   0     1000     1000        0 2024-04-26 16:25:02.000000 mistralrs_metal-0.1.1/mistralrs-lora/README.md
+-rw-r--r--   0     1000     1000     2395 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.1/mistralrs-lora/src/layer.rs
+-rw-r--r--   0     1000     1000     5657 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.1/mistralrs-lora/src/lib.rs
+-rw-r--r--   0     1000     1000     9437 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.1/mistralrs-lora/src/loralinear.rs
+-rw-r--r--   0     1000     1000     9937 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.1/mistralrs-lora/src/qloralinear.rs
+-rw-r--r--   0     1000     1000     1809 2024-04-27 15:00:53.000000 mistralrs_metal-0.1.1/mistralrs-core/Cargo.toml
+-rw-r--r--   0     1000     1000        0 2024-04-26 16:25:02.000000 mistralrs_metal-0.1.1/mistralrs-core/README.md
+-rw-r--r--   0     1000     1000      133 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.1/mistralrs-core/src/aici/README.md
+-rw-r--r--   0     1000     1000     6551 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.1/mistralrs-core/src/aici/bintokens.rs
+-rw-r--r--   0     1000     1000      320 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.1/mistralrs-core/src/aici/bytes.rs
+-rw-r--r--   0     1000     1000    15114 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.1/mistralrs-core/src/aici/cfg.rs
+-rw-r--r--   0     1000     1000     9819 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.1/mistralrs-core/src/aici/lex.rs
+-rw-r--r--   0     1000     1000      179 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.1/mistralrs-core/src/aici/mod.rs
+-rw-r--r--   0     1000     1000     2447 2024-04-19 18:01:00.000000 mistralrs_metal-0.1.1/mistralrs-core/src/aici/recognizer.rs
+-rw-r--r--   0     1000     1000     1696 2024-04-12 01:34:41.000000 mistralrs_metal-0.1.1/mistralrs-core/src/aici/rx.rs
+-rw-r--r--   0     1000     1000     3094 2024-04-11 10:11:30.000000 mistralrs_metal-0.1.1/mistralrs-core/src/aici/svob.rs
+-rw-r--r--   0     1000     1000    17311 2024-04-19 18:01:00.000000 mistralrs_metal-0.1.1/mistralrs-core/src/aici/toktree.rs
+-rw-r--r--   0     1000     1000     2935 2024-04-25 14:28:35.000000 mistralrs_metal-0.1.1/mistralrs-core/src/device_map.rs
+-rw-r--r--   0     1000     1000    30518 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.1/mistralrs-core/src/engine/mod.rs
+-rw-r--r--   0     1000     1000     7286 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.1/mistralrs-core/src/layers.rs
+-rw-r--r--   0     1000     1000     7646 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.1/mistralrs-core/src/lib.rs
+-rw-r--r--   0     1000     1000     8310 2024-04-25 00:00:52.000000 mistralrs_metal-0.1.1/mistralrs-core/src/model_loader.rs
+-rw-r--r--   0     1000     1000    10703 2024-04-27 09:46:04.000000 mistralrs_metal-0.1.1/mistralrs-core/src/model_selected.rs
+-rw-r--r--   0     1000     1000    15669 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/models/gemma.rs
+-rw-r--r--   0     1000     1000    14022 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/models/llama.rs
+-rw-r--r--   0     1000     1000    15585 2024-04-27 09:51:16.000000 mistralrs_metal-0.1.1/mistralrs-core/src/models/mistral.rs
+-rw-r--r--   0     1000     1000    20102 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/models/mixtral.rs
+-rw-r--r--   0     1000     1000     2620 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.1/mistralrs-core/src/models/mod.rs
+-rw-r--r--   0     1000     1000    14708 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/models/phi2.rs
+-rw-r--r--   0     1000     1000    14527 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/models/phi3.rs
+-rw-r--r--   0     1000     1000    19588 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.1/mistralrs-core/src/models/quantized_llama.rs
+-rw-r--r--   0     1000     1000    10095 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.1/mistralrs-core/src/models/quantized_phi2.rs
+-rw-r--r--   0     1000     1000    15130 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/models/qwen2.rs
+-rw-r--r--   0     1000     1000     4424 2024-04-25 23:09:22.000000 mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/chat_template.rs
+-rw-r--r--   0     1000     1000    14978 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/ggml.rs
+-rw-r--r--   0     1000     1000    17012 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/gguf.rs
+-rw-r--r--   0     1000     1000    19303 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/loaders.rs
+-rw-r--r--   0     1000     1000     9952 2024-04-27 14:43:53.000000 mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/macros.rs
+-rw-r--r--   0     1000     1000    32323 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/mod.rs
+-rw-r--r--   0     1000     1000    12875 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/normal.rs
+-rw-r--r--   0     1000     1000     6358 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.1/mistralrs-core/src/prefix_cacher.rs
+-rw-r--r--   0     1000     1000     1241 2024-04-26 13:13:55.000000 mistralrs_metal-0.1.1/mistralrs-core/src/request.rs
+-rw-r--r--   0     1000     1000     3848 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.1/mistralrs-core/src/response.rs
+-rw-r--r--   0     1000     1000    10578 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.1/mistralrs-core/src/sampler.rs
+-rw-r--r--   0     1000     1000     7286 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.1/mistralrs-core/src/scheduler.rs
+-rw-r--r--   0     1000     1000    15888 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.1/mistralrs-core/src/sequence.rs
+-rw-r--r--   0     1000     1000     7016 2024-04-27 10:11:41.000000 mistralrs_metal-0.1.1/mistralrs-core/src/utils/mod.rs
+-rw-r--r--   0     1000     1000     1716 2024-04-27 14:58:30.000000 mistralrs_metal-0.1.1/mistralrs-core/src/utils/tokens.rs
+-rw-r--r--   0     1000     1000     4799 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.1/mistralrs-core/src/utils/varbuilder_utils.rs
+-rw-r--r--   0     1000     1000    11049 2024-04-06 02:02:23.000000 mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/classifier.rs
+-rw-r--r--   0     1000     1000     1544 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/config.rs
+-rw-r--r--   0     1000     1000    24214 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/gemma.rs
+-rw-r--r--   0     1000     1000    21882 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/llama.rs
+-rw-r--r--   0     1000     1000    23588 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/mistral.rs
+-rw-r--r--   0     1000     1000    28628 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/mixtral.rs
+-rw-r--r--   0     1000     1000     4181 2024-04-25 18:24:04.000000 mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/mod.rs
+-rw-r--r--   0     1000     1000    22218 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/phi2.rs
+-rw-r--r--   0     1000     1000    21111 2024-04-27 02:47:50.000000 mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/phi3.rs
+-rw-r--r--   0     1000     1000    34138 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/quantized_llama.rs
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/Cargo.toml
+-rw-r--r--   0     1000     1000      686 2024-03-08 12:45:25.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/.gitignore
+-rw-r--r--   0     1000     1000     3516 2024-04-27 09:46:04.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/API.md
+-rw-r--r--   0     1000     1000      819 2024-04-27 15:00:53.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/Cargo_template.toml
+-rw-r--r--   0     1000     1000     3755 2024-04-27 10:12:38.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/README.md
+-rw-r--r--   0     1000     1000     8231 2024-04-27 02:02:03.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/mistralrs.pyi
+-rw-r--r--   0     1000     1000      530 2024-04-27 15:00:53.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/pyproject_template.toml
+-rw-r--r--   0     1000     1000    28363 2024-04-26 13:56:27.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/src/lib.rs
+-rw-r--r--   0     1000     1000      397 2024-04-25 14:28:35.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/src/message.rs
+-rw-r--r--   0     1000     1000     1590 2024-04-23 22:49:11.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/src/stream.rs
+-rw-r--r--   0     1000     1000     3058 2024-04-25 00:00:52.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/src/which.rs
+-rwxr-xr-x   0     1000     1000     2044 2024-04-27 10:25:16.000000 mistralrs_metal-0.1.1/mistralrs-pyo3/upload.py
+-rw-r--r--   0     1000     1000    97009 2024-04-27 15:00:53.000000 mistralrs_metal-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 mistralrs_metal-0.1.1/Cargo.toml
+-rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 mistralrs_metal-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4451 1970-01-01 00:00:00.000000 mistralrs_metal-0.1.1/PKG-INFO
```

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/Cargo.toml` & `mistralrs_metal-0.1.1/mistralrs-core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 dirs = "5.0.1"
 hf-hub = "0.3.2"
 thiserror = "1.0.57"
 tokenizers = "0.15.2"
 tqdm = "0.7.0"
 range-checked = { git = "https://github.com/EricLBuehler/range-checked.git", version = "0.1.0" }
 chrono = "0.4.34"
-mistralrs-lora = { version = "0.1.0", path = "../mistralrs-lora" }
+mistralrs-lora = { version = "0.1.1", path = "../mistralrs-lora" }
 minijinja = "1.0.12"
 either.workspace = true
 indexmap.workspace = true
 half = "2.4.0"
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 tracing.workspace = true
```

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/aici/bintokens.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/aici/bintokens.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/aici/cfg.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/aici/cfg.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/aici/lex.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/aici/lex.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/aici/recognizer.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/aici/recognizer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/aici/rx.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/aici/rx.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/aici/svob.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/aici/svob.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/aici/toktree.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/aici/toktree.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/device_map.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/device_map.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/engine/mod.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/engine/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/layers.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/layers.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/lib.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/model_loader.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/model_loader.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/model_selected.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/model_selected.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/models/gemma.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/models/gemma.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/models/llama.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/models/llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/models/mistral.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/models/mistral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/models/mixtral.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/models/mixtral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/models/mod.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/models/phi2.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/models/phi2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/models/phi3.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/models/phi3.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/models/quantized_llama.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/models/quantized_llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/models/quantized_phi2.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/models/quantized_phi2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/models/qwen2.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/models/qwen2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/chat_template.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/chat_template.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/ggml.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/ggml.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/gguf.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/gguf.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/loaders.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/loaders.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/macros.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/macros.rs`

 * *Files 4% similar despite different names*

```diff
@@ -4,34 +4,55 @@
         $api.info()
             .map(|repo| {
                 repo.siblings
                     .iter()
                     .map(|x| x.rfilename.clone())
                     .collect::<Vec<String>>()
             })
-            .unwrap_or(
-                std::fs::read_dir($model_id)?
+            .unwrap_or_else(|e| {
+                // If we do not get a 404, it was something else.
+                let format = format!("{e:?}");
+                if let hf_hub::api::sync::ApiError::RequestError(resp) = e {
+                    if resp.into_response().is_some_and(|r| r.status() != 404) {
+                        panic!("{format}");
+                    }
+                }
+
+                let listing = std::fs::read_dir($model_id);
+                if listing.is_err() {
+                    panic!("Cannot list directory {:?}", $model_id)
+                }
+                let listing = listing.unwrap();
+                listing
                     .into_iter()
                     .map(|s| {
                         s.unwrap()
                             .path()
                             .to_str()
                             .expect("Could not convert to str")
                             .to_string()
                     })
-                    .collect::<Vec<String>>(),
-            )
+                    .collect::<Vec<String>>()
+            })
             .into_iter()
     };
 }
 
 #[macro_export]
 macro_rules! api_get_file {
     ($api:expr, $file:expr, $model_id:expr) => {
-        $api.get($file).unwrap_or_else(|_| {
+        $api.get($file).unwrap_or_else(|e| {
+            // If we do not get a 404, it was something else.
+            let format = format!("{e:?}");
+            if let hf_hub::api::sync::ApiError::RequestError(resp) = e {
+                if resp.into_response().is_some_and(|r| r.status() != 404) {
+                    panic!("{format}");
+                }
+            }
+
             let path = $model_id.join($file);
             if !path.exists() {
                 panic!("File \"{}\" not found at model id {:?}", $file, $model_id)
             }
             path
         })
     };
```

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/mod.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/pipeline/normal.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/pipeline/normal.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/prefix_cacher.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/prefix_cacher.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/request.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/request.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/response.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/response.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/sampler.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/sampler.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/scheduler.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/scheduler.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/sequence.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/sequence.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/utils/mod.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/utils/varbuilder_utils.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/utils/varbuilder_utils.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/classifier.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/classifier.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/config.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/config.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/gemma.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/gemma.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/llama.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/mistral.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/mistral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/mixtral.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/mixtral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/mod.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/phi2.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/phi2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/phi3.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/phi3.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-core/src/xlora_models/quantized_llama.rs` & `mistralrs_metal-0.1.1/mistralrs-core/src/xlora_models/quantized_llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-lora/Cargo.toml` & `mistralrs_metal-0.1.1/mistralrs-lora/Cargo.toml`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-lora/src/layer.rs` & `mistralrs_metal-0.1.1/mistralrs-lora/src/layer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-lora/src/lib.rs` & `mistralrs_metal-0.1.1/mistralrs-lora/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-lora/src/loralinear.rs` & `mistralrs_metal-0.1.1/mistralrs-lora/src/loralinear.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-lora/src/qloralinear.rs` & `mistralrs_metal-0.1.1/mistralrs-lora/src/qloralinear.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-pyo3/Cargo.toml` & `mistralrs_metal-0.1.1/mistralrs-pyo3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.0", path = "../mistralrs-core", features=["metal"] }
+mistralrs-core = { version = "0.1.1", path = "../mistralrs-core", features=["metal"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["metal"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
```

### Comparing `mistralrs_metal-0.1.0/mistralrs-pyo3/.gitignore` & `mistralrs_metal-0.1.1/mistralrs-pyo3/.gitignore`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-pyo3/API.md` & `mistralrs_metal-0.1.1/mistralrs-pyo3/API.md`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-pyo3/Cargo_template.toml` & `mistralrs_metal-0.1.1/mistralrs-pyo3/Cargo_template.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.0", path = "../mistralrs-core", features=["$feature_name"] }
+mistralrs-core = { version = "0.1.1", path = "../mistralrs-core", features=["$feature_name"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["$feature_name"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
```

### Comparing `mistralrs_metal-0.1.0/mistralrs-pyo3/README.md` & `mistralrs_metal-0.1.1/mistralrs-pyo3/README.md`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-pyo3/mistralrs.pyi` & `mistralrs_metal-0.1.1/mistralrs-pyo3/mistralrs.pyi`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-pyo3/pyproject_template.toml` & `mistralrs_metal-0.1.1/mistralrs-pyo3/pyproject_template.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
 name = "$name"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mistralrs_metal-0.1.0/mistralrs-pyo3/src/lib.rs` & `mistralrs_metal-0.1.1/mistralrs-pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-pyo3/src/stream.rs` & `mistralrs_metal-0.1.1/mistralrs-pyo3/src/stream.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-pyo3/src/which.rs` & `mistralrs_metal-0.1.1/mistralrs-pyo3/src/which.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_metal-0.1.0/mistralrs-pyo3/upload.py` & `mistralrs_metal-0.1.1/mistralrs-pyo3/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 print(
     f"⭐ Generated sdists for features {[k for k,_ in features.items()]} with corresponding names {[v for _,v in features.items()]}"
 )
 
 # Generate CPU lib
-#os.system("maturin sdist --out dist")
+os.system("maturin sdist --out dist")
 
 password = input("Enter API token: ")
 target = input("Enter target (testpypi or pypi): ")
 print(f"🚀 Uploading to {target} in 5 seconds. Press <CTRL>-C to abort.")
 time.sleep(5)
 
 # Upload
```

### Comparing `mistralrs_metal-0.1.0/Cargo.lock` & `mistralrs_metal-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1807,24 +1807,24 @@
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mistralrs"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "candle-core",
  "mistralrs-core",
 ]
 
 [[package]]
 name = "mistralrs-bench"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "candle-core",
  "clap",
  "cli-table",
  "either",
  "mistralrs-core",
@@ -1832,15 +1832,15 @@
  "serde_json",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-core"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "bytemuck",
  "candle-core",
  "candle-flash-attn",
  "candle-nn",
@@ -1871,28 +1871,28 @@
  "tqdm",
  "tracing",
  "vob",
 ]
 
 [[package]]
 name = "mistralrs-lora"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "candle-nn",
  "either",
  "intel-mkl-src",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "mistralrs-pyo3"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "either",
  "futures",
  "indexmap",
  "intel-mkl-src",
@@ -1900,15 +1900,15 @@
  "pyo3",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "mistralrs-server"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "axum",
  "candle-core",
  "clap",
  "dyn-fmt",
```

### Comparing `mistralrs_metal-0.1.0/Cargo.toml` & `mistralrs_metal-0.1.1/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["mistralrs-core", "mistralrs-lora", "mistralrs-pyo3"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 description = "Fast and easy LLM serving."
 homepage = "https://github.com/EricLBuehler/mistral.rs"
 repository = "https://github.com/EricLBuehler/mistral.rs"
 keywords = ["machine-learning"]
 categories = ["science"]
 license = "MIT"
```

### Comparing `mistralrs_metal-0.1.0/pyproject.toml` & `mistralrs_metal-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
 name = "mistralrs-metal"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mistralrs_metal-0.1.0/PKG-INFO` & `mistralrs_metal-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistralrs-metal
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Rust
 Summary: Fast and easy LLM serving.
```

