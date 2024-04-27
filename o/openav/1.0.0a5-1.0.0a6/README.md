# Comparing `tmp/openav-1.0.0a5.tar.gz` & `tmp/openav-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openav-1.0.0a5.tar", last modified: Sat Apr 27 14:41:54 2024, max compression
+gzip compressed data, was "openav-1.0.0a6.tar", last modified: Sat Apr 27 18:25:49 2024, max compression
```

## Comparing `openav-1.0.0a5.tar` & `openav-1.0.0a6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.746554 openav-1.0.0a5/
--rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a5/LICENSE
--rw-r--r--   0 dl         (501) staff       (20)      101 2023-02-26 14:02:17.000000 openav-1.0.0a5/MANIFEST.in
--rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 14:41:54.746965 openav-1.0.0a5/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1123 2023-02-26 13:59:14.000000 openav-1.0.0a5/README.md
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.695815 openav-1.0.0a5/openav/
--rw-r--r--   0 dl         (501) staff       (20)     2903 2023-02-26 17:36:46.000000 openav-1.0.0a5/openav/__garbage__.py
--rw-r--r--   0 dl         (501) staff       (20)     1077 2024-04-27 14:34:18.000000 openav-1.0.0a5/openav/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.713590 openav-1.0.0a5/openav/api/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a5/openav/api/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    23628 2024-04-17 13:01:05.000000 openav-1.0.0a5/openav/api/augmentation.py
--rw-r--r--   0 dl         (501) staff       (20)    15668 2024-04-17 13:01:21.000000 openav-1.0.0a5/openav/api/download.py
--rw-r--r--   0 dl         (501) staff       (20)    21181 2024-04-27 12:48:45.000000 openav-1.0.0a5/openav/api/preprocess_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    19835 2024-04-27 12:48:33.000000 openav-1.0.0a5/openav/api/preprocess_video.py
--rw-r--r--   0 dl         (501) staff       (20)    17452 2023-11-01 09:37:48.000000 openav-1.0.0a5/openav/api/test_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    17453 2023-11-01 09:37:48.000000 openav-1.0.0a5/openav/api/test_video.py
--rw-r--r--   0 dl         (501) staff       (20)    12587 2023-10-16 09:10:27.000000 openav-1.0.0a5/openav/api/testing.py
--rw-r--r--   0 dl         (501) staff       (20)    17771 2023-11-01 09:37:48.000000 openav-1.0.0a5/openav/api/train_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    21500 2024-04-27 13:02:21.000000 openav-1.0.0a5/openav/api/train_audiovisual.py
--rw-r--r--   0 dl         (501) staff       (20)    17761 2023-11-01 09:37:48.000000 openav-1.0.0a5/openav/api/train_video.py
--rw-r--r--   0 dl         (501) staff       (20)    23149 2024-04-17 21:11:51.000000 openav-1.0.0a5/openav/api/vad.py
--rw-r--r--   0 dl         (501) staff       (20)     7301 2024-04-17 13:01:45.000000 openav-1.0.0a5/openav/api/vad_gui.py
--rw-r--r--   0 dl         (501) staff       (20)    23001 2024-04-27 12:49:02.000000 openav-1.0.0a5/openav/api/vosk_sr.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.714482 openav-1.0.0a5/openav/modules/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a5/openav/modules/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.720120 openav-1.0.0a5/openav/modules/core/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a5/openav/modules/core/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    31017 2024-04-26 16:59:06.000000 openav-1.0.0a5/openav/modules/core/core.py
--rw-r--r--   0 dl         (501) staff       (20)     3353 2023-10-16 08:55:02.000000 openav-1.0.0a5/openav/modules/core/exceptions.py
--rw-r--r--   0 dl         (501) staff       (20)     9266 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/core/language.py
--rw-r--r--   0 dl         (501) staff       (20)     9887 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/core/logging.py
--rw-r--r--   0 dl         (501) staff       (20)     2906 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/core/messages.py
--rw-r--r--   0 dl         (501) staff       (20)    14550 2024-04-21 20:40:49.000000 openav-1.0.0a5/openav/modules/core/settings.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.721299 openav-1.0.0a5/openav/modules/dataset_recording/
--rw-r--r--   0 dl         (501) staff       (20)        0 2024-04-11 17:37:56.000000 openav-1.0.0a5/openav/modules/dataset_recording/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)     4518 2024-04-26 09:47:40.000000 openav-1.0.0a5/openav/modules/dataset_recording/app.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.725708 openav-1.0.0a5/openav/modules/file_manager/
--rw-r--r--   0 dl         (501) staff       (20)        0 2020-06-10 13:20:15.000000 openav-1.0.0a5/openav/modules/file_manager/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    13911 2023-04-07 08:51:58.000000 openav-1.0.0a5/openav/modules/file_manager/download.py
--rw-r--r--   0 dl         (501) staff       (20)    15231 2023-04-05 13:58:17.000000 openav-1.0.0a5/openav/modules/file_manager/file_manager.py
--rw-r--r--   0 dl         (501) staff       (20)     7272 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/file_manager/json_manager.py
--rw-r--r--   0 dl         (501) staff       (20)    13451 2023-04-07 13:22:08.000000 openav-1.0.0a5/openav/modules/file_manager/unzip.py
--rw-r--r--   0 dl         (501) staff       (20)     6804 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/file_manager/yaml_manager.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.733838 openav-1.0.0a5/openav/modules/lab/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a5/openav/modules/lab/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)   120642 2024-04-24 09:54:17.000000 openav-1.0.0a5/openav/modules/lab/audio.py
--rw-r--r--   0 dl         (501) staff       (20)    24934 2024-04-27 14:31:18.000000 openav-1.0.0a5/openav/modules/lab/audiovisual.py
--rw-r--r--   0 dl         (501) staff       (20)     1726 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/lab/build.py
--rw-r--r--   0 dl         (501) staff       (20)    24427 2024-04-24 13:03:57.000000 openav-1.0.0a5/openav/modules/lab/video.py
--rw-r--r--   0 dl         (501) staff       (20)      202 2024-04-23 19:00:17.000000 openav-1.0.0a5/openav/modules/lab/video_converter.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.691086 openav-1.0.0a5/openav/modules/locales/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.690896 openav-1.0.0a5/openav/modules/locales/en/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.735541 openav-1.0.0a5/openav/modules/locales/en/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 14:16:44.000000 openav-1.0.0a5/openav/modules/locales/en/LC_MESSAGES/argparse.mo
--rw-r--r--   0 dl         (501) staff       (20)      558 2022-12-21 13:56:06.000000 openav-1.0.0a5/openav/modules/locales/en/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.691209 openav-1.0.0a5/openav/modules/locales/ru/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.738048 openav-1.0.0a5/openav/modules/locales/ru/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)     3736 2022-12-21 14:16:59.000000 openav-1.0.0a5/openav/modules/locales/ru/LC_MESSAGES/argparse.mo
--rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 13:56:18.000000 openav-1.0.0a5/openav/modules/locales/ru/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.742851 openav-1.0.0a5/openav/modules/nn/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a5/openav/modules/nn/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    11245 2024-04-26 16:34:46.000000 openav-1.0.0a5/openav/modules/nn/av_dataset.py
--rw-r--r--   0 dl         (501) staff       (20)    10390 2024-04-27 13:08:42.000000 openav-1.0.0a5/openav/modules/nn/models.py
--rw-r--r--   0 dl         (501) staff       (20)     2727 2024-04-26 17:11:00.000000 openav-1.0.0a5/openav/modules/nn/utils.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.745023 openav-1.0.0a5/openav/modules/trml/
--rw-r--r--   0 dl         (501) staff       (20)        0 2020-05-28 10:15:52.000000 openav-1.0.0a5/openav/modules/trml/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)     2450 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/trml/shell.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.745830 openav-1.0.0a5/openav/rsrs/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a5/openav/rsrs/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.746223 openav-1.0.0a5/openav/rsrs/favicon/
--rw-r--r--   0 dl         (501) staff       (20)        0 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/rsrs/favicon/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.698122 openav-1.0.0a5/openav.egg-info/
--rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1834 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/SOURCES.txt
--rw-r--r--   0 dl         (501) staff       (20)        1 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/dependency_links.txt
--rw-r--r--   0 dl         (501) staff       (20)      271 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/entry_points.txt
--rw-r--r--   0 dl         (501) staff       (20)      459 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/requires.txt
--rw-r--r--   0 dl         (501) staff       (20)        7 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/top_level.txt
--rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 openav-1.0.0a5/pyproject.toml
--rw-r--r--   0 dl         (501) staff       (20)       79 2024-04-27 14:41:54.747915 openav-1.0.0a5/setup.cfg
--rw-r--r--   0 dl         (501) staff       (20)     4489 2024-04-26 16:55:19.000000 openav-1.0.0a5/setup.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.392135 openav-1.0.0a6/
+-rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a6/LICENSE
+-rw-r--r--   0 dl         (501) staff       (20)      101 2023-02-26 14:02:17.000000 openav-1.0.0a6/MANIFEST.in
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 18:25:49.392816 openav-1.0.0a6/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1123 2023-02-26 13:59:14.000000 openav-1.0.0a6/README.md
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.284140 openav-1.0.0a6/openav/
+-rw-r--r--   0 dl         (501) staff       (20)     2903 2023-02-26 17:36:46.000000 openav-1.0.0a6/openav/__garbage__.py
+-rw-r--r--   0 dl         (501) staff       (20)     1077 2024-04-27 18:25:46.000000 openav-1.0.0a6/openav/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.304405 openav-1.0.0a6/openav/api/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a6/openav/api/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    23628 2024-04-17 13:01:05.000000 openav-1.0.0a6/openav/api/augmentation.py
+-rw-r--r--   0 dl         (501) staff       (20)    15668 2024-04-17 13:01:21.000000 openav-1.0.0a6/openav/api/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    21181 2024-04-27 12:48:45.000000 openav-1.0.0a6/openav/api/preprocess_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    19835 2024-04-27 12:48:33.000000 openav-1.0.0a6/openav/api/preprocess_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    17452 2023-11-01 09:37:48.000000 openav-1.0.0a6/openav/api/test_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    17453 2023-11-01 09:37:48.000000 openav-1.0.0a6/openav/api/test_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    12587 2023-10-16 09:10:27.000000 openav-1.0.0a6/openav/api/testing.py
+-rw-r--r--   0 dl         (501) staff       (20)    17771 2023-11-01 09:37:48.000000 openav-1.0.0a6/openav/api/train_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    21953 2024-04-27 18:16:48.000000 openav-1.0.0a6/openav/api/train_audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)    17761 2023-11-01 09:37:48.000000 openav-1.0.0a6/openav/api/train_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    23149 2024-04-17 21:11:51.000000 openav-1.0.0a6/openav/api/vad.py
+-rw-r--r--   0 dl         (501) staff       (20)     7301 2024-04-17 13:01:45.000000 openav-1.0.0a6/openav/api/vad_gui.py
+-rw-r--r--   0 dl         (501) staff       (20)    23001 2024-04-27 12:49:02.000000 openav-1.0.0a6/openav/api/vosk_sr.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.305420 openav-1.0.0a6/openav/modules/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a6/openav/modules/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.309350 openav-1.0.0a6/openav/modules/core/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a6/openav/modules/core/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    31017 2024-04-26 16:59:06.000000 openav-1.0.0a6/openav/modules/core/core.py
+-rw-r--r--   0 dl         (501) staff       (20)     3353 2023-10-16 08:55:02.000000 openav-1.0.0a6/openav/modules/core/exceptions.py
+-rw-r--r--   0 dl         (501) staff       (20)     9266 2023-03-23 13:47:11.000000 openav-1.0.0a6/openav/modules/core/language.py
+-rw-r--r--   0 dl         (501) staff       (20)     9887 2023-03-23 13:47:11.000000 openav-1.0.0a6/openav/modules/core/logging.py
+-rw-r--r--   0 dl         (501) staff       (20)     2906 2023-03-23 13:47:11.000000 openav-1.0.0a6/openav/modules/core/messages.py
+-rw-r--r--   0 dl         (501) staff       (20)    14550 2024-04-21 20:40:49.000000 openav-1.0.0a6/openav/modules/core/settings.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.311648 openav-1.0.0a6/openav/modules/dataset_recording/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2024-04-11 17:37:56.000000 openav-1.0.0a6/openav/modules/dataset_recording/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     4518 2024-04-26 09:47:40.000000 openav-1.0.0a6/openav/modules/dataset_recording/app.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.320741 openav-1.0.0a6/openav/modules/file_manager/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-06-10 13:20:15.000000 openav-1.0.0a6/openav/modules/file_manager/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    13911 2023-04-07 08:51:58.000000 openav-1.0.0a6/openav/modules/file_manager/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    15231 2023-04-05 13:58:17.000000 openav-1.0.0a6/openav/modules/file_manager/file_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)     7272 2023-03-23 13:47:11.000000 openav-1.0.0a6/openav/modules/file_manager/json_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)    13451 2023-04-07 13:22:08.000000 openav-1.0.0a6/openav/modules/file_manager/unzip.py
+-rw-r--r--   0 dl         (501) staff       (20)     6804 2023-03-23 13:47:11.000000 openav-1.0.0a6/openav/modules/file_manager/yaml_manager.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.344267 openav-1.0.0a6/openav/modules/lab/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a6/openav/modules/lab/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)   120642 2024-04-24 09:54:17.000000 openav-1.0.0a6/openav/modules/lab/audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    25953 2024-04-27 18:24:32.000000 openav-1.0.0a6/openav/modules/lab/audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)     1726 2023-03-23 13:47:11.000000 openav-1.0.0a6/openav/modules/lab/build.py
+-rw-r--r--   0 dl         (501) staff       (20)    24427 2024-04-24 13:03:57.000000 openav-1.0.0a6/openav/modules/lab/video.py
+-rw-r--r--   0 dl         (501) staff       (20)      202 2024-04-23 19:00:17.000000 openav-1.0.0a6/openav/modules/lab/video_converter.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.277786 openav-1.0.0a6/openav/modules/locales/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.277580 openav-1.0.0a6/openav/modules/locales/en/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.348235 openav-1.0.0a6/openav/modules/locales/en/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 14:16:44.000000 openav-1.0.0a6/openav/modules/locales/en/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      558 2022-12-21 13:56:06.000000 openav-1.0.0a6/openav/modules/locales/en/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.277913 openav-1.0.0a6/openav/modules/locales/ru/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.367385 openav-1.0.0a6/openav/modules/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)     3736 2022-12-21 14:16:59.000000 openav-1.0.0a6/openav/modules/locales/ru/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 13:56:18.000000 openav-1.0.0a6/openav/modules/locales/ru/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.388634 openav-1.0.0a6/openav/modules/nn/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a6/openav/modules/nn/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    11245 2024-04-26 16:34:46.000000 openav-1.0.0a6/openav/modules/nn/av_dataset.py
+-rw-r--r--   0 dl         (501) staff       (20)    10390 2024-04-27 13:08:42.000000 openav-1.0.0a6/openav/modules/nn/models.py
+-rw-r--r--   0 dl         (501) staff       (20)     2727 2024-04-26 17:11:00.000000 openav-1.0.0a6/openav/modules/nn/utils.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.390145 openav-1.0.0a6/openav/modules/trml/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-05-28 10:15:52.000000 openav-1.0.0a6/openav/modules/trml/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     2450 2023-03-23 13:47:11.000000 openav-1.0.0a6/openav/modules/trml/shell.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.390984 openav-1.0.0a6/openav/rsrs/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a6/openav/rsrs/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.391625 openav-1.0.0a6/openav/rsrs/favicon/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2023-03-23 13:47:11.000000 openav-1.0.0a6/openav/rsrs/favicon/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 18:25:49.288821 openav-1.0.0a6/openav.egg-info/
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 18:25:49.000000 openav-1.0.0a6/openav.egg-info/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1834 2024-04-27 18:25:49.000000 openav-1.0.0a6/openav.egg-info/SOURCES.txt
+-rw-r--r--   0 dl         (501) staff       (20)        1 2024-04-27 18:25:49.000000 openav-1.0.0a6/openav.egg-info/dependency_links.txt
+-rw-r--r--   0 dl         (501) staff       (20)      271 2024-04-27 18:25:49.000000 openav-1.0.0a6/openav.egg-info/entry_points.txt
+-rw-r--r--   0 dl         (501) staff       (20)      459 2024-04-27 18:25:49.000000 openav-1.0.0a6/openav.egg-info/requires.txt
+-rw-r--r--   0 dl         (501) staff       (20)        7 2024-04-27 18:25:49.000000 openav-1.0.0a6/openav.egg-info/top_level.txt
+-rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 openav-1.0.0a6/pyproject.toml
+-rw-r--r--   0 dl         (501) staff       (20)       79 2024-04-27 18:25:49.393928 openav-1.0.0a6/setup.cfg
+-rw-r--r--   0 dl         (501) staff       (20)     4489 2024-04-26 16:55:19.000000 openav-1.0.0a6/setup.py
```

### Comparing `openav-1.0.0a5/LICENSE` & `openav-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/PKG-INFO` & `openav-1.0.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
```

### Comparing `openav-1.0.0a5/README.md` & `openav-1.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/__garbage__.py` & `openav-1.0.0a6/openav/__garbage__.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/__init__.py` & `openav-1.0.0a6/openav/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 __title__ = "OpenAV"
 __summary__ = "OpenAV"
 __uri__ = "https://github.com/DmitryRyumin/openav"
 
 __version__ = "1.0"
