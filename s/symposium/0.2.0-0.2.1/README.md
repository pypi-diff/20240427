# Comparing `tmp/symposium-0.2.0.tar.gz` & `tmp/symposium-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symposium-0.2.0.tar", last modified: Thu Mar 21 15:09:53 2024, max compression
+gzip compressed data, was "symposium-0.2.1.tar", last modified: Sat Apr 27 16:20:26 2024, max compression
```

## Comparing `symposium-0.2.0.tar` & `symposium-0.2.1.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-03-21 15:09:53.546624 symposium-0.2.0/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2023-09-13 23:21:39.000000 symposium-0.2.0/LICENSE
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)     8832 2024-03-21 15:09:53.546624 symposium-0.2.0/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     7654 2024-03-21 14:13:57.000000 symposium-0.2.0/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1025 2024-03-21 15:08:13.000000 symposium-0.2.0/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-03-21 15:09:53.546624 symposium-0.2.0/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-03-21 15:09:53.518617 symposium-0.2.0/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-03-21 15:09:53.538622 symposium-0.2.0/src/manual_testing/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1119 2024-03-21 15:06:52.000000 symposium-0.2.0/src/manual_testing/anthropic_native_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      959 2024-03-21 15:06:52.000000 symposium-0.2.0/src/manual_testing/anthropic_rest_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1997 2024-03-20 12:18:54.000000 symposium-0.2.0/src/manual_testing/gemini_rest_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      771 2024-03-16 13:50:13.000000 symposium-0.2.0/src/manual_testing/openai_native_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2695 2024-03-20 00:25:32.000000 symposium-0.2.0/src/manual_testing/openai_rest_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2387 2024-03-20 14:26:20.000000 symposium-0.2.0/src/manual_testing/palm_rest_test.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-03-21 15:09:53.538622 symposium-0.2.0/src/symposium/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-13 23:21:39.000000 symposium-0.2.0/src/symposium/__init__.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-03-21 15:09:53.538622 symposium-0.2.0/src/symposium/adapters/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-08 23:53:58.000000 symposium-0.2.0/src/symposium/adapters/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3236 2024-03-21 14:59:26.000000 symposium-0.2.0/src/symposium/adapters/anth.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2012 2024-03-20 00:25:32.000000 symposium-0.2.0/src/symposium/adapters/gem_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      245 2024-03-19 23:38:45.000000 symposium-0.2.0/src/symposium/adapters/oai_native.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2799 2024-03-20 00:01:26.000000 symposium-0.2.0/src/symposium/adapters/oai_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1552 2024-03-20 13:30:26.000000 symposium-0.2.0/src/symposium/adapters/plm_rest.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-03-21 15:09:53.542623 symposium-0.2.0/src/symposium/connectors/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      753 2024-03-15 20:42:25.000000 symposium-0.2.0/src/symposium/connectors/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4825 2024-03-21 14:50:52.000000 symposium-0.2.0/src/symposium/connectors/anthropic_native.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4634 2024-03-21 14:48:40.000000 symposium-0.2.0/src/symposium/connectors/anthropic_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-02 14:53:27.000000 symposium-0.2.0/src/symposium/connectors/bedrock.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3406 2024-01-03 15:06:20.000000 symposium-0.2.0/src/symposium/connectors/brcloud.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      766 2024-03-06 19:20:16.000000 symposium-0.2.0/src/symposium/connectors/gemini_google.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6347 2024-03-20 00:25:32.000000 symposium-0.2.0/src/symposium/connectors/gemini_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6715 2023-10-24 22:57:19.000000 symposium-0.2.0/src/symposium/connectors/govert.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      896 2023-10-29 23:20:06.000000 symposium-0.2.0/src/symposium/connectors/hugface.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6529 2024-03-16 13:50:13.000000 symposium-0.2.0/src/symposium/connectors/openai_native.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)    11100 2024-03-20 00:08:34.000000 symposium-0.2.0/src/symposium/connectors/openai_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1311 2024-03-03 14:20:15.000000 symposium-0.2.0/src/symposium/connectors/palm_google.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6420 2024-03-20 13:47:08.000000 symposium-0.2.0/src/symposium/connectors/palm_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-11-16 19:25:23.000000 symposium-0.2.0/src/symposium/connectors/together.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-02 14:53:27.000000 symposium-0.2.0/src/symposium/connectors/vertex.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6420 2023-12-08 20:56:28.000000 symposium-0.2.0/src/symposium/connectors/vertrest.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-03-21 15:09:53.542623 symposium-0.2.0/src/symposium/recorders/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      428 2023-09-21 19:23:09.000000 symposium-0.2.0/src/symposium/recorders/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4593 2023-09-21 19:23:09.000000 symposium-0.2.0/src/symposium/recorders/githublog.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-03-21 15:09:53.542623 symposium-0.2.0/src/symposium/templates/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-21 19:23:09.000000 symposium-0.2.0/src/symposium/templates/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      311 2023-09-21 19:23:09.000000 symposium-0.2.0/src/symposium/templates/four_hypotheses.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      285 2023-09-26 18:39:22.000000 symposium-0.2.0/src/symposium/templates/one_thread.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3783 2023-09-21 19:23:09.000000 symposium-0.2.0/src/symposium/templates/sentence.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2834 2023-09-21 19:23:09.000000 symposium-0.2.0/src/symposium/templates/three_branch.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-21 19:23:09.000000 symposium-0.2.0/src/symposium/templates/two_branch.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-03-21 15:09:53.542623 symposium-0.2.0/src/symposium/util/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-19 23:31:57.000000 symposium-0.2.0/src/symposium/util/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2407 2024-03-19 23:38:45.000000 symposium-0.2.0/src/symposium/util/xml_tags.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-03-21 15:09:53.542623 symposium-0.2.0/src/symposium.egg-info/
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)     8832 2024-03-21 15:09:53.000000 symposium-0.2.0/src/symposium.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1873 2024-03-21 15:09:53.000000 symposium-0.2.0/src/symposium.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-03-21 15:09:53.000000 symposium-0.2.0/src/symposium.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      262 2024-03-21 15:09:53.000000 symposium-0.2.0/src/symposium.egg-info/requires.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       31 2024-03-21 15:09:53.000000 symposium-0.2.0/src/symposium.egg-info/top_level.txt
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-03-21 15:09:53.542623 symposium-0.2.0/src/tests/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        0 2024-03-05 19:48:52.000000 symposium-0.2.0/src/tests/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      847 2024-03-15 20:42:25.000000 symposium-0.2.0/src/tests/test_anthropic.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1273 2024-03-06 18:23:43.000000 symposium-0.2.0/src/tests/test_anthropic_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      404 2024-03-05 20:37:21.000000 symposium-0.2.0/src/tests/test_gemini_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      470 2024-03-15 20:42:25.000000 symposium-0.2.0/src/tests/test_openai.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      305 2024-03-05 20:00:36.000000 symposium-0.2.0/src/tests/test_openai_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1884 2024-03-06 18:49:23.000000 symposium-0.2.0/src/tests/test_palm_rest.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.939495 symposium-0.2.1/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2023-09-13 23:21:39.000000 symposium-0.2.1/LICENSE
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)     9081 2024-04-27 16:20:26.939495 symposium-0.2.1/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     7903 2024-04-14 20:40:51.000000 symposium-0.2.1/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1025 2024-04-01 00:21:09.000000 symposium-0.2.1/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-04-27 16:20:26.939495 symposium-0.2.1/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.927495 symposium-0.2.1/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.931495 symposium-0.2.1/src/manual_testing/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1119 2024-03-21 15:06:52.000000 symposium-0.2.1/src/manual_testing/anthropic_native_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      984 2024-03-31 22:54:55.000000 symposium-0.2.1/src/manual_testing/anthropic_rest_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1997 2024-03-20 12:18:54.000000 symposium-0.2.1/src/manual_testing/gemini_rest_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2723 2024-04-27 16:17:06.000000 symposium-0.2.1/src/manual_testing/groq_rest_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      771 2024-03-16 13:50:13.000000 symposium-0.2.1/src/manual_testing/openai_native_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2695 2024-03-20 00:25:32.000000 symposium-0.2.1/src/manual_testing/openai_rest_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2387 2024-03-20 14:26:20.000000 symposium-0.2.1/src/manual_testing/palm_rest_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      385 2024-04-09 18:06:23.000000 symposium-0.2.1/src/manual_testing/yaml_config.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.931495 symposium-0.2.1/src/symposium/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-13 23:21:39.000000 symposium-0.2.1/src/symposium/__init__.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.931495 symposium-0.2.1/src/symposium/adapters/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-08 23:53:58.000000 symposium-0.2.1/src/symposium/adapters/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3226 2024-03-31 22:54:55.000000 symposium-0.2.1/src/symposium/adapters/anth.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2012 2024-03-20 00:25:32.000000 symposium-0.2.1/src/symposium/adapters/gem_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2796 2024-04-27 16:07:01.000000 symposium-0.2.1/src/symposium/adapters/grq_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      245 2024-03-19 23:38:45.000000 symposium-0.2.1/src/symposium/adapters/oai_native.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2799 2024-03-20 00:01:26.000000 symposium-0.2.1/src/symposium/adapters/oai_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1552 2024-03-20 13:30:26.000000 symposium-0.2.1/src/symposium/adapters/plm_rest.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.935495 symposium-0.2.1/src/symposium/connectors/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      753 2024-03-15 20:42:25.000000 symposium-0.2.1/src/symposium/connectors/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4825 2024-03-21 14:50:52.000000 symposium-0.2.1/src/symposium/connectors/anthropic_native.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4634 2024-03-31 22:50:13.000000 symposium-0.2.1/src/symposium/connectors/anthropic_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-02 14:53:27.000000 symposium-0.2.1/src/symposium/connectors/bedrock.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3406 2024-01-03 15:06:20.000000 symposium-0.2.1/src/symposium/connectors/brcloud.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      766 2024-03-06 19:20:16.000000 symposium-0.2.1/src/symposium/connectors/gemini_google.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6347 2024-03-20 00:25:32.000000 symposium-0.2.1/src/symposium/connectors/gemini_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6715 2023-10-24 22:57:19.000000 symposium-0.2.1/src/symposium/connectors/govert.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4139 2024-04-27 16:17:06.000000 symposium-0.2.1/src/symposium/connectors/groq_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      896 2023-10-29 23:20:06.000000 symposium-0.2.1/src/symposium/connectors/hugface.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6529 2024-03-16 13:50:13.000000 symposium-0.2.1/src/symposium/connectors/openai_native.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)    11100 2024-03-20 00:08:34.000000 symposium-0.2.1/src/symposium/connectors/openai_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1311 2024-03-03 14:20:15.000000 symposium-0.2.1/src/symposium/connectors/palm_google.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6420 2024-03-20 13:47:08.000000 symposium-0.2.1/src/symposium/connectors/palm_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-11-16 19:25:23.000000 symposium-0.2.1/src/symposium/connectors/together.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-02 14:53:27.000000 symposium-0.2.1/src/symposium/connectors/vertex.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6420 2023-12-08 20:56:28.000000 symposium-0.2.1/src/symposium/connectors/vertrest.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.935495 symposium-0.2.1/src/symposium/recorders/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      428 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/recorders/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4591 2024-04-12 12:32:29.000000 symposium-0.2.1/src/symposium/recorders/githublog.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.939495 symposium-0.2.1/src/symposium/templates/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/templates/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      311 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/templates/four_hypotheses.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      285 2023-09-26 18:39:22.000000 symposium-0.2.1/src/symposium/templates/one_thread.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3783 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/templates/sentence.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2834 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/templates/three_branch.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/templates/two_branch.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.939495 symposium-0.2.1/src/symposium/util/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-19 23:31:57.000000 symposium-0.2.1/src/symposium/util/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2407 2024-03-19 23:38:45.000000 symposium-0.2.1/src/symposium/util/xml_tags.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.939495 symposium-0.2.1/src/symposium.egg-info/
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)     9081 2024-04-27 16:20:26.000000 symposium-0.2.1/src/symposium.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2017 2024-04-27 16:20:26.000000 symposium-0.2.1/src/symposium.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-04-27 16:20:26.000000 symposium-0.2.1/src/symposium.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      262 2024-04-27 16:20:26.000000 symposium-0.2.1/src/symposium.egg-info/requires.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       31 2024-04-27 16:20:26.000000 symposium-0.2.1/src/symposium.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.939495 symposium-0.2.1/src/tests/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        0 2024-03-05 19:48:52.000000 symposium-0.2.1/src/tests/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      847 2024-03-15 20:42:25.000000 symposium-0.2.1/src/tests/test_anthropic.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1273 2024-03-06 18:23:43.000000 symposium-0.2.1/src/tests/test_anthropic_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      404 2024-03-05 20:37:21.000000 symposium-0.2.1/src/tests/test_gemini_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      470 2024-03-15 20:42:25.000000 symposium-0.2.1/src/tests/test_openai.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      305 2024-03-05 20:00:36.000000 symposium-0.2.1/src/tests/test_openai_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1884 2024-03-06 18:49:23.000000 symposium-0.2.1/src/tests/test_palm_rest.py
```

### Comparing `symposium-0.2.0/LICENSE` & `symposium-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/PKG-INFO` & `symposium-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symposium
-Version: 0.2.0
+Version: 0.2.1
 Summary: Interaction of multiple language models
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/symposium
 Project-URL: Bug Tracker, https://github.com/multilogue/sumposium/issues
 Keywords: symposium,conversations,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,45 +33,47 @@
 ## Unification
 One of the motivations for this package was the need in a unified format for messaging language models, which is particularly useful if you are going to experiment with interactions between them.
 
 The unified standard used by this package is as follows.
 ### 'System' messages
 ```python
 messages = [
-    {"role": "world",   "name": "openai",   "content": "Be an Abstract Intellect."}
+    {"role": "world", "name": "openai", "content": "Be an Antagonist."}
 ]
 ```
 Name field should be set to 'openai', 'anthropic', 'google_gemini' or 'google_palm'.
 For the 'anthropic' name, the last 
 'system' message will be used as the 'system' parameter in the request. For palm_messages v1beta3 format this message will be used in the 'context' parameter.
 ### 'User' messages
 ```python
 messages = [
-    {"role": "human",   "name": "alex",     "content": "Let's discuss human nature."}
+    {"role": "human", "name": "Alex", "content": "Let's discuss human nature."}
 ]
 ```
 The utility functions stored in the `adapters` sub-package transform incoming and outgoing messages of particular model from this format to a model-specific format and back from the format of its' response to the following output format. This includes the text synthesis with older (but in)
 ## Output format
 The unified standard used by this package is:
 ```python
 message = {
-    "role": "machine",   "name": "claude",     "content": " ... ", 
+    "role": "machine", "name": "claude",  
+    "content": " ... ", 
     "tags": [{}],   # optional, if in the response, then returned
-    "other": [{}]   # optional, for n > 1
+    "other": [{}]   # optional, if n > 1
 }
 ```
