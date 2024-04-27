# Comparing `tmp/openav-1.0.0a3.tar.gz` & `tmp/openav-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openav-1.0.0a3.tar", last modified: Mon Apr 22 19:28:43 2024, max compression
+gzip compressed data, was "openav-1.0.0a4.tar", last modified: Sat Apr 27 13:26:16 2024, max compression
```

## Comparing `openav-1.0.0a3.tar` & `openav-1.0.0a4.tar`

### file list

```diff
@@ -1,77 +1,81 @@
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.503719 openav-1.0.0a3/
--rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a3/LICENSE
--rw-r--r--   0 dl         (501) staff       (20)      101 2023-02-26 14:02:17.000000 openav-1.0.0a3/MANIFEST.in
--rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-22 19:28:43.504009 openav-1.0.0a3/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1123 2023-02-26 13:59:14.000000 openav-1.0.0a3/README.md
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.449355 openav-1.0.0a3/openav/
--rw-r--r--   0 dl         (501) staff       (20)     2903 2023-02-26 17:36:46.000000 openav-1.0.0a3/openav/__garbage__.py
--rw-r--r--   0 dl         (501) staff       (20)     1077 2024-04-22 19:28:31.000000 openav-1.0.0a3/openav/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.469220 openav-1.0.0a3/openav/api/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a3/openav/api/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    23628 2024-04-17 13:01:05.000000 openav-1.0.0a3/openav/api/augmentation.py
--rw-r--r--   0 dl         (501) staff       (20)    15668 2024-04-17 13:01:21.000000 openav-1.0.0a3/openav/api/download.py
--rw-r--r--   0 dl         (501) staff       (20)    21146 2024-04-21 20:52:18.000000 openav-1.0.0a3/openav/api/preprocess_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    19817 2024-04-22 19:20:53.000000 openav-1.0.0a3/openav/api/preprocess_video.py
--rw-r--r--   0 dl         (501) staff       (20)    17452 2023-11-01 09:37:48.000000 openav-1.0.0a3/openav/api/test_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    17453 2023-11-01 09:37:48.000000 openav-1.0.0a3/openav/api/test_video.py
--rw-r--r--   0 dl         (501) staff       (20)    12587 2023-10-16 09:10:27.000000 openav-1.0.0a3/openav/api/testing.py
--rw-r--r--   0 dl         (501) staff       (20)    17771 2023-11-01 09:37:48.000000 openav-1.0.0a3/openav/api/train_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    17761 2023-11-01 09:37:48.000000 openav-1.0.0a3/openav/api/train_video.py
--rw-r--r--   0 dl         (501) staff       (20)    23149 2024-04-17 21:11:51.000000 openav-1.0.0a3/openav/api/vad.py
--rw-r--r--   0 dl         (501) staff       (20)     7301 2024-04-17 13:01:45.000000 openav-1.0.0a3/openav/api/vad_gui.py
--rw-r--r--   0 dl         (501) staff       (20)    22993 2024-04-11 17:21:44.000000 openav-1.0.0a3/openav/api/vosk_sr.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.470538 openav-1.0.0a3/openav/modules/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a3/openav/modules/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.477845 openav-1.0.0a3/openav/modules/core/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a3/openav/modules/core/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    30660 2024-04-22 12:20:50.000000 openav-1.0.0a3/openav/modules/core/core.py
--rw-r--r--   0 dl         (501) staff       (20)     3353 2023-10-16 08:55:02.000000 openav-1.0.0a3/openav/modules/core/exceptions.py
--rw-r--r--   0 dl         (501) staff       (20)     9266 2023-03-23 13:47:11.000000 openav-1.0.0a3/openav/modules/core/language.py
--rw-r--r--   0 dl         (501) staff       (20)     9887 2023-03-23 13:47:11.000000 openav-1.0.0a3/openav/modules/core/logging.py
--rw-r--r--   0 dl         (501) staff       (20)     2906 2023-03-23 13:47:11.000000 openav-1.0.0a3/openav/modules/core/messages.py
--rw-r--r--   0 dl         (501) staff       (20)    14550 2024-04-21 20:40:49.000000 openav-1.0.0a3/openav/modules/core/settings.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.479950 openav-1.0.0a3/openav/modules/dataset_recording/
--rw-r--r--   0 dl         (501) staff       (20)        0 2024-04-11 17:37:56.000000 openav-1.0.0a3/openav/modules/dataset_recording/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)     3539 2024-04-11 17:37:56.000000 openav-1.0.0a3/openav/modules/dataset_recording/app.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.488654 openav-1.0.0a3/openav/modules/file_manager/
--rw-r--r--   0 dl         (501) staff       (20)        0 2020-06-10 13:20:15.000000 openav-1.0.0a3/openav/modules/file_manager/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    13911 2023-04-07 08:51:58.000000 openav-1.0.0a3/openav/modules/file_manager/download.py
--rw-r--r--   0 dl         (501) staff       (20)    15231 2023-04-05 13:58:17.000000 openav-1.0.0a3/openav/modules/file_manager/file_manager.py
--rw-r--r--   0 dl         (501) staff       (20)     7272 2023-03-23 13:47:11.000000 openav-1.0.0a3/openav/modules/file_manager/json_manager.py
--rw-r--r--   0 dl         (501) staff       (20)    13451 2023-04-07 13:22:08.000000 openav-1.0.0a3/openav/modules/file_manager/unzip.py
--rw-r--r--   0 dl         (501) staff       (20)     6804 2023-03-23 13:47:11.000000 openav-1.0.0a3/openav/modules/file_manager/yaml_manager.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.495150 openav-1.0.0a3/openav/modules/lab/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a3/openav/modules/lab/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)   120640 2024-04-22 18:12:32.000000 openav-1.0.0a3/openav/modules/lab/audio.py
--rw-r--r--   0 dl         (501) staff       (20)     4351 2023-03-23 13:47:11.000000 openav-1.0.0a3/openav/modules/lab/audiovisual.py
--rw-r--r--   0 dl         (501) staff       (20)     1726 2023-03-23 13:47:11.000000 openav-1.0.0a3/openav/modules/lab/build.py
--rw-r--r--   0 dl         (501) staff       (20)    24163 2024-04-22 19:24:54.000000 openav-1.0.0a3/openav/modules/lab/video.py
--rw-r--r--   0 dl         (501) staff       (20)      215 2024-04-11 17:37:56.000000 openav-1.0.0a3/openav/modules/lab/video_converter.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.444130 openav-1.0.0a3/openav/modules/locales/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.443966 openav-1.0.0a3/openav/modules/locales/en/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.497446 openav-1.0.0a3/openav/modules/locales/en/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 14:16:44.000000 openav-1.0.0a3/openav/modules/locales/en/LC_MESSAGES/argparse.mo
--rw-r--r--   0 dl         (501) staff       (20)      558 2022-12-21 13:56:06.000000 openav-1.0.0a3/openav/modules/locales/en/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.444235 openav-1.0.0a3/openav/modules/locales/ru/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.500164 openav-1.0.0a3/openav/modules/locales/ru/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)     3736 2022-12-21 14:16:59.000000 openav-1.0.0a3/openav/modules/locales/ru/LC_MESSAGES/argparse.mo
--rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 13:56:18.000000 openav-1.0.0a3/openav/modules/locales/ru/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.501023 openav-1.0.0a3/openav/modules/nn/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a3/openav/modules/nn/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.502184 openav-1.0.0a3/openav/modules/trml/
--rw-r--r--   0 dl         (501) staff       (20)        0 2020-05-28 10:15:52.000000 openav-1.0.0a3/openav/modules/trml/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)     2450 2023-03-23 13:47:11.000000 openav-1.0.0a3/openav/modules/trml/shell.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.502931 openav-1.0.0a3/openav/rsrs/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a3/openav/rsrs/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.503453 openav-1.0.0a3/openav/rsrs/favicon/
--rw-r--r--   0 dl         (501) staff       (20)        0 2023-03-23 13:47:11.000000 openav-1.0.0a3/openav/rsrs/favicon/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-22 19:28:43.453234 openav-1.0.0a3/openav.egg-info/
--rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-22 19:28:43.000000 openav-1.0.0a3/openav.egg-info/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1715 2024-04-22 19:28:43.000000 openav-1.0.0a3/openav.egg-info/SOURCES.txt
--rw-r--r--   0 dl         (501) staff       (20)        1 2024-04-22 19:28:43.000000 openav-1.0.0a3/openav.egg-info/dependency_links.txt
--rw-r--r--   0 dl         (501) staff       (20)      210 2024-04-22 19:28:43.000000 openav-1.0.0a3/openav.egg-info/entry_points.txt
--rw-r--r--   0 dl         (501) staff       (20)      392 2024-04-22 19:28:43.000000 openav-1.0.0a3/openav.egg-info/requires.txt
--rw-r--r--   0 dl         (501) staff       (20)        7 2024-04-22 19:28:43.000000 openav-1.0.0a3/openav.egg-info/top_level.txt
--rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 openav-1.0.0a3/pyproject.toml
--rw-r--r--   0 dl         (501) staff       (20)       79 2024-04-22 19:28:43.504849 openav-1.0.0a3/setup.cfg
--rw-r--r--   0 dl         (501) staff       (20)     4306 2024-04-22 19:28:08.000000 openav-1.0.0a3/setup.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.418958 openav-1.0.0a4/
+-rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a4/LICENSE
+-rw-r--r--   0 dl         (501) staff       (20)      101 2023-02-26 14:02:17.000000 openav-1.0.0a4/MANIFEST.in
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 13:26:16.419300 openav-1.0.0a4/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1123 2023-02-26 13:59:14.000000 openav-1.0.0a4/README.md
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.385582 openav-1.0.0a4/openav/
+-rw-r--r--   0 dl         (501) staff       (20)     2903 2023-02-26 17:36:46.000000 openav-1.0.0a4/openav/__garbage__.py
+-rw-r--r--   0 dl         (501) staff       (20)     1077 2024-04-27 13:25:59.000000 openav-1.0.0a4/openav/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.400757 openav-1.0.0a4/openav/api/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a4/openav/api/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    23628 2024-04-17 13:01:05.000000 openav-1.0.0a4/openav/api/augmentation.py
+-rw-r--r--   0 dl         (501) staff       (20)    15668 2024-04-17 13:01:21.000000 openav-1.0.0a4/openav/api/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    21181 2024-04-27 12:48:45.000000 openav-1.0.0a4/openav/api/preprocess_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    19835 2024-04-27 12:48:33.000000 openav-1.0.0a4/openav/api/preprocess_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    17452 2023-11-01 09:37:48.000000 openav-1.0.0a4/openav/api/test_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    17453 2023-11-01 09:37:48.000000 openav-1.0.0a4/openav/api/test_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    12587 2023-10-16 09:10:27.000000 openav-1.0.0a4/openav/api/testing.py
+-rw-r--r--   0 dl         (501) staff       (20)    17771 2023-11-01 09:37:48.000000 openav-1.0.0a4/openav/api/train_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    21500 2024-04-27 13:02:21.000000 openav-1.0.0a4/openav/api/train_audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)    17761 2023-11-01 09:37:48.000000 openav-1.0.0a4/openav/api/train_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    23149 2024-04-17 21:11:51.000000 openav-1.0.0a4/openav/api/vad.py
+-rw-r--r--   0 dl         (501) staff       (20)     7301 2024-04-17 13:01:45.000000 openav-1.0.0a4/openav/api/vad_gui.py
+-rw-r--r--   0 dl         (501) staff       (20)    23001 2024-04-27 12:49:02.000000 openav-1.0.0a4/openav/api/vosk_sr.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.401714 openav-1.0.0a4/openav/modules/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a4/openav/modules/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.405122 openav-1.0.0a4/openav/modules/core/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a4/openav/modules/core/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    31017 2024-04-26 16:59:06.000000 openav-1.0.0a4/openav/modules/core/core.py
+-rw-r--r--   0 dl         (501) staff       (20)     3353 2023-10-16 08:55:02.000000 openav-1.0.0a4/openav/modules/core/exceptions.py
+-rw-r--r--   0 dl         (501) staff       (20)     9266 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/core/language.py
+-rw-r--r--   0 dl         (501) staff       (20)     9887 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/core/logging.py
+-rw-r--r--   0 dl         (501) staff       (20)     2906 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/core/messages.py
+-rw-r--r--   0 dl         (501) staff       (20)    14550 2024-04-21 20:40:49.000000 openav-1.0.0a4/openav/modules/core/settings.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.406481 openav-1.0.0a4/openav/modules/dataset_recording/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2024-04-11 17:37:56.000000 openav-1.0.0a4/openav/modules/dataset_recording/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     4518 2024-04-26 09:47:40.000000 openav-1.0.0a4/openav/modules/dataset_recording/app.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.409920 openav-1.0.0a4/openav/modules/file_manager/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-06-10 13:20:15.000000 openav-1.0.0a4/openav/modules/file_manager/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    13911 2023-04-07 08:51:58.000000 openav-1.0.0a4/openav/modules/file_manager/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    15231 2023-04-05 13:58:17.000000 openav-1.0.0a4/openav/modules/file_manager/file_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)     7272 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/file_manager/json_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)    13451 2023-04-07 13:22:08.000000 openav-1.0.0a4/openav/modules/file_manager/unzip.py
+-rw-r--r--   0 dl         (501) staff       (20)     6804 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/file_manager/yaml_manager.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.413291 openav-1.0.0a4/openav/modules/lab/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a4/openav/modules/lab/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)   120642 2024-04-24 09:54:17.000000 openav-1.0.0a4/openav/modules/lab/audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    23286 2024-04-27 13:24:05.000000 openav-1.0.0a4/openav/modules/lab/audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)     1726 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/lab/build.py
+-rw-r--r--   0 dl         (501) staff       (20)    24427 2024-04-24 13:03:57.000000 openav-1.0.0a4/openav/modules/lab/video.py
+-rw-r--r--   0 dl         (501) staff       (20)      202 2024-04-23 19:00:17.000000 openav-1.0.0a4/openav/modules/lab/video_converter.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.380816 openav-1.0.0a4/openav/modules/locales/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.380630 openav-1.0.0a4/openav/modules/locales/en/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.414483 openav-1.0.0a4/openav/modules/locales/en/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 14:16:44.000000 openav-1.0.0a4/openav/modules/locales/en/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      558 2022-12-21 13:56:06.000000 openav-1.0.0a4/openav/modules/locales/en/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.380935 openav-1.0.0a4/openav/modules/locales/ru/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.415290 openav-1.0.0a4/openav/modules/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)     3736 2022-12-21 14:16:59.000000 openav-1.0.0a4/openav/modules/locales/ru/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 13:56:18.000000 openav-1.0.0a4/openav/modules/locales/ru/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.417018 openav-1.0.0a4/openav/modules/nn/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a4/openav/modules/nn/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    11245 2024-04-26 16:34:46.000000 openav-1.0.0a4/openav/modules/nn/av_dataset.py
+-rw-r--r--   0 dl         (501) staff       (20)    10390 2024-04-27 13:08:42.000000 openav-1.0.0a4/openav/modules/nn/models.py
+-rw-r--r--   0 dl         (501) staff       (20)     2727 2024-04-26 17:11:00.000000 openav-1.0.0a4/openav/modules/nn/utils.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.417702 openav-1.0.0a4/openav/modules/trml/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-05-28 10:15:52.000000 openav-1.0.0a4/openav/modules/trml/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     2450 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/modules/trml/shell.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.418362 openav-1.0.0a4/openav/rsrs/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a4/openav/rsrs/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.418681 openav-1.0.0a4/openav/rsrs/favicon/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2023-03-23 13:47:11.000000 openav-1.0.0a4/openav/rsrs/favicon/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 13:26:16.388143 openav-1.0.0a4/openav.egg-info/
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1834 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/SOURCES.txt
+-rw-r--r--   0 dl         (501) staff       (20)        1 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/dependency_links.txt
+-rw-r--r--   0 dl         (501) staff       (20)      271 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/entry_points.txt
+-rw-r--r--   0 dl         (501) staff       (20)      459 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/requires.txt
+-rw-r--r--   0 dl         (501) staff       (20)        7 2024-04-27 13:26:16.000000 openav-1.0.0a4/openav.egg-info/top_level.txt
+-rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 openav-1.0.0a4/pyproject.toml
+-rw-r--r--   0 dl         (501) staff       (20)       79 2024-04-27 13:26:16.420318 openav-1.0.0a4/setup.cfg
+-rw-r--r--   0 dl         (501) staff       (20)     4489 2024-04-26 16:55:19.000000 openav-1.0.0a4/setup.py
```

### Comparing `openav-1.0.0a3/LICENSE` & `openav-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/PKG-INFO` & `openav-1.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
```

### Comparing `openav-1.0.0a3/README.md` & `openav-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/__garbage__.py` & `openav-1.0.0a4/openav/__garbage__.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/__init__.py` & `openav-1.0.0a4/openav/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 __title__ = "OpenAV"
 __summary__ = "OpenAV"
 __uri__ = "https://github.com/DmitryRyumin/openav"
 
 __version__ = "1.0"
