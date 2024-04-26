# Comparing `tmp/zcmds-1.4.81.tar.gz` & `tmp/zcmds-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcmds-1.4.81.tar", last modified: Fri Apr 26 03:55:35 2024, max compression
+gzip compressed data, was "zcmds-1.4.9.tar", last modified: Thu Apr  6 18:07:06 2023, max compression
```

## Comparing `zcmds-1.4.81.tar` & `zcmds-1.4.9.tar`

### file list

```diff
@@ -1,138 +1,111 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.146685 zcmds-1.4.81/
--rw-rw-rw-   0        0        0       78 2024-04-19 04:50:35.000000 zcmds-1.4.81/.aiderignore
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:34.983685 zcmds-1.4.81/.github/
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.020687 zcmds-1.4.81/.github/workflows/
--rw-rw-rw-   0        0        0      859 2024-02-08 19:22:29.000000 zcmds-1.4.81/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      801 2023-12-11 21:15:36.000000 zcmds-1.4.81/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      803 2023-12-11 21:15:36.000000 zcmds-1.4.81/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0     1652 2023-12-11 21:15:36.000000 zcmds-1.4.81/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     2147 2024-04-25 17:28:16.000000 zcmds-1.4.81/.gitignore
--rw-rw-rw-   0        0        0    27051 2023-12-11 21:15:36.000000 zcmds-1.4.81/.pylintrc
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.023687 zcmds-1.4.81/.vscode/
--rw-rw-rw-   0        0        0      250 2023-12-15 00:13:37.000000 zcmds-1.4.81/.vscode/launch.json
--rw-rw-rw-   0        0        0      677 2024-04-11 19:58:45.000000 zcmds-1.4.81/.vscode/settings.json
--rw-rw-rw-   0        0        0     1064 2023-12-11 21:15:36.000000 zcmds-1.4.81/LICENSE
--rw-rw-rw-   0        0        0      205 2023-12-11 21:15:36.000000 zcmds-1.4.81/MANIFEST.in
--rw-rw-rw-   0        0        0      106 2023-12-11 21:15:36.000000 zcmds-1.4.81/NOTES.md
--rw-rw-rw-   0        0        0    14295 2024-04-26 03:55:35.145685 zcmds-1.4.81/PKG-INFO
--rw-rw-rw-   0        0        0    13910 2024-04-26 03:55:01.000000 zcmds-1.4.81/README.md
--rw-rw-rw-   0        0        0     1460 2023-12-16 01:23:44.000000 zcmds-1.4.81/activate.sh
--rw-rw-rw-   0        0        0       11 2023-12-16 01:28:51.000000 zcmds-1.4.81/clean
--rw-rw-rw-   0        0        0     1013 2023-12-16 01:23:11.000000 zcmds-1.4.81/install
--rw-rw-rw-   0        0        0     6949 2023-12-16 01:24:15.000000 zcmds-1.4.81/install.py
--rw-rw-rw-   0        0        0      284 2023-12-11 21:15:36.000000 zcmds-1.4.81/lint
--rw-rw-rw-   0        0        0     1994 2023-12-11 21:15:36.000000 zcmds-1.4.81/make_venv.py
--rw-rw-rw-   0        0        0      658 2024-02-08 03:10:35.000000 zcmds-1.4.81/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-12-11 21:15:36.000000 zcmds-1.4.81/requirements.testing.txt
--rw-rw-rw-   0        0        0      376 2024-04-11 19:55:00.000000 zcmds-1.4.81/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 03:55:35.146685 zcmds-1.4.81/setup.cfg
--rw-rw-rw-   0        0        0     1618 2023-12-15 05:40:06.000000 zcmds-1.4.81/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:34.985687 zcmds-1.4.81/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.027687 zcmds-1.4.81/src/zcmds/
--rw-rw-rw-   0        0        0       33 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.036687 zcmds-1.4.81/src/zcmds/assets/
--rw-rw-rw-   0        0        0    77452 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/assets/bell.mp3
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.038686 zcmds-1.4.81/src/zcmds/cmds/
--rw-rw-rw-   0        0        0        0 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.108689 zcmds-1.4.81/src/zcmds/cmds/common/
--rw-rw-rw-   0        0        0       83 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/README.md
--rw-rw-rw-   0        0        0        0 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/__init__.py
--rw-rw-rw-   0        0        0    13319 2024-04-26 03:51:39.000000 zcmds-1.4.81/src/zcmds/cmds/common/aicode.py
--rw-rw-rw-   0        0        0     2512 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/archive.py
--rw-rw-rw-   0        0        0     8384 2024-04-19 04:56:52.000000 zcmds-1.4.81/src/zcmds/cmds/common/askai.py
--rw-rw-rw-   0        0        0     4461 2024-04-12 06:39:05.000000 zcmds-1.4.81/src/zcmds/cmds/common/audnorm.py
--rw-rw-rw-   0        0        0     2954 2024-03-24 21:02:23.000000 zcmds-1.4.81/src/zcmds/cmds/common/codeup.py
--rw-rw-rw-   0        0        0      311 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/comports.py
--rw-rw-rw-   0        0        0     5674 2024-02-19 00:17:55.000000 zcmds-1.4.81/src/zcmds/cmds/common/diskaudit.py
--rw-rw-rw-   0        0        0     3195 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/findfiles.py
--rw-rw-rw-   0        0        0      616 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/fixinternet.py
--rw-rw-rw-   0        0        0     6434 2023-12-12 20:48:20.000000 zcmds-1.4.81/src/zcmds/cmds/common/geninvoice.py
--rw-rw-rw-   0        0        0     1677 2024-03-12 18:29:19.000000 zcmds-1.4.81/src/zcmds/cmds/common/gitconfig.py
--rw-rw-rw-   0        0        0     7785 2024-02-19 00:17:55.000000 zcmds-1.4.81/src/zcmds/cmds/common/gitsummary.py
--rw-rw-rw-   0        0        0     1713 2024-02-19 00:17:55.000000 zcmds-1.4.81/src/zcmds/cmds/common/img2vid.py
--rw-rw-rw-   0        0        0     6336 2024-04-12 06:59:38.000000 zcmds-1.4.81/src/zcmds/cmds/common/img2webp.py
--rw-rw-rw-   0        0        0     3303 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/imgai.py
--rw-rw-rw-   0        0        0     1212 2024-02-19 00:17:54.000000 zcmds-1.4.81/src/zcmds/cmds/common/imgshrink.py
--rw-rw-rw-   0        0        0     2598 2023-12-15 05:12:11.000000 zcmds-1.4.81/src/zcmds/cmds/common/losslesscut.py
--rw-rw-rw-   0        0        0     1486 2024-01-07 00:52:20.000000 zcmds-1.4.81/src/zcmds/cmds/common/merge_to.py
--rw-rw-rw-   0        0        0      526 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/myip.py
--rw-rw-rw-   0        0        0      364 2024-02-19 00:18:03.000000 zcmds-1.4.81/src/zcmds/cmds/common/new.py
--rw-rw-rw-   0        0        0     1785 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/obs_organize.py
--rw-rw-rw-   0        0        0      739 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/openaicfg.py
--rw-rw-rw-   0        0        0     2322 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/pdf2png.py
--rw-rw-rw-   0        0        0     1166 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/pdf2txt.py
--rw-rw-rw-   0        0        0      661 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/printenv.py
--rw-rw-rw-   0        0        0     3416 2024-02-09 06:46:03.000000 zcmds-1.4.81/src/zcmds/cmds/common/pull.py
--rw-rw-rw-   0        0        0     1632 2024-01-31 03:51:11.000000 zcmds-1.4.81/src/zcmds/cmds/common/push.py
--rw-rw-rw-   0        0        0    11999 2024-04-26 01:25:28.000000 zcmds-1.4.81/src/zcmds/cmds/common/removebackground.py
--rw-rw-rw-   0        0        0      756 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/say.py
--rw-rw-rw-   0        0        0      113 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/search_and_replace.py
--rw-rw-rw-   0        0        0      102 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/search_in_files.py
--rw-rw-rw-   0        0        0     1400 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/sharedir.py
--rw-rw-rw-   0        0        0     1927 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/stereo2mono.py
--rw-rw-rw-   0        0        0      472 2024-02-19 00:17:54.000000 zcmds-1.4.81/src/zcmds/cmds/common/trash.py
--rw-rw-rw-   0        0        0     2030 2023-12-15 01:49:04.000000 zcmds-1.4.81/src/zcmds/cmds/common/tsdownloader.py
--rw-rw-rw-   0        0        0     1581 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vid2gif.py
--rw-rw-rw-   0        0        0     1936 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vid2jpg.py
--rw-rw-rw-   0        0        0     1442 2024-04-12 06:39:05.000000 zcmds-1.4.81/src/zcmds/cmds/common/vid2mp3.py
--rw-rw-rw-   0        0        0     2653 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vid2mp4.py
--rw-rw-rw-   0        0        0     1049 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vid2webm.py
--rw-rw-rw-   0        0        0     3553 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vidcat.py
--rw-rw-rw-   0        0        0     4891 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vidclip.py
--rw-rw-rw-   0        0        0     1984 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/viddur.py
--rw-rw-rw-   0        0        0     3533 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vidhero.py
--rw-rw-rw-   0        0        0     5987 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vidinfo.py
--rw-rw-rw-   0        0        0     1242 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vidlist.py
--rw-rw-rw-   0        0        0     2777 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vidmatrix.py
--rw-rw-rw-   0        0        0     1653 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vidmute.py
--rw-rw-rw-   0        0        0     1642 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vidshrink.py
--rw-rw-rw-   0        0        0     1726 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vidspeed.py
--rw-rw-rw-   0        0        0     1751 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vidvol.py
--rw-rw-rw-   0        0        0     6103 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/vidwebmaster.py
--rw-rw-rw-   0        0        0     3408 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/common/whichall.py
--rw-rw-rw-   0        0        0      629 2024-02-19 00:17:54.000000 zcmds-1.4.81/src/zcmds/cmds/common/zcmds_main.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.111685 zcmds-1.4.81/src/zcmds/cmds/darwin/
--rw-rw-rw-   0        0        0        0 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/darwin/__init__.py
--rw-rw-rw-   0        0        0     3379 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/darwin/test_net_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.114685 zcmds-1.4.81/src/zcmds/cmds/linux/
--rw-rw-rw-   0        0        0       34 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/linux/TODO
--rw-rw-rw-   0        0        0        0 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/cmds/linux/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-03-14 02:01:26.000000 zcmds-1.4.81/src/zcmds/cmds.txt
--rw-rw-rw-   0        0        0      559 2024-01-16 02:03:41.000000 zcmds-1.4.81/src/zcmds/get_cmds.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.115688 zcmds-1.4.81/src/zcmds/install/
--rw-rw-rw-   0        0        0        0 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/install/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.118686 zcmds-1.4.81/src/zcmds/install/darwin/
--rw-rw-rw-   0        0        0        0 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/install/darwin/__init__.py
--rw-rw-rw-   0        0        0     1392 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/install/darwin/darwin_update.py
--rw-rw-rw-   0        0        0      607 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/install/darwin/macOS_key_bindings.dict
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.134685 zcmds-1.4.81/src/zcmds/util/
--rw-rw-rw-   0        0        0        0 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/util/__init__.py
--rw-rw-rw-   0        0        0     2490 2024-02-08 19:22:29.000000 zcmds-1.4.81/src/zcmds/util/_gpt4all.py
--rw-rw-rw-   0        0        0     5058 2024-04-19 06:52:20.000000 zcmds-1.4.81/src/zcmds/util/chatgpt.py
--rw-rw-rw-   0        0        0     1097 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/util/config.py
--rw-rw-rw-   0        0        0     1656 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/util/file_search_and_replacer.py
--rw-rw-rw-   0        0        0     1028 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/util/file_searcher.py
--rw-rw-rw-   0        0        0     4309 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/util/fileutils.py
--rw-rw-rw-   0        0        0      638 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/util/index_all_files.py
--rw-rw-rw-   0        0        0      853 2024-02-08 06:11:19.000000 zcmds-1.4.81/src/zcmds/util/prompt_input.py
--rw-rw-rw-   0        0        0      532 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/util/say.py
--rw-rw-rw-   0        0        0      249 2023-12-11 21:15:36.000000 zcmds-1.4.81/src/zcmds/util/sound.py
--rw-rw-rw-   0        0        0     4665 2024-04-12 06:59:38.000000 zcmds-1.4.81/src/zcmds/util/streaming_console.py
--rw-rw-rw-   0        0        0      153 2024-04-26 03:53:07.000000 zcmds-1.4.81/src/zcmds/version.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.035687 zcmds-1.4.81/src/zcmds.egg-info/
--rw-rw-rw-   0        0        0    14295 2024-04-26 03:55:34.000000 zcmds-1.4.81/src/zcmds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3406 2024-04-26 03:55:34.000000 zcmds-1.4.81/src/zcmds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 03:55:34.000000 zcmds-1.4.81/src/zcmds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2359 2024-04-26 03:55:34.000000 zcmds-1.4.81/src/zcmds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      361 2024-04-26 03:55:34.000000 zcmds-1.4.81/src/zcmds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 03:55:34.000000 zcmds-1.4.81/src/zcmds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       72 2024-04-11 20:04:15.000000 zcmds-1.4.81/test
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.140685 zcmds-1.4.81/tests/
-drwxrwxrwx   0        0        0        0 2024-04-26 03:55:35.142685 zcmds-1.4.81/tests/test_data/
--rw-rw-rw-   0        0        0    38274 2024-04-25 16:59:14.000000 zcmds-1.4.81/tests/test_data/rembg.mp4
--rw-rw-rw-   0        0        0     4786 2023-12-11 21:15:36.000000 zcmds-1.4.81/tests/test_findfiles.py
--rw-rw-rw-   0        0        0      876 2023-12-11 21:15:36.000000 zcmds-1.4.81/tests/test_main.py
--rw-rw-rw-   0        0        0      260 2023-12-11 21:15:36.000000 zcmds-1.4.81/tests/test_sound.py
--rw-rw-rw-   0        0        0     5609 2023-12-15 04:50:34.000000 zcmds-1.4.81/tests/test_streaming_console.py
--rw-rw-rw-   0        0        0      451 2023-12-11 21:15:36.000000 zcmds-1.4.81/tox.ini
--rw-rw-rw-   0        0        0      306 2023-12-18 03:05:54.000000 zcmds-1.4.81/upload_package.sh
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.523714 zcmds-1.4.9/
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.401713 zcmds-1.4.9/.github/
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.427716 zcmds-1.4.9/.github/workflows/
+-rw-rw-rw-   0        0        0      899 2022-11-05 21:21:20.000000 zcmds-1.4.9/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      833 2022-11-05 21:19:03.000000 zcmds-1.4.9/.github/workflows/push_macos.yml
+-rw-rw-rw-   0        0        0      803 2023-02-02 07:49:35.000000 zcmds-1.4.9/.github/workflows/push_ubuntu.yml
+-rw-rw-rw-   0        0        0     1650 2023-02-02 07:49:35.000000 zcmds-1.4.9/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     2013 2022-10-08 21:49:27.000000 zcmds-1.4.9/.gitignore
+-rw-rw-rw-   0        0        0    27051 2023-02-02 07:58:31.000000 zcmds-1.4.9/.pylintrc
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.428712 zcmds-1.4.9/.vscode/
+-rw-rw-rw-   0        0        0     1046 2023-04-02 08:55:51.000000 zcmds-1.4.9/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1085 2022-02-21 03:22:36.000000 zcmds-1.4.9/LICENSE
+-rw-rw-rw-   0        0        0      205 2023-04-02 09:38:20.000000 zcmds-1.4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      106 2023-04-03 23:26:07.000000 zcmds-1.4.9/NOTES.md
+-rw-rw-rw-   0        0        0     7554 2023-04-06 18:07:06.522715 zcmds-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7170 2023-04-06 18:05:22.000000 zcmds-1.4.9/README.md
+-rw-rw-rw-   0        0        0      292 2023-04-02 08:27:52.000000 zcmds-1.4.9/activate.sh
+-rw-rw-rw-   0        0        0      284 2023-03-14 23:38:05.000000 zcmds-1.4.9/lint.sh
+-rw-rw-rw-   0        0        0     1994 2022-07-27 00:44:21.000000 zcmds-1.4.9/make_venv.py
+-rw-rw-rw-   0        0        0      571 2023-04-06 18:04:11.000000 zcmds-1.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0       28 2022-02-21 03:22:36.000000 zcmds-1.4.9/requirements.testing.txt
+-rw-rw-rw-   0        0        0      217 2023-04-03 18:51:55.000000 zcmds-1.4.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-06 18:07:06.523714 zcmds-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1431 2023-04-02 09:38:31.000000 zcmds-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.402719 zcmds-1.4.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.433714 zcmds-1.4.9/src/zcmds/
+-rw-rw-rw-   0        0        0       33 2022-10-15 20:55:39.000000 zcmds-1.4.9/src/zcmds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.454716 zcmds-1.4.9/src/zcmds/assets/
+-rw-rw-rw-   0        0        0    77452 2023-02-02 07:49:35.000000 zcmds-1.4.9/src/zcmds/assets/bell.mp3
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.455713 zcmds-1.4.9/src/zcmds/cmds/
+-rw-rw-rw-   0        0        0        0 2022-02-21 10:38:44.000000 zcmds-1.4.9/src/zcmds/cmds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.499713 zcmds-1.4.9/src/zcmds/cmds/common/
+-rw-rw-rw-   0        0        0       83 2022-02-24 09:10:00.000000 zcmds-1.4.9/src/zcmds/cmds/common/README.md
+-rw-rw-rw-   0        0        0        0 2022-02-21 10:39:02.000000 zcmds-1.4.9/src/zcmds/cmds/common/__init__.py
+-rw-rw-rw-   0        0        0     5364 2023-04-03 19:00:15.000000 zcmds-1.4.9/src/zcmds/cmds/common/askai.py
+-rw-rw-rw-   0        0        0     1561 2023-04-06 17:36:45.000000 zcmds-1.4.9/src/zcmds/cmds/common/audnorm.py
+-rw-rw-rw-   0        0        0      311 2023-01-01 07:58:23.000000 zcmds-1.4.9/src/zcmds/cmds/common/comports.py
+-rw-rw-rw-   0        0        0     4305 2022-12-03 00:29:53.000000 zcmds-1.4.9/src/zcmds/cmds/common/diskaudit.py
+-rw-rw-rw-   0        0        0     1172 2023-03-29 02:40:46.000000 zcmds-1.4.9/src/zcmds/cmds/common/findfiles.py
+-rw-rw-rw-   0        0        0      616 2023-02-02 08:05:19.000000 zcmds-1.4.9/src/zcmds/cmds/common/fixinternet.py
+-rw-rw-rw-   0        0        0     2107 2023-04-03 03:08:28.000000 zcmds-1.4.9/src/zcmds/cmds/common/geninvoice.py
+-rw-rw-rw-   0        0        0     7264 2023-04-02 23:37:24.000000 zcmds-1.4.9/src/zcmds/cmds/common/gitsummary.py
+-rw-rw-rw-   0        0        0     1714 2023-02-27 00:07:25.000000 zcmds-1.4.9/src/zcmds/cmds/common/img2vid.py
+-rw-rw-rw-   0        0        0     3303 2023-02-02 07:49:35.000000 zcmds-1.4.9/src/zcmds/cmds/common/imgai.py
+-rw-rw-rw-   0        0        0     1785 2023-02-02 07:57:46.000000 zcmds-1.4.9/src/zcmds/cmds/common/obs_organize.py
+-rw-rw-rw-   0        0        0      739 2023-01-11 08:02:51.000000 zcmds-1.4.9/src/zcmds/cmds/common/openaicfg.py
+-rw-rw-rw-   0        0        0     2394 2023-02-09 20:17:45.000000 zcmds-1.4.9/src/zcmds/cmds/common/pdf2png.py
+-rw-rw-rw-   0        0        0     1166 2023-03-30 01:50:51.000000 zcmds-1.4.9/src/zcmds/cmds/common/pdf2txt.py
+-rw-rw-rw-   0        0        0      556 2023-03-24 04:23:48.000000 zcmds-1.4.9/src/zcmds/cmds/common/printenv.py
+-rw-rw-rw-   0        0        0      756 2023-04-04 04:43:30.000000 zcmds-1.4.9/src/zcmds/cmds/common/say.py
+-rw-rw-rw-   0        0        0      119 2022-02-21 05:10:16.000000 zcmds-1.4.9/src/zcmds/cmds/common/search_and_replace.py
+-rw-rw-rw-   0        0        0      108 2022-02-21 05:10:10.000000 zcmds-1.4.9/src/zcmds/cmds/common/search_in_files.py
+-rw-rw-rw-   0        0        0       44 2022-03-31 06:58:04.000000 zcmds-1.4.9/src/zcmds/cmds/common/sharedir.py
+-rw-rw-rw-   0        0        0     1986 2023-03-23 20:09:17.000000 zcmds-1.4.9/src/zcmds/cmds/common/stereo2mono.py
+-rw-rw-rw-   0        0        0     1340 2022-05-20 06:00:29.000000 zcmds-1.4.9/src/zcmds/cmds/common/vid2gif.py
+-rw-rw-rw-   0        0        0     1830 2022-03-10 02:29:32.000000 zcmds-1.4.9/src/zcmds/cmds/common/vid2jpg.py
+-rw-rw-rw-   0        0        0     1128 2023-04-06 18:03:51.000000 zcmds-1.4.9/src/zcmds/cmds/common/vid2mp3.py
+-rw-rw-rw-   0        0        0     1333 2022-11-05 02:45:38.000000 zcmds-1.4.9/src/zcmds/cmds/common/vid2mp4.py
+-rw-rw-rw-   0        0        0     1080 2022-08-16 20:18:02.000000 zcmds-1.4.9/src/zcmds/cmds/common/vid2webm.py
+-rw-rw-rw-   0        0        0     3397 2023-04-06 18:04:01.000000 zcmds-1.4.9/src/zcmds/cmds/common/vidcat.py
+-rw-rw-rw-   0        0        0     4891 2022-11-10 05:10:07.000000 zcmds-1.4.9/src/zcmds/cmds/common/vidclip.py
+-rw-rw-rw-   0        0        0     1984 2022-02-24 06:01:55.000000 zcmds-1.4.9/src/zcmds/cmds/common/viddur.py
+-rw-rw-rw-   0        0        0     3533 2023-01-01 07:59:58.000000 zcmds-1.4.9/src/zcmds/cmds/common/vidhero.py
+-rw-rw-rw-   0        0        0     5987 2023-03-14 20:56:14.000000 zcmds-1.4.9/src/zcmds/cmds/common/vidinfo.py
+-rw-rw-rw-   0        0        0     1242 2022-09-03 19:04:52.000000 zcmds-1.4.9/src/zcmds/cmds/common/vidlist.py
+-rw-rw-rw-   0        0        0     2777 2022-09-03 19:04:52.000000 zcmds-1.4.9/src/zcmds/cmds/common/vidmatrix.py
+-rw-rw-rw-   0        0        0     1705 2022-11-09 03:22:17.000000 zcmds-1.4.9/src/zcmds/cmds/common/vidmute.py
+-rw-rw-rw-   0        0        0     1688 2023-03-23 20:09:17.000000 zcmds-1.4.9/src/zcmds/cmds/common/vidshrink.py
+-rw-rw-rw-   0        0        0     1726 2023-02-26 19:57:37.000000 zcmds-1.4.9/src/zcmds/cmds/common/vidspeed.py
+-rw-rw-rw-   0        0        0     1807 2022-07-27 02:41:03.000000 zcmds-1.4.9/src/zcmds/cmds/common/vidvol.py
+-rw-rw-rw-   0        0        0     5750 2023-04-03 19:35:12.000000 zcmds-1.4.9/src/zcmds/cmds/common/vidwebmaster.py
+-rw-rw-rw-   0        0        0     3408 2023-03-24 04:25:59.000000 zcmds-1.4.9/src/zcmds/cmds/common/whichall.py
+-rw-rw-rw-   0        0        0      933 2023-03-23 20:09:17.000000 zcmds-1.4.9/src/zcmds/cmds/common/zcmds_main.py
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.501712 zcmds-1.4.9/src/zcmds/cmds/darwin/
+-rw-rw-rw-   0        0        0        0 2022-02-21 10:38:44.000000 zcmds-1.4.9/src/zcmds/cmds/darwin/__init__.py
+-rw-rw-rw-   0        0        0     3505 2022-11-04 21:13:40.000000 zcmds-1.4.9/src/zcmds/cmds/darwin/test_net_connection.py
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.504712 zcmds-1.4.9/src/zcmds/cmds/linux/
+-rw-rw-rw-   0        0        0       34 2022-02-21 09:21:39.000000 zcmds-1.4.9/src/zcmds/cmds/linux/TODO
+-rw-rw-rw-   0        0        0        0 2022-02-21 10:38:44.000000 zcmds-1.4.9/src/zcmds/cmds/linux/__init__.py
+-rw-rw-rw-   0        0        0      366 2023-04-02 09:48:39.000000 zcmds-1.4.9/src/zcmds/cmds.py
+-rw-rw-rw-   0        0        0     1792 2023-04-04 01:35:43.000000 zcmds-1.4.9/src/zcmds/cmds.txt
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.505713 zcmds-1.4.9/src/zcmds/install/
+-rw-rw-rw-   0        0        0        0 2022-02-21 03:22:36.000000 zcmds-1.4.9/src/zcmds/install/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.508714 zcmds-1.4.9/src/zcmds/install/darwin/
+-rw-rw-rw-   0        0        0        0 2022-02-24 11:15:15.000000 zcmds-1.4.9/src/zcmds/install/darwin/__init__.py
+-rw-rw-rw-   0        0        0     1438 2022-07-27 03:33:16.000000 zcmds-1.4.9/src/zcmds/install/darwin/darwin_update.py
+-rw-rw-rw-   0        0        0      617 2022-02-21 07:57:18.000000 zcmds-1.4.9/src/zcmds/install/darwin/macOS_key_bindings.dict
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.518715 zcmds-1.4.9/src/zcmds/util/
+-rw-rw-rw-   0        0        0        0 2022-02-21 05:09:08.000000 zcmds-1.4.9/src/zcmds/util/__init__.py
+-rw-rw-rw-   0        0        0     1097 2023-04-02 22:01:35.000000 zcmds-1.4.9/src/zcmds/util/config.py
+-rw-rw-rw-   0        0        0     1710 2023-03-31 05:34:41.000000 zcmds-1.4.9/src/zcmds/util/file_search_and_replacer.py
+-rw-rw-rw-   0        0        0     1063 2023-03-31 05:28:50.000000 zcmds-1.4.9/src/zcmds/util/file_searcher.py
+-rw-rw-rw-   0        0        0     4309 2023-04-02 06:56:44.000000 zcmds-1.4.9/src/zcmds/util/fileutils.py
+-rw-rw-rw-   0        0        0      669 2022-02-21 05:08:59.000000 zcmds-1.4.9/src/zcmds/util/index_all_files.py
+-rw-rw-rw-   0        0        0      381 2023-04-03 18:54:53.000000 zcmds-1.4.9/src/zcmds/util/prompt_input.py
+-rw-rw-rw-   0        0        0      532 2023-04-03 19:36:05.000000 zcmds-1.4.9/src/zcmds/util/say.py
+-rw-rw-rw-   0        0        0      249 2023-02-02 07:49:35.000000 zcmds-1.4.9/src/zcmds/util/sound.py
+-rw-rw-rw-   0        0        0      147 2023-04-06 18:04:23.000000 zcmds-1.4.9/src/zcmds/version.py
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.453714 zcmds-1.4.9/src/zcmds.egg-info/
+-rw-rw-rw-   0        0        0     7554 2023-04-06 18:07:06.000000 zcmds-1.4.9/src/zcmds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2691 2023-04-06 18:07:06.000000 zcmds-1.4.9/src/zcmds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-06 18:07:06.000000 zcmds-1.4.9/src/zcmds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1734 2023-04-06 18:07:06.000000 zcmds-1.4.9/src/zcmds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      223 2023-04-06 18:07:06.000000 zcmds-1.4.9/src/zcmds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-06 18:07:06.000000 zcmds-1.4.9/src/zcmds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-06 18:07:06.521713 zcmds-1.4.9/tests/
+-rw-rw-rw-   0        0        0      876 2022-11-05 20:55:29.000000 zcmds-1.4.9/tests/test_main.py
+-rw-rw-rw-   0        0        0      260 2023-02-02 07:49:35.000000 zcmds-1.4.9/tests/test_sound.py
+-rw-rw-rw-   0        0        0      746 2023-01-03 06:43:04.000000 zcmds-1.4.9/tests/test_version.py
+-rw-rw-rw-   0        0        0      451 2023-02-02 07:49:35.000000 zcmds-1.4.9/tox.ini
+-rw-rw-rw-   0        0        0      275 2023-01-01 07:58:23.000000 zcmds-1.4.9/upload_package.sh
```

### Comparing `zcmds-1.4.81/.github/workflows/lint.yml` & `zcmds-1.4.9/.github/workflows/lint.yml`

 * *Files 18% similar despite different names*

```diff
@@ -26,8 +26,10 @@
       run: |
         python -m pip install --upgrade pip
         sudo apt-get install libasound2-dev
         python -m pip install .
         python -m pip install -r requirements.testing.txt
     - name: Run Linting
       run: |
