# Comparing `tmp/openav-1.0.0a4.tar.gz` & `tmp/openav-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openav-1.0.0a4.tar", last modified: Sat Apr 27 13:26:16 2024, max compression
+gzip compressed data, was "openav-1.0.0a5.tar", last modified: Sat Apr 27 14:41:54 2024, max compression
```

## Comparing `openav-1.0.0a4.tar` & `openav-1.0.0a5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.418958 openav-1.0.0a4/
--rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a4/LICENSE
--rw-r--r--   0 dl         (501) staff       (20)      101 2023-02-26 14:02:17.000000 openav-1.0.0a4/MANIFEST.in
--rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 13:26:16.419300 openav-1.0.0a4/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1123 2023-02-26 13:59:14.000000 openav-1.0.0a4/README.md
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.385582 openav-1.0.0a4/openav/
--rw-r--r--   0 dl         (501) staff       (20)     2903 2023-02-26 17:36:46.000000 openav-1.0.0a4/openav/__garbage__.py
--rw-r--r--   0 dl         (501) staff       (20)     1077 2024-04-27 13:25:59.000000 openav-1.0.0a4/openav/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.400757 openav-1.0.0a4/openav/api/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a4/openav/api/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    23628 2024-04-17 13:01:05.000000 openav-1.0.0a4/openav/api/augmentation.py
--rw-r--r--   0 dl         (501) staff       (20)    15668 2024-04-17 13:01:21.000000 openav-1.0.0a4/openav/api/download.py
--rw-r--r--   0 dl         (501) staff       (20)    21181 2024-04-27 12:48:45.000000 openav-1.0.0a4/openav/api/preprocess_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    19835 2024-04-27 12:48:33.000000 openav-1.0.0a4/openav/api/preprocess_video.py
--rw-r--r--   0 dl         (501) staff       (20)    17452 2023-11-01 09:37:48.000000 openav-1.0.0a4/openav/api/test_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    17453 2023-11-01 09:37:48.000000 openav-1.0.0a4/openav/api/test_video.py
--rw-r--r--   0 dl         (501) staff       (20)    12587 2023-10-16 09:10:27.000000 openav-1.0.0a4/openav/api/testing.py
--rw-r--r--   0 dl         (501) staff       (20)    17771 2023-11-01 09:37:48.000000 openav-1.0.0a4/openav/api/train_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    21500 2024-04-27 13:02:21.000000 openav-1.0.0a4/openav/api/train_audiovisual.py
--rw-r--r--   0 dl         (501) staff       (20)    17761 2023-11-01 09:37:48.000000 openav-1.0.0a4/openav/api/train_video.py
--rw-r--r--   0 dl         (501) staff       (20)    23149 2024-04-17 21:11:51.000000 openav-1.0.0a4/openav/api/vad.py
--rw-r--r--   0 dl         (501) staff       (20)     7301 2024-04-17 13:01:45.000000 openav-1.0.0a4/openav/api/vad_gui.py
--rw-r--r--   0 dl         (501) staff       (20)    23001 2024-04-27 12:49:02.000000 openav-1.0.0a4/openav/api/vosk_sr.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.401714 openav-1.0.0a4/openav/modules/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a4/openav/modules/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.405122 openav-1.0.0a4/openav/modules/core/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a4/openav/modules/core/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    31017 2024-04-26 16:59:06.000000 openav-1.0.0a4/openav/modules/core/core.py
--rw-r--r--   0 dl         (501) staff       (20)     3353 2023-10-16 08:55:02.000000 openav-1.0.0a4/openav/modules/core/exceptions.py
--rw-r--r--   0 dl         (501) staff       (20)     9266 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/core/language.py
--rw-r--r--   0 dl         (501) staff       (20)     9887 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/core/logging.py
--rw-r--r--   0 dl         (501) staff       (20)     2906 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/core/messages.py
--rw-r--r--   0 dl         (501) staff       (20)    14550 2024-04-21 20:40:49.000000 openav-1.0.0a4/openav/modules/core/settings.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.406481 openav-1.0.0a4/openav/modules/dataset_recording/
--rw-r--r--   0 dl         (501) staff       (20)        0 2024-04-11 17:37:56.000000 openav-1.0.0a4/openav/modules/dataset_recording/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)     4518 2024-04-26 09:47:40.000000 openav-1.0.0a4/openav/modules/dataset_recording/app.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.409920 openav-1.0.0a4/openav/modules/file_manager/
--rw-r--r--   0 dl         (501) staff       (20)        0 2020-06-10 13:20:15.000000 openav-1.0.0a4/openav/modules/file_manager/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    13911 2023-04-07 08:51:58.000000 openav-1.0.0a4/openav/modules/file_manager/download.py
--rw-r--r--   0 dl         (501) staff       (20)    15231 2023-04-05 13:58:17.000000 openav-1.0.0a4/openav/modules/file_manager/file_manager.py
--rw-r--r--   0 dl         (501) staff       (20)     7272 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/file_manager/json_manager.py
--rw-r--r--   0 dl         (501) staff       (20)    13451 2023-04-07 13:22:08.000000 openav-1.0.0a4/openav/modules/file_manager/unzip.py
--rw-r--r--   0 dl         (501) staff       (20)     6804 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/file_manager/yaml_manager.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.413291 openav-1.0.0a4/openav/modules/lab/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a4/openav/modules/lab/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)   120642 2024-04-24 09:54:17.000000 openav-1.0.0a4/openav/modules/lab/audio.py
--rw-r--r--   0 dl         (501) staff       (20)    23286 2024-04-27 13:24:05.000000 openav-1.0.0a4/openav/modules/lab/audiovisual.py
--rw-r--r--   0 dl         (501) staff       (20)     1726 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/lab/build.py
--rw-r--r--   0 dl         (501) staff       (20)    24427 2024-04-24 13:03:57.000000 openav-1.0.0a4/openav/modules/lab/video.py
--rw-r--r--   0 dl         (501) staff       (20)      202 2024-04-23 19:00:17.000000 openav-1.0.0a4/openav/modules/lab/video_converter.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.380816 openav-1.0.0a4/openav/modules/locales/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.380630 openav-1.0.0a4/openav/modules/locales/en/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.414483 openav-1.0.0a4/openav/modules/locales/en/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 14:16:44.000000 openav-1.0.0a4/openav/modules/locales/en/LC_MESSAGES/argparse.mo
--rw-r--r--   0 dl         (501) staff       (20)      558 2022-12-21 13:56:06.000000 openav-1.0.0a4/openav/modules/locales/en/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.380935 openav-1.0.0a4/openav/modules/locales/ru/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.415290 openav-1.0.0a4/openav/modules/locales/ru/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)     3736 2022-12-21 14:16:59.000000 openav-1.0.0a4/openav/modules/locales/ru/LC_MESSAGES/argparse.mo
--rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 13:56:18.000000 openav-1.0.0a4/openav/modules/locales/ru/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.417018 openav-1.0.0a4/openav/modules/nn/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a4/openav/modules/nn/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    11245 2024-04-26 16:34:46.000000 openav-1.0.0a4/openav/modules/nn/av_dataset.py
--rw-r--r--   0 dl         (501) staff       (20)    10390 2024-04-27 13:08:42.000000 openav-1.0.0a4/openav/modules/nn/models.py
--rw-r--r--   0 dl         (501) staff       (20)     2727 2024-04-26 17:11:00.000000 openav-1.0.0a4/openav/modules/nn/utils.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.417702 openav-1.0.0a4/openav/modules/trml/
--rw-r--r--   0 dl         (501) staff       (20)        0 2020-05-28 10:15:52.000000 openav-1.0.0a4/openav/modules/trml/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)     2450 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/trml/shell.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.418362 openav-1.0.0a4/openav/rsrs/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a4/openav/rsrs/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.418681 openav-1.0.0a4/openav/rsrs/favicon/
--rw-r--r--   0 dl         (501) staff       (20)        0 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/rsrs/favicon/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.388143 openav-1.0.0a4/openav.egg-info/
--rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1834 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/SOURCES.txt
--rw-r--r--   0 dl         (501) staff       (20)        1 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/dependency_links.txt
--rw-r--r--   0 dl         (501) staff       (20)      271 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/entry_points.txt
--rw-r--r--   0 dl         (501) staff       (20)      459 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/requires.txt
--rw-r--r--   0 dl         (501) staff       (20)        7 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/top_level.txt
--rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 openav-1.0.0a4/pyproject.toml
--rw-r--r--   0 dl         (501) staff       (20)       79 2024-04-27 13:26:16.420318 openav-1.0.0a4/setup.cfg
--rw-r--r--   0 dl         (501) staff       (20)     4489 2024-04-26 16:55:19.000000 openav-1.0.0a4/setup.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.746554 openav-1.0.0a5/
+-rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a5/LICENSE
+-rw-r--r--   0 dl         (501) staff       (20)      101 2023-02-26 14:02:17.000000 openav-1.0.0a5/MANIFEST.in
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 14:41:54.746965 openav-1.0.0a5/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1123 2023-02-26 13:59:14.000000 openav-1.0.0a5/README.md
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.695815 openav-1.0.0a5/openav/
+-rw-r--r--   0 dl         (501) staff       (20)     2903 2023-02-26 17:36:46.000000 openav-1.0.0a5/openav/__garbage__.py
+-rw-r--r--   0 dl         (501) staff       (20)     1077 2024-04-27 14:34:18.000000 openav-1.0.0a5/openav/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.713590 openav-1.0.0a5/openav/api/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a5/openav/api/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    23628 2024-04-17 13:01:05.000000 openav-1.0.0a5/openav/api/augmentation.py
+-rw-r--r--   0 dl         (501) staff       (20)    15668 2024-04-17 13:01:21.000000 openav-1.0.0a5/openav/api/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    21181 2024-04-27 12:48:45.000000 openav-1.0.0a5/openav/api/preprocess_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    19835 2024-04-27 12:48:33.000000 openav-1.0.0a5/openav/api/preprocess_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    17452 2023-11-01 09:37:48.000000 openav-1.0.0a5/openav/api/test_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    17453 2023-11-01 09:37:48.000000 openav-1.0.0a5/openav/api/test_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    12587 2023-10-16 09:10:27.000000 openav-1.0.0a5/openav/api/testing.py
+-rw-r--r--   0 dl         (501) staff       (20)    17771 2023-11-01 09:37:48.000000 openav-1.0.0a5/openav/api/train_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    21500 2024-04-27 13:02:21.000000 openav-1.0.0a5/openav/api/train_audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)    17761 2023-11-01 09:37:48.000000 openav-1.0.0a5/openav/api/train_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    23149 2024-04-17 21:11:51.000000 openav-1.0.0a5/openav/api/vad.py
+-rw-r--r--   0 dl         (501) staff       (20)     7301 2024-04-17 13:01:45.000000 openav-1.0.0a5/openav/api/vad_gui.py
+-rw-r--r--   0 dl         (501) staff       (20)    23001 2024-04-27 12:49:02.000000 openav-1.0.0a5/openav/api/vosk_sr.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.714482 openav-1.0.0a5/openav/modules/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a5/openav/modules/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.720120 openav-1.0.0a5/openav/modules/core/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a5/openav/modules/core/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    31017 2024-04-26 16:59:06.000000 openav-1.0.0a5/openav/modules/core/core.py
+-rw-r--r--   0 dl         (501) staff       (20)     3353 2023-10-16 08:55:02.000000 openav-1.0.0a5/openav/modules/core/exceptions.py
+-rw-r--r--   0 dl         (501) staff       (20)     9266 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/core/language.py
+-rw-r--r--   0 dl         (501) staff       (20)     9887 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/core/logging.py
+-rw-r--r--   0 dl         (501) staff       (20)     2906 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/core/messages.py
+-rw-r--r--   0 dl         (501) staff       (20)    14550 2024-04-21 20:40:49.000000 openav-1.0.0a5/openav/modules/core/settings.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.721299 openav-1.0.0a5/openav/modules/dataset_recording/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2024-04-11 17:37:56.000000 openav-1.0.0a5/openav/modules/dataset_recording/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     4518 2024-04-26 09:47:40.000000 openav-1.0.0a5/openav/modules/dataset_recording/app.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.725708 openav-1.0.0a5/openav/modules/file_manager/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-06-10 13:20:15.000000 openav-1.0.0a5/openav/modules/file_manager/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    13911 2023-04-07 08:51:58.000000 openav-1.0.0a5/openav/modules/file_manager/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    15231 2023-04-05 13:58:17.000000 openav-1.0.0a5/openav/modules/file_manager/file_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)     7272 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/file_manager/json_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)    13451 2023-04-07 13:22:08.000000 openav-1.0.0a5/openav/modules/file_manager/unzip.py
+-rw-r--r--   0 dl         (501) staff       (20)     6804 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/file_manager/yaml_manager.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.733838 openav-1.0.0a5/openav/modules/lab/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a5/openav/modules/lab/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)   120642 2024-04-24 09:54:17.000000 openav-1.0.0a5/openav/modules/lab/audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    24934 2024-04-27 14:31:18.000000 openav-1.0.0a5/openav/modules/lab/audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)     1726 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/lab/build.py
+-rw-r--r--   0 dl         (501) staff       (20)    24427 2024-04-24 13:03:57.000000 openav-1.0.0a5/openav/modules/lab/video.py
+-rw-r--r--   0 dl         (501) staff       (20)      202 2024-04-23 19:00:17.000000 openav-1.0.0a5/openav/modules/lab/video_converter.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.691086 openav-1.0.0a5/openav/modules/locales/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.690896 openav-1.0.0a5/openav/modules/locales/en/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.735541 openav-1.0.0a5/openav/modules/locales/en/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 14:16:44.000000 openav-1.0.0a5/openav/modules/locales/en/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      558 2022-12-21 13:56:06.000000 openav-1.0.0a5/openav/modules/locales/en/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.691209 openav-1.0.0a5/openav/modules/locales/ru/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.738048 openav-1.0.0a5/openav/modules/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)     3736 2022-12-21 14:16:59.000000 openav-1.0.0a5/openav/modules/locales/ru/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 13:56:18.000000 openav-1.0.0a5/openav/modules/locales/ru/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.742851 openav-1.0.0a5/openav/modules/nn/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a5/openav/modules/nn/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    11245 2024-04-26 16:34:46.000000 openav-1.0.0a5/openav/modules/nn/av_dataset.py
+-rw-r--r--   0 dl         (501) staff       (20)    10390 2024-04-27 13:08:42.000000 openav-1.0.0a5/openav/modules/nn/models.py
+-rw-r--r--   0 dl         (501) staff       (20)     2727 2024-04-26 17:11:00.000000 openav-1.0.0a5/openav/modules/nn/utils.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.745023 openav-1.0.0a5/openav/modules/trml/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-05-28 10:15:52.000000 openav-1.0.0a5/openav/modules/trml/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     2450 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/modules/trml/shell.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.745830 openav-1.0.0a5/openav/rsrs/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a5/openav/rsrs/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.746223 openav-1.0.0a5/openav/rsrs/favicon/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2023-03-23 13:47:11.000000 openav-1.0.0a5/openav/rsrs/favicon/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 14:41:54.698122 openav-1.0.0a5/openav.egg-info/
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1834 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/SOURCES.txt
+-rw-r--r--   0 dl         (501) staff       (20)        1 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/dependency_links.txt
+-rw-r--r--   0 dl         (501) staff       (20)      271 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/entry_points.txt
+-rw-r--r--   0 dl         (501) staff       (20)      459 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/requires.txt
+-rw-r--r--   0 dl         (501) staff       (20)        7 2024-04-27 14:41:54.000000 openav-1.0.0a5/openav.egg-info/top_level.txt
+-rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 openav-1.0.0a5/pyproject.toml
+-rw-r--r--   0 dl         (501) staff       (20)       79 2024-04-27 14:41:54.747915 openav-1.0.0a5/setup.cfg
+-rw-r--r--   0 dl         (501) staff       (20)     4489 2024-04-26 16:55:19.000000 openav-1.0.0a5/setup.py
```

### Comparing `openav-1.0.0a4/LICENSE` & `openav-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/PKG-INFO` & `openav-1.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
```

### Comparing `openav-1.0.0a4/README.md` & `openav-1.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/__garbage__.py` & `openav-1.0.0a5/openav/__garbage__.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/__init__.py` & `openav-1.0.0a5/openav/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 __title__ = "OpenAV"
 __summary__ = "OpenAV"
 __uri__ = "https://github.com/DmitryRyumin/openav"
 
 __version__ = "1.0"