-__release__ = __version__ + ".0-a3"
+__release__ = __version__ + ".0-a4"
 
 __author__ru__ = "Рюмин Дмитрий, Иванько Денис, Шилов Николай, Маркитантов Максим, Карпов Алексей"
 __author__en__ = "Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov"
 __email__ = (
     "dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, " "karpov@iias.spb.su"
 )
```

### Comparing `openav-1.0.0a3/openav/api/augmentation.py` & `openav-1.0.0a4/openav/api/augmentation.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/api/download.py` & `openav-1.0.0a4/openav/api/download.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/api/preprocess_audio.py` & `openav-1.0.0a4/openav/api/preprocess_audio.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # Персональные
 import openav  # Библиотека в целом
 from openav.modules.trml.shell import Shell  # Работа с Shell
 from openav.modules.lab.build import Run  # Сборка библиотеки
 from openav import rsrs  # Ресурсы библиотеки
 
 from openav.modules.core.logging import ARG_PATH_TO_LOGS
-from openav.modules.lab.audio import SAMPLING_RATE_MS, PAD_MODE_MS, DPI, COLOR_GRADIENTS, EXT_AUDIO
+from openav.modules.lab.audio import SAMPLING_RATE_MS, PAD_MODE_MS, DPI, COLOR_GRADIENTS, EXT_AUDIO_L, EXT_AUDIO
 
 
 # ######################################################################################################################
 # Сообщения
 # ######################################################################################################################
 @dataclass
 class MessagesPreprocessAudio(Run):
