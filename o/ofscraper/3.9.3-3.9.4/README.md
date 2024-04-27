# Comparing `tmp/ofscraper-3.9.3.tar.gz` & `tmp/ofscraper-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.9.3.tar", max compression
+gzip compressed data, was "ofscraper-3.9.4.tar", max compression
```

## Comparing `ofscraper-3.9.3.tar` & `ofscraper-3.9.4.tar`

### file list

```diff
@@ -1,189 +1,188 @@
--rw-r--r--   0        0        0     1067 2024-04-25 22:48:22.868404 ofscraper-3.9.3/LICENSE
--rw-r--r--   0        0        0     4213 2024-04-25 22:48:22.868404 ofscraper-3.9.3/README.md
--rwxr-xr-x   0        0        0      283 2024-04-25 22:48:22.872404 ofscraper-3.9.3/ofscraper/__main__.py
--rw-r--r--   0        0        0     1064 2024-04-25 22:48:22.872404 ofscraper-3.9.3/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2024-04-25 22:48:22.872404 ofscraper-3.9.3/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2024-04-25 22:48:22.872404 ofscraper-3.9.3/ofscraper/actions/__init__.py
--rw-r--r--   0        0        0     8505 2024-04-25 22:48:22.872404 ofscraper-3.9.3/ofscraper/actions/like.py
--rw-r--r--   0        0        0    10057 2024-04-25 22:48:22.872404 ofscraper-3.9.3/ofscraper/actions/process.py
--rw-r--r--   0        0        0    21651 2024-04-25 22:48:22.872404 ofscraper-3.9.3/ofscraper/actions/scraper.py
--rw-r--r--   0        0        0    15640 2024-04-25 22:48:22.872404 ofscraper-3.9.3/ofscraper/api/archive.py
--rw-r--r--   0        0        0      274 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/common/logs.py
--rw-r--r--   0        0        0    14646 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1479 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/init.py
--rw-r--r--   0        0        0    14203 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/labels.py
--rw-r--r--   0        0        0     2912 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/me.py
--rw-r--r--   0        0        0    18732 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/messages.py
--rw-r--r--   0        0        0    13861 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/paid.py
--rw-r--r--   0        0        0     8091 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     6180 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1718 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/subscriptions/helpers.py
--rw-r--r--   0        0        0     3275 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/subscriptions/individual.py
--rw-r--r--   0        0        0    12660 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/subscriptions/lists.py
--rw-r--r--   0        0        0     8171 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/subscriptions/subscriptions.py
--rw-r--r--   0        0        0    16611 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     1453 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/classes/base.py
--rw-r--r--   0        0        0      876 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/classes/labels.py
--rw-r--r--   0        0        0    15553 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/classes/media.py
--rw-r--r--   0        0        0     6005 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/classes/models.py
--rw-r--r--   0        0        0     1771 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0    20557 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     5156 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/classes/posts.py
--rw-r--r--   0        0        0      456 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/classes/semaphoreDelayed.py
--rw-r--r--   0        0        0    18103 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/classes/sessionmanager.py
--rw-r--r--   0        0        0    31979 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/classes/table.py
--rw-r--r--   0        0        0    26079 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/commands/check.py
--rw-r--r--   0        0        0    11014 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/commands/manual.py
--rw-r--r--   0        0        0      430 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/commands/picker.py
--rwxr-xr-x   0        0        0     3810 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0       53 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/binary.py
--rw-r--r--   0        0        0     1655 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/config.py
--rw-r--r--   0        0        0      966 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/constants.py
--rw-r--r--   0        0        0       74 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/date.py
--rw-r--r--   0        0        0      184 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/download.py
--rw-r--r--   0        0        0      204 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/files.py
--rw-r--r--   0        0        0     1333 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/general.py
--rw-r--r--   0        0        0       93 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/logger.py
--rw-r--r--   0        0        0       69 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/metadata.py
--rw-r--r--   0        0        0      862 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/other_url.py
--rw-r--r--   0        0        0     1908 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/prompts.py
--rw-r--r--   0        0        0     1743 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/req.py
--rw-r--r--   0        0        0   265533 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/test_constants.py
--rw-r--r--   0        0        0      248 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/time.py
--rw-r--r--   0        0        0     3594 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/const/url.py
--rw-r--r--   0        0        0        1 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    15585 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/db/operations.py
--rw-r--r--   0        0        0      206 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/db/operations_/helpers.py
--rw-r--r--   0        0        0     8568 2024-04-25 22:48:22.876404 ofscraper-3.9.3/ofscraper/db/operations_/labels.py
--rw-r--r--   0        0        0    19112 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/db/operations_/media.py
--rw-r--r--   0        0        0    11056 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/db/operations_/merge.py
--rw-r--r--   0        0        0     8504 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/db/operations_/messages.py
--rw-r--r--   0        0        0     8928 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/db/operations_/others.py
--rw-r--r--   0        0        0    10366 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/db/operations_/posts.py
--rw-r--r--   0        0        0     6720 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/db/operations_/profile.py
--rw-r--r--   0        0        0     7485 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/db/operations_/stories.py
--rw-r--r--   0        0        0     4810 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/db/operations_/wrapper.py
--rw-r--r--   0        0        0    10881 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/alt_download.py
--rw-r--r--   0        0        0    10682 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/alt_downloadbatch.py
--rw-r--r--   0        0        0     4930 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/download.py
--rw-r--r--   0        0        0    17167 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/downloadbatch.py
--rw-r--r--   0        0        0     9077 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/downloadnormal.py
--rw-r--r--   0        0        0    10787 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/main_download.py
--rw-r--r--   0        0        0    11235 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/main_downloadbatch.py
--rw-r--r--   0        0        0     1414 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/classes/retries.py
--rw-r--r--   0        0        0     1356 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/classes/session.py
--rw-r--r--   0        0        0     3796 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/common/alt_common.py
--rw-r--r--   0        0        0     6372 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/common/general.py
--rw-r--r--   0        0        0     2063 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/common/main_common.py
--rw-r--r--   0        0        0     2404 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/globals.py
--rw-r--r--   0        0        0     9440 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/utils/keyhelpers.py
--rw-r--r--   0        0        0     3431 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/utils/log.py
--rw-r--r--   0        0        0      317 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/utils/media.py
--rw-r--r--   0        0        0      790 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/utils/message.py
--rw-r--r--   0        0        0     3927 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/utils/metadata.py
--rw-r--r--   0        0        0     2590 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/utils/paths.py
--rw-r--r--   0        0        0      453 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/utils/progress.py
--rw-r--r--   0        0        0     1155 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/download/shared/utils/text.py
--rw-r--r--   0        0        0     8075 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/filters/media/helpers.py
--rw-r--r--   0        0        0     5019 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/filters/media/main.py
--rw-r--r--   0        0        0     3136 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/filters/models/date.py
--rw-r--r--   0        0        0     3143 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/filters/models/flags.py
--rw-r--r--   0        0        0      957 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/filters/models/helpers.py
--rw-r--r--   0        0        0      726 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/filters/models/other.py
--rw-r--r--   0        0        0     7561 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/filters/models/price.py
--rw-r--r--   0        0        0     1538 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/filters/models/sort.py
--rw-r--r--   0        0        0     1454 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/filters/models/subtype.py
--rw-r--r--   0        0        0     3457 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/models/retriver.py
--rw-r--r--   0        0        0     8011 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/models/selector.py
--rw-r--r--   0        0        0     2466 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/helpers/model_helpers.py
--rw-r--r--   0        0        0    15219 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/helpers/prompt_helpers.py
--rw-r--r--   0        0        0      846 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     7747 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0      917 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompt_groups/actions.py
--rw-r--r--   0        0        0     6595 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompt_groups/area.py
--rw-r--r--   0        0        0     8257 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompt_groups/auth.py
--rw-r--r--   0        0        0     4438 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompt_groups/binary.py
--rw-r--r--   0        0        0    27895 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompt_groups/config.py
--rw-r--r--   0        0        0     1879 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompt_groups/menu.py
--rw-r--r--   0        0        0     2682 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompt_groups/merge.py
--rw-r--r--   0        0        0    16090 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompt_groups/model.py
--rw-r--r--   0        0        0     4135 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompt_groups/profile.py
--rw-r--r--   0        0        0     7609 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    10346 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0     1342 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      567 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/runner/exit.py
--rw-r--r--   0        0        0     1578 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/runner/load.py
--rw-r--r--   0        0        0     2743 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/runner/run.py
--rw-r--r--   0        0        0        1 2024-04-25 22:48:22.880404 ofscraper-3.9.3/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3803 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/actions.py
--rw-r--r--   0        0        0     1838 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/areas.py
--rw-r--r--   0        0        0       12 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/globals.py
--rw-r--r--   0        0        0     6624 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/groups/common_args.py
--rw-r--r--   0        0        0    20010 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/groups/main_args.py
--rw-r--r--   0        0        0     1318 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/groups/manual_args.py
--rw-r--r--   0        0        0     1587 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/groups/message_args.py
--rw-r--r--   0        0        0     1588 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/groups/paid_args.py
--rw-r--r--   0        0        0     1955 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/groups/post_args.py
--rw-r--r--   0        0        0     1641 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/groups/story_args.py
--rw-r--r--   0        0        0     5571 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/helpers.py
--rw-r--r--   0        0        0     1928 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/parse.py
--rw-r--r--   0        0        0      395 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/quality.py
--rw-r--r--   0        0        0      863 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/read.py
--rw-r--r--   0        0        0      721 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/user.py
--rw-r--r--   0        0        0      261 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/args/write.py
--rw-r--r--   0        0        0     2148 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/auth/context.py
--rw-r--r--   0        0        0     1680 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/auth/data.py
--rw-r--r--   0        0        0     2034 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/auth/file.py
--rw-r--r--   0        0        0     2844 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/auth/helpers.py
--rw-r--r--   0        0        0     1669 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/auth/make.py
--rw-r--r--   0        0        0     6902 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/auth/request.py
--rw-r--r--   0        0        0      802 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/auth/schema.py
--rw-r--r--   0        0        0     9824 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0     1780 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/cache.py
--rw-r--r--   0        0        0     1612 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/checkers.py
--rw-r--r--   0        0        0     2856 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/config/config.py
--rw-r--r--   0        0        0     1442 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/config/context.py
--rw-r--r--   0        0        0      522 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/config/custom.py
--rw-r--r--   0        0        0    24693 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/config/data.py
--rw-r--r--   0        0        0     2146 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/config/file.py
--rw-r--r--   0        0        0     2073 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/config/menu.py
--rw-r--r--   0        0        0     4797 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/config/schema.py
--rw-r--r--   0        0        0      409 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/config/wrapper.py
--rw-r--r--   0        0        0      499 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/console.py
--rw-r--r--   0        0        0      788 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/constants.py
--rw-r--r--   0        0        0     3401 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/context/exit.py
--rw-r--r--   0        0        0     1135 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/context/run_async.py
--rw-r--r--   0        0        0     1004 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/context/stdout.py
--rw-r--r--   0        0        0     3460 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/dates.py
--rw-r--r--   0        0        0     1040 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     1781 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/hash.py
--rw-r--r--   0        0        0     7226 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/logs/classes.py
--rw-r--r--   0        0        0     2588 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/logs/close.py
--rw-r--r--   0        0        0      477 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/logs/globals.py
--rw-r--r--   0        0        0     1670 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/logs/helpers.py
--rw-r--r--   0        0        0     2098 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/logs/logger.py
--rw-r--r--   0        0        0     1672 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/logs/logs.py
--rw-r--r--   0        0        0     5955 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/logs/other.py
--rw-r--r--   0        0        0     3652 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/logs/stdout.py
--rw-r--r--   0        0        0      601 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/manager.py
--rw-r--r--   0        0        0      388 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/me.py
--rw-r--r--   0        0        0     4161 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/menu.py
--rw-r--r--   0        0        0      659 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/merge.py
--rw-r--r--   0        0        0     1710 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/paths/check.py
--rw-r--r--   0        0        0     3091 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/paths/common.py
--rw-r--r--   0        0        0      279 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/paths/manage.py
--rw-r--r--   0        0        0     5222 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/paths/paths.py
--rw-r--r--   0        0        0     1034 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/profiles/data.py
--rw-r--r--   0        0        0     2785 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/profiles/manage.py
--rw-r--r--   0        0        0     1583 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/profiles/tools.py
--rw-r--r--   0        0        0    10893 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/progress.py
--rw-r--r--   0        0        0     4406 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/run.py
--rw-r--r--   0        0        0        1 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/sems.py
--rw-r--r--   0        0        0     1595 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     4038 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/settings.py
--rw-r--r--   0        0        0      417 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/system/free.py
--rw-r--r--   0        0        0     3279 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/system/network.py
--rw-r--r--   0        0        0     2472 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/system/system.py
--rw-r--r--   0        0        0     2002 2024-04-25 22:48:22.884404 ofscraper-3.9.3/ofscraper/utils/text.py
--rw-r--r--   0        0        0     2117 2024-04-25 22:48:52.028364 ofscraper-3.9.3/pyproject.toml
--rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 ofscraper-3.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-27 15:37:09.008659 ofscraper-3.9.4/LICENSE
+-rw-r--r--   0        0        0     4213 2024-04-27 15:37:09.008659 ofscraper-3.9.4/README.md
+-rwxr-xr-x   0        0        0      283 2024-04-27 15:37:09.012659 ofscraper-3.9.4/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1064 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/__version__.pye
+-rw-r--r--   0        0        0        1 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/actions/__init__.py
+-rw-r--r--   0        0        0     8505 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/actions/like.py
+-rw-r--r--   0        0        0    10057 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/actions/process.py
+-rw-r--r--   0        0        0    21651 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/actions/scraper.py
+-rw-r--r--   0        0        0    15624 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/archive.py
+-rw-r--r--   0        0        0      274 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/common/logs.py
+-rw-r--r--   0        0        0    14646 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1479 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/init.py
+-rw-r--r--   0        0        0    14203 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2912 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/me.py
+-rw-r--r--   0        0        0    18946 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    13861 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     8091 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     6180 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1718 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/subscriptions/helpers.py
+-rw-r--r--   0        0        0     3275 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/subscriptions/individual.py
+-rw-r--r--   0        0        0    12660 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/subscriptions/lists.py
+-rw-r--r--   0        0        0     8171 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/subscriptions/subscriptions.py
+-rw-r--r--   0        0        0    16613 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     1460 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/base.py
+-rw-r--r--   0        0        0      876 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0    15560 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     6005 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/models.py
+-rw-r--r--   0        0        0     1771 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0    20557 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     5156 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0    18324 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/sessionmanager.py
+-rw-r--r--   0        0        0    31979 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    26079 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/commands/check.py
+-rw-r--r--   0        0        0    11014 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/commands/manual.py
+-rw-r--r--   0        0        0      430 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/commands/picker.py
+-rwxr-xr-x   0        0        0     3810 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0       53 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/binary.py
+-rw-r--r--   0        0        0     1655 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/config.py
+-rw-r--r--   0        0        0      966 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/constants.py
+-rw-r--r--   0        0        0       74 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/date.py
+-rw-r--r--   0        0        0      190 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/download.py
+-rw-r--r--   0        0        0      204 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/files.py
+-rw-r--r--   0        0        0     1333 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/general.py
+-rw-r--r--   0        0        0       93 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/logger.py
+-rw-r--r--   0        0        0       69 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/metadata.py
+-rw-r--r--   0        0        0      862 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/other_url.py
+-rw-r--r--   0        0        0     1908 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/prompts.py
+-rw-r--r--   0        0        0     1804 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/req.py
+-rw-r--r--   0        0        0   265533 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/const/test_constants.py
+-rw-r--r--   0        0        0      248 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/const/time.py
+-rw-r--r--   0        0        0     3594 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/const/url.py
+-rw-r--r--   0        0        0        1 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    15585 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations.py
+-rw-r--r--   0        0        0      206 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/helpers.py
+-rw-r--r--   0        0        0     8568 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/labels.py
+-rw-r--r--   0        0        0    19112 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/media.py
+-rw-r--r--   0        0        0    11270 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/merge.py
+-rw-r--r--   0        0        0     8504 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/messages.py
+-rw-r--r--   0        0        0     8928 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/others.py
+-rw-r--r--   0        0        0    10366 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/posts.py
+-rw-r--r--   0        0        0     6725 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/profile.py
+-rw-r--r--   0        0        0     7485 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/stories.py
+-rw-r--r--   0        0        0     4810 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/wrapper.py
+-rw-r--r--   0        0        0    10881 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/alt_download.py
+-rw-r--r--   0        0        0    10682 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/alt_downloadbatch.py
+-rw-r--r--   0        0        0     4930 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/download.py
+-rw-r--r--   0        0        0    17167 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/downloadbatch.py
+-rw-r--r--   0        0        0     9077 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/downloadnormal.py
+-rw-r--r--   0        0        0    10787 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/main_download.py
+-rw-r--r--   0        0        0    11235 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/main_downloadbatch.py
+-rw-r--r--   0        0        0     1414 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/classes/retries.py
+-rw-r--r--   0        0        0     1356 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/classes/session.py
+-rw-r--r--   0        0        0     3796 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/common/alt_common.py
+-rw-r--r--   0        0        0     6372 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/common/general.py
+-rw-r--r--   0        0        0     2063 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/common/main_common.py
+-rw-r--r--   0        0        0     2341 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/globals.py
+-rw-r--r--   0        0        0     9440 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/keyhelpers.py
+-rw-r--r--   0        0        0     3431 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/log.py
+-rw-r--r--   0        0        0      317 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/media.py
+-rw-r--r--   0        0        0      790 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/message.py
+-rw-r--r--   0        0        0     3927 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/metadata.py
+-rw-r--r--   0        0        0     2590 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/paths.py
+-rw-r--r--   0        0        0      453 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/progress.py
+-rw-r--r--   0        0        0     1155 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/text.py
+-rw-r--r--   0        0        0     8075 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/media/helpers.py
+-rw-r--r--   0        0        0     5019 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/media/main.py
+-rw-r--r--   0        0        0     3136 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/date.py
+-rw-r--r--   0        0        0     3143 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/flags.py
+-rw-r--r--   0        0        0      957 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/helpers.py
+-rw-r--r--   0        0        0      726 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/other.py
+-rw-r--r--   0        0        0     7561 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/price.py
+-rw-r--r--   0        0        0     1538 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/sort.py
+-rw-r--r--   0        0        0     1454 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/subtype.py
+-rw-r--r--   0        0        0     3457 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/models/retriver.py
+-rw-r--r--   0        0        0     8011 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/models/selector.py
+-rw-r--r--   0        0        0     2466 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/helpers/model_helpers.py
+-rw-r--r--   0        0        0    15219 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/helpers/prompt_helpers.py
+-rw-r--r--   0        0        0      846 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     7747 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0      917 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/actions.py
+-rw-r--r--   0        0        0     6595 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/area.py
+-rw-r--r--   0        0        0     8257 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/auth.py
+-rw-r--r--   0        0        0     4438 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/binary.py
+-rw-r--r--   0        0        0    27915 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/config.py
+-rw-r--r--   0        0        0     1879 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/menu.py
+-rw-r--r--   0        0        0     2740 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/merge.py
+-rw-r--r--   0        0        0    16090 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/model.py
+-rw-r--r--   0        0        0     4135 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/profile.py
+-rw-r--r--   0        0        0     7609 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    10346 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0     1342 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      567 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/runner/exit.py
+-rw-r--r--   0        0        0     1578 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/runner/load.py
+-rw-r--r--   0        0        0     2743 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/runner/run.py
+-rw-r--r--   0        0        0        1 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3803 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/actions.py
+-rw-r--r--   0        0        0     1838 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/areas.py
+-rw-r--r--   0        0        0       12 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/globals.py
+-rw-r--r--   0        0        0     7512 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/common_args.py
+-rw-r--r--   0        0        0    20038 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/main_args.py
+-rw-r--r--   0        0        0     1318 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/manual_args.py
+-rw-r--r--   0        0        0     1587 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/message_args.py
+-rw-r--r--   0        0        0     1588 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/paid_args.py
+-rw-r--r--   0        0        0     1955 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/post_args.py
+-rw-r--r--   0        0        0     1641 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/story_args.py
+-rw-r--r--   0        0        0     5571 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/helpers.py
+-rw-r--r--   0        0        0     1928 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/parse.py
+-rw-r--r--   0        0        0      395 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/quality.py
+-rw-r--r--   0        0        0      863 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/read.py
+-rw-r--r--   0        0        0      721 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/user.py
+-rw-r--r--   0        0        0      261 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/write.py
+-rw-r--r--   0        0        0     2148 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/context.py
+-rw-r--r--   0        0        0     1680 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/data.py
+-rw-r--r--   0        0        0     2034 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/file.py
+-rw-r--r--   0        0        0     2844 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/helpers.py
+-rw-r--r--   0        0        0     1669 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/make.py
+-rw-r--r--   0        0        0     6902 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/request.py
+-rw-r--r--   0        0        0      802 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/schema.py
+-rw-r--r--   0        0        0     9824 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0     1780 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/cache.py
+-rw-r--r--   0        0        0     1612 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/checkers.py
+-rw-r--r--   0        0        0     2856 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/config.py
+-rw-r--r--   0        0        0     1442 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/context.py
+-rw-r--r--   0        0        0      522 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/custom.py
+-rw-r--r--   0        0        0    24693 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/data.py
+-rw-r--r--   0        0        0     2146 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/file.py
+-rw-r--r--   0        0        0     2073 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/menu.py
+-rw-r--r--   0        0        0     4797 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/schema.py
+-rw-r--r--   0        0        0      409 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/wrapper.py
+-rw-r--r--   0        0        0      499 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      788 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/constants.py
+-rw-r--r--   0        0        0     3401 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/context/exit.py
+-rw-r--r--   0        0        0     1135 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/context/run_async.py
+-rw-r--r--   0        0        0     1004 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/context/stdout.py
+-rw-r--r--   0        0        0     3460 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0     1040 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     1781 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/hash.py
+-rw-r--r--   0        0        0     7226 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/classes.py
+-rw-r--r--   0        0        0     2588 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/close.py
+-rw-r--r--   0        0        0      477 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/globals.py
+-rw-r--r--   0        0        0     1670 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/helpers.py
+-rw-r--r--   0        0        0     2098 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/logger.py
+-rw-r--r--   0        0        0     1672 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/logs.py
+-rw-r--r--   0        0        0     5955 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/other.py
+-rw-r--r--   0        0        0     3652 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/stdout.py
+-rw-r--r--   0        0        0      601 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/manager.py
+-rw-r--r--   0        0        0      388 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/me.py
+-rw-r--r--   0        0        0     4161 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/menu.py
+-rw-r--r--   0        0        0      659 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/merge.py
+-rw-r--r--   0        0        0     1710 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/paths/check.py
+-rw-r--r--   0        0        0     3091 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/paths/common.py
+-rw-r--r--   0        0        0      279 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/paths/manage.py
+-rw-r--r--   0        0        0     5269 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/paths/paths.py
+-rw-r--r--   0        0        0     1034 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/profiles/data.py
+-rw-r--r--   0        0        0     2785 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/profiles/manage.py
+-rw-r--r--   0        0        0     1583 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/profiles/tools.py
+-rw-r--r--   0        0        0    10893 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/progress.py
+-rw-r--r--   0        0        0     4406 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/run.py
+-rw-r--r--   0        0        0        1 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/sems.py
+-rw-r--r--   0        0        0     1595 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     4680 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/settings.py
+-rw-r--r--   0        0        0      417 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/system/free.py
+-rw-r--r--   0        0        0     3279 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/system/network.py
+-rw-r--r--   0        0        0     2472 2024-04-27 15:37:09.028659 ofscraper-3.9.4/ofscraper/utils/system/system.py
+-rw-r--r--   0        0        0     2002 2024-04-27 15:37:09.028659 ofscraper-3.9.4/ofscraper/utils/text.py
+-rw-r--r--   0        0        0     2117 2024-04-27 15:37:34.264635 ofscraper-3.9.4/pyproject.toml
+-rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 ofscraper-3.9.4/PKG-INFO
```

### Comparing `ofscraper-3.9.3/LICENSE` & `ofscraper-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/README.md` & `ofscraper-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/__version__.py` & `ofscraper-3.9.4/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/__version__.pye` & `ofscraper-3.9.4/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/actions/like.py` & `ofscraper-3.9.4/ofscraper/actions/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/actions/process.py` & `ofscraper-3.9.4/ofscraper/actions/process.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/actions/scraper.py` & `ofscraper-3.9.4/ofscraper/actions/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/archive.py` & `ofscraper-3.9.4/ofscraper/api/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import logging
 import math
 import traceback
 
 import arrow
 
 import ofscraper.api.common.logs as common_logs