-Name field will be set to 'chatgpt', 'claude', 'gemini' or 'palm'.<br>
+`name` field will be set to 'chatgpt', 'claude', 'gemini' or 'palm'.<br>
 Tags are extracted from the text and put into a list. The placeholder for the tags is: (tag_name).<br>
 If there are more than one response, the other field will contain the list of the rest (transformed too).
 ## Anthropic
 There are two ways of interaction with Anthropic API, through the REST API and through the native Anthropic Python library with 'client'. If you don't want any dependencies (and uncertainty) use `anthropic_rest` connector. If you want to install this dependency do `pip install symposium[anthropic_native]`.
 #### Messages
 REST version:
 ```python
 from symposium.connectors import anthropic_rest as ant
+
 messages = [
     {"role": "human", "name": "alex", "content": "Can we change human nature?"}
 ]
 kwargs = {
     "model":                "claude-3-sonnet-20240229",
     "system":               "answer concisely",
     # "messages":             [],
@@ -83,14 +85,15 @@
     "top_p":                0.5
 }
 response = ant.claud_message(messages,**kwargs)
 ```
 Native version:
 ```python
 from symposium.connectors import anthropic_native as ant
+
 ant_client = ant.get_claud_client()
 messages = [
     {"role": "human", "name": "alex", "content": "Can we change human nature?"}
 ]
 anthropic_message = ant.claud_message(
     client=ant_client,
     messages=messages,
@@ -98,14 +101,15 @@
 )
 ```
 #### Completion
 Again, there is a REST version and a native version.
 REST version:
 ```python
 from symposium.connectors import anthropic_rest as ant
+
 messages = [
     {"role": "human", "name": "alex", "content": "Can we change human nature?"}
 ]
 kwargs = {
     "model":                "claude-instant-1.2",
     "max_tokens":           5,
     # "prompt":               prompt,
@@ -119,14 +123,16 @@
 ## OpenAI
 Import:
 ```python
 from symposium.connectors import openai_rest as oai
 ```
 #### Messages
 ```python
