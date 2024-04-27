# Comparing `tmp/autorag-0.1.5.tar.gz` & `tmp/autorag-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autorag-0.1.5.tar", last modified: Wed Apr 24 16:52:39 2024, max compression
+gzip compressed data, was "autorag-0.1.6.tar", last modified: Sat Apr 27 07:42:44 2024, max compression
```

## Comparing `autorag-0.1.5.tar` & `autorag-0.1.6.tar`

### file list

```diff
@@ -1,514 +1,517 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.229396 autorag-0.1.5/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.109232 autorag-0.1.5/.github/
--rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 autorag-0.1.5/.github/dependabot.yml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.109813 autorag-0.1.5/.github/workflows/
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 autorag-0.1.5/.github/workflows/sphinx.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)      927 2024-04-22 05:42:18.000000 autorag-0.1.5/.github/workflows/test.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 autorag-0.1.5/.gitignore
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.228604 autorag-0.1.5/AutoRAG.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)    24161 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)    19810 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      512 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     2936 2024-04-22 05:42:18.000000 autorag-0.1.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     6374 2024-04-22 05:42:18.000000 autorag-0.1.5/CONTRIBUTING.md
--rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 autorag-0.1.5/LICENSE
--rw-r--r--   0 jeffrey    (501) staff       (20)    24161 2024-04-24 16:52:39.229115 autorag-0.1.5/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     9161 2024-04-15 08:09:03.000000 autorag-0.1.5/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.113097 autorag-0.1.5/autorag/
--rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-24 15:34:10.000000 autorag-0.1.5/autorag/VERSION
--rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-03-27 16:56:49.000000 autorag-0.1.5/autorag/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4400 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/cli.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.113300 autorag-0.1.5/autorag/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 autorag-0.1.5/autorag/data/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.113843 autorag-0.1.5/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 autorag-0.1.5/autorag/data/corpus/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1538 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/data/corpus/langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3645 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/data/corpus/llama_index.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.115334 autorag-0.1.5/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-04-11 07:54:19.000000 autorag-0.1.5/autorag/data/qacreation/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3123 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/data/qacreation/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7473 2024-04-17 13:38:02.000000 autorag-0.1.5/autorag/data/qacreation/llama_index.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 autorag-0.1.5/autorag/data/qacreation/llama_index_default_prompt.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     2924 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/data/qacreation/ragas.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/data/qacreation/simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.115656 autorag-0.1.5/autorag/data/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/data/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1496 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/data/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 autorag-0.1.5/autorag/deploy.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.116859 autorag-0.1.5/autorag/evaluate/
--rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/evaluate/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 autorag-0.1.5/autorag/evaluate/generation.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.118028 autorag-0.1.5/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 autorag-0.1.5/autorag/evaluate/metric/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.119256 autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)    12720 2024-04-19 08:38:15.000000 autorag-0.1.5/autorag/evaluate/metric/generation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1477 2024-02-23 18:16:58.000000 autorag-0.1.5/autorag/evaluate/metric/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2131 2024-02-23 18:16:58.000000 autorag-0.1.5/autorag/evaluate/metric/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/evaluate/metric/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/evaluate/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/evaluate/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 autorag-0.1.5/autorag/evaluate/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    17273 2024-04-12 13:21:55.000000 autorag-0.1.5/autorag/evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/node_line.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.119411 autorag-0.1.5/autorag/nodes/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.120387 autorag-0.1.5/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 autorag-0.1.5/autorag/nodes/generator/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 autorag-0.1.5/autorag/nodes/generator/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 autorag-0.1.5/autorag/nodes/generator/llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 autorag-0.1.5/autorag/nodes/generator/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 autorag-0.1.5/autorag/nodes/generator/vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.121567 autorag-0.1.5/autorag/nodes/passageaugmenter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      112 2024-04-24 15:33:34.000000 autorag-0.1.5/autorag/nodes/passageaugmenter/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4688 2024-04-24 15:33:34.000000 autorag-0.1.5/autorag/nodes/passageaugmenter/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      388 2024-04-24 15:33:34.000000 autorag-0.1.5/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/nodes/passageaugmenter/prev_next_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3387 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/nodes/passageaugmenter/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.123015 autorag-0.1.5/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)      115 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/nodes/passagecompressor/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2445 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/nodes/passagecompressor/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 autorag-0.1.5/autorag/nodes/passagecompressor/pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2857 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/nodes/passagecompressor/refine.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 autorag-0.1.5/autorag/nodes/passagecompressor/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 autorag-0.1.5/autorag/nodes/passagecompressor/tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.124582 autorag-0.1.5/autorag/nodes/passagefilter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      207 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/nodes/passagefilter/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2242 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/nodes/passagefilter/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      417 2024-04-11 14:32:56.000000 autorag-0.1.5/autorag/nodes/passagefilter/pass_passage_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3922 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/nodes/passagefilter/percentile_cutoff.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2399 2024-04-24 16:50:09.000000 autorag-0.1.5/autorag/nodes/passagefilter/recency.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3951 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/nodes/passagefilter/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4022 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/nodes/passagefilter/threshold_cutoff.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.128761 autorag-0.1.5/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      504 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/nodes/passagereranker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/nodes/passagereranker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 autorag-0.1.5/autorag/nodes/passagereranker/cohere.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3625 2024-04-24 15:33:34.000000 autorag-0.1.5/autorag/nodes/passagereranker/colbert.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2722 2024-04-24 07:39:51.000000 autorag-0.1.5/autorag/nodes/passagereranker/flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2397 2024-04-24 07:39:51.000000 autorag-0.1.5/autorag/nodes/passagereranker/flag_embedding_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 autorag-0.1.5/autorag/nodes/passagereranker/jina.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 autorag-0.1.5/autorag/nodes/passagereranker/koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5697 2024-04-19 15:05:28.000000 autorag-0.1.5/autorag/nodes/passagereranker/monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-04-10 15:52:33.000000 autorag-0.1.5/autorag/nodes/passagereranker/pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 autorag-0.1.5/autorag/nodes/passagereranker/rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4167 2024-04-10 13:46:46.000000 autorag-0.1.5/autorag/nodes/passagereranker/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2884 2024-04-19 08:38:15.000000 autorag-0.1.5/autorag/nodes/passagereranker/sentence_transformer.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.129544 autorag-0.1.5/autorag/nodes/passagereranker/tart/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/passagereranker/tart/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3832 2024-04-23 11:22:32.000000 autorag-0.1.5/autorag/nodes/passagereranker/tart/tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/nodes/passagereranker/time_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-03-06 19:44:35.000000 autorag-0.1.5/autorag/nodes/passagereranker/upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.130803 autorag-0.1.5/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 autorag-0.1.5/autorag/nodes/promptmaker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 autorag-0.1.5/autorag/nodes/promptmaker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/promptmaker/fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 autorag-0.1.5/autorag/nodes/promptmaker/long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 autorag-0.1.5/autorag/nodes/promptmaker/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.132248 autorag-0.1.5/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 autorag-0.1.5/autorag/nodes/queryexpansion/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 autorag-0.1.5/autorag/nodes/queryexpansion/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 autorag-0.1.5/autorag/nodes/queryexpansion/hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 autorag-0.1.5/autorag/nodes/queryexpansion/pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 autorag-0.1.5/autorag/nodes/queryexpansion/query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 autorag-0.1.5/autorag/nodes/queryexpansion/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.134794 autorag-0.1.5/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      227 2024-04-11 14:29:33.000000 autorag-0.1.5/autorag/nodes/retrieval/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6444 2024-04-11 14:29:33.000000 autorag-0.1.5/autorag/nodes/retrieval/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 autorag-0.1.5/autorag/nodes/retrieval/bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/retrieval/hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3221 2024-04-11 14:29:33.000000 autorag-0.1.5/autorag/nodes/retrieval/hybrid_dbsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 autorag-0.1.5/autorag/nodes/retrieval/hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4148 2024-04-11 14:29:33.000000 autorag-0.1.5/autorag/nodes/retrieval/hybrid_rsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    10780 2024-04-11 14:29:33.000000 autorag-0.1.5/autorag/nodes/retrieval/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4651 2024-03-25 07:44:05.000000 autorag-0.1.5/autorag/nodes/retrieval/vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.135655 autorag-0.1.5/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/schema/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/schema/module.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/schema/node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4202 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/support.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.136515 autorag-0.1.5/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)      177 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3314 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/utils/preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    11592 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 autorag-0.1.5/autorag/web.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       73 2024-04-19 08:38:15.000000 autorag-0.1.5/dev_requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.137354 autorag-0.1.5/docs/
--rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 autorag-0.1.5/docs/Makefile
--rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 autorag-0.1.5/docs/make.bat
--rw-r--r--   0 jeffrey    (501) staff       (20)      125 2024-04-19 08:38:15.000000 autorag-0.1.5/docs/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.138956 autorag-0.1.5/docs/source/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.146987 autorag-0.1.5/docs/source/_static/
--rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/data_creation.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/data_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/node_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/node_line_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/node_line_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/node_lines.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/node_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 autorag-0.1.5/docs/source/_static/project_folder_example.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/project_folders.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/resources_folder.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.150528 autorag-0.1.5/docs/source/_static/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/RAG_paradigms.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/advanced_RAG.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/cycle.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/merger.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/node_line_modular.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/policy.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 autorag-0.1.5/docs/source/_static/samsung_sundae.jpeg
--rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/trial_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/trial_json.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/trial_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 autorag-0.1.5/docs/source/_static/web_interface.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.155380 autorag-0.1.5/docs/source/api_spec/
--rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 autorag-0.1.5/docs/source/api_spec/autorag.data.corpus.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      939 2024-04-14 04:49:44.000000 autorag-0.1.5/docs/source/api_spec/autorag.data.qacreation.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 autorag-0.1.5/docs/source/api_spec/autorag.data.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 autorag-0.1.5/docs/source/api_spec/autorag.data.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 autorag-0.1.5/docs/source/api_spec/autorag.evaluate.metric.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 autorag-0.1.5/docs/source/api_spec/autorag.evaluate.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.generator.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      864 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1294 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagecompressor.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1471 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagefilter.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     3434 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagereranker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.promptmaker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.queryexpansion.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1896 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.retrieval.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      466 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 autorag-0.1.5/docs/source/api_spec/autorag.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 autorag-0.1.5/docs/source/api_spec/autorag.schema.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 autorag-0.1.5/docs/source/api_spec/autorag.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 autorag-0.1.5/docs/source/api_spec/modules.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1454 2024-04-19 08:38:15.000000 autorag-0.1.5/docs/source/conf.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.156438 autorag-0.1.5/docs/source/data_creation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 autorag-0.1.5/docs/source/data_creation/data_format.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2206 2024-04-12 13:21:50.000000 autorag-0.1.5/docs/source/data_creation/ragas.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 autorag-0.1.5/docs/source/data_creation/tutorial.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.156995 autorag-0.1.5/docs/source/deploy/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/deploy/api_endpoint.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 autorag-0.1.5/docs/source/deploy/web.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4124 2024-04-12 13:21:50.000000 autorag-0.1.5/docs/source/index.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 autorag-0.1.5/docs/source/install.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     6153 2024-04-12 13:21:50.000000 autorag-0.1.5/docs/source/local_model.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.157210 autorag-0.1.5/docs/source/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.157845 autorag-0.1.5/docs/source/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 autorag-0.1.5/docs/source/nodes/generator/generator.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/generator/llama_index_llm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 autorag-0.1.5/docs/source/nodes/generator/vllm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      172 2024-04-11 14:29:33.000000 autorag-0.1.5/docs/source/nodes/index.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.158205 autorag-0.1.5/docs/source/nodes/passage_augmenter/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1591 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/nodes/passage_augmenter/passage_augmenter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      727 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.158750 autorag-0.1.5/docs/source/nodes/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3046 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/nodes/passage_compressor/passage_compressor.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1182 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/nodes/passage_compressor/refine.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/passage_compressor/tree_summarize.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.159879 autorag-0.1.5/docs/source/nodes/passage_filter/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1765 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/nodes/passage_filter/passage_filter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1127 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/nodes/passage_filter/recency_filter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1028 2024-04-12 13:21:50.000000 autorag-0.1.5/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1085 2024-04-10 13:46:46.000000 autorag-0.1.5/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.162697 autorag-0.1.5/docs/source/nodes/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/cohere.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/colbert.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      675 2024-04-11 14:29:33.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      654 2024-04-11 14:29:33.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/jina_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/koreranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/monot5.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2372 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/passage_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/rankgpt.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/tart.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      561 2024-04-12 13:21:50.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/time_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1435 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/upr.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.163486 autorag-0.1.5/docs/source/nodes/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/prompt_maker/fstring.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 autorag-0.1.5/docs/source/nodes/prompt_maker/long_context_reorder.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 autorag-0.1.5/docs/source/nodes/prompt_maker/prompt_maker.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.164037 autorag-0.1.5/docs/source/nodes/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/query_expansion/hyde.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/query_expansion/query_decompose.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 autorag-0.1.5/docs/source/nodes/query_expansion/query_expansion.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.165410 autorag-0.1.5/docs/source/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/retrieval/bm25.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-10 06:33:52.000000 autorag-0.1.5/docs/source/nodes/retrieval/hybrid_cc.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2294 2024-04-11 14:29:33.000000 autorag-0.1.5/docs/source/nodes/retrieval/hybrid_dbsf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2053 2024-04-10 06:33:52.000000 autorag-0.1.5/docs/source/nodes/retrieval/hybrid_rrf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2304 2024-04-10 06:33:52.000000 autorag-0.1.5/docs/source/nodes/retrieval/hybrid_rsf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1910 2024-04-11 14:29:33.000000 autorag-0.1.5/docs/source/nodes/retrieval/retrieval.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/retrieval/vectordb.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.166363 autorag-0.1.5/docs/source/optimization/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 autorag-0.1.5/docs/source/optimization/custom_config.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/optimization/folder_structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 autorag-0.1.5/docs/source/optimization/optimization.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/optimization/sample_full_config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.166578 autorag-0.1.5/docs/source/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/roadmap/modular_rag.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 autorag-0.1.5/docs/source/troubleshooting.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 autorag-0.1.5/docs/source/tutorial.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-02-18 20:58:37.000000 autorag-0.1.5/pyproject.toml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1149 2024-04-12 13:21:50.000000 autorag-0.1.5/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.168158 autorag-0.1.5/sample_config/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 autorag-0.1.5/sample_config/compact_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 autorag-0.1.5/sample_config/compact_openai.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 autorag-0.1.5/sample_config/config_korean.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 autorag-0.1.5/sample_config/extracted_sample.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     4769 2024-04-23 11:20:05.000000 autorag-0.1.5/sample_config/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 autorag-0.1.5/sample_config/simple_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 autorag-0.1.5/sample_config/simple_openai.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.168353 autorag-0.1.5/sample_dataset/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 autorag-0.1.5/sample_dataset/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.168592 autorag-0.1.5/sample_dataset/eli5/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 autorag-0.1.5/sample_dataset/eli5/load_eli5_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.168768 autorag-0.1.5/sample_dataset/msmarco/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 autorag-0.1.5/sample_dataset/msmarco/load_msmarco_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.169050 autorag-0.1.5/sample_dataset/triviaqa/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 autorag-0.1.5/sample_dataset/triviaqa/load_triviaqa_dataset.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-24 16:52:39.229444 autorag-0.1.5/setup.cfg
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.169871 autorag-0.1.5/tests/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.171394 autorag-0.1.5/tests/autorag/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.103562 autorag-0.1.5/tests/autorag/data/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.172491 autorag-0.1.5/tests/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 autorag-0.1.5/tests/autorag/data/corpus/test_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      646 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/autorag/data/corpus/test_langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1317 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/autorag/data/corpus/test_llama_index_corpus.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.173594 autorag-0.1.5/tests/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/data/qacreation/test_base_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3129 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/data/qacreation/test_llama_index_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      897 2024-04-12 13:21:50.000000 autorag-0.1.5/tests/autorag/data/qacreation/test_ragas_qa_creation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2097 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/data/qacreation/test_simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.174416 autorag-0.1.5/tests/autorag/evaluate/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.175060 autorag-0.1.5/tests/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 autorag-0.1.5/tests/autorag/evaluate/metric/test_generation_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1578 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1569 2024-04-10 13:46:46.000000 autorag-0.1.5/tests/autorag/evaluate/metric/test_retrieval_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 autorag-0.1.5/tests/autorag/evaluate/test_evaluate_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4701 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/evaluate/test_generation_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/evaluate/test_retrieval_evaluate.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.104392 autorag-0.1.5/tests/autorag/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.176256 autorag-0.1.5/tests/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 autorag-0.1.5/tests/autorag/nodes/generator/test_generator_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 autorag-0.1.5/tests/autorag/nodes/generator/test_llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 autorag-0.1.5/tests/autorag/nodes/generator/test_run_generator_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 autorag-0.1.5/tests/autorag/nodes/generator/test_vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.177237 autorag-0.1.5/tests/autorag/nodes/passageaugmenter/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1159 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      751 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2594 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3080 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.178536 autorag-0.1.5/tests/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-04-15 08:09:03.000000 autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1852 2024-04-15 08:09:03.000000 autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_refine.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5091 2024-02-22 16:01:50.000000 autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1933 2024-04-15 08:09:03.000000 autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.180550 autorag-0.1.5/tests/autorag/nodes/passagefilter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      710 2024-04-11 14:32:56.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3615 2024-04-15 08:09:03.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2999 2024-04-10 13:46:46.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      981 2024-04-12 13:21:50.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4380 2024-04-24 16:50:09.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_recency_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      860 2024-04-10 13:46:46.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.184156 autorag-0.1.5/tests/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1160 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1105 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1994 2024-04-24 07:39:51.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2213 2024-04-24 07:39:51.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1881 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_jina_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1407 2024-04-23 11:22:32.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4364 2024-04-12 13:21:50.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2230 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1604 2024-04-23 11:22:32.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1371 2024-04-23 11:22:32.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1210 2024-04-12 13:21:50.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_time_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      956 2024-02-18 20:58:37.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.185071 autorag-0.1.5/tests/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 autorag-0.1.5/tests/autorag/nodes/promptmaker/test_fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 autorag-0.1.5/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 autorag-0.1.5/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8310 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.186362 autorag-0.1.5/tests/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.188935 autorag-0.1.5/tests/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4013 2024-04-11 14:29:33.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1525 2024-04-11 14:29:33.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      879 2024-04-11 14:29:33.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2989 2024-04-10 06:33:52.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      780 2024-04-11 14:29:33.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_retrieval_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3757 2024-03-25 07:44:05.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.189404 autorag-0.1.5/tests/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/schema/test_module_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/schema/test_node_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 autorag-0.1.5/tests/autorag/test_cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6869 2024-04-10 13:46:46.000000 autorag-0.1.5/tests/autorag/test_deploy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    14669 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/test_evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/test_strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/test_support.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 autorag-0.1.5/tests/autorag/test_web.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.189880 autorag-0.1.5/tests/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2788 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/autorag/utils/test_preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     9696 2024-04-12 13:21:50.000000 autorag-0.1.5/tests/autorag/utils/test_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 autorag-0.1.5/tests/conftest.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 autorag-0.1.5/tests/delete_tests.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 autorag-0.1.5/tests/mock.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.192654 autorag-0.1.5/tests/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 autorag-0.1.5/tests/resources/README.md
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.5/tests/resources/corpus_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.104743 autorag-0.1.5/tests/resources/data_creation/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.194028 autorag-0.1.5/tests/resources/data_creation/raw_dir/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 autorag-0.1.5/tests/resources/data_creation/raw_dir/sample1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 autorag-0.1.5/tests/resources/data_creation/raw_dir/sample2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 autorag-0.1.5/tests/resources/data_creation/raw_dir/sample3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-04-12 16:43:24.000000 autorag-0.1.5/tests/resources/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.5/tests/resources/qa_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.194786 autorag-0.1.5/tests/resources/qa_gen_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-04-17 01:53:11.000000 autorag-0.1.5/tests/resources/qa_gen_prompts/prompt1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 autorag-0.1.5/tests/resources/qa_gen_prompts/prompt2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 autorag-0.1.5/tests/resources/qa_gen_prompts/prompt3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 autorag-0.1.5/tests/resources/qa_test_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.195398 autorag-0.1.5/tests/resources/result_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.195865 autorag-0.1.5/tests/resources/result_project/0/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.196074 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.198778 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.199769 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.200011 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.201350 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.201500 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.202401 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.203909 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.205377 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 autorag-0.1.5/tests/resources/result_project/0/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.205623 autorag-0.1.5/tests/resources/result_project/1/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.205897 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.208020 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.106328 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.208168 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.209169 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.210786 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.211077 autorag-0.1.5/tests/resources/result_project/2/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.106523 autorag-0.1.5/tests/resources/result_project/2/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.211273 autorag-0.1.5/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.211870 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.213603 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.213749 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.214427 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.216199 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.217974 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.218190 autorag-0.1.5/tests/resources/result_project/3/
--rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/3/config.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 autorag-0.1.5/tests/resources/result_project/best.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.219120 autorag-0.1.5/tests/resources/result_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.219375 autorag-0.1.5/tests/resources/result_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/resources/bm25.pkl
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.219631 autorag-0.1.5/tests/resources/result_project/resources/chroma/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.226159 autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
--rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 autorag-0.1.5/tests/resources/result_project/resources/chroma/chroma.sqlite3
--rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/trial.json
--rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 autorag-0.1.5/tests/resources/sample_contents_nqa.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.107437 autorag-0.1.5/tests/resources/sample_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.227275 autorag-0.1.5/tests/resources/sample_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   115302 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/resources/sample_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.5/tests/resources/sample_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.227775 autorag-0.1.5/tests/resources/sample_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 autorag-0.1.5/tests/resources/sample_project/resources/bm25.pkl
--rw-r--r--   0 jeffrey    (501) staff       (20)      893 2024-04-10 13:46:46.000000 autorag-0.1.5/tests/resources/simple.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 autorag-0.1.5/tests/resources/test_bm25_retrieval.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.145281 autorag-0.1.6/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.880763 autorag-0.1.6/.github/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 autorag-0.1.6/.github/dependabot.yml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.881645 autorag-0.1.6/.github/workflows/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1486 2024-04-27 07:08:56.000000 autorag-0.1.6/.github/workflows/publish.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 autorag-0.1.6/.github/workflows/sphinx.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      927 2024-04-27 01:36:13.000000 autorag-0.1.6/.github/workflows/test.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 autorag-0.1.6/.gitignore
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.144420 autorag-0.1.6/AutoRAG.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    24168 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)    19936 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      519 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2936 2024-04-27 01:36:13.000000 autorag-0.1.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6374 2024-04-27 01:36:13.000000 autorag-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 autorag-0.1.6/LICENSE
+-rw-r--r--   0 jeffrey    (501) staff       (20)    24168 2024-04-27 07:42:44.144996 autorag-0.1.6/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9161 2024-04-15 08:09:03.000000 autorag-0.1.6/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.884851 autorag-0.1.6/autorag/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/VERSION
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-03-27 16:56:49.000000 autorag-0.1.6/autorag/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4400 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/cli.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.885204 autorag-0.1.6/autorag/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 autorag-0.1.6/autorag/data/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.885881 autorag-0.1.6/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 autorag-0.1.6/autorag/data/corpus/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1538 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/data/corpus/langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3645 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/data/corpus/llama_index.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.887636 autorag-0.1.6/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-04-11 07:54:19.000000 autorag-0.1.6/autorag/data/qacreation/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3123 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/data/qacreation/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7473 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/data/qacreation/llama_index.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 autorag-0.1.6/autorag/data/qacreation/llama_index_default_prompt.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2924 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/data/qacreation/ragas.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/data/qacreation/simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.888022 autorag-0.1.6/autorag/data/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/data/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1496 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/data/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 autorag-0.1.6/autorag/deploy.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.889442 autorag-0.1.6/autorag/evaluate/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/evaluate/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 autorag-0.1.6/autorag/evaluate/generation.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.890933 autorag-0.1.6/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 autorag-0.1.6/autorag/evaluate/metric/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.893597 autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)    12720 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/evaluate/metric/generation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1671 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/evaluate/metric/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2310 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/evaluate/metric/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/evaluate/metric/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/evaluate/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/evaluate/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 autorag-0.1.6/autorag/evaluate/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    17379 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/node_line.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.893887 autorag-0.1.6/autorag/nodes/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.895035 autorag-0.1.6/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 autorag-0.1.6/autorag/nodes/generator/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 autorag-0.1.6/autorag/nodes/generator/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 autorag-0.1.6/autorag/nodes/generator/llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 autorag-0.1.6/autorag/nodes/generator/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 autorag-0.1.6/autorag/nodes/generator/vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.896087 autorag-0.1.6/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      112 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passageaugmenter/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4688 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passageaugmenter/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      388 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passageaugmenter/prev_next_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3555 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passageaugmenter/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.898797 autorag-0.1.6/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      115 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/nodes/passagecompressor/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2445 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/nodes/passagecompressor/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 autorag-0.1.6/autorag/nodes/passagecompressor/pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2857 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/nodes/passagecompressor/refine.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 autorag-0.1.6/autorag/nodes/passagecompressor/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 autorag-0.1.6/autorag/nodes/passagecompressor/tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.900483 autorag-0.1.6/autorag/nodes/passagefilter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      207 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/nodes/passagefilter/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2242 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/nodes/passagefilter/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      417 2024-04-11 14:32:56.000000 autorag-0.1.6/autorag/nodes/passagefilter/pass_passage_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3922 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/nodes/passagefilter/percentile_cutoff.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2399 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagefilter/recency.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4119 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagefilter/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4022 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/nodes/passagefilter/threshold_cutoff.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.905128 autorag-0.1.6/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      504 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/nodes/passagereranker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/nodes/passagereranker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 autorag-0.1.6/autorag/nodes/passagereranker/cohere.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5376 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/nodes/passagereranker/colbert.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2722 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2397 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/flag_embedding_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 autorag-0.1.6/autorag/nodes/passagereranker/jina.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 autorag-0.1.6/autorag/nodes/passagereranker/koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5697 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-04-10 15:52:33.000000 autorag-0.1.6/autorag/nodes/passagereranker/pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 autorag-0.1.6/autorag/nodes/passagereranker/rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4335 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2884 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/sentence_transformer.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.905919 autorag-0.1.6/autorag/nodes/passagereranker/tart/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/passagereranker/tart/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3832 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/tart/tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5371 2024-04-27 02:56:02.000000 autorag-0.1.6/autorag/nodes/passagereranker/temp_new_colbert.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-04-27 01:40:21.000000 autorag-0.1.6/autorag/nodes/passagereranker/temp_old_upr.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/nodes/passagereranker/time_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/nodes/passagereranker/upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.907317 autorag-0.1.6/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 autorag-0.1.6/autorag/nodes/promptmaker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 autorag-0.1.6/autorag/nodes/promptmaker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/promptmaker/fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 autorag-0.1.6/autorag/nodes/promptmaker/long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 autorag-0.1.6/autorag/nodes/promptmaker/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.908988 autorag-0.1.6/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 autorag-0.1.6/autorag/nodes/queryexpansion/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 autorag-0.1.6/autorag/nodes/queryexpansion/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 autorag-0.1.6/autorag/nodes/queryexpansion/hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 autorag-0.1.6/autorag/nodes/queryexpansion/pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 autorag-0.1.6/autorag/nodes/queryexpansion/query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 autorag-0.1.6/autorag/nodes/queryexpansion/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.911868 autorag-0.1.6/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      227 2024-04-11 14:29:33.000000 autorag-0.1.6/autorag/nodes/retrieval/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6444 2024-04-11 14:29:33.000000 autorag-0.1.6/autorag/nodes/retrieval/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 autorag-0.1.6/autorag/nodes/retrieval/bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/retrieval/hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3221 2024-04-11 14:29:33.000000 autorag-0.1.6/autorag/nodes/retrieval/hybrid_dbsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 autorag-0.1.6/autorag/nodes/retrieval/hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4148 2024-04-11 14:29:33.000000 autorag-0.1.6/autorag/nodes/retrieval/hybrid_rsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    10949 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/retrieval/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4907 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/retrieval/vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.912599 autorag-0.1.6/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/schema/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/schema/module.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/schema/node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4202 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/support.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.913384 autorag-0.1.6/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      237 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4020 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/utils/preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    12038 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 autorag-0.1.6/autorag/web.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       73 2024-04-27 01:36:13.000000 autorag-0.1.6/dev_requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.914188 autorag-0.1.6/docs/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 autorag-0.1.6/docs/Makefile
+-rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 autorag-0.1.6/docs/make.bat
+-rw-r--r--   0 jeffrey    (501) staff       (20)      125 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.916159 autorag-0.1.6/docs/source/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.922714 autorag-0.1.6/docs/source/_static/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/data_creation.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/data_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/node_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/node_line_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/node_line_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/node_lines.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/node_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 autorag-0.1.6/docs/source/_static/project_folder_example.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/project_folders.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/resources_folder.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.927026 autorag-0.1.6/docs/source/_static/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/RAG_paradigms.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/advanced_RAG.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/cycle.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/merger.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/node_line_modular.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/policy.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 autorag-0.1.6/docs/source/_static/samsung_sundae.jpeg
+-rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/trial_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/trial_json.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/trial_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 autorag-0.1.6/docs/source/_static/web_interface.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.934553 autorag-0.1.6/docs/source/api_spec/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 autorag-0.1.6/docs/source/api_spec/autorag.data.corpus.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      939 2024-04-14 04:49:44.000000 autorag-0.1.6/docs/source/api_spec/autorag.data.qacreation.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 autorag-0.1.6/docs/source/api_spec/autorag.data.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 autorag-0.1.6/docs/source/api_spec/autorag.data.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 autorag-0.1.6/docs/source/api_spec/autorag.evaluate.metric.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 autorag-0.1.6/docs/source/api_spec/autorag.evaluate.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.generator.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      864 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1294 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagecompressor.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1471 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagefilter.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3434 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagereranker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.promptmaker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.queryexpansion.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1896 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.retrieval.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      466 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 autorag-0.1.6/docs/source/api_spec/autorag.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 autorag-0.1.6/docs/source/api_spec/autorag.schema.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 autorag-0.1.6/docs/source/api_spec/autorag.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 autorag-0.1.6/docs/source/api_spec/modules.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1454 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/conf.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.935406 autorag-0.1.6/docs/source/data_creation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 autorag-0.1.6/docs/source/data_creation/data_format.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2206 2024-04-12 13:21:50.000000 autorag-0.1.6/docs/source/data_creation/ragas.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 autorag-0.1.6/docs/source/data_creation/tutorial.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.935908 autorag-0.1.6/docs/source/deploy/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/deploy/api_endpoint.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 autorag-0.1.6/docs/source/deploy/web.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4124 2024-04-12 13:21:50.000000 autorag-0.1.6/docs/source/index.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 autorag-0.1.6/docs/source/install.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6153 2024-04-12 13:21:50.000000 autorag-0.1.6/docs/source/local_model.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.936241 autorag-0.1.6/docs/source/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.936941 autorag-0.1.6/docs/source/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 autorag-0.1.6/docs/source/nodes/generator/generator.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/generator/llama_index_llm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 autorag-0.1.6/docs/source/nodes/generator/vllm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      172 2024-04-11 14:29:33.000000 autorag-0.1.6/docs/source/nodes/index.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.937410 autorag-0.1.6/docs/source/nodes/passage_augmenter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1591 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/nodes/passage_augmenter/passage_augmenter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      727 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.938562 autorag-0.1.6/docs/source/nodes/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3046 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/nodes/passage_compressor/passage_compressor.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1182 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/nodes/passage_compressor/refine.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/passage_compressor/tree_summarize.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.939786 autorag-0.1.6/docs/source/nodes/passage_filter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1765 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/nodes/passage_filter/passage_filter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1127 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/nodes/passage_filter/recency_filter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1028 2024-04-12 13:21:50.000000 autorag-0.1.6/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1085 2024-04-10 13:46:46.000000 autorag-0.1.6/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.945094 autorag-0.1.6/docs/source/nodes/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/cohere.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/colbert.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      675 2024-04-11 14:29:33.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      654 2024-04-11 14:29:33.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/jina_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/koreranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/monot5.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2372 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/passage_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/rankgpt.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/tart.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      561 2024-04-12 13:21:50.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/time_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1435 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/upr.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.946003 autorag-0.1.6/docs/source/nodes/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/prompt_maker/fstring.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 autorag-0.1.6/docs/source/nodes/prompt_maker/long_context_reorder.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 autorag-0.1.6/docs/source/nodes/prompt_maker/prompt_maker.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.946535 autorag-0.1.6/docs/source/nodes/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/query_expansion/hyde.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/query_expansion/query_decompose.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 autorag-0.1.6/docs/source/nodes/query_expansion/query_expansion.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.948424 autorag-0.1.6/docs/source/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/retrieval/bm25.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-10 06:33:52.000000 autorag-0.1.6/docs/source/nodes/retrieval/hybrid_cc.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2294 2024-04-11 14:29:33.000000 autorag-0.1.6/docs/source/nodes/retrieval/hybrid_dbsf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2053 2024-04-10 06:33:52.000000 autorag-0.1.6/docs/source/nodes/retrieval/hybrid_rrf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2304 2024-04-10 06:33:52.000000 autorag-0.1.6/docs/source/nodes/retrieval/hybrid_rsf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1910 2024-04-11 14:29:33.000000 autorag-0.1.6/docs/source/nodes/retrieval/retrieval.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/retrieval/vectordb.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.949443 autorag-0.1.6/docs/source/optimization/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 autorag-0.1.6/docs/source/optimization/custom_config.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/optimization/folder_structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 autorag-0.1.6/docs/source/optimization/optimization.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/optimization/sample_full_config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.949655 autorag-0.1.6/docs/source/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/roadmap/modular_rag.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 autorag-0.1.6/docs/source/troubleshooting.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 autorag-0.1.6/docs/source/tutorial.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-04-26 05:39:23.000000 autorag-0.1.6/pyproject.toml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1156 2024-04-27 01:36:13.000000 autorag-0.1.6/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.951739 autorag-0.1.6/sample_config/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 autorag-0.1.6/sample_config/compact_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 autorag-0.1.6/sample_config/compact_openai.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 autorag-0.1.6/sample_config/config_korean.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 autorag-0.1.6/sample_config/extracted_sample.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4769 2024-04-27 01:36:13.000000 autorag-0.1.6/sample_config/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 autorag-0.1.6/sample_config/simple_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 autorag-0.1.6/sample_config/simple_openai.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.951958 autorag-0.1.6/sample_dataset/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 autorag-0.1.6/sample_dataset/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.952387 autorag-0.1.6/sample_dataset/eli5/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 autorag-0.1.6/sample_dataset/eli5/load_eli5_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.952667 autorag-0.1.6/sample_dataset/msmarco/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 autorag-0.1.6/sample_dataset/msmarco/load_msmarco_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.952980 autorag-0.1.6/sample_dataset/triviaqa/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 autorag-0.1.6/sample_dataset/triviaqa/load_triviaqa_dataset.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-27 07:42:44.145331 autorag-0.1.6/setup.cfg
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.954226 autorag-0.1.6/tests/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.955873 autorag-0.1.6/tests/autorag/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.875777 autorag-0.1.6/tests/autorag/data/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.956785 autorag-0.1.6/tests/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 autorag-0.1.6/tests/autorag/data/corpus/test_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      646 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/data/corpus/test_langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1317 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/data/corpus/test_llama_index_corpus.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.958163 autorag-0.1.6/tests/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/data/qacreation/test_base_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3129 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/data/qacreation/test_llama_index_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      897 2024-04-12 13:21:50.000000 autorag-0.1.6/tests/autorag/data/qacreation/test_ragas_qa_creation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2097 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/data/qacreation/test_simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.959217 autorag-0.1.6/tests/autorag/evaluate/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.959937 autorag-0.1.6/tests/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 autorag-0.1.6/tests/autorag/evaluate/metric/test_generation_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1731 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1634 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/evaluate/metric/test_retrieval_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 autorag-0.1.6/tests/autorag/evaluate/test_evaluate_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4701 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/evaluate/test_generation_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/evaluate/test_retrieval_evaluate.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.876452 autorag-0.1.6/tests/autorag/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.961058 autorag-0.1.6/tests/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 autorag-0.1.6/tests/autorag/nodes/generator/test_generator_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 autorag-0.1.6/tests/autorag/nodes/generator/test_llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 autorag-0.1.6/tests/autorag/nodes/generator/test_run_generator_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 autorag-0.1.6/tests/autorag/nodes/generator/test_vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.961918 autorag-0.1.6/tests/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1159 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      751 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2594 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3080 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.963308 autorag-0.1.6/tests/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-04-15 08:09:03.000000 autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1852 2024-04-15 08:09:03.000000 autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_refine.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5073 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1933 2024-04-15 08:09:03.000000 autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.965582 autorag-0.1.6/tests/autorag/nodes/passagefilter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      710 2024-04-11 14:32:56.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3615 2024-04-15 08:09:03.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2999 2024-04-10 13:46:46.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      981 2024-04-12 13:21:50.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4380 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_recency_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      860 2024-04-10 13:46:46.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.970081 autorag-0.1.6/tests/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1160 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3283 2024-04-27 06:36:55.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1994 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2213 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1881 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_jina_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1407 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4364 2024-04-27 06:36:55.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2230 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1604 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1371 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1210 2024-04-12 13:21:50.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_time_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      956 2024-04-27 06:36:55.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.972069 autorag-0.1.6/tests/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 autorag-0.1.6/tests/autorag/nodes/promptmaker/test_fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 autorag-0.1.6/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 autorag-0.1.6/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8310 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.973767 autorag-0.1.6/tests/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.977232 autorag-0.1.6/tests/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4013 2024-04-11 14:29:33.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1525 2024-04-11 14:29:33.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      879 2024-04-11 14:29:33.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2989 2024-04-10 06:33:52.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      780 2024-04-11 14:29:33.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_retrieval_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4692 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.977962 autorag-0.1.6/tests/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/schema/test_module_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/schema/test_node_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 autorag-0.1.6/tests/autorag/test_cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6869 2024-04-10 13:46:46.000000 autorag-0.1.6/tests/autorag/test_deploy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14669 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/test_evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/test_strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/test_support.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 autorag-0.1.6/tests/autorag/test_web.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.978741 autorag-0.1.6/tests/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3773 2024-04-27 06:36:55.000000 autorag-0.1.6/tests/autorag/utils/test_preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9970 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/utils/test_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 autorag-0.1.6/tests/conftest.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 autorag-0.1.6/tests/delete_tests.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 autorag-0.1.6/tests/mock.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.982321 autorag-0.1.6/tests/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 autorag-0.1.6/tests/resources/README.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.6/tests/resources/corpus_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.876758 autorag-0.1.6/tests/resources/data_creation/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.983395 autorag-0.1.6/tests/resources/data_creation/raw_dir/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 autorag-0.1.6/tests/resources/data_creation/raw_dir/sample1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 autorag-0.1.6/tests/resources/data_creation/raw_dir/sample2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 autorag-0.1.6/tests/resources/data_creation/raw_dir/sample3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-04-12 16:43:24.000000 autorag-0.1.6/tests/resources/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.6/tests/resources/qa_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.984480 autorag-0.1.6/tests/resources/qa_gen_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-04-17 01:53:11.000000 autorag-0.1.6/tests/resources/qa_gen_prompts/prompt1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 autorag-0.1.6/tests/resources/qa_gen_prompts/prompt2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 autorag-0.1.6/tests/resources/qa_gen_prompts/prompt3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 autorag-0.1.6/tests/resources/qa_test_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.985179 autorag-0.1.6/tests/resources/result_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.985978 autorag-0.1.6/tests/resources/result_project/0/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.986524 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.990866 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.996673 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.997050 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.999166 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.999506 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.000654 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.002820 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.004956 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 autorag-0.1.6/tests/resources/result_project/0/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.005203 autorag-0.1.6/tests/resources/result_project/1/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.005881 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.008094 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.878005 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.008413 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.009614 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.116036 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.116512 autorag-0.1.6/tests/resources/result_project/2/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.878189 autorag-0.1.6/tests/resources/result_project/2/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.117092 autorag-0.1.6/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.117494 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.122495 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.122821 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.124069 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.126726 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.129135 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.129399 autorag-0.1.6/tests/resources/result_project/3/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/3/config.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 autorag-0.1.6/tests/resources/result_project/best.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.131748 autorag-0.1.6/tests/resources/result_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.132082 autorag-0.1.6/tests/resources/result_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/resources/bm25.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.132422 autorag-0.1.6/tests/resources/result_project/resources/chroma/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.141537 autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
+-rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 autorag-0.1.6/tests/resources/result_project/resources/chroma/chroma.sqlite3
+-rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/trial.json
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 autorag-0.1.6/tests/resources/sample_contents_nqa.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.879104 autorag-0.1.6/tests/resources/sample_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.142756 autorag-0.1.6/tests/resources/sample_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   115302 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/resources/sample_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.6/tests/resources/sample_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.143471 autorag-0.1.6/tests/resources/sample_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 autorag-0.1.6/tests/resources/sample_project/resources/bm25.pkl
+-rw-r--r--   0 jeffrey    (501) staff       (20)      893 2024-04-10 13:46:46.000000 autorag-0.1.6/tests/resources/simple.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 autorag-0.1.6/tests/resources/test_bm25_retrieval.pkl
```

### Comparing `autorag-0.1.5/.github/workflows/sphinx.yml` & `autorag-0.1.6/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/.github/workflows/test.yml` & `autorag-0.1.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/.gitignore` & `autorag-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/AutoRAG.egg-info/PKG-INFO` & `autorag-0.1.6/AutoRAG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -230,15 +230,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: pyarrow
 Requires-Dist: fastparquet
 Requires-Dist: sacrebleu
 Requires-Dist: evaluate
 Requires-Dist: rouge_score
 Requires-Dist: rich
