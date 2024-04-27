# Comparing `tmp/kss-5.2.0.tar.gz` & `tmp/kss-5.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kss-5.2.0.tar", last modified: Mon Apr  1 23:54:54 2024, max compression
+gzip compressed data, was "kss-5.3.0.dev0.tar", last modified: Sat Apr 27 14:14:25 2024, max compression
```

## Comparing `kss-5.2.0.tar` & `kss-5.3.0.dev0.tar`

### file list

```diff
@@ -1,54 +1,235 @@
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.926372 kss-5.2.0/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1569 2024-04-01 04:29:21.000000 kss-5.2.0/LICENSE
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      165 2024-03-31 20:17:42.000000 kss-5.2.0/MANIFEST.in
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    78578 2024-04-01 23:54:54.926515 kss-5.2.0/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    77826 2024-04-01 04:29:21.000000 kss-5.2.0/README.md
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.918974 kss-5.2.0/csrc/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-5.2.0/csrc/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-5.2.0/csrc/kss_cython.pyx
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-5.2.0/csrc/sentence_splitter.cpp
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-5.2.0/csrc/sentence_splitter.h
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.919088 kss-5.2.0/kss/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      432 2024-04-01 23:54:10.000000 kss-5.2.0/kss/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.920798 kss-5.2.0/kss/_elements/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_elements/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_elements/element.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_elements/empty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      369 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_elements/subclasses.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.921111 kss-5.2.0/kss/_modules/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.922027 kss-5.2.0/kss/_modules/morphemes/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/morphemes/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-5.2.0/kss/_modules/morphemes/analyzers.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1702 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/morphemes/split_morphemes.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3403 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/morphemes/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.924256 kss-5.2.0/kss/_modules/sentences/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/sentences/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/sentences/embracing_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/sentences/sentence_postprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-5.2.0/kss/_modules/sentences/sentence_preprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/sentences/sentence_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/sentences/sentence_splitter.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-5.2.0/kss/_modules/sentences/sentence_splitter_fast.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6829 2024-03-31 20:48:01.000000 kss-5.2.0/kss/_modules/sentences/split_sentences.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.925005 kss-5.2.0/kss/_modules/summarization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/summarization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      820 2023-05-16 17:34:32.000000 kss-5.2.0/kss/_modules/summarization/sentence.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3600 2023-05-16 17:34:32.000000 kss-5.2.0/kss/_modules/summarization/summarize_sentences.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2727 2023-05-16 17:34:32.000000 kss-5.2.0/kss/_modules/summarization/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.926172 kss-5.2.0/kss/_utils/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_utils/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-5.2.0/kss/_utils/const.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1408 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_utils/emojis.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      269 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_utils/logging.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_utils/multiprocessing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    12324 2024-03-31 14:02:55.000000 kss-5.2.0/kss/_utils/sanity_checks.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.919965 kss-5.2.0/kss.egg-info/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    78578 2024-04-01 23:54:54.000000 kss-5.2.0/kss.egg-info/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1251 2024-04-01 23:54:54.000000 kss-5.2.0/kss.egg-info/SOURCES.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-01 23:54:54.000000 kss-5.2.0/kss.egg-info/dependency_links.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-03-31 20:01:41.000000 kss-5.2.0/kss.egg-info/not-zip-safe
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       34 2024-04-01 23:54:54.000000 kss-5.2.0/kss.egg-info/requires.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       20 2024-04-01 23:54:54.000000 kss-5.2.0/kss.egg-info/top_level.txt
--rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-04-01 23:54:54.926737 kss-5.2.0/setup.cfg
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5863 2024-04-01 23:54:10.000000 kss-5.2.0/setup.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.379005 kss-5.3.0.dev0/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1569 2024-04-01 04:29:21.000000 kss-5.3.0.dev0/LICENSE
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-26 04:11:11.000000 kss-5.3.0.dev0/MANIFEST.in
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   204755 2024-04-27 14:14:25.379206 kss-5.3.0.dev0/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   203997 2024-04-27 14:03:15.000000 kss-5.3.0.dev0/README.md
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.354754 kss-5.3.0.dev0/bench/
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.359760 kss-5.3.0.dev0/bench/sentence_split/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 04:39:09.000000 kss-5.3.0.dev0/bench/sentence_split/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4379 2023-05-16 17:34:32.000000 kss-5.3.0.dev0/bench/sentence_split/sentence_split.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      615 2023-05-16 17:34:32.000000 kss-5.3.0.dev0/bench/sentence_split/test_baseline.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      600 2023-05-16 17:34:32.000000 kss-5.3.0.dev0/bench/sentence_split/test_kiwi.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1015 2023-05-16 17:34:32.000000 kss-5.3.0.dev0/bench/sentence_split/test_koalanlp.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      700 2024-03-31 14:00:52.000000 kss-5.3.0.dev0/bench/sentence_split/test_kss.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      587 2023-05-16 17:34:32.000000 kss-5.3.0.dev0/bench/sentence_split/test_word_split.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.360181 kss-5.3.0.dev0/csrc/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-5.3.0.dev0/csrc/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-5.3.0.dev0/csrc/kss_cython.pyx
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-5.3.0.dev0/csrc/sentence_splitter.cpp
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-5.3.0.dev0/csrc/sentence_splitter.h
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.360276 kss-5.3.0.dev0/kss/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6882 2024-04-27 14:14:13.000000 kss-5.3.0.dev0/kss/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.361378 kss-5.3.0.dev0/kss/_elements/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_elements/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_elements/element.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_elements/empty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      536 2024-04-14 01:15:11.000000 kss-5.3.0.dev0/kss/_elements/subclasses.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.361473 kss-5.3.0.dev0/kss/_modules/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_modules/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.361954 kss-5.3.0.dev0/kss/_modules/augmentation/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:47:16.000000 kss-5.3.0.dev0/kss/_modules/augmentation/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.362050 kss-5.3.0.dev0/kss/_modules/augmentation/assets/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)  4865459 2021-09-26 12:11:43.000000 kss-5.3.0.dev0/kss/_modules/augmentation/assets/wordnet.json
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3892 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/augmentation/augment.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3251 2024-04-23 11:22:09.000000 kss-5.3.0.dev0/kss/_modules/augmentation/distance.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3602 2024-04-27 11:42:40.000000 kss-5.3.0.dev0/kss/_modules/augmentation/replacement.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1411 2024-04-27 11:42:40.000000 kss-5.3.0.dev0/kss/_modules/augmentation/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.364902 kss-5.3.0.dev0/kss/_modules/collocation/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 18:49:12.000000 kss-5.3.0.dev0/kss/_modules/collocation/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9351 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/collocation/collocate.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.365591 kss-5.3.0.dev0/kss/_modules/g2p/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 11:01:28.000000 kss-5.3.0.dev0/kss/_modules/g2p/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.365807 kss-5.3.0.dev0/kss/_modules/g2p/assets/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    14802 2024-04-21 10:45:23.000000 kss-5.3.0.dev0/kss/_modules/g2p/assets/rules.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5390 2024-04-21 10:46:10.000000 kss-5.3.0.dev0/kss/_modules/g2p/assets/table.csv
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6586 2024-04-27 11:42:40.000000 kss-5.3.0.dev0/kss/_modules/g2p/english.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7184 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/g2p/g2p.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4459 2024-04-27 11:42:40.000000 kss-5.3.0.dev0/kss/_modules/g2p/numerals.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2722 2024-04-27 11:42:40.000000 kss-5.3.0.dev0/kss/_modules/g2p/regular.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4949 2024-04-27 11:42:40.000000 kss-5.3.0.dev0/kss/_modules/g2p/special.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8131 2024-04-27 11:42:40.000000 kss-5.3.0.dev0/kss/_modules/g2p/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.365985 kss-5.3.0.dev0/kss/_modules/hangulization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-26 07:28:27.000000 kss-5.3.0.dev0/kss/_modules/hangulization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3616 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulization.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.366496 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     2277 2024-04-27 09:12:39.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/__init__.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)    10423 2024-04-27 09:00:03.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/hangul.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.366597 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     1426 2018-08-18 18:42:06.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.366698 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/aze/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5272 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/aze/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.366795 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/bel/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5425 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/bel/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.366891 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/bul/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4925 2018-08-18 18:42:06.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/bul/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.366998 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/cat/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4328 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/cat/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.367098 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/ces/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4820 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/ces/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.367197 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/cym/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5791 2018-08-18 18:42:06.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/cym/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.367297 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/deu/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     7415 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/deu/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.367413 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/ell/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     9068 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/ell/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.367518 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/epo/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4103 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/epo/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.367625 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/est/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3931 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/est/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.367727 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/fin/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3410 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/fin/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.367827 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/grc/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     8626 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/grc/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.367929 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/hbs/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5606 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.368035 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/hun/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4990 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/hun/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.368136 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/isl/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5626 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/isl/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.368232 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/ita/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4371 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/ita/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.368326 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/jpn/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4446 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.368539 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6118 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/__init__.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6408 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/narrow.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.368637 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/lat/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3314 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/lat/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.368735 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/lav/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4116 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/lav/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.368831 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/lit/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4080 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/lit/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.368935 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/mkd/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5354 2018-08-18 18:42:06.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.369035 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/nld/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)    22064 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/nld/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.369169 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/pol/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5785 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/pol/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.369371 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/por/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6048 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/por/__init__.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/por/br.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.369473 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/ron/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5120 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/ron/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.369568 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/rus/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4994 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/rus/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.369666 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/slk/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6693 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/slk/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.369763 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/slv/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3836 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/slv/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.369869 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/spa/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4002 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/spa/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.369966 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/sqi/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3177 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.370061 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/swe/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     7896 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/swe/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.370156 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/tur/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3528 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/tur/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.370255 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/ukr/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5072 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.370355 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/vie/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4742 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/vie/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.370453 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/wlm/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5599 2024-04-27 09:05:48.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)    16108 2024-04-27 09:00:03.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/models.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     1069 2018-08-18 18:42:06.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/normalization.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     2897 2024-04-27 08:57:42.000000 kss-5.3.0.dev0/kss/_modules/hangulization/hangulize/processing.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.370730 kss-5.3.0.dev0/kss/_modules/hanja/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:46:48.000000 kss-5.3.0.dev0/kss/_modules/hanja/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4462 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/hanja/_hanja.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2021 2024-04-25 08:27:31.000000 kss-5.3.0.dev0/kss/_modules/hanja/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.370994 kss-5.3.0.dev0/kss/_modules/jamo/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:46:59.000000 kss-5.3.0.dev0/kss/_modules/jamo/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    12624 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/jamo/_jamo.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      912 2024-04-25 08:38:54.000000 kss-5.3.0.dev0/kss/_modules/jamo/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.371264 kss-5.3.0.dev0/kss/_modules/josa/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 07:12:50.000000 kss-5.3.0.dev0/kss/_modules/josa/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2580 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/josa/josa.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7030 2024-04-25 16:33:55.000000 kss-5.3.0.dev0/kss/_modules/josa/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.371526 kss-5.3.0.dev0/kss/_modules/keywords/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 11:01:42.000000 kss-5.3.0.dev0/kss/_modules/keywords/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6362 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/keywords/extract_keywords.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    17289 2024-04-27 12:31:02.000000 kss-5.3.0.dev0/kss/_modules/keywords/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.371925 kss-5.3.0.dev0/kss/_modules/morphemes/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_modules/morphemes/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-5.3.0.dev0/kss/_modules/morphemes/analyzers.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1849 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/morphemes/split_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3588 2024-04-23 09:05:15.000000 kss-5.3.0.dev0/kss/_modules/morphemes/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.372103 kss-5.3.0.dev0/kss/_modules/paradigm/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 08:40:05.000000 kss-5.3.0.dev0/kss/_modules/paradigm/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    18316 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/paradigm/paradigm.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.373214 kss-5.3.0.dev0/kss/_modules/preprocessing/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-26 07:58:23.000000 kss-5.3.0.dev0/kss/_modules/preprocessing/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    15532 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/preprocessing/anonymize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    29789 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/preprocessing/clean_news.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    81169 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/preprocessing/completed_form.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    24570 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/preprocessing/filter_out.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2088 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/preprocessing/half2full.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/preprocessing/normalize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    26257 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/preprocessing/preprocess.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7186 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/preprocessing/reduce_repeats.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7661 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/preprocessing/remove_invisible_chars.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.373481 kss-5.3.0.dev0/kss/_modules/qwerty/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 08:21:28.000000 kss-5.3.0.dev0/kss/_modules/qwerty/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6262 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/qwerty/qwerty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5941 2024-04-21 19:55:18.000000 kss-5.3.0.dev0/kss/_modules/qwerty/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.373751 kss-5.3.0.dev0/kss/_modules/romanization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:48:29.000000 kss-5.3.0.dev0/kss/_modules/romanization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5813 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/romanization/romanize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8901 2024-04-21 17:45:54.000000 kss-5.3.0.dev0/kss/_modules/romanization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.374021 kss-5.3.0.dev0/kss/_modules/safety/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 04:59:07.000000 kss-5.3.0.dev0/kss/_modules/safety/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3525 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/safety/check_safety.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    35374 2024-04-21 06:06:58.000000 kss-5.3.0.dev0/kss/_modules/safety/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.374911 kss-5.3.0.dev0/kss/_modules/sentences/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_modules/sentences/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_modules/sentences/embracing_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_modules/sentences/sentence_postprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-5.3.0.dev0/kss/_modules/sentences/sentence_preprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_modules/sentences/sentence_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_modules/sentences/sentence_splitter.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-5.3.0.dev0/kss/_modules/sentences/sentence_splitter_fast.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8423 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/sentences/split_sentences.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.375213 kss-5.3.0.dev0/kss/_modules/spacing/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 14:16:36.000000 kss-5.3.0.dev0/kss/_modules/spacing/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5539 2024-04-27 13:58:40.000000 kss-5.3.0.dev0/kss/_modules/spacing/correct_spacing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   296979 2024-04-27 02:42:16.000000 kss-5.3.0.dev0/kss/_modules/spacing/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.375862 kss-5.3.0.dev0/kss/_modules/summarization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_modules/summarization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5603 2024-04-27 13:55:54.000000 kss-5.3.0.dev0/kss/_modules/summarization/summarize_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3396 2024-04-26 07:26:56.000000 kss-5.3.0.dev0/kss/_modules/summarization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.376622 kss-5.3.0.dev0/kss/_utils/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_utils/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       66 2024-04-27 04:09:55.000000 kss-5.3.0.dev0/kss/_utils/api.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-5.3.0.dev0/kss/_utils/const.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1399 2024-04-21 19:08:53.000000 kss-5.3.0.dev0/kss/_utils/emojis.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      910 2024-04-23 08:15:52.000000 kss-5.3.0.dev0/kss/_utils/logger.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-5.3.0.dev0/kss/_utils/multiprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    17275 2024-04-27 03:50:29.000000 kss-5.3.0.dev0/kss/_utils/sanity_checks.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.360987 kss-5.3.0.dev0/kss.egg-info/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   204755 2024-04-27 14:14:25.000000 kss-5.3.0.dev0/kss.egg-info/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6339 2024-04-27 14:14:25.000000 kss-5.3.0.dev0/kss.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:14:25.000000 kss-5.3.0.dev0/kss.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:04:55.000000 kss-5.3.0.dev0/kss.egg-info/not-zip-safe
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      136 2024-04-27 14:14:25.000000 kss-5.3.0.dev0/kss.egg-info/requires.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       32 2024-04-27 14:14:25.000000 kss-5.3.0.dev0/kss.egg-info/top_level.txt
+-rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-04-27 14:14:25.379454 kss-5.3.0.dev0/setup.cfg
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6191 2024-04-27 09:17:01.000000 kss-5.3.0.dev0/setup.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:14:25.378746 kss-5.3.0.dev0/tests/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 02:40:08.000000 kss-5.3.0.dev0/tests/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1033 2024-04-27 09:25:57.000000 kss-5.3.0.dev0/tests/test_augmentation.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8258 2024-04-27 08:00:32.000000 kss-5.3.0.dev0/tests/test_collocation.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      250 2024-04-27 08:00:32.000000 kss-5.3.0.dev0/tests/test_g2p.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      238 2024-04-27 08:00:32.000000 kss-5.3.0.dev0/tests/test_hangulize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      747 2024-04-27 04:21:47.000000 kss-5.3.0.dev0/tests/test_hanja.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      978 2024-04-27 04:13:17.000000 kss-5.3.0.dev0/tests/test_jamo.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      442 2024-04-27 04:17:41.000000 kss-5.3.0.dev0/tests/test_josa.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3405 2024-04-27 04:17:41.000000 kss-5.3.0.dev0/tests/test_keywords.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-27 09:20:57.000000 kss-5.3.0.dev0/tests/test_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    19148 2024-04-27 04:25:01.000000 kss-5.3.0.dev0/tests/test_paradigm.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    97981 2024-04-27 13:38:44.000000 kss-5.3.0.dev0/tests/test_preprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      290 2024-04-27 07:33:52.000000 kss-5.3.0.dev0/tests/test_qwerty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      257 2024-04-27 07:39:43.000000 kss-5.3.0.dev0/tests/test_romanize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      313 2024-04-27 08:03:40.000000 kss-5.3.0.dev0/tests/test_safety.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      776 2024-04-27 07:56:55.000000 kss-5.3.0.dev0/tests/test_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      236 2024-04-27 08:00:32.000000 kss-5.3.0.dev0/tests/test_spacing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1966 2024-04-27 08:00:32.000000 kss-5.3.0.dev0/tests/test_summarization.py
```

### Comparing `kss-5.2.0/LICENSE` & `kss-5.3.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/csrc/kss_cython.pyx` & `kss-5.3.0.dev0/csrc/kss_cython.pyx`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/csrc/sentence_splitter.cpp` & `kss-5.3.0.dev0/csrc/sentence_splitter.cpp`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/csrc/sentence_splitter.h` & `kss-5.3.0.dev0/csrc/sentence_splitter.h`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_elements/element.py` & `kss-5.3.0.dev0/kss/_elements/element.py`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_elements/empty.py` & `kss-5.3.0.dev0/kss/_elements/empty.py`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_modules/morphemes/analyzers.py` & `kss-5.3.0.dev0/kss/_modules/morphemes/analyzers.py`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_modules/morphemes/split_morphemes.py` & `kss-5.3.0.dev0/kss/_modules/morphemes/split_morphemes.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,37 +14,39 @@
 
 
 def split_morphemes(
     text: Union[str, List[str], Tuple[str]],
     backend: str = "auto",
     num_workers: Union[int, str] = "auto",
     drop_space: bool = True,
-    return_pos: bool = True,
 ) -> Union[List[Tuple[str, str]], List[List[Tuple[str, str]]], Union[List, Tuple]]:
     """
-    Split texts into morphemes.
+    This splits texts into morphemes.
 
     Args:
         text (Union[str, List[str], Tuple[str]]): single text or list/tuple of texts
         backend (str): morpheme analyzer backend. 'mecab', 'pecab' are supported.
         num_workers (Union[int, str])): the number of multiprocessing workers
         drop_space (bool): drop all spaces in output or not
 
     Returns:
         Union[List[Tuple[str, str]], List[List[Tuple[str, str]]], Union[List, Tuple]]:
             outputs of morpheme analysis.
+
+    Examples:
+        >>> from kss import Kss
+        >>> split_morphemes = Kss("split_morphemes")
+        >>> text = "아버지가방에들어오시다."
+        >>> output = split_morphemes(text)
+        >>> print(output)
+        [('아버지', 'NNG'), ('가', 'JKS'), ('방', 'NNG'), ('에', 'JKB'), ('들어오', 'VV'), ('시', 'EP'), ('다', 'EF'), ('.', 'SF')]
     """
     text, finish = _check_text(text)
     drop_space = _check_type(drop_space, "drop_space", bool)
 
     if finish:
         return text
 
     num_workers = _check_num_workers(text, num_workers)
     backend = _check_analyzer_backend(backend)
     result = _run_job(partial(backend.pos, drop_space=drop_space), text, num_workers)