-        ./lint
+        flake8 src
+        pylint src
+        mypy src
```

### Comparing `zcmds-1.4.81/.github/workflows/push_ubuntu.yml` & `zcmds-1.4.9/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/.github/workflows/push_win.yml` & `zcmds-1.4.9/.github/workflows/push_win.yml`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     - name: Print device
       run: Get-CimInstance Win32_SoundDevice | fl *
     - name: Install Scream
       shell: powershell
       run: |
         Start-Service audio*
         Invoke-WebRequest https://github.com/duncanthrax/scream/releases/download/3.6/Scream3.6.zip -OutFile C:\Scream3.6.zip
-        Expand-Archive -Path C:\Scream3.6.zip -DestinationPath C:\Scream
+        Extract-7Zip -Path C:\Scream3.6.zip -DestinationPath C:\Scream
         $cert = (Get-AuthenticodeSignature C:\Scream\Install\driver\Scream.sys).SignerCertificate
         $store = [System.Security.Cryptography.X509Certificates.X509Store]::new("TrustedPublisher", "LocalMachine")
         $store.Open("ReadWrite")
         $store.Add($cert)
         $store.Close()
         cd C:\Scream\Install\driver
         C:\Scream\Install\helpers\devcon install Scream.inf *Scream
```

### Comparing `zcmds-1.4.81/.gitignore` & `zcmds-1.4.9/.gitignore`

 * *Files 17% similar despite different names*