@@ -196,21 +196,21 @@
                 # Проверка значения
                 if type(val) is not list or len(val) == 0:
                     continue
 
                 # Проход по всем подразделам текущего раздела
                 for v in val:
                     # Проверка значения
-                    if type(v) is not str or not v or (v in EXT_AUDIO) is False:
+                    if type(v) is not str or not v or (v in EXT_AUDIO_L) is False:
                         curr_valid_layer_2 += 100
                         continue
 
                     curr_valid_layer_2 += 1
 
-                if curr_valid_layer_2 <= len(EXT_AUDIO):
+                if curr_valid_layer_2 <= len(EXT_AUDIO_L):
                     curr_valid_layer += 1
 
             # 1. Путь к директории набора данных
             # 2. Путь к директории набора данных состоящего из спектрограмм
             if key == "path_to_dataset" or key == "path_to_dataset_audio":
                 # Проверка значения
                 if type(val) is not str or not val:
@@ -430,13 +430,13 @@
         )
 
         return True
 
 
 def main():
     # Запуск предобработки речевых аудиоданных
-    vad = RunPreprocessAudio(lang="ru", path_to_logs="./openav/logs")
-    vad.run(out=True)
+    preprocess_a = RunPreprocessAudio(lang="ru", path_to_logs="./openav/logs")
+    preprocess_a.run(out=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `openav-1.0.0a3/openav/api/preprocess_video.py` & `openav-1.0.0a4/openav/api/preprocess_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,14 +399,14 @@
             out=out,
         )
 
         return True
 
 
 def main():
-    # Запуск предобработки речевых аудиоданных
-    vad = RunPreprocessVideo(lang="ru", path_to_logs="./openav/logs")
-    vad.run(out=True)
+    # Запуск предобработки речевых видеоданных
+    preprocess_v = RunPreprocessVideo(lang="ru", path_to_logs="./openav/logs")
+    preprocess_v.run(out=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `openav-1.0.0a3/openav/api/test_audio.py` & `openav-1.0.0a4/openav/api/test_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/api/test_video.py` & `openav-1.0.0a4/openav/api/test_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/api/testing.py` & `openav-1.0.0a4/openav/api/testing.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/api/train_audio.py` & `openav-1.0.0a4/openav/api/train_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/api/train_video.py` & `openav-1.0.0a4/openav/api/train_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/api/vad.py` & `openav-1.0.0a4/openav/api/vad.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/api/vad_gui.py` & `openav-1.0.0a4/openav/api/vad_gui.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/api/vosk_sr.py` & `openav-1.0.0a4/openav/api/vosk_sr.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,13 +453,13 @@
         )
 
         return True
 
 
 def main():
     # Запуск детектирования речевой активности в аудиовизуальном сигнале
