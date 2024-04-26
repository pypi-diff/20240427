# Comparing `tmp/qualitative_coding-1.2.8.tar.gz` & `tmp/qualitative_coding-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualitative_coding-1.2.8.tar", max compression
+gzip compressed data, was "qualitative_coding-1.2.9.tar", max compression
```

## Comparing `qualitative_coding-1.2.8.tar` & `qualitative_coding-1.2.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      781 2021-07-13 19:40:03.158793 qualitative_coding-1.2.8/LICENSE
--rw-r--r--   0        0        0    13681 2024-03-12 15:05:27.802641 qualitative_coding-1.2.8/README.md
--rw-r--r--   0        0        0      717 2024-03-18 13:10:42.419850 qualitative_coding-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     1010 2024-03-12 15:05:27.805722 qualitative_coding-1.2.8/qualitative_coding/cli/__init__.py
--rw-r--r--   0        0        0      498 2024-03-12 15:05:27.806804 qualitative_coding-1.2.8/qualitative_coding/cli/check.py
--rw-r--r--   0        0        0     3278 2024-02-11 22:24:40.918879 qualitative_coding-1.2.8/qualitative_coding/cli/click_aliases.py
--rw-r--r--   0        0        0     2182 2024-03-12 15:05:27.807580 qualitative_coding-1.2.8/qualitative_coding/cli/code.py
--rw-r--r--   0        0        0      481 2024-03-12 15:05:27.808260 qualitative_coding-1.2.8/qualitative_coding/cli/codebook.py
--rw-r--r--   0        0        0      664 2024-03-12 15:05:27.808807 qualitative_coding-1.2.8/qualitative_coding/cli/coders.py
--rw-r--r--   0        0        0      649 2024-03-15 21:48:34.219106 qualitative_coding-1.2.8/qualitative_coding/cli/codes/__init__.py
--rw-r--r--   0        0        0     3733 2024-03-14 01:20:49.652977 qualitative_coding-1.2.8/qualitative_coding/cli/codes/crosstab.py
--rw-r--r--   0        0        0     2533 2024-03-16 17:56:09.955659 qualitative_coding-1.2.8/qualitative_coding/cli/codes/find.py
--rw-r--r--   0        0        0      668 2024-03-12 15:05:27.810392 qualitative_coding-1.2.8/qualitative_coding/cli/codes/list.py
--rw-r--r--   0        0        0     1010 2024-03-14 01:20:49.653588 qualitative_coding-1.2.8/qualitative_coding/cli/codes/rename.py
--rw-r--r--   0        0        0     3551 2024-03-14 01:20:49.653928 qualitative_coding-1.2.8/qualitative_coding/cli/codes/stats.py
--rw-r--r--   0        0        0      611 2024-03-12 15:05:27.811349 qualitative_coding-1.2.8/qualitative_coding/cli/corpus/__init__.py
--rw-r--r--   0        0        0     1108 2024-03-12 15:05:27.812144 qualitative_coding-1.2.8/qualitative_coding/cli/corpus/import_media.py
--rw-r--r--   0        0        0      620 2024-03-12 15:05:27.812691 qualitative_coding-1.2.8/qualitative_coding/cli/corpus/list.py
--rw-r--r--   0        0        0      629 2024-03-12 15:05:27.813169 qualitative_coding-1.2.8/qualitative_coding/cli/corpus/move.py
--rw-r--r--   0        0        0      581 2024-03-12 15:05:27.814175 qualitative_coding-1.2.8/qualitative_coding/cli/corpus/remove.py
--rw-r--r--   0        0        0      611 2024-02-20 00:15:13.174056 qualitative_coding-1.2.8/qualitative_coding/cli/decorators.py
--rw-r--r--   0        0        0      651 2024-03-12 15:05:27.814632 qualitative_coding-1.2.8/qualitative_coding/cli/export.py
--rw-r--r--   0        0        0      895 2024-03-12 15:05:27.815075 qualitative_coding-1.2.8/qualitative_coding/cli/init.py
--rw-r--r--   0        0        0      836 2024-03-12 15:05:27.815550 qualitative_coding-1.2.8/qualitative_coding/cli/memo.py
--rw-r--r--   0        0        0     1575 2024-02-11 22:24:40.931614 qualitative_coding-1.2.8/qualitative_coding/cli/options.py
--rw-r--r--   0        0        0      743 2024-03-12 15:05:27.816080 qualitative_coding-1.2.8/qualitative_coding/cli/upgrade.py
--rw-r--r--   0        0        0      216 2024-02-11 22:24:40.936290 qualitative_coding-1.2.8/qualitative_coding/cli/version.py
--rw-r--r--   0        0        0       96 2021-07-13 19:40:03.159583 qualitative_coding-1.2.8/qualitative_coding/codebook.py
--rw-r--r--   0        0        0    36543 2024-03-14 01:20:49.654765 qualitative_coding-1.2.8/qualitative_coding/corpus.py
--rw-r--r--   0        0        0       50 2024-02-11 22:24:40.939611 qualitative_coding-1.2.8/qualitative_coding/database/errors.py
--rw-r--r--   0        0        0     3293 2024-03-12 15:05:27.817461 qualitative_coding-1.2.8/qualitative_coding/database/models.py
--rw-r--r--   0        0        0      865 2024-02-23 21:08:31.319862 qualitative_coding-1.2.8/qualitative_coding/editors.py
--rw-r--r--   0        0        0      210 2024-02-23 20:28:22.231952 qualitative_coding-1.2.8/qualitative_coding/exceptions.py
--rw-r--r--   0        0        0     4220 2024-03-14 01:36:39.218279 qualitative_coding-1.2.8/qualitative_coding/helpers.py
--rw-r--r--   0        0        0      895 2021-07-13 19:40:03.160344 qualitative_coding-1.2.8/qualitative_coding/logs.py
--rw-r--r--   0        0        0      288 2024-02-11 22:24:40.943568 qualitative_coding-1.2.8/qualitative_coding/media_importers/__init__.py
--rw-r--r--   0        0        0      560 2024-02-20 00:15:13.183338 qualitative_coding-1.2.8/qualitative_coding/media_importers/base.py
--rw-r--r--   0        0        0      335 2024-02-20 19:36:20.339419 qualitative_coding-1.2.8/qualitative_coding/media_importers/pandoc.py
--rw-r--r--   0        0        0      353 2024-02-20 00:15:13.185541 qualitative_coding-1.2.8/qualitative_coding/media_importers/verbatim.py
--rw-r--r--   0        0        0     1758 2024-02-20 00:15:13.185938 qualitative_coding-1.2.8/qualitative_coding/migrations/__init__.py
--rw-r--r--   0        0        0     1297 2024-02-20 00:15:13.186379 qualitative_coding-1.2.8/qualitative_coding/migrations/migration.py
--rw-r--r--   0        0        0      235 2024-02-20 00:15:13.186910 qualitative_coding-1.2.8/qualitative_coding/migrations/migration_0_2_3.py
--rw-r--r--   0        0        0     4779 2024-02-20 00:15:13.187298 qualitative_coding-1.2.8/qualitative_coding/migrations/migration_1_0_0.py
--rw-r--r--   0        0        0     7192 2024-03-12 15:05:27.818639 qualitative_coding-1.2.8/qualitative_coding/refi_qda/reader.py
--rw-r--r--   0        0        0    26395 2024-03-12 15:05:27.819881 qualitative_coding-1.2.8/qualitative_coding/refi_qda/schema.xsd
--rw-r--r--   0        0        0     6700 2024-03-12 15:05:27.821709 qualitative_coding-1.2.8/qualitative_coding/refi_qda/writer.py
--rw-r--r--   0        0        0        0 2024-02-23 20:28:22.232030 qualitative_coding-1.2.8/qualitative_coding/tests/__init__.py
--rw-r--r--   0        0        0     5376 2024-03-13 17:38:55.890252 qualitative_coding-1.2.8/qualitative_coding/tests/fixtures.py
--rwxr-xr-x   0        0        0     1764 2024-02-25 14:55:54.222091 qualitative_coding-1.2.8/qualitative_coding/tests/mock_editor.py
--rw-r--r--   0        0        0     1272 2024-03-10 23:28:47.301794 qualitative_coding-1.2.8/qualitative_coding/tests/test_check.py
--rw-r--r--   0        0        0     1435 2024-03-13 17:43:57.402983 qualitative_coding-1.2.8/qualitative_coding/tests/test_code.py
--rw-r--r--   0        0        0     1622 2024-02-25 14:55:54.222645 qualitative_coding-1.2.8/qualitative_coding/tests/test_code_parsing.py
--rw-r--r--   0        0        0      608 2024-02-20 18:16:30.592678 qualitative_coding-1.2.8/qualitative_coding/tests/test_codebook.py
--rw-r--r--   0        0        0      489 2024-02-20 18:16:30.593175 qualitative_coding-1.2.8/qualitative_coding/tests/test_coders.py
--rw-r--r--   0        0        0      889 2024-03-13 17:49:21.059115 qualitative_coding-1.2.8/qualitative_coding/tests/test_codes_crosstab.py
--rw-r--r--   0        0        0      606 2024-02-25 14:55:54.223096 qualitative_coding-1.2.8/qualitative_coding/tests/test_codes_find.py
--rw-r--r--   0        0        0     1015 2024-02-20 18:16:30.594077 qualitative_coding-1.2.8/qualitative_coding/tests/test_codes_list.py
--rw-r--r--   0        0        0      805 2024-02-20 18:16:30.594499 qualitative_coding-1.2.8/qualitative_coding/tests/test_codes_rename.py
--rw-r--r--   0        0        0     1646 2024-03-14 01:25:32.455628 qualitative_coding-1.2.8/qualitative_coding/tests/test_codes_stats.py
--rw-r--r--   0        0        0     2663 2024-02-25 14:55:54.223410 qualitative_coding-1.2.8/qualitative_coding/tests/test_corpus_import.py
--rw-r--r--   0        0        0     1501 2024-02-25 14:55:54.223880 qualitative_coding-1.2.8/qualitative_coding/tests/test_corpus_move.py
--rw-r--r--   0        0        0      655 2024-03-12 15:05:27.823674 qualitative_coding-1.2.8/qualitative_coding/tests/test_corpus_remove.py
--rw-r--r--   0        0        0      440 2024-03-12 15:05:27.824552 qualitative_coding-1.2.8/qualitative_coding/tests/test_export.py
--rw-r--r--   0        0        0     1561 2024-02-20 19:35:33.608542 qualitative_coding-1.2.8/qualitative_coding/tests/test_init.py
--rw-r--r--   0        0        0     1270 2024-03-12 15:05:27.825269 qualitative_coding-1.2.8/qualitative_coding/tests/test_init_import.py
--rw-r--r--   0        0        0      300 2024-02-20 13:17:05.364224 qualitative_coding-1.2.8/qualitative_coding/tests/test_memo.py
--rw-r--r--   0        0        0     1220 2024-03-12 15:05:27.826027 qualitative_coding-1.2.8/qualitative_coding/tests/test_refi_qda_writer.py
--rw-r--r--   0        0        0      849 2024-02-23 20:28:22.234574 qualitative_coding-1.2.8/qualitative_coding/tests/test_tree_node.py
--rw-r--r--   0        0        0      685 2024-02-20 13:17:05.358844 qualitative_coding-1.2.8/qualitative_coding/tests/test_upgrade.py
--rw-r--r--   0        0        0      313 2024-02-23 20:28:22.234832 qualitative_coding-1.2.8/qualitative_coding/tests/test_version.py
--rw-r--r--   0        0        0     6300 2024-02-23 15:06:25.209429 qualitative_coding-1.2.8/qualitative_coding/tree_node.py
--rw-r--r--   0        0        0      556 2023-12-07 20:04:17.916204 qualitative_coding-1.2.8/qualitative_coding/user_input.py
--rw-r--r--   0        0        0    12042 2024-02-11 22:24:40.952711 qualitative_coding-1.2.8/qualitative_coding/views/coding_ui.py
--rw-r--r--   0        0        0      910 2024-02-11 22:24:40.954722 qualitative_coding-1.2.8/qualitative_coding/views/styles.py
--rw-r--r--   0        0        0    31571 2024-03-18 13:10:07.602161 qualitative_coding-1.2.8/qualitative_coding/views/viewer.py
--rw-r--r--   0        0        0    14582 1970-01-01 00:00:00.000000 qualitative_coding-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0      781 2021-07-13 19:40:03.158793 qualitative_coding-1.2.9/LICENSE
+-rw-r--r--   0        0        0    13681 2024-03-12 15:05:27.802641 qualitative_coding-1.2.9/README.md
+-rw-r--r--   0        0        0      717 2024-03-23 02:58:23.658303 qualitative_coding-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1010 2024-03-12 15:05:27.805722 qualitative_coding-1.2.9/qualitative_coding/cli/__init__.py
+-rw-r--r--   0        0        0      498 2024-03-12 15:05:27.806804 qualitative_coding-1.2.9/qualitative_coding/cli/check.py
+-rw-r--r--   0        0        0     3278 2024-02-11 22:24:40.918879 qualitative_coding-1.2.9/qualitative_coding/cli/click_aliases.py
+-rw-r--r--   0        0        0     2182 2024-03-12 15:05:27.807580 qualitative_coding-1.2.9/qualitative_coding/cli/code.py
+-rw-r--r--   0        0        0      481 2024-03-12 15:05:27.808260 qualitative_coding-1.2.9/qualitative_coding/cli/codebook.py
+-rw-r--r--   0        0        0      664 2024-03-12 15:05:27.808807 qualitative_coding-1.2.9/qualitative_coding/cli/coders.py
+-rw-r--r--   0        0        0      649 2024-03-15 21:48:34.219106 qualitative_coding-1.2.9/qualitative_coding/cli/codes/__init__.py
+-rw-r--r--   0        0        0     3733 2024-03-14 01:20:49.652977 qualitative_coding-1.2.9/qualitative_coding/cli/codes/crosstab.py
+-rw-r--r--   0        0        0     2533 2024-03-16 17:56:09.955659 qualitative_coding-1.2.9/qualitative_coding/cli/codes/find.py
+-rw-r--r--   0        0        0      668 2024-03-12 15:05:27.810392 qualitative_coding-1.2.9/qualitative_coding/cli/codes/list.py
+-rw-r--r--   0        0        0     1010 2024-03-14 01:20:49.653588 qualitative_coding-1.2.9/qualitative_coding/cli/codes/rename.py
+-rw-r--r--   0        0        0     3551 2024-03-14 01:20:49.653928 qualitative_coding-1.2.9/qualitative_coding/cli/codes/stats.py
+-rw-r--r--   0        0        0      611 2024-03-12 15:05:27.811349 qualitative_coding-1.2.9/qualitative_coding/cli/corpus/__init__.py
+-rw-r--r--   0        0        0     1108 2024-03-12 15:05:27.812144 qualitative_coding-1.2.9/qualitative_coding/cli/corpus/import_media.py
+-rw-r--r--   0        0        0      620 2024-03-12 15:05:27.812691 qualitative_coding-1.2.9/qualitative_coding/cli/corpus/list.py
+-rw-r--r--   0        0        0      629 2024-03-12 15:05:27.813169 qualitative_coding-1.2.9/qualitative_coding/cli/corpus/move.py
+-rw-r--r--   0        0        0      581 2024-03-12 15:05:27.814175 qualitative_coding-1.2.9/qualitative_coding/cli/corpus/remove.py
+-rw-r--r--   0        0        0      611 2024-02-20 00:15:13.174056 qualitative_coding-1.2.9/qualitative_coding/cli/decorators.py
+-rw-r--r--   0        0        0      651 2024-03-12 15:05:27.814632 qualitative_coding-1.2.9/qualitative_coding/cli/export.py
+-rw-r--r--   0        0        0      895 2024-03-12 15:05:27.815075 qualitative_coding-1.2.9/qualitative_coding/cli/init.py
+-rw-r--r--   0        0        0      836 2024-03-12 15:05:27.815550 qualitative_coding-1.2.9/qualitative_coding/cli/memo.py
+-rw-r--r--   0        0        0     1575 2024-02-11 22:24:40.931614 qualitative_coding-1.2.9/qualitative_coding/cli/options.py
+-rw-r--r--   0        0        0      743 2024-03-12 15:05:27.816080 qualitative_coding-1.2.9/qualitative_coding/cli/upgrade.py
+-rw-r--r--   0        0        0      216 2024-02-11 22:24:40.936290 qualitative_coding-1.2.9/qualitative_coding/cli/version.py
+-rw-r--r--   0        0        0       96 2021-07-13 19:40:03.159583 qualitative_coding-1.2.9/qualitative_coding/codebook.py
+-rw-r--r--   0        0        0    36543 2024-03-14 01:20:49.654765 qualitative_coding-1.2.9/qualitative_coding/corpus.py
+-rw-r--r--   0        0        0       50 2024-02-11 22:24:40.939611 qualitative_coding-1.2.9/qualitative_coding/database/errors.py
+-rw-r--r--   0        0        0     3293 2024-03-12 15:05:27.817461 qualitative_coding-1.2.9/qualitative_coding/database/models.py
+-rw-r--r--   0        0        0      865 2024-02-23 21:08:31.319862 qualitative_coding-1.2.9/qualitative_coding/editors.py
+-rw-r--r--   0        0        0      210 2024-02-23 20:28:22.231952 qualitative_coding-1.2.9/qualitative_coding/exceptions.py
+-rw-r--r--   0        0        0     4220 2024-03-14 01:36:39.218279 qualitative_coding-1.2.9/qualitative_coding/helpers.py
+-rw-r--r--   0        0        0      895 2021-07-13 19:40:03.160344 qualitative_coding-1.2.9/qualitative_coding/logs.py
+-rw-r--r--   0        0        0      288 2024-02-11 22:24:40.943568 qualitative_coding-1.2.9/qualitative_coding/media_importers/__init__.py
+-rw-r--r--   0        0        0      560 2024-02-20 00:15:13.183338 qualitative_coding-1.2.9/qualitative_coding/media_importers/base.py
+-rw-r--r--   0        0        0      335 2024-02-20 19:36:20.339419 qualitative_coding-1.2.9/qualitative_coding/media_importers/pandoc.py
+-rw-r--r--   0        0        0      353 2024-02-20 00:15:13.185541 qualitative_coding-1.2.9/qualitative_coding/media_importers/verbatim.py
+-rw-r--r--   0        0        0     1758 2024-02-20 00:15:13.185938 qualitative_coding-1.2.9/qualitative_coding/migrations/__init__.py
+-rw-r--r--   0        0        0     1297 2024-02-20 00:15:13.186379 qualitative_coding-1.2.9/qualitative_coding/migrations/migration.py
+-rw-r--r--   0        0        0      235 2024-02-20 00:15:13.186910 qualitative_coding-1.2.9/qualitative_coding/migrations/migration_0_2_3.py
+-rw-r--r--   0        0        0     4779 2024-02-20 00:15:13.187298 qualitative_coding-1.2.9/qualitative_coding/migrations/migration_1_0_0.py
+-rw-r--r--   0        0        0     7192 2024-03-12 15:05:27.818639 qualitative_coding-1.2.9/qualitative_coding/refi_qda/reader.py
+-rw-r--r--   0        0        0    26395 2024-03-12 15:05:27.819881 qualitative_coding-1.2.9/qualitative_coding/refi_qda/schema.xsd
+-rw-r--r--   0        0        0     6700 2024-03-12 15:05:27.821709 qualitative_coding-1.2.9/qualitative_coding/refi_qda/writer.py
+-rw-r--r--   0        0        0        0 2024-02-23 20:28:22.232030 qualitative_coding-1.2.9/qualitative_coding/tests/__init__.py
+-rw-r--r--   0        0        0     5376 2024-03-13 17:38:55.890252 qualitative_coding-1.2.9/qualitative_coding/tests/fixtures.py
+-rwxr-xr-x   0        0        0     1764 2024-02-25 14:55:54.222091 qualitative_coding-1.2.9/qualitative_coding/tests/mock_editor.py
+-rw-r--r--   0        0        0     1272 2024-03-10 23:28:47.301794 qualitative_coding-1.2.9/qualitative_coding/tests/test_check.py
+-rw-r--r--   0        0        0     1435 2024-03-13 17:43:57.402983 qualitative_coding-1.2.9/qualitative_coding/tests/test_code.py
+-rw-r--r--   0        0        0     1622 2024-02-25 14:55:54.222645 qualitative_coding-1.2.9/qualitative_coding/tests/test_code_parsing.py
+-rw-r--r--   0        0        0      608 2024-02-20 18:16:30.592678 qualitative_coding-1.2.9/qualitative_coding/tests/test_codebook.py
+-rw-r--r--   0        0        0      489 2024-02-20 18:16:30.593175 qualitative_coding-1.2.9/qualitative_coding/tests/test_coders.py
+-rw-r--r--   0        0        0      889 2024-03-13 17:49:21.059115 qualitative_coding-1.2.9/qualitative_coding/tests/test_codes_crosstab.py
+-rw-r--r--   0        0        0      606 2024-02-25 14:55:54.223096 qualitative_coding-1.2.9/qualitative_coding/tests/test_codes_find.py
+-rw-r--r--   0        0        0     1015 2024-02-20 18:16:30.594077 qualitative_coding-1.2.9/qualitative_coding/tests/test_codes_list.py
+-rw-r--r--   0        0        0      805 2024-02-20 18:16:30.594499 qualitative_coding-1.2.9/qualitative_coding/tests/test_codes_rename.py
+-rw-r--r--   0        0        0     1646 2024-03-14 01:25:32.455628 qualitative_coding-1.2.9/qualitative_coding/tests/test_codes_stats.py
+-rw-r--r--   0        0        0     2663 2024-02-25 14:55:54.223410 qualitative_coding-1.2.9/qualitative_coding/tests/test_corpus_import.py
+-rw-r--r--   0        0        0     1501 2024-02-25 14:55:54.223880 qualitative_coding-1.2.9/qualitative_coding/tests/test_corpus_move.py
+-rw-r--r--   0        0        0      655 2024-03-12 15:05:27.823674 qualitative_coding-1.2.9/qualitative_coding/tests/test_corpus_remove.py
+-rw-r--r--   0        0        0      440 2024-03-12 15:05:27.824552 qualitative_coding-1.2.9/qualitative_coding/tests/test_export.py
+-rw-r--r--   0        0        0     1561 2024-02-20 19:35:33.608542 qualitative_coding-1.2.9/qualitative_coding/tests/test_init.py
+-rw-r--r--   0        0        0     1270 2024-03-12 15:05:27.825269 qualitative_coding-1.2.9/qualitative_coding/tests/test_init_import.py
+-rw-r--r--   0        0        0      300 2024-02-20 13:17:05.364224 qualitative_coding-1.2.9/qualitative_coding/tests/test_memo.py
+-rw-r--r--   0        0        0     1220 2024-03-12 15:05:27.826027 qualitative_coding-1.2.9/qualitative_coding/tests/test_refi_qda_writer.py
+-rw-r--r--   0        0        0      849 2024-02-23 20:28:22.234574 qualitative_coding-1.2.9/qualitative_coding/tests/test_tree_node.py
+-rw-r--r--   0        0        0      685 2024-02-20 13:17:05.358844 qualitative_coding-1.2.9/qualitative_coding/tests/test_upgrade.py
+-rw-r--r--   0        0        0      313 2024-02-23 20:28:22.234832 qualitative_coding-1.2.9/qualitative_coding/tests/test_version.py
+-rw-r--r--   0        0        0     6300 2024-02-23 15:06:25.209429 qualitative_coding-1.2.9/qualitative_coding/tree_node.py
+-rw-r--r--   0        0        0      556 2023-12-07 20:04:17.916204 qualitative_coding-1.2.9/qualitative_coding/user_input.py
+-rw-r--r--   0        0        0    12042 2024-02-11 22:24:40.952711 qualitative_coding-1.2.9/qualitative_coding/views/coding_ui.py
+-rw-r--r--   0        0        0      910 2024-02-11 22:24:40.954722 qualitative_coding-1.2.9/qualitative_coding/views/styles.py
+-rw-r--r--   0        0        0    31597 2024-03-23 02:57:53.554336 qualitative_coding-1.2.9/qualitative_coding/views/viewer.py
+-rw-r--r--   0        0        0    14582 1970-01-01 00:00:00.000000 qualitative_coding-1.2.9/PKG-INFO
```

### Comparing `qualitative_coding-1.2.8/LICENSE` & `qualitative_coding-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/README.md` & `qualitative_coding-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/pyproject.toml` & `qualitative_coding-1.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qualitative-coding"
-version = "1.2.8"
+version = "1.2.9"
 description = "Qualitative coding tools for computer scientists"
 authors = ["Chris Proctor <chris@chrisproctor.net>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "qualitative_coding"}]
 include = ["refi_qda/schema.xml"]
```

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/__init__.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/click_aliases.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/click_aliases.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/code.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/code.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/coders.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/coders.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/codes/__init__.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/codes/__init__.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/codes/crosstab.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/codes/crosstab.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/codes/find.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/codes/find.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/codes/list.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/codes/list.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/codes/rename.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/codes/rename.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/codes/stats.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/codes/stats.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/corpus/__init__.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/corpus/import_media.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/corpus/import_media.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/corpus/list.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/corpus/list.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/corpus/move.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/corpus/move.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/corpus/remove.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/corpus/remove.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/decorators.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/export.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/export.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/init.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/init.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/memo.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/memo.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/options.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/options.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/cli/upgrade.py` & `qualitative_coding-1.2.9/qualitative_coding/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/corpus.py` & `qualitative_coding-1.2.9/qualitative_coding/corpus.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/database/models.py` & `qualitative_coding-1.2.9/qualitative_coding/database/models.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/editors.py` & `qualitative_coding-1.2.9/qualitative_coding/editors.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/helpers.py` & `qualitative_coding-1.2.9/qualitative_coding/helpers.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/logs.py` & `qualitative_coding-1.2.9/qualitative_coding/logs.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/media_importers/base.py` & `qualitative_coding-1.2.9/qualitative_coding/media_importers/base.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/migrations/__init__.py` & `qualitative_coding-1.2.9/qualitative_coding/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/migrations/migration.py` & `qualitative_coding-1.2.9/qualitative_coding/migrations/migration.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/migrations/migration_1_0_0.py` & `qualitative_coding-1.2.9/qualitative_coding/migrations/migration_1_0_0.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/refi_qda/reader.py` & `qualitative_coding-1.2.9/qualitative_coding/refi_qda/reader.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/refi_qda/schema.xsd` & `qualitative_coding-1.2.9/qualitative_coding/refi_qda/schema.xsd`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/refi_qda/writer.py` & `qualitative_coding-1.2.9/qualitative_coding/refi_qda/writer.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/fixtures.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/mock_editor.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/mock_editor.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_check.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_code.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_code_parsing.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_code_parsing.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_codebook.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_codebook.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_codes_crosstab.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_codes_crosstab.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_codes_find.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_codes_find.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_codes_list.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_codes_list.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_codes_rename.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_codes_rename.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_codes_stats.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_codes_stats.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_corpus_import.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_corpus_import.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_corpus_move.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_corpus_move.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_corpus_remove.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_corpus_remove.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_init.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_init_import.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_init_import.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_refi_qda_writer.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_refi_qda_writer.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_tree_node.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_tree_node.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tests/test_upgrade.py` & `qualitative_coding-1.2.9/qualitative_coding/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/tree_node.py` & `qualitative_coding-1.2.9/qualitative_coding/tree_node.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/user_input.py` & `qualitative_coding-1.2.9/qualitative_coding/user_input.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/views/coding_ui.py` & `qualitative_coding-1.2.9/qualitative_coding/views/coding_ui.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/views/styles.py` & `qualitative_coding-1.2.9/qualitative_coding/views/styles.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.2.8/qualitative_coding/views/viewer.py` & `qualitative_coding-1.2.9/qualitative_coding/views/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                     codes=codes, 
                     coders=coders,
                     recursive_codes=recursive_codes, 
                     depth=depth,
                     pattern=pattern,
                     file_list=file_list,
                     unit=unit,
-                    totals=True
+                    totals=recursive_counts,
                 )
                 if coders:
                     all_coders = sorted(coders)
                 else:
                     all_coders = sorted(c.name for c in self.corpus.get_all_coders())
                 cols = all_coders + ["Total"]
                 results = []
@@ -123,15 +123,15 @@
                     codes=codes, 
                     coders=coders,
                     recursive_codes=recursive_codes, 
                     depth=depth,
                     pattern=pattern,
                     file_list=file_list,
                     unit=unit,
-                    totals=True
+                    totals=recursive_counts,
                 )
                 all_docs = self.corpus.get_documents(pattern=pattern, file_list=file_list)
                 all_docs = sorted(d.file_path for d in all_docs)
                 cols = all_docs + ["Total"]
                 results = []
                 for n in nodes:
                     row = []
```

### Comparing `qualitative_coding-1.2.8/PKG-INFO` & `qualitative_coding-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualitative-coding
-Version: 1.2.8
+Version: 1.2.9
 Summary: Qualitative coding tools for computer scientists
 License: MIT
 Author: Chris Proctor
 Author-email: chris@chrisproctor.net
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