-__release__ = __version__ + ".0-a4"
+__release__ = __version__ + ".0-a5"
 
 __author__ru__ = "Рюмин Дмитрий, Иванько Денис, Шилов Николай, Маркитантов Максим, Карпов Алексей"
 __author__en__ = "Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov"
 __email__ = (
     "dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, " "karpov@iias.spb.su"
 )
```

### Comparing `openav-1.0.0a4/openav/api/augmentation.py` & `openav-1.0.0a5/openav/api/augmentation.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/download.py` & `openav-1.0.0a5/openav/api/download.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/preprocess_audio.py` & `openav-1.0.0a5/openav/api/preprocess_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/preprocess_video.py` & `openav-1.0.0a5/openav/api/preprocess_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/test_audio.py` & `openav-1.0.0a5/openav/api/test_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/test_video.py` & `openav-1.0.0a5/openav/api/test_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/testing.py` & `openav-1.0.0a5/openav/api/testing.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/train_audio.py` & `openav-1.0.0a5/openav/api/train_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/train_audiovisual.py` & `openav-1.0.0a5/openav/api/train_audiovisual.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/train_video.py` & `openav-1.0.0a5/openav/api/train_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/vad.py` & `openav-1.0.0a5/openav/api/vad.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/vad_gui.py` & `openav-1.0.0a5/openav/api/vad_gui.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/api/vosk_sr.py` & `openav-1.0.0a5/openav/api/vosk_sr.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/core/core.py` & `openav-1.0.0a5/openav/modules/core/core.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/core/exceptions.py` & `openav-1.0.0a5/openav/modules/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/core/language.py` & `openav-1.0.0a5/openav/modules/core/language.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/core/logging.py` & `openav-1.0.0a5/openav/modules/core/logging.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/core/messages.py` & `openav-1.0.0a5/openav/modules/core/messages.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/core/settings.py` & `openav-1.0.0a5/openav/modules/core/settings.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/dataset_recording/app.py` & `openav-1.0.0a5/openav/modules/dataset_recording/app.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/file_manager/download.py` & `openav-1.0.0a5/openav/modules/file_manager/download.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/file_manager/file_manager.py` & `openav-1.0.0a5/openav/modules/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/file_manager/json_manager.py` & `openav-1.0.0a5/openav/modules/file_manager/json_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/file_manager/unzip.py` & `openav-1.0.0a5/openav/modules/file_manager/unzip.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/file_manager/yaml_manager.py` & `openav-1.0.0a5/openav/modules/file_manager/yaml_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/lab/audio.py` & `openav-1.0.0a5/openav/modules/lab/audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/lab/audiovisual.py` & `openav-1.0.0a5/openav/modules/lab/audiovisual.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,22 @@
 
         self._sampling_nn_true: str = self._("Обучающая - {} {}, валидационная - {} {}, тестовая - {} {}") + self._em
         self._format_percentage = lambda x: "({}%)".format(x)
 
         self._run_train: str = self._("Запуск процесса обучения") + self._em
         self._epoch: str = self._("Эпоха: {} из {}") + self._em
         self._loss: str = self._("Значения ошибки: обучение - {}, валидация - {}, тест - {}")