-import ofscraper.db.operations as operations
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
 from ofscraper.utils.context.run_async import run
 from ofscraper.utils.logs.helpers import is_trace
@@ -32,19 +31,19 @@
 
 sem = None
 
 
 @run
 async def get_archived_posts_progress(model_id, username, forced_after=None, c=None):
 
-    oldarchived = (
-        await get_archived_post_info(model_id=model_id, username=username)
-        if not read_args.retriveArgs().no_cache
-        else []
-    )
+    oldarchived = None
+    if not settings.get_api_cache_disabled():
+        oldarchived=await get_archived_post_info(model_id=model_id, username=username)
+    else:
+        oldarchived = []
     trace_log_old(oldarchived)
 
     log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
     oldarchived = list(filter(lambda x: x is not None, oldarchived))
     after = await get_after(model_id, username, forced_after)
     after_log(username, after)
     splitArrays = get_split_array(oldarchived, after)
@@ -52,19 +51,18 @@
     data = await process_tasks(tasks, model_id, after)
     progress_utils.archived_layout.visible = False
     return data
 
 
 @run
 async def get_archived_posts(model_id, username, forced_after=None, c=None):
-    oldarchived = (
-        await get_archived_post_info(model_id=model_id, username=username)
-        if not read_args.retriveArgs().no_cache
-        else []
-    )
+    if not settings.get_api_cache_disabled():
+        oldarchived=await get_archived_post_info(model_id=model_id, username=username)
+    else:
+        oldarchived = []
     trace_log_old(oldarchived)
 
     log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
     oldarchived = list(filter(lambda x: x is not None, oldarchived))
     after = await get_after(model_id, username, forced_after)
     after_log(username, after)
     with progress_utils.set_up_api_archived():