-Requires-Dist: chromadb
+Requires-Dist: chromadb>=0.5.0
 Requires-Dist: click
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: torch
 Requires-Dist: sentencepiece
 Requires-Dist: guidance
 Requires-Dist: cohere>=5.0.0a9
```

### Comparing `autorag-0.1.5/AutoRAG.egg-info/SOURCES.txt` & `autorag-0.1.6/AutoRAG.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 CONTRIBUTING.md
 LICENSE
 README.md
 dev_requirements.txt
 pyproject.toml
 requirements.txt
 .github/dependabot.yml
+.github/workflows/publish.yml
 .github/workflows/sphinx.yml
 .github/workflows/test.yml
 AutoRAG.egg-info/PKG-INFO
 AutoRAG.egg-info/SOURCES.txt
 AutoRAG.egg-info/dependency_links.txt
 AutoRAG.egg-info/entry_points.txt
 AutoRAG.egg-info/requires.txt
@@ -83,14 +84,16 @@
 autorag/nodes/passagereranker/jina.py
 autorag/nodes/passagereranker/koreranker.py
 autorag/nodes/passagereranker/monot5.py
 autorag/nodes/passagereranker/pass_reranker.py
 autorag/nodes/passagereranker/rankgpt.py
 autorag/nodes/passagereranker/run.py
 autorag/nodes/passagereranker/sentence_transformer.py