```diff
@@ -130,16 +130,8 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 .activate.sh
-.DS_Store
-src/zcmds/cmds/common/losslesscut_bins/**
-.aider*
-
-!.aider.conf.yml
-!.aiderignore
-
-tests/test_data/rembg-nobackground.webm
-
+.DS_Store
```

### Comparing `zcmds-1.4.81/.pylintrc` & `zcmds-1.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/make_venv.py` & `zcmds-1.4.9/make_venv.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/pyproject.toml` & `zcmds-1.4.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 name = "zcmds"
 description = "Cross platform(ish) productivity commands written in python."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["zcmds"]
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
-dynamic = ["dependencies", "scripts", "entry-points", "version"]
+dynamic = ["dependencies"]
 # Change this with the version number bump.
 # Also make the change in zcmds/version.py
-# version = "1.4.32"
+version = "1.4.9"
 
 [tool.setuptools.dynamic]
-dependencies = { file = ["requirements.txt"] }
-
-[tool.mypy]
-ignore_missing_imports = true
+dependencies = {file = ["requirements.txt"]}
```

### Comparing `zcmds-1.4.81/src/zcmds/assets/bell.mp3` & `zcmds-1.4.9/src/zcmds/assets/bell.mp3`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/fixinternet.py` & `zcmds-1.4.9/src/zcmds/cmds/common/fixinternet.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/gitsummary.py` & `zcmds-1.4.9/src/zcmds/cmds/common/gitsummary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Returns a git summary of the current directory.
 """
 
+
 import json
 import os
 import subprocess
 import sys
 from argparse import Action, ArgumentParser
 from collections import OrderedDict
 from datetime import datetime, timedelta
@@ -152,22 +153,14 @@
             sys.exit(1)
     else:
         repo = args.repo
         if not os.path.isdir(repo):
             sys.stderr.write(f"Error: {repo} is not a directory\n")
             sys.exit(1)
     os.chdir(repo)
-    if not os.path.exists(".git"):
-        sys.stderr.write(f"Error: {repo} is not a git repo\n")
-        sys.exit(1)
-    if 0 != os.system("git status"):
-        sys.stderr.write(
-            f"Error: {repo} has a .git dir but is not a valid git repo (corrupted?)\n"
-        )
-        sys.exit(1)
     save_config(CONFIG_NAME, config)
     start_date_dt = datetime.strptime(start_date, "%Y-%m-%d")
     end_date_dt = datetime.strptime(end_date, "%Y-%m-%d")
     repo = ""
     cmd = create_cmd(start_date_dt - timedelta(days=1), end_date_dt + timedelta(days=1))
     sys.stderr.write(f"Running: {cmd}\n")
     cp: subprocess.CompletedProcess = subprocess.run(
@@ -206,17 +199,16 @@
     data = parse_to_json_data(repo_url, start_date_dt, end_date_dt, stdout.splitlines())
     json_str = json.dumps(data, indent=4)
     write_output(json_str)
     return 0
 
 
 def unit_test() -> None:
-    # "C:\Users\niteris\dev\Accessibility-Test-Framework-for-Android" --start_date 2023-11-15 --end_date 2023-11-30 --output "gitsummary\2023-11-15_2023-11-30\Accessibility-Test-Framework-for-Android.json"
     args = [
-        r"C:\Users\niteris\dev\Accessibility-Test-Framework-for-Android",
+        r"C:\Users\niteris\dev\androidmonitor-backend",
         "--output",
         "out.json",
         "--start_date",
         "2023-01-01",
         "--end_date",
         "2023-01-31",
     ]
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/img2vid.py` & `zcmds-1.4.9/src/zcmds/cmds/common/img2vid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Stitches a bunch of files together to make a video.
 """
 
+
 # pylint: skip-file
 
 import argparse
 import os
 import subprocess
 import sys
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/imgai.py` & `zcmds-1.4.9/src/zcmds/cmds/common/imgai.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/obs_organize.py` & `zcmds-1.4.9/src/zcmds/cmds/common/obs_organize.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/openaicfg.py` & `zcmds-1.4.9/src/zcmds/cmds/common/openaicfg.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/pdf2png.py` & `zcmds-1.4.9/src/zcmds/cmds/common/pdf2png.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-# pylint: skip-file
-
-
-import builtins
-import os
-import sys
-import traceback
-from argparse import ArgumentParser
-
-from pdf2image import convert_from_path  # type: ignore
-
-
-def main() -> None:
-    parser = ArgumentParser()
-    parser.add_argument("input_pdf", help="input", nargs="?")
-    parser.add_argument("--first_page", help="First page to include in the output.")
-    parser.add_argument(
-        "--last_page", help="Last page (inclusive) to include in the output."
-    )
-    parser.add_argument("--dpi", help="Dpi to render the output in")
-    args = parser.parse_args()
-
-    if args.input_pdf is None:
-        args.input_pdf = input("input pdf: ")
-
-    if args.first_page is None:
-        args.first_page = int(input("first page: "))
-        if args.first_page < 0:
-            raise ValueError("first page must be >= 0")
-
-    if args.last_page is None:
-        args.last_page = int(input("last page: "))
-        if args.last_page < 0:
-            raise ValueError("last page must be >= 0")
-
-    if args.dpi is None:
-        args.dpi = int(input("dpi: "))
-
-    save_dir = os.path.splitext(args.input_pdf)[0]
-    os.makedirs(save_dir, exist_ok=True)
-    infile = save_dir + ".pdf"
-    images = convert_from_path(
-        infile, first_page=args.first_page, last_page=args.last_page, dpi=args.dpi
-    )
-    for i, image in enumerate(images):
-        output_png = os.path.join(save_dir, f"{i+args.first_page}.png")
-        if os.path.isfile(output_png):
-            os.remove(output_png)
-        print(f"Writing: {output_png}")
-        image.save(output_png)
-        if not os.path.isfile(output_png):
-            print(f"Error: could not save {output_png}")
-
-
-if __name__ == "__main__":
-    try:
-        main()
-    except builtins.BaseException as e:
-        traceback.print_exc()
-        print(f"Error: could not convert pdf to png, because of {e}")
-        if sys.platform == "win32":
-            print("--> Try running `choco install poppler`")
-        elif sys.platform == "darwin":
-            print("--> Try running `brew install poppler`")
-        elif sys.platform == "linux":
-            print(
-                "--> Try running `sudo apt-get install poppler-utils`"
-            )  # Should this be poppler?
-        else:
-            print(f"Unexpected os {sys.platform}")
-        sys.exit(1)
-    sys.exit(0)
+# pylint: skip-file
+
+
+import builtins
+import os
+import sys
+import traceback
+from argparse import ArgumentParser
+
+from pdf2image import convert_from_path  # type: ignore
+
+
+def main() -> None:
+    parser = ArgumentParser()
+    parser.add_argument("input_pdf", help="input", nargs="?")
+    parser.add_argument("--first_page", help="First page to include in the output.")
+    parser.add_argument(
+        "--last_page", help="Last page (inclusive) to include in the output."
+    )
+    parser.add_argument("--dpi", help="Dpi to render the output in")
+    args = parser.parse_args()
+
+    if args.input_pdf is None:
+        args.input_pdf = input("input pdf: ")
+
+    if args.first_page is None:
+        args.first_page = int(input("first page: "))
+        if args.first_page < 0:
+            raise ValueError("first page must be >= 0")
+
+    if args.last_page is None:
+        args.last_page = int(input("last page: "))
+        if args.last_page < 0:
+            raise ValueError("last page must be >= 0")
+
+    if args.dpi is None:
+        args.dpi = int(input("dpi: "))
+
+    save_dir = os.path.splitext(args.input_pdf)[0]
+    os.makedirs(save_dir, exist_ok=True)
+    infile = save_dir + ".pdf"
+    images = convert_from_path(
+        infile, first_page=args.first_page, last_page=args.last_page, dpi=args.dpi
+    )
+    for i, image in enumerate(images):
+        output_png = os.path.join(save_dir, f"{i+args.first_page}.png")
+        if os.path.isfile(output_png):
+            os.remove(output_png)
+        print(f"Writing: {output_png}")
+        image.save(output_png)
+        if not os.path.isfile(output_png):
+            print(f"Error: could not save {output_png}")
+
+
+if __name__ == "__main__":
+    try:
+        main()
+    except builtins.BaseException as e:
+        traceback.print_exc()
+        print(f"Error: could not convert pdf to png, because of {e}")
+        if sys.platform == "win32":
+            print("--> Try running `choco install poppler`")
+        elif sys.platform == "darwin":
+            print("--> Try running `brew install poppler`")
+        elif sys.platform == "linux":
+            print(
+                "--> Try running `sudo apt-get install poppler-utils`"
+            )  # Should this be poppler?
+        else:
+            print(f"Unexpected os {sys.platform}")
+        sys.exit(1)
+    sys.exit(0)
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/pdf2txt.py` & `zcmds-1.4.9/src/zcmds/cmds/common/pdf2txt.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/printenv.py` & `zcmds-1.4.9/src/zcmds/cmds/common/printenv.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 
 def main():
     """Prints the environment variables"""
     # Copy the environment variables to a new dictionary
     env = os.environ.copy()
     # Remove the path variable
     paths = None
-    env_items = list(env.items())
-    # sort
-    env_items = sorted(env_items, key=lambda x: x[0].lower())
-    for key, val in env_items:
+    for key, val in env.items():
         if key.lower() == "path":
             paths = val
             continue
         else:
             print(f"{key}={val}")
     print("PATH:")
     for path in paths.split(os.pathsep):
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/say.py` & `zcmds-1.4.9/src/zcmds/cmds/common/say.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/stereo2mono.py` & `zcmds-1.4.9/src/zcmds/cmds/common/stereo2mono.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import argparse
-import os
-import sys
-
-
-def _apply_name_suffix(path, new_name_suffix):
-    """
-    Adds a suffix to the name of a file.
-    _add_name_suffix("/path/to/file.ext", "_left") -> "/path/to/file_left.ext"
-    """
-    name, ext = os.path.splitext(path)
-    return f"{name}{new_name_suffix}{ext}"
-
-
-def _apply_ext(path, new_ext):
-    """
-    Sets the extension of a file.
-    _apply_ext("/path/to/file.ext", ".wav") -> "/path/to/file.wav"
-    """
-    name, _ = os.path.splitext(path)
-    return f"{name}{new_ext}"
-
-
-def _print_file_exists(path):
-    if os.path.exists(path):
-        print(f"Generated {path}")
-    else:
-        print(f"WARNING: failed to generate {path}")
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description="Print video durations\n",
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser.add_argument("vidfile", help="Path to vid file", nargs="?")
-    parser.add_argument("outwavfile", help="Path to output wav file", nargs="?")
-    args = parser.parse_args()
-    path = args.vidfile or input("in vid file: ")
-    out_wav = args.outwavfile or path
-    out_wav = _apply_ext(out_wav, ".wav")
-    if not os.path.exists(path):
-        print(f"{path} does not exist")
-        sys.exit(1)
-    out_left_path = _apply_name_suffix(out_wav, "_left")
-    out_right_path = _apply_name_suffix(out_wav, "_right")
-    cmd0 = f'static_ffmpeg -y -i "{path}" -filter_complex "[0:a]channelsplit=channel_layout=stereo:channels=FR[right]" -map "[right]" "{out_right_path}"'
-    cmd1 = f'static_ffmpeg -y -i "{path}" -filter_complex "[0:a]channelsplit=channel_layout=stereo:channels=FL[left]" -map "[left]" "{out_left_path}"'
-    print(f"Executing:\n  {cmd0}\n")
-    os.system(cmd0)
-    print(f"Executing:\n  {cmd1}\n")
-    os.system(cmd1)
-    print("\nDone\n")
-    _print_file_exists(out_right_path)
-    _print_file_exists(out_left_path)
-
-
-if __name__ == "__main__":
-    main()
+import argparse
+import os
+import sys
+
+
+def _apply_name_suffix(path, new_name_suffix):
+    """
+    Adds a suffix to the name of a file.
+    _add_name_suffix("/path/to/file.ext", "_left") -> "/path/to/file_left.ext"
+    """
+    name, ext = os.path.splitext(path)
+    return f"{name}{new_name_suffix}{ext}"
+
+
+def _apply_ext(path, new_ext):
+    """
+    Sets the extension of a file.
+    _apply_ext("/path/to/file.ext", ".wav") -> "/path/to/file.wav"
+    """
+    name, _ = os.path.splitext(path)
+    return f"{name}{new_ext}"
+
+
+def _print_file_exists(path):
+    if os.path.exists(path):
+        print(f"Generated {path}")
+    else:
+        print(f"WARNING: failed to generate {path}")
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description="Print video durations\n",
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser.add_argument("vidfile", help="Path to vid file", nargs="?")
+    parser.add_argument("outwavfile", help="Path to output wav file", nargs="?")
+    args = parser.parse_args()
+    path = args.vidfile or input("in vid file: ")
+    out_wav = args.outwavfile or path
+    out_wav = _apply_ext(out_wav, ".wav")
+    if not os.path.exists(path):
+        print(f"{path} does not exist")
+        sys.exit(1)
+    out_left_path = _apply_name_suffix(out_wav, "_left")
+    out_right_path = _apply_name_suffix(out_wav, "_right")
+    cmd0 = f'static_ffmpeg -y -i "{path}" -filter_complex "[0:a]channelsplit=channel_layout=stereo:channels=FR[right]" -map "[right]" "{out_right_path}"'
+    cmd1 = f'static_ffmpeg -y -i "{path}" -filter_complex "[0:a]channelsplit=channel_layout=stereo:channels=FL[left]" -map "[left]" "{out_left_path}"'
+    print(f"Executing:\n  {cmd0}\n")
+    os.system(cmd0)
+    print(f"Executing:\n  {cmd1}\n")
+    os.system(cmd1)
+    print("\nDone\n")
+    _print_file_exists(out_right_path)
+    _print_file_exists(out_left_path)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vid2gif.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vid2gif.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,35 +9,29 @@
 def main():
     parser = argparse.ArgumentParser(
         description="Extracts a video frame.\n",
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument("input", help="input")
     parser.add_argument("--outname", help="output name of the file")
-    parser.add_argument(
-        "--height", help="height of the output image", default=320, type=int
-    )
-    parser.add_argument("--fps", help="frames per second", default=10, type=int)
     args = parser.parse_args()
     infile = args.input
     if args.outname:
         output_path = os.path.splitext(args.outname)[0]
     else:
         output_path = os.path.splitext(args.input)[0]
     if not os.path.exists(infile):
         print(f"{infile} does not exist")
         sys.exit(1)
 
     if not os.path.isdir(output_path):
         os.makedirs(output_path)
-    height = args.height
-    fps = args.fps
     # ffmpeg -i foo.avi -r 1 -s WxH -f image2 foo-%03d.jpeg -ss -frames:v
     file_out = f'"{output_path}.gif"'
-    cmd = f'static_ffmpeg -hide_banner -y -i "{infile}" -vf "fps={fps},scale={height}:-1:flags=lanczos,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse" -loop 0 {file_out}'
+    cmd = f'static_ffmpeg -hide_banner -y -i "{infile}" -vf "fps=10,scale=320:-1:flags=lanczos,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse" -loop 0 {file_out}'
     print(f"Executing:\n  {cmd}\n")
     subprocess.call(cmd, shell=True, universal_newlines=True)
     if not os.path.exists(output_path):
         print(f"Error, did not generate {output_path}")
         print(f"Error from cmd:\n  {cmd}\n")
     else:
         print(f"\nGenerated gif: {file_out}")
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vid2jpg.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vid2jpg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-# pylint: skip-file
-
-import argparse
-import os
-import subprocess
-import sys
-
-
-def stripext(s: str) -> str:
-    return os.path.splitext(s)[0]
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description="Extracts a video frame.\n",
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser.add_argument("input", help="input")
-    parser.add_argument("--timestamp", help="start of the clip")
-    parser.add_argument("--length", help="length of the clip")
-    parser.add_argument("--outname", help="output name of the file")
-    parser.add_argument("--no-open-folder", action="store_true", help="debug")
-    args = parser.parse_args()
-    infile = args.input
-    timestamp = args.timestamp or input("timestamp: ")
-    length = args.length or input("length (secs): ")
-    do_open_folder = not args.no_open_folder
-    if args.outname:
-        output_path = os.path.splitext(args.outname)[0]
-    else:
-        output_path = os.path.splitext(args.input)[0]
-    output_path = output_path + "_imgs"
-    if not os.path.exists(infile):
-        print(f"{infile} does not exist")
-        sys.exit(1)
-
-    if not os.path.isdir(output_path):
-        os.makedirs(output_path)
-    # ffmpeg -i foo.avi -r 1 -s WxH -f image2 foo-%03d.jpeg -ss -frames:v
-    file_output_fmt = f'"{output_path}/%03d.jpg"'
-
-    cmd = f'static_ffmpeg -hide_banner -i "{infile}" -ss {timestamp} -t {length} -f image2 {file_output_fmt}'
-    print(f"Executing:\n  {cmd}\n")
-    subprocess.call(cmd, shell=True, universal_newlines=True, stderr=subprocess.DEVNULL)
-    if not os.path.exists(output_path):
-        print(f"Error, did not generate {output_path}")
-        print(f"Error from cmd:\n  {cmd}\n")
-    else:
-        print(f"Generated images are in directory: {output_path}")
-        if do_open_folder:
-            if sys.platform == "win32":
-                os.system(f"start explorer {output_path}")
-
-
-if __name__ == "__main__":
-    main()
+# pylint: skip-file
+
+import argparse
+import os
+import subprocess
+import sys
+
+
+def stripext(s: str) -> str:
+    return os.path.splitext(s)[0]
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description="Extracts a video frame.\n",
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser.add_argument("input", help="input")
+    parser.add_argument("--timestamp", help="start of the clip")
+    parser.add_argument("--length", help="length of the clip")
+    parser.add_argument("--outname", help="output name of the file")
+    args = parser.parse_args()
+    infile = args.input
+    timestamp = args.timestamp or input("timestamp: ")
+    length = args.length or input("length (secs): ")
+    if args.outname:
+        output_path = os.path.splitext(args.outname)[0]
+    else:
+        output_path = os.path.splitext(args.input)[0]
+    output_path = output_path + "_imgs"
+    if not os.path.exists(infile):
+        print(f"{infile} does not exist")
+        sys.exit(1)
+
+    if not os.path.isdir(output_path):
+        os.makedirs(output_path)
+    # ffmpeg -i foo.avi -r 1 -s WxH -f image2 foo-%03d.jpeg -ss -frames:v
+    file_output_fmt = f'"{output_path}/%03d.jpg"'
+
+    cmd = f'static_ffmpeg -hide_banner -i "{infile}" -ss {timestamp} -t {length} -f image2 {file_output_fmt}'
+    print(f"Executing:\n  {cmd}\n")
+    subprocess.call(cmd, shell=True, universal_newlines=True, stderr=subprocess.DEVNULL)
+    if not os.path.exists(output_path):
+        print(f"Error, did not generate {output_path}")
+        print(f"Error from cmd:\n  {cmd}\n")
+    else:
+        print(f"Generated images are in directory: {output_path}")
+        if sys.platform == "win32":
+            os.system(f"start explorer {output_path}")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vid2mp3.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vid2mp3.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,48 +2,38 @@
 
 import argparse
 import os
 import sys
 from pathlib import Path
 
 
-def run(filename: str, output: str | None, normalize: bool) -> int:
+def main() -> int:
+    parser = argparse.ArgumentParser()
+    parser.add_argument("filename", help="The video file to convert to mp3")
+    parser.add_argument("-o", "--output", help="The output file name")
+    parser.add_argument("-n", "--normalize", action="store_true")
+    args = parser.parse_args()
+    filename = sys.argv[1:2][0]
     if not os.path.exists(filename):
         print(f"{filename} does not exist")
         sys.exit(1)
-    if output:
-        out_path = output
+    if args.output:
+        out_path = args.output
         assert out_path.endswith(".mp3")
     else:
-        out_path = str(Path(filename).with_suffix(".mp3"))
+        out_path = Path(filename).with_suffix(".mp3")
     cmd = f'static_ffmpeg -hide_banner -i "{filename}" -vn -c:a libmp3lame -y ".{out_path}"'
     print(f"Executing:\n  {cmd}")
     os.system(cmd)
-    assert os.path.exists(f".{out_path}")
-    if not normalize:
+    if not args.normalize:
         os.rename(f".{out_path}", f"{out_path}")
     else:
         cmd = f'audnorm ".{out_path}" "{out_path}"'
         print(f"Executing:\n  {cmd}")
-        rtn = os.system(cmd)
-        if rtn != 0:
-            print(f"Failed to normalize {out_path}")
-            return 1
+        os.system(cmd)
         os.remove(f".{out_path}")
     os.system(cmd)
     return 0
 
 
-def main() -> int:
-    parser = argparse.ArgumentParser()
-    parser.add_argument("filename", help="The video file to convert to mp3")
-    parser.add_argument("-o", "--output", help="The output file name")
-    parser.add_argument("-n", "--normalize", action="store_true")
-    args = parser.parse_args()
-    filename = sys.argv[1:2][0]
-    print(f"Converting {filename} to mp3")
-    rtn = run(filename, args.output, args.normalize)
-    return rtn
-
-
 if __name__ == "__main__":
     main()
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vid2webm.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vid2mp4.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,43 @@
-# pylint: skip-file
-
-import argparse
-import os
-import sys
-from pathlib import Path
-from typing import Optional
-
-VERSION = "0.1.0"
-
-
-def main():
-    parser = argparse.ArgumentParser(description="Convert video to mp4")
-    parser.add_argument("filename", help="Path to video file", nargs="?")
-    parser.add_argument("--rencode", help="rencode the video", action="store_true")
-    parser.add_argument("--version", help="Print version and exit", action="store_true")
-    parser.add_argument("--crf", help="CRF value", default=None, type=Optional[int])
-    args = parser.parse_args()
-    filename = args.filename or input("filname: ")
-    if not os.path.exists(filename):
-        print(f"{filename} does not exist")
-        sys.exit(1)
-    out_path = Path(filename).with_suffix(".webm")
-    crf = args.crf or int(input("crf: "))
-    cmd = f'static_ffmpeg -hide_banner -i "{filename}" -preset veryslow -vcodec libvpx -acodec libvorbis -crf {crf} "{out_path}"'
-    os.system(cmd)
-    print(f"Generated {out_path}")
-
-
-if __name__ == "__main__":
-    main()
+# pylint: skip-file
+
+import argparse
+import os
+import sys
+from pathlib import Path
+
+VERSION = "0.1.0"
+
+
+def main():
+    parser = argparse.ArgumentParser(description="Convert video to mp4")
+    parser.add_argument("filename", help="Path to video file", nargs="?")
+    parser.add_argument("--rencode", help="rencode the video", action="store_true")
+    parser.add_argument("--version", help="Print version and exit", action="store_true")
+    args = parser.parse_args()
+    if args.version:
+        print(VERSION)
+        sys.exit(0)
+    filename = args.filename
+    if not os.path.exists(filename):
+        print(f"{filename} does not exist")
+        sys.exit(1)
+    out_path = Path(filename).with_suffix(".mp4")
+    if out_path.exists():
+        # Remove suffix from file name and add _converted.mp4
+        out_path = (
+            Path(filename)
+            .with_suffix("")
+            .with_name(f"{Path(filename).stem}_converted.mp4")
+        )
+
+    # -c:v libx264
+    if args.rencode:
+        cmd = f'static_ffmpeg -hide_banner -i "{filename}" -preset veryslow -vcodec libx264 -preset -crf 18 -c:a copy -y "{out_path}"'
+    else:
+        cmd = f'ffmpeg -i "{filename}" -c copy "{out_path}"'
+    os.system(cmd)
+    print(f"Generated {out_path}")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vidcat.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vidcat.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,21 +40,15 @@
 
 
 def get_resolution(infile: str) -> Resolution:
     cmd = f'static_ffprobe -v error -select_streams v:0 -show_entries stream=width,height -of csv=p=0 "{infile}"'
     rtn, stdout, _ = exec(cmd)
     if rtn != 0:
         print(f"{__file__}: WARNING: '{cmd}' returned code {rtn}")
-    try:
-        width, height = stdout.split(",")
-    except ValueError:
-        print(f"{__file__}: ERROR: could not parse resolution from '{stdout}'")
-        import sys
-
-        sys.exit(1)
+    width, height = stdout.split(",")
     return Resolution(int(width), int(height))
 
 
 def get_highest_resolution(infiles: list[str]) -> Resolution:
     resolutions = [get_resolution(infile) for infile in infiles]
     return max(resolutions, key=lambda resolution: resolution.width)
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vidclip.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vidclip.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/viddur.py` & `zcmds-1.4.9/src/zcmds/cmds/common/viddur.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vidhero.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vidhero.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vidinfo.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vidinfo.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vidlist.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vidlist.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vidmatrix.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vidmatrix.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vidshrink.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vidshrink.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# pylint: skip-file
-
-import argparse
-import os
-import sys
-
-
-def main():
-    # Expects a single argument: the path to the video file to shrink
-    parser = argparse.ArgumentParser(description="Shrink a video file")
-    parser.add_argument("video_path", help="Path to the video file to shrink")
-    # Adds optional crf argument
-    parser.add_argument("--crf", help="CRF value to use", type=int, default=26)
-    # Adds optional height argument
-    parser.add_argument(
-        "--height", help="height of the output video, e.g 1080 = 1080p", default=480
-    )
-    parser.add_argument(
-        "--downmix", help="downmix the audio from stereo to mono", action="store_true"
-    )
-    parser.add_argument(
-        "--fps",
-        help="frames per second of the output video, default is no framerate change",
-        default=None,
-    )
-    args = parser.parse_args()
-    filename = args.video_path
-    if not os.path.exists(filename):
-        print(f"{filename} does not exist")
-        sys.exit(1)
-    height = args.height
-    crf = args.crf
-    path, _ = os.path.splitext(filename)
-    out_path = f"{path}_small.mp4"
-
-    downmix_stmt = "-ac 1" if args.downmix else ""
-    fps_stmt = f"fps=fps={args.fps}," if args.fps else ""
-    filter_stmt = f'-vf "{fps_stmt}scale=trunc(oh*a/2)*2:{height}"'
-    # trunc(oh*...) fixes issue with libx264 encoder not liking an add number of width pixels.
-    cmd = f'static_ffmpeg -hide_banner -y -i "{filename}" {filter_stmt} {downmix_stmt} -movflags +faststart -preset veryslow -c:v libx264 -crf {crf} "{out_path}"'
-    print(f"Running:\n  {cmd}")
-    os.system(cmd)
-
-
-if __name__ == "__main__":
-    main()
+# pylint: skip-file
+
+import argparse
+import os
+import sys
+
+
+def main():
+    # Expects a single argument: the path to the video file to shrink
+    parser = argparse.ArgumentParser(description="Shrink a video file")
+    parser.add_argument("video_path", help="Path to the video file to shrink")
+    # Adds optional crf argument
+    parser.add_argument("--crf", help="CRF value to use", type=int, default=26)
+    # Adds optional height argument
+    parser.add_argument(
+        "--height", help="height of the output video, e.g 1080 = 1080p", default=480
+    )
+    parser.add_argument(
+        "--downmix", help="downmix the audio from stereo to mono", action="store_true"
+    )
+    parser.add_argument(
+        "--fps",
+        help="frames per second of the output video, default is no framerate change",
+        default=None,
+    )
+    args = parser.parse_args()
+    filename = args.video_path
+    if not os.path.exists(filename):
+        print(f"{filename} does not exist")
+        sys.exit(1)
+    height = args.height
+    crf = args.crf
+    path, _ = os.path.splitext(filename)
+    out_path = f"{path}_small.mp4"
+
+    downmix_stmt = "-ac 1" if args.downmix else ""
+    fps_stmt = f"fps=fps={args.fps}," if args.fps else ""
+    filter_stmt = f'-vf "{fps_stmt}scale=trunc(oh*a/2)*2:{height}"'
+    # trunc(oh*...) fixes issue with libx264 encoder not liking an add number of width pixels.
+    cmd = f'static_ffmpeg -hide_banner -y -i "{filename}" {filter_stmt} {downmix_stmt} -movflags +faststart -preset veryslow -c:v libx264 -crf {crf} "{out_path}"'
+    print(f"Running:\n  {cmd}")
+    os.system(cmd)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vidspeed.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vidspeed.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vidvol.py` & `zcmds-1.4.9/src/zcmds/cmds/common/audnorm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 """
     Normalizes the audio of a video file.
 """
 
 import argparse
 import os
+import subprocess
 
+from static_ffmpeg import add_paths  # type: ignore
 
-def _is_media_file(filename: str) -> bool:
-    if not os.path.isfile(filename):
-        return False
-    ext = os.path.splitext(filename.lower())[1]
-    return ext in [".mp4", ".mkv", ".avi", ".mov", ".mp3", ".wav"]
 
-
-def ffmpeg_adjust_volume(filename: str, volume: float, out_file: str):
+def ffprobe_duration(filename: str) -> float:
     """
-    Adjusts the volume of a video file.
+    Uses ffprobe to get the duration of a video file.
     """
-    cmd = f'static_ffmpeg  -i "{filename}" -filter:a "volume={volume}" "{out_file}"'
-    print(f"Executing:\n  {cmd}")
-    os.system(cmd)
+    add_paths(weak=True)
+    cmd = f"ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 {filename}"
+    result = subprocess.check_output(cmd, shell=True, universal_newlines=True)
+    result = result.replace("\n", "").replace(" ", "")
+    return float(result)
 
 
-def ffmpeg_print_volume_detect(filename: str) -> None:
-    """
-    Uses ffmpeg to get the volume of a video file.
-    """
-    cmd = f'static_ffmpeg -i "{filename}" -nostats -hide_banner -af "volumedetect" -f null /dev/null'
-    print("Executing:\n  " + cmd + "\n")
-    os.system(cmd)
+def _is_media_file(filename: str) -> bool:
+    if not os.path.isfile(filename):
+        return False
+    ext = os.path.splitext(filename.lower())[1]
+    return ext in [".mp4", ".mkv", ".avi", ".mov", ".mp3", ".wav"]
 
 
 def main():
     parser = argparse.ArgumentParser(
-        description="Prints the video volume or sets it.\n",
+        description="Print video durations\n",
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument("vidfile", help="Path to vid file", nargs="?")
-    parser.add_argument("--out", help="Path to vid file")
-    parser.add_argument("--volume", help="Volume to adjust to")
+    parser.add_argument("out", help="Path to vid file", nargs="?")
     args = parser.parse_args()
-    vidfile = args.vidfile or input("in vid file: ")
-    if args.out is None and args.volume is None:
-        ffmpeg_print_volume_detect(vidfile)
-        return
-    vol = args.volume or input("volume: ")
+    path = args.vidfile or input("in vid file: ")
     out = args.out or input("out vid file: ")
-    if len(os.path.dirname(vidfile)):
+    if len(os.path.dirname(out)):
         os.makedirs(os.path.dirname(out), exist_ok=True)
-    assert _is_media_file(vidfile), f"{vidfile} is not a media file"
-    ffmpeg_adjust_volume(vidfile, vol, out)
+    assert _is_media_file(path), f"{path} is not a media file"
+    add_paths(weak=True)
+    cmd = f'ffmpeg-normalize -f "{path}" -o "{out}" -c:a libmp3lame -b:a 192k'
+    print(f"Executing:\n  {cmd}")
+    os.system(cmd)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/vidwebmaster.py` & `zcmds-1.4.9/src/zcmds/cmds/common/vidwebmaster.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from zcmds.util.say import say
 
 
 @dataclass
 class VidInfo:
     vidbitrate: str
     height: int
-    fast_start: bool
     filetype: str = "mp4"
 
 
 def get_encoder(filetype: str) -> str:
     if filetype == "mp4":
         return "libx264"
     if filetype == "webm":
@@ -44,26 +43,25 @@
             encoder = get_encoder(vidinfo.filetype)
             bitrate_str = vidbitrate.replace(".", "_")
             ext = vidinfo.filetype
             out_path = os.path.join(path, f"{height}_{bitrate_str}.{ext}")
             downmix_stmt = "-ac 1" if height <= 480 else ""
             # trunc(oh*...) fixes issue with libx264 encoder not liking an add number of width pixels.
             null_stm: str = "/dev/null" if platform.system() != "Windows" else "NUL"
-            movflags_stmt = "-movflags +faststart" if vidinfo.fast_start else ""
             cmd_1stpass = (
                 f'static_ffmpeg -y -hide_banner -v quiet -stats -i "{videopath}"'
                 f' -vf scale="trunc(oh*a/2)*2:{height}" {downmix_stmt}'
-                f" {movflags_stmt} -preset veryslow -c:v {encoder}"
+                f" -movflags +faststart -preset veryslow -c:v {encoder}"
                 f" -an -passlogfile {passlogfile} -pass 1 -f null {null_stm}"
                 f' -b:v {vidbitrate} "{out_path}"'
             )
             cmd_2ndpass = (
                 f'static_ffmpeg -y -hide_banner -v quiet -stats -i "{videopath}"'
                 f' -vf scale="trunc(oh*a/2)*2:{height}" {downmix_stmt}'
-                f" {movflags_stmt} -preset veryslow -c:v {encoder}"
+                f" -movflags +faststart -preset veryslow -c:v {encoder}"
                 f" -passlogfile {passlogfile}"
                 f' -pass 2 -b:v {vidbitrate} "{out_path}"'
             )
             print(f"\nRunning first pass:\n  {cmd_1stpass}\n")
             proc = subprocess.Popen(cmd_1stpass, shell=True)
             proc.wait()
             print(f"\nRunning second pass:\n  {cmd_2ndpass}\n")
@@ -125,21 +123,19 @@
         Thread(target=_encode_then_beep, daemon=True).start()
 
     ui = MainWidget(callback)
     ui.show()
     sys.exit(app.exec())
 
 
-def parse_vidinfos(vidinfos_str: str, fast_start: bool) -> list[VidInfo]:
+def parse_vidinfos(vidinfos_str: str) -> list[VidInfo]:
     vidinfos = []
     for vidinfo_str in vidinfos_str.split(","):
         height, bitrate = vidinfo_str.split(":")
-        vidinfos.append(
-            VidInfo(vidbitrate=bitrate, height=int(height), fast_start=fast_start)
-        )
+        vidinfos.append(VidInfo(vidbitrate=bitrate, height=int(height)))
     # sort so that smallest resolution is first
     vidinfos.sort(key=lambda x: x.height)
     return vidinfos
 
 
 def main():
     # Expects a single argument: the path to the video file to shrink
@@ -152,31 +148,26 @@
     # Adds optional height argument
     parser.add_argument(
         "--encodings",
         help="Height and avg bitrate, seperated by commas. Example: 1080:3.0M,720:1.6M,480:0.9M",
         default="1080:3.0M,720:1.6M,480:0.9M",
     )
     parser.add_argument(
-        "--no-fast-start", help="Add fast start flag", action="store_true"
-    )
-    parser.add_argument(
         "--type", help="mp4 or webm", default="mp4", choices=["mp4", "webm"]
     )
     args = parser.parse_args()
-    fast_start = not args.no_fast_start
-    vidinfos = parse_vidinfos(args.encodings, fast_start=fast_start)
+    vidinfos = parse_vidinfos(args.encodings)
     for vidinfo in vidinfos:
         vidinfo.filetype = args.type
     # sort by smallest first
     if not args.video_path:
-        run_gui(vidinfos=vidinfos)
+        run_gui(vidinfos)
         return
     videopath = args.video_path
     if not os.path.exists(videopath):
         print(f"{videopath} does not exist")
         sys.exit(1)
-
-    encode(videopath=args.video_path, vidinfos=vidinfos)
+    encode(args.video_path, vidinfos)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds/common/whichall.py` & `zcmds-1.4.9/src/zcmds/cmds/common/whichall.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/cmds/darwin/test_net_connection.py` & `zcmds-1.4.9/src/zcmds/cmds/darwin/test_net_connection.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-# pylint: skip-file
-
-import shlex
-import subprocess
-import sys
-
-DNS_BACKBONE = "8.8.8.8"
-
-
-def ParsePingOutput(line):
-    time_ms = "".join(shlex.split(line)[6:7])[5:]
-    if time_ms:
-        return str(int(float(time_ms) + 0.5))
-    else:
-        return line
-
-
-def RunMultiPing(ip_array):
-    procs = []
-    for ip in ip_array:
-        cmd_str = "ping -n -c 1 -t 1 " + ip
-        p = subprocess.Popen(
-            cmd_str, shell=True, stdout=subprocess.PIPE, universal_newlines=True
-        )
-        procs.append(p)
-    out = []
-    for p in procs:
-        p.stdout.readline()  # Throw away first readline
-        line = p.stdout.readline().rstrip()
-        if line:
-            out.append(ParsePingOutput(line))
-        else:
-            out.append("NET_ERR")
-        p.wait()
-    return out
-
-
-def GetTraceRoute(dest_ip):
-    """Returns a list of routes to 8.8.8.8 in [(name, ip), ...] form."""
-    trace_route = []
-    cmd = "traceroute " + dest_ip
-    try:
-        p = subprocess.Popen(
-            cmd, shell=True, stdout=subprocess.PIPE, universal_newlines=True
-        )
-        for line in iter(p.stdout.readline, ""):
-            if line.startswith("  "):
-                continue
-            line = line.rstrip().replace("* ", "")
-            tokens = shlex.split(line)
-            try:
-                name = tokens[1]
-                ip = tokens[2].replace("(", "").replace(")", "")
-                print(f"found: {name} ({ip})")
-                trace_route.append((name, ip))
-            except IndexError:
-                print(f"Error tokenizing {line}, skipping")
-    finally:
-        p.kill()
-    return trace_route
-
-
-def main():
-    # if os is not linux/darwin
-    #     print("This script is only for Linux and Darwin")
-    if sys.platform not in ("linux", "darwin"):
-        print("This script is only for Linux and Darwin")
-        return
-
-    def IsIpPingable(ip):
-        p = subprocess.Popen(
-            "ping -c 5 -t 1 " + ip,
-            shell=True,
-            stdout=subprocess.PIPE,
-            universal_newlines=True,
-        )
-        for line in iter(p.stdout.readline, ""):
-            if "time=" in line:
-                p.wait()
-                return True
-        print(ip + " is invalid")
-        return False
-
-    trace_route = GetTraceRoute("8.8.8.8")
-    # Filter out ip's that won't ping fast.
-    trace_route = [e for e in trace_route if IsIpPingable(e[1])]
-
-    def MakeDataRow():
-        ips = [e[1] for e in trace_route]
-        times = RunMultiPing(ips)
-        out_str = ""
-        for t in times:
-            out_str += "{0: ^16s} | ".format(t)
-        return out_str
-
-    def MakeHeaderRow():
-        def sizeStr(s, n):
-            if len(s) < n:
-                return s
-            else:
-                s = s[0 : n - 3] + "..."
-                return s
-
-        tmp = []
-        out_str = ""
-        for name, ip in trace_route:
-            tmp.append(ip)
-            out_str += "{0: ^16s} | ".format(sizeStr(name, 16))
-        out_str += "\n"
-        for name, ip in trace_route:
-            tmp.append(ip)
-            out_str += "{0: ^16s} | ".format(ip)
-        return "\n" + out_str + "\n"
-
-    while True:
-        print(MakeHeaderRow())
-        for i in range(0, 50):
-            row = MakeDataRow()
-            print(row)
-
-
-if __name__ == "__main__":
-    try:
-        main()
-    except KeyboardInterrupt:
-        pass
+# pylint: skip-file
+
+import shlex
+import subprocess
+import sys
+
+DNS_BACKBONE = "8.8.8.8"
+
+
+def ParsePingOutput(line):
+    time_ms = "".join(shlex.split(line)[6:7])[5:]
+    if time_ms:
+        return str(int(float(time_ms) + 0.5))
+    else:
+        return line
+
+
+def RunMultiPing(ip_array):
+    procs = []
+    for ip in ip_array:
+        cmd_str = "ping -n -c 1 -t 1 " + ip
+        p = subprocess.Popen(
+            cmd_str, shell=True, stdout=subprocess.PIPE, universal_newlines=True
+        )
+        procs.append(p)
+    out = []
+    for p in procs:
+        p.stdout.readline()  # Throw away first readline
+        line = p.stdout.readline().rstrip()
+        if line:
+            out.append(ParsePingOutput(line))
+        else:
+            out.append("NET_ERR")
+        p.wait()
+    return out
+
+
+def GetTraceRoute(dest_ip):
+    """Returns a list of routes to 8.8.8.8 in [(name, ip), ...] form."""
+    trace_route = []
+    cmd = "traceroute " + dest_ip
+    try:
+        p = subprocess.Popen(
+            cmd, shell=True, stdout=subprocess.PIPE, universal_newlines=True
+        )
+        for line in iter(p.stdout.readline, ""):
+            if line.startswith("  "):
+                continue
+            line = line.rstrip().replace("* ", "")
+            tokens = shlex.split(line)
+            try:
+                name = tokens[1]
+                ip = tokens[2].replace("(", "").replace(")", "")
+                print(f"found: {name} ({ip})")
+                trace_route.append((name, ip))
+            except IndexError:
+                print(f"Error tokenizing {line}, skipping")
+    finally:
+        p.kill()
+    return trace_route
+
+
+def main():
+    # if os is not linux/darwin
+    #     print("This script is only for Linux and Darwin")
+    if sys.platform not in ("linux", "darwin"):
+        print("This script is only for Linux and Darwin")
+        return
+
+    def IsIpPingable(ip):
+        p = subprocess.Popen(
+            "ping -c 5 -t 1 " + ip,
+            shell=True,
+            stdout=subprocess.PIPE,
+            universal_newlines=True,
+        )
+        for line in iter(p.stdout.readline, ""):
+            if "time=" in line:
+                p.wait()
+                return True
+        print(ip + " is invalid")
+        return False
+
+    trace_route = GetTraceRoute("8.8.8.8")
+    # Filter out ip's that won't ping fast.
+    trace_route = [e for e in trace_route if IsIpPingable(e[1])]
+
+    def MakeDataRow():
+        ips = [e[1] for e in trace_route]
+        times = RunMultiPing(ips)
+        out_str = ""
+        for t in times:
+            out_str += "{0: ^16s} | ".format(t)
+        return out_str
+
+    def MakeHeaderRow():
+        def sizeStr(s, n):
+            if len(s) < n:
+                return s
+            else:
+                s = s[0 : n - 3] + "..."
+                return s
+
+        tmp = []
+        out_str = ""
+        for name, ip in trace_route:
+            tmp.append(ip)
+            out_str += "{0: ^16s} | ".format(sizeStr(name, 16))
+        out_str += "\n"
+        for name, ip in trace_route:
+            tmp.append(ip)
+            out_str += "{0: ^16s} | ".format(ip)
+        return "\n" + out_str + "\n"
+
+    while True:
+        print(MakeHeaderRow())
+        for i in range(0, 50):
+            row = MakeDataRow()
+            print(row)
+
+
+if __name__ == "__main__":
+    try:
+        main()
+    except KeyboardInterrupt:
+        pass
```