```

### Comparing `ofscraper-3.9.3/ofscraper/api/highlights.py` & `ofscraper-3.9.4/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/init.py` & `ofscraper-3.9.4/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/labels.py` & `ofscraper-3.9.4/ofscraper/api/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/me.py` & `ofscraper-3.9.4/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/messages.py` & `ofscraper-3.9.4/ofscraper/api/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,62 +15,64 @@
 import logging
 import traceback
 
 import arrow
 
 import ofscraper.api.common.logs as common_logs
 import ofscraper.classes.sessionmanager as sessionManager
-import ofscraper.db.operations as operations
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
 from ofscraper.utils.context.run_async import run
 from ofscraper.utils.logs.helpers import is_trace
 from ofscraper.db.operations_.messages import get_messages_post_info,get_youngest_message_date
 from ofscraper.db.operations_.media import get_messages_media
 
 
 
 log = logging.getLogger("shared")
+sleeper=None
+
 
 
 @run
 async def get_messages_progress(model_id, username, forced_after=None, c=None):
     global after
-
-    oldmessages = (
-        await get_messages_post_info(model_id=model_id, username=username)
-        if not read_args.retriveArgs().no_cache
-        else []
-    )
+    oldmessages=None
+    if not settings.get_api_cache_disabled():
+        oldmessages=await get_messages_post_info(model_id=model_id, username=username)
+    else:
+        oldmessages = []
     trace_log_old(oldmessages)
 
     before = (read_args.retriveArgs().before or arrow.now()).float_timestamp
     after = await get_after(model_id, username, forced_after)
     log_after_before(after, before, username)
 
     filteredArray = get_filterArray(after, before, oldmessages)
     splitArrays = get_split_array(filteredArray)