+autorag/nodes/passagereranker/temp_new_colbert.py
+autorag/nodes/passagereranker/temp_old_upr.py
 autorag/nodes/passagereranker/time_reranker.py
 autorag/nodes/passagereranker/upr.py
 autorag/nodes/passagereranker/tart/__init__.py
 autorag/nodes/passagereranker/tart/modeling_enc_t5.py
 autorag/nodes/passagereranker/tart/tart.py
 autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
 autorag/nodes/promptmaker/__init__.py
```

### Comparing `autorag-0.1.5/AutoRAG.egg-info/requires.txt` & `autorag-0.1.6/AutoRAG.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 pyyaml
 pyarrow
 fastparquet
 sacrebleu
 evaluate
 rouge_score
 rich
-chromadb
+chromadb>=0.5.0
 click
 fastapi
 uvicorn
 torch
 sentencepiece
 guidance
 cohere>=5.0.0a9
```

### Comparing `autorag-0.1.5/CODE_OF_CONDUCT.md` & `autorag-0.1.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/CONTRIBUTING.md` & `autorag-0.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/LICENSE` & `autorag-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/PKG-INFO` & `autorag-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -230,15 +230,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: pyarrow
 Requires-Dist: fastparquet
 Requires-Dist: sacrebleu
 Requires-Dist: evaluate
 Requires-Dist: rouge_score
 Requires-Dist: rich
