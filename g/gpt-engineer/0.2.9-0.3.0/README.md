# Comparing `tmp/gpt_engineer-0.2.9.tar.gz` & `tmp/gpt_engineer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_engineer-0.2.9.tar", max compression
+gzip compressed data, was "gpt_engineer-0.3.0.tar", max compression
```

## Comparing `gpt_engineer-0.2.9.tar` & `gpt_engineer-0.3.0.tar`

### file list

```diff
@@ -1,65 +1,68 @@
--rw-r--r--   0        0        0     1068 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/LICENSE
--rw-r--r--   0        0        0     5024 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/README.md
--rw-r--r--   0        0        0      160 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/__init__.py
--rw-r--r--   0        0        0     8888 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/cli_agent.py
--rw-r--r--   0        0        0     5749 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/collect.py
--rw-r--r--   0        0        0    17912 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/file_selector.py
--rw-r--r--   0        0        0     9812 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/learning.py
--rw-r--r--   0        0        0    16232 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/main.py
--rw-r--r--   0        0        0     3200 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/__main__.py
--rw-r--r--   0        0        0     3822 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/apps/load.py
--rw-r--r--   0        0        0      555 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/apps/problem.py
--rw-r--r--   0        0        0       98 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/apps/problems.py
--rw-r--r--   0        0        0      381 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/__init__.py
--rw-r--r--   0        0        0     6202 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/eval_tools.py
--rw-r--r--   0        0        0     1631 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/EVAL_NEW_CODE_RESULTS.md
--rw-r--r--   0        0        0     4331 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/IMPROVE_CODE_RESULTS.md
--rw-r--r--   0        0        0      645 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/README.md
--rw-r--r--   0        0        0     2813 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/snake_game_files.txt
--rw-r--r--   0        0        0     2744 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/web_todo_files.txt
--rw-r--r--   0        0        0     7958 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/load.py
--rw-r--r--   0        0        0     4086 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gptme/load.py
--rw-r--r--   0        0        0     1320 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/load.py
--rw-r--r--   0        0        0     3587 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/mbpp/load.py
--rw-r--r--   0        0        0      531 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/mbpp/problem.py
--rw-r--r--   0        0        0       93 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/mbpp/problems.py
--rw-r--r--   0        0        0     4244 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/run.py
--rw-r--r--   0        0        0     2417 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/types.py
--rw-r--r--   0        0        0        0 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/__init__.py
--rw-r--r--   0        0        0    14416 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/ai.py
--rw-r--r--   0        0        0     1015 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/base_agent.py
--rw-r--r--   0        0        0     1191 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/base_execution_env.py
--rw-r--r--   0        0        0      485 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/base_memory.py
--rw-r--r--   0        0        0     8902 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/chat_to_files.py
--rw-r--r--   0        0        0        0 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/__init__.py
--rw-r--r--   0        0        0      387 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/constants.py
--rw-r--r--   0        0        0     3618 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/disk_execution_env.py
--rw-r--r--   0        0        0     9680 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/disk_memory.py
--rw-r--r--   0        0        0     1802 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/file_store.py
--rw-r--r--   0        0        0     2370 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/paths.py
--rw-r--r--   0        0        0     3582 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/simple_agent.py
--rw-r--r--   0        0        0    11984 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/steps.py
--rw-r--r--   0        0        0    19158 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/diff.py
--rw-r--r--   0        0        0     3877 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/files_dict.py
--rw-r--r--   0        0        0     2389 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/git.py
--rw-r--r--   0        0        0      869 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/preprompts_holder.py
--rw-r--r--   0        0        0     4993 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/project_config.py
--rw-r--r--   0        0        0      901 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/prompt.py
--rw-r--r--   0        0        0     9483 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/token_usage.py
--rw-r--r--   0        0        0      917 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/version_manager.py
--rw-r--r--   0        0        0      228 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/clarify
--rw-r--r--   0        0        0      432 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/entrypoint
--rw-r--r--   0        0        0      496 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/file_format
--rw-r--r--   0        0        0     1555 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/file_format_diff
--rw-r--r--   0        0        0      498 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/file_format_fix
--rw-r--r--   0        0        0      998 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/generate
--rw-r--r--   0        0        0     1146 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/improve
--rw-r--r--   0        0        0      548 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/philosophy
--rw-r--r--   0        0        0      165 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/roadmap
--rw-r--r--   0        0        0        0 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/tools/__init__.py
--rw-r--r--   0        0        0     7691 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/tools/custom_steps.py
--rw-r--r--   0        0        0     1884 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/tools/supported_languages.py
--rw-r--r--   0        0        0     2661 2024-04-12 09:05:38.896566 gpt_engineer-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     6592 1970-01-01 00:00:00.000000 gpt_engineer-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5442 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/README.md
+-rw-r--r--   0        0        0      160 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/applications/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/applications/cli/__init__.py
+-rw-r--r--   0        0        0     8888 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/applications/cli/cli_agent.py
+-rw-r--r--   0        0        0     5749 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/applications/cli/collect.py
+-rw-r--r--   0        0        0    17912 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/applications/cli/file_selector.py
+-rw-r--r--   0        0        0     9834 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/applications/cli/learning.py
+-rw-r--r--   0        0        0    16225 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/applications/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/__init__.py
+-rw-r--r--   0        0        0     4121 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/__main__.py
+-rw-r--r--   0        0        0     1525 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/bench_config.py
+-rw-r--r--   0        0        0     4082 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/apps/load.py
+-rw-r--r--   0        0        0      555 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/apps/problem.py
+-rw-r--r--   0        0        0       98 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/apps/problems.py
+-rw-r--r--   0        0        0      381 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/__init__.py
+-rw-r--r--   0        0        0     6202 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/eval_tools.py
+-rw-r--r--   0        0        0     1631 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/evals/EVAL_NEW_CODE_RESULTS.md
+-rw-r--r--   0        0        0     4331 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/evals/IMPROVE_CODE_RESULTS.md
+-rw-r--r--   0        0        0      645 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/evals/README.md
+-rw-r--r--   0        0        0     2813 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/snake_game_files.txt
+-rw-r--r--   0        0        0     2744 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/web_todo_files.txt
+-rw-r--r--   0        0        0     8104 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/load.py
+-rw-r--r--   0        0        0     4178 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gptme/load.py
+-rw-r--r--   0        0        0     1504 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/load.py
+-rw-r--r--   0        0        0     3764 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/mbpp/load.py
+-rw-r--r--   0        0        0      531 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/mbpp/problem.py
+-rw-r--r--   0        0        0       93 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/mbpp/problems.py
+-rw-r--r--   0        0        0      301 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/default_bench_config.toml
+-rw-r--r--   0        0        0     4080 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/run.py
+-rw-r--r--   0        0        0     2417 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/benchmark/types.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/__init__.py
+-rw-r--r--   0        0        0    14560 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/ai.py
+-rw-r--r--   0        0        0     1015 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/base_agent.py
+-rw-r--r--   0        0        0     1191 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/base_execution_env.py
+-rw-r--r--   0        0        0      485 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/base_memory.py
+-rw-r--r--   0        0        0     8902 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/chat_to_files.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/default/__init__.py
+-rw-r--r--   0        0        0      387 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/default/constants.py
+-rw-r--r--   0        0        0     3618 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/default/disk_execution_env.py
+-rw-r--r--   0        0        0     9680 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/default/disk_memory.py
+-rw-r--r--   0        0        0     1802 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/default/file_store.py
+-rw-r--r--   0        0        0     2370 2024-04-27 18:40:12.663485 gpt_engineer-0.3.0/gpt_engineer/core/default/paths.py
+-rw-r--r--   0        0        0     3582 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/core/default/simple_agent.py
+-rw-r--r--   0        0        0    12097 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/core/default/steps.py
+-rw-r--r--   0        0        0    19158 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/core/diff.py
+-rw-r--r--   0        0        0     3877 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/core/files_dict.py
+-rw-r--r--   0        0        0     2389 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/core/git.py
+-rw-r--r--   0        0        0      869 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/core/preprompts_holder.py
+-rw-r--r--   0        0        0     4993 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/core/project_config.py
+-rw-r--r--   0        0        0     1162 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/core/prompt.py
+-rw-r--r--   0        0        0     9483 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/core/token_usage.py
+-rw-r--r--   0        0        0      917 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/core/version_manager.py
+-rw-r--r--   0        0        0      228 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/preprompts/clarify
+-rw-r--r--   0        0        0      432 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/preprompts/entrypoint
+-rw-r--r--   0        0        0      496 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/preprompts/file_format
+-rw-r--r--   0        0        0     1555 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/preprompts/file_format_diff
+-rw-r--r--   0        0        0      498 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/preprompts/file_format_fix
+-rw-r--r--   0        0        0      998 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/preprompts/generate
+-rw-r--r--   0        0        0     1146 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/preprompts/improve
+-rw-r--r--   0        0        0      548 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/preprompts/philosophy
+-rw-r--r--   0        0        0      165 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/preprompts/roadmap
+-rw-r--r--   0        0        0        0 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/tools/__init__.py
+-rw-r--r--   0        0        0     7691 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/tools/custom_steps.py
+-rw-r--r--   0        0        0     1884 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/gpt_engineer/tools/supported_languages.py
+-rw-r--r--   0        0        0     2825 2024-04-27 18:40:12.667485 gpt_engineer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7007 1970-01-01 00:00:00.000000 gpt_engineer-0.3.0/PKG-INFO
```

### Comparing `gpt_engineer-0.2.9/LICENSE` & `gpt_engineer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/README.md` & `gpt_engineer-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-# GPT-Engineer
+# gpt-engineer
 