-    vad = RunVoskSR(lang="ru", path_to_logs="./openav/logs")
-    vad.run(out=True)
+    vosk_sr = RunVoskSR(lang="ru", path_to_logs="./openav/logs")
+    vosk_sr.run(out=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `openav-1.0.0a3/openav/modules/core/core.py` & `openav-1.0.0a4/openav/modules/core/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 import yaml  # Кодирование и декодирование данные в удобном формате
 import pymediainfo  # Получение meta данных из медиафайлов
 import librosa
 import librosa.display
 import matplotlib as mpl
 import mediapipe as mp
 import cv2
+import einops
+import tqdm
+import sklearn
 
 from datetime import datetime  # Работа со временем
 from prettytable import PrettyTable  # Отображение таблиц в терминале
 import pkg_resources  # Работа с ресурсами внутри пакетов
 
 from IPython import get_ipython
 
@@ -656,14 +659,18 @@
                     "Colorama",
                     "Prettytable",
                     "PyYAML",
                     "PyMediaInfo",
                     "Librosa",
                     "MediaPipe",
                     "OpenCV",
+                    "Einops",
+                    "Tqdm",
+                    "Scikit-learn",
+                    "lion-pytorch",
                     "Streamlit",
                     "Vosk",
                 ],
                 "Version": [
                     i.__version__
                     for i in [
                         torch,
@@ -678,17 +685,21 @@
                         colorama,
                         prettytable,
                         yaml,
                         pymediainfo,
                         librosa,
                         mp,
                         cv2,
+                        einops,
+                        tqdm,
+                        sklearn,
                     ]
                 ],
             }
+            pkgs["Version"].append(pkg_resources.get_distribution("lion_pytorch").version)
             pkgs["Version"].append(pkg_resources.get_distribution("streamlit").version)
             pkgs["Version"].append(pkg_resources.get_distribution("vosk").version)
 
             self._df_pkgs = pd.DataFrame(data=pkgs)  # Версии используемых библиотек
             self._df_pkgs.index += 1
 
             if self.is_notebook is False:
```

### Comparing `openav-1.0.0a3/openav/modules/core/exceptions.py` & `openav-1.0.0a4/openav/modules/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/core/language.py` & `openav-1.0.0a4/openav/modules/core/language.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/core/logging.py` & `openav-1.0.0a4/openav/modules/core/logging.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/core/messages.py` & `openav-1.0.0a4/openav/modules/core/messages.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/core/settings.py` & `openav-1.0.0a4/openav/modules/core/settings.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/file_manager/download.py` & `openav-1.0.0a4/openav/modules/file_manager/download.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/file_manager/file_manager.py` & `openav-1.0.0a4/openav/modules/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/file_manager/json_manager.py` & `openav-1.0.0a4/openav/modules/file_manager/json_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/file_manager/unzip.py` & `openav-1.0.0a4/openav/modules/file_manager/unzip.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/file_manager/yaml_manager.py` & `openav-1.0.0a4/openav/modules/file_manager/yaml_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/lab/audio.py` & `openav-1.0.0a4/openav/modules/lab/audio.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 MIN_SPEECH_DURATION_MS_VAD: int = 250  # Минимальная длительность речевого фрагмента в миллисекундах
 # Минимальная длительность тишины в выборках между отдельными речевыми фрагментами
 MIN_SILENCE_DURATION_MS_VAD: int = 50
 SAMPLING_RATE_MS: List[int] = [16000, 22050, 44100, 48000]  # Частота дискретизации
 PAD_MODE_MS: List[int] = ["constant", "reflect", "replicate", "circular"]  # Управление оступами
 DPI: List[int] = [72, 96, 150, 300, 600, 1200]  # DPI
 COLOR_GRADIENTS: List[str] = ["viridis", "plasma", "inferno", "magma", "cividis"]
-EXT_AUDIO: List[str] = ["mov", "mp4", "webm", "wav"]  # Расширения искомых файлов
+EXT_AUDIO_L: List[str] = ["mov", "mp4", "webm", "wav"]  # Расширения искомых файлов
 
 # Количество выборок в каждом окне
 # (512, 1024, 1536 для частоты дискретизации 16000 или 256, 512, 768 для частоты дискретизации 8000)
 WINDOW_SIZE_SAMPLES_VAD: Dict[int, List[int]] = {8000: [256, 512, 768], 16000: [512, 1024, 1536]}
 SPEECH_PAD_MS: int = 150  # Внутренние отступы для итоговых речевых фрагментов
 # Суффиксы каналов аудиофрагментов
 FRONT: Dict[str, List[str]] = {"mono": ["_mono"], "stereo": ["_left", "_right"]}
```

### Comparing `openav-1.0.0a3/openav/modules/lab/build.py` & `openav-1.0.0a4/openav/modules/lab/build.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/lab/video.py` & `openav-1.0.0a4/openav/modules/lab/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,18 @@
     IsNestedCatalogsNotFoundError,
 )
 from openav.modules.file_manager.json_manager import Json  # Класс для работы с Json
 
 sys.stdout = sys.__stdout__
 sys.stderr = sys.__stderr__
 