-Requires-Dist: chromadb
+Requires-Dist: chromadb>=0.5.0
 Requires-Dist: click
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: torch
 Requires-Dist: sentencepiece
 Requires-Dist: guidance
 Requires-Dist: cohere>=5.0.0a9
```

### Comparing `autorag-0.1.5/README.md` & `autorag-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/__init__.py` & `autorag-0.1.6/autorag/__init__.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/cli.py` & `autorag-0.1.6/autorag/cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/data/corpus/langchain.py` & `autorag-0.1.6/autorag/data/corpus/langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/data/corpus/llama_index.py` & `autorag-0.1.6/autorag/data/corpus/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/data/qacreation/base.py` & `autorag-0.1.6/autorag/data/qacreation/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/data/qacreation/llama_index.py` & `autorag-0.1.6/autorag/data/qacreation/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/data/qacreation/llama_index_default_prompt.txt` & `autorag-0.1.6/autorag/data/qacreation/llama_index_default_prompt.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/data/qacreation/ragas.py` & `autorag-0.1.6/autorag/data/qacreation/ragas.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/data/qacreation/simple.py` & `autorag-0.1.6/autorag/data/qacreation/simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/data/utils/util.py` & `autorag-0.1.6/autorag/data/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/deploy.py` & `autorag-0.1.6/autorag/deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/evaluate/generation.py` & `autorag-0.1.6/autorag/evaluate/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt` & `autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt` & `autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt` & `autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt` & `autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/evaluate/metric/generation.py` & `autorag-0.1.6/autorag/evaluate/metric/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/evaluate/metric/retrieval.py` & `autorag-0.1.6/autorag/evaluate/metric/retrieval.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import functools
 from typing import List
 
 
 def retrieval_metric(func):
     @functools.wraps(func)
     def wrapper(retrieval_gt: List[List[List[str]]], pred_ids: List[List[str]]) -> List[float]:
-        return list(map(lambda x: func(x[0], x[1]), zip(retrieval_gt, pred_ids)))
+        results = []
+        for gt, pred in zip(retrieval_gt, pred_ids):
+            if gt == [[]] or any(bool(g_) is False for g in gt for g_ in g):
+                results.append(None)
+            else:
+                results.append(func(gt, pred))
+        return results
 
     return wrapper
 
 
 @retrieval_metric
 def retrieval_f1(gt: List[List[str]], pred: List[str]):
     """
```

### Comparing `autorag-0.1.5/autorag/evaluate/metric/retrieval_contents.py` & `autorag-0.1.6/autorag/evaluate/metric/retrieval_contents.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,21 @@
 
 from autorag.utils.util import normalize_string
 
 
 def retrieval_contents_metric(func):
     @functools.wraps(func)
     def wrapper(gt_contents: List[List[str]], pred_contents: List[List[str]]) -> List[float]:
-        return list(map(lambda x: func(x[0], x[1]), zip(gt_contents, pred_contents)))
+        results = []
+        for gt, pred in zip(gt_contents, pred_contents):
+            if gt == [] or any(bool(g) is False for g in gt):
+                results.append(None)
+            else:
+                results.append(func(gt, pred))
+        return results
 
     return wrapper
 
 
 def single_token_f1(ground_truth: str, prediction: str):
     prediction_tokens = normalize_string(prediction).split()
     ground_truth_tokens = normalize_string(ground_truth).split()
```

### Comparing `autorag-0.1.5/autorag/evaluate/retrieval.py` & `autorag-0.1.6/autorag/evaluate/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/evaluate/retrieval_contents.py` & `autorag-0.1.6/autorag/evaluate/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/evaluate/util.py` & `autorag-0.1.6/autorag/evaluate/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/evaluator.py` & `autorag-0.1.6/autorag/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from autorag import embedding_models
 from autorag.node_line import run_node_line
 from autorag.nodes.retrieval.bm25 import bm25_ingest
 from autorag.nodes.retrieval.vectordb import vectordb_ingest
 from autorag.schema import Node
 from autorag.schema.node import module_type_exists, extract_values_from_nodes
-from autorag.utils import cast_qa_dataset, cast_corpus_dataset
+from autorag.utils import cast_qa_dataset, cast_corpus_dataset, validate_qa_from_corpus_dataset
 from autorag.utils.util import load_summary_file, convert_string_to_tuple_in_dict, convert_env_in_dict, explode
 
 logger = logging.getLogger("AutoRAG")
 
 ascii_art = """
                 _        _____            _____ 
      /\        | |      |  __ \     /\   / ____|
@@ -59,14 +59,16 @@
         self.corpus_data = pd.read_parquet(corpus_data_path)
         self.qa_data = cast_qa_dataset(self.qa_data)
         self.corpus_data = cast_corpus_dataset(self.corpus_data)
         self.project_dir = project_dir if project_dir is not None else os.getcwd()
         if not os.path.exists(self.project_dir):
             os.makedirs(self.project_dir)
 
+        validate_qa_from_corpus_dataset(self.qa_data, self.corpus_data)
+
         # copy dataset to project directory
         if not os.path.exists(os.path.join(self.project_dir, 'data')):
             os.makedirs(os.path.join(self.project_dir, 'data'))
         qa_path_in_project = os.path.join(self.project_dir, 'data', 'qa.parquet')
         if not os.path.exists(qa_path_in_project):
             self.qa_data.to_parquet(qa_path_in_project, index=False)
         corpus_path_in_project = os.path.join(self.project_dir, 'data', 'corpus.parquet')
```

### Comparing `autorag-0.1.5/autorag/node_line.py` & `autorag-0.1.6/autorag/node_line.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/generator/base.py` & `autorag-0.1.6/autorag/nodes/generator/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/generator/llama_index_llm.py` & `autorag-0.1.6/autorag/nodes/generator/llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/generator/run.py` & `autorag-0.1.6/autorag/nodes/generator/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/generator/vllm.py` & `autorag-0.1.6/autorag/nodes/generator/vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passageaugmenter/base.py` & `autorag-0.1.6/autorag/nodes/passageaugmenter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passageaugmenter/prev_next_augmenter.py` & `autorag-0.1.6/autorag/nodes/passageaugmenter/prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passageaugmenter/run.py` & `autorag-0.1.6/autorag/nodes/passageaugmenter/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
                                node_line_dir: str,
                                strategies: Dict,
                                ) -> pd.DataFrame:
     if not os.path.exists(node_line_dir):
         os.makedirs(node_line_dir)
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
     retrieval_gt = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))['retrieval_gt'].tolist()
+    retrieval_gt = [[[str(uuid) for uuid in sub_array] if sub_array.size > 0 else [] for sub_array in inner_array]
+                    for inner_array in retrieval_gt]
 
     results, execution_times = zip(*map(lambda task: measure_speed(
         task[0], project_dir=project_dir, previous_result=previous_result, **task[1]), zip(modules, module_params)))
     average_times = list(map(lambda x: x / len(results[0]), execution_times))
 
     # run metrics before filtering
     if strategies.get('metrics') is None:
```

### Comparing `autorag-0.1.5/autorag/nodes/passagecompressor/base.py` & `autorag-0.1.6/autorag/nodes/passagecompressor/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagecompressor/refine.py` & `autorag-0.1.6/autorag/nodes/passagecompressor/refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagecompressor/run.py` & `autorag-0.1.6/autorag/nodes/passagecompressor/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagecompressor/tree_summarize.py` & `autorag-0.1.6/autorag/nodes/passagecompressor/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagefilter/base.py` & `autorag-0.1.6/autorag/nodes/passagefilter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagefilter/percentile_cutoff.py` & `autorag-0.1.6/autorag/nodes/passagefilter/percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagefilter/recency.py` & `autorag-0.1.6/autorag/nodes/passagefilter/recency.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagefilter/run.py` & `autorag-0.1.6/autorag/nodes/passagefilter/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         You can skip evaluation when you use only one module and a module parameter.
     :return: The best result dataframe with previous result columns.
     """
     if not os.path.exists(node_line_dir):
         os.makedirs(node_line_dir)
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
     retrieval_gt = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))['retrieval_gt'].tolist()
+    retrieval_gt = [[[str(uuid) for uuid in sub_array] if sub_array.size > 0 else [] for sub_array in inner_array]
+                    for inner_array in retrieval_gt]
 
     results, execution_times = zip(*map(lambda task: measure_speed(
         task[0], project_dir=project_dir, previous_result=previous_result, **task[1]), zip(modules, module_params)))
     average_times = list(map(lambda x: x / len(results[0]), execution_times))
 
     # run metrics before filtering
     if strategies.get('metrics') is None:
```

### Comparing `autorag-0.1.5/autorag/nodes/passagefilter/threshold_cutoff.py` & `autorag-0.1.6/autorag/nodes/passagefilter/threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/base.py` & `autorag-0.1.6/autorag/nodes/passagereranker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/cohere.py` & `autorag-0.1.6/autorag/nodes/passagereranker/cohere.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/flag_embedding.py` & `autorag-0.1.6/autorag/nodes/passagereranker/flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/flag_embedding_llm.py` & `autorag-0.1.6/autorag/nodes/passagereranker/flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/jina.py` & `autorag-0.1.6/autorag/nodes/passagereranker/jina.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/koreranker.py` & `autorag-0.1.6/autorag/nodes/passagereranker/koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/monot5.py` & `autorag-0.1.6/autorag/nodes/passagereranker/monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/pass_reranker.py` & `autorag-0.1.6/autorag/nodes/passagereranker/pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/rankgpt.py` & `autorag-0.1.6/autorag/nodes/passagereranker/rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/run.py` & `autorag-0.1.6/autorag/nodes/passagereranker/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         You can skip evaluation when you use only one module and a module parameter.
     :return: The best result dataframe with previous result columns.
     """
     if not os.path.exists(node_line_dir):
         os.makedirs(node_line_dir)
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
     retrieval_gt = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))['retrieval_gt'].tolist()
+    retrieval_gt = [[[str(uuid) for uuid in sub_array] if sub_array.size > 0 else [] for sub_array in inner_array]
+                    for inner_array in retrieval_gt]
 
     results, execution_times = zip(*map(lambda task: measure_speed(
         task[0], project_dir=project_dir, previous_result=previous_result, **task[1]), zip(modules, module_params)))
     average_times = list(map(lambda x: x / len(results[0]), execution_times))
 
     # run metrics before filtering
     if strategies.get('metrics') is None:
```

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/sentence_transformer.py` & `autorag-0.1.6/autorag/nodes/passagereranker/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/tart/modeling_enc_t5.py` & `autorag-0.1.6/autorag/nodes/passagereranker/tart/modeling_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/tart/tart.py` & `autorag-0.1.6/autorag/nodes/passagereranker/tart/tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py` & `autorag-0.1.6/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/time_reranker.py` & `autorag-0.1.6/autorag/nodes/passagereranker/time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/passagereranker/upr.py` & `autorag-0.1.6/autorag/nodes/passagereranker/temp_old_upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/promptmaker/base.py` & `autorag-0.1.6/autorag/nodes/promptmaker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/promptmaker/fstring.py` & `autorag-0.1.6/autorag/nodes/promptmaker/fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/promptmaker/long_context_reorder.py` & `autorag-0.1.6/autorag/nodes/promptmaker/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/promptmaker/run.py` & `autorag-0.1.6/autorag/nodes/promptmaker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/queryexpansion/base.py` & `autorag-0.1.6/autorag/nodes/queryexpansion/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/queryexpansion/hyde.py` & `autorag-0.1.6/autorag/nodes/queryexpansion/hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/queryexpansion/query_decompose.py` & `autorag-0.1.6/autorag/nodes/queryexpansion/query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/queryexpansion/run.py` & `autorag-0.1.6/autorag/nodes/queryexpansion/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/retrieval/base.py` & `autorag-0.1.6/autorag/nodes/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/retrieval/bm25.py` & `autorag-0.1.6/autorag/nodes/retrieval/bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/retrieval/hybrid_cc.py` & `autorag-0.1.6/autorag/nodes/retrieval/hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/retrieval/hybrid_dbsf.py` & `autorag-0.1.6/autorag/nodes/retrieval/hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/retrieval/hybrid_rrf.py` & `autorag-0.1.6/autorag/nodes/retrieval/hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/retrieval/hybrid_rsf.py` & `autorag-0.1.6/autorag/nodes/retrieval/hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/nodes/retrieval/run.py` & `autorag-0.1.6/autorag/nodes/retrieval/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     :return: The best result dataframe.
         It contains previous result columns and retrieval node's result columns.
     """
     if not os.path.exists(node_line_dir):
         os.makedirs(node_line_dir)
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
     retrieval_gt = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))['retrieval_gt'].tolist()
+    retrieval_gt = [[[str(uuid) for uuid in sub_array] if sub_array.size > 0 else [] for sub_array in inner_array]
+                    for inner_array in retrieval_gt]
+
     save_dir = os.path.join(node_line_dir, "retrieval")  # node name
     if not os.path.exists(save_dir):
         os.makedirs(save_dir)
 
     def run_and_save(input_modules, input_module_params, filename_start: int):
         result, execution_times = zip(*map(lambda task: measure_speed(
             task[0], project_dir=project_dir, previous_result=previous_result, **task[1]),
```

### Comparing `autorag-0.1.5/autorag/nodes/retrieval/vectordb.py` & `autorag-0.1.6/autorag/nodes/retrieval/vectordb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 from typing import List, Tuple
 
 import chromadb
 import pandas as pd
+from chromadb.utils.batch_utils import create_batches
 from llama_index.core.embeddings import BaseEmbedding
 from llama_index.embeddings.openai import OpenAIEmbedding
 
 from autorag.nodes.retrieval.base import retrieval_node, evenly_distribute_passages
 from autorag.utils import validate_corpus_dataset
 from autorag.utils.util import process_batch, openai_truncate_by_token
 
@@ -91,8 +92,12 @@
         # truncate by token if embedding_model is OpenAIEmbedding
         if isinstance(embedding_model, OpenAIEmbedding):
             openai_embedding_limit = 8191
             new_contents = openai_truncate_by_token(new_contents, openai_embedding_limit, embedding_model.model_name)
 
         new_ids = new_passage['doc_id'].tolist()
         embedded_contents = embedding_model.get_text_embedding_batch(new_contents, show_progress=True)
-        collection.add(ids=new_ids, embeddings=embedded_contents)
+        input_batches = create_batches(api=collection._client, ids=new_ids, embeddings=embedded_contents)
+        for batch in input_batches:
+            ids = batch[0]
+            embed_content = batch[1]
+            collection.add(ids=ids, embeddings=embed_content)
```

### Comparing `autorag-0.1.5/autorag/schema/module.py` & `autorag-0.1.6/autorag/schema/module.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/schema/node.py` & `autorag-0.1.6/autorag/schema/node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/strategy.py` & `autorag-0.1.6/autorag/strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/support.py` & `autorag-0.1.6/autorag/support.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/autorag/utils/util.py` & `autorag-0.1.6/autorag/utils/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,35 @@
 import tiktoken
 
 logger = logging.getLogger("AutoRAG")
 
 
 def fetch_contents(corpus_data: pd.DataFrame, ids: List[List[str]],
                    column_name: str = 'contents') -> List[List[Any]]:
-    flat_ids = itertools.chain.from_iterable(ids)
-    contents = list(map(lambda x: corpus_data.loc[lambda row: row['doc_id'] == x][column_name].values[0], flat_ids))
-
-    result = []
-    idx = 0
-    for sublist in ids:
-        result.append(contents[idx:idx + len(sublist)])
-        idx += len(sublist)
+    def fetch_contents_pure(ids: List[str], corpus_data: pd.DataFrame, column_name: str):
+        return list(map(lambda x: fetch_one_content(corpus_data, x, column_name), ids))
 
+    result = flatten_apply(fetch_contents_pure, ids, corpus_data=corpus_data, column_name=column_name)
     return result
 
 
+def fetch_one_content(corpus_data: pd.DataFrame, id_: str,
+                      column_name: str = 'contents') -> Any:
+    if isinstance(id_, str):
+        if id_ in ['', ""]:
+            return None
+        fetch_result = corpus_data[corpus_data['doc_id'] == id_]
+        if fetch_result.empty:
+            raise ValueError(f"doc_id: {id_} not found in corpus_data.")
+        else:
+            return fetch_result[column_name].iloc[0]
+    else:
+        return None
+
+
 def result_to_dataframe(column_names: List[str]):
     """
     Decorator for converting results to pd.DataFrame.
     """
 
     def decorator_result_to_dataframe(func: Callable):
         @functools.wraps(func)
```

### Comparing `autorag-0.1.5/autorag/web.py` & `autorag-0.1.6/autorag/web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/Makefile` & `autorag-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/make.bat` & `autorag-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/data_creation.png` & `autorag-0.1.6/docs/source/_static/data_creation.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/data_folder.png` & `autorag-0.1.6/docs/source/_static/data_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/node_folder.png` & `autorag-0.1.6/docs/source/_static/node_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/node_line_folder.png` & `autorag-0.1.6/docs/source/_static/node_line_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/node_line_summary.png` & `autorag-0.1.6/docs/source/_static/node_line_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/node_lines.png` & `autorag-0.1.6/docs/source/_static/node_lines.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/node_summary.png` & `autorag-0.1.6/docs/source/_static/node_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/project_folder_example.png` & `autorag-0.1.6/docs/source/_static/project_folder_example.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/project_folders.png` & `autorag-0.1.6/docs/source/_static/project_folders.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/resources_folder.png` & `autorag-0.1.6/docs/source/_static/resources_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/roadmap/RAG_paradigms.png` & `autorag-0.1.6/docs/source/_static/roadmap/RAG_paradigms.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/roadmap/advanced_RAG.png` & `autorag-0.1.6/docs/source/_static/roadmap/advanced_RAG.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/roadmap/cycle.png` & `autorag-0.1.6/docs/source/_static/roadmap/cycle.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/roadmap/merger.png` & `autorag-0.1.6/docs/source/_static/roadmap/merger.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/roadmap/node_line_modular.png` & `autorag-0.1.6/docs/source/_static/roadmap/node_line_modular.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/roadmap/policy.png` & `autorag-0.1.6/docs/source/_static/roadmap/policy.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/samsung_sundae.jpeg` & `autorag-0.1.6/docs/source/_static/samsung_sundae.jpeg`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/trial_folder.png` & `autorag-0.1.6/docs/source/_static/trial_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/trial_json.png` & `autorag-0.1.6/docs/source/_static/trial_json.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/trial_summary.png` & `autorag-0.1.6/docs/source/_static/trial_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/_static/web_interface.png` & `autorag-0.1.6/docs/source/_static/web_interface.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.data.corpus.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.data.corpus.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.data.qacreation.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.data.qacreation.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.evaluate.metric.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.evaluate.metric.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.evaluate.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.evaluate.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.nodes.generator.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.nodes.generator.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.nodes.passageaugmenter.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.nodes.passageaugmenter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagecompressor.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagecompressor.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagefilter.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagefilter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagereranker.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagereranker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.nodes.promptmaker.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.nodes.promptmaker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.nodes.queryexpansion.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.nodes.queryexpansion.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.nodes.retrieval.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.nodes.retrieval.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/api_spec/autorag.rst` & `autorag-0.1.6/docs/source/api_spec/autorag.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/conf.py` & `autorag-0.1.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/data_creation/data_format.md` & `autorag-0.1.6/docs/source/data_creation/data_format.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/data_creation/ragas.md` & `autorag-0.1.6/docs/source/data_creation/ragas.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/data_creation/tutorial.md` & `autorag-0.1.6/docs/source/data_creation/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/deploy/api_endpoint.md` & `autorag-0.1.6/docs/source/deploy/api_endpoint.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/deploy/web.md` & `autorag-0.1.6/docs/source/deploy/web.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/index.rst` & `autorag-0.1.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/install.md` & `autorag-0.1.6/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/local_model.md` & `autorag-0.1.6/docs/source/local_model.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/generator/generator.md` & `autorag-0.1.6/docs/source/nodes/generator/generator.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/generator/llama_index_llm.md` & `autorag-0.1.6/docs/source/nodes/generator/llama_index_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/generator/vllm.md` & `autorag-0.1.6/docs/source/nodes/generator/vllm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_augmenter/passage_augmenter.md` & `autorag-0.1.6/docs/source/nodes/passage_augmenter/passage_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_augmenter/prev_next_augmenter.md` & `autorag-0.1.6/docs/source/nodes/passage_augmenter/prev_next_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_compressor/passage_compressor.md` & `autorag-0.1.6/docs/source/nodes/passage_compressor/passage_compressor.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_compressor/refine.md` & `autorag-0.1.6/docs/source/nodes/passage_compressor/refine.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_compressor/tree_summarize.md` & `autorag-0.1.6/docs/source/nodes/passage_compressor/tree_summarize.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_filter/passage_filter.md` & `autorag-0.1.6/docs/source/nodes/passage_filter/passage_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_filter/recency_filter.md` & `autorag-0.1.6/docs/source/nodes/passage_filter/recency_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md` & `autorag-0.1.6/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md` & `autorag-0.1.6/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/cohere.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/cohere.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/colbert.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/colbert.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/flag_embedding_reranker.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/flag_embedding_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/jina_reranker.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/jina_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/monot5.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/monot5.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/passage_reranker.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/passage_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/rankgpt.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/rankgpt.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/tart.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/tart.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/time_reranker.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/time_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/passage_reranker/upr.md` & `autorag-0.1.6/docs/source/nodes/passage_reranker/upr.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/prompt_maker/fstring.md` & `autorag-0.1.6/docs/source/nodes/prompt_maker/fstring.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/prompt_maker/long_context_reorder.md` & `autorag-0.1.6/docs/source/nodes/prompt_maker/long_context_reorder.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/prompt_maker/prompt_maker.md` & `autorag-0.1.6/docs/source/nodes/prompt_maker/prompt_maker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/query_expansion/hyde.md` & `autorag-0.1.6/docs/source/nodes/query_expansion/hyde.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/query_expansion/query_decompose.md` & `autorag-0.1.6/docs/source/nodes/query_expansion/query_decompose.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/query_expansion/query_expansion.md` & `autorag-0.1.6/docs/source/nodes/query_expansion/query_expansion.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/retrieval/bm25.md` & `autorag-0.1.6/docs/source/nodes/retrieval/bm25.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/retrieval/hybrid_cc.md` & `autorag-0.1.6/docs/source/nodes/retrieval/hybrid_cc.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/retrieval/hybrid_dbsf.md` & `autorag-0.1.6/docs/source/nodes/retrieval/hybrid_dbsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/retrieval/hybrid_rrf.md` & `autorag-0.1.6/docs/source/nodes/retrieval/hybrid_rrf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/retrieval/hybrid_rsf.md` & `autorag-0.1.6/docs/source/nodes/retrieval/hybrid_rsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/retrieval/retrieval.md` & `autorag-0.1.6/docs/source/nodes/retrieval/retrieval.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/nodes/retrieval/vectordb.md` & `autorag-0.1.6/docs/source/nodes/retrieval/vectordb.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/optimization/custom_config.md` & `autorag-0.1.6/docs/source/optimization/custom_config.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/optimization/folder_structure.md` & `autorag-0.1.6/docs/source/optimization/folder_structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/optimization/optimization.md` & `autorag-0.1.6/docs/source/optimization/optimization.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/optimization/sample_full_config.yaml` & `autorag-0.1.6/docs/source/optimization/sample_full_config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/roadmap/modular_rag.md` & `autorag-0.1.6/docs/source/roadmap/modular_rag.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/structure.md` & `autorag-0.1.6/docs/source/structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/troubleshooting.md` & `autorag-0.1.6/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/docs/source/tutorial.md` & `autorag-0.1.6/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/pyproject.toml` & `autorag-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/requirements.txt` & `autorag-0.1.6/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 pyyaml  # for yaml file
 pyarrow  # for pandas with parquet
 fastparquet  # for pandas with parquet
 sacrebleu  # for bleu score
 evaluate  # for meteor and other scores
 rouge_score  # for rouge score
 rich  # for pretty logging
-chromadb # for vectordb retrieval
+chromadb>=0.5.0 # for vectordb retrieval
 click  # for cli
 fastapi  # for api server
 uvicorn  # for api server
 torch  # for monot5 reranker
 sentencepiece  # for monot5 reranker
 guidance # for qa data creation
 cohere>=5.0.0a9 # for cohere services
```