-__release__ = __version__ + ".0-a5"
+__release__ = __version__ + ".0-a6"
 
 __author__ru__ = "Рюмин Дмитрий, Иванько Денис, Шилов Николай, Маркитантов Максим, Карпов Алексей"
 __author__en__ = "Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov"
 __email__ = (
     "dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, " "karpov@iias.spb.su"
 )
```

### Comparing `openav-1.0.0a5/openav/api/augmentation.py` & `openav-1.0.0a6/openav/api/augmentation.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/api/download.py` & `openav-1.0.0a6/openav/api/download.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/api/preprocess_audio.py` & `openav-1.0.0a6/openav/api/preprocess_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/api/preprocess_video.py` & `openav-1.0.0a6/openav/api/preprocess_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/api/test_audio.py` & `openav-1.0.0a6/openav/api/test_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/api/test_video.py` & `openav-1.0.0a6/openav/api/test_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/api/testing.py` & `openav-1.0.0a6/openav/api/testing.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/api/train_audio.py` & `openav-1.0.0a6/openav/api/train_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/api/train_audiovisual.py` & `openav-1.0.0a6/openav/api/train_audiovisual.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # Персональные
 import openav  # Библиотека в целом
 from openav.modules.trml.shell import Shell  # Работа с Shell
 from openav.modules.lab.build import Run  # Сборка библиотеки
 from openav import rsrs  # Ресурсы библиотеки
 
 from openav.modules.core.logging import ARG_PATH_TO_LOGS