+# ######################################################################################################################
+# Константы
+# ######################################################################################################################
+
 # Метрики оценки нейросетевой модели
 METRICS_VIDEO: List[str] = [
     "accuracy",
 ]
 DPI: List[int] = [72, 96, 150, 300, 600, 1200]  # DPI
 COLOR_MODE: List[str] = ["gray", "rgb"]  # Цветовая гамма конечного изображения
 RESIZE_RESAMPLE_MODE: List[str] = ["nearest", "bilinear", "lanczos"]  # Фильтры для масштабирования
```

### Comparing `openav-1.0.0a3/openav/modules/locales/en/LC_MESSAGES/base.mo` & `openav-1.0.0a4/openav/modules/locales/en/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/locales/ru/LC_MESSAGES/argparse.mo` & `openav-1.0.0a4/openav/modules/locales/ru/LC_MESSAGES/argparse.mo`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav/modules/trml/shell.py` & `openav-1.0.0a4/openav/modules/trml/shell.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a3/openav.egg-info/PKG-INFO` & `openav-1.0.0a4/openav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
```

### Comparing `openav-1.0.0a3/openav.egg-info/SOURCES.txt` & `openav-1.0.0a4/openav.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 openav/api/download.py
 openav/api/preprocess_audio.py
 openav/api/preprocess_video.py
 openav/api/test_audio.py
 openav/api/test_video.py
 openav/api/testing.py
 openav/api/train_audio.py