+    # Set charged sleeper
+    get_sleeper()
     tasks = get_tasks(splitArrays, filteredArray, oldmessages, model_id, c)
     data = await process_tasks(tasks, model_id)
     progress_utils.messages_layout.visible = False
     return data
 
 
 @run
 async def get_messages(model_id, username, forced_after=None, c=None):
     global after
 
-    oldmessages = (
-        await get_messages_post_info(model_id=model_id, username=username)
-        if not read_args.retriveArgs().no_cache
-        else []
-    )
+    oldmessages=None
+    if not settings.get_api_cache_disabled():
+        oldmessages=await get_messages_post_info(model_id=model_id, username=username)
+    else:
+        oldmessages = []
     trace_log_old(oldmessages)
 
     before = (read_args.retriveArgs().before or arrow.now()).float_timestamp
     after = await get_after(model_id, username, forced_after)
     log_after_before(after, before, username)
 
     log.info(
@@ -321,15 +323,15 @@
         else constants.getattr("messagesEP")
     )
     url = ep.format(model_id, message_id)
     log.debug(f"{message_id if message_id else 'init'} {url}")
     new_tasks = []
     await asyncio.sleep(1)
     try:
-        async with c.requests_async(url=url) as r:
+        async with c.requests_async(url=url, sleeper=get_sleeper()) as r:
             task = (
                 job_progress.add_task(
                     f": Message ID-> {message_id if message_id else 'initial'}"
                 )
                 if job_progress
                 else None
             )
@@ -516,7 +518,13 @@
         f"""
 Setting initial message scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
 [yellow]Hint: append ' --after 2000' to command to force scan of all messages + download of new files only[/yellow]
 [yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all messages + download/re-download of all files[/yellow]
 
         """
     )
+
+def get_sleeper():
+    global sleeper
+    if not sleeper:
+        sleeper=sessionManager.SessionSleep(sleep=8)
+    return sleeper
```

### Comparing `ofscraper-3.9.3/ofscraper/api/paid.py` & `ofscraper-3.9.4/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/pinned.py` & `ofscraper-3.9.4/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/profile.py` & `ofscraper-3.9.4/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/subscriptions/helpers.py` & `ofscraper-3.9.4/ofscraper/api/subscriptions/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/subscriptions/individual.py` & `ofscraper-3.9.4/ofscraper/api/subscriptions/individual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/subscriptions/lists.py` & `ofscraper-3.9.4/ofscraper/api/subscriptions/lists.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/subscriptions/subscriptions.py` & `ofscraper-3.9.4/ofscraper/api/subscriptions/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/api/timeline.py` & `ofscraper-3.9.4/ofscraper/api/timeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     data = await process_tasks(tasks)
     progress_utils.timeline_layout.visible = False
     return data
 
 
 @run
 async def get_timeline_posts(model_id, username, forced_after=None, c=None):
-    if not read_args.retriveArgs().no_cache:
+    if not settings.get_api_cache_disabled():
         oldtimeline = await get_timeline_posts_info(
             model_id=model_id, username=username
         )
     else:
         oldtimeline = []
     trace_log_old(oldtimeline)
 
@@ -118,15 +118,15 @@
     log.debug(f"{common_logs.FINAL_COUNT.format('Timeline')} {len(responseArray)}")
 
     trace_log_task(responseArray)
     return responseArray
 
 
 async def get_oldtimeline(model_id, username):
-    if not read_args.retriveArgs().no_cache:
+    if not settings.get_api_cache_disabled():
         oldtimeline = await get_timeline_posts_info(
             model_id=model_id, username=username
         )
     else:
         oldtimeline = []
     oldtimeline = list(filter(lambda x: x is not None, oldtimeline))
     # dedupe oldtimeline
```

### Comparing `ofscraper-3.9.3/ofscraper/classes/base.py` & `ofscraper-3.9.4/ofscraper/classes/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import importlib
 import re
 
 from bs4 import BeautifulSoup
 
-import ofscraper.utils.config.data as data
+import ofscraper.utils.settings as settings
 
 html_parser = "lxml" if importlib.util.find_spec("lxml") else "html.parser"
 
 
 class base:
     def __init__(self):
         None
 
     def text_trunicate(self, text):
         text = str(text)
         if text is None:
             return "None"
         if len(text) == 0:
             return text
-        length = int(data.get_textlength(mediatype="Text"))
+        length = int(settings.get_textlength(mediatype=self.mediatype))
         if length == 0:
             return text
-        elif data.get_textType(mediatype="Text") == "letter":
+        elif settings.get_text_type() == "letter":
             return f"{''.join(list(text)[:length])}"
         else:
             # split and reduce
             wordarray = list(filter(lambda x: len(x) != 0, re.split("( )", text)))
             splitArray = wordarray[: length + 1]
             text = f"{''.join(splitArray)}"
         text = re.sub(" +$", "", text)
@@ -33,15 +33,15 @@
 
     def file_cleanup(self, text, mediatype=None):
         text = str(text)
         text = re.sub("<[^>]*>", "", text)
         text = re.sub('[\n<>:"/\|?*:;]+', "", text)
         text = re.sub("-+", "_", text)
         text = re.sub(" +", " ", text)
