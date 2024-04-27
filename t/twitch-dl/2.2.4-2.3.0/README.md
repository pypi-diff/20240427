# Comparing `tmp/twitch_dl-2.2.4.tar.gz` & `tmp/twitch_dl-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch_dl-2.2.4.tar", last modified: Thu Apr 25 05:35:26 2024, max compression
+gzip compressed data, was "twitch_dl-2.3.0.tar", last modified: Sat Apr 27 18:24:51 2024, max compression
```

## Comparing `twitch_dl-2.2.4.tar` & `twitch_dl-2.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.850946 twitch_dl-2.2.4/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       41 2023-08-11 10:29:42.000000 twitch_dl-2.2.4/.flake8
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.844946 twitch_dl-2.2.4/.github/
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.845946 twitch_dl-2.2.4/.github/workflows/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/.github/workflows/test.yml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      166 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/.gitignore
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       65 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/.vermin
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10336 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/CHANGELOG.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2023-08-11 10:29:42.000000 twitch_dl-2.2.4/LICENSE
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      954 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/Makefile
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-04-25 05:35:26.850946 twitch_dl-2.2.4/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/README.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      343 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/TODO.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      481 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/book.css
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      223 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/book.toml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8622 2024-04-25 05:32:53.000000 twitch_dl-2.2.4/changelog.yaml
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.846946 twitch_dl-2.2.4/docs/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      484 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/docs/SUMMARY.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      282 2023-08-11 10:29:47.000000 twitch_dl-2.2.4/docs/advanced.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10336 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/changelog.md
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.847946 twitch_dl-2.2.4/docs/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    69599 2023-08-11 10:29:47.000000 twitch_dl-2.2.4/docs/commands/auth_token.png
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2499 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/commands/clips.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6159 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/commands/download.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      722 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/commands/env.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/commands/info.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2030 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/commands/videos.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      420 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/docs/environment_variables.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1653 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/docs/installation.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1169 2023-08-11 10:29:47.000000 twitch_dl-2.2.4/docs/introduction.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    34916 2023-08-11 10:29:47.000000 twitch_dl-2.2.4/docs/license.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      664 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/docs/shell_completion.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      690 2023-08-11 10:29:47.000000 twitch_dl-2.2.4/docs/usage.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1308 2024-04-24 06:41:19.000000 twitch_dl-2.2.4/pyproject.toml
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.847946 twitch_dl-2.2.4/scripts/
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1026 2023-10-08 19:39:41.000000 twitch_dl-2.2.4/scripts/generate_changelog
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     3686 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/scripts/generate_docs
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1587 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/scripts/tag_version
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-25 05:35:26.850946 twitch_dl-2.2.4/setup.cfg
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.847946 twitch_dl-2.2.4/tests/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2076 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/tests/test_api.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4659 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/tests/test_cli.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2518 2024-04-25 05:31:42.000000 twitch_dl-2.2.4/tests/test_patterns.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2605 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/tests/test_progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/tests/test_utils.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1350 2023-08-11 10:29:42.000000 twitch_dl-2.2.4/twitch-dl.1.scd
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.850946 twitch_dl-2.2.4/twitch_dl.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1240 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       47 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      133 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/top_level.txt
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.849946 twitch_dl-2.2.4/twitchdl/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      196 2024-04-23 15:35:36.000000 twitch_dl-2.2.4/twitchdl/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       36 2024-04-23 15:35:35.000000 twitch_dl-2.2.4/twitchdl/__main__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9715 2024-04-24 06:43:02.000000 twitch_dl-2.2.4/twitchdl/cli.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.850946 twitch_dl-2.2.4/twitchdl/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/twitchdl/commands/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2561 2024-04-23 15:09:23.000000 twitch_dl-2.2.4/twitchdl/commands/clips.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11691 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/twitchdl/commands/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3015 2024-04-24 06:41:19.000000 twitch_dl-2.2.4/twitchdl/commands/info.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2039 2024-04-25 05:30:23.000000 twitch_dl-2.2.4/twitchdl/commands/videos.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      932 2024-04-23 15:35:34.000000 twitch_dl-2.2.4/twitchdl/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      522 2024-04-23 16:09:59.000000 twitch_dl-2.2.4/twitchdl/entities.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      139 2024-04-23 15:35:32.000000 twitch_dl-2.2.4/twitchdl/exceptions.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4138 2024-04-23 15:35:32.000000 twitch_dl-2.2.4/twitchdl/http.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4577 2024-04-23 16:11:39.000000 twitch_dl-2.2.4/twitchdl/output.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3676 2024-04-24 06:41:19.000000 twitch_dl-2.2.4/twitchdl/playlists.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4722 2024-04-23 15:35:30.000000 twitch_dl-2.2.4/twitchdl/progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    12422 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/twitchdl/twitch.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3113 2024-04-25 05:30:27.000000 twitch_dl-2.2.4/twitchdl/utils.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.601963 twitch_dl-2.3.0/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       41 2022-08-04 08:32:39.000000 twitch_dl-2.3.0/.flake8
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.587963 twitch_dl-2.3.0/.github/
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.590963 twitch_dl-2.3.0/.github/workflows/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-24 12:52:36.000000 twitch_dl-2.3.0/.github/workflows/test.yml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      166 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/.gitignore
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       65 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/.vermin
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10556 2024-04-27 18:23:25.000000 twitch_dl-2.3.0/CHANGELOG.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2022-08-04 08:32:39.000000 twitch_dl-2.3.0/LICENSE
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      959 2024-04-27 18:22:52.000000 twitch_dl-2.3.0/Makefile
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-04-27 18:24:51.601963 twitch_dl-2.3.0/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/README.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      343 2022-11-13 13:02:23.000000 twitch_dl-2.3.0/TODO.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      481 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/book.css
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      223 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/book.toml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8805 2024-04-27 18:23:09.000000 twitch_dl-2.3.0/changelog.yaml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.591963 twitch_dl-2.3.0/docs/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      484 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/docs/SUMMARY.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      282 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/docs/advanced.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10556 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/changelog.md
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.592963 twitch_dl-2.3.0/docs/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    69599 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/docs/commands/auth_token.png
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2499 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/commands/clips.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6159 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/commands/download.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      722 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/commands/env.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/commands/info.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2030 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/commands/videos.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      420 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/docs/environment_variables.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1653 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/docs/installation.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1169 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/docs/introduction.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    34916 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/docs/license.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      664 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/docs/shell_completion.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      690 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/docs/usage.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1308 2024-04-24 06:19:51.000000 twitch_dl-2.3.0/pyproject.toml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.593963 twitch_dl-2.3.0/scripts/
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1026 2022-11-13 13:02:23.000000 twitch_dl-2.3.0/scripts/generate_changelog
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     3686 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/scripts/generate_docs
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1587 2024-04-10 06:26:52.000000 twitch_dl-2.3.0/scripts/tag_version
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-27 18:24:51.601963 twitch_dl-2.3.0/setup.cfg
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.596963 twitch_dl-2.3.0/tests/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2076 2024-04-24 12:38:54.000000 twitch_dl-2.3.0/tests/test_api.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4659 2024-04-24 12:44:22.000000 twitch_dl-2.3.0/tests/test_cli.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2518 2024-04-27 18:22:52.000000 twitch_dl-2.3.0/tests/test_patterns.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2605 2022-11-13 13:02:23.000000 twitch_dl-2.3.0/tests/test_progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2022-08-04 08:32:39.000000 twitch_dl-2.3.0/tests/test_utils.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1350 2022-08-04 08:32:39.000000 twitch_dl-2.3.0/twitch-dl.1.scd
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.600963 twitch_dl-2.3.0/twitch_dl.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1240 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       47 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      133 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/top_level.txt
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.599963 twitch_dl-2.3.0/twitchdl/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      196 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/twitchdl/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       36 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/twitchdl/__main__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9715 2024-04-24 06:58:58.000000 twitch_dl-2.3.0/twitchdl/cli.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.600963 twitch_dl-2.3.0/twitchdl/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/twitchdl/commands/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2561 2024-04-24 05:25:48.000000 twitch_dl-2.3.0/twitchdl/commands/clips.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11691 2024-04-27 17:02:55.000000 twitch_dl-2.3.0/twitchdl/commands/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3015 2024-04-27 16:59:23.000000 twitch_dl-2.3.0/twitchdl/commands/info.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2039 2024-04-24 12:30:02.000000 twitch_dl-2.3.0/twitchdl/commands/videos.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      932 2024-04-24 05:25:48.000000 twitch_dl-2.3.0/twitchdl/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      522 2024-04-24 05:25:48.000000 twitch_dl-2.3.0/twitchdl/entities.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      139 2024-04-04 06:27:17.000000 twitch_dl-2.3.0/twitchdl/exceptions.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4138 2024-04-24 12:09:16.000000 twitch_dl-2.3.0/twitchdl/http.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4775 2024-04-27 18:22:53.000000 twitch_dl-2.3.0/twitchdl/output.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4553 2024-04-27 18:22:53.000000 twitch_dl-2.3.0/twitchdl/playlists.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4722 2024-04-12 07:42:26.000000 twitch_dl-2.3.0/twitchdl/progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    12422 2024-04-24 12:29:56.000000 twitch_dl-2.3.0/twitchdl/twitch.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3113 2024-04-27 18:22:52.000000 twitch_dl-2.3.0/twitchdl/utils.py
```

### Comparing `twitch_dl-2.2.4/.github/workflows/test.yml` & `twitch_dl-2.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/CHANGELOG.md` & `twitch_dl-2.3.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 twitch-dl changelog
 ===================
 
 <!-- Do not edit. This file is automatically generated from changelog.yaml.-->
 