+openav/api/train_audiovisual.py
 openav/api/train_video.py
 openav/api/vad.py
 openav/api/vad_gui.py
 openav/api/vosk_sr.py
 openav/modules/__init__.py
 openav/modules/core/__init__.py
 openav/modules/core/core.py
@@ -48,11 +49,14 @@
 openav/modules/lab/video.py
 openav/modules/lab/video_converter.py
 openav/modules/locales/en/LC_MESSAGES/argparse.mo
 openav/modules/locales/en/LC_MESSAGES/base.mo
 openav/modules/locales/ru/LC_MESSAGES/argparse.mo
 openav/modules/locales/ru/LC_MESSAGES/base.mo
 openav/modules/nn/__init__.py
+openav/modules/nn/av_dataset.py
+openav/modules/nn/models.py
+openav/modules/nn/utils.py
 openav/modules/trml/__init__.py
 openav/modules/trml/shell.py
 openav/rsrs/__init__.py
 openav/rsrs/favicon/__init__.py
```

### Comparing `openav-1.0.0a3/setup.py` & `openav-1.0.0a4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     "imgaug >= 0.4.0",
     "flask >= 2.3.3",
     "ffmpeg >= 1.4",
     "librosa >= 0.10.1",
     "matplotlib >= 3.6.3",
     "mediapipe == 0.9.3.0",
     "opencv_contrib_python >= 4.9.0.80",
+    "einops >= 0.7.0",
+    "lion_pytorch >= 0.1.4",
+    "scikit-learn >= 1.4.2",
+    "tqdm >= 4.66.2",
 ]
 
 CLASSIFIERS = """\
 Development Status :: 3 - Alpha
 Natural Language :: Russian
 Natural Language :: English
 Intended Audience :: Developers
@@ -115,14 +119,15 @@
         python_requires=">=3.9, <4",
         entry_points={
             "console_scripts": [
                 "openav_vad = openav.api.vad:main",
                 "openav_vosk_sr = openav.api.vosk_sr:main",
                 "openav_preprocess_audio = openav.api.preprocess_audio:main",
                 "openav_preprocess_video = openav.api.preprocess_video:main",
+                "openav_train_audiovisual = openav.api_train_audiovisual:main",
             ],
         },
         project_urls={
             "Bug Reports": "https://github.com/DmitryRyumin/openav/issues",
             "Documentation": "https://openav.readthedocs.io",
             "Source Code": "https://github.com/DmitryRyumin/openav/tree/main/openav",
             "Download": "https://github.com/DmitryRyumin/openav/tags",
```