### Comparing `zcmds-1.4.81/src/zcmds/cmds.txt` & `zcmds-1.4.9/src/zcmds/cmds.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 askai = "zcmds.cmds.common.askai:main"
-aicode = "zcmds.cmds.common.aicode:main"
-imgai = "zcmds.cmds.common.imgai:main"
-img2webp = "zcmds.cmds.common.img2webp:main"
+imgai= "zcmds.cmds.common.imgai:main"
 zcmds = "zcmds.cmds.common.zcmds_main:main"
 audnorm = "zcmds.cmds.common.audnorm:main"
-codeup = "zcmds.cmds.common.codeup:main"
 comports = "zcmds.cmds.common.comports:main"
 diskaudit = "zcmds.cmds.common.diskaudit:main"
 findfiles = "zcmds.cmds.common.findfiles:main"
 gitsummary = "zcmds.cmds.common.gitsummary:main"
 obs_organize = "zcmds.cmds.common.obs_organize:main"
 printenv = "zcmds.cmds.common.printenv:main"
 pdf2png = "zcmds.cmds.common.pdf2png:main"
 pdf2txt = "zcmds.cmds.common.pdf2txt:main"
 search_and_replace = "zcmds.cmds.common.search_and_replace:main"
 search_in_files = "zcmds.cmds.common.search_in_files:main"
 sharedir = "zcmds.cmds.common.sharedir:main"
 stereo2mono = "zcmds.cmds.common.stereo2mono:main"