-from openav.modules.lab.audiovisual import SUBFOLDERS, SHAPE_AUDIO, SHAPE_VIDEO, EXT_MODELS
+from openav.modules.lab.audiovisual import SUBFOLDERS, SHAPE_AUDIO, SHAPE_VIDEO, EXT_MODELS, OPTIMIZERS
 
 
 # ######################################################################################################################
 # Сообщения
 # ######################################################################################################################
 @dataclass
 class MessagesTrainAudioVisual(Run):
@@ -71,15 +71,15 @@
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
         super().__post_init__()  # Выполнение конструктора из суперкласса
 
-        self._all_layer_in_yaml = 21  # Общее количество настроек в конфигурационном файле
+        self._all_layer_in_yaml = 23  # Общее количество настроек в конфигурационном файле
 
         #  Регистратор логирования с указанным именем
         self._logger_run_train_audiovisual: logging.Logger = logging.getLogger(__class__.__name__)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внутренние методы (защищенные)
     # ------------------------------------------------------------------------------------------------------------------
@@ -243,16 +243,17 @@
             if key == "seed":
                 # Проверка значения
                 if type(val) is not int or not (0 < val):
                     continue
 
                 curr_valid_layer += 1
 
-            # Скорость обучения
-            if key == "leaning_rate":
+            # 1. Скорость обучения
+            # 2. L2 регуляризатор
+            if key == "leaning_rate" or key == "weight_decay":
                 # Проверка значения
                 if type(val) is not float:
                     continue
 
                 curr_valid_layer += 1
 
             # 1. Количество классов
