# Comparing `tmp/gloe-0.5.8.tar.gz` & `tmp/gloe-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gloe-0.5.8.tar", last modified: Thu Apr 25 20:56:00 2024, max compression
+gzip compressed data, was "gloe-0.5.9.tar", last modified: Sat Apr 27 17:21:17 2024, max compression
```

## Comparing `gloe-0.5.8.tar` & `gloe-0.5.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.292173 gloe-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-25 20:55:54.000000 gloe-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 20:55:54.000000 gloe-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-25 20:56:00.292173 gloe-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-04-25 20:55:54.000000 gloe-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.276173 gloe-0.5.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.280173 gloe-0.5.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.280173 gloe-0.5.8/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.280173 gloe-0.5.8/docs/source/_static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/assets/gloe-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/assets/gloe-logo-small.webp
--rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/assets/gloe-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/assets/graph_example.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.280173 gloe-0.5.8/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.284173 gloe-0.5.8/docs/source/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/api-reference/gloe.collection.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/api-reference/gloe.experimental.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/api-reference/gloe.utils.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/docutils.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.284173 gloe-0.5.8/docs/source/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/async-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/conditional-flows.md
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/ensurers.md
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/partial-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/plotting.md
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/utilities.md
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/limitations.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.284173 gloe-0.5.8/docs/source/pygments/
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/pygments/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/theory.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/_composition_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/_generic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/_plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/_transformer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/_typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/base_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/collection/_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/collection/_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/collection/_mapover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/conditional/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/conditional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/conditional/_conditioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/ensurer/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/ensurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/ensurer/_ensure.py
--rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/ensurer/_transformer_ensurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/experimental/_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.292173 gloe-0.5.8/gloe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-25 20:56:00.000000 gloe-0.5.8/gloe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-25 20:56:00.000000 gloe-0.5.8/gloe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:56:00.000000 gloe-0.5.8/gloe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 20:56:00.000000 gloe-0.5.8/gloe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 20:56:00.000000 gloe-0.5.8/gloe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-25 20:55:54.000000 gloe-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 20:56:00.292173 gloe-0.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.292173 gloe-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.292173 gloe-0.5.8/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/lib/conditioners.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/lib/ensurers.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/lib/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_conditioner_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_ensurer.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.147554 gloe-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-27 17:21:10.000000 gloe-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 17:21:10.000000 gloe-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-27 17:21:17.147554 gloe-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-04-27 17:21:10.000000 gloe-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.131554 gloe-0.5.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.135554 gloe-0.5.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.135554 gloe-0.5.9/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.135554 gloe-0.5.9/docs/source/_static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/_static/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/_static/assets/gloe-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/_static/assets/gloe-logo-small.webp
+-rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/_static/assets/gloe-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/_static/assets/graph_example.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/_static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.135554 gloe-0.5.9/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.135554 gloe-0.5.9/docs/source/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/api-reference/gloe.collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/api-reference/gloe.experimental.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/api-reference/gloe.utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/docutils.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.139554 gloe-0.5.9/docs/source/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/getting-started/async-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/getting-started/conditional-flows.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/getting-started/ensurers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/getting-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/getting-started/partial-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/getting-started/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/getting-started/transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/getting-started/utilities.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/limitations.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.139554 gloe-0.5.9/docs/source/pygments/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/pygments/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-27 17:21:10.000000 gloe-0.5.9/docs/source/theory.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.139554 gloe-0.5.9/gloe/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/_composition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/_generic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/_plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/_transformer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/_typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/base_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.143554 gloe-0.5.9/gloe/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/collection/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/collection/_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/collection/_mapover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.143554 gloe-0.5.9/gloe/conditional/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/conditional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/conditional/_conditioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.143554 gloe-0.5.9/gloe/ensurer/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/ensurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/ensurer/_ensure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8754 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/ensurer/_transformer_ensurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.143554 gloe-0.5.9/gloe/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.143554 gloe-0.5.9/gloe/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/experimental/_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-27 17:21:10.000000 gloe-0.5.9/gloe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.147554 gloe-0.5.9/gloe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-27 17:21:17.000000 gloe-0.5.9/gloe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-27 17:21:17.000000 gloe-0.5.9/gloe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:21:17.000000 gloe-0.5.9/gloe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-27 17:21:17.000000 gloe-0.5.9/gloe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-27 17:21:17.000000 gloe-0.5.9/gloe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-27 17:21:10.000000 gloe-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 17:21:17.147554 gloe-0.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.147554 gloe-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:17.147554 gloe-0.5.9/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/lib/conditioners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/lib/ensurers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/lib/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/test_async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/test_conditioner_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/test_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/test_transformer_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/test_transformer_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/test_transformer_ensurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/test_transformer_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/test_transformer_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/test_transformer_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-27 17:21:10.000000 gloe-0.5.9/tests/test_transformer_utils.py
```

### Comparing `gloe-0.5.8/LICENSE` & `gloe-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/PKG-INFO` & `gloe-0.5.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.8
+Version: 0.5.9
 Summary: Gloe (pronounced /ɡloʊ/, like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions~=4.7
 Requires-Dist: networkx~=3.1
 Provides-Extra: plot
 Requires-Dist: pygraphviz>=1.11; extra == "plot"
 Provides-Extra: types
```

### Comparing `gloe-0.5.8/README.md` & `gloe-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/_static/assets/favicon.ico` & `gloe-0.5.9/docs/source/_static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/_static/assets/gloe-logo-small.png` & `gloe-0.5.9/docs/source/_static/assets/gloe-logo-small.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/_static/assets/gloe-logo-small.webp` & `gloe-0.5.9/docs/source/_static/assets/gloe-logo-small.webp`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/_static/assets/gloe-logo.png` & `gloe-0.5.9/docs/source/_static/assets/gloe-logo.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/_static/assets/graph_example.jpeg` & `gloe-0.5.9/docs/source/_static/assets/graph_example.jpeg`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/_templates/page.html` & `gloe-0.5.9/docs/source/_templates/page.html`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/api-reference/index.md` & `gloe-0.5.9/docs/source/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/conf.py` & `gloe-0.5.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/getting-started/async-transformers.md` & `gloe-0.5.9/docs/source/getting-started/async-transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/getting-started/conditional-flows.md` & `gloe-0.5.9/docs/source/getting-started/conditional-flows.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/getting-started/ensurers.md` & `gloe-0.5.9/docs/source/getting-started/ensurers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/getting-started/partial-transformers.md` & `gloe-0.5.9/docs/source/getting-started/partial-transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/getting-started/plotting.md` & `gloe-0.5.9/docs/source/getting-started/plotting.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/getting-started/transformers.md` & `gloe-0.5.9/docs/source/getting-started/transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/getting-started/utilities.md` & `gloe-0.5.9/docs/source/getting-started/utilities.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/index.md` & `gloe-0.5.9/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/limitations.md` & `gloe-0.5.9/docs/source/limitations.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/pygments/styles.py` & `gloe-0.5.9/docs/source/pygments/styles.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/docs/source/theory.md` & `gloe-0.5.9/docs/source/theory.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/gloe/__init__.py` & `gloe-0.5.9/gloe/__init__.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/gloe/_composition_utils.py` & `gloe-0.5.9/gloe/_composition_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import types
 from inspect import Signature
 from types import GenericAlias
-from typing import TypeVar, Any, cast, Optional
+from typing import TypeVar, Any, cast, Optional, Union
 
 from gloe._plotting_utils import PlottingSettings, NodeType
 from gloe.async_transformer import AsyncTransformer
 from gloe.base_transformer import BaseTransformer
 from gloe.transformers import Transformer
 from gloe._typing_utils import _match_types, _specify_types
 from gloe.exceptions import UnsupportedTransformerArgException
@@ -74,15 +74,15 @@
             return _resolve_serial_connection_signatures(
                 transformer2, generic_vars, signature2
             )
 
         def __len__(self):
             return len(transformer1) + len(transformer2)
 
-    new_transformer: BaseTransformer | None = None
+    new_transformer: Optional[BaseTransformer] = None
     if is_transformer(transformer1) and is_transformer(_transformer2):
 
         class NewTransformer1(BaseNewTransformer, Transformer[_In, _NextOut]):
             def transform(self, data: _In) -> _NextOut:
                 transformer2_call = transformer2.__call__
                 transformer1_call = transformer1.__call__
                 transformed = transformer2_call(transformer1_call(data))
@@ -244,15 +244,15 @@
     new_transformer._plotting_settings = PlottingSettings(node_type=NodeType.Convergent)
 
     return new_transformer
 
 
 def _compose_nodes(
     current: BaseTransformer,
-    next_node: tuple | BaseTransformer,
+    next_node: Union[tuple, BaseTransformer],
 ):
     if issubclass(type(current), BaseTransformer):
         if issubclass(type(next_node), BaseTransformer):
             return _compose_serial(current, next_node)
         elif type(next_node) is tuple:
             is_all_base_transformers = all(
                 issubclass(type(next_transformer), BaseTransformer)
```

### Comparing `gloe-0.5.8/gloe/_generic_types.py` & `gloe-0.5.9/gloe/_generic_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import TypeVar, TypeAlias, Union
+from typing import TypeVar, Union
+from typing_extensions import TypeAlias
 
 from gloe.base_transformer import BaseTransformer
 from gloe.async_transformer import AsyncTransformer
 
 _I = TypeVar("_I")
 _O = TypeVar("_O", covariant=True)
```

### Comparing `gloe-0.5.8/gloe/_plotting_utils.py` & `gloe-0.5.9/gloe/_plotting_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,25 +20,22 @@
     is_async: bool = False
     parent_id: Optional[str] = None
 
 
 def export_dot_props(settings: PlottingSettings, instance_id: UUID) -> dict[str, Any]:
     node_props: dict[str, Any] = {"shape": "box"}
 
-    match settings.node_type:
-        case NodeType.Condition:
-            node_props = {"shape": "diamond", "style": "filled", "port": "n"}
-        case NodeType.Convergent:
-            node_props = {
-                "shape": "diamond",
-                "width": 0.5,
-                "height": 0.5,
-            }
-        case _:
-            pass
+    if settings.node_type == NodeType.Condition:
+        node_props = {"shape": "diamond", "style": "filled", "port": "n"}
+    elif settings.node_type == NodeType.Convergent:
+        node_props = {
+            "shape": "diamond",
+            "width": 0.5,
+            "height": 0.5,
+        }
 
     if settings.has_children:
         node_props = node_props | {
             "parent_id": instance_id,
             "bounding_box": True,
             "box_label": "mapping",
         }
```

### Comparing `gloe-0.5.8/gloe/_transformer_utils.py` & `gloe-0.5.9/gloe/_transformer_utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/gloe/_typing_utils.py` & `gloe-0.5.9/gloe/_typing_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,19 +39,23 @@
 def _format_return_annotation(
     return_annotation, generic_input_param, input_annotation
 ) -> str:
     if isinstance(return_annotation, str):
         return return_annotation
     if isinstance(return_annotation, tuple):
         return _format_tuple(return_annotation, generic_input_param, input_annotation)
-    if return_annotation.__name__ in {"tuple", "Tuple"}:
+    return_name = getattr(return_annotation, "__name__", None)
+    if return_name is None:
+        return_name = getattr(return_annotation, "_name", None)
+
+    if return_name in {"tuple", "Tuple"}:
         return _format_tuple(
             return_annotation.__args__, generic_input_param, input_annotation
         )
-    if return_annotation.__name__ in {"Union"}:
+    if return_name in {"Union"}:
         return _format_union(
             return_annotation.__args__, generic_input_param, input_annotation
         )
     if (
         type(return_annotation) is GenericAlias
     ):  # _GenericAlias must be investigated too
         return _format_generic_alias(
```

### Comparing `gloe-0.5.8/gloe/async_transformer.py` & `gloe-0.5.9/gloe/async_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import abstractmethod
 from inspect import Signature
-from typing import TypeVar, overload, cast, Callable, Generic
+from typing import TypeVar, overload, cast, Callable, Generic, Optional
 
 from typing_extensions import Self
 
 from gloe._plotting_utils import PlottingSettings, NodeType
 from gloe._transformer_utils import catch_transformer_exception
 from gloe.base_transformer import BaseTransformer
 
@@ -53,15 +53,15 @@
             f" -> ({type(self).__name__})"
             f" -> {self.output_annotation}"
         )
 
     async def __call__(self, data: _In) -> _Out:
         transform_exception = None
 
-        transformed: _Out | None = None
+        transformed: Optional[_Out] = None
         try:
             transformed = await self.transform_async(data)
         except Exception as exception:
             transform_exception = catch_transformer_exception(exception, self)
 
         if transform_exception is not None:
             raise transform_exception.internal_exception
@@ -69,15 +69,15 @@
         if type(transformed) is not None:
             return cast(_Out, transformed)
 
         raise NotImplementedError  # pragma: no cover
 
     def copy(
         self,
-        transform: Callable[[Self, _In], _Out] | None = None,
+        transform: Optional[Callable[[Self, _In], _Out]] = None,
         regenerate_instance_id: bool = False,
     ) -> Self:
         return self._copy(transform, regenerate_instance_id, "transform_async")
 
     @overload
     def __rshift__(
         self, next_node: BaseTransformer[_Out, _NextOut]
```

### Comparing `gloe-0.5.8/gloe/base_transformer.py` & `gloe-0.5.9/gloe/base_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
     Generic,
     TypeVar,
     Union,
     cast,
     Iterable,
     get_args,
     get_origin,
-    TypeAlias,
     Type,
+    Optional,
 )
 from uuid import UUID
 from itertools import groupby
 
-from typing_extensions import Self
+from typing_extensions import Self, TypeAlias
 
 from gloe._plotting_utils import PlottingSettings, NodeType, export_dot_props
 from gloe._typing_utils import _format_return_annotation
 
 __all__ = ["BaseTransformer", "TransformerException", "PreviousTransformer"]
 
 _NextOut = TypeVar("_NextOut")
@@ -57,15 +57,15 @@
 
 
 class TransformerException(Exception):
     def __init__(
         self,
         internal_exception: Union["TransformerException", Exception],
         raiser_transformer: "BaseTransformer",
-        message: str | None = None,
+        message: Union[str, None] = None,
     ):
         self._internal_exception = internal_exception
         self.raiser_transformer = raiser_transformer
         self._traceback = internal_exception.__traceback__
         internal_exception.__cause__ = self
         super().__init__(message)
 
@@ -133,15 +133,15 @@
     def __eq__(self, other):
         if isinstance(other, BaseTransformer):
             return self.id == other.id
         return NotImplemented
 
     def _copy(
         self: Self,
-        transform: Callable[[Self, _In], _Out] | None = None,
+        transform: Optional[Callable[[Self, _In], _Out]] = None,
         regenerate_instance_id: bool = False,
         transform_method: str = "transform",
     ) -> Self:
         copied: Self = copy.copy(self)
 
         func_type = types.MethodType
         if transform is not None:
@@ -164,15 +164,15 @@
             child.copy(regenerate_instance_id=True) for child in self.children
         ]
 
         return copied
 
     def copy(
         self: Self,
-        transform: Callable[[Self, _In], _Out] | None = None,
+        transform: Optional[Callable[[Self, _In], _Out]] = None,
         regenerate_instance_id: bool = False,
     ) -> Self:
         return self._copy(transform, regenerate_instance_id)
 
     @property
     def graph_nodes(self) -> dict[UUID, "BaseTransformer"]:
         nodes = {self.instance_id: self}