-gitconfig = "zcmds.cmd.common.gitconfig:main"
 img2vid = "zcmds.cmds.common.img2vid:main"
 vidmute = "zcmds.cmds.common.vidmute:main"
 vidinfo = "zcmds.cmds.common.vidinfo:main"
 vid2gif = "zcmds.cmds.common.vid2gif:main"
 vid2jpg = "zcmds.cmds.common.vid2jpg:main"
 vid2mp3 = "zcmds.cmds.common.vid2mp3:main"
 vid2mp4 = "zcmds.cmds.common.vid2mp4:main"
@@ -36,19 +32,8 @@
 vidhero = "zcmds.cmds.common.vidhero:main"
 vidlist = "zcmds.cmds.common.vidlist:main"
 test_net_connection = "zcmds.cmds.darwin.test_net_connection:main"
 fixinternet = "zcmds.cmds.common.fixinternet:main"
 whichall = "zcmds.cmds.common.whichall:main"
 geninvoice = "zcmds.cmds.common.geninvoice:main"
 say = "zcmds.cmds.common.say:main"
-vidcat = "zcmds.cmds.common.vidcat:main"
-myip = "zcmds.cmds.common.myip:main"
-losslesscut = "zcmds.cmds.common.losslesscut:main"
-archive = "zcmds.cmds.common.archive:main"
-imgshrink = "zcmds.cmds.common.imgshrink:main"
-merge-to = "zcmds.cmds.common.merge_to:main"
-removebackground = "zcmds.cmds.common.removebackground:main"
-trash = "zcmds.cmds.common.trash:main"
-push = "zcmds.cmds.common.push:main"
-pull = "zcmds.cmds.common.pull:main"
-gitconfigure = "zcmds.cmds.common.gitconfig:main"
-new  = "zcmds.cmds.common.new:main"
+vidcat = "zcmds.cmds.common.vidcat:main"
```

### Comparing `zcmds-1.4.81/src/zcmds/install/darwin/darwin_update.py` & `zcmds-1.4.9/src/zcmds/install/darwin/darwin_update.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# pylint: disable=invalid-name
-
-"""
-    Update mechanism for darwin (MacOS)
-"""
-
-import os
-import sys
-
-SELF_DIR = os.path.dirname(__file__)
-
-# No longer generating MacOS commands, we use the console scripts instead.
-
-
-def add_python_key_bindings():
-    """Adds keybindings to make python development work much better."""
-    target_file = os.path.join(
-        os.path.expanduser("~"), "Library", "Keybindings", "DefaultKeyBinding.dict"
-    )
-    if not os.path.exists(target_file):
-        os.makedirs(os.path.dirname(target_file), exist_ok=True)
-        with open(target_file, encoding="utf-8", mode="w") as filed:
-            filed.write("")
-    src_file = os.path.join(SELF_DIR, "macOS_key_bindings.dict")
-    with open(src_file, encoding="utf-8", mode="rt") as fd:
-        src_file_content = fd.read()
-    if not os.path.exists(target_file):
-        with open(target_file, encoding="utf-8", mode="rt") as fd:
-            fd.write(src_file_content)
-            return
-    else:
-        with open(target_file, encoding="utf-8", mode="rt") as fd:
-            target_file_content = fd.read()
-        if target_file_content != src_file_content:
-            sys.stderr.write(f"Please manually merge {src_file} with {target_file}\n")
-
-
-def main():
-    """Main entry point."""
-    # gen_macos_cmds()
-    # add_cmds_to_path()
-    add_python_key_bindings()
-
-
-if __name__ == "__main__":
-    main()
+# pylint: disable=invalid-name
+
+"""
+    Update mechanism for darwin (MacOS)
+"""
+
+import os
+import sys
+
+SELF_DIR = os.path.dirname(__file__)
+
+# No longer generating MacOS commands, we use the console scripts instead.
+
+
+def add_python_key_bindings():
+    """Adds keybindings to make python development work much better."""
+    target_file = os.path.join(
+        os.path.expanduser("~"), "Library", "Keybindings", "DefaultKeyBinding.dict"
+    )
+    if not os.path.exists(target_file):
+        os.makedirs(os.path.dirname(target_file), exist_ok=True)
+        with open(target_file, encoding="utf-8", mode="w") as filed:
+            filed.write("")
+    src_file = os.path.join(SELF_DIR, "macOS_key_bindings.dict")
+    with open(src_file, encoding="utf-8", mode="rt") as fd:
+        src_file_content = fd.read()
+    if not os.path.exists(target_file):
+        with open(target_file, encoding="utf-8", mode="rt") as fd:
+            fd.write(src_file_content)
+            return
+    else:
+        with open(target_file, encoding="utf-8", mode="rt") as fd:
+            target_file_content = fd.read()
+        if target_file_content != src_file_content:
+            sys.stderr.write(f"Please manually merge {src_file} with {target_file}\n")
+
+
+def main():
+    """Main entry point."""
+    # gen_macos_cmds()
+    # add_cmds_to_path()
+    add_python_key_bindings()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `zcmds-1.4.81/src/zcmds/util/config.py` & `zcmds-1.4.9/src/zcmds/util/config.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/util/file_search_and_replacer.py` & `zcmds-1.4.9/src/zcmds/util/file_search_and_replacer.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-"""
-    Module for doing file searching and replacing stuff.
-"""
-
-import os
-
-from . import fileutils
-
-
-def main() -> None:
-    """Main function for search and replace."""
-    args: fileutils.SearchArgs = fileutils.get_search_args(require_replace_args=True)
-    files = []
-
-    for file in fileutils.iter_matching_files(
-        cur_dir=args.cur_dir,
-        file_patterns=args.file_patterns,
-        text_search_string=args.search_string,
-        ignore_errors=args.ignore_errors,
-    ):
-        files.append(file)
-        with open(
-            file, encoding="utf-8"
-        ) as fd:  # pylint: disable=invalid-name,duplicate-code
-            file_data = fd.read()
-        matches = []
-        for i, line in enumerate(file_data.splitlines()):
-            if args.search_string in line:
-                matches.append((i, line))
-
-        print(f"Found {len(matches)} matches in {os.path.abspath(file)}:")
-
-        for match in matches:
-            haystack = match[1].strip()
-            # pos = haystack.find(match)
-            # if len(haystack) > 60:
-            #  haystack = haystack[0:60] + '...'
-            absfile = os.path.abspath(file)
-            # print(f"  {match[0]}: {haystack}")
-            print(f"{absfile}:{match[0]}:\n  {haystack}")
-
-    if "y" == input("Apply replace? (y/n): ").lower():
-        print(f"Replacing now... {len(files)}")
-        for file in files:
-            print(f"Replace in file {file} ")
-            fileutils.replace_in_file(
-                file_path=file,
-                search_text=args.search_string,
-                replace_text=args.replace_string,
-            )
-
-
-if __name__ == "__main__":
-    main()
+"""
+    Module for doing file searching and replacing stuff.
+"""
+
+import os
+
+from . import fileutils
+
+
+def main() -> None:
+    """Main function for search and replace."""
+    args: fileutils.SearchArgs = fileutils.get_search_args(require_replace_args=True)
+    files = []
+
+    for file in fileutils.iter_matching_files(
+        cur_dir=args.cur_dir,
+        file_patterns=args.file_patterns,
+        text_search_string=args.search_string,
+        ignore_errors=args.ignore_errors,
+    ):
+        files.append(file)
+        with open(
+            file, encoding="utf-8"
+        ) as fd:  # pylint: disable=invalid-name,duplicate-code
+            file_data = fd.read()
+        matches = []
+        for i, line in enumerate(file_data.splitlines()):
+            if args.search_string in line:
+                matches.append((i, line))
+
+        print(f"Found {len(matches)} matches in {os.path.abspath(file)}:")
+
+        for match in matches:
+            haystack = match[1].strip()
+            # pos = haystack.find(match)
+            # if len(haystack) > 60:
+            #  haystack = haystack[0:60] + '...'
+            absfile = os.path.abspath(file)
+            # print(f"  {match[0]}: {haystack}")
+            print(f"{absfile}:{match[0]}:\n  {haystack}")
+
+    if "y" == input("Apply replace? (y/n): ").lower():
+        print(f"Replacing now... {len(files)}")
+        for file in files:
+            print(f"Replace in file {file} ")
+            fileutils.replace_in_file(
+                file_path=file,
+                search_text=args.search_string,
+                replace_text=args.replace_string,
+            )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `zcmds-1.4.81/src/zcmds/util/file_searcher.py` & `zcmds-1.4.9/src/zcmds/util/file_searcher.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# pylint: skip-file
-"""
-    Module for doing file searching stuff.
-"""
-import os
-
-from . import fileutils
-
-
-def main() -> None:
-    """Main program"""
-    args: fileutils.SearchArgs = fileutils.get_search_args()
-    for file in fileutils.iter_matching_files(
-        cur_dir=args.cur_dir,
-        file_patterns=args.file_patterns,
-        text_search_string=args.search_string,
-        ignore_errors=args.ignore_errors,
-    ):
-        with open(file, encoding="utf-8") as fd:
-            file_data = fd.read()
-        matches = []
-        for i, line in enumerate(file_data.splitlines()):
-            if args.search_string in line:
-                matches.append((i, line))
-        if len(matches):
-            # print(f"Found {len(matches)} matches in {os.path.abspath(file)}:")
-            for match in matches:
-                haystack = match[1].strip()
-                absfile = os.path.abspath(file)
-                print(f"{absfile}:{match[0]}:\n  {haystack}")
-            print()
-
-
-if __name__ == "__main__":
-    main()
+# pylint: skip-file
+"""
+    Module for doing file searching stuff.
+"""
+import os
+
+from . import fileutils
+
+
+def main() -> None:
+    """Main program"""
+    args: fileutils.SearchArgs = fileutils.get_search_args()
+    for file in fileutils.iter_matching_files(
+        cur_dir=args.cur_dir,
+        file_patterns=args.file_patterns,
+        text_search_string=args.search_string,
+        ignore_errors=args.ignore_errors,
+    ):
+        with open(file, encoding="utf-8") as fd:
+            file_data = fd.read()
+        matches = []
+        for i, line in enumerate(file_data.splitlines()):
+            if args.search_string in line:
+                matches.append((i, line))
+        if len(matches):
+            # print(f"Found {len(matches)} matches in {os.path.abspath(file)}:")
+            for match in matches:
+                haystack = match[1].strip()
+                absfile = os.path.abspath(file)
+                print(f"{absfile}:{match[0]}:\n  {haystack}")
+            print()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `zcmds-1.4.81/src/zcmds/util/fileutils.py` & `zcmds-1.4.9/src/zcmds/util/fileutils.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds/util/say.py` & `zcmds-1.4.9/src/zcmds/util/say.py`

 * *Files identical despite different names*