@@ -329,14 +330,22 @@
             if key == "encoder_decoder":
                 # Проверка значения
                 if type(val) is not int or not (1 <= val <= 50):
                     continue
 
                 curr_valid_layer += 1
 
+            # Оптимизатор
+            if key == "optimizer":
+                # Проверка значения
+                if type(val) is not str or (val in OPTIMIZERS) is False:
+                    continue
+
+                curr_valid_layer += 1
+
         # Сравнение общего количества ожидаемых настроек и валидных настроек в конфигурационном файле
         if self._all_layer_in_yaml != curr_valid_layer:
             try:
                 raise TypeError
             except TypeError:
                 self.message_error(self._invalid_file, space=self._space, out=out)
                 return False
@@ -456,14 +465,16 @@
             encoder_decoder=self._args["encoder_decoder"],
             batch_size=self._args["batch_size"],
             max_segment=self._args["max_segment"],
             patience=self._args["patience"],
             epochs=self._args["epochs"],
             seed=self._args["seed"],
             leaning_rate=self._args["leaning_rate"],
+            weight_decay=self._args["weight_decay"],
+            optimizer=self._args["optimizer"],
             hidden_units=self._args["hidden_units"],
             hidden_features=self._args["hidden_features"],
             input_dim=self._args["input_dim"],
             shape_audio=self._args["shape_audio"],
             shape_video=self._args["shape_video"],
             path_to_model_fa=self._args["path_to_model_fa"],
             path_to_model_fv=self._args["path_to_model_fv"],