-[![Discord Follow](https://dcbadge.vercel.app/api/server/8tcDQ89Ej2?style=flat)](https://discord.gg/8tcDQ89Ej2)
 [![GitHub Repo stars](https://img.shields.io/github/stars/gpt-engineer-org/gpt-engineer?style=social)](https://github.com/gpt-engineer-org/gpt-engineer)
+[![Discord Follow](https://dcbadge.vercel.app/api/server/8tcDQ89Ej2?style=flat)](https://discord.gg/8tcDQ89Ej2)
+[![License](https://img.shields.io/github/license/gpt-engineer-org/gpt-engineer)](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/LICENSE)
+[![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/gpt-engineer-org/gpt-engineer)](https://github.com/gpt-engineer-org/gpt-engineer/issues)
+![GitHub Release](https://img.shields.io/github/v/release/gpt-engineer-org/gpt-engineer)
 [![Twitter Follow](https://img.shields.io/twitter/follow/antonosika?style=social)](https://twitter.com/antonosika)
 
-GPT-engineer lets you:
-- Specify a software in natural language
+gpt-engineer lets you:
+- Specify software in natural language
 - Sit back and watch as an AI writes and executes the code
 - Ask the AI to implement improvements
 
 ## Getting Started
 
 ### Install gpt-engineer
 
@@ -19,28 +22,28 @@
 
 For **development**:
 - `git clone https://github.com/gpt-engineer-org/gpt-engineer.git`
 - `cd gpt-engineer`
 - `poetry install`
 - `poetry shell` to activate the virtual environment
 
-We actively support Python 3.10 - 3.12. The last version to support python 3.8 - 3.9 was [0.2.6](https://pypi.org/project/gpt-engineer/0.2.6/).
+We actively support Python 3.10 - 3.12. The last version to support Python 3.8 - 3.9 was [0.2.6](https://pypi.org/project/gpt-engineer/0.2.6/).
 
 ### Setup API Key
 
 Choose **one** of:
 - Export env variable (you can add this to .bashrc so that you don't have to do it each time you start the terminal)
     - `export OPENAI_API_KEY=[your api key]`
 - .env file:
     - Create a copy of `.env.template` named `.env`
     - Add your OPENAI_API_KEY in .env
 - Custom model:
     - See [docs](https://gpt-engineer.readthedocs.io/en/latest/open_models.html), supports local model, azure, etc.
 
-Check the [Windows README](./WINDOWS_README.md) for windows usage.
+Check the [Windows README](./WINDOWS_README.md) for Windows usage.
 
 **Other ways to run:**
 - Use Docker ([instructions](docker/README.md))
 - Do everything in your browser:
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/gpt-engineer-org/gpt-engineer/codespaces)
 
 ### Create new code (default usage)
@@ -54,49 +57,49 @@
 - Create a file called `prompt` (no extension) inside your new folder and fill it with instructions for how you want to improve the code
 - Run `gpte <project_dir> -i` with a relative path to your folder
   - For example: `gpte projects/my-old-project -i` from the gpt-engineer directory root with your folder in `projects/`
 
 By running gpt-engineer you agree to our [terms](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/TERMS_OF_USE.md).
 
 
-## Relation to gptengineer.app
-[gptengineer.app](https://gptengineer.app/) is a commercial project for automatic generation of web-apps.
-It features a UI for non-technical users, connected to a git controlled codebase.
+## Relation to gptengineer.app (GPT Engineer)
+[gptengineer.app](https://gptengineer.app/) is a commercial project for the automatic generation of web apps.
+It features a UI for non-technical users connected to a git-controlled codebase.
 The gptengineer.app team is actively supporting the open source community.
 
 
 ## Features
 
 ### Pre Prompts
 You can specify the "identity" of the AI agent by overriding the `preprompts` folder, with your own version of the `preprompts`, using the `--use-custom-preprompts` argument.
 
 Editing the `preprompts` is how you make the agent remember things between projects.
 
 ### Vision
 
-By default, GPT Engineer expects text input via a `prompt` file. It can also accept imagine inputs for vision capable models. This can be useful for adding UX or architecture diagrams as additional context for GPT Engineer. You can do this by specifiying an image directory with the --image_directory flag and setting a vision capable model in the second cli argument.
+By default, gpt-engineer expects text input via a `prompt` file. It can also accept imagine inputs for vision-capable models. This can be useful for adding UX or architecture diagrams as additional context for GPT Engineer. You can do this by specifying an image directory with the—-image_directory flag and setting a vision-capable model in the second cli argument.
 
 E.g. `gpte projects/example-vision gpt-4-vision-preview --prompt_file prompt/text --image_directory prompt/images -i`
 
 ### Open source, local and alternative models
 
-By defaul GPT Engineer supports OpenAI Models via the OpenAI API or Azure Open AI API, and Anthropic models.
+By default, gpt-engineer supports OpenAI Models via the OpenAI API or Azure Open AI API, and Anthropic models.
 
 With a little extra set up you can also run with open source models, like WizardCoder. See the [documentation](https://gpt-engineer.readthedocs.io/en/latest/open_models.html) for example instructions.
 
 ## Mission
 
 The gpt-engineer community mission is to **maintain tools that coding agent builders can use and facilitate collaboration in the open source community**.
 
 If you are interested in contributing to this, we are interested in having you.
 
 If you want to see our broader ambitions, check out the [roadmap](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/ROADMAP.md), and join
 [discord](https://discord.gg/8tcDQ89Ej2)
 to get input on how you can [contribute](.github/CONTRIBUTING.md) to it.
 
-gpt-engineer is [governed](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/GOVERNANCE.md) by a board of long term contributors. If you contribute routinely and have an interest in shaping the future of gpt-engineer, you will be considered for the board.
+gpt-engineer is [governed](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/GOVERNANCE.md) by a board of long-term contributors. If you contribute routinely and have an interest in shaping the future of gpt-engineer, you will be considered for the board.
 
 ## Example
 
 
 
 https://github.com/gpt-engineer-org/gpt-engineer/assets/4467025/40d0a9a8-82d0-4432-9376-136df0d57c99
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/applications/cli/cli_agent.py` & `gpt_engineer-0.3.0/gpt_engineer/applications/cli/cli_agent.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/applications/cli/collect.py` & `gpt_engineer-0.3.0/gpt_engineer/applications/cli/collect.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/applications/cli/file_selector.py` & `gpt_engineer-0.3.0/gpt_engineer/applications/cli/file_selector.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/applications/cli/learning.py` & `gpt_engineer-0.3.0/gpt_engineer/applications/cli/learning.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 class Learning:
     """
     A dataclass that encapsulates the learning data collected during a GPT Engineer session.
 
     Attributes
     ----------
     prompt : str
-        The initial prompt provided to the GPT Engineer.
+        A JSON string representing the prompt provided to GPT Engineer.
     model : str
         The name of the model used during the session.
     temperature : float
         The temperature setting used for the model's responses.
     config : str
         A JSON string representing the configuration settings for the session.
     logs : str
@@ -94,15 +94,15 @@
         The user's review of the generated code.
     timestamp : str
         The UTC timestamp when the learning data was created.
     version : str
         The version of the learning data schema.
     """
 
-    prompt: Prompt
+    prompt: str
     model: str
     temperature: float
     config: str
     logs: str
     session: str
     review: Optional[Review]
     timestamp: str = field(default_factory=lambda: datetime.utcnow().isoformat())
@@ -262,15 +262,15 @@
 
     Returns
     -------
     Learning
         An instance of Learning containing all the session details and user feedback.
     """
     return Learning(
-        prompt=prompt,
+        prompt=prompt.to_json(),
         model=model,
         temperature=temperature,
         config=json.dumps(config),
         session=get_session(),
         logs=memory.to_json(),
         review=review,
     )
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/applications/cli/main.py` & `gpt_engineer-0.3.0/gpt_engineer/applications/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         - Specify a software in natural language
         - Sit back and watch as an AI writes and executes the code
         - Ask the AI to implement improvements
     """
 )
 def main(
     project_path: str = typer.Argument(".", help="path"),
-    model: str = typer.Argument("gpt-4-0125-preview", help="model id string"),
+    model: str = typer.Argument("gpt-4-turbo", help="model id string"),
     temperature: float = typer.Option(
         0.1,
         "--temperature",
         "-t",
         help="Controls randomness: lower values for more focused, deterministic outputs",
     ),
     improve_mode: bool = typer.Option(
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/__main__.py` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,26 +16,30 @@
 
 Attributes
 ----------
 __name__ : str
     The standard boilerplate for invoking the main function when the script is executed.
 """
 import importlib
+import os.path
 
 from typing import Annotated, Optional
 
 import typer
 
 from langchain.cache import SQLiteCache
 from langchain.globals import set_llm_cache
 
 from gpt_engineer.applications.cli.main import load_env_if_needed
+from gpt_engineer.benchmark.bench_config import BenchConfig
 from gpt_engineer.benchmark.benchmarks.load import get_benchmark
 from gpt_engineer.benchmark.run import print_results, run
 
+app = typer.Typer()  # creates a CLI app
+
 
 def get_agent(path):
     """
     Dynamically imports and returns the default configuration agent from the given path.
 
     Parameters
     ----------
@@ -48,58 +52,77 @@
         An instance of the imported default configuration agent.
     """
     # Dynamically import the python module at path
     agent_module = importlib.import_module(path.replace("/", ".").replace(".py", ""))
     return agent_module.default_config_agent()
 
 
+@app.command(
+    help="""
+        Run any benchmark(s) against the specified agent.
+
+        \b
+        Currently available benchmarks are: apps and mbpp
+    """
+)
 def main(
     path_to_agent: Annotated[
         str,
         typer.Argument(
             help="python file that contains a function called 'default_config_agent'"
         ),
     ],
-    benchmarks: Annotated[
-        str, typer.Argument(help="benchmark name(s) separated by ','")
-    ],
-    task_name: Annotated[
+    bench_config: Annotated[
         Optional[str], typer.Argument(help="optional task name in benchmark")
-    ] = None,
+    ] = os.path.join(os.path.dirname(__file__), "default_bench_config.toml"),
     verbose: Annotated[
         bool, typer.Option(help="print results for each task", show_default=False)
     ] = False,
 ):
     """
     The main function that runs the specified benchmarks with the given agent and outputs the results to the console.
 
     Parameters
     ----------
     path_to_agent : str
         The file path to the Python module that contains a function called 'default_config_agent'.
     benchmarks : str
         A comma-separated string of benchmark names to run.
-    task_name : Optional[str], default=None
-        An optional task name to run within the benchmark.
+    bench_config : Optional[str], default=default_bench_config.toml
+        Configuration file for choosing which benchmark problems to run. See default config for more details.
     verbose : bool, default=False
         A flag to indicate whether to print results for each task.
 
     Returns
     -------
     None
     """
     set_llm_cache(SQLiteCache(database_path=".langchain.db"))
     load_env_if_needed()
+    config = BenchConfig.from_toml(bench_config)
+    print("using config file: " + bench_config)
+    benchmarks = list()
+    for specific_config_name in vars(config):
+        specific_config = getattr(config, specific_config_name)
+        if hasattr(specific_config, "active"):
+            if specific_config.active:
+                benchmarks.append(specific_config_name)
 
-    benchmarks = benchmarks.split(",")
     for benchmark_name in benchmarks:
-        benchmark = get_benchmark(benchmark_name)
+        benchmark = get_benchmark(benchmark_name, config)
+        if len(benchmark.tasks) == 0:
+            print(
+                benchmark_name
+                + " was skipped, since no tasks are specified. Increase the number of tasks in the config file at: "
+                + bench_config
+            )
+            continue
         agent = get_agent(path_to_agent)
 
-        results = run(agent, benchmark, task_name, verbose=verbose)
+        results = run(agent, benchmark, verbose=verbose)
         print(
             f"\n--- Results for agent {path_to_agent}, benchmark: {benchmark_name} ---"
         )
         print_results(results)
         print()
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/apps/load.py` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/apps/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 """
 from pathlib import Path
 from subprocess import TimeoutExpired
 from typing import Union
 
 from datasets import Dataset, DatasetDict, load_dataset, load_from_disk
 
+from gpt_engineer.benchmark.bench_config import AppsConfig
 from gpt_engineer.benchmark.benchmarks.apps.problem import Problem
-from gpt_engineer.benchmark.benchmarks.apps.problems import PROBLEM_IDS
 from gpt_engineer.benchmark.types import Assertable, Benchmark, Task
 from gpt_engineer.core.default.disk_execution_env import DiskExecutionEnv
 from gpt_engineer.core.files_dict import FilesDict
 from gpt_engineer.core.prompt import Prompt
 
 DATASET_PATH = Path(__file__).parent / "dataset"
 MAX_N_TEST_EXAMPLES = 10
@@ -53,41 +53,43 @@
 def _get_dataset() -> Union[Dataset, DatasetDict]:
     try:
         return load_from_disk(str(DATASET_PATH))
     except FileNotFoundError:
         print("Dataset not found locally, downloading...")
 
     dataset = load_dataset("codeparrot/apps", trust_remote_code=True)
-    dataset.save_to_disk(DATASET_PATH)
+    dataset.save_to_disk(str(DATASET_PATH))
 
     return dataset
 
 
-def load_apps():
+def load_apps(config: AppsConfig) -> Benchmark:
     """
     Loads the APPS benchmark, which consists of a series coding problems.
 
     Returns
     -------
     Benchmark
         A Benchmark object containing a list of Task objects for the APPS evaluation.
     """
     dataset = _get_dataset()
     tasks = []
-
-    problems = [
-        Problem(
-            id=problem["problem_id"],
-            question=problem["question"],
-            input_output=problem["input_output"],
-            starter_code=problem["starter_code"],
-        )
-        for problem in dataset["test"]
-        if problem["problem_id"] in PROBLEM_IDS
-    ]
+    problems = list()
+    for dataset_type in ["test", "train"]:
+        problems += [
+            Problem(
+                id=problem["problem_id"],
+                question=problem["question"],
+                input_output=problem["input_output"],
+                starter_code=problem["starter_code"],
+            )
+            for index, problem in enumerate(dataset[dataset_type])
+            if (index < config.__getattribute__(dataset_type + "_end_index"))
+            and (index >= config.__getattribute__(dataset_type + "_start_index"))
+        ]
 
     for problem in problems:
         prompt = Prompt(
             problem.question
             + "\nThe program, including its inputs, should be run from the command "
             "line like 'python main \"input1 input2 etc \"', with all inputs inside "
             "the quotation marks. The program should not read inputs from stdin."
@@ -106,10 +108,10 @@
                     ).evaluate
                     for i in range(min(len(problem.outputs), MAX_N_TEST_EXAMPLES))
                 },
             )
         )
 
     return Benchmark(
-        name="APPS",
+        name="apps",
         tasks=tasks,
     )
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/apps/problem.py` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/apps/problem.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/eval_tools.py` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/eval_tools.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/EVAL_NEW_CODE_RESULTS.md` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/evals/EVAL_NEW_CODE_RESULTS.md`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/IMPROVE_CODE_RESULTS.md` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/evals/IMPROVE_CODE_RESULTS.md`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/README.md` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/evals/README.md`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/snake_game_files.txt` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/snake_game_files.txt`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/web_todo_files.txt` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/web_todo_files.txt`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/load.py` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gpteng/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 
 load_gpteng : function
     Loads the GPT-Eng benchmark, which consists of a series of tasks for evaluation.
 """
 
 from pathlib import Path
 
+from gpt_engineer.benchmark.bench_config import GptengConfig
 from gpt_engineer.benchmark.benchmarks.gpteng.eval_tools import (
     check_evaluation_component,
 )
 from gpt_engineer.benchmark.types import Assertable, Benchmark, Task
 from gpt_engineer.core.chat_to_files import chat_to_files_dict
+from gpt_engineer.core.prompt import Prompt
 
 evaluations = [
     {
         "name": "simple_code_modify",
         "project_root": "projects/snake_game_eval",
         "code_blob": "gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/snake_game_files.txt",
         "improve_code_prompt": "The grid is currently 10x10, change the grid to be 42x42.",
@@ -188,24 +190,24 @@
         prompt = case["improve_code_prompt"]
     else:
         prompt = case["code_prompt"]
 
     return Task(
         name=case["name"],
         initial_code=chat_to_files_dict(Path(case["code_blob"]).read_text()),
-        prompt=prompt,
+        prompt=Prompt(prompt),
         command=None,
         assertions={
             f"{e['type']}_{i}": expect_to_assertion(e)
             for i, e in enumerate(case["expected_results"])
         },
     )
 
 
-def load_gpteng():
+def load_gpteng(config: GptengConfig) -> Benchmark:
     """
     Loads the GPT-Eng benchmark, which consists of a series of tasks for evaluation.
 
     Returns
     -------
     Benchmark
         A Benchmark object containing a list of Task objects for the GPT-Eng evaluation.
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gptme/load.py` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/gptme/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 and assertions to benchmark the performance of AI models.
 
 Functions
 ---------
 load_gptme : function
     Loads the GPT-Me benchmark, which consists of a series of tasks for evaluation.
 """
+from gpt_engineer.benchmark.bench_config import GptmeConfig
 from gpt_engineer.benchmark.types import Benchmark, Task
 from gpt_engineer.core.files_dict import FilesDict
 from gpt_engineer.core.prompt import Prompt
 
 
-def load_gptme():
+def load_gptme(config: GptmeConfig) -> Benchmark:
     """
     Loads the GPT-Me benchmark, which consists of a series of tasks for evaluation.
 
     Returns
     -------
     Benchmark
         A Benchmark object containing a list of Task objects for the GPT-Me evaluation.
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/load.py` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/load.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,43 +5,46 @@
 It maps benchmark names to their respective loading functions.
 
 Functions
 ---------
 get_benchmark : function
     Retrieves a Benchmark object by name. Raises ValueError if the benchmark is unknown.
 """
+from gpt_engineer.benchmark.bench_config import BenchConfig
 from gpt_engineer.benchmark.benchmarks.apps.load import load_apps
 from gpt_engineer.benchmark.benchmarks.gpteng.load import load_gpteng
 from gpt_engineer.benchmark.benchmarks.gptme.load import load_gptme
 from gpt_engineer.benchmark.benchmarks.mbpp.load import load_mbpp
 from gpt_engineer.benchmark.types import Benchmark
 
 BENCHMARKS = {
     "gptme": load_gptme,
     "gpteng": load_gpteng,
     "apps": load_apps,
     "mbpp": load_mbpp,
 }
 
 
-def get_benchmark(name: str) -> Benchmark:
+def get_benchmark(name: str, config: BenchConfig) -> Benchmark:
     """
     Retrieves a Benchmark object by name. Raises ValueError if the benchmark is unknown.
 
     Parameters
     ----------
     name : str
         The name of the benchmark to retrieve.
+    config : BenchConfig
+        Configuration object for the benchmarks.
 
     Returns
     -------
     Benchmark
         The Benchmark object corresponding to the given name.
 
     Raises
     ------
     ValueError
         If the benchmark name is not found in the BENCHMARKS mapping.
     """
     if name not in BENCHMARKS:
         raise ValueError(f"Unknown benchmark {name}.")
-    return BENCHMARKS[name]()
+    return BENCHMARKS[name](config.__getattribute__(name))
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/mbpp/load.py` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/mbpp/load.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 """
 from pathlib import Path
 from subprocess import TimeoutExpired
 from typing import Union
 
 from datasets import Dataset, DatasetDict, load_dataset, load_from_disk
 
+from gpt_engineer.benchmark.bench_config import MbppConfig
 from gpt_engineer.benchmark.benchmarks.mbpp.problem import Problem
-from gpt_engineer.benchmark.benchmarks.mbpp.problems import PROBLEM_IDS
 from gpt_engineer.benchmark.types import Assertable, Benchmark, Task
 from gpt_engineer.core.default.disk_execution_env import DiskExecutionEnv
 from gpt_engineer.core.files_dict import FilesDict
 from gpt_engineer.core.prompt import Prompt
 
 DATASET_PATH = Path(__file__).parent / "dataset"
 MAX_N_TEST_EXAMPLES = 10
@@ -53,43 +53,44 @@
 def _get_dataset() -> Union[Dataset, DatasetDict]:
     try:
         return load_from_disk(str(DATASET_PATH))
     except FileNotFoundError:
         print("Dataset not found locally, downloading...")
 
     dataset = load_dataset("mbpp", "sanitized", trust_remote_code=True)
-    dataset.save_to_disk(DATASET_PATH)
+    dataset.save_to_disk(str(DATASET_PATH))
 
     return dataset
 
 
-def load_mbpp():
+def load_mbpp(config: MbppConfig) -> Benchmark:
     """
     Loads the MBPP benchmark, which consists of a series coding problems.
 
     Returns
     -------
     Benchmark
         A Benchmark object containing a list of Task objects for the MBPP evaluation.
     """
     dataset = _get_dataset()
     tasks = []
-
-    problems = [
-        Problem(
-            source_file=problem["source_file"],
-            task_id=problem["task_id"],
-            prompt=problem["prompt"],
-            code=problem["code"],
-            test_imports=problem["test_imports"],
-            test_list=problem["test_list"],
-        )
-        for problem in dataset["test"]
-        if problem["task_id"] in PROBLEM_IDS
-    ]
+    problems = []
+    for dataset_type in ["test", "train"]:
+        problems += [
+            Problem(
+                source_file=problem["source_file"],
+                task_id=problem["task_id"],
+                prompt=problem["prompt"],
+                code=problem["code"],
+                test_imports=problem["test_imports"],
+                test_list=problem["test_list"],
+            )
+            for index, problem in enumerate(dataset[dataset_type])
+            if index < config.__getattribute__(dataset_type + "_len")
+        ]
 
     for problem in problems:
         prompt = Prompt(
             problem.prompt
             + "Please extend given function without changing it's declaration including arguments."
         )
 
@@ -105,10 +106,10 @@
                     ).evaluate
                     for i, assertion in enumerate(problem.test_list)
                 },
             )
         )
 
     return Benchmark(
-        name="MBPP",
+        name="mbpp",
         tasks=tasks,
     )
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/mbpp/problem.py` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/benchmarks/mbpp/problem.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/run.py` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,38 +10,35 @@
     Runs the benchmark tasks using the provided agent and returns a list of TaskResult objects.
 
 print_results : function
     Prints the results of the benchmark tasks to the console.
 """
 import time
 
-from typing import List, Optional
+from typing import List
 
 from gpt_engineer.benchmark.types import Assertable, Benchmark, TaskResult
 from gpt_engineer.core.base_agent import BaseAgent
 from gpt_engineer.core.default.disk_execution_env import DiskExecutionEnv
 
 
 def run(
     agent: BaseAgent,
     benchmark: Benchmark,
-    task_name: Optional[str] = None,
     verbose=False,
 ) -> List[TaskResult]:
     """
     Runs the benchmark tasks using the provided agent and returns a list of TaskResult objects.
 
     Parameters
     ----------
     agent : BaseAgent
         The agent to use for running the benchmark tasks.
     benchmark : Benchmark
         The benchmark containing the tasks to run.
-    task_name : Optional[str], default=None
-        An optional name of a specific task to run within the benchmark.
     verbose : bool, default=False
         A flag to indicate whether to print verbose output during the benchmark.
 
     Returns
     -------
     List[TaskResult]
         A list of TaskResult objects representing the results of the benchmark tasks.
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/benchmark/types.py` & `gpt_engineer-0.3.0/gpt_engineer/benchmark/types.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/ai.py` & `gpt_engineer-0.3.0/gpt_engineer/core/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         Deserialize a JSON string to a list of messages.
     _create_chat_model() -> BaseChatModel
         Create a chat model with the specified model name and temperature.
     """
 
     def __init__(
         self,
-        model_name="gpt-4-0125-preview",
+        model_name="gpt-4-turbo",
         temperature=0.1,
         azure_endpoint=None,
         streaming=True,
         vision=False,
     ):
         """
         Initialize the AI class.
@@ -103,15 +103,19 @@
         temperature : float, optional
             The temperature to use for the model, by default 0.1.
         """
         self.temperature = temperature
         self.azure_endpoint = azure_endpoint
         self.model_name = model_name
         self.streaming = streaming
-        self.vision = "vision" in model_name
+        self.vision = (
+            ("vision-preview" in model_name)
+            or ("gpt-4-turbo" in model_name and "preview" not in model_name)
+            or ("claude" in model_name)
+        )
         self.llm = self._create_chat_model()
         self.token_usage_log = TokenUsageLog(model_name)
 
         logger.debug(f"Using model {self.model_name}")
 
     def start(self, system: str, user: Any, *, step_name: str) -> List[Message]:
         """
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/base_agent.py` & `gpt_engineer-0.3.0/gpt_engineer/core/base_agent.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/base_execution_env.py` & `gpt_engineer-0.3.0/gpt_engineer/core/base_execution_env.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/chat_to_files.py` & `gpt_engineer-0.3.0/gpt_engineer/core/chat_to_files.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/default/disk_execution_env.py` & `gpt_engineer-0.3.0/gpt_engineer/core/default/disk_execution_env.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/default/disk_memory.py` & `gpt_engineer-0.3.0/gpt_engineer/core/default/disk_memory.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/default/file_store.py` & `gpt_engineer-0.3.0/gpt_engineer/core/default/file_store.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/default/paths.py` & `gpt_engineer-0.3.0/gpt_engineer/core/default/paths.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/default/simple_agent.py` & `gpt_engineer-0.3.0/gpt_engineer/core/default/simple_agent.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/default/steps.py` & `gpt_engineer-0.3.0/gpt_engineer/core/default/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     Improves the code based on user input and returns the updated files.
 """
 
 import inspect
 import io
 import re
 import sys
+import traceback
 
 from pathlib import Path
 from typing import List, MutableMapping, Union
 
 from langchain.schema import HumanMessage, SystemMessage
 from termcolor import colored
 
@@ -376,16 +377,17 @@
     old_stdout = sys.stdout
     sys.stdout = Tee(sys.stdout, captured_output)
 
     try:
         files_dict = agent.improve(files_dict, prompt)
     except Exception as e:
         print(
-            f"Error while improving the project: {e}\nCould you please upload the debug_log_file.txt in {memory.path} folder to github?"
+            f"Error while improving the project: {e}\nCould you please upload the debug_log_file.txt in {memory.path} folder to github?\nFULL STACK TRACE:\n"
         )
+        traceback.print_exc(file=sys.stdout)  # Print the full stack trace
     finally:
         # Reset stdout
         sys.stdout = old_stdout
 
         # Get the captured output
         captured_string = captured_output.getvalue()
         print(captured_string)
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/diff.py` & `gpt_engineer-0.3.0/gpt_engineer/core/diff.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/files_dict.py` & `gpt_engineer-0.3.0/gpt_engineer/core/files_dict.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/git.py` & `gpt_engineer-0.3.0/gpt_engineer/core/git.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/preprompts_holder.py` & `gpt_engineer-0.3.0/gpt_engineer/core/preprompts_holder.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/project_config.py` & `gpt_engineer-0.3.0/gpt_engineer/core/project_config.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/prompt.py` & `gpt_engineer-0.3.0/gpt_engineer/core/prompt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 from typing import Dict, Optional
 
 
 class Prompt:
     def __init__(
         self,
         text: str,
@@ -26,7 +28,17 @@
                         "url": url,
                         "detail": "low",
                     },
                 }
                 content.append(image_content)
 
         return content
+
+    def to_dict(self):
+        return {
+            "text": self.text,
+            "image_urls": self.image_urls,
+            "entrypoint_prompt": self.entrypoint_prompt,
+        }
+
+    def to_json(self):
+        return json.dumps(self.to_dict())
```

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/token_usage.py` & `gpt_engineer-0.3.0/gpt_engineer/core/token_usage.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/core/version_manager.py` & `gpt_engineer-0.3.0/gpt_engineer/core/version_manager.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/preprompts/file_format_diff` & `gpt_engineer-0.3.0/gpt_engineer/preprompts/file_format_diff`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/preprompts/generate` & `gpt_engineer-0.3.0/gpt_engineer/preprompts/generate`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/preprompts/improve` & `gpt_engineer-0.3.0/gpt_engineer/preprompts/improve`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/preprompts/philosophy` & `gpt_engineer-0.3.0/gpt_engineer/preprompts/philosophy`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/tools/custom_steps.py` & `gpt_engineer-0.3.0/gpt_engineer/tools/custom_steps.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/gpt_engineer/tools/supported_languages.py` & `gpt_engineer-0.3.0/gpt_engineer/tools/supported_languages.py`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.9/pyproject.toml` & `gpt_engineer-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-engineer"
-version = "0.2.9"
+version = "0.3.0"
 description = "Specify what you want it to build, the AI asks for clarification, and then builds it."
 authors = ["Anton Osika <anton.osika@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/gpt-engineer-org/gpt-engineer"
 repository = "https://github.com/gpt-engineer-org/gpt-engineer"
 documentation = "https://gpt-engineer.readthedocs.io/en/latest/"
@@ -23,15 +23,15 @@
 termcolor = "2.3.0"
 typer = ">=0.3.2"
 rudder-sdk-python = ">=2.0.2"
 dataclasses-json = "0.5.7"
 tiktoken = ">=0.0.4"
 tabulate = "0.9.0"
 python-dotenv = ">=0.21.0"
-langchain = "^0.1"
+langchain = ">=0.1.2"
 langchain_openai = "*"
 toml = ">=0.10.2"
 tomlkit = "^0.12.4"
 pyperclip = "^1.8.2"
 langchain-anthropic = "^0.1.1"
 regex = "^2023.12.25"
 pillow = "^10.2.0"
@@ -62,15 +62,15 @@
 markdown-include = ">=0.6.0"
 sphinx_copybutton = ">=0.5.2"
 
 [tool.poetry.scripts]
 gpt-engineer = 'gpt_engineer.applications.cli.main:app'
 ge = 'gpt_engineer.applications.cli.main:app'
 gpte = 'gpt_engineer.applications.cli.main:app'
-bench = 'gpt_engineer.benchmark.__main__:main'
+bench = 'gpt_engineer.benchmark.__main__:app'
 gpte_test_application = 'tests.caching_main:app'
 
 [tool.poetry.extras]
 test = ["pytest", "pytest-cov"]
 doc = ["autodoc_pydantic", "myst_parser", "nbsphinx", "sphinx", "sphinx-autobuild", "sphinx_book_theme", "sphinx_rtd_theme", "sphinx-typlog-theme", "myst-nb", "linkchecker", "sphinx-copybutton", "markdown-include", "sphinx_copybutton"]
 
 [tool.ruff]
@@ -92,7 +92,12 @@
     "third-party",
     "first-party",
     "local-folder",
 ]
 combine-as-imports = true
 split-on-trailing-comma = false
 lines-between-types = 1
+
+[tool.pytest.ini_options]
+markers = [
+    "requires_key: marks tests as requiring access to a valid OPENAI_API_KEY (deselect with '-m \"not requires_key\"')",
+]
```

### Comparing `gpt_engineer-0.2.9/PKG-INFO` & `gpt_engineer-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-engineer
-Version: 0.2.9
+Version: 0.3.0
 Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
 Home-page: https://github.com/gpt-engineer-org/gpt-engineer
 License: MIT
 Author: Anton Osika
 Author-email: anton.osika@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: dataclasses-json (==0.5.7)
 Requires-Dist: datasets (>=2.17.1,<3.0.0)
-Requires-Dist: langchain (>=0.1,<0.2)
+Requires-Dist: langchain (>=0.1.2)
 Requires-Dist: langchain-anthropic (>=0.1.1,<0.2.0)
 Requires-Dist: langchain_openai
 Requires-Dist: openai (>=1.0,<2.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.0)
 Requires-Dist: regex (>=2023.12.25,<2024.0.0)
@@ -33,22 +33,25 @@
 Requires-Dist: toml (>=0.10.2)
 Requires-Dist: tomlkit (>=0.12.4,<0.13.0)
 Requires-Dist: typer (>=0.3.2)
 Project-URL: Documentation, https://gpt-engineer.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/gpt-engineer-org/gpt-engineer
 Description-Content-Type: text/markdown
 
-# GPT-Engineer
+# gpt-engineer
 
-[![Discord Follow](https://dcbadge.vercel.app/api/server/8tcDQ89Ej2?style=flat)](https://discord.gg/8tcDQ89Ej2)
 [![GitHub Repo stars](https://img.shields.io/github/stars/gpt-engineer-org/gpt-engineer?style=social)](https://github.com/gpt-engineer-org/gpt-engineer)
+[![Discord Follow](https://dcbadge.vercel.app/api/server/8tcDQ89Ej2?style=flat)](https://discord.gg/8tcDQ89Ej2)
+[![License](https://img.shields.io/github/license/gpt-engineer-org/gpt-engineer)](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/LICENSE)
+[![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/gpt-engineer-org/gpt-engineer)](https://github.com/gpt-engineer-org/gpt-engineer/issues)
+![GitHub Release](https://img.shields.io/github/v/release/gpt-engineer-org/gpt-engineer)
 [![Twitter Follow](https://img.shields.io/twitter/follow/antonosika?style=social)](https://twitter.com/antonosika)
 
-GPT-engineer lets you:
-- Specify a software in natural language
+gpt-engineer lets you:
+- Specify software in natural language
 - Sit back and watch as an AI writes and executes the code
 - Ask the AI to implement improvements
 
 ## Getting Started
 
 ### Install gpt-engineer
 
@@ -58,28 +61,28 @@
 
 For **development**:
 - `git clone https://github.com/gpt-engineer-org/gpt-engineer.git`
 - `cd gpt-engineer`
 - `poetry install`
 - `poetry shell` to activate the virtual environment
 
-We actively support Python 3.10 - 3.12. The last version to support python 3.8 - 3.9 was [0.2.6](https://pypi.org/project/gpt-engineer/0.2.6/).
+We actively support Python 3.10 - 3.12. The last version to support Python 3.8 - 3.9 was [0.2.6](https://pypi.org/project/gpt-engineer/0.2.6/).
 
 ### Setup API Key
 
 Choose **one** of:
 - Export env variable (you can add this to .bashrc so that you don't have to do it each time you start the terminal)
     - `export OPENAI_API_KEY=[your api key]`
 - .env file:
     - Create a copy of `.env.template` named `.env`
     - Add your OPENAI_API_KEY in .env
 - Custom model:
     - See [docs](https://gpt-engineer.readthedocs.io/en/latest/open_models.html), supports local model, azure, etc.
 
-Check the [Windows README](./WINDOWS_README.md) for windows usage.
+Check the [Windows README](./WINDOWS_README.md) for Windows usage.
 
 **Other ways to run:**
 - Use Docker ([instructions](docker/README.md))
 - Do everything in your browser:
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/gpt-engineer-org/gpt-engineer/codespaces)
 
 ### Create new code (default usage)
@@ -93,50 +96,50 @@
 - Create a file called `prompt` (no extension) inside your new folder and fill it with instructions for how you want to improve the code
 - Run `gpte <project_dir> -i` with a relative path to your folder
   - For example: `gpte projects/my-old-project -i` from the gpt-engineer directory root with your folder in `projects/`
 
 By running gpt-engineer you agree to our [terms](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/TERMS_OF_USE.md).
 
 
-## Relation to gptengineer.app
-[gptengineer.app](https://gptengineer.app/) is a commercial project for automatic generation of web-apps.
-It features a UI for non-technical users, connected to a git controlled codebase.
+## Relation to gptengineer.app (GPT Engineer)
+[gptengineer.app](https://gptengineer.app/) is a commercial project for the automatic generation of web apps.
+It features a UI for non-technical users connected to a git-controlled codebase.
 The gptengineer.app team is actively supporting the open source community.
 
 
 ## Features
 
 ### Pre Prompts
 You can specify the "identity" of the AI agent by overriding the `preprompts` folder, with your own version of the `preprompts`, using the `--use-custom-preprompts` argument.
 
 Editing the `preprompts` is how you make the agent remember things between projects.
 
 ### Vision
 
-By default, GPT Engineer expects text input via a `prompt` file. It can also accept imagine inputs for vision capable models. This can be useful for adding UX or architecture diagrams as additional context for GPT Engineer. You can do this by specifiying an image directory with the --image_directory flag and setting a vision capable model in the second cli argument.
+By default, gpt-engineer expects text input via a `prompt` file. It can also accept imagine inputs for vision-capable models. This can be useful for adding UX or architecture diagrams as additional context for GPT Engineer. You can do this by specifying an image directory with the—-image_directory flag and setting a vision-capable model in the second cli argument.
 
 E.g. `gpte projects/example-vision gpt-4-vision-preview --prompt_file prompt/text --image_directory prompt/images -i`
 
 ### Open source, local and alternative models
 
-By defaul GPT Engineer supports OpenAI Models via the OpenAI API or Azure Open AI API, and Anthropic models.
+By default, gpt-engineer supports OpenAI Models via the OpenAI API or Azure Open AI API, and Anthropic models.
 
 With a little extra set up you can also run with open source models, like WizardCoder. See the [documentation](https://gpt-engineer.readthedocs.io/en/latest/open_models.html) for example instructions.
 
 ## Mission
 
 The gpt-engineer community mission is to **maintain tools that coding agent builders can use and facilitate collaboration in the open source community**.
 
 If you are interested in contributing to this, we are interested in having you.
 
 If you want to see our broader ambitions, check out the [roadmap](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/ROADMAP.md), and join
 [discord](https://discord.gg/8tcDQ89Ej2)
 to get input on how you can [contribute](.github/CONTRIBUTING.md) to it.
 
-gpt-engineer is [governed](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/GOVERNANCE.md) by a board of long term contributors. If you contribute routinely and have an interest in shaping the future of gpt-engineer, you will be considered for the board.
+gpt-engineer is [governed](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/GOVERNANCE.md) by a board of long-term contributors. If you contribute routinely and have an interest in shaping the future of gpt-engineer, you will be considered for the board.
 
 ## Example
 
 
 
 https://github.com/gpt-engineer-org/gpt-engineer/assets/4467025/40d0a9a8-82d0-4432-9376-136df0d57c99
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