### Comparing `zcmds-1.4.81/src/zcmds.egg-info/SOURCES.txt` & `zcmds-1.4.9/src/zcmds.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,61 @@
-.aiderignore
 .gitignore
 .pylintrc
 LICENSE
 MANIFEST.in
 NOTES.md
 README.md
 activate.sh
-clean
-install
-install.py
-lint
+lint.sh
 make_venv.py
 pyproject.toml
 requirements.testing.txt
 requirements.txt
 setup.py
-test
 tox.ini
 upload_package.sh
 .github/workflows/lint.yml
 .github/workflows/push_macos.yml
 .github/workflows/push_ubuntu.yml
 .github/workflows/push_win.yml
-.vscode/launch.json
 .vscode/settings.json
 src/zcmds/__init__.py
+src/zcmds/cmds.py
 src/zcmds/cmds.txt
-src/zcmds/get_cmds.py
 src/zcmds/version.py
 src/zcmds.egg-info/PKG-INFO
 src/zcmds.egg-info/SOURCES.txt
 src/zcmds.egg-info/dependency_links.txt
 src/zcmds.egg-info/entry_points.txt
 src/zcmds.egg-info/requires.txt
 src/zcmds.egg-info/top_level.txt
 src/zcmds/assets/bell.mp3
 src/zcmds/cmds/__init__.py
 src/zcmds/cmds/common/README.md
 src/zcmds/cmds/common/__init__.py