+        self._acc_valid_and_test: str = self._("Валидация: точность {} | Тест: точность {}")
+        self._acc_valid_up: str = (
+            self._("Точность на валидационной выборке увеличилась ({} ---> {}). Сохранение модели") + self._em
+        )
+        self._acc_test: str = self._("Точность для тестовой выборке: {}")
+        self._acc_test_up: str = self._("Точность на тестовой выборке увеличилась ({} ---> {})")
+
+        self._end_train: str = self._("Процесс обучения завершен") + self._em
 
 
 # ######################################################################################################################
 # Видео
 # ######################################################################################################################
 @dataclass
 class AV(AVMessages):
@@ -467,36 +475,62 @@
 
                     model.eval()
                     acc, avg_vloss = val_one_epoch(val_dataloader, criterion, model, self.__device)
 
                     model.eval()
                     test_acc, avg_tloss = val_one_epoch(test_dataloader, criterion, model, self.__device)
 
+                    round_f = 6
+
                     self.message_info(
                         self._loss.format(
-                            self.message_line(str(avg_loss)),
-                            self.message_line(str(avg_vloss)),
-                            self.message_line(str(avg_tloss)),
+                            self.message_line(str(round(avg_loss, round_f))),
+                            self.message_line(str(round(avg_vloss, round_f))),
+                            self.message_line(str(round(avg_tloss, round_f))),
                         ),
                         out=out,
                     )
 
                     if max_acc < acc:
                         stop_flag_training = 0