### Comparing `autorag-0.1.5/sample_config/compact_local.yaml` & `autorag-0.1.6/sample_config/compact_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/sample_config/compact_openai.yaml` & `autorag-0.1.6/sample_config/compact_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/sample_config/config_korean.yaml` & `autorag-0.1.6/sample_config/config_korean.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/sample_config/extracted_sample.yaml` & `autorag-0.1.6/sample_config/extracted_sample.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/sample_config/full.yaml` & `autorag-0.1.6/sample_config/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/sample_config/simple_local.yaml` & `autorag-0.1.6/sample_config/simple_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/sample_config/simple_openai.yaml` & `autorag-0.1.6/sample_config/simple_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/sample_dataset/README.md` & `autorag-0.1.6/sample_dataset/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/sample_dataset/eli5/load_eli5_dataset.py` & `autorag-0.1.6/sample_dataset/eli5/load_eli5_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/sample_dataset/msmarco/load_msmarco_dataset.py` & `autorag-0.1.6/sample_dataset/msmarco/load_msmarco_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/sample_dataset/triviaqa/load_triviaqa_dataset.py` & `autorag-0.1.6/sample_dataset/triviaqa/load_triviaqa_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/data/corpus/test_base.py` & `autorag-0.1.6/tests/autorag/data/corpus/test_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/data/corpus/test_langchain.py` & `autorag-0.1.6/tests/autorag/data/corpus/test_langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/data/corpus/test_llama_index_corpus.py` & `autorag-0.1.6/tests/autorag/data/corpus/test_llama_index_corpus.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/data/qacreation/test_base_qacreation.py` & `autorag-0.1.6/tests/autorag/data/qacreation/test_base_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/data/qacreation/test_llama_index_qacreation.py` & `autorag-0.1.6/tests/autorag/data/qacreation/test_llama_index_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/data/qacreation/test_ragas_qa_creation.py` & `autorag-0.1.6/tests/autorag/data/qacreation/test_ragas_qa_creation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/data/qacreation/test_simple.py` & `autorag-0.1.6/tests/autorag/data/qacreation/test_simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/evaluate/metric/test_generation_metric.py` & `autorag-0.1.6/tests/autorag/evaluate/metric/test_generation_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py` & `autorag-0.1.6/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import pytest
 
 from autorag.evaluate.metric.retrieval_contents import single_token_f1, retrieval_token_f1, retrieval_token_precision, \
     retrieval_token_recall
 
 gt = [
     ['Enough for drinking water', 'Just looking for a water bottle'],
-    ['Do you want to buy some?']
+    ['Do you want to buy some?'],
+    [''],
+    []
 ]
 pred = [
     ['Enough for mixing water', 'I want to do a nothing', 'Just looking is a very healthy'],
-    ['Do you want to buy some?', 'I want to buy some', 'I want to buy some water']
+    ['Do you want to buy some?', 'I want to buy some', 'I want to buy some water'],
+    ['Who is son? He is great player in the world'],
+    ['i love havertz', 'i love kai havertz']
 ]
 
 
 def test_single_token_f1():
     precision, recall, f1 = single_token_f1(gt[0][0], pred[0][0])
     assert precision == 0.75
     assert recall == 0.75
@@ -29,18 +33,18 @@
     f1 = retrieval_token_f1.__wrapped__(gt[0], pred[0])
     assert f1 == pytest.approx(0.38333, rel=0.001)
 
     f1 = retrieval_token_f1.__wrapped__(gt[1], pred[1])
     assert f1 == pytest.approx(0.797979, rel=0.001)
 
     result_f1 = retrieval_token_f1(gt_contents=gt, pred_contents=pred)
-    assert result_f1 == pytest.approx([0.38333, 0.797979], rel=0.001)
+    assert result_f1 == pytest.approx([0.38333, 0.797979, None, None], rel=0.001)
 
 
 def test_retrieval_token_precision():
     result_precision = retrieval_token_precision(gt_contents=gt, pred_contents=pred)
-    assert result_precision == pytest.approx([0.383333, 0.8222222], rel=0.001)
+    assert result_precision == pytest.approx([0.383333, 0.8222222, None, None], rel=0.001)
 
 
 def test_retrieval_token_recall():
     result_recall = retrieval_token_recall(gt_contents=gt, pred_contents=pred)
-    assert result_recall == pytest.approx([0.383333, 0.777777], rel=0.001)
+    assert result_recall == pytest.approx([0.383333, 0.777777, None, None], rel=0.001)
```

### Comparing `autorag-0.1.5/tests/autorag/evaluate/metric/test_retrieval_metric.py` & `autorag-0.1.6/tests/autorag/evaluate/metric/test_retrieval_metric.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import math
-
 import pytest
 
 from autorag.evaluate.metric import retrieval_f1, retrieval_precision, retrieval_recall
 
 retrieval_gt = [
     [['test-1', 'test-2'], ['test-3']],
     [['test-4', 'test-5'], ['test-6', 'test-7'], ['test-8']],
     [['test-9', 'test-10']],
     [['test-11'], ['test-12'], ['test-13']],
     [['test-14']],
-    [['test-15']],
+    [[]],
+    [['']]
 ]
 
 pred = [
     ['test-1', 'pred-1', 'test-2', 'pred-3'],  # recall: 0.5, precision: 0.5, f1: 0.5
     ['test-6', 'pred-5', 'pred-6', 'pred-7'],  # recall: 1/3, precision: 0.25, f1: 2/7
     ['test-9', 'pred-0', 'pred-8', 'pred-9'],  # recall: 1.0, precision: 0.25, f1: 2/5
     ['test-13', 'test-12', 'pred-10', 'pred-11'],  # recall: 2/3, precision: 0.5, f1: 4/7
     ['test-14', 'pred-12'],  # recall: 1.0, precision: 0.5, f1: 2/3
-    ['pred-13'],  # recall: 0.0, precision: 0.0, f1: 0.0
+    ['pred-13'],  # retrieval_gt is empty so not counted
+    ['pred-14']  # retrieval_gt is empty so not counted
 ]
 
 
 def test_retrieval_f1():
-    solution = [0.5, 2 / 7, 2 / 5, 4 / 7, 2 / 3, 0.0]
+    solution = [0.5, 2 / 7, 2 / 5, 4 / 7, 2 / 3, None, None]
     result = retrieval_f1(retrieval_gt=retrieval_gt, pred_ids=pred)
     for gt, res in zip(solution, result):
-        assert math.isclose(gt, res, rel_tol=1e-4)
+        assert gt == pytest.approx(res, rel=1e-4)
 
 
 def test_retrieval_recall():
-    solution = [0.5, 1 / 3, 1, 2 / 3, 1, 0.0]
+    solution = [0.5, 1 / 3, 1, 2 / 3, 1, None, None]
     result = retrieval_recall(retrieval_gt=retrieval_gt, pred_ids=pred)
     for gt, res in zip(solution, result):
         assert gt == pytest.approx(res, rel=1e-4)
 
 
 def test_retrieval_precision():
-    solution = [0.5, 0.25, 0.25, 0.5, 0.5, 0.0]
+    solution = [0.5, 0.25, 0.25, 0.5, 0.5, None, None]
     result = retrieval_precision(retrieval_gt=retrieval_gt, pred_ids=pred)
     for gt, res in zip(solution, result):
         assert gt == pytest.approx(res, rel=1e-4)