-src/zcmds/cmds/common/aicode.py
-src/zcmds/cmds/common/archive.py
 src/zcmds/cmds/common/askai.py
 src/zcmds/cmds/common/audnorm.py
-src/zcmds/cmds/common/codeup.py
 src/zcmds/cmds/common/comports.py
 src/zcmds/cmds/common/diskaudit.py
 src/zcmds/cmds/common/findfiles.py
 src/zcmds/cmds/common/fixinternet.py
 src/zcmds/cmds/common/geninvoice.py
-src/zcmds/cmds/common/gitconfig.py
 src/zcmds/cmds/common/gitsummary.py
 src/zcmds/cmds/common/img2vid.py
-src/zcmds/cmds/common/img2webp.py
 src/zcmds/cmds/common/imgai.py
-src/zcmds/cmds/common/imgshrink.py
-src/zcmds/cmds/common/losslesscut.py
-src/zcmds/cmds/common/merge_to.py
-src/zcmds/cmds/common/myip.py
-src/zcmds/cmds/common/new.py
 src/zcmds/cmds/common/obs_organize.py
 src/zcmds/cmds/common/openaicfg.py
 src/zcmds/cmds/common/pdf2png.py
 src/zcmds/cmds/common/pdf2txt.py
 src/zcmds/cmds/common/printenv.py