```

### Comparing `openav-1.0.0a5/openav/api/train_video.py` & `openav-1.0.0a6/openav/api/train_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/api/vad.py` & `openav-1.0.0a6/openav/api/vad.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/api/vad_gui.py` & `openav-1.0.0a6/openav/api/vad_gui.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/api/vosk_sr.py` & `openav-1.0.0a6/openav/api/vosk_sr.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/core/core.py` & `openav-1.0.0a6/openav/modules/core/core.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/core/exceptions.py` & `openav-1.0.0a6/openav/modules/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/core/language.py` & `openav-1.0.0a6/openav/modules/core/language.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/core/logging.py` & `openav-1.0.0a6/openav/modules/core/logging.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/core/messages.py` & `openav-1.0.0a6/openav/modules/core/messages.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/core/settings.py` & `openav-1.0.0a6/openav/modules/core/settings.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/dataset_recording/app.py` & `openav-1.0.0a6/openav/modules/dataset_recording/app.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/file_manager/download.py` & `openav-1.0.0a6/openav/modules/file_manager/download.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/file_manager/file_manager.py` & `openav-1.0.0a6/openav/modules/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/file_manager/json_manager.py` & `openav-1.0.0a6/openav/modules/file_manager/json_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/file_manager/unzip.py` & `openav-1.0.0a6/openav/modules/file_manager/unzip.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/file_manager/yaml_manager.py` & `openav-1.0.0a6/openav/modules/file_manager/yaml_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/lab/audio.py` & `openav-1.0.0a6/openav/modules/lab/audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/lab/audiovisual.py` & `openav-1.0.0a6/openav/modules/lab/audiovisual.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 # ######################################################################################################################
 
 SUBFOLDERS: List[str] = ["train", "val", "test"]
 SHAPE_AUDIO: List[str] = ["channels", "n_mels", "samples"]
 SHAPE_VIDEO: List[str] = ["frames", "channels", "width", "height"]
 EXT_AV_VIDEO: List[str] = ["mov", "mp4", "webm"]  # Расширения искомых файлов
 EXT_MODELS: str = "pt"