-        text = re.sub(" ", data.get_spacereplacer(mediatype=mediatype), text)
+        text = re.sub(" ", settings.get_space_replacer(mediatype=mediatype), text)
         return text
 
     def db_cleanup(self, string):
         string = re.sub("<[^>]*>", "", string)
         string = " ".join(string.split())
         string = BeautifulSoup(string, html_parser).get_text()
         return string
```

### Comparing `ofscraper-3.9.3/ofscraper/classes/labels.py` & `ofscraper-3.9.4/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/classes/media.py` & `ofscraper-3.9.4/ofscraper/classes/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import ofscraper.utils.logs.helpers as log_helpers
 
 warnings.filterwarnings("ignore", category=MarkupResemblesLocatorWarning)
 
 
 log = logging.getLogger("shared")
 
-semaphore = asyncio.Semaphore(constants.getattr("MPD_MAX_SEMS"))
+semaphore = asyncio.BoundedSemaphore(constants.getattr("MPD_MAX_SEMS"))
 
 
 class Media(base.base):
     def __init__(self, media, count, post):
         super().__init__()
         self._media = media
         self._count = count
```

### Comparing `ofscraper-3.9.3/ofscraper/classes/models.py` & `ofscraper-3.9.4/ofscraper/classes/models.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.9.4/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/classes/placeholder.py` & `ofscraper-3.9.4/ofscraper/classes/placeholder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/classes/posts.py` & `ofscraper-3.9.4/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/classes/sessionmanager.py` & `ofscraper-3.9.4/ofscraper/classes/sessionmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,32 +36,29 @@
             )
             in {429, 504}
         )
     )
 
 
 class SessionSleep:
-    def __init__(self):
-        self._sleep = None
-        self._last_date = None
+    def __init__(self,sleep=None):
+        self._sleep = sleep
+        self._last_date = arrow.now()
         self._alock=asyncio.Lock()
     async def async_toomany_req(self):
         async with self._alock:
             self.toomany_req()
     def toomany_req(self):
         log=logging.getLogger("shared")
-        if self._last_date is None:
-                self._sleep = constants.getattr("SESSION_SLEEP_INIT")
-                log.debug(f"too many req => setting sleep to init [{self._sleep} seconds]")
-
-        elif self._sleep is None:
+        dif_min=constants.getattr("SESSION_SLEEP_INCREASE_TIME_DIFF")
+        if self._sleep is None:
             self._sleep = constants.getattr("SESSION_SLEEP_INIT")
             log.debug(f"too many req => setting sleep to init [{self._sleep} seconds]")
-        elif arrow.now().float_timestamp - self._last_date.float_timestamp < 120:
-            log.debug(f"too many req => not changing sleep [{self._sleep} seconds] because last call less than 120 seconds")
+        elif arrow.now().float_timestamp - self._last_date.float_timestamp < dif_min:
+            log.debug(f"too many req => not changing sleep [{self._sleep} seconds] because last call less than {dif_min} seconds")
             return self._sleep
         else:
             self._sleep = self._sleep * 2
             log.debug(f"too many req => setting sleep to [{self._sleep} seconds]")
         self._last_date = arrow.now()
         return self._sleep     
     async def async_do_sleep(self):
@@ -71,14 +68,18 @@
     def do_sleep(self):
         if self._sleep:
             logging.getLogger("shared").debug(f"too many req => waiting [{self._sleep} seconds] before next req")
             time.sleep(self._sleep)
     @property
     def sleep(self):
         return self._sleep