+### [2.3.0 (2024-04-27)](https://github.com/ihabunek/twitch-dl/releases/tag/2.3.0)
+
+* Show more playlist data when choosing quality
+* Improve detection of 'source' quality for Twitch Enhanced Broadcast Streams
+  (#154)
+
 ### [2.2.4 (2024-04-25)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.4)
 
 * Add m dot url support to video and clip regexes (thanks @localnerve)
 
 ### [2.2.3 (2024-04-24)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.3)
 
 * Respect --dry-run option when downloading videos
```

### Comparing `twitch_dl-2.2.4/LICENSE` & `twitch_dl-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/Makefile` & `twitch_dl-2.3.0/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 default : clean dist
 
 dist:
 	python -m build
 
 clean :
 	find . -name "*pyc" | xargs rm -rf $1
-	rm -rf build dist bundle MANIFEST htmlcov deb_dist twitch-dl.*.pyz twitch-dl.1.man twitch_dl.egg-info
+	rm -rf build dist book bundle MANIFEST htmlcov deb_dist twitch-dl.*.pyz twitch-dl.1.man twitch_dl.egg-info
 
 bundle:
 	mkdir bundle
 	cp twitchdl/__main__.py bundle
 	pip install . --target=bundle
 	rm -rf bundle/*.dist-info
 	find bundle/ -type d -name "__pycache__" -exec rm -rf {} +
```

### Comparing `twitch_dl-2.2.4/PKG-INFO` & `twitch_dl-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dl
-Version: 2.2.4
+Version: 2.3.0
 Summary: Quickly download videos from twitch.tv from the comort of your terminal emulator
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `twitch_dl-2.2.4/README.md` & `twitch_dl-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/changelog.yaml` & `twitch_dl-2.3.0/changelog.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2.3.0:
+  date: 2024-04-27
+  changes:
+    - "Show more playlist data when choosing quality"
+    - "Improve detection of 'source' quality for Twitch Enhanced Broadcast Streams (#154)"
+
 2.2.4:
   date: 2024-04-25
   changes:
     - "Add m dot url support to video and clip regexes (thanks @localnerve)"
 
 2.2.3:
   date: 2024-04-24
```

### Comparing `twitch_dl-2.2.4/docs/changelog.md` & `twitch_dl-2.3.0/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 twitch-dl changelog
 ===================
 
 <!-- Do not edit. This file is automatically generated from changelog.yaml.-->
 
+### [2.3.0 (2024-04-27)](https://github.com/ihabunek/twitch-dl/releases/tag/2.3.0)
+
+* Show more playlist data when choosing quality
+* Improve detection of 'source' quality for Twitch Enhanced Broadcast Streams
+  (#154)
+
 ### [2.2.4 (2024-04-25)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.4)
 
 * Add m dot url support to video and clip regexes (thanks @localnerve)
 
 ### [2.2.3 (2024-04-24)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.3)
 
 * Respect --dry-run option when downloading videos
```

### Comparing `twitch_dl-2.2.4/docs/commands/auth_token.png` & `twitch_dl-2.3.0/docs/commands/auth_token.png`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/docs/commands/clips.md` & `twitch_dl-2.3.0/docs/commands/clips.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/docs/commands/download.md` & `twitch_dl-2.3.0/docs/commands/download.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/docs/commands/env.md` & `twitch_dl-2.3.0/docs/commands/env.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/docs/commands/info.md` & `twitch_dl-2.3.0/docs/commands/info.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/docs/commands/videos.md` & `twitch_dl-2.3.0/docs/commands/videos.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/docs/installation.md` & `twitch_dl-2.3.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/docs/introduction.md` & `twitch_dl-2.3.0/docs/introduction.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/docs/license.md` & `twitch_dl-2.3.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/docs/shell_completion.md` & `twitch_dl-2.3.0/docs/shell_completion.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/docs/usage.md` & `twitch_dl-2.3.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/pyproject.toml` & `twitch_dl-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/scripts/generate_changelog` & `twitch_dl-2.3.0/scripts/generate_changelog`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/scripts/generate_docs` & `twitch_dl-2.3.0/scripts/generate_docs`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/scripts/tag_version` & `twitch_dl-2.3.0/scripts/tag_version`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/tests/test_api.py` & `twitch_dl-2.3.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/tests/test_cli.py` & `twitch_dl-2.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/tests/test_patterns.py` & `twitch_dl-2.3.0/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/tests/test_progress.py` & `twitch_dl-2.3.0/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitch-dl.1.scd` & `twitch_dl-2.3.0/twitch-dl.1.scd`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitch_dl.egg-info/PKG-INFO` & `twitch_dl-2.3.0/twitch_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dl
-Version: 2.2.4
+Version: 2.3.0
 Summary: Quickly download videos from twitch.tv from the comort of your terminal emulator
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `twitch_dl-2.2.4/twitch_dl.egg-info/SOURCES.txt` & `twitch_dl-2.3.0/twitch_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitchdl/cli.py` & `twitch_dl-2.3.0/twitchdl/cli.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitchdl/commands/clips.py` & `twitch_dl-2.3.0/twitchdl/commands/clips.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitchdl/commands/download.py` & `twitch_dl-2.3.0/twitchdl/commands/download.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitchdl/commands/info.py` & `twitch_dl-2.3.0/twitchdl/commands/info.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitchdl/commands/videos.py` & `twitch_dl-2.3.0/twitchdl/commands/videos.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitchdl/download.py` & `twitch_dl-2.3.0/twitchdl/download.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitchdl/entities.py` & `twitch_dl-2.3.0/twitchdl/entities.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitchdl/http.py` & `twitch_dl-2.3.0/twitchdl/http.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitchdl/output.py` & `twitch_dl-2.3.0/twitchdl/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,23 +21,32 @@
     click.echo(json.dumps(data))
 
 
 def print_log(message: Any):
     click.secho(message, err=True, dim=True)
 
 
+def visual_len(text: str):
+    return len(click.unstyle(text))
+
+
+def ljust(text: str, width: int):
+    diff = width - visual_len(text)
+    return text + (" " * diff) if diff > 0 else text
+
+
 def print_table(headers: List[str], data: List[List[str]]):
-    widths = [[len(cell) for cell in row] for row in data + [headers]]
+    widths = [[visual_len(cell) for cell in row] for row in data + [headers]]
     widths = [max(width) for width in zip(*widths)]
     underlines = ["-" * width for width in widths]
 
     def print_row(row: List[str]):
         for idx, cell in enumerate(row):
             width = widths[idx]
-            click.echo(cell.ljust(width), nl=False)
+            click.echo(ljust(cell, width), nl=False)
             click.echo("  ", nl=False)
         click.echo()
 
     print_row(headers)
     print_row(underlines)
 
     for row in data:
```

### Comparing `twitch_dl-2.2.4/twitchdl/playlists.py` & `twitch_dl-2.3.0/twitchdl/playlists.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 from dataclasses import dataclass
 from typing import Generator, List, Optional, OrderedDict
 
 import click
 import m3u8
 
 from twitchdl import utils
-from twitchdl.output import bold, dim
+from twitchdl.output import bold, dim, print_table
 
 
 @dataclass
 class Playlist:
     name: str
+    group_id: str
     resolution: Optional[str]
     url: str
+    is_source: bool
 
 
 @dataclass
 class Vod:
     index: int
     """Ordinal number of the VOD in the playlist"""
     path: str
@@ -30,25 +32,25 @@
 
 
 def parse_playlists(playlists_m3u8: str) -> List[Playlist]:
     def _parse(source: str) -> Generator[Playlist, None, None]:
         document = load_m3u8(source)
 
         for p in document.playlists:
-            if p.stream_info.resolution:
-                name = p.media[0].name
-                resolution = "x".join(str(r) for r in p.stream_info.resolution)
-            else:
-                name = p.media[0].group_id
-                resolution = None
+            resolution = (
+                "x".join(str(r) for r in p.stream_info.resolution)
+                if p.stream_info.resolution
+                else None
+            )
+
+            media = p.media[0]
+            is_source = media.group_id == "chunked"
+            yield Playlist(media.name, media.group_id, resolution, p.uri, is_source)
 
-            yield Playlist(name, resolution, p.uri)
-
-    # Move audio to bottom, it has no resolution
-    return sorted(_parse(playlists_m3u8), key=lambda p: p.resolution is None)
+    return list(_parse(playlists_m3u8))
 
 
 def load_m3u8(playlist_m3u8: str) -> m3u8.M3U8:
     return m3u8.loads(playlist_m3u8)
 
 
 def enumerate_vods(
@@ -103,29 +105,66 @@
         if quality is not None
         else select_playlist_interactive(playlists)
     )
 
 
 def select_playlist_by_name(playlists: List[Playlist], quality: str) -> Playlist:
     if quality == "source":
-        return playlists[0]
+        for playlist in playlists:
+            if playlist.is_source:
+                return playlist
+        raise click.ClickException("Source quality not found, please report an issue on github.")
 
     for playlist in playlists:
-        if playlist.name == quality:
+        if playlist.name == quality or playlist.group_id == quality:
             return playlist
 
     available = ", ".join([p.name for p in playlists])
     msg = f"Quality '{quality}' not found. Available qualities are: {available}"
     raise click.ClickException(msg)
 
 
 def select_playlist_interactive(playlists: List[Playlist]) -> Playlist:
-    click.echo("\nAvailable qualities:")
-    for n, playlist in enumerate(playlists):
-        if playlist.resolution:
-            click.echo(f"{n + 1}) {bold(playlist.name)} {dim(f'({playlist.resolution})')}")
-        else:
-            click.echo(f"{n + 1}) {bold(playlist.name)}")
+    playlists = sorted(playlists, key=_playlist_key)
+    headers = ["#", "Name", "Group ID", "Resolution"]
+
+    rows = [
+        [
+            f"{n + 1})",
+            bold(playlist.name),
+            dim(playlist.group_id),
+            dim(playlist.resolution or ""),
+        ]
+        for n, playlist in enumerate(playlists)
+    ]
+
+    click.echo()
+    print_table(headers, rows)
+
+    default = 1
+    for index, playlist in enumerate(playlists):
+        if playlist.is_source:
+            default = index + 1
 
-    no = utils.read_int("Choose quality", min=1, max=len(playlists) + 1, default=1)
+    no = utils.read_int("\nChoose quality", min=1, max=len(playlists) + 1, default=default)
     playlist = playlists[no - 1]
     return playlist
+
+
+MAX = 1_000_000
+
+
+def _playlist_key(playlist: Playlist) -> int:
+    """Attempt to sort playlists so that source quality is on top, audio only
+    is on bottom and others are sorted descending by resolution."""
+    if playlist.is_source:
+        return 0
+
+    if playlist.group_id == "audio_only":
+        return MAX
+
+    try:
+        return MAX - int(playlist.name.split("p")[0])
+    except Exception:
+        pass
+
+    return MAX
```

### Comparing `twitch_dl-2.2.4/twitchdl/progress.py` & `twitch_dl-2.3.0/twitchdl/progress.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitchdl/twitch.py` & `twitch_dl-2.3.0/twitchdl/twitch.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.4/twitchdl/utils.py` & `twitch_dl-2.3.0/twitchdl/utils.py`

 * *Files identical despite different names*