```

### Comparing `autorag-0.1.5/tests/autorag/evaluate/test_evaluate_util.py` & `autorag-0.1.6/tests/autorag/evaluate/test_evaluate_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/evaluate/test_generation_evaluate.py` & `autorag-0.1.6/tests/autorag/evaluate/test_generation_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/evaluate/test_retrieval_contents_evaluate.py` & `autorag-0.1.6/tests/autorag/evaluate/test_retrieval_contents_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/evaluate/test_retrieval_evaluate.py` & `autorag-0.1.6/tests/autorag/evaluate/test_retrieval_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/generator/test_generator_base.py` & `autorag-0.1.6/tests/autorag/nodes/generator/test_generator_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/generator/test_llama_index_llm.py` & `autorag-0.1.6/tests/autorag/nodes/generator/test_llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/generator/test_run_generator_node.py` & `autorag-0.1.6/tests/autorag/nodes/generator/test_run_generator_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/generator/test_vllm.py` & `autorag-0.1.6/tests/autorag/nodes/generator/test_vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py` & `autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py` & `autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py` & `autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py` & `autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py` & `autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_pass_compressor.py` & `autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_pass_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_refine.py` & `autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py` & `autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 root_dir = pathlib.PurePath(os.path.dirname(os.path.realpath(__file__))).parent.parent.parent
 resources_dir = os.path.join(root_dir, "resources")
 qa_data = pd.DataFrame({
     'qid': ['id-1', 'id-2', 'id-3'],
     'query': ['query-1', 'query-2', 'query-3'],
     'retrieval_gt': [
         [['doc-1'], ['doc-2']],
-        [['doc-3'], ['doc-4']],
+        [[]],
         [['doc-5'], ['doc-6']],
     ],
     'generation_gt': [['generation-1'], ['generation-2'], ['generation-3']],
 })
 corpus_data = pd.DataFrame({
     'doc_id': ['doc-1', 'doc-2', 'doc-3', 'doc-4', 'doc-5', 'doc-6'],
     'contents': [
```

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_tree_summarize.py` & `autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py` & `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagefilter/test_passage_filter_base.py` & `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_passage_filter_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagefilter/test_passage_filter_run.py` & `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_passage_filter_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py` & `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagefilter/test_recency_filter.py` & `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_recency_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py` & `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_cohere_reranker.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_colbert_reranker.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_koreranker.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import pytest
 
-from autorag.nodes.passagereranker import colbert_reranker
-from tests.autorag.nodes.passagereranker.test_passage_reranker_base import queries_example, contents_example, \
-    scores_example, ids_example, base_reranker_test, project_dir, previous_result, base_reranker_node_test
+from autorag.nodes.passagereranker import koreranker
+from tests.autorag.nodes.passagereranker.test_passage_reranker_base \
+    import (base_reranker_test, base_reranker_node_test, ko_queries_example,
+            ko_contents_example, scores_example, ids_example, project_dir, ko_previous_result)
 from tests.delete_tests import is_github_action
 
 
-@pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions because it uses local model.")
-def test_colbert_reranker():
-    top_k = 2
-    original_colbert_reranker = colbert_reranker.__wrapped__
+@pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
+def test_koreranker():
+    top_k = 1
+    original_koreranker = koreranker.__wrapped__
     contents_result, id_result, score_result \
-        = original_colbert_reranker(queries_example, contents_example, scores_example, ids_example, top_k)
-    base_reranker_test(contents_result, id_result, score_result, top_k)
+        = original_koreranker(ko_queries_example, ko_contents_example, scores_example, ids_example, top_k)
+    base_reranker_test(contents_result, id_result, score_result, top_k, use_ko=True)
 
 
-@pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions because it uses local model.")
-def test_colbert_reranker_node():
+@pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
+def test_koreranker_node():
     top_k = 1
-    result_df = colbert_reranker(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
-    base_reranker_node_test(result_df, top_k)
+    result_df = koreranker(project_dir=project_dir, previous_result=ko_previous_result, top_k=top_k)
+    base_reranker_node_test(result_df, top_k, use_ko=True)
```

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_flag_embedding.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_jina_reranker.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_jina_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_koreranker.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_upr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import pytest
 
-from autorag.nodes.passagereranker import koreranker
-from tests.autorag.nodes.passagereranker.test_passage_reranker_base \
-    import (base_reranker_test, base_reranker_node_test, ko_queries_example,
-            ko_contents_example, scores_example, ids_example, project_dir, ko_previous_result)
+from autorag.nodes.passagereranker import upr
+from tests.autorag.nodes.passagereranker.test_passage_reranker_base import base_reranker_test, queries_example, \
+    contents_example, scores_example, ids_example, base_reranker_node_test, project_dir, previous_result
 from tests.delete_tests import is_github_action
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
-def test_koreranker():
+def test_upr():
     top_k = 1
-    original_koreranker = koreranker.__wrapped__
+    original_upr = upr.__wrapped__
     contents_result, id_result, score_result \
-        = original_koreranker(ko_queries_example, ko_contents_example, scores_example, ids_example, top_k)
-    base_reranker_test(contents_result, id_result, score_result, top_k, use_ko=True)
+        = original_upr(queries_example, contents_example, scores_example, ids_example, top_k)
+    base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
-def test_koreranker_node():
+def test_upr_node():
     top_k = 1
-    result_df = koreranker(project_dir=project_dir, previous_result=ko_previous_result, top_k=top_k)
-    base_reranker_node_test(result_df, top_k, use_ko=True)
+    result_df = upr(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
+    base_reranker_node_test(result_df, top_k)
```

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_monot5.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_pass_reranker.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_rankgpt.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_sentence_transformer.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_tart.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_time_reranker.py` & `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/promptmaker/test_fstring.py` & `autorag-0.1.6/tests/autorag/nodes/promptmaker/test_fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/promptmaker/test_long_context_reorder.py` & `autorag-0.1.6/tests/autorag/nodes/promptmaker/test_long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py` & `autorag-0.1.6/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py` & `autorag-0.1.6/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_hyde.py` & `autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py` & `autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_decompose.py` & `autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py` & `autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py` & `autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/retrieval/test_bm25.py` & `autorag-0.1.6/tests/autorag/nodes/retrieval/test_bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_base.py` & `autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_cc.py` & `autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py` & `autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_rrf.py` & `autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_rsf.py` & `autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/retrieval/test_retrieval_base.py` & `autorag-0.1.6/tests/autorag/nodes/retrieval/test_retrieval_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/retrieval/test_run_retrieval_node.py` & `autorag-0.1.6/tests/autorag/nodes/retrieval/test_run_retrieval_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/nodes/retrieval/test_vectordb.py` & `autorag-0.1.6/tests/autorag/nodes/retrieval/test_vectordb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import pathlib
 import shutil
 import tempfile
+import uuid
 from datetime import datetime
+from unittest.mock import patch
 
 import chromadb
 import pandas as pd
 import pytest
 from llama_index.embeddings.openai import OpenAIEmbedding
 
 from autorag.nodes.retrieval import vectordb
@@ -29,14 +31,23 @@
         vectordb_ingest(collection, corpus_df, embedding_model)
 
         assert collection.count() == 5
         yield collection
 
 
 @pytest.fixture
+def empty_chromadb():
+    with tempfile.TemporaryDirectory() as chroma_path:
+        db = chromadb.PersistentClient(path=chroma_path)
+        collection = db.create_collection(name="test_vectordb_retrieval", metadata={"hnsw:space": "cosine"})
+
+        yield collection
+
+
+@pytest.fixture
 def project_dir_for_vectordb_node():
     with tempfile.TemporaryDirectory() as test_project_dir:
         sample_project_dir = os.path.join(resource_path, "sample_project")
         # copy & paste all folders and files in sample_project folder
         shutil.copytree(sample_project_dir, test_project_dir, dirs_exist_ok=True)
 
         chroma_path = os.path.join(test_project_dir, "resources", "chroma")
@@ -84,7 +95,22 @@
                     "This is a test" * 40000]
     new_metadata = [{'datetime': datetime.now()} for _ in range(2)]
     new_corpus_df = pd.DataFrame({"doc_id": new_doc_id, "contents": new_contents, "metadata": new_metadata})
     assert isinstance(embedding_model, OpenAIEmbedding)
     vectordb_ingest(ingested_vectordb, new_corpus_df, embedding_model)
 
     assert ingested_vectordb.count() == 7
+
+
+def mock_get_text_embedding_batch(self, texts, **kwargs):
+    return [[3.0, 4.1, 3.2] for _ in range(len(texts))]
+
+
+@patch.object(OpenAIEmbedding, 'get_text_embedding_batch', mock_get_text_embedding_batch)
+def test_long_ids_ingest(empty_chromadb):
+    embedding_model = OpenAIEmbedding()
+    content_df = pd.DataFrame({
+        'doc_id': [str(uuid.uuid4()) for _ in range(100_000)],
+        'contents': ['havertz' for _ in range(100_000)],
+        'metadata': [{'last_modified_datetime': datetime.now()} for _ in range(100_000)],
+    })
+    vectordb_ingest(empty_chromadb, content_df, embedding_model)
```

### Comparing `autorag-0.1.5/tests/autorag/schema/test_module_schema.py` & `autorag-0.1.6/tests/autorag/schema/test_module_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/schema/test_node_schema.py` & `autorag-0.1.6/tests/autorag/schema/test_node_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/test_cli.py` & `autorag-0.1.6/tests/autorag/test_cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/test_deploy.py` & `autorag-0.1.6/tests/autorag/test_deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/test_evaluator.py` & `autorag-0.1.6/tests/autorag/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/test_strategy.py` & `autorag-0.1.6/tests/autorag/test_strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/test_web.py` & `autorag-0.1.6/tests/autorag/test_web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/autorag/utils/test_util.py` & `autorag-0.1.6/tests/autorag/utils/test_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,22 @@
     assert find_contents[1] == ['banana']
 
     find_metadatas = fetch_contents(corpus_data, [['doc3', 'doc1'], ['doc2']], 'metadata')
     assert find_metadatas[0] == [{'last_modified_datetime': datetime(2022, 1, 3, 0, 0, 0)},
                                  {'last_modified_datetime': datetime(2022, 1, 1, 0, 0, 0)}]
     assert find_metadatas[1] == [{'last_modified_datetime': datetime(2022, 1, 2, 0, 0, 0)}]
 
+    find_empty = fetch_contents(corpus_data, [[], ['doc2']])
+    assert find_empty[0] == [None]
+    assert find_empty[1] == ['banana']
+
+    find_blank = fetch_contents(corpus_data, [[''], ['doc2']])
+    assert find_blank[0] == [None]
+    assert find_blank[1] == ['banana']
+
 
 def test_load_summary_file(summary_path):
     with pytest.raises(ValueError):
         load_summary_file(summary_path)
     df = load_summary_file(summary_path, ['best_module_params'])
     assert df.equals(summary_df)
```

### Comparing `autorag-0.1.5/tests/delete_tests.py` & `autorag-0.1.6/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/mock.py` & `autorag-0.1.6/tests/mock.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/README.md` & `autorag-0.1.6/tests/resources/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/corpus_data_sample.parquet` & `autorag-0.1.6/tests/resources/corpus_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/data_creation/raw_dir/sample1.txt` & `autorag-0.1.6/tests/resources/data_creation/raw_dir/sample1.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/data_creation/raw_dir/sample2.txt` & `autorag-0.1.6/tests/resources/data_creation/raw_dir/sample2.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/data_creation/raw_dir/sample3.txt` & `autorag-0.1.6/tests/resources/data_creation/raw_dir/sample3.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/full.yaml` & `autorag-0.1.6/tests/resources/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/qa_data_sample.parquet` & `autorag-0.1.6/tests/resources/qa_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/qa_test_data_sample.parquet` & `autorag-0.1.6/tests/resources/qa_test_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/config.yaml` & `autorag-0.1.6/tests/resources/result_project/0/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv` & `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/0/summary.csv` & `autorag-0.1.6/tests/resources/result_project/0/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/config.yaml` & `autorag-0.1.6/tests/resources/result_project/1/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/config.yaml` & `autorag-0.1.6/tests/resources/result_project/2/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.6/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/3/config.yaml` & `autorag-0.1.6/tests/resources/result_project/3/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/best.yaml` & `autorag-0.1.6/tests/resources/result_project/best.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/data/corpus.parquet` & `autorag-0.1.6/tests/resources/result_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/data/qa.parquet` & `autorag-0.1.6/tests/resources/result_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/resources/bm25.pkl` & `autorag-0.1.6/tests/resources/result_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin` & `autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin` & `autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/result_project/resources/chroma/chroma.sqlite3` & `autorag-0.1.6/tests/resources/result_project/resources/chroma/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/sample_contents_nqa.csv` & `autorag-0.1.6/tests/resources/sample_contents_nqa.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/sample_project/data/corpus.parquet` & `autorag-0.1.6/tests/resources/sample_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/sample_project/data/qa.parquet` & `autorag-0.1.6/tests/resources/sample_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/sample_project/resources/bm25.pkl` & `autorag-0.1.6/tests/resources/sample_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/simple.yaml` & `autorag-0.1.6/tests/resources/simple.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.5/tests/resources/test_bm25_retrieval.pkl` & `autorag-0.1.6/tests/resources/test_bm25_retrieval.pkl`

 * *Files identical despite different names*