```

### Comparing `gloe-0.5.8/gloe/collection/_filter.py` & `gloe-0.5.9/gloe/collection/_filter.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/gloe/collection/_map.py` & `gloe-0.5.9/gloe/collection/_map.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/gloe/collection/_mapover.py` & `gloe-0.5.9/gloe/collection/_mapover.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/gloe/conditional/_conditioner.py` & `gloe-0.5.9/gloe/conditional/_conditioner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
+import sys
 from dataclasses import dataclass
 from inspect import Signature
-from types import GenericAlias, UnionType
-from typing import Callable, Generic, Optional, TypeVar, Union
+from types import GenericAlias
+
+if sys.version_info >= (3, 10):
+    from types import UnionType
+from typing import (
+    Callable,
+    Generic,
+    Optional,
+    TypeVar,
+    Union,
+)
 
 from typing_extensions import Self
 
 from gloe._plotting_utils import PlottingSettings, NodeType
 from gloe.transformers import Transformer
 from gloe.utils import forget
 
@@ -51,22 +61,34 @@
 
     def signature(self) -> Signature:
         else_signature: Signature = self.else_transformer.signature()
         return_signature: list[Signature] = [
             impl.then_transformer.signature().return_annotation
             for impl in self.implications
         ] + [else_signature.return_annotation]