-src/zcmds/cmds/common/pull.py
-src/zcmds/cmds/common/push.py
-src/zcmds/cmds/common/removebackground.py
 src/zcmds/cmds/common/say.py
 src/zcmds/cmds/common/search_and_replace.py
 src/zcmds/cmds/common/search_in_files.py
 src/zcmds/cmds/common/sharedir.py
 src/zcmds/cmds/common/stereo2mono.py
-src/zcmds/cmds/common/trash.py
-src/zcmds/cmds/common/tsdownloader.py
 src/zcmds/cmds/common/vid2gif.py
 src/zcmds/cmds/common/vid2jpg.py
 src/zcmds/cmds/common/vid2mp3.py
 src/zcmds/cmds/common/vid2mp4.py
 src/zcmds/cmds/common/vid2webm.py
 src/zcmds/cmds/common/vidcat.py
 src/zcmds/cmds/common/vidclip.py
@@ -97,23 +76,18 @@
 src/zcmds/cmds/linux/TODO
 src/zcmds/cmds/linux/__init__.py
 src/zcmds/install/__init__.py
 src/zcmds/install/darwin/__init__.py
 src/zcmds/install/darwin/darwin_update.py
 src/zcmds/install/darwin/macOS_key_bindings.dict
 src/zcmds/util/__init__.py
-src/zcmds/util/_gpt4all.py
-src/zcmds/util/chatgpt.py
 src/zcmds/util/config.py
 src/zcmds/util/file_search_and_replacer.py
 src/zcmds/util/file_searcher.py
 src/zcmds/util/fileutils.py
 src/zcmds/util/index_all_files.py
 src/zcmds/util/prompt_input.py
 src/zcmds/util/say.py
 src/zcmds/util/sound.py
-src/zcmds/util/streaming_console.py
-tests/test_findfiles.py
 tests/test_main.py
 tests/test_sound.py
-tests/test_streaming_console.py
-tests/test_data/rembg.mp4
+tests/test_version.py
```

### Comparing `zcmds-1.4.81/src/zcmds.egg-info/entry_points.txt` & `zcmds-1.4.9/src/zcmds.egg-info/entry_points.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,28 @@
 [console_scripts]
-aicode = zcmds.cmds.common.aicode:main
-archive = zcmds.cmds.common.archive:main
 askai = zcmds.cmds.common.askai:main
 audnorm = zcmds.cmds.common.audnorm:main
-codeup = zcmds.cmds.common.codeup:main
 comports = zcmds.cmds.common.comports:main
 diskaudit = zcmds.cmds.common.diskaudit:main
 findfiles = zcmds.cmds.common.findfiles:main
 fixinternet = zcmds.cmds.common.fixinternet:main
 geninvoice = zcmds.cmds.common.geninvoice:main
-gitconfig = zcmds.cmd.common.gitconfig:main
-gitconfigure = zcmds.cmds.common.gitconfig:main
 gitsummary = zcmds.cmds.common.gitsummary:main
 img2vid = zcmds.cmds.common.img2vid:main
-img2webp = zcmds.cmds.common.img2webp:main
 imgai = zcmds.cmds.common.imgai:main
-imgshrink = zcmds.cmds.common.imgshrink:main
-losslesscut = zcmds.cmds.common.losslesscut:main
-merge-to = zcmds.cmds.common.merge_to:main
-myip = zcmds.cmds.common.myip:main
-new = zcmds.cmds.common.new:main
 obs_organize = zcmds.cmds.common.obs_organize:main
 pdf2png = zcmds.cmds.common.pdf2png:main
 pdf2txt = zcmds.cmds.common.pdf2txt:main
 printenv = zcmds.cmds.common.printenv:main
-pull = zcmds.cmds.common.pull:main
-push = zcmds.cmds.common.push:main
-removebackground = zcmds.cmds.common.removebackground:main
 say = zcmds.cmds.common.say:main
 search_and_replace = zcmds.cmds.common.search_and_replace:main
 search_in_files = zcmds.cmds.common.search_in_files:main
 sharedir = zcmds.cmds.common.sharedir:main
 stereo2mono = zcmds.cmds.common.stereo2mono:main
 test_net_connection = zcmds.cmds.darwin.test_net_connection:main
-trash = zcmds.cmds.common.trash:main
 vid2gif = zcmds.cmds.common.vid2gif:main
 vid2jpg = zcmds.cmds.common.vid2jpg:main
 vid2mp3 = zcmds.cmds.common.vid2mp3:main
 vid2mp4 = zcmds.cmds.common.vid2mp4:main
 vid2webm = zcmds.cmds.common.vid2webm:main
 vidcat = zcmds.cmds.common.vidcat:main
 vidclip = zcmds.cmds.common.vidclip:main
```

### Comparing `zcmds-1.4.81/tests/test_main.py` & `zcmds-1.4.9/tests/test_main.py`

 * *Files identical despite different names*