+OPTIMIZERS: List[str] = ["adam", "adamw", "sgd", "lion"]
 
 
 # ######################################################################################################################
 # Сообщения
 # ######################################################################################################################
 @dataclass
 class AVMessages(Audio, Video):
@@ -179,14 +180,16 @@
         encoder_decoder: int,
         batch_size: int,
         max_segment: int,
         patience: int,
         epochs: int,
         seed: int,
         leaning_rate: float,
+        weight_decay: float,
+        optimizer: str,
         hidden_units: int,
         hidden_features: int,
         input_dim: int,
         shape_audio: Dict[str, int],
         shape_video: Dict[str, int],
         path_to_model_fa: str,
         path_to_model_fv: str,
@@ -202,14 +205,16 @@
             encoder_decoder (int): Количество энкодеров и декодеров
             batch_size (int): Размер батча
             max_segment (int): Максимальная длительность сегмента видео
             patience (int): Количество неудачных эпох
             epochs (int): Количество эпох
             seed (int): Начальное состояние обучения
             leaning_rate (float): Скорость обучения
+            weight_decay (float): Скорость обучения
+            optimizer (str): Оптимизатор
             hidden_units (int): Количество скрытых нейронов
             hidden_features (int): Количество скрытых признаков
             input_dim (int): Количество входных признаков
             shape_audio (Dict[str, int]): Входная размерность аудио лог-мел спектрограммы
             shape_video (Dict[str, int]): Входная размерность видеокадров
             path_to_model_fa (str): Путь к нейросетевой модели (аудио)
             path_to_model_fv (str): Путь к нейросетевой модели (видео)