-        new_signature = else_signature.replace(
-            return_annotation=GenericAlias(UnionType, tuple(return_signature))
-        )
+
+        if sys.version_info >= (3, 10):
+            new_signature = else_signature.replace(
+                return_annotation=GenericAlias(
+                    UnionType,
+                    tuple(return_signature),
+                )
+            )
+        else:
+            new_signature = else_signature.replace(
+                return_annotation=GenericAlias(
+                    Union,  # type: ignore
+                    tuple(return_signature),
+                )
+            )
         return new_signature
 
     def copy(
         self,
-        transform: Callable[[Self, In], Union[ThenOut, ElseOut]] | None = None,
+        transform: Union[Callable[[Self, In], Union[ThenOut, ElseOut]], None] = None,
         regenerate_instance_id: bool = False,
     ) -> Self:
         copied: Self = super().copy(transform, regenerate_instance_id)
         copied.implications = [
             _Implication(
                 impl.condition, impl.then_transformer.copy(regenerate_instance_id=True)
             )
@@ -170,15 +192,15 @@
             )
 
     Args:
         condition: callable returning a boolean.
         name: optional argument that adds a label to condition node during plotting.
     """
 
-    def __init__(self, condition: Callable[[In], bool], name: str | None = None):
+    def __init__(self, condition: Callable[[In], bool], name: Union[str, None] = None):
         super().__init__()
         self._condition = condition
         self._name: str = name or condition.__name__
 
     def Then(
         self, next_transformer: Transformer[In, ThenOut]
     ) -> _IfThen[In, ThenOut, ThenOut]:
```

### Comparing `gloe-0.5.8/gloe/ensurer/_ensure.py` & `gloe-0.5.9/gloe/ensurer/_ensure.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/gloe/ensurer/_transformer_ensurer.py` & `gloe-0.5.9/gloe/ensurer/_transformer_ensurer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 from abc import abstractmethod, ABC
 from types import FunctionType
-from typing import Any, Callable, Generic, ParamSpec, Sequence, TypeVar, cast, overload
+from typing import Any, Callable, Generic, Sequence, TypeVar, cast, overload
+from typing_extensions import ParamSpec
 
 from gloe.exceptions import UnsupportedTransformerArgException
 from gloe.async_transformer import AsyncTransformer
 from gloe.transformers import Transformer
 
 _T = TypeVar("_T")
 _S = TypeVar("_S")
```

### Comparing `gloe-0.5.8/gloe/experimental/_bridge.py` & `gloe-0.5.9/gloe/experimental/_bridge.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/gloe/functional.py` & `gloe-0.5.9/gloe/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import inspect
 import warnings
 from inspect import Signature
 from types import FunctionType
 from typing import (
     Callable,
-    Concatenate,
-    ParamSpec,
     TypeVar,
     cast,
     Awaitable,
 )
+from typing_extensions import Concatenate, ParamSpec
 
 from gloe.async_transformer import AsyncTransformer
 from gloe.transformers import Transformer
 
 __all__ = [
     "transformer",
     "partial_transformer",
```

### Comparing `gloe-0.5.8/gloe/transformers.py` & `gloe-0.5.9/gloe/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC, abstractmethod
 from inspect import Signature
 
-from typing import TypeVar, overload, cast, TypeAlias
+from typing import TypeVar, overload, cast, Optional
+from typing_extensions import TypeAlias
 
 from gloe.async_transformer import AsyncTransformer
 from gloe._transformer_utils import catch_transformer_exception
 from gloe.base_transformer import BaseTransformer
 
 from gloe._generic_types import (
     AsyncNext2,
@@ -69,15 +70,15 @@
             f" -> ({type(self).__name__})"
             f" -> {self.output_annotation}"
         )
 
     def __call__(self, data: _I) -> _O:
         transform_exception = None
 
-        transformed: _O | None = None
+        transformed: Optional[_O] = None
         try:
             transformed = self.transform(data)
         except Exception as exception:
             transform_exception = catch_transformer_exception(exception, self)
 
         if transform_exception is not None:
             raise transform_exception.internal_exception
```

### Comparing `gloe-0.5.8/gloe/utils.py` & `gloe-0.5.9/gloe/utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/gloe.egg-info/PKG-INFO` & `gloe-0.5.9/gloe.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.8
+Version: 0.5.9
 Summary: Gloe (pronounced /ɡloʊ/, like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions~=4.7
 Requires-Dist: networkx~=3.1
 Provides-Extra: plot
 Requires-Dist: pygraphviz>=1.11; extra == "plot"
 Provides-Extra: types
```

### Comparing `gloe-0.5.8/gloe.egg-info/SOURCES.txt` & `gloe-0.5.9/gloe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/pyproject.toml` & `gloe-0.5.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gloe"
-version = "0.5.8"
+version = "0.5.9"
 authors = [
   { name="Samir Braga", email="samirchavess@gmail.com" },
 ]
 description = "Gloe (pronounced /ɡloʊ/, like \"glow\") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

### Comparing `gloe-0.5.8/tests/lib/ensurers.py` & `gloe-0.5.9/tests/lib/ensurers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/tests/lib/transformers.py` & `gloe-0.5.9/tests/lib/transformers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/tests/test_async_transformer.py` & `gloe-0.5.9/tests/test_async_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/tests/test_conditioner_transformer.py` & `gloe-0.5.9/tests/test_conditioner_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/tests/test_function_transformer.py` & `gloe-0.5.9/tests/test_function_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/tests/test_transformer_bridge.py` & `gloe-0.5.9/tests/test_transformer_bridge.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/tests/test_transformer_collections.py` & `gloe-0.5.9/tests/test_transformer_collections.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/tests/test_transformer_ensurer.py` & `gloe-0.5.9/tests/test_transformer_ensurer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/tests/test_transformer_graph.py` & `gloe-0.5.9/tests/test_transformer_graph.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.8/tests/test_transformer_types.py` & `gloe-0.5.9/tests/test_transformer_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import os
 import unittest
 from pathlib import Path
-from typing import TypeVar, Iterable
+from typing import TypeVar, Iterable, Union
 from typing_extensions import assert_type
 
 from tests.lib.conditioners import if_not_zero, if_is_even
 from tests.lib.ensurers import is_even, same_value, same_value_int, is_greater_than_10
 from tests.lib.transformers import (
     square,
     square_root,
@@ -112,26 +112,28 @@
 
         assert_type(conditioned_graph, Transformer[float, float])
 
         conditioned_graph2 = (
             square >> square_root >> if_not_zero.Then(to_string).Else(square)
         )
 
-        assert_type(conditioned_graph2, Transformer[float, str | float])
+        assert_type(conditioned_graph2, Transformer[float, Union[str, float]])
 
     def _test_chained_condition_flow_types(self):
         """
         Test the most simple transformer typing
         """
 
         chained_conditions_graph = (
             if_is_even.Then(square).ElseIf(lambda x: x < 10).Then(to_string).ElseNone()
         )
 
-        assert_type(chained_conditions_graph, Transformer[float, float | str | None])
+        assert_type(
+            chained_conditions_graph, Transformer[float, Union[float, str, None]]
+        )
 
     def _test_partial_transformer(self):
         """
         Test the curried transformer typing
         """
 
         log2 = logarithm(base=2)
```

### Comparing `gloe-0.5.8/tests/test_transformer_utils.py` & `gloe-0.5.9/tests/test_transformer_utils.py`

 * *Files identical despite different names*