+    @sleep.setter
+    def sleep(self,val):
+        self._sleep=val
+
 
 
 
 
 class CustomTenacity(AsyncRetrying):
     """
     A custom context manager using tenacity for asynchronous retries with wait strategies and stopping without exceptions.
@@ -168,15 +169,15 @@
         self._read_timeout = read_timeout
         self._pool_connect_timeout = pool_timeout
         self._connect_limit = limit
         self._keep_alive = keep_alive
         self._keep_alive_exp = keep_alive_exp
         self._proxy = proxy
         self._delay = delay or 0
-        self._sem = semaphore or asyncio.Semaphore(sem or 100000)
+        self._sem = semaphore or asyncio.BoundedSemaphore(sem or 100000)
         self._sync_sem = sync_semaphore or threading.Semaphore(
             sync_sem or constants.getattr("SESSION_MANAGER_SYNC_SEM_DEFAULT")
         )
         self._retries = retries or constants.getattr("OF_NUM_RETRIES_SESSION_DEFAULT")
         self._wait_min = wait_min or constants.getattr("OF_MIN_WAIT_SESSION_DEFAULT")
         self._wait_max = wait_max or constants.getattr("OF_NUM_RETRIES_SESSION_DEFAULT")
         self._wait_min_exponential = wait_min_exponential or constants.getattr(
@@ -260,27 +261,29 @@
         wait_max=None,
         log=None,
         total_timeout=None,
         connect_timeout=None,
         pool_connect_timeout=None,
         read_timeout=None,
         sync_sem=None,
+        sleeper=None
     ):
         auth_requests.read_request_auth(forced=True) if sign else None
 
         headers = self._create_headers(headers, url, sign) if headers is None else None
         cookies = self._create_cookies() if cookies is None else None
         json = json or None
         params = params or None
         r = None
         log = log or self._log
         min = wait_min or self._wait_min
         max = wait_max or self._wait_max
         retries = retries or self._retries
         sync_sem = self._sync_sem or sync_sem
+        sleeper=sleeper or self._sleeper
         for _ in Retrying(
             retry=retry_if_not_exception_type(
                 (KeyboardInterrupt, asyncio.TimeoutError)
             ),
             stop=tenacity.stop.stop_after_attempt(retries),
             wait=tenacity.wait.wait_random(min=min, max=max),
             before=lambda x: (
@@ -289,15 +292,15 @@
                 else None
             ),
             reraise=True,
         ):
             r = None
             with _:
                 sync_sem.acquire()
-                self._sleeper.do_sleep()
+                sleeper.do_sleep()
                 try:
                     r = self._httpx_funct(
                         method,
                         timeout=httpx.Timeout(
                             total_timeout or self._total_timeout,
                             connect=connect_timeout or self._connect_timeout,
                             pool=pool_connect_timeout or self._pool_connect_timeout,
@@ -317,15 +320,15 @@
                         log.debug(f"[bold]failed: [bold] {r.url}")
                         log.debug(f"[bold]status: [bold] {r.status}")
                         log.debug(f"[bold]response text [/bold]: {r.text_()}")
                         log.debug(f"[bold]headers[/bold]: {r.headers}")
                         r.raise_for_status()
                 except Exception as E:
                     if(is_rate_limited(E)):
-                        self._sleeper.toomany_req()
+                        sleeper.toomany_req()
                     log.traceback_(E)
                     log.traceback_(traceback.format_exc())
                     raise E
         yield r
         sync_sem.release()
 
     @contextlib.asynccontextmanager
@@ -347,24 +350,26 @@
         sign=None,
         log=None,
         sem=None,
         total_timeout=None,
         connect_timeout=None,
         pool_connect_timeout=None,
         read_timeout=None,
+        sleeper=None,
         *args,
         **kwargs,
     ):
         wait_min = wait_min or self._wait_min
         wait_max = wait_max or self._wait_max
         wait_min_exponential = wait_min_exponential or self._wait_min_exponential
         wait_max_exponential = wait_max_exponential or self._wait_max_exponential
         log = log or self._log
         retries = retries or self._retries
         sem = sem or self._sem
+        sleeper=sleeper or self._sleeper
         async for _ in CustomTenacity(
             wait_exponential=tenacity.wait.wait_exponential(
                 multiplier=2, min=wait_min_exponential, max=wait_max_exponential
             ),
             retry=retry_if_not_exception_type(
                 (KeyboardInterrupt, asyncio.TimeoutError)
             ),
@@ -376,15 +381,15 @@
                 else None
             ),
             reraise=True,
         ):
             with _:
                 r = None
                 await sem.acquire()
-                await self._sleeper.async_do_sleep()
+                await sleeper.async_do_sleep()
                 try:
                     headers = (
                         self._create_headers(headers, url, sign)
                         if headers is None
                         else headers
                     )
                     cookies = self._create_cookies() if cookies is None else None
@@ -433,22 +438,29 @@
                         log.debug(f"[bold]failed: [bold] {r.url}")
                         log.debug(f"[bold]status: [bold] {r.status}")
                         log.debug(f"[bold]response text [/bold]: {await r.text_()}")
                         log.debug(f"[bold]headers[/bold]: {r.headers}")
                         r.raise_for_status()
                 except Exception as E:
                     if(is_rate_limited(E)):
-                        await self._sleeper.async_toomany_req()
+                        await sleeper.async_toomany_req()
                     log.traceback_(E)
                     log.traceback_(traceback.format_exc())
                     sem.release()
                     raise E
         yield r
         sem.release()
 
+    @property
+    def sleep(self):
+        return self._sleeper._sleep
+    @sleep.setter
+    def sleep(self,val):
+        self._sleeper._sleep=val
+
     async def _httpx_funct_async(self, *args, **kwargs):
         t = await self._session.request(*args, **kwargs)
         t.ok = not t.is_error
         t.json_ = lambda: self.factoryasync(t.json)
         t.text_ = lambda: self.factoryasync(t.text)
         t.status = t.status_code
         t.iter_chunked = t.aiter_bytes
@@ -474,8 +486,8 @@
         r.status_code = r.status
         r.read_ = r.content.read
         return r
 
     async def factoryasync(self, input):
         if callable(input):
             return input()
-        return input
+        return input
```

### Comparing `ofscraper-3.9.3/ofscraper/classes/table.py` & `ofscraper-3.9.4/ofscraper/classes/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/commands/check.py` & `ofscraper-3.9.4/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/commands/manual.py` & `ofscraper-3.9.4/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/commands/scraper.py` & `ofscraper-3.9.4/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/const/config.py` & `ofscraper-3.9.4/ofscraper/const/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/const/constants.py` & `ofscraper-3.9.4/ofscraper/const/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/const/general.py` & `ofscraper-3.9.4/ofscraper/const/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/const/other_url.py` & `ofscraper-3.9.4/ofscraper/const/other_url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/const/prompts.py` & `ofscraper-3.9.4/ofscraper/const/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/const/req.py` & `ofscraper-3.9.4/ofscraper/const/req.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,13 +65,16 @@
 
 
 MAX_THREAD_WORKERS = 20
 API_MAX_AREAS = 2
 API_TIMEOUT_PER_TASK = 500
 API_REQUEST_THREADONLY = ["Windows", "Linux", "Darwin"]
 
-SESSION_SLEEP_INIT = 8
+SESSION_SLEEP_INIT = 2
+SESSION_SLEEP_INCREASE_TIME_DIFF=30
+MESSAGE_SLEEP_DEFAULT=0
 # page must be 50 post, and 50 is a reasonable size for max number of pages
 REASONABLE_MAX_PAGE = 50
 MIN_PAGE_POST_COUNT = 50
+
 # messages
 REASONABLE_MAX_PAGE_MESSAGES = 80
```

### Comparing `ofscraper-3.9.3/ofscraper/const/test_constants.py` & `ofscraper-3.9.4/ofscraper/const/test_constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/const/url.py` & `ofscraper-3.9.4/ofscraper/const/url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/db/operations.py` & `ofscraper-3.9.4/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/db/operations_/labels.py` & `ofscraper-3.9.4/ofscraper/db/operations_/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/db/operations_/media.py` & `ofscraper-3.9.4/ofscraper/db/operations_/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/db/operations_/merge.py` & `ofscraper-3.9.4/ofscraper/db/operations_/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,33 +53,35 @@
     old_root = pathlib.Path(old_root)
     new_root = pathlib.Path(new_root)
     new_root.mkdir(exist_ok=True, parents=True)
     new_db_path = new_root / "user_data.db"
     db_merger = MergeDatabase(new_db_path)
 
     await create_tables(db_path=new_db_path)
+    failures=[]
     for ele in paths.get_all_db(old_root):
         if ele == new_db_path:
             continue
         log.info(f"Merging {ele} with {new_db_path}")
         try:
             model_id = get_single_model_via_profile(db_path=ele)
             if not model_id:
-                raise Exception("No model ID")
+                raise Exception("Not exactly one model_id in profile table")
             elif not str(model_id).isnumeric():
-                raise Exception("Model ID is not numeric")
+                raise Exception("Found model_id was not numeric")
             await create_tables(db_path=ele)
             await modify_tables(model_id=model_id, db_path=ele)
             await db_merger(ele)
 
         except Exception as E:
+            failures.append({"path":str(ele),"reason":E})
             log.error(f"Issue getting required info for {ele}")
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
-
+    log.info("\n\n\n".join(list(map(lambda x:str([(key,value) for key,value in x.items()]),failures))))
 
 class MergeDatabase:
     def __init__(self, new_db_path):
         self._data_init = False
         self._new_db = new_db_path
         self._media_keys = ["media_id", "model_id"]
         self._label_keys = ["post_id", "label_id", "model_id"]
```

### Comparing `ofscraper-3.9.3/ofscraper/db/operations_/messages.py` & `ofscraper-3.9.4/ofscraper/db/operations_/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/db/operations_/others.py` & `ofscraper-3.9.4/ofscraper/db/operations_/others.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/db/operations_/posts.py` & `ofscraper-3.9.4/ofscraper/db/operations_/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/db/operations_/profile.py` & `ofscraper-3.9.4/ofscraper/db/operations_/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 console = Console()
 log = logging.getLogger("shared")
 
 # user_id==modes.id cause of legacy
 profilesCreate = """
 CREATE TABLE IF NOT EXISTS profiles (
+    
 	id INTEGER NOT NULL, 
 	user_id INTEGER NOT NULL, 
 	username VARCHAR NOT NULL,
 	PRIMARY KEY (id)
     UNIQUE (user_id,username)
 )
 """
```

### Comparing `ofscraper-3.9.3/ofscraper/db/operations_/stories.py` & `ofscraper-3.9.4/ofscraper/db/operations_/stories.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/db/operations_/wrapper.py` & `ofscraper-3.9.4/ofscraper/db/operations_/wrapper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/alt_download.py` & `ofscraper-3.9.4/ofscraper/download/alt_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/alt_downloadbatch.py` & `ofscraper-3.9.4/ofscraper/download/alt_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/download.py` & `ofscraper-3.9.4/ofscraper/download/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/downloadbatch.py` & `ofscraper-3.9.4/ofscraper/download/downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/downloadnormal.py` & `ofscraper-3.9.4/ofscraper/download/downloadnormal.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/main_download.py` & `ofscraper-3.9.4/ofscraper/download/main_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/main_downloadbatch.py` & `ofscraper-3.9.4/ofscraper/download/main_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/classes/retries.py` & `ofscraper-3.9.4/ofscraper/download/shared/classes/retries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/classes/session.py` & `ofscraper-3.9.4/ofscraper/download/shared/classes/session.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/common/alt_common.py` & `ofscraper-3.9.4/ofscraper/download/shared/common/alt_common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/common/general.py` & `ofscraper-3.9.4/ofscraper/download/shared/common/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/common/main_common.py` & `ofscraper-3.9.4/ofscraper/download/shared/common/main_common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/globals.py` & `ofscraper-3.9.4/ofscraper/download/shared/globals.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from concurrent.futures import ThreadPoolExecutor
 
 import aioprocessing
 
 import ofscraper.utils.config.data as config_data
 import ofscraper.utils.console as console_
 import ofscraper.utils.constants as constants
-from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
 
 attempt = None
 attempt2 = None
 total_count = None
 total_count2 = None
 innerlog = None
 localDirSet = None
@@ -53,15 +52,15 @@
     global cache_thread
     cache_thread = ThreadPoolExecutor()
     global dirSet
     dirSet = set()
     global lock
     lock = asyncio.Lock()
     global maxfile_sem
-    maxfile_sem = semaphoreDelayed(constants.getattr("MAXFILE_SEMAPHORE"))
+    maxfile_sem = asyncio.Semaphore(constants.getattr("MAXFILE_SEMAPHORE"))
     global console
     console = console_.get_shared_console()
     global localDirSet
     localDirSet = set()
     global fileHashes
     fileHashes = {}
```

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/utils/keyhelpers.py` & `ofscraper-3.9.4/ofscraper/download/shared/utils/keyhelpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/utils/log.py` & `ofscraper-3.9.4/ofscraper/download/shared/utils/log.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/utils/message.py` & `ofscraper-3.9.4/ofscraper/download/shared/utils/message.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/utils/metadata.py` & `ofscraper-3.9.4/ofscraper/download/shared/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/utils/paths.py` & `ofscraper-3.9.4/ofscraper/download/shared/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/download/shared/utils/text.py` & `ofscraper-3.9.4/ofscraper/download/shared/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/filters/media/helpers.py` & `ofscraper-3.9.4/ofscraper/filters/media/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/filters/media/main.py` & `ofscraper-3.9.4/ofscraper/filters/media/main.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/filters/models/date.py` & `ofscraper-3.9.4/ofscraper/filters/models/date.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/filters/models/flags.py` & `ofscraper-3.9.4/ofscraper/filters/models/flags.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/filters/models/helpers.py` & `ofscraper-3.9.4/ofscraper/filters/models/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/filters/models/other.py` & `ofscraper-3.9.4/ofscraper/filters/models/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/filters/models/price.py` & `ofscraper-3.9.4/ofscraper/filters/models/price.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/filters/models/sort.py` & `ofscraper-3.9.4/ofscraper/filters/models/sort.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/filters/models/subtype.py` & `ofscraper-3.9.4/ofscraper/filters/models/subtype.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/models/retriver.py` & `ofscraper-3.9.4/ofscraper/models/retriver.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/models/selector.py` & `ofscraper-3.9.4/ofscraper/models/selector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/helpers/model_helpers.py` & `ofscraper-3.9.4/ofscraper/prompts/helpers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/helpers/prompt_helpers.py` & `ofscraper-3.9.4/ofscraper/prompts/helpers/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/keybindings.py` & `ofscraper-3.9.4/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/promptConvert.py` & `ofscraper-3.9.4/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompt_groups/actions.py` & `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompt_groups/area.py` & `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/area.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompt_groups/auth.py` & `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompt_groups/binary.py` & `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/binary.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompt_groups/config.py` & `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
                 "option_instruction": "Enter Date format",
                 "default": data.get_date(),
                 "validate": prompt_validators.dateplaceholdervalidator(),
             },
             {
                 "type": "list",
                 "name": "text_type_default",
-                "message": "date: ",
+                "message": "text type: ",
                 "option_instruction": "How should textlength be interpreted",
                 "default": data.get_textType(),
                 "choices": [Choice("letter", "Letter"), Choice("word", "Word")],
                 "validate": prompt_validators.emptyListValidator(),
             },
             {
                 "type": "list",
@@ -469,15 +469,15 @@
                 "choices": ["deviint", "digitalcriminals", "sneaky"],
             },
             {
                 "type": "list",
                 "name": "cache-mode",
                 "message": "sqlite should be fine unless your using a network drive\nSee https://grantjenks.com/docs/diskcache/tutorial.html#caveats ",
                 "default": data.cache_mode_helper(),
-                "choices": ["sqlite", "json", "disabled"],
+                "choices": ["sqlite", "json", "disabled","api_disabled"],
             },
             {
                 "type": "list",
                 "name": "backend",
                 "choices": [Choice("aio", "aiohttp"), Choice("httpx", "httpx")],
                 "message": "Select Which Backend you want:\n",
                 "default": data.get_backend() or "",
```

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompt_groups/menu.py` & `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompt_groups/merge.py` & `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/merge.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     name = "continue"
     answer = promptClasses.batchConverter(
         *[
             {
                 "type": "list",
                 "name": name,
                 "message": "Have you backed up your database files?",
-                "option_instruction": "Database files will be modified during the merge process",
+                "option_instruction": "Database files will be recursely searched and modified during the merge process",
                 "choices": [Choice(True, "Yes"), Choice(False, "No")],
             }
         ]
     )
     return answer[name]
 
 
@@ -48,15 +48,15 @@
 
 def new_db_prompt():
     answer = promptClasses.batchConverter(
         *[
             {
                 "type": "filepath",
                 "name": "database",
-                "message": "Merge db dir: ",
+                "message": "Merge db folder: ",
                 "option_instruction": """
                 directory for new merge database
                 It is best if merged database is stored seperately from source database(s)
                 """,
                 "default": str(get_profile_path()),
                 "filter": lambda x: prompt_validators.cleanTextInput(x),
             },
@@ -68,18 +68,19 @@
 def confirm_prompt_db(folder, new_db) -> bool:
     name = "continue"
     answer = promptClasses.batchConverter(
         *[
             {
                 "type": "list",
                 "name": name,
-                "message": "confirm merge: ",
+                "message": "Confirm merge: ",
                 "instruction": f"user_data.db files from {folder} will be merged into {str(pathlib.Path(new_db,'user_data.db'))}",
                 "choices": [
                     Choice(True, "Yes"),
                     Choice(False, "No"),
                     Choice(None, "Back to Main Menu"),
                 ],
+                "default":False
             }
         ]
     )
     return answer[name]
```

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompt_groups/model.py` & `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/model.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompt_groups/profile.py` & `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.9.4/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.9.4/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/prompts/prompts.py` & `ofscraper-3.9.4/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/runner/exit.py` & `ofscraper-3.9.4/ofscraper/runner/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/runner/load.py` & `ofscraper-3.9.4/ofscraper/runner/load.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/runner/run.py` & `ofscraper-3.9.4/ofscraper/runner/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/actions.py` & `ofscraper-3.9.4/ofscraper/utils/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/areas.py` & `ofscraper-3.9.4/ofscraper/utils/args/areas.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/groups/common_args.py` & `ofscraper-3.9.4/ofscraper/utils/args/groups/common_args.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,15 +73,22 @@
         help="Settings for logging",
     )
     @click.option_group(
         "Advanced Program Options",
         click.option(
             "-nc",
             "--no-cache",
-            help="Disable cache",
+            help="Disable cache and forces consecutive api scan",
+            default=False,
+            is_flag=True,
+        ),
+        click.option(
+            "-nca",
+            "--no-api-cache",
+            help="Forces consecutive api scan",
             default=False,
             is_flag=True,
         ),
         click.option(
             "-k",
             "--key-mode",
             help="Key mode override",
@@ -179,23 +186,17 @@
     def wrapper(ctx, *args, **kwargs):
         return func(ctx, *args, **kwargs)
 
     return wrapper
 
 
 def common_other_params(func):
-    click.option_group(
+    @click.option_group(
         "Downloading options",
         click.option(
-            "-g",
-            "--original",
-            help="Don't truncate long paths",
-            is_flag=True,
-        ),
-        click.option(
             "-q",
             "--quality",
             type=click.Choice(["240", "720", "source"], case_sensitive=False),
         ),
         click.option(
             "-lb",
             "--label",
@@ -207,13 +208,46 @@
                 list(set(itertools.chain.from_iterable(value))) if value else []
             ),
             multiple=True,
         ),
         help="Options for controlling download behavior",
     )
 
+    @click.option_group(
+        "Filename Modification options",
+        click.option(
+            "-g",
+            "--original",
+            help="Don't truncate long paths",
+            is_flag=True,
+        ),
+
+        click.option(
+            "-tt",
+            "--text-type",
+            help="set length based on word or letter",
+            type=click.Choice(["word", "letter"], case_sensitive=False),
+        ),
+
+        click.option(
+            "-sr",
+            "--space-replacer",
+            help="character to replace spaces with",
+        ),
+        click.option(
+            "-tl",
+            "--textlength",
+            help="max length of text",
+            type=click.INT
+        ),
+help="""
+\b
+Options for controlling the output of the final filename after placeholders are replaced
+"""
+     )
+
     @functools.wraps(func)
     @click.pass_context
     def wrapper(ctx, *args, **kwargs):
         return func(ctx, *args, **kwargs)
 
     return wrapper
```

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/groups/main_args.py` & `ofscraper-3.9.4/ofscraper/utils/args/groups/main_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,11 +625,12 @@
             help="Search entire enabled lists before filtering for usernames when --username is provided",
             default=False,
             is_flag=True,
         ),
     ),
     help="Choose how usernames are searched, and define the order in which users are processed for actions",
 )
+@common.common_other_params
 @common.common_params
 @click.pass_context
 def program(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/groups/manual_args.py` & `ofscraper-3.9.4/ofscraper/utils/args/groups/manual_args.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,12 +38,12 @@
 @click.option(
     "-fo",
     "--force",
     help="Force retrieval of new messages info from API",
     is_flag=True,
     default=False,
 )
-@common.common_params
 @common.common_other_params
+@common.common_params
 @click.pass_context
 def manual(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/groups/message_args.py` & `ofscraper-3.9.4/ofscraper/utils/args/groups/message_args.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,12 +43,12 @@
 @click.option(
     "-fo",
     "--force",
     help="Force retrieval of new messages info from API",
     is_flag=True,
     default=False,
 )
-@common.common_params
 @common.common_other_params
+@common.common_params
 @click.pass_context
 def message_check(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/groups/paid_args.py` & `ofscraper-3.9.4/ofscraper/utils/args/groups/paid_args.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -45,12 +45,12 @@
 @click.option(
     "-fo",
     "--force",
     help="Force retrieval of new purchases info from API",
     is_flag=True,
     default=False,
 )
-@common.common_params
 @common.common_other_params
+@common.common_params
 @click.pass_context
 def paid_check(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/groups/post_args.py` & `ofscraper-3.9.4/ofscraper/utils/args/groups/post_args.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -54,12 +54,12 @@
         ["Timeline", "Pinned", "Archived", "Labels"], case_sensitive=False
     ),
     callback=lambda ctx, param, value: (
         list(set(helpers.post_check_area(value))) if value else None
     ),
     multiple=True,
 )
-@common.common_params
 @common.common_other_params
+@common.common_params
 @click.pass_context
 def post_check(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/groups/story_args.py` & `ofscraper-3.9.4/ofscraper/utils/args/groups/story_args.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -45,12 +45,12 @@
 @click.option(
     "-fo",
     "--force",
     help="Force retrieval of new messages info from API",
     is_flag=True,
     default=False,
 )
-@common.common_params
 @common.common_other_params
+@common.common_params
 @click.pass_context
 def story_check(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/helpers.py` & `ofscraper-3.9.4/ofscraper/utils/args/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/parse.py` & `ofscraper-3.9.4/ofscraper/utils/args/parse.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/read.py` & `ofscraper-3.9.4/ofscraper/utils/args/read.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/args/user.py` & `ofscraper-3.9.4/ofscraper/utils/args/user.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/auth/context.py` & `ofscraper-3.9.4/ofscraper/utils/auth/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/auth/data.py` & `ofscraper-3.9.4/ofscraper/utils/auth/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/auth/file.py` & `ofscraper-3.9.4/ofscraper/utils/auth/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/auth/helpers.py` & `ofscraper-3.9.4/ofscraper/utils/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/auth/make.py` & `ofscraper-3.9.4/ofscraper/utils/auth/make.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/auth/request.py` & `ofscraper-3.9.4/ofscraper/utils/auth/request.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/auth/schema.py` & `ofscraper-3.9.4/ofscraper/utils/auth/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/binaries.py` & `ofscraper-3.9.4/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/cache.py` & `ofscraper-3.9.4/ofscraper/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/checkers.py` & `ofscraper-3.9.4/ofscraper/utils/checkers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/config/config.py` & `ofscraper-3.9.4/ofscraper/utils/config/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/config/context.py` & `ofscraper-3.9.4/ofscraper/utils/config/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/config/custom.py` & `ofscraper-3.9.4/ofscraper/utils/config/custom.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/config/data.py` & `ofscraper-3.9.4/ofscraper/utils/config/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/config/file.py` & `ofscraper-3.9.4/ofscraper/utils/config/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/config/menu.py` & `ofscraper-3.9.4/ofscraper/utils/config/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/config/schema.py` & `ofscraper-3.9.4/ofscraper/utils/config/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/constants.py` & `ofscraper-3.9.4/ofscraper/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/context/exit.py` & `ofscraper-3.9.4/ofscraper/utils/context/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/context/run_async.py` & `ofscraper-3.9.4/ofscraper/utils/context/run_async.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/context/stdout.py` & `ofscraper-3.9.4/ofscraper/utils/context/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/dates.py` & `ofscraper-3.9.4/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/encoding.py` & `ofscraper-3.9.4/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/hash.py` & `ofscraper-3.9.4/ofscraper/utils/hash.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/logs/classes.py` & `ofscraper-3.9.4/ofscraper/utils/logs/classes.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/logs/close.py` & `ofscraper-3.9.4/ofscraper/utils/logs/close.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/logs/helpers.py` & `ofscraper-3.9.4/ofscraper/utils/logs/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/logs/logger.py` & `ofscraper-3.9.4/ofscraper/utils/logs/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/logs/logs.py` & `ofscraper-3.9.4/ofscraper/utils/logs/logs.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/logs/other.py` & `ofscraper-3.9.4/ofscraper/utils/logs/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/logs/stdout.py` & `ofscraper-3.9.4/ofscraper/utils/logs/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/manager.py` & `ofscraper-3.9.4/ofscraper/utils/manager.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/menu.py` & `ofscraper-3.9.4/ofscraper/utils/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/merge.py` & `ofscraper-3.9.4/ofscraper/utils/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/paths/check.py` & `ofscraper-3.9.4/ofscraper/utils/paths/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/paths/common.py` & `ofscraper-3.9.4/ofscraper/utils/paths/common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/paths/paths.py` & `ofscraper-3.9.4/ofscraper/utils/paths/paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,10 +157,10 @@
 
 def speed_file():
     return pathlib.Path(common_paths.get_profile_path() / "speed.zip")
 
 
 def get_all_db(path):
     for ele in filter(
-        lambda x: re.search("user_data.db", str(x)), pathlib.Path(path).glob("**/*")
+        lambda x: re.search("user_data.db$", str(x)) and not re.search("(backup.db|_copy)",str(x)), pathlib.Path(path).glob("**/*")
     ):
         yield ele
```

### Comparing `ofscraper-3.9.3/ofscraper/utils/profiles/data.py` & `ofscraper-3.9.4/ofscraper/utils/profiles/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/profiles/manage.py` & `ofscraper-3.9.4/ofscraper/utils/profiles/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/profiles/tools.py` & `ofscraper-3.9.4/ofscraper/utils/profiles/tools.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/progress.py` & `ofscraper-3.9.4/ofscraper/utils/progress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/run.py` & `ofscraper-3.9.4/ofscraper/utils/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/separate.py` & `ofscraper-3.9.4/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/settings.py` & `ofscraper-3.9.4/ofscraper/utils/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,19 +49,41 @@
 def get_trunication(mediatype=None):
     return (
         read_args.retriveArgs().original
         or not config_data.get_truncation(mediatype=mediatype)
     ) is False
 
 
+def get_text_type(mediatype=None):
+    return (
+        read_args.retriveArgs().text_type or config_data.get_textType(mediatype=mediatype)
+    )
+
+
+def get_space_replacer(mediatype=None):
+    return (
+        read_args.retriveArgs().space_replacer or config_data.get_spacereplacer(mediatype=mediatype)
+    )
+
+
+def get_textlength(mediatype=None):
+    return (
+        read_args.retriveArgs().text_length or config_data.get_textlength(mediatype=mediatype)
+    )
+
 def get_cache_disabled():
     return (
         read_args.retriveArgs().no_cache or config_data.get_cache_mode() == "disabled"
     )
 
+def get_api_cache_disabled():
+     return (
+        read_args.retriveArgs().no_cache or read_args.retriveArgs().no_api_cache or config_data.get_cache_mode() == "api_disabled"
+    )
+
 
 def get_dynamic_rules():
     return read_args.retriveArgs().dynamic_rules or config_data.get_dynamic()
 
 
 def get_size_limit(mediatype=None):
     return read_args.retriveArgs().size_max or config_data.get_filesize_limit(
```

### Comparing `ofscraper-3.9.3/ofscraper/utils/system/network.py` & `ofscraper-3.9.4/ofscraper/utils/system/network.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/system/system.py` & `ofscraper-3.9.4/ofscraper/utils/system/system.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/ofscraper/utils/text.py` & `ofscraper-3.9.4/ofscraper/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.3/pyproject.toml` & `ofscraper-3.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.9.3"
+version = "3.9.4"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.14"
```

### Comparing `ofscraper-3.9.3/PKG-INFO` & `ofscraper-3.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.9.3
+Version: 3.9.4
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ofscraper Version: 3.9.3 Summary: automatically
+Metadata-Version: 2.1 Name: ofscraper Version: 3.9.4 Summary: automatically
 scrape onlyfans Author: datawhores Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: pyinstaller Requires-Dist: aiofiles
 (>=23.2.1,<24.0.0) Requires-Dist: aiohttp (==3.9.4) Requires-Dist:
 aioprocessing (>=2.0.1,<3.0.0) Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: arrow (>=1.3.0,<2.0.0) Requires-Dist: browser-cookie3 (==0.19.1)
```