-    if not return_pos:
-        if isinstance(text, str):
-            result = [token[0] for token in result]
-        else:
-            result = [[token[0] for token in tokens] for tokens in result]
     return result
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kss-5.2.0/kss/_modules/morphemes/utils.py` & `kss-5.3.0.dev0/kss/_modules/morphemes/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -134,7 +134,12 @@
                 token = tokens[token_idx]
                 results.append(token)
                 text_idx += len(token[0])
                 token_idx += 1
             else:
                 break
     return results
+
+
+def _reset_spaces(text: str, tokens: List[Tuple[str, str]]):
+    tokens = [(text, pos) for text, pos in tokens if pos != "SP"]
+    return _preserve_space(text, tokens, " \n\r\t\v\f")
```

### Comparing `kss-5.2.0/kss/_modules/sentences/embracing_processor.py` & `kss-5.3.0.dev0/kss/_modules/sentences/embracing_processor.py`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_modules/sentences/sentence_postprocessor.py` & `kss-5.3.0.dev0/kss/_modules/sentences/sentence_postprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_modules/sentences/sentence_preprocessor.py` & `kss-5.3.0.dev0/kss/_modules/sentences/sentence_preprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_modules/sentences/sentence_processor.py` & `kss-5.3.0.dev0/kss/_modules/sentences/sentence_processor.py`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_modules/sentences/sentence_splitter.py` & `kss-5.3.0.dev0/kss/_modules/sentences/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_modules/sentences/sentence_splitter_fast.py` & `kss-5.3.0.dev0/kss/_modules/sentences/sentence_splitter_fast.py`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_modules/summarization/utils.py` & `kss-5.3.0.dev0/kss/_modules/summarization/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,37 @@
 # This code was copied from Text Rank KR [https://github.com/theeluwin/textrankr]
 # And modified by Hyunwoong Ko [https://github.com/hyunwoongko]
-
 from collections import Counter
 from itertools import combinations
 from typing import List
 
-from kss import split_morphemes, split_sentences
-from kss._modules.summarization.sentence import Sentence
+from kss._modules.morphemes.split_morphemes import split_morphemes
+from kss._modules.sentences.split_sentences import split_sentences
+
+
+class Sentence:
+    """
+    Notes:
+        The purpose of this class is as follows:
+            1. In order to use the 'pagerank' function in the networkx library, you need a hashable object.
+            2. Summaries should keep the sentence order from its original text to improve the verbosity.
+
+        Note that the 'bow' stands for 'bag-of-words'.
+    """
+
+    def __init__(self, index: int, text: str, bow: Counter) -> None:
+        self.index: int = index
+        self.text: str = text
+        self.bow: Counter = bow
+
+    def __str__(self) -> str:
+        return self.text
+
+    def __hash__(self) -> int:
+        return self.index
 
 
 def _parse_text_into_sentences(
     text: str, backend: str, strip: bool, ignores: List[str]
 ) -> List[Sentence]:
     """
     This function splits the given text into sentence candidates using a pre-defined splitter,
@@ -80,7 +101,8 @@
     for sentence1, sentence2 in combinations(sentences, 2):
         weight: float = _multiset_jaccard_index(sentence1.bow, sentence2.bow)
         if weight > tolerance:
             graph.add_edge(sentence1, sentence2, weight=weight)
 
     # return
     return graph
+
```