-                        print(f"validation acc: {acc} | test accuracy: {test_acc}")
-                        print(f"Validation Acc Increased ({max_acc:.6f}--->{acc:.6f}) \t Saving The Model")
+
+                        self.message_info(
+                            self._acc_valid_and_test.format(
+                                self.message_line(str(round(acc, round_f))),
+                                self.message_line(str(round(test_acc, round_f))),
+                            ),
+                            out=out,
+                        )
+                        self.message_info(
+                            self._acc_valid_up.format(
+                                self.message_line(str(round(max_acc, round_f))),
+                                self.message_line(str(round(acc, round_f))),
+                            ),
+                            out=out,
+                        )
                         max_acc = acc
-                        torch.save(
-                            model.state_dict(), "{}/e{}_{:.6f}.pth".format(session_path, e, acc)
-                        )  # записываем веса модели
+                        torch.save(model.state_dict(), "{}/e{}_{:.6f}.pth".format(session_path, e, acc))
 
                     if max_test_acc < test_acc:
-                        print(f"test accuracy: {test_acc}")
-                        print(f"Test Acc Increased ({max_test_acc:.6f}--->{test_acc:.6f})")
+                        self.message_info(
+                            self._acc_test.format(
+                                self.message_line(str(round(test_acc, round_f))),
+                            ),
+                            out=out,
+                        )
+                        self.message_info(
+                            self._acc_test_up.format(
+                                self.message_line(str(round(max_test_acc, round_f))),
+                                self.message_line(str(round(test_acc, round_f))),
+                            ),
+                            out=out,
+                        )
+
                         max_test_acc = test_acc
 
                     else:
                         stop_flag_training += 1
 
                     if stop_flag_training > patience:
-                        print("Обучение закончилось")
-                        break
+                        self.message_info(self._end_train, out=out)
+
+                        return True
```

### Comparing `openav-1.0.0a4/openav/modules/lab/build.py` & `openav-1.0.0a5/openav/modules/lab/build.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/lab/video.py` & `openav-1.0.0a5/openav/modules/lab/video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/locales/en/LC_MESSAGES/base.mo` & `openav-1.0.0a5/openav/modules/locales/en/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/locales/ru/LC_MESSAGES/argparse.mo` & `openav-1.0.0a5/openav/modules/locales/ru/LC_MESSAGES/argparse.mo`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/nn/av_dataset.py` & `openav-1.0.0a5/openav/modules/nn/av_dataset.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/nn/models.py` & `openav-1.0.0a5/openav/modules/nn/models.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/nn/utils.py` & `openav-1.0.0a5/openav/modules/nn/utils.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav/modules/trml/shell.py` & `openav-1.0.0a5/openav/modules/trml/shell.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/openav.egg-info/PKG-INFO` & `openav-1.0.0a5/openav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
```

### Comparing `openav-1.0.0a4/openav.egg-info/SOURCES.txt` & `openav-1.0.0a5/openav.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a4/setup.py` & `openav-1.0.0a5/setup.py`

 * *Files identical despite different names*