+from symposium.connectors import openai_rest as oai
+
 messages = [
   {"role": "user", "content": "Can we change human nature?"}
 ]
 kwargs = {
     "model":                "gpt-3.5-turbo",
     # "messages":             [],
     "max_tokens":           5,
@@ -142,14 +148,16 @@
     "top_p":                0.5,
     "user":                 None
 }
 responses = oai.gpt_message(messages, **kwargs)
 ```
 #### Completion
 ```python
+from symposium.connectors import openai_rest as oai
+
 prompt = "Can we change human nature?"
 kwargs = {
     "model":                "gpt-3.5-turbo-instruct",
     # "prompt":               str,
     "suffix":               str,
     "max_tokens":           5,
     "n":                    1,
@@ -170,14 +178,16 @@
 ## Gemini
 Import:
 ```python
 from symposium.connectors import gemini_rest as gem
 ```
 #### Messages
 ```python
+from symposium.connectors import gemini_rest as gem
+
 messages = [
         {
             "role": "user",
             "parts": [
                 {"text": "Human nature can not be changed, because..."},
                 {"text": "...and that is why human nature can not be changed."}
             ]
@@ -210,27 +220,31 @@
 ## PaLM
 Import:
 ```python
 from symposium.connectors import palm_rest as path
 ```
 #### Completion
 ```python
+from symposium.connectors import palm_rest as path
+
 kwargs = {
     "model": "text-bison-001",
     "prompt": str,
     "temperature": 0.5,
     "n": 1,
     "max_tokens": 10,
     "top_p": 0.5,
     "top_k": None
 }
 responses = path.palm_complete(prompt, **kwargs)
 ```
 #### Messages
 ```python
+from symposium.connectors import palm_rest as path
+
 context = "This conversation will be happening between Albert and Niels"
 examples = [
         {
             "input": {"author": "Albert", "content": "We didn't talk about quantum mechanics lately..."},
             "output": {"author": "Niels", "content": "Yes, indeed."}
         }
 ]
```

### Comparing `symposium-0.2.0/README.md` & `symposium-0.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,45 +3,47 @@
 ## Unification
 One of the motivations for this package was the need in a unified format for messaging language models, which is particularly useful if you are going to experiment with interactions between them.
 
 The unified standard used by this package is as follows.
 ### 'System' messages
 ```python
 messages = [
-    {"role": "world",   "name": "openai",   "content": "Be an Abstract Intellect."}
+    {"role": "world", "name": "openai", "content": "Be an Antagonist."}
 ]
 ```
 Name field should be set to 'openai', 'anthropic', 'google_gemini' or 'google_palm'.
 For the 'anthropic' name, the last 
 'system' message will be used as the 'system' parameter in the request. For palm_messages v1beta3 format this message will be used in the 'context' parameter.
 ### 'User' messages
 ```python
 messages = [
-    {"role": "human",   "name": "alex",     "content": "Let's discuss human nature."}
+    {"role": "human", "name": "Alex", "content": "Let's discuss human nature."}
 ]
 ```
 The utility functions stored in the `adapters` sub-package transform incoming and outgoing messages of particular model from this format to a model-specific format and back from the format of its' response to the following output format. This includes the text synthesis with older (but in)
 ## Output format
 The unified standard used by this package is:
 ```python
 message = {
-    "role": "machine",   "name": "claude",     "content": " ... ", 
+    "role": "machine", "name": "claude",  
+    "content": " ... ", 
     "tags": [{}],   # optional, if in the response, then returned
-    "other": [{}]   # optional, for n > 1
+    "other": [{}]   # optional, if n > 1
 }
 ```
-Name field will be set to 'chatgpt', 'claude', 'gemini' or 'palm'.<br>
+`name` field will be set to 'chatgpt', 'claude', 'gemini' or 'palm'.<br>
 Tags are extracted from the text and put into a list. The placeholder for the tags is: (tag_name).<br>
 If there are more than one response, the other field will contain the list of the rest (transformed too).
 ## Anthropic
 There are two ways of interaction with Anthropic API, through the REST API and through the native Anthropic Python library with 'client'. If you don't want any dependencies (and uncertainty) use `anthropic_rest` connector. If you want to install this dependency do `pip install symposium[anthropic_native]`.
 #### Messages
 REST version:
 ```python
 from symposium.connectors import anthropic_rest as ant
+
 messages = [
     {"role": "human", "name": "alex", "content": "Can we change human nature?"}
 ]
 kwargs = {
     "model":                "claude-3-sonnet-20240229",
     "system":               "answer concisely",
     # "messages":             [],
@@ -53,14 +55,15 @@
     "top_p":                0.5
 }
 response = ant.claud_message(messages,**kwargs)
 ```
 Native version:
 ```python
 from symposium.connectors import anthropic_native as ant
+
 ant_client = ant.get_claud_client()
 messages = [
     {"role": "human", "name": "alex", "content": "Can we change human nature?"}
 ]
 anthropic_message = ant.claud_message(
     client=ant_client,
     messages=messages,
@@ -68,14 +71,15 @@
 )
 ```
 #### Completion
 Again, there is a REST version and a native version.
 REST version:
 ```python
 from symposium.connectors import anthropic_rest as ant
+
 messages = [
     {"role": "human", "name": "alex", "content": "Can we change human nature?"}
 ]
 kwargs = {
     "model":                "claude-instant-1.2",
     "max_tokens":           5,
     # "prompt":               prompt,
@@ -89,14 +93,16 @@
 ## OpenAI
 Import:
 ```python
 from symposium.connectors import openai_rest as oai
 ```
 #### Messages
 ```python
+from symposium.connectors import openai_rest as oai
+
 messages = [
   {"role": "user", "content": "Can we change human nature?"}
 ]
 kwargs = {
     "model":                "gpt-3.5-turbo",
     # "messages":             [],
     "max_tokens":           5,
@@ -112,14 +118,16 @@
     "top_p":                0.5,
     "user":                 None
 }
 responses = oai.gpt_message(messages, **kwargs)
 ```
 #### Completion
 ```python
+from symposium.connectors import openai_rest as oai
+
 prompt = "Can we change human nature?"
 kwargs = {
     "model":                "gpt-3.5-turbo-instruct",
     # "prompt":               str,
     "suffix":               str,
     "max_tokens":           5,
     "n":                    1,
@@ -140,14 +148,16 @@
 ## Gemini
 Import:
 ```python
 from symposium.connectors import gemini_rest as gem
 ```
 #### Messages
 ```python
+from symposium.connectors import gemini_rest as gem
+
 messages = [
         {
             "role": "user",
             "parts": [
                 {"text": "Human nature can not be changed, because..."},
                 {"text": "...and that is why human nature can not be changed."}
             ]
@@ -180,27 +190,31 @@
 ## PaLM
 Import:
 ```python
 from symposium.connectors import palm_rest as path
 ```
 #### Completion
 ```python
+from symposium.connectors import palm_rest as path
+
 kwargs = {
     "model": "text-bison-001",
     "prompt": str,
     "temperature": 0.5,
     "n": 1,
     "max_tokens": 10,
     "top_p": 0.5,
     "top_k": None
 }
 responses = path.palm_complete(prompt, **kwargs)
 ```
 #### Messages
 ```python
+from symposium.connectors import palm_rest as path
+
 context = "This conversation will be happening between Albert and Niels"
 examples = [
         {
             "input": {"author": "Albert", "content": "We didn't talk about quantum mechanics lately..."},
             "output": {"author": "Niels", "content": "Yes, indeed."}
         }
 ]
```

### Comparing `symposium-0.2.0/pyproject.toml` & `symposium-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "symposium"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Interaction of multiple language models"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `symposium-0.2.0/src/manual_testing/anthropic_native_test.py` & `symposium-0.2.1/src/manual_testing/anthropic_native_test.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/manual_testing/gemini_rest_test.py` & `symposium-0.2.1/src/manual_testing/gemini_rest_test.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/manual_testing/openai_native_test.py` & `symposium-0.2.1/src/manual_testing/openai_native_test.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/manual_testing/openai_rest_test.py` & `symposium-0.2.1/src/manual_testing/openai_rest_test.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/manual_testing/palm_rest_test.py` & `symposium-0.2.1/src/manual_testing/palm_rest_test.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/adapters/anth.py` & `symposium-0.2.1/src/symposium/adapters/anth.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 MACHINE_PREFIX = "\n\nAssistant:"
 
 
 def prepared_ant_messages(input):
     """
     :input_format
         messages = [
-            {"role": "human",   "name": "alex",     "content": "Can we discuss this?"},
-            {"role": "machine", "name": "claude",   "content": "Yes."}
-            {"role": "human",   "name": "alex",     "content": "Then let's do it."}
+            {"role": "human", "name": "alex", "content": "Can we discuss this?"},
+            {"role": "machine", "name": "claude", "content": "Yes."}
+            {"role": "human", "name": "alex",     "content": "Then let's do it."}
         ]
     :outputformat
         messages = [
             {"role": "user",        "content": "Can we discuss this?"}
             {"role": "assistant",   "content": "Yes."}
             {"role": "user",        "content": "Then let's do it."}
         ]
```

### Comparing `symposium-0.2.0/src/symposium/adapters/gem_rest.py` & `symposium-0.2.1/src/symposium/adapters/gem_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/adapters/oai_rest.py` & `symposium-0.2.1/src/symposium/adapters/oai_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/adapters/plm_rest.py` & `symposium-0.2.1/src/symposium/adapters/plm_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/__init__.py` & `symposium-0.2.1/src/symposium/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/anthropic_native.py` & `symposium-0.2.1/src/symposium/connectors/anthropic_native.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/anthropic_rest.py` & `symposium-0.2.1/src/symposium/connectors/anthropic_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/brcloud.py` & `symposium-0.2.1/src/symposium/connectors/brcloud.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/gemini_google.py` & `symposium-0.2.1/src/symposium/connectors/gemini_google.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/gemini_rest.py` & `symposium-0.2.1/src/symposium/connectors/gemini_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/govert.py` & `symposium-0.2.1/src/symposium/connectors/govert.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/hugface.py` & `symposium-0.2.1/src/symposium/connectors/hugface.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/openai_native.py` & `symposium-0.2.1/src/symposium/connectors/openai_native.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/openai_rest.py` & `symposium-0.2.1/src/symposium/connectors/openai_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/palm_google.py` & `symposium-0.2.1/src/symposium/connectors/palm_google.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/palm_rest.py` & `symposium-0.2.1/src/symposium/connectors/palm_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/connectors/vertrest.py` & `symposium-0.2.1/src/symposium/connectors/vertrest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/recorders/githublog.py` & `symposium-0.2.1/src/symposium/recorders/githublog.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,19 +43,19 @@
             template_repo = gh.get_repo(f'multilogue/multilogue-template')
             repo = org.create_repo_from_template(repository_name,
                                                  template_repo,
                                                  description,
                                                  private=private)
         return repo
     else:
+        user = gh.get_user()
         try:
-            repo = gh.get_repo(repository_name)
+            repo = user.get_repo(repository_name)
         except UnknownObjectException:
             template_repo = gh.get_repo(f'multilogue/multilogue-template')
-            user = gh.get_user()
             repo = user.create_repo_from_template(repository_name,
                                                   description,
                                                   template_repo,
                                                   private=private)
         return repo
```

### Comparing `symposium-0.2.0/src/symposium/templates/sentence.py` & `symposium-0.2.1/src/symposium/templates/sentence.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/templates/three_branch.py` & `symposium-0.2.1/src/symposium/templates/three_branch.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium/util/xml_tags.py` & `symposium-0.2.1/src/symposium/util/xml_tags.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/symposium.egg-info/PKG-INFO` & `symposium-0.2.1/src/symposium.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symposium
-Version: 0.2.0
+Version: 0.2.1
 Summary: Interaction of multiple language models
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/symposium
 Project-URL: Bug Tracker, https://github.com/multilogue/sumposium/issues
 Keywords: symposium,conversations,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,45 +33,47 @@
 ## Unification
 One of the motivations for this package was the need in a unified format for messaging language models, which is particularly useful if you are going to experiment with interactions between them.
 
 The unified standard used by this package is as follows.
 ### 'System' messages
 ```python
 messages = [
-    {"role": "world",   "name": "openai",   "content": "Be an Abstract Intellect."}
+    {"role": "world", "name": "openai", "content": "Be an Antagonist."}
 ]
 ```
 Name field should be set to 'openai', 'anthropic', 'google_gemini' or 'google_palm'.
 For the 'anthropic' name, the last 
 'system' message will be used as the 'system' parameter in the request. For palm_messages v1beta3 format this message will be used in the 'context' parameter.
 ### 'User' messages
 ```python
 messages = [
-    {"role": "human",   "name": "alex",     "content": "Let's discuss human nature."}
+    {"role": "human", "name": "Alex", "content": "Let's discuss human nature."}
 ]
 ```
 The utility functions stored in the `adapters` sub-package transform incoming and outgoing messages of particular model from this format to a model-specific format and back from the format of its' response to the following output format. This includes the text synthesis with older (but in)
 ## Output format
 The unified standard used by this package is:
 ```python
 message = {
-    "role": "machine",   "name": "claude",     "content": " ... ", 
+    "role": "machine", "name": "claude",  
+    "content": " ... ", 
     "tags": [{}],   # optional, if in the response, then returned
-    "other": [{}]   # optional, for n > 1
+    "other": [{}]   # optional, if n > 1
 }
 ```
-Name field will be set to 'chatgpt', 'claude', 'gemini' or 'palm'.<br>
+`name` field will be set to 'chatgpt', 'claude', 'gemini' or 'palm'.<br>
 Tags are extracted from the text and put into a list. The placeholder for the tags is: (tag_name).<br>
 If there are more than one response, the other field will contain the list of the rest (transformed too).
 ## Anthropic
 There are two ways of interaction with Anthropic API, through the REST API and through the native Anthropic Python library with 'client'. If you don't want any dependencies (and uncertainty) use `anthropic_rest` connector. If you want to install this dependency do `pip install symposium[anthropic_native]`.
 #### Messages
 REST version:
 ```python
 from symposium.connectors import anthropic_rest as ant
+
 messages = [
     {"role": "human", "name": "alex", "content": "Can we change human nature?"}
 ]
 kwargs = {
     "model":                "claude-3-sonnet-20240229",
     "system":               "answer concisely",
     # "messages":             [],
@@ -83,14 +85,15 @@
     "top_p":                0.5
 }
 response = ant.claud_message(messages,**kwargs)
 ```
 Native version:
 ```python
 from symposium.connectors import anthropic_native as ant
+
 ant_client = ant.get_claud_client()
 messages = [
     {"role": "human", "name": "alex", "content": "Can we change human nature?"}
 ]
 anthropic_message = ant.claud_message(
     client=ant_client,
     messages=messages,
@@ -98,14 +101,15 @@
 )
 ```
 #### Completion
 Again, there is a REST version and a native version.
 REST version:
 ```python
 from symposium.connectors import anthropic_rest as ant
+
 messages = [
     {"role": "human", "name": "alex", "content": "Can we change human nature?"}
 ]
 kwargs = {
     "model":                "claude-instant-1.2",
     "max_tokens":           5,
     # "prompt":               prompt,
@@ -119,14 +123,16 @@
 ## OpenAI
 Import:
 ```python
 from symposium.connectors import openai_rest as oai
 ```
 #### Messages
 ```python
+from symposium.connectors import openai_rest as oai
+
 messages = [
   {"role": "user", "content": "Can we change human nature?"}
 ]
 kwargs = {
     "model":                "gpt-3.5-turbo",
     # "messages":             [],
     "max_tokens":           5,
@@ -142,14 +148,16 @@
     "top_p":                0.5,
     "user":                 None
 }
 responses = oai.gpt_message(messages, **kwargs)
 ```
 #### Completion
 ```python
+from symposium.connectors import openai_rest as oai
+
 prompt = "Can we change human nature?"
 kwargs = {
     "model":                "gpt-3.5-turbo-instruct",
     # "prompt":               str,
     "suffix":               str,
     "max_tokens":           5,
     "n":                    1,
@@ -170,14 +178,16 @@
 ## Gemini
 Import:
 ```python
 from symposium.connectors import gemini_rest as gem
 ```
 #### Messages
 ```python
+from symposium.connectors import gemini_rest as gem
+
 messages = [
         {
             "role": "user",
             "parts": [
                 {"text": "Human nature can not be changed, because..."},
                 {"text": "...and that is why human nature can not be changed."}
             ]
@@ -210,27 +220,31 @@
 ## PaLM
 Import:
 ```python
 from symposium.connectors import palm_rest as path
 ```
 #### Completion
 ```python
+from symposium.connectors import palm_rest as path
+
 kwargs = {
     "model": "text-bison-001",
     "prompt": str,
     "temperature": 0.5,
     "n": 1,
     "max_tokens": 10,
     "top_p": 0.5,
     "top_k": None
 }
 responses = path.palm_complete(prompt, **kwargs)
 ```
 #### Messages
 ```python
+from symposium.connectors import palm_rest as path
+
 context = "This conversation will be happening between Albert and Niels"
 examples = [
         {
             "input": {"author": "Albert", "content": "We didn't talk about quantum mechanics lately..."},
             "output": {"author": "Niels", "content": "Yes, indeed."}
         }
 ]
```

### Comparing `symposium-0.2.0/src/symposium.egg-info/SOURCES.txt` & `symposium-0.2.1/src/symposium.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 LICENSE
 README.md
 pyproject.toml
 src/manual_testing/anthropic_native_test.py
 src/manual_testing/anthropic_rest_test.py
 src/manual_testing/gemini_rest_test.py
+src/manual_testing/groq_rest_test.py
 src/manual_testing/openai_native_test.py
 src/manual_testing/openai_rest_test.py
 src/manual_testing/palm_rest_test.py
+src/manual_testing/yaml_config.py
 src/symposium/__init__.py
 src/symposium.egg-info/PKG-INFO
 src/symposium.egg-info/SOURCES.txt
 src/symposium.egg-info/dependency_links.txt
 src/symposium.egg-info/requires.txt
 src/symposium.egg-info/top_level.txt
 src/symposium/adapters/__init__.py
 src/symposium/adapters/anth.py
 src/symposium/adapters/gem_rest.py
+src/symposium/adapters/grq_rest.py
 src/symposium/adapters/oai_native.py
 src/symposium/adapters/oai_rest.py
 src/symposium/adapters/plm_rest.py
 src/symposium/connectors/__init__.py
 src/symposium/connectors/anthropic_native.py
 src/symposium/connectors/anthropic_rest.py
 src/symposium/connectors/bedrock.py
 src/symposium/connectors/brcloud.py
 src/symposium/connectors/gemini_google.py
 src/symposium/connectors/gemini_rest.py
 src/symposium/connectors/govert.py
+src/symposium/connectors/groq_rest.py
 src/symposium/connectors/hugface.py
 src/symposium/connectors/openai_native.py
 src/symposium/connectors/openai_rest.py
 src/symposium/connectors/palm_google.py
 src/symposium/connectors/palm_rest.py
 src/symposium/connectors/together.py
 src/symposium/connectors/vertex.py
```

### Comparing `symposium-0.2.0/src/tests/test_anthropic.py` & `symposium-0.2.1/src/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/tests/test_anthropic_rest.py` & `symposium-0.2.1/src/tests/test_anthropic_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.0/src/tests/test_palm_rest.py` & `symposium-0.2.1/src/tests/test_palm_rest.py`

 * *Files identical despite different names*