@@ -238,15 +243,18 @@
                 or type(max_segment) is not int
                 or not (1 <= max_segment <= 10)
                 or type(epochs) is not int
                 or not (0 <= epochs <= 1000)
                 or type(seed) is not int
                 or not (0 < seed)
                 or type(leaning_rate) is not float
+                or type(weight_decay) is not float
                 or type(hidden_units) is not int
+                or type(optimizer) is not str
+                or (optimizer in OPTIMIZERS) is False
                 or not (0 < hidden_units)
                 or type(hidden_features) is not int
                 or not (0 < hidden_features)
                 or type(patience) is not int
                 or not (0 < patience)
                 or type(input_dim) is not int
                 or not (0 < input_dim)
@@ -271,14 +279,15 @@
                 raise TypeError
         except TypeError:
             self.inv_args(__class__.__name__, self.train_audiovisual.__name__, out=out)
             return False
         else:
             depth = 3
             classes = [cls.lower() for cls in classes]
+            optimizer = optimizer.lower()
 
             shape_audio = (
                 None,
                 max_segment,
                 shape_audio[SHAPE_AUDIO[0]],
                 shape_audio[SHAPE_AUDIO[1]],
                 shape_audio[SHAPE_AUDIO[2]],
@@ -442,15 +451,25 @@
                 model.feature_video.load_state_dict(torch.load(path_to_model_fv))
 
                 for name, param in model.named_parameters():
                     if any(layer_name.split(".")[0] in name for layer_name in ["feature_audio", "feature_video"]):
                         param.requires_grad = False
 
                 criterion = CrossEntropyLoss()
-                optimizer = Lion(model.parameters(), lr=leaning_rate, weight_decay=0)
+
+                if optimizer == OPTIMIZERS[0]:
+                    optimizer = torch.optim.Adam(model.parameters(), lr=leaning_rate, weight_decay=weight_decay)
+                elif optimizer == OPTIMIZERS[1]:
+                    optimizer = torch.optim.AdamW(model.parameters(), lr=leaning_rate, weight_decay=weight_decay)
+                elif optimizer == OPTIMIZERS[2]:
+                    optimizer = torch.optim.SGD(model.parameters(), lr=leaning_rate, weight_decay=weight_decay)
+                elif optimizer == OPTIMIZERS[3]:
+                    optimizer = Lion(model.parameters(), lr=leaning_rate, weight_decay=weight_decay)
+                else:
+                    pass
 
                 max_acc = 0
                 max_test_acc = 0
 
                 date_time = datetime.datetime.now()
                 date_path = date_time.strftime(self.__model_session)
                 session_path = os.path.join(self.path_to_save_models, date_path)
```

### Comparing `openav-1.0.0a5/openav/modules/lab/build.py` & `openav-1.0.0a6/openav/modules/lab/build.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/lab/video.py` & `openav-1.0.0a6/openav/modules/lab/video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/locales/en/LC_MESSAGES/base.mo` & `openav-1.0.0a6/openav/modules/locales/en/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/locales/ru/LC_MESSAGES/argparse.mo` & `openav-1.0.0a6/openav/modules/locales/ru/LC_MESSAGES/argparse.mo`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/nn/av_dataset.py` & `openav-1.0.0a6/openav/modules/nn/av_dataset.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/nn/models.py` & `openav-1.0.0a6/openav/modules/nn/models.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/nn/utils.py` & `openav-1.0.0a6/openav/modules/nn/utils.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav/modules/trml/shell.py` & `openav-1.0.0a6/openav/modules/trml/shell.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/openav.egg-info/PKG-INFO` & `openav-1.0.0a6/openav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
```

### Comparing `openav-1.0.0a5/openav.egg-info/SOURCES.txt` & `openav-1.0.0a6/openav.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a5/setup.py` & `openav-1.0.0a6/setup.py`

 * *Files identical despite different names*