### Comparing `kss-5.2.0/kss/_utils/const.py` & `kss-5.3.0.dev0/kss/_utils/const.py`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_utils/emojis.py` & `kss-5.3.0.dev0/kss/_utils/emojis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (C) 2021 Hyunwoong Ko <kevin.brain@kakaobrain.com> and Sang-Kil Park <skpark1224@hyundai.com>
 # All rights reserved.
 
 import emoji
-import regex
+import re
 
 _emojis = {}
 _specials = ["♡", "♥"]
 _unicodes = [
     "‍",  # Zero width joiner
     "︀",  # Variation Selector-1
     "︁",  # Variation Selector-2
@@ -33,14 +33,14 @@
         _emojis.update({k: "" for k in _unicodes})
 except Exception as e:
     raise ImportError("Kss requires `emoji==1.2.0`. please install that version.")
 
 
 def get_emoji(text):
     emoji_list = []
-    flags = regex.findall("[\U0001F1E6-\U0001F1FF]", text)
+    flags = re.findall("[\U0001F1E6-\U0001F1FF]", text)
 
-    for grapheme in regex.findall(r"\X", text):
+    for grapheme in re.findall(r"\X", text):
         if any(char in _emojis for char in grapheme):
             emoji_list.append(grapheme)
 
     return emoji_list + flags
```

### Comparing `kss-5.2.0/kss/_utils/multiprocessing.py` & `kss-5.3.0.dev0/kss/_utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `kss-5.2.0/kss/_utils/sanity_checks.py` & `kss-5.3.0.dev0/kss/_utils/sanity_checks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright (C) 2021 Hyunwoong Ko <kevin.brain@kakaobrain.com> and Sang-Kil Park <skpark1224@hyundai.com>
 # All rights reserved.
-
+import numbers
 import platform
 import unicodedata
 from typing import Union, Tuple, List, Any, Optional, Type, Callable, Iterable
 
 from kss._modules.morphemes.analyzers import (
     MecabAnalyzer,
     PecabAnalyzer,
     Analyzer,
     CharacterAnalyzer,
     FastAnalyzer,
 )
-from kss._utils.logging import logger
+from kss._utils.logger import logger
 
 MECAB_INFORM, KONLPY_MECAB_INFORM, PECAB_INFORM, FAST_INFORM = (
     False,
     False,
     False,
     False,
 )
@@ -105,14 +105,17 @@
         types (Union[Type, List[Type]]): types
 
     Returns:
         Any: param value
     """
     was_list = True
 
+    if types == int or types == float:
+        types = numbers.Number
+
     if not isinstance(types, list) or not isinstance(types, tuple):
         types = [types]
         was_list = False
 
     available = any([isinstance(param, _type) for _type in types])
 
     if not available:
@@ -121,14 +124,34 @@
             f"Currently kss only supports {types if was_list else types[0]} {'types' if was_list else 'type'} for this.\n"
             f"Please check `{param_name}` parameter again ;)\n"
         )
 
     return param
 
 
+def _check_char(text: str) -> str:
+    """
+    Check text length is 1.
+
+    Args:
+        text (str): text
+
+    Returns:
+        str: text
+    """
+    if len(text) != 1:
+        raise ValueError(
+            f"Oops! '{text}' is not a single character.\n"
+            f"Currently kss only supports single character for this.\n"
+            f"Please check `text` parameter again ;)"
+        )
+
+    return text
+
+
 def _check_text(
     text: Union[str, List[str], Tuple[str]]
 ) -> Tuple[Union[str, List[str], Tuple[str]], bool]:
     """
     Check input text type.
 
     Args:
@@ -157,33 +180,127 @@
             not_string_idx = are_strings.index(False)
             raise TypeError(
                 "Oops! Some elements in `text` were not string.\n"
                 f"For example, index {not_string_idx} was {type(text[not_string_idx])}.\n"
                 f"Currently kss only supports [str, List[str], Tuple[str]] for this.\n"
                 f"Please check `text` parameter again ;)\n"
             )
-        else:
-            text = [unicodedata.normalize("NFC", t) for t in text]
 
         # unwrap list or tuple with single text
         if len(text) == 1:
             text = text[0]
 
         if isinstance(text, list):
             text = tuple(text)
 
-    elif not isinstance(text, str) and len(text) == 0:
+    elif len(text) == 0:
         finish = True
 
-    elif isinstance(text, str):
-        text = unicodedata.normalize("NFC", text)
-
     return text, finish
 
 
+def _check_backend_mecab_pecab_only(backend: str) -> Analyzer:
+    global MECAB_INFORM, KONLPY_MECAB_INFORM, PECAB_INFORM
+
+    if isinstance(backend, str):
+        backend = backend.lower()
+
+    if backend not in ["auto", "mecab", "pecab"]:
+        raise ValueError(
+            f"Oops! '{backend}' is not supported value for spacing correction module.\n"
+            f"Currently the spacing correction module only supports ['auto', 'pecab', 'mecab'] for this.\n"
+            f"Please check `backend` parameter again ;)\n"
+        )
+
+    mecab_backend = MecabAnalyzer()
+    pecab_backend = PecabAnalyzer()
+
+    if backend == "mecab":
+        if mecab_backend._backend is not None:
+            return mecab_backend
+        else:
+            raise ImportError(
+                _message_by_user_os(
+                    linux_macos="Oops! You specified `backend` as 'mecab', but you don't have mecab in your environment.\n"
+                    "If you want to use mecab backend, please install mecab or konlpy.tag.Mecab!\n"
+                    "Please refer to following web sites for details:\n"
+                    f"- mecab: {_mecab_info_linux_macos}\n"
+                    f"- konlpy.tag.Mecab: {_konlpy_info_linux_macos}\n",
+                    windows="Oops! You specified `backend` as 'mecab', but you don't have mecab in your environment.\n"
+                    "If you want to use mecab backend, please install mecab or konlpy.tag.Mecab!\n"
+                    "Please refer to following web sites for details:\n"
+                    f"- mecab: {_mecab_info_windows}\n"
+                    f"- konlpy.tag.Mecab: {_konlpy_info_windows}\n",
+                )
+            )
+
+    elif backend == "pecab":
+        if pecab_backend._backend is not None:
+            return pecab_backend
+        else:
+            raise ImportError(
+                "Oops! You specified `backend` as 'pecab', but you don't have pecab in your environment.\n"
+                "If you want to use pecab backend, please install pecab!\n"
+                "Please refer to following web sites for details:\n"
+                "- pecab: https://github.com/hyunwoongko/pecab\n"
+            )
+
+    elif backend == "auto":
+        if mecab_backend._backend == "mecab":
+            if not MECAB_INFORM:
+                logger.warning(
+                    "Oh! You have mecab in your environment. Kss will take this as a backend! :D\n"
+                )
+                MECAB_INFORM = True
+            return mecab_backend
+
+        elif mecab_backend._backend == "konlpy":
+            if not KONLPY_MECAB_INFORM:
+                logger.warning(
+                    "Oh! You have konlpy.tag.Mecab in your environment. Kss will take this as a backend! :D\n"
+                )
+                KONLPY_MECAB_INFORM = True
+            return mecab_backend
+
+        elif pecab_backend._backend == "pecab":
+            if not PECAB_INFORM:
+
+                installation_help_message = _message_by_user_os(
+                    linux_macos="For your information, Kss also supports mecab backend.\n"
+                    "We recommend you to install mecab or konlpy.tag.Mecab for faster execution of Kss.\n"
+                    "Please refer to following web sites for details:\n"
+                    f"- mecab: {_mecab_info_linux_macos}\n"
+                    f"- konlpy.tag.Mecab: {_konlpy_info_linux_macos}\n",
+                    windows="For your information, Kss also supports mecab backend.\n"
+                    "We recommend you to install mecab or konlpy.tag.Mecab for faster execution of Kss.\n"
+                    "Please refer to following web sites for details:\n"
+                    f"- mecab: {_mecab_info_windows}\n"
+                    f"- konlpy.tag.Mecab: {_konlpy_info_windows}\n",
+                )
+
+                logger.warning(
+                    "Because there's no supported C++ morpheme analyzer, "
+                    "Kss will take pecab as a backend. :D\n"
+                    f"{installation_help_message}"
+                )
+                PECAB_INFORM = True
+
+            return pecab_backend
+        else:
+            raise ImportError(
+                f"Oops! You don't have any supported morpheme analyzer in your environment.\n"
+                f"If you want to use spacing correction module, please install mecab or pecab!\n"
+                f"Please refer to following web sites for details:\n"
+                f"- mecab:\n"
+                f"  - Linux/MacOS: {_mecab_info_linux_macos}\n"
+                f"  - Windows: {_mecab_info_windows}\n"
+                f"- pecab: {_pecab_info}\n"
+            )
+
+
 def _check_analyzer_backend(backend: str) -> Analyzer:
     """
     Check morpheme analyzer backend type.
 
     Args:
         backend (str):
 
@@ -335,15 +452,15 @@
         )
 
     if (
         isinstance(inputs, str)
         or (
             (isinstance(inputs, list) or isinstance(inputs, tuple)) and len(inputs) == 1
         )
-        or num_workers == 1
+        or (isinstance(num_workers, numbers.Number) and num_workers < 2)
     ):
         return False
         # no multiprocessing worker
 
     elif num_workers == "auto":
         num_workers = None
         # maximum multiprocessing workers
```

### Comparing `kss-5.2.0/setup.py` & `kss-5.3.0.dev0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import codecs
 import os
 import platform
 import subprocess
 import sys
 from contextlib import suppress
-from distutils.extension import Extension
 from distutils.ccompiler import new_compiler
+from distutils.extension import Extension
 from distutils.sysconfig import customize_compiler
 
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 """
 How pip install works:
 
-1. pip creates a temporary file, in Linux it's in /tmp, and on Windows it's in the temp dir of the user.
+1. pip creates a temporary file, in Linux it"s in /tmp, and on Windows it"s in the temp dir of the user.
 2. pip downloads/extracts the package to that temp directory (whether from a tar.gz or from an online source or from a repository)
 3. pip runs the following operations in order:
   - setup.py install
   - setup.py build
   - setup.py install_lib
   - setup.py build_py
   - setup.py build_ext
@@ -55,22 +55,22 @@
                     # 4. Cannot install mecab.
                     pass
 
         super().run()
 
 
 def get_extra_compile_args():
-    if platform.system() == 'Linux':
-        extra_compile_args = ['-std=c++11']
+    if platform.system() == "Linux":
+        extra_compile_args = ["-std=c++11"]
         extra_link_args = []
-    elif platform.system() == 'Darwin':
-        extra_compile_args = ['-std=c++11', '-stdlib=libc++']
-        extra_link_args = ['-stdlib=libc++']
-    elif platform.system() == 'Windows':
-        extra_compile_args = ['/utf-8']
+    elif platform.system() == "Darwin":
+        extra_compile_args = ["-std=c++11", "-stdlib=libc++"]
+        extra_link_args = ["-stdlib=libc++"]
+    elif platform.system() == "Windows":
+        extra_compile_args = ["/utf-8"]
         extra_link_args = []
     else:
         extra_compile_args = []
         extra_link_args = []
     return extra_compile_args, extra_link_args
 
 
@@ -78,18 +78,18 @@
     extra_compile_args, extra_link_args = \
         get_extra_compile_args()
 
     _ext_modules = [
         Extension(
             "kss_cython",
             sources=[
-                'csrc/kss_cython.pyx',
-                'csrc/sentence_splitter.cpp',
+                "csrc/kss_cython.pyx",
+                "csrc/sentence_splitter.cpp",
             ],
-            language='c++',
+            language="c++",
             extra_compile_args=extra_compile_args,
             extra_link_args=extra_link_args,
             include_dirs=["."],
         )
     ]
 
     try:
@@ -114,15 +114,15 @@
 
 def is_compilable():
     try:
         # 1. Try to compile csrc/sentence_splitter.cpp
         extra_compile_args, extra_link_args = get_extra_compile_args()
         compiler = new_compiler()
         customize_compiler(compiler)
-        compiler.compile(['csrc/sentence_splitter.cpp'], extra_postargs=extra_compile_args)
+        compiler.compile(["csrc/sentence_splitter.cpp"], extra_postargs=extra_compile_args)
         return True
     except:
         # 2. Cannot compile csrc/sentence_splitter.cpp
         return False
 
 
 def cythonize_if_possible():
@@ -141,35 +141,46 @@
         return cb(f)
 
 
 version = None
 with open(os.path.join("kss", "__init__.py"), encoding="utf-8") as f:
     for line in f:
         if line.strip().startswith("__version__"):
-            version = line.split("=")[1].strip().replace('"', "").replace("'", "")
+            version = line.split("=")[1].strip().replace("'", "").replace('"', "")
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
+install_requires = [
+    "emoji==1.2.0", "pecab", "networkx", "jamo",
+    "hangul-jamo", "hanja==0.13.3", "tossi", "distance",
+    "unidecode", "cmudict", "koparadigm", "kollocate",
+    "bs4", "numpy", "pytest", "scipy"
+]
+
 setup(
     name="kss",
     version=version,
     author="Hyunwoong Ko",
     author_email="kevin.brain@kakaobrain.com",
     url="https://github.com/hyunwoongko/kss",
-    license='BSD 3-Clause "New" or "Revised" License',
+    license="BSD 3-Clause \"New\" or \"Revised\" License",
     description="A Toolkit for Korean sentence segmentation",
     long_description_content_type="text/markdown",
     platforms=["any"],
-    install_requires=["emoji==1.2.0", "regex", "pecab", "networkx"],
+    install_requires=install_requires,
     long_description=long_description,
     packages=find_packages(exclude=["bench", "assets", ".java", ".pytest_cache"]),
     python_requires=">=3",
     zip_safe=False,
-    package_data={"": ["csrc/*"]},
+    package_data={
+        "cython": ["csrc/*"],
+        "g2p": ["kss/_modules/g2p/assets/*"],
+        "augmentation": ["kss/_modules/augmentation/assets/*"],
+    },
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
```

