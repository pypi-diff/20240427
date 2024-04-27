# Comparing `tmp/letmedoit-2.1.84.tar.gz` & `tmp/letmedoit-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letmedoit-2.1.84.tar", last modified: Sat Apr 27 15:32:06 2024, max compression
+gzip compressed data, was "letmedoit-2.1.9.tar", last modified: Mon Jan 29 23:35:49 2024, max compression
```

## Comparing `letmedoit-2.1.84.tar` & `letmedoit-2.1.9.tar`

### file list

```diff
@@ -1,189 +1,163 @@
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.721554 letmedoit-2.1.84/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    23450 2024-04-27 15:32:06.721554 letmedoit-2.1.84/PKG-INFO
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.681554 letmedoit-2.1.84/letmedoit/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    20314 2024-04-27 15:32:06.000000 letmedoit-2.1.84/letmedoit/README.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2023-11-28 12:28:19.000000 letmedoit-2.1.84/letmedoit/__init__.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.681554 letmedoit-2.1.84/letmedoit/audio/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 letmedoit-2.1.84/letmedoit/audio/notification1.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 letmedoit-2.1.84/letmedoit/audio/notification1_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 letmedoit-2.1.84/letmedoit/audio/notification2.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 letmedoit-2.1.84/letmedoit/audio/notification2_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6036 2024-03-04 06:59:14.000000 letmedoit-2.1.84/letmedoit/autoassist.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9757 2024-03-04 06:59:14.000000 letmedoit-2.1.84/letmedoit/autobuilder.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5417 2024-03-04 06:59:14.000000 letmedoit-2.1.84/letmedoit/automath.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9921 2024-03-04 06:59:14.000000 letmedoit-2.1.84/letmedoit/autoretriever.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-03-04 09:29:57.000000 letmedoit-2.1.84/letmedoit/chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7207 2024-03-04 09:29:57.000000 letmedoit-2.1.84/letmedoit/codey.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1021 2024-03-04 06:59:14.000000 letmedoit-2.1.84/letmedoit/commandprompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.000000 letmedoit-2.1.84/letmedoit/config.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 letmedoit-2.1.84/letmedoit/eTextEdit.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.681554 letmedoit-2.1.84/letmedoit/files/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 letmedoit-2.1.84/letmedoit/files/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11836 2024-03-04 09:29:57.000000 letmedoit-2.1.84/letmedoit/geminipro.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-03-04 06:59:14.000000 letmedoit-2.1.84/letmedoit/geminiprovision.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.681554 letmedoit-2.1.84/letmedoit/gui/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9923 2024-03-12 11:05:48.000000 letmedoit-2.1.84/letmedoit/gui/chatgui.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2499 2024-03-08 11:52:20.000000 letmedoit-2.1.84/letmedoit/gui/quicktask.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2153 2024-03-12 10:38:39.000000 letmedoit-2.1.84/letmedoit/gui/worker.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    23454 2024-03-11 22:20:06.000000 letmedoit-2.1.84/letmedoit/health_check.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.685554 letmedoit-2.1.84/letmedoit/history/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 letmedoit-2.1.84/letmedoit/history/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.701554 letmedoit-2.1.84/letmedoit/icons/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2745 2023-12-01 18:33:14.000000 letmedoit-2.1.84/letmedoit/icons/CyberTask.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   822229 2023-12-01 14:16:21.000000 letmedoit-2.1.84/letmedoit/icons/CyberTask.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   142154 2023-12-23 12:00:17.000000 letmedoit-2.1.84/letmedoit/icons/GeminiPro.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   922938 2023-12-23 12:00:17.000000 letmedoit-2.1.84/letmedoit/icons/GeminiPro.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   180039 2023-11-28 12:28:19.000000 letmedoit-2.1.84/letmedoit/icons/LetMeDoIt.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  1751831 2023-11-28 12:28:19.000000 letmedoit-2.1.84/letmedoit/icons/LetMeDoIt.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   163394 2023-11-28 12:28:19.000000 letmedoit-2.1.84/letmedoit/icons/MyHand.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  1285185 2023-11-28 12:28:19.000000 letmedoit-2.1.84/letmedoit/icons/MyHand.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   192498 2023-11-28 12:28:19.000000 letmedoit-2.1.84/letmedoit/icons/TaskWiz.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  1588126 2023-11-28 11:23:47.000000 letmedoit-2.1.84/letmedoit/icons/TaskWiz.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   163928 2024-01-06 20:58:34.000000 letmedoit-2.1.84/letmedoit/icons/systemtray.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   833737 2024-01-06 20:58:34.000000 letmedoit-2.1.84/letmedoit/icons/systemtray.png
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.677554 letmedoit-2.1.84/letmedoit/macOS_service/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.673554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Download_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.701554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.701554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5677 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.673554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.705554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      646 2023-12-07 18:59:13.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.705554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5676 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.673554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Files_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.705554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      634 2023-12-01 10:53:39.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.705554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.677554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.705554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      648 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.705554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5678 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.677554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.705554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      642 2023-12-07 18:59:13.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.705554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5678 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.677554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Text_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.705554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      639 2023-12-01 10:53:44.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.705554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5653 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.677554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.709554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      646 2023-12-07 18:59:13.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.709554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5678 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.677554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.709554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      646 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.709554 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5689 2023-12-09 18:05:15.000000 letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/document.wflow
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10459 2024-03-04 10:36:59.000000 letmedoit-2.1.84/letmedoit/main.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10990 2024-03-04 09:29:57.000000 letmedoit-2.1.84/letmedoit/ollamachat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        9 2024-04-27 15:32:06.000000 letmedoit-2.1.84/letmedoit/package_name.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7741 2024-03-04 09:29:57.000000 letmedoit-2.1.84/letmedoit/palm2.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.717554 letmedoit-2.1.84/letmedoit/plugins/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1406 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/000_check_ffmpeg.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1668 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/000_check_pyaudio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1545 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/000_check_vlc.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 letmedoit-2.1.84/letmedoit/plugins/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6751 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/add calendar event.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3335 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/aliases.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2561 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/analyze audio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2223 2024-03-14 11:36:48.000000 letmedoit-2.1.84/letmedoit/plugins/analyze files.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1492 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/analyze images with gemini.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2768 2024-03-12 10:07:25.000000 letmedoit-2.1.84/letmedoit/plugins/analyze images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2101 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/analyze web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1025 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/ask chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      963 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/ask codey.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1007 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/ask gemini pro.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      950 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/ask gemma.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      953 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/ask llama2.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      940 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/ask llava.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      958 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/ask mistral.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2497 2024-03-04 09:29:57.000000 letmedoit-2.1.84/letmedoit/plugins/ask ollama.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      955 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/ask palm2.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2473 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/auto heal python code.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1858 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/awesome prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5874 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/character analysis.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      787 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/contexts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7218 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/counselling.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1613 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/create ai assistants.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2913 2024-03-12 10:02:19.000000 letmedoit-2.1.84/letmedoit/plugins/create images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1192 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/create maps.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1362 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/create qrcode.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1461 2024-03-14 14:25:18.000000 letmedoit-2.1.84/letmedoit/plugins/create statistical graphics.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1026 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/dates and times.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4111 2024-03-04 09:29:57.000000 letmedoit-2.1.84/letmedoit/plugins/download youtube or web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2004 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/edit text.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3836 2024-03-03 21:17:11.000000 letmedoit-2.1.84/letmedoit/plugins/execute python code.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4359 2024-03-03 21:26:13.000000 letmedoit-2.1.84/letmedoit/plugins/execute termux command.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6938 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/global finance.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      973 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/improve British English.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1332 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/input suggestions.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1120 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/install python package.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1658 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/integrate google searches.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1099 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/manipulate files.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5595 2024-03-14 17:15:07.000000 letmedoit-2.1.84/letmedoit/plugins/memory.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5445 2024-03-12 09:57:39.000000 letmedoit-2.1.84/letmedoit/plugins/modify images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1068 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/open web browser.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1337 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/pronounce words.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2424 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/remove image background.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6279 2024-03-04 09:29:57.000000 letmedoit-2.1.84/letmedoit/plugins/search chat records.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1228 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/search financial data.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2011 2024-03-14 17:31:59.000000 letmedoit-2.1.84/letmedoit/plugins/search latest news.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3670 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/search sqlite.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1798 2024-03-13 13:55:29.000000 letmedoit-2.1.84/letmedoit/plugins/search weather info.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4084 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/send email.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1035 2024-03-03 16:10:41.000000 letmedoit-2.1.84/letmedoit/plugins/send tweet.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1388 2024-03-02 08:24:08.000000 letmedoit-2.1.84/letmedoit/plugins/send whatsapp messages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      531 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/plugins/simplified Chinese to traditional Chinese.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1033 2024-03-30 21:38:40.000000 letmedoit-2.1.84/letmedoit/plugins/solve math problems.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1429 2024-03-12 09:31:15.000000 letmedoit-2.1.84/letmedoit/qt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-04-27 15:31:13.000000 letmedoit-2.1.84/letmedoit/requirements.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6401 2024-03-12 11:53:33.000000 letmedoit-2.1.84/letmedoit/systemtray.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.717554 letmedoit-2.1.84/letmedoit/temp/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 letmedoit-2.1.84/letmedoit/temp/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.717554 letmedoit-2.1.84/letmedoit/utils/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    91019 2024-03-12 11:42:04.000000 letmedoit-2.1.84/letmedoit/utils/assistant.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11120 2024-03-12 11:44:48.000000 letmedoit-2.1.84/letmedoit/utils/config_essential.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3622 2024-03-04 10:01:50.000000 letmedoit-2.1.84/letmedoit/utils/config_tools.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      373 2024-01-07 00:10:34.000000 letmedoit-2.1.84/letmedoit/utils/file_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    14372 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/utils/get_path_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2246 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/utils/install.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3351 2024-03-06 22:12:07.000000 letmedoit-2.1.84/letmedoit/utils/ollama_models.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3922 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/utils/promptValidator.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7030 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/utils/prompt_multiline_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7923 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/utils/prompt_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21667 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/utils/prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    47612 2024-03-19 12:19:17.000000 letmedoit-2.1.84/letmedoit/utils/shared_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21333 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/utils/shortcuts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7885 2024-02-25 21:16:23.000000 letmedoit-2.1.84/letmedoit/utils/streaming_word_wrapper.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 letmedoit-2.1.84/letmedoit/utils/sttLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6034 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/utils/terminal_mode_dialogs.py
--rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9965 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/utils/terminal_system_command_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    23916 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/utils/text_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 letmedoit-2.1.84/letmedoit/utils/ttsLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8471 2024-02-25 20:32:06.000000 letmedoit-2.1.84/letmedoit/utils/tts_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4702 2024-02-24 17:48:40.000000 letmedoit-2.1.84/letmedoit/utils/vlc_utils.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:32:06.721554 letmedoit-2.1.84/letmedoit.egg-info/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    23450 2024-04-27 15:32:06.000000 letmedoit-2.1.84/letmedoit.egg-info/PKG-INFO
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6064 2024-04-27 15:32:06.000000 letmedoit-2.1.84/letmedoit.egg-info/SOURCES.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-27 15:32:06.000000 letmedoit-2.1.84/letmedoit.egg-info/dependency_links.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1088 2024-04-27 15:32:06.000000 letmedoit-2.1.84/letmedoit.egg-info/entry_points.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-04-27 15:32:06.000000 letmedoit-2.1.84/letmedoit.egg-info/requires.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-27 15:32:06.000000 letmedoit-2.1.84/letmedoit.egg-info/top_level.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-27 15:32:06.721554 letmedoit-2.1.84/setup.cfg
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9718 2024-04-27 15:31:30.000000 letmedoit-2.1.84/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.311887 letmedoit-2.1.9/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    20115 2024-01-29 23:35:49.311887 letmedoit-2.1.9/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.279885 letmedoit-2.1.9/letmedoit/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18731 2024-01-29 23:35:49.000000 letmedoit-2.1.9/letmedoit/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2023-11-28 12:28:19.000000 letmedoit-2.1.9/letmedoit/__init__.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5450 2024-01-29 23:33:01.000000 letmedoit-2.1.9/letmedoit/autoassist.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9386 2024-01-29 23:33:01.000000 letmedoit-2.1.9/letmedoit/autobuilder.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4784 2024-01-29 23:33:01.000000 letmedoit-2.1.9/letmedoit/automath.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9358 2024-01-29 23:33:05.000000 letmedoit-2.1.9/letmedoit/autoretriever.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7081 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7248 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/codey.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1043 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/commandprompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.000000 letmedoit-2.1.9/letmedoit/config.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 letmedoit-2.1.9/letmedoit/eTextEdit.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.283885 letmedoit-2.1.9/letmedoit/files/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 letmedoit-2.1.9/letmedoit/files/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10627 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/geminipro.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9407 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/geminiprovision.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    16623 2024-01-29 23:26:25.000000 letmedoit-2.1.9/letmedoit/health_check.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.283885 letmedoit-2.1.9/letmedoit/history/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 letmedoit-2.1.9/letmedoit/history/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.299886 letmedoit-2.1.9/letmedoit/icons/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2745 2023-12-01 18:33:14.000000 letmedoit-2.1.9/letmedoit/icons/CyberTask.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   822229 2023-12-01 14:16:21.000000 letmedoit-2.1.9/letmedoit/icons/CyberTask.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   142154 2023-12-23 12:00:17.000000 letmedoit-2.1.9/letmedoit/icons/GeminiPro.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   922938 2023-12-23 12:00:17.000000 letmedoit-2.1.9/letmedoit/icons/GeminiPro.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   180039 2023-11-28 12:28:19.000000 letmedoit-2.1.9/letmedoit/icons/LetMeDoIt.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  1751831 2023-11-28 12:28:19.000000 letmedoit-2.1.9/letmedoit/icons/LetMeDoIt.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   163394 2023-11-28 12:28:19.000000 letmedoit-2.1.9/letmedoit/icons/MyHand.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  1285185 2023-11-28 12:28:19.000000 letmedoit-2.1.9/letmedoit/icons/MyHand.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   192498 2023-11-28 12:28:19.000000 letmedoit-2.1.9/letmedoit/icons/TaskWiz.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  1588126 2023-11-28 11:23:47.000000 letmedoit-2.1.9/letmedoit/icons/TaskWiz.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   163928 2024-01-06 20:58:34.000000 letmedoit-2.1.9/letmedoit/icons/systemtray.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   833737 2024-01-06 20:58:34.000000 letmedoit-2.1.9/letmedoit/icons/systemtray.png
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.279885 letmedoit-2.1.9/letmedoit/macOS_service/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.275884 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Download_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.299886 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.299886 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5677 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.275884 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.299886 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      646 2023-12-07 18:59:13.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.299886 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5676 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.275884 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Files_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.299886 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      634 2023-12-01 10:53:39.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.299886 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.279885 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.299886 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      648 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.299886 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5678 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.279885 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.299886 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      642 2023-12-07 18:59:13.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.299886 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5678 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.279885 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Text_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.303887 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      639 2023-12-01 10:53:44.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.303887 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5653 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.279885 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.303887 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      646 2023-12-07 18:59:13.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.303887 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5678 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.279885 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.303887 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      646 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.303887 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5689 2023-12-09 18:05:15.000000 letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/document.wflow
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14390 2024-01-24 22:21:31.000000 letmedoit-2.1.9/letmedoit/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        9 2024-01-29 23:35:49.000000 letmedoit-2.1.9/letmedoit/package_name.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7785 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/palm2.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.307887 letmedoit-2.1.9/letmedoit/plugins/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 letmedoit-2.1.9/letmedoit/plugins/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6711 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/add calendar event.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1961 2024-01-24 22:21:31.000000 letmedoit-2.1.9/letmedoit/plugins/aliases.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2231 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/analyze files.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-01-29 23:27:43.000000 letmedoit-2.1.9/letmedoit/plugins/analyze images with gemini.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4966 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/analyze images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2066 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/analyze web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1031 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/ask chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      967 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/ask codey.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1020 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/ask gemini pro.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      960 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/ask palm2.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3576 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/ask sqlite.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2532 2024-01-24 22:21:31.000000 letmedoit-2.1.9/letmedoit/plugins/auto heal python code.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1858 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/awesome prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5874 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/character analysis.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      787 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/contexts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7218 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/counselling.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1535 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/create ai assistants.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5061 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/create images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1200 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/create maps.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1372 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/create qrcode.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1446 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/create statistical graphics.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      928 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/dates and times.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4006 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/download youtube or web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2011 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/edit text.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6938 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/global finance.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      973 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/improve British English.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1332 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/input suggestions.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1137 2024-01-24 22:21:31.000000 letmedoit-2.1.9/letmedoit/plugins/install python package.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1735 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/integrate google searches.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1120 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/manipulate files.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5210 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/memory.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9673 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/modify images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      989 2024-01-24 22:21:31.000000 letmedoit-2.1.9/letmedoit/plugins/open web browser.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1353 2024-01-24 22:21:31.000000 letmedoit-2.1.9/letmedoit/plugins/pronounce words.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2449 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/remove image background.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6174 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/search chat records.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1213 2024-01-24 22:21:31.000000 letmedoit-2.1.9/letmedoit/plugins/search financial data.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2312 2024-01-24 22:21:31.000000 letmedoit-2.1.9/letmedoit/plugins/search latest news.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1737 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/search weather info.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4038 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/send email.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1345 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/send whatsapp messages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      532 2024-01-24 22:21:31.000000 letmedoit-2.1.9/letmedoit/plugins/simplified Chinese to traditional Chinese.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1035 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/plugins/solve math problems.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      465 2024-01-24 22:21:31.000000 letmedoit-2.1.9/letmedoit/requirements.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3992 2024-01-24 22:21:31.000000 letmedoit-2.1.9/letmedoit/systemtray.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.307887 letmedoit-2.1.9/letmedoit/temp/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 letmedoit-2.1.9/letmedoit/temp/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.311887 letmedoit-2.1.9/letmedoit/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    97642 2024-01-29 23:30:30.000000 letmedoit-2.1.9/letmedoit/utils/assistant.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8025 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/configDefault.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      373 2024-01-07 00:10:34.000000 letmedoit-2.1.9/letmedoit/utils/file_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14482 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/get_path_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2246 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/install.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3995 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/promptValidator.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7030 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/prompt_multiline_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7760 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/prompt_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14935 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    28788 2024-01-29 23:31:39.000000 letmedoit-2.1.9/letmedoit/utils/shared_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21333 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/shortcuts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7607 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/streaming_word_wrapper.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6034 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/terminal_mode_dialogs.py
+-rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9510 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/terminal_system_command_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    23916 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/text_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    26940 2023-11-28 12:28:19.000000 letmedoit-2.1.9/letmedoit/utils/ttsLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7693 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/tts_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4702 2024-01-22 11:51:15.000000 letmedoit-2.1.9/letmedoit/utils/vlc_utils.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-01-29 23:35:49.283885 letmedoit-2.1.9/letmedoit.egg-info/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    20115 2024-01-29 23:35:49.000000 letmedoit-2.1.9/letmedoit.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5276 2024-01-29 23:35:49.000000 letmedoit-2.1.9/letmedoit.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-01-29 23:35:49.000000 letmedoit-2.1.9/letmedoit.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      512 2024-01-29 23:35:49.000000 letmedoit-2.1.9/letmedoit.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      466 2024-01-29 23:35:49.000000 letmedoit-2.1.9/letmedoit.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-01-29 23:35:49.000000 letmedoit-2.1.9/letmedoit.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-01-29 23:35:49.311887 letmedoit-2.1.9/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8804 2024-01-29 23:35:00.000000 letmedoit-2.1.9/setup.py
```

### Comparing `letmedoit-2.1.84/PKG-INFO` & `letmedoit-2.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,156 +1,69 @@
 Metadata-Version: 2.1
 Name: letmedoit
-Version: 2.1.84
+Version: 2.1.9
 Summary: LetMeDoIt AI, an advanced AI assistant, leveraging the capabilities of ChatGPT API, Gemini Pro and AutoGen, capable of engaging in conversations, executing codes with auto-healing, and assisting you with a wide range of tasks on your local devices.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
 Project-URL: Documentation, https://github.com/eliranwong/letmedoit/wiki
-Project-URL: Funding, https://www.paypal.me/letmedoitai
+Project-URL: Funding, https://www.paypal.me/MarvelBible
 Keywords: ai assistant openai chatgpt gemini autogen rag interpreter auto-heal
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <3.12
-Requires-Dist: openai==1.19.0
-Requires-Dist: groq==0.5.0
-Requires-Dist: requests
-Requires-Dist: argparse
-Requires-Dist: pendulum
-Requires-Dist: folium
-Requires-Dist: seaborn[stats]
-Requires-Dist: sympy
-Requires-Dist: numpy
-Requires-Dist: prompt_toolkit
-Requires-Dist: Pygments
-Requires-Dist: datetime
-Requires-Dist: netifaces
-Requires-Dist: geocoder
-Requires-Dist: googlesearch-python
-Requires-Dist: art
-Requires-Dist: apsw
-Requires-Dist: gTTS
-Requires-Dist: google-cloud-speech
-Requires-Dist: google-cloud-texttospeech
-Requires-Dist: google-cloud-aiplatform==1.47.0
-Requires-Dist: pywhatkit
-Requires-Dist: yt-dlp
-Requires-Dist: rembg
-Requires-Dist: qrcode
-Requires-Dist: pyperclip
-Requires-Dist: colorama
-Requires-Dist: pillow
-Requires-Dist: docker
-Requires-Dist: einops
-Requires-Dist: transformers==4.40.1
-Requires-Dist: torch==2.2.2
-Requires-Dist: torchvision==0.17.2
-Requires-Dist: sentence-transformers
-Requires-Dist: chromadb==0.4.24
-Requires-Dist: unstructured[all-docs]
-Requires-Dist: pyautogen[autobuild,retrievechat]==0.2.24
-Requires-Dist: autogenstudio==0.0.56
-Requires-Dist: tiktoken
-Requires-Dist: pygame
-Requires-Dist: PySide6
-Requires-Dist: feedparser
-Requires-Dist: html2text
-Requires-Dist: pypdf
-Requires-Dist: PyMuPDF
-Requires-Dist: yfinance
-Requires-Dist: setuptools-rust
-Requires-Dist: SpeechRecognition
-Requires-Dist: openai-whisper
-Requires-Dist: soundfile==0.12.1
-Requires-Dist: sounddevice==0.4.6
-Requires-Dist: elevenlabs==1.0.3
-Requires-Dist: ollama==0.1.8
-Requires-Dist: llama-cpp-python[server]==0.2.61
-Requires-Dist: huggingface-hub
-Requires-Dist: langchain==0.1.13
-Requires-Dist: langchain_openai==0.1.3
-Requires-Dist: pydub
-Requires-Dist: stable-diffusion-cpp-python
-Requires-Dist: pytz
-Requires-Dist: geopy
-Requires-Dist: guidance==0.1.13
 
 # LetMeDoIt AI
 
 Welcome to LetMeDoIt AI, your premier virtual assistant designed to revolutionize the way you work! More than a mere chatbot, I am equipped with the capability to conduct meaningful interactions and actively carry out computing tasks as per your directives. My real-time code generation and execution prowess guarantees not only effectiveness but also efficiency in task fulfillment. With an advanced auto-correction feature, I autonomously repair any malfunctioning code segments and automatically install necessary libraries, ensuring uninterrupted workflow. My commitment to your digital safety is paramount, with inbuilt risk assessments and tailored user confirmation protocols to protect your data and device.
 
-With LetMeDoIt AI, you can access OpenAI ChatGPT-4, Google Gemini Pro, and Microsoft AutoGen, local LLMs, all in one place, to enhance your productivity. [Read more ...](https://github.com/eliranwong/letmedoit/wiki#letmedoit-ai)
+With LetMeDoIt AI, you can access OpenAI ChatGPT-4, Google Gemini Pro, and Microsoft AutoGen, all in one place, to enhance your productivity. [Read more ...](https://github.com/eliranwong/letmedoit/wiki#letmedoit-ai)
 
 Developer: [Eliran Wong](https://github.com/eliranwong)
 
 Website: https://LetMeDoIt.ai
 
 Source: https://github.com/eliranwong/letmedoit
 
 Installation: https://github.com/eliranwong/letmedoit/wiki/Installation
 
 Quick-Guide: https://github.com/eliranwong/letmedoit/wiki/Quick-Guide
 
 Wiki: https://github.com/eliranwong/letmedoit/wiki
 
-Video Demo: https://www.youtube.com/watch?v=Eeat6h_ktbQ&list=PLo4xQ5NqC8SEMM71xC4NNhOHJCFlW-jaJ
+Support this project: https://www.paypal.me/MarvelBible
 
-Support this project: https://www.paypal.me/letmedoitai
+# An Interview
 
-# Video Demo
+[![Watch the video](https://img.youtube.com/vi/Dfsl-Cxx0bQ/maxresdefault.jpg)](https://youtu.be/Dfsl-Cxx0bQ)
 
-[![Watch the video](https://img.youtube.com/vi/Eeat6h_ktbQ/maxresdefault.jpg)](https://youtu.be/Eeat6h_ktbQ)
-
-Youtube Playlist: https://www.youtube.com/watch?v=Eeat6h_ktbQ&list=PLo4xQ5NqC8SEMM71xC4NNhOHJCFlW-jaJ
-
-# LetMeDoIt Features without OpenAI?
-
-You can utilize Google Gemini or open-source LLMs through Ollama for chat features in the LetMeDoIt AI.
-
-If you're seeking the complete functionality of LetMeDoIt, which includes both chat and task execution features, without the need for an Open AI API key, we offer support for Gemini Pro, Ollama, and Llama.cpp in our related project, FreeGenius AI:
-
-https://github.com/eliranwong/freegenius
+Read more at: https://github.com/eliranwong/letmedoit/wiki#an-interview
 
 # Requirements
 
 1. ChatGPT API key (read https://github.com/eliranwong/letmedoit/wiki/ChatGPT-API-Key)
 
 2. [Python](https://www.python.org) version 3.8-3.11; read [Install a Supported Python Version](https://github.com/eliranwong/letmedoit/wiki/Install-a-Supported-Python-Version)
 
 3. Supported OS: Windows / macOS / Linux / ChromeOS / Android (Termux)
 
 # Recent Additions
 
-[Generate tweets](https://github.com/eliranwong/letmedoit/wiki/Social-Media)
-
-<img width="798" alt="twitter" src="https://github.com/eliranwong/letmedoit/assets/25262722/d19c7bca-3bdc-48be-a907-b75afb34615b">
-
-[Run Local LLM Offline](https://github.com/eliranwong/letmedoit/wiki/Run-Local-LLM-Offline)
-
-<img width="832" alt="support_localllm" src="https://github.com/eliranwong/letmedoit/assets/25262722/587aba21-7f89-4b78-bfc4-3b32b442b287">
-
-[Talk to LetMeDoIt in Multiple Languages](https://github.com/eliranwong/letmedoit/wiki/Speak-to-LetMeDoIt-AI)
-
-![talk_to_letmedoit](https://github.com/eliranwong/letmedoit/assets/25262722/6aa33f2d-8971-45ad-b5ac-e8f4e290bff5)
-
-[Analyze audio](https://github.com/eliranwong/letmedoit/wiki/Analyze-Audio)
-
-<img width="1440" alt="analyze_audio" src="https://github.com/eliranwong/letmedoit/assets/25262722/24e49f3b-289d-40f6-bf9c-45ed1e0eeed6">
-
 [Search / Analyze Financial Data](https://github.com/eliranwong/letmedoit/wiki/Search-Financial-Data)
 
 <img width="1312" alt="search_financial_data" src="https://github.com/eliranwong/letmedoit/assets/25262722/9976f15b-85e1-4c5b-97a0-5124c04ffa8a">
 
 [Access Weather Information](https://github.com/eliranwong/letmedoit/wiki/Search-Weather-Information)
 
 ![test_weather_plugin](https://github.com/eliranwong/letmedoit/assets/25262722/e9fd4376-1579-40e0-b1b2-a2b7c5583f0c)
@@ -237,22 +150,14 @@
 
 * developer mode available
 
 # Examples of Plugin Features (selective only):
 
 Latest LetMeDoIt Plugins allow you to acheive variety of tasks with natural language:
 
-* [NEW] generate tweets
-
-> Post a short tweet about LetMeDoIt AI
-
-* [NEW] analyze audio
-
-> transcribe "meeting_records.mp3"
-
 * [NEW] search / analyze financial data
 
 > What was the average stock price of Apple Inc. in 2023?
 
 > Analyze Apple Inc's stock price over last 5 years.
 
 * [NEW] search weather information
@@ -604,8 +509,10 @@
 
 > share text "Hello World!" on Android
 
 Read more at: https://github.com/eliranwong/letmedoit/wiki/Android-Support
 
 # Donations
 
-https://www.paypal.me/letmedoitai
+https://www.paypal.me/MarvelBible
+
+
```

### Comparing `letmedoit-2.1.84/letmedoit/README.md` & `letmedoit-2.1.9/letmedoit/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,43 @@
 # LetMeDoIt AI
 
 Welcome to LetMeDoIt AI, your premier virtual assistant designed to revolutionize the way you work! More than a mere chatbot, I am equipped with the capability to conduct meaningful interactions and actively carry out computing tasks as per your directives. My real-time code generation and execution prowess guarantees not only effectiveness but also efficiency in task fulfillment. With an advanced auto-correction feature, I autonomously repair any malfunctioning code segments and automatically install necessary libraries, ensuring uninterrupted workflow. My commitment to your digital safety is paramount, with inbuilt risk assessments and tailored user confirmation protocols to protect your data and device.
 
-With LetMeDoIt AI, you can access OpenAI ChatGPT-4, Google Gemini Pro, and Microsoft AutoGen, local LLMs, all in one place, to enhance your productivity. [Read more ...](https://github.com/eliranwong/letmedoit/wiki#letmedoit-ai)
+With LetMeDoIt AI, you can access OpenAI ChatGPT-4, Google Gemini Pro, and Microsoft AutoGen, all in one place, to enhance your productivity. [Read more ...](https://github.com/eliranwong/letmedoit/wiki#letmedoit-ai)
 
 Developer: [Eliran Wong](https://github.com/eliranwong)
 
 Website: https://LetMeDoIt.ai
 
 Source: https://github.com/eliranwong/letmedoit
 
 Installation: https://github.com/eliranwong/letmedoit/wiki/Installation
 
 Quick-Guide: https://github.com/eliranwong/letmedoit/wiki/Quick-Guide
 
 Wiki: https://github.com/eliranwong/letmedoit/wiki
 
-Video Demo: https://www.youtube.com/watch?v=Eeat6h_ktbQ&list=PLo4xQ5NqC8SEMM71xC4NNhOHJCFlW-jaJ
+Support this project: https://www.paypal.me/MarvelBible
 
-Support this project: https://www.paypal.me/letmedoitai
+# An Interview
 
-# Video Demo
+[![Watch the video](https://img.youtube.com/vi/Dfsl-Cxx0bQ/maxresdefault.jpg)](https://youtu.be/Dfsl-Cxx0bQ)
 
-[![Watch the video](https://img.youtube.com/vi/Eeat6h_ktbQ/maxresdefault.jpg)](https://youtu.be/Eeat6h_ktbQ)
-
-Youtube Playlist: https://www.youtube.com/watch?v=Eeat6h_ktbQ&list=PLo4xQ5NqC8SEMM71xC4NNhOHJCFlW-jaJ
-
-# LetMeDoIt Features without OpenAI?
-
-You can utilize Google Gemini or open-source LLMs through Ollama for chat features in the LetMeDoIt AI.
-
-If you're seeking the complete functionality of LetMeDoIt, which includes both chat and task execution features, without the need for an Open AI API key, we offer support for Gemini Pro, Ollama, and Llama.cpp in our related project, FreeGenius AI:
-
-https://github.com/eliranwong/freegenius
+Read more at: https://github.com/eliranwong/letmedoit/wiki#an-interview
 
 # Requirements
 
 1. ChatGPT API key (read https://github.com/eliranwong/letmedoit/wiki/ChatGPT-API-Key)
 
 2. [Python](https://www.python.org) version 3.8-3.11; read [Install a Supported Python Version](https://github.com/eliranwong/letmedoit/wiki/Install-a-Supported-Python-Version)
 
 3. Supported OS: Windows / macOS / Linux / ChromeOS / Android (Termux)
 
 # Recent Additions
 
-[Generate tweets](https://github.com/eliranwong/letmedoit/wiki/Social-Media)
-
-<img width="798" alt="twitter" src="https://github.com/eliranwong/letmedoit/assets/25262722/d19c7bca-3bdc-48be-a907-b75afb34615b">
-
-[Run Local LLM Offline](https://github.com/eliranwong/letmedoit/wiki/Run-Local-LLM-Offline)
-
-<img width="832" alt="support_localllm" src="https://github.com/eliranwong/letmedoit/assets/25262722/587aba21-7f89-4b78-bfc4-3b32b442b287">
-
-[Talk to LetMeDoIt in Multiple Languages](https://github.com/eliranwong/letmedoit/wiki/Speak-to-LetMeDoIt-AI)
-
-![talk_to_letmedoit](https://github.com/eliranwong/letmedoit/assets/25262722/6aa33f2d-8971-45ad-b5ac-e8f4e290bff5)
-
-[Analyze audio](https://github.com/eliranwong/letmedoit/wiki/Analyze-Audio)
-
-<img width="1440" alt="analyze_audio" src="https://github.com/eliranwong/letmedoit/assets/25262722/24e49f3b-289d-40f6-bf9c-45ed1e0eeed6">
-
 [Search / Analyze Financial Data](https://github.com/eliranwong/letmedoit/wiki/Search-Financial-Data)
 
 <img width="1312" alt="search_financial_data" src="https://github.com/eliranwong/letmedoit/assets/25262722/9976f15b-85e1-4c5b-97a0-5124c04ffa8a">
 
 [Access Weather Information](https://github.com/eliranwong/letmedoit/wiki/Search-Weather-Information)
 
 ![test_weather_plugin](https://github.com/eliranwong/letmedoit/assets/25262722/e9fd4376-1579-40e0-b1b2-a2b7c5583f0c)
@@ -150,22 +124,14 @@
 
 * developer mode available
 
 # Examples of Plugin Features (selective only):
 
 Latest LetMeDoIt Plugins allow you to acheive variety of tasks with natural language:
 
-* [NEW] generate tweets
-
-> Post a short tweet about LetMeDoIt AI
-
-* [NEW] analyze audio
-
-> transcribe "meeting_records.mp3"
-
 * [NEW] search / analyze financial data
 
 > What was the average stock price of Apple Inc. in 2023?
 
 > Analyze Apple Inc's stock price over last 5 years.
 
 * [NEW] search weather information
@@ -517,8 +483,8 @@
 
 > share text "Hello World!" on Android
 
 Read more at: https://github.com/eliranwong/letmedoit/wiki/Android-Support
 
 # Donations
 
-https://www.paypal.me/letmedoitai
+https://www.paypal.me/MarvelBible
```

### Comparing `letmedoit-2.1.84/letmedoit/autoassist.py` & `letmedoit-2.1.9/letmedoit/autoassist.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 if not os.path.isfile(configFile):
     open(configFile, "a", encoding="utf-8").close()
 from letmedoit import config
 if not hasattr(config, "max_consecutive_auto_reply"):
     config.max_consecutive_auto_reply = 10
 
 from letmedoit.health_check import HealthCheck
-if not hasattr(config, "currentMessages"):
+if not hasattr(config, "openaiApiKey") or not config.openaiApiKey:
     HealthCheck.setBasicConfig()
-    if not hasattr(config, "openaiApiKey") or not config.openaiApiKey:
-        HealthCheck.changeAPIkey()
-    config.saveConfig()
-    #print("Configurations updated!")
+    HealthCheck.changeAPIkey()
+    HealthCheck.saveConfig()
+    print("Configurations updated!")
 HealthCheck.checkCompletion()
 
 import autogen, os, json, traceback
 from letmedoit.utils.prompts import Prompts
 from letmedoit.utils.shared_utils import SharedUtil
 from prompt_toolkit import print_formatted_text, HTML
 from prompt_toolkit.styles import Style
@@ -34,27 +33,17 @@
     def __init__(self):
         #config_list = autogen.get_config_list(
         #    [config.openaiApiKey], # assume openaiApiKey is in place in config.py
         #    api_type="openai",
         #    api_version=None,
         #)
         oai_config_list = []
-        for model in HealthCheck.tokenLimits.keys():
+        for model in ("gpt-4-turbo-preview", "gpt-4-0125-preview", "gpt-4-1106-preview", "gpt-3.5-turbo", "gpt-3.5-turbo-16k", "gpt-4", "gpt-4-32k"):
             oai_config_list.append({"model": model, "api_key": config.openaiApiKey})
-        if not config.chatGPTApiModel in HealthCheck.tokenLimits:
-            oai_config_list.append({"model": config.chatGPTApiModel, "api_key": config.openaiApiKey})
         os.environ["OAI_CONFIG_LIST"] = json.dumps(oai_config_list)
-        """
-        Code execution is set to be run in docker (default behaviour) but docker is not running.
-        The options available are:
-        - Make sure docker is running (advised approach for code execution)
-        - Set "use_docker": False in code_execution_config
-        - Set AUTOGEN_USE_DOCKER to "0/False/no" in your environment variables
-        """
-        os.environ["AUTOGEN_USE_DOCKER"] = "False"
 
     def getResponse(self, message, auto=False):
 
         message = f"""Current device information is given below:
 {SharedUtil.getDeviceInfo()}
 
 Below is my message:
@@ -115,15 +104,15 @@
             auto = True
             self.print("Enter maximum consecutive auto-reply below:")
             max_consecutive_auto_reply = prompts.simplePrompt(numberOnly=True, style=promptStyle, default=str(config.max_consecutive_auto_reply),)
             if max_consecutive_auto_reply and int(max_consecutive_auto_reply) > 1:
                 config.max_consecutive_auto_reply = int(max_consecutive_auto_reply)
 
         self.print(f"<{config.terminalCommandEntryColor1}>AutoGen Assistant launched!</{config.terminalCommandEntryColor1}>")
-        self.print(f"""[press '{str(config.hotkey_exit).replace("'", "")[1:-1]}' to exit]""")
+        self.print("[press 'ctrl+q' to exit]")
         while True:
             self.print(f"<{config.terminalCommandEntryColor1}>New chat started!</{config.terminalCommandEntryColor1}>")
             self.print(f"<{config.terminalCommandEntryColor1}>Enter your message below:</{config.terminalCommandEntryColor1}>")
             message = prompts.simplePrompt(style=promptStyle)
             if message == config.exit_entry:
                 break
             try:
```

### Comparing `letmedoit-2.1.84/letmedoit/autobuilder.py` & `letmedoit-2.1.9/letmedoit/autobuilder.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     config.max_agents = 5
 if not hasattr(config, "max_group_chat_round"):
     config.max_group_chat_round = 12
 if not hasattr(config, "use_oai_assistant"):
     config.use_oai_assistant = False
 
 from letmedoit.health_check import HealthCheck
-if not hasattr(config, "currentMessages"):
+if not hasattr(config, "openaiApiKey") or not config.openaiApiKey:
     HealthCheck.setBasicConfig()
-    if not hasattr(config, "openaiApiKey") or not config.openaiApiKey:
-        HealthCheck.changeAPIkey()
-    config.saveConfig()
-    #print("Configurations updated!")
+    HealthCheck.changeAPIkey()
+    HealthCheck.saveConfig()
+    print("Configurations updated!")
 HealthCheck.checkCompletion()
+HealthCheck.setPrint()
 
 from autogen.agentchat.contrib.agent_builder import AgentBuilder
 #from letmedoit.utils.agent_builder import AgentBuilder
 import autogen, os, json, traceback, re, datetime, argparse
 from pathlib import Path
 from urllib.parse import quote
 from letmedoit.utils.prompts import Prompts
@@ -36,32 +36,24 @@
 #from prompt_toolkit.history import FileHistory
 
 # Reference: https://microsoft.github.io/autogen/docs/reference/agentchat/contrib/agent_builder
 class AutoGenBuilder:
 
     def __init__(self):
         #config_list = autogen.get_config_list(
-        #    [config.openaiApiKey], # assume openaiApiKey is in config.py
+        #    [config.openaiApiKey], # assume openaiApiKey is in place in config.py
         #    api_type="openai",
         #    api_version=None,
         #)
-        # assign ChatGPT4 to run the builder
-        self.chatGPTmodel = "gpt-4-turbo-preview"
         oai_config_list = []
-        for model in (self.chatGPTmodel,):
+        for model in ("gpt-4-turbo-preview", "gpt-4-0125-preview", "gpt-4-1106-preview", "gpt-3.5-turbo", "gpt-3.5-turbo-16k", "gpt-4", "gpt-4-32k"):
             oai_config_list.append({"model": model, "api_key": config.openaiApiKey})
         os.environ["OAI_CONFIG_LIST"] = json.dumps(oai_config_list)
-        """
-        Code execution is set to be run in docker (default behaviour) but docker is not running.
-        The options available are:
-        - Make sure docker is running (advised approach for code execution)
-        - Set "use_docker": False in code_execution_config
-        - Set AUTOGEN_USE_DOCKER to "0/False/no" in your environment variables
-        """
-        os.environ["AUTOGEN_USE_DOCKER"] = "False"
+        # assign ChatGPT4 to run the builder
+        self.chatGPTmodel = "gpt-4-turbo-preview"
         # prompt style
         self.promptStyle = Style.from_dict({
             # User input (default text).
             "": config.terminalCommandEntryColor2,
             # Prompt.
             "indicator": config.terminalPromptIndicatorColor2,
         })
@@ -148,21 +140,21 @@
         max_group_chat_round = self.prompts.simplePrompt(numberOnly=True, style=self.promptStyle, default=str(config.max_group_chat_round),)
         if max_group_chat_round and int(max_group_chat_round) > 1:
             config.max_group_chat_round = int(max_group_chat_round)
         self.print("Do you want to support OpenAI Assistant API (y/yes/N/NO)?")
         userInput = self.prompts.simplePrompt(style=self.promptStyle, default="y" if config.use_oai_assistant else "NO")
         if userInput:
             config.use_oai_assistant = True if userInput.strip().lower() in ("y", "yes") else False
-        config.saveConfig()
+        HealthCheck.saveConfig()
 
     def run(self):
         self.promptConfig()
 
         self.print(f"<{config.terminalCommandEntryColor1}>AutoGen Agent Builder launched!</{config.terminalCommandEntryColor1}>")
-        self.print(f"""[press '{str(config.hotkey_exit).replace("'", "")[1:-1]}' to exit]""")
+        self.print("[press 'ctrl+q' to exit]")
         while True:
             self.print(f"<{config.terminalCommandEntryColor1}>Hi! I am ready for a new task.</{config.terminalCommandEntryColor1}>")
             task = self.promptTask()
             if task == config.exit_entry:
                 break
             try:
                 self.getResponse(task)
```

### Comparing `letmedoit-2.1.84/letmedoit/automath.py` & `letmedoit-2.1.9/letmedoit/automath.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,20 +6,19 @@
     os.chdir(packageFolder)
 configFile = os.path.join(packageFolder, "config.py")
 if not os.path.isfile(configFile):
     open(configFile, "a", encoding="utf-8").close()
 from letmedoit import config
 
 from letmedoit.health_check import HealthCheck
-if not hasattr(config, "currentMessages"):
+if not hasattr(config, "openaiApiKey") or not config.openaiApiKey:
     HealthCheck.setBasicConfig()
-    if not hasattr(config, "openaiApiKey") or not config.openaiApiKey:
-        HealthCheck.changeAPIkey()
-    config.saveConfig()
-    #print("Configurations updated!")
+    HealthCheck.changeAPIkey()
+    HealthCheck.saveConfig()
+    print("Configurations updated!")
 HealthCheck.checkCompletion()
 
 import autogen, os, json, traceback
 from pathlib import Path
 from letmedoit.utils.prompts import Prompts
 from prompt_toolkit import print_formatted_text, HTML
 from prompt_toolkit.styles import Style
@@ -32,27 +31,17 @@
     def __init__(self):
         #config_list = autogen.get_config_list(
         #    [config.openaiApiKey], # assume openaiApiKey is in place in config.py
         #    api_type="openai",
         #    api_version=None,
         #)
         oai_config_list = []
-        for model in HealthCheck.tokenLimits.keys():
+        for model in ("gpt-4-turbo-preview", "gpt-4-0125-preview", "gpt-4-1106-preview", "gpt-3.5-turbo", "gpt-3.5-turbo-16k", "gpt-4", "gpt-4-32k"):
             oai_config_list.append({"model": model, "api_key": config.openaiApiKey})
-        if not config.chatGPTApiModel in HealthCheck.tokenLimits:
-            oai_config_list.append({"model": config.chatGPTApiModel, "api_key": config.openaiApiKey})
         os.environ["OAI_CONFIG_LIST"] = json.dumps(oai_config_list)
-        """
-        Code execution is set to be run in docker (default behaviour) but docker is not running.
-        The options available are:
-        - Make sure docker is running (advised approach for code execution)
-        - Set "use_docker": False in code_execution_config
-        - Set AUTOGEN_USE_DOCKER to "0/False/no" in your environment variables
-        """
-        os.environ["AUTOGEN_USE_DOCKER"] = "False"
 
     def getResponse(self, math_problem):
         config_list = autogen.config_list_from_json(
             env_or_file="OAI_CONFIG_LIST",  # or OAI_CONFIG_LIST.json if file extension is added
             filter_dict={
                 "model": {
                     config.chatGPTApiModel,
@@ -104,19 +93,19 @@
             # User input (default text).
             "": config.terminalCommandEntryColor2,
             # Prompt.
             "indicator": config.terminalPromptIndicatorColor2,
         })
         prompts = Prompts()
         self.print(f"<{config.terminalCommandEntryColor1}>AutoGen Math Solver launched!</{config.terminalCommandEntryColor1}>")
-        self.print(f"""[press '{str(config.hotkey_exit).replace("'", "")[1:-1]}' to exit]""")
+        self.print("[press 'ctrl+q' to exit]")
         while True:
             self.print(f"<{config.terminalCommandEntryColor1}>New session started!</{config.terminalCommandEntryColor1}>")
             self.print(f"<{config.terminalCommandEntryColor1}>Enter a math problem below:</{config.terminalCommandEntryColor1}>")
-            self.print(f"""[press '{str(config.hotkey_exit).replace("'", "")[1:-1]}' to exit]""")
+            self.print("[press 'ctrl+q' to exit]")
             math_problem = prompts.simplePrompt(style=promptStyle)
             if math_problem == config.exit_entry:
                 break
             try:
                 self.getResponse(math_problem)
             except:
                 self.print(traceback.format_exc())
```

### Comparing `letmedoit-2.1.84/letmedoit/autoretriever.py` & `letmedoit-2.1.9/letmedoit/autoretriever.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 if not os.path.isfile(configFile):
     open(configFile, "a", encoding="utf-8").close()
 from letmedoit import config
 if not hasattr(config, "max_consecutive_auto_reply"):
     config.max_consecutive_auto_reply = 10
 
 from letmedoit.health_check import HealthCheck
-if not hasattr(config, "currentMessages"):
+if not hasattr(config, "openaiApiKey") or not config.openaiApiKey:
     HealthCheck.setBasicConfig()
-    if not hasattr(config, "openaiApiKey") or not config.openaiApiKey:
-        HealthCheck.changeAPIkey()
-    config.saveConfig()
-    #print("Configurations updated!")
+    HealthCheck.changeAPIkey()
+    HealthCheck.saveConfig()
+    print("Configurations updated!")
 HealthCheck.checkCompletion()
+HealthCheck.setPrint()
 
 import autogen, os, json, traceback, chromadb, re, zipfile, datetime, traceback
 from chromadb.config import Settings
 from pathlib import Path
 from letmedoit.utils.prompts import Prompts
 from prompt_toolkit import print_formatted_text, HTML
 from prompt_toolkit.styles import Style
@@ -36,27 +36,17 @@
     def __init__(self):
         #config_list = autogen.get_config_list(
         #    [config.openaiApiKey], # assume openaiApiKey is in place in config.py
         #    api_type="openai",
         #    api_version=None,
         #)
         oai_config_list = []
-        for model in HealthCheck.tokenLimits.keys():
+        for model in ("gpt-4-turbo-preview", "gpt-4-0125-preview", "gpt-4-1106-preview", "gpt-3.5-turbo", "gpt-3.5-turbo-16k", "gpt-4", "gpt-4-32k"):
             oai_config_list.append({"model": model, "api_key": config.openaiApiKey})
-        if not config.chatGPTApiModel in HealthCheck.tokenLimits:
-            oai_config_list.append({"model": config.chatGPTApiModel, "api_key": config.openaiApiKey})
         os.environ["OAI_CONFIG_LIST"] = json.dumps(oai_config_list)
-        """
-        Code execution is set to be run in docker (default behaviour) but docker is not running.
-        The options available are:
-        - Make sure docker is running (advised approach for code execution)
-        - Set "use_docker": False in code_execution_config
-        - Set AUTOGEN_USE_DOCKER to "0/False/no" in your environment variables
-        """
-        os.environ["AUTOGEN_USE_DOCKER"] = "False"
 
     def getResponse(self, docs_path, message, auto=False):
         if not os.path.exists(docs_path):
             config.print2("Invalid path!")
             return None
 
         package = os.path.basename(packageFolder)
@@ -175,15 +165,15 @@
             auto = True
             self.print("Enter maximum consecutive auto-reply below:")
             max_consecutive_auto_reply = prompts.simplePrompt(numberOnly=True, style=promptStyle, default=str(config.max_consecutive_auto_reply),)
             if max_consecutive_auto_reply and int(max_consecutive_auto_reply) > 1:
                 config.max_consecutive_auto_reply = int(max_consecutive_auto_reply)
 
         self.print(f"<{config.terminalCommandEntryColor1}>AutoGen Retriever launched!</{config.terminalCommandEntryColor1}>")
-        self.print(f"""[press '{str(config.hotkey_exit).replace("'", "")[1:-1]}' to exit]""")
+        self.print("[press 'ctrl+q' to exit]")
         
         self.print(f"<{config.terminalCommandEntryColor1}>Enter document path below (file / folder):</{config.terminalCommandEntryColor1}>")
         self.print(f"""Supported formats: *.{", *.".join(TEXT_FORMATS)}""" + ", *.zip")
         docs_path = prompts.simplePrompt(style=promptStyle)
 
         # handle path dragged to terminal
         docs_path = self.refinePath(docs_path)
```

### Comparing `letmedoit-2.1.84/letmedoit/chatgpt.py` & `letmedoit-2.1.9/letmedoit/chatgpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from letmedoit import config
 from letmedoit.utils.streaming_word_wrapper import StreamingWordWrapper
 from letmedoit.health_check import HealthCheck
-if not hasattr(config, "currentMessages"):
+if not hasattr(config, "openaiApiKey") or not config.openaiApiKey:
     HealthCheck.setBasicConfig()
-    if not hasattr(config, "openaiApiKey") or not config.openaiApiKey:
-        HealthCheck.changeAPIkey()
-    config.saveConfig()
-    #print("Configurations updated!")
+    HealthCheck.changeAPIkey()
+    HealthCheck.saveConfig()
+    print("Configurations updated!")
 HealthCheck.checkCompletion()
+HealthCheck.setPrint()
 
 from openai import OpenAI
 from prompt_toolkit.styles import Style
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.shortcuts import clear
 from pathlib import Path
@@ -29,46 +29,46 @@
         self.client = OpenAI()
         self.messages = self.resetMessages()
         if hasattr(config, "currentMessages") and config.currentMessages:
             self.messages += config.currentMessages[:-1]
         self.defaultPrompt = ""
 
     def resetMessages(self):
-        return [{"role": "system", "content": config.systemMessage_chatgpt},]
+        return [{"role": "system", "content": "You are a helpful assistant."},]
 
     def getDynamicTokens(self):
         tokenLimit = HealthCheck.tokenLimits[config.chatGPTApiModel]
         currentMessagesTokens = HealthCheck.count_tokens_from_messages(self.messages)
         availableTokens = tokenLimit - currentMessagesTokens
         if availableTokens >= self.max_output_tokens:
             return self.max_output_tokens
         elif (self.max_output_tokens > availableTokens > config.chatGPTApiMinTokens):
             return availableTokens
         return config.chatGPTApiMinTokens
 
     def run(self, prompt=""):
         if self.defaultPrompt:
             prompt, self.defaultPrompt = self.defaultPrompt, ""
-        historyFolder = os.path.join(HealthCheck.getLocalStorage(), "history")
+        historyFolder = os.path.join(HealthCheck.getFiles(), "history")
         Path(historyFolder).mkdir(parents=True, exist_ok=True)
         chat_history = os.path.join(historyFolder, "chatgpt")
         chat_session = PromptSession(history=FileHistory(chat_history))
 
         promptStyle = Style.from_dict({
             # User input (default text).
             "": config.terminalCommandEntryColor2,
             # Prompt.
             "indicator": config.terminalPromptIndicatorColor2,
         })
 
         HealthCheck.print2(f"\n{self.name} loaded!")
         if hasattr(config, "currentMessages"):
-            bottom_toolbar = f""" {str(config.hotkey_exit).replace("'", "")} {config.exit_entry}"""
+            bottom_toolbar = f" [ctrl+q] {config.exit_entry}"
         else:
-            bottom_toolbar = f""" {str(config.hotkey_exit).replace("'", "")} {config.exit_entry} {str(config.hotkey_new).replace("'", "")} .new"""
+            bottom_toolbar = f" [ctrl+q] {config.exit_entry} [ctrl+n] .new"
             print("(To start a new chart, enter '.new')")
         print(f"(To exit, enter '{config.exit_entry}')\n")
         while True:
             if not prompt:
                 prompt = HealthCheck.simplePrompt(style=promptStyle, promptSession=chat_session, bottom_toolbar=bottom_toolbar)
                 userMessage = {"role": "user", "content": prompt}
                 self.messages.append(userMessage)
@@ -117,15 +117,15 @@
                     self.streaming_thread.join()
                     HealthCheck.print2(traceback.format_exc())
 
             prompt = ""
 
         HealthCheck.print2(f"\n{self.name} closed!")
         if hasattr(config, "currentMessages"):
-            HealthCheck.print2(f"Return back to {config.letMeDoItName} prompt ...")
+            HealthCheck.print2(f"Going back to {config.letMeDoItName} prompt ...")
 
 def main():
     # Create the parser
     parser = argparse.ArgumentParser(description="chatgpt cli options")
     # Add arguments
     parser.add_argument("default", nargs="?", default=None, help="default entry")
     parser.add_argument('-o', '--outputtokens', action='store', dest='outputtokens', help=f"specify maximum output tokens with -o flag; default: {config.chatGPTApiMaxTokens}")
```

### Comparing `letmedoit-2.1.84/letmedoit/codey.py` & `letmedoit-2.1.9/letmedoit/codey.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import vertexai, os, traceback, argparse
 from vertexai.language_models import CodeChatModel, ChatMessage
 from letmedoit import config
 from letmedoit.health_check import HealthCheck
-if not hasattr(config, "currentMessages"):
+if not hasattr(config, "exit_entry"):
     HealthCheck.setBasicConfig()
-    config.saveConfig()
-    #print("Configurations updated!")
+    HealthCheck.saveConfig()
+    print("Configurations updated!")
+HealthCheck.setPrint()
 import pygments
 from pygments.lexers.markup import MarkdownLexer
 from prompt_toolkit.formatted_text import PygmentsTokens
 from prompt_toolkit import print_formatted_text
 from prompt_toolkit.styles import Style
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
@@ -21,26 +22,28 @@
 #!pip install --upgrade google-cloud-aiplatform
 
 
 class Codey:
 
     def __init__(self, name="Codey"):
         # authentication
-        if os.environ["GOOGLE_APPLICATION_CREDENTIALS"] and "Vertex AI" in config.enabledGoogleAPIs:
+        authpath1 = os.path.join(HealthCheck.getFiles(), "credentials_googleaistudio.json")
+        if os.path.isfile(authpath1):
+            os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = authpath1
             self.runnable = True
         else:
-            print("Vertex AI is disabled!")
+            print(f"API key json file '{authpath1}' not found!")
             print("Read https://github.com/eliranwong/letmedoit/wiki/Google-API-Setup for setting up Google API.")
             self.runnable = False
         # initiation
         vertexai.init()
         self.name = name
 
     def run(self, prompt="", model="codechat-bison-32k", temperature=0.2, max_output_tokens=2048):
-        historyFolder = os.path.join(HealthCheck.getLocalStorage(), "history")
+        historyFolder = os.path.join(HealthCheck.getFiles(), "history")
         Path(historyFolder).mkdir(parents=True, exist_ok=True)
         chat_history = os.path.join(historyFolder, self.name.replace(" ", "_"))
         chat_session = PromptSession(history=FileHistory(chat_history))
 
         promptStyle = Style.from_dict({
             # User input (default text).
             "": config.terminalCommandEntryColor2,
@@ -69,22 +72,22 @@
                 history = history[:-1]
             elif not history:
                 history = None
         else:
             history = None
         # start chat
         chat = model.start_chat(
-            context=config.systemMessage_codey,
+            context=f"You're {self.name}, an expert in coding.",
             message_history=history,
         )
         HealthCheck.print2(f"\n{self.name} loaded!")
         if hasattr(config, "currentMessages"):
-            bottom_toolbar = f""" {str(config.hotkey_exit).replace("'", "")} {config.exit_entry}"""
+            bottom_toolbar = f" [ctrl+q] {config.exit_entry}"
         else:
-            bottom_toolbar = f""" {str(config.hotkey_exit).replace("'", "")} {config.exit_entry} {str(config.hotkey_new).replace("'", "")} .new"""
+            bottom_toolbar = f" [ctrl+q] {config.exit_entry} [ctrl+n] .new"
             print("(To start a new chart, enter '.new')")
         print(f"(To exit, enter '{config.exit_entry}')\n")
         while True:
             if not prompt:
                 prompt = HealthCheck.simplePrompt(style=promptStyle, promptSession=chat_session, bottom_toolbar=bottom_toolbar)
                 if prompt and not prompt in (".new", config.exit_entry) and hasattr(config, "currentMessages"):
                     config.currentMessages.append({"content": prompt, "role": "user"})
@@ -114,15 +117,15 @@
                     HealthCheck.stopSpinning()
                     HealthCheck.print2(traceback.format_exc())
 
             prompt = ""
 
         HealthCheck.print2(f"\n{self.name} closed!")
         if hasattr(config, "currentMessages"):
-            HealthCheck.print2(f"Return back to {config.letMeDoItName} prompt ...")
+            HealthCheck.print2(f"Going back to {config.letMeDoItName} prompt ...")
 
 def main():
     # Create the parser
     parser = argparse.ArgumentParser(description="codey cli options")
     # Add arguments
     parser.add_argument("default", nargs="?", default=None, help="default entry")
     parser.add_argument('-m', '--model', action='store', dest='model', help="specify language model with -m flag; default: codechat-bison-32k")
```

### Comparing `letmedoit-2.1.84/letmedoit/commandprompt.py` & `letmedoit-2.1.9/letmedoit/commandprompt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from letmedoit import config
 from letmedoit.health_check import HealthCheck
-if not hasattr(config, "currentMessages"):
+if not hasattr(config, "exit_entry"):
     HealthCheck.setBasicConfig()
-    config.saveConfig()
-    #print("Configurations updated!")
+    HealthCheck.saveConfig()
+    print("Configurations updated!")
+HealthCheck.setPrint()
 from letmedoit.utils.prompts import Prompts
 from letmedoit.utils.terminal_system_command_prompt import SystemCommandPrompt
 import platform
 
 def setOsOpenCmd():
     thisPlatform = platform.system()
     config.thisPlatform = thisPlatform
```

### Comparing `letmedoit-2.1.84/letmedoit/eTextEdit.py` & `letmedoit-2.1.9/letmedoit/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/geminipro.py` & `letmedoit-2.1.9/letmedoit/geminipro.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,19 @@
     GenerationConfig,
     HarmCategory,
     HarmBlockThreshold,
 )
 from letmedoit import config
 from letmedoit.utils.streaming_word_wrapper import StreamingWordWrapper
 from letmedoit.health_check import HealthCheck
-if not hasattr(config, "currentMessages"):
+if not hasattr(config, "exit_entry"):
     HealthCheck.setBasicConfig()
-    config.saveConfig()
-    #print("Configurations updated!")
+    HealthCheck.saveConfig()
+    print("Configurations updated!")
+HealthCheck.setPrint()
 from prompt_toolkit.styles import Style
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.shortcuts import clear
 from pathlib import Path
 import threading
 
@@ -24,54 +25,43 @@
 #!pip install --upgrade google-cloud-aiplatform
 
 
 class GeminiPro:
 
     def __init__(self, name="Gemini Pro", temperature=0.9, max_output_tokens=8192):
         # authentication
-        if os.environ["GOOGLE_APPLICATION_CREDENTIALS"] and "Vertex AI" in config.enabledGoogleAPIs:
+        authpath1 = os.path.join(HealthCheck.getFiles(), "credentials_googleaistudio.json")
+        if os.path.isfile(authpath1):
+            os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = authpath1
             self.runnable = True
         else:
-            print("Vertex AI is disabled!")
+            print(f"API key json file '{authpath1}' not found!")
             print("Read https://github.com/eliranwong/letmedoit/wiki/Google-API-Setup for setting up Google API.")
             self.runnable = False
         # initiation
         vertexai.init()
         self.name, self.temperature = name, temperature
         self.generation_config=GenerationConfig(
             temperature=temperature, # 0.0-1.0; default 0.9
             max_output_tokens=max_output_tokens, # default
             candidate_count=1,
         )
-        # Note: BLOCK_NONE is not allowed
         self.safety_settings={
-            HarmCategory.HARM_CATEGORY_UNSPECIFIED: HarmBlockThreshold.BLOCK_ONLY_HIGH,
-            HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_ONLY_HIGH,
-            HarmCategory.HARM_CATEGORY_HATE_SPEECH: HarmBlockThreshold.BLOCK_ONLY_HIGH,
-            HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_ONLY_HIGH,
-            HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT: HarmBlockThreshold.BLOCK_ONLY_HIGH,
+            HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_NONE,
+            HarmCategory.HARM_CATEGORY_HATE_SPEECH: HarmBlockThreshold.BLOCK_NONE,
+            HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_NONE,
+            HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT: HarmBlockThreshold.BLOCK_NONE,
         }
-        """
-        Alternately,
-        from google.cloud.aiplatform_v1beta1.types.content import SafetySetting
-        self.safety_settings = [
-            SafetySetting(category=HarmCategory.HARM_CATEGORY_UNSPECIFIED, threshold=HarmBlockThreshold.BLOCK_ONLY_HIGH)
-            SafetySetting(category=HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT, threshold=HarmBlockThreshold.BLOCK_ONLY_HIGH)
-            SafetySetting(category=HarmCategory.HARM_CATEGORY_HATE_SPEECH, threshold=HarmBlockThreshold.BLOCK_ONLY_HIGH)
-            SafetySetting(category=HarmCategory.HARM_CATEGORY_HARASSMENT, threshold=HarmBlockThreshold.BLOCK_ONLY_HIGH)
-            SafetySetting(category=HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT, threshold=HarmBlockThreshold.BLOCK_ONLY_HIGH)
-        ]
-        """
         self.defaultPrompt = ""
         #self.enableVision = (os.path.realpath(__file__).endswith("vision.py"))
 
     def run(self, prompt=""):
         if self.defaultPrompt:
             prompt, self.defaultPrompt = self.defaultPrompt, ""
-        historyFolder = os.path.join(HealthCheck.getLocalStorage(), "history")
+        historyFolder = os.path.join(HealthCheck.getFiles(), "history")
         Path(historyFolder).mkdir(parents=True, exist_ok=True)
         chat_history = os.path.join(historyFolder, "geminipro")
         chat_session = PromptSession(history=FileHistory(chat_history))
 
         promptStyle = Style.from_dict({
             # User input (default text).
             "": config.terminalCommandEntryColor2,
@@ -98,36 +88,34 @@
             if history and history[-1].role == "user":
                 history = history[:-1]
             elif not history:
                 history = None
         else:
             history = None
         chat = model.start_chat(history=history)
-        justStarted = True
         #HealthCheck.print2(f"\n{self.name} + Vision loaded!" if self.enableVision else f"\n{self.name} loaded!")
         HealthCheck.print2(f"\n{self.name} loaded!")
         if hasattr(config, "currentMessages"):
-            bottom_toolbar = f""" {str(config.hotkey_exit).replace("'", "")} {config.exit_entry}"""
+            bottom_toolbar = f" [ctrl+q] {config.exit_entry}"
         else:
-            bottom_toolbar = f""" {str(config.hotkey_exit).replace("'", "")} {config.exit_entry} {str(config.hotkey_new).replace("'", "")} .new"""
+            bottom_toolbar = f" [ctrl+q] {config.exit_entry} [ctrl+n] .new"
             print("(To start a new chart, enter '.new')")
         print(f"(To exit, enter '{config.exit_entry}')\n")
         while True:
             if not prompt:
                 prompt = HealthCheck.simplePrompt(style=promptStyle, promptSession=chat_session, bottom_toolbar=bottom_toolbar)
                 if prompt and not prompt in (".new", config.exit_entry) and hasattr(config, "currentMessages"):
                     config.currentMessages.append({"content": prompt, "role": "user"})
             else:
                 prompt = HealthCheck.simplePrompt(style=promptStyle, promptSession=chat_session, bottom_toolbar=bottom_toolbar, default=prompt, accept_default=True)
             if prompt == config.exit_entry:
                 break
             elif prompt == ".new" and not hasattr(config, "currentMessages"):
                 clear()
                 chat = model.start_chat()
-                justStarted = True
                 print("New chat started!")
             elif prompt := prompt.strip():
                 streamingWordWrapper = StreamingWordWrapper()
                 config.pagerContent = ""
                 #self.addPagerContent = True
 
                 # declare a function
@@ -150,17 +138,14 @@
 #                    },
 #                )
 #                vision_tool = generative_models.Tool(
 #                    function_declarations=[get_vision_func],
 #                )
 
                 try:
-                    if not hasattr(config, "currentMessages") and config.systemMessage_geminipro and justStarted:
-                        prompt = f"{config.systemMessage_geminipro}\n{prompt}"
-                        justStarted = False
                     # https://cloud.google.com/vertex-ai/docs/generative-ai/model-reference/gemini
                     # Note: At the time of writing, function call feature with Gemini Pro is very weak, compared with the function call feature offerred by ChatGPT:
                     # 1. Gemini Pro do not accept multiple tools in a single message
                     # 2. Gemini Pro is weak to determine if it is appropriate to use the given tool or not.  When a tool is given, it is called by mistake so often.  In contrast, ChatGPT has the "auto" setting which makes ChatGPT obviously smarter than Gemini Pro.
                     #if "[NO_FUNCTION_CALL]" in prompt or not self.enableVision:
                     #    allow_function_call = False
                     #    prompt = prompt.replace("[NO_FUNCTION_CALL]", "")
@@ -195,15 +180,15 @@
                     self.streaming_thread.join()
                     HealthCheck.print2(traceback.format_exc())
 
             prompt = ""
 
         HealthCheck.print2(f"\n{self.name} closed!")
         if hasattr(config, "currentMessages"):
-            HealthCheck.print2(f"Return back to {config.letMeDoItName} prompt ...")
+            HealthCheck.print2(f"Going back to {config.letMeDoItName} prompt ...")
 
 def main():
     # Create the parser
     parser = argparse.ArgumentParser(description="geminipro cli options")
     # Add arguments
     parser.add_argument("default", nargs="?", default=None, help="default entry")
     parser.add_argument('-o', '--outputtokens', action='store', dest='outputtokens', help="specify maximum output tokens with -o flag; default: 8192")
```

### Comparing `letmedoit-2.1.84/letmedoit/geminiprovision.py` & `letmedoit-2.1.9/letmedoit/geminiprovision.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,19 @@
     GenerationConfig,
     HarmCategory,
     HarmBlockThreshold,
 )
 from letmedoit import config
 from letmedoit.utils.streaming_word_wrapper import StreamingWordWrapper
 from letmedoit.health_check import HealthCheck
-if not hasattr(config, "currentMessages"):
+if not hasattr(config, "exit_entry"):
     HealthCheck.setBasicConfig()
-    config.saveConfig()
-    #print("Configurations updated!")
+    HealthCheck.saveConfig()
+    print("Configurations updated!")
+HealthCheck.setPrint()
 
 import shutil, textwrap
 from PIL import Image as im
 import requests
 import http.client
 import typing
 import urllib.request
@@ -27,33 +28,34 @@
 #!pip install --upgrade google-cloud-aiplatform
 
 
 class GeminiProVision:
 
     def __init__(self, temperature=0.9, max_output_tokens=2048):
         # authentication
-        if os.environ["GOOGLE_APPLICATION_CREDENTIALS"] and "Vertex AI" in config.enabledGoogleAPIs:
+        authpath1 = os.path.join(HealthCheck.getFiles(), "credentials_googleaistudio.json")
+        if os.path.isfile(authpath1):
+            os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = authpath1
             self.runnable = True
         else:
-            print("Vertex AI is disabled!")
+            print(f"API key json file '{authpath1}' not found!")
             print("Read https://github.com/eliranwong/letmedoit/wiki/Google-API-Setup for setting up Google API.")
             self.runnable = False
         # initiation
         vertexai.init()
         self.generation_config=GenerationConfig(
             temperature=temperature, # 0.0-1.0; default 0.9
             max_output_tokens=max_output_tokens, # default
             candidate_count=1,
         )
         self.safety_settings={
-            HarmCategory.HARM_CATEGORY_UNSPECIFIED: HarmBlockThreshold.BLOCK_ONLY_HIGH,
-            HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_ONLY_HIGH,
-            HarmCategory.HARM_CATEGORY_HATE_SPEECH: HarmBlockThreshold.BLOCK_ONLY_HIGH,
-            HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_ONLY_HIGH,
-            HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT: HarmBlockThreshold.BLOCK_ONLY_HIGH,
+            HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_NONE,
+            HarmCategory.HARM_CATEGORY_HATE_SPEECH: HarmBlockThreshold.BLOCK_NONE,
+            HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_NONE,
+            HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT: HarmBlockThreshold.BLOCK_NONE,
         }
 
     def refinePath(self, img_path):
         img_path = img_path.strip()
         img_path = re.sub("^'(.*?)'$", r"\1", img_path)
         if "\\ " in img_path or "\(" in img_path:
             img_path = img_path.replace("\\ ", " ")
@@ -65,15 +67,15 @@
             # User input (default text).
             "": config.terminalCommandEntryColor2,
             # Prompt.
             "indicator": config.terminalPromptIndicatorColor2,
         })
 
         HealthCheck.print2("\nGemini Pro Vision loaded!")
-        print(f"""[press '{str(config.hotkey_exit).replace("'", "")[1:-1]}' to exit]""")
+        print("[press 'ctrl+q' to exit]")
         if not files:
             HealthCheck.print2("Enter image path below (file / folder):")
             files = HealthCheck.simplePrompt(style=promptStyle)
         if files:
             # handle path dragged to terminal
             files = self.refinePath(files)
         if files == config.exit_entry:
```

### Comparing `letmedoit-2.1.84/letmedoit/health_check.py` & `letmedoit-2.1.9/letmedoit/health_check.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,26 +14,18 @@
 import openai, tiktoken
 from openai import OpenAI
 from pygments.styles import get_style_by_name
 from prompt_toolkit.styles.pygments import style_from_pygments_cls
 from prompt_toolkit import print_formatted_text, HTML
 from prompt_toolkit import prompt
 from prompt_toolkit.filters import Condition
-from prompt_toolkit.key_binding import KeyBindings, merge_key_bindings, ConditionalKeyBindings
+from prompt_toolkit.key_binding import KeyBindings, merge_key_bindings
 from prompt_toolkit.clipboard.pyperclip import PyperclipClipboard
-from prompt_toolkit.application import run_in_terminal
-from letmedoit.utils.vlc_utils import VlcUtil
-from letmedoit.utils.tts_utils import TTSUtil
-from letmedoit.utils.config_essential import defaultSettings
+from letmedoit.utils.prompt_shared_key_bindings import prompt_shared_key_bindings
 from pathlib import Path
-from PIL import Image
-import speech_recognition as sr
-# a dummy import line to resolve ALSA error display
-import sounddevice
-
 
 def check_openai_errors(func):
     def wrapper(*args, **kwargs):
         try: 
             return func(*args, **kwargs)
         except openai.APIError as e:
             print("Error: Issue on OpenAI side.")
@@ -74,70 +66,52 @@
     return wrapper
 
 class HealthCheck:
 
     # token limit
     # reference: https://platform.openai.com/docs/models/gpt-4
     tokenLimits = {
-        "gpt-4-turbo-preview": 128000, # Returns a maximum of 4,096 output tokens.
-        "gpt-4-0125-preview": 128000, # Returns a maximum of 4,096 output tokens.
-        "gpt-4-1106-preview": 128000, # Returns a maximum of 4,096 output tokens.
-        "gpt-3.5-turbo": 16385, # Returns a maximum of 4,096 output tokens.
+        #"gpt-3.5-turbo-instruct": 4097,
+        "gpt-3.5-turbo": 4097,
         "gpt-3.5-turbo-16k": 16385,
+        "gpt-4-turbo-preview": 128000,
+        "gpt-4-0125-preview": 128000,
+        "gpt-4-1106-preview": 128000, # official 128,000; but "This model supports at most 4096 completion tokens"; set 8192 here to work with LetMeDoIt AI dynamic token feature
+        #"gpt-4-vision-preview": 128,000, # used in plugin "analyze images"
         "gpt-4": 8192,
         "gpt-4-32k": 32768,
     }
 
     models = tuple(tokenLimits.keys())
 
     @staticmethod
-    def setBasicConfig():
-        if not hasattr(config, "setBasicConfigDone") or not config.setBasicConfigDone:
-            # package folder
-            config.letMeDoItAIFolder = packageFolder
-            config.excludeConfigList = []
-            # Default Settings
-            for key, value in defaultSettings:
-                if not hasattr(config, key):
-                    value = pprint.pformat(value)
-                    exec(f"""config.{key} = {value} """)
-            # tts
-            config.isVlcPlayerInstalled = VlcUtil.isVlcPlayerInstalled()
-            config.tts = False if not config.isVlcPlayerInstalled and not config.isPygameInstalled and not config.ttsCommand and not config.elevenlabsApi else True
-            # Google Credentials
-            if config.google_cloud_credentials and os.path.isfile(config.google_cloud_credentials):
-                os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = config.google_cloud_credentials
-            else:
-                files = HealthCheck.getLocalStorage()
-                gccfile1 = os.path.join(files, "credentials_google_cloud.json")
-                gccfile2 = os.path.join(files, "credentials_googleaistudio.json")
-                gccfile3 = os.path.join(files, "credentials_googletts.json")
-                # set required file
-                config.google_cloud_credentials_file = gccfile1
-
-                if os.path.isfile(gccfile1):
-                    config.google_cloud_credentials = gccfile1
-                elif os.path.isfile(gccfile2):
-                    config.google_cloud_credentials = gccfile2
-                elif os.path.isfile(gccfile3):
-                    config.google_cloud_credentials = gccfile3
-                else:
-                    config.google_cloud_credentials = ""
-                os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = config.google_cloud_credentials if config.google_cloud_credentials else ""
-                
-            # print functions
-            HealthCheck.setPrint()
-
-            config.setBasicConfigDone = True
-
-    @staticmethod
-    def showErrors():
-        trace = traceback.format_exc()
-        print(trace if config.developer else "Error encountered!")
-        return trace
+    def setBasicConfig(): # minimum config to work with standalone scripts built with AutoGen
+        config.openaiApiKey = ''
+        config.chatGPTApiModel = 'gpt-3.5-turbo-16k'
+        config.chatGPTApiMaxTokens = 4000
+        config.chatGPTApiMinTokens = 256
+        config.llmTemperature = 0.8
+        config.max_consecutive_auto_reply = 10
+        config.exit_entry = '.exit'
+        config.cancel_entry = '.cancel'
+        config.terminalPromptIndicatorColor1 = "ansimagenta"
+        config.terminalPromptIndicatorColor2 = "ansicyan"
+        config.terminalCommandEntryColor1 = "ansiyellow"
+        config.terminalCommandEntryColor2 = "ansigreen"
+        config.terminalResourceLinkColor = "ansiyellow"
+        config.terminalHeadingTextColor = "ansigreen"
+        config.mouseSupport = False
+        config.embeddingModel = "paraphrase-multilingual-mpnet-base-v2"
+        config.max_agents = 5
+        config.max_group_chat_round = 12
+        config.max_consecutive_auto_reply = 10
+        config.includeIpInSystemMessage = False
+        config.wrapWords = True
+        config.pygments_style = ""
+        HealthCheck.setPrint()
 
     @staticmethod
     def spinning_animation(stop_event):
         while not stop_event.is_set():
             for symbol in "|/-\\":
                 print(symbol, end="\r")
                 time.sleep(0.1)
@@ -155,129 +129,31 @@
         try:
             config.stop_event.set()
             config.spinner_thread.join()
         except:
             pass
 
     @staticmethod
-    def is_valid_image_file(file_path):
-        try:
-            # Open the image file
-            with Image.open(file_path) as img:
-                # Check if the file format is supported by PIL
-                img.verify()
-                return True
-        except (IOError, SyntaxError) as e:
-            # The file path is not a valid image file path
-            return False
-
-    @staticmethod
     def simplePrompt(inputIndicator="", validator=None, default="", accept_default=False, completer=None, promptSession=None, style=None, is_password=False, bottom_toolbar=None):
         this_key_bindings = KeyBindings()
-        @this_key_bindings.add(*config.hotkey_exit)
+        @this_key_bindings.add("c-q")
         def _(event):
             buffer = event.app.current_buffer
             buffer.text = config.exit_entry
             buffer.validate_and_handle()
-        @this_key_bindings.add(*config.hotkey_cancel)
-        def _(event):
-            buffer = event.app.current_buffer
-            buffer.reset()
-        @this_key_bindings.add(*config.hotkey_insert_newline)
-        def _(event):
-            buffer = event.app.current_buffer
-            buffer.newline()
-        @this_key_bindings.add(*config.hotkey_toggle_word_wrap)
-        def _(_):
-            config.wrapWords = not config.wrapWords
-            config.saveConfig()
-            run_in_terminal(lambda: config.print3(f"Word Wrap: '{'enabled' if config.wrapWords else 'disabled'}'!"))
-        @this_key_bindings.add(*config.hotkey_toggle_response_audio)
-        def _(_):
-            if config.tts:
-                config.ttsOutput = not config.ttsOutput
-                config.saveConfig()
-                run_in_terminal(lambda: config.print3(f"Response Audio: '{'enabled' if config.ttsOutput else 'disabled'}'!"))
-        @this_key_bindings.add(*config.hotkey_voice_entry)
-        def _(event):
-            # reference: https://github.com/Uberi/speech_recognition/blob/master/examples/microphone_recognition.py
-            def voiceTyping():
-                r = sr.Recognizer()
-                with sr.Microphone() as source:
-                    if config.voiceTypingNotification:
-                        TTSUtil.playAudioFilePygame(os.path.join(packageFolder, "audio", "notification1_mild.mp3"))
-                    #run_in_terminal(lambda: config.print2("Listensing to your voice ..."))
-                    if config.voiceTypingAdjustAmbientNoise:
-                        r.adjust_for_ambient_noise(source)
-                    audio = r.listen(source)
-                if config.voiceTypingNotification:
-                    TTSUtil.playAudioFilePygame(os.path.join(packageFolder, "audio", "notification2_mild.mp3"))
-                #run_in_terminal(lambda: config.print2("Processing to your voice ..."))
-                if config.voiceTypingPlatform == "google":
-                    # recognize speech using Google Speech Recognition
-                    try:
-                        # check google.recognize_legacy in SpeechRecognition package
-                        # check availabl languages at: https://cloud.google.com/speech-to-text/docs/speech-to-text-supported-languages
-                        # config.voiceTypingLanguage should be code list in column BCP-47 at https://cloud.google.com/speech-to-text/docs/speech-to-text-supported-languages
-                        return r.recognize_google(audio, language=config.voiceTypingLanguage)
-                    except sr.UnknownValueError:
-                        #return "[Speech unrecognized!]"
-                        return ""
-                    except sr.RequestError as e:
-                        return "[Error: {0}]".format(e)
-                elif config.voiceTypingPlatform == "googlecloud" and os.environ["GOOGLE_APPLICATION_CREDENTIALS"] and "Speech-to-Text" in config.enabledGoogleAPIs:
-                    # recognize speech using Google Cloud Speech
-                    try:
-                        # check availabl languages at: https://cloud.google.com/speech-to-text/docs/speech-to-text-supported-languages
-                        # config.voiceTypingLanguage should be code list in column BCP-47 at https://cloud.google.com/speech-to-text/docs/speech-to-text-supported-languages
-                        return r.recognize_google_cloud(audio, language=config.voiceTypingLanguage, credentials_json=config.google_cloud_credentials)
-                    except sr.UnknownValueError:
-                        #return "[Speech unrecognized!]"
-                        return ""
-                    except sr.RequestError as e:
-                        return "[Error: {0}]".format(e)
-                elif config.voiceTypingPlatform == "whisper":
-                    # recognize speech using whisper
-                    try:
-                        # check availabl languages at: https://github.com/openai/whisper/blob/main/whisper/tokenizer.py
-                        # config.voiceTypingLanguage should be uncapitalized full language name like "english" or "chinese"
-                        return r.recognize_whisper(audio, model=config.voiceTypingWhisperEnglishModel if config.voiceTypingLanguage == "english" else "large", language=config.voiceTypingLanguage)
-                    except sr.UnknownValueError:
-                        return ""
-                    except sr.RequestError as e:
-                        return "[Error]"
-
-            if config.pyaudioInstalled:
-                buffer = event.app.current_buffer
-                buffer.text = f"{buffer.text}{' ' if buffer.text else ''}{voiceTyping()}"
-                if config.voiceTypingAutoComplete:
-                    buffer.validate_and_handle()
-                else:
-                    buffer.cursor_position = buffer.cursor_position + buffer.document.get_end_of_line_position()
-            else:
-                run_in_terminal(lambda: config.print2("Install PyAudio first to enable voice entry!"))
-
         if hasattr(config, "currentMessages"):
-            from letmedoit.utils.prompt_shared_key_bindings import prompt_shared_key_bindings
-            from letmedoit.utils.prompt_multiline_shared_key_bindings import prompt_multiline_shared_key_bindings
-            @this_key_bindings.add(*config.hotkey_launch_pager_view)
+            @this_key_bindings.add("c-g")
             def _(_):
                 config.launchPager()
-            # additional key binding
-            conditional_prompt_multiline_shared_key_bindings = ConditionalKeyBindings(
-                key_bindings=prompt_multiline_shared_key_bindings,
-                filter=Condition(lambda: config.multilineInput),
-            )
             this_key_bindings = merge_key_bindings([
                 this_key_bindings,
                 prompt_shared_key_bindings,
-                conditional_prompt_multiline_shared_key_bindings,
             ])
         else:
-            @this_key_bindings.add(*config.hotkey_new)
+            @this_key_bindings.add("c-n")
             def _(event):
                 buffer = event.app.current_buffer
                 config.defaultEntry = buffer.text
                 buffer.text = ".new"
                 buffer.validate_and_handle()
 
         config.selectAll = False
@@ -287,20 +163,20 @@
         if not inputIndicator:
             inputIndicator = [
                 ("class:indicator", ">>> "),
             ]
         userInput = inputPrompt(
             inputIndicator,
             key_bindings=this_key_bindings,
-            bottom_toolbar=bottom_toolbar if bottom_toolbar is not None else f""" {str(config.hotkey_exit).replace("'", "")} {config.exit_entry}""",
+            bottom_toolbar=bottom_toolbar if bottom_toolbar is not None else f" [ctrl+q] {config.exit_entry}",
             #enable_system_prompt=True,
             swap_light_and_dark_colors=Condition(lambda: not config.terminalResourceLinkColor.startswith("ansibright")),
             style=style,
             validator=validator,
-            multiline=Condition(lambda: hasattr(config, "currentMessages") and config.multilineInput),
+            #multiline=Condition(lambda: config.multilineInput),
             default=default,
             accept_default=accept_default,
             completer=completer,
             is_password=is_password,
             mouse_support=Condition(lambda: config.mouseSupport),
             clipboard=config.clipboard,
         )
@@ -316,15 +192,15 @@
 
     @staticmethod
     def getPygmentsStyle():
         theme = config.pygments_style if hasattr(config, "pygments_style") and config.pygments_style else "stata-dark" if not config.terminalResourceLinkColor.startswith("ansibright") else "stata-light"
         return style_from_pygments_cls(get_style_by_name(theme))
 
     @staticmethod
-    def getLocalStorage():
+    def getFiles():
         apps = {
             "myhand": ("MyHand", "MyHand Bot"),
             "letmedoit": ("LetMeDoIt", "LetMeDoIt AI"),
             "taskwiz": ("TaskWiz", "TaskWiz AI"),
             "cybertask": ("CyberTask", "CyberTask AI"),
             "googleaistudio": ("GoogleAIStudio", "GoogleAIStudio"),
         }
@@ -372,16 +248,16 @@
             config.print2(splittedContent)
 
     @staticmethod
     def getEmbeddingFunction(embeddingModel=None):
         # import statement is placed here to make this file compatible on Android
         from chromadb.utils import embedding_functions
         embeddingModel = embeddingModel if embeddingModel is not None else config.embeddingModel
-        if embeddingModel in ("text-embedding-3-large", "text-embedding-3-small", "text-embedding-ada-002"):
-            return embedding_functions.OpenAIEmbeddingFunction(api_key=config.openaiApiKey, model_name=embeddingModel)
+        if embeddingModel == "text-embedding-ada-002":
+            return embedding_functions.OpenAIEmbeddingFunction(api_key=config.openaiApiKey, model_name="text-embedding-ada-002")
         return embedding_functions.SentenceTransformerEmbeddingFunction(model_name=embeddingModel) # support custom Sentence Transformer Embedding models by modifying config.embeddingModel
 
     @staticmethod
     def changeAPIkey():
         print("Enter your OpenAI API Key [required]:")
         apikey = prompt(default=config.openaiApiKey, is_password=True)
         if apikey and not apikey.strip().lower() in (config.cancel_entry, config.exit_entry):
@@ -402,14 +278,31 @@
         )
         # set variable 'OAI_CONFIG_LIST' to work with pyautogen
         oai_config_list = []
         for model in HealthCheck.models:
             oai_config_list.append({"model": model, "api_key": config.openaiApiKey})
         os.environ["OAI_CONFIG_LIST"] = json.dumps(oai_config_list)
 
+    @staticmethod
+    def saveConfig():
+        #print(configFile)
+        with open(configFile, "w", encoding="utf-8") as fileObj:
+            #print(dir(config))
+            for name in dir(config):
+                excludeConfigList = [
+                    "isTermux",
+                ]
+                if not name.startswith("__") and not name in excludeConfigList:
+                    try:
+                        value = eval(f"config.{name}")
+                        if not callable(value) and not str(value).startswith("<"):
+                            fileObj.write("{0} = {1}\n".format(name, pprint.pformat(value)))
+                    except:
+                        pass
+
     # The following method was modified from source:
     # https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     @staticmethod
     def count_tokens_from_messages(messages, model=""):
         if not model:
             model = config.chatGPTApiModel
 
@@ -417,16 +310,14 @@
         try:
             encoding = tiktoken.encoding_for_model(model)
         except KeyError:
             print("Warning: model not found. Using cl100k_base encoding.")
             encoding = tiktoken.get_encoding("cl100k_base")
         if model in {
                 "gpt-3.5-turbo",
-                "gpt-3.5-turbo-0125",
-                "gpt-3.5-turbo-1106",
                 "gpt-3.5-turbo-0613",
                 "gpt-3.5-turbo-16k",
                 "gpt-3.5-turbo-16k-0613",
                 "gpt-4-turbo-preview",
                 "gpt-4-0125-preview",
                 "gpt-4-1106-preview",
                 "gpt-4-0314",
```

### Comparing `letmedoit-2.1.84/letmedoit/icons/CyberTask.ico` & `letmedoit-2.1.9/letmedoit/icons/CyberTask.ico`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/icons/CyberTask.png` & `letmedoit-2.1.9/letmedoit/icons/CyberTask.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/icons/GeminiPro.ico` & `letmedoit-2.1.9/letmedoit/icons/GeminiPro.ico`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/icons/GeminiPro.png` & `letmedoit-2.1.9/letmedoit/icons/GeminiPro.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/icons/LetMeDoIt.ico` & `letmedoit-2.1.9/letmedoit/icons/LetMeDoIt.ico`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/icons/LetMeDoIt.png` & `letmedoit-2.1.9/letmedoit/icons/LetMeDoIt.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/icons/MyHand.ico` & `letmedoit-2.1.9/letmedoit/icons/MyHand.ico`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/icons/MyHand.png` & `letmedoit-2.1.9/letmedoit/icons/MyHand.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/icons/TaskWiz.ico` & `letmedoit-2.1.9/letmedoit/icons/TaskWiz.ico`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/icons/TaskWiz.png` & `letmedoit-2.1.9/letmedoit/icons/TaskWiz.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/icons/systemtray.ico` & `letmedoit-2.1.9/letmedoit/icons/systemtray.ico`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/icons/systemtray.png` & `letmedoit-2.1.9/letmedoit/icons/systemtray.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/Info.plist` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/QuickLook/Thumbnail.png` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/document.wflow` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/Info.plist` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/document.wflow` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/Info.plist` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/QuickLook/Thumbnail.png` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/document.wflow` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/Info.plist` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/document.wflow` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/Info.plist` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/document.wflow` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/Info.plist` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/QuickLook/Thumbnail.png` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/document.wflow` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/Info.plist` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/document.wflow` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/Info.plist` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/document.wflow` & `letmedoit-2.1.9/letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/main.py` & `letmedoit-2.1.9/letmedoit/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,21 +48,30 @@
 config.letMeDoItAIFolder = letMeDoItAIFolder
 config.isTermux = True if os.path.isdir("/data/data/com.termux/files/home") else False
 
 # package name
 with open(os.path.join(config.letMeDoItAIFolder, "package_name.txt"), "r", encoding="utf-8") as fileObj:
     package = fileObj.read()
 
+def getStorageDir():
+    storageDir = os.path.join(os.path.expanduser('~'), package)
+    try:
+        Path(storageDir).mkdir(parents=True, exist_ok=True)
+    except:
+        pass
+    return storageDir if os.path.isdir(storageDir) else ""
+config.getStorageDir = getStorageDir
+
 def restartApp():
     print(f"Restarting {config.letMeDoItName} ...")
     os.system(f"{sys.executable} {config.letMeDoItFile}")
     exit(0)
 config.restartApp = restartApp
 
-from letmedoit.utils.config_tools import *
+from letmedoit.utils.configDefault import *
 from letmedoit.utils.install import installmodule
 from letmedoit.utils.shared_utils import SharedUtil
 
 # automatic update
 config.pipIsUpdated = False
 def updateApp():
     thisPackage = f"{package}_android" if config.isTermux else package
@@ -100,14 +109,111 @@
     os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
     import pygame
     pygame.mixer.init()
     config.isPygameInstalled = True
 except:
     config.isPygameInstalled = False
 
+def setOsOpenCmd():
+    config.thisPlatform = thisPlatform
+    if config.terminalEnableTermuxAPI:
+        config.open = "termux-share"
+    elif thisPlatform == "Linux":
+        config.open = "xdg-open"
+    elif thisPlatform == "Darwin":
+        config.open = "open"
+    elif thisPlatform == "Windows":
+        config.open = "start"
+    # name macOS
+    if config.thisPlatform == "Darwin":
+        config.thisPlatform = "macOS"
+
+def saveConfig():
+    with open(configFile, "w", encoding="utf-8") as fileObj:
+        for name in dir(config):
+            excludeConfigList = [
+                "isTermux",
+                "oai_client",
+                "includeIpInSystemMessageTemp",
+                "initialCompletionCheck",
+                "promptStyle1",
+                "promptStyle2",
+                "runSpecificFuntion",
+                "pluginsWithFunctionCall",
+                "restartApp",
+                "getStorageDir",
+                "saveConfig",
+                "aliases",
+                "addPathAt",
+                "multilineInput",
+                "conversationStarted",
+                "dynamicToolBarText",
+                "tokenLimits",
+                "currentMessages",
+                "pagerContent",
+                "selectAll",
+                "clipboard",
+                "showKeyBindings",
+                "divider",
+                "systemCommandPromptEntry",
+                "stop_event",
+                "spinner_thread",
+                "tts",
+                "isPygameInstalled",
+                "isVlcPlayerInstalled",
+                "accept_default",
+                "defaultEntry",
+                "pipIsUpdated",
+                "setConfig",
+                "excludeConfigList",
+                "tempContent",
+                "tempChunk",
+                "predefinedContextTemp",
+                "thisPlatform",
+                "letMeDoItAI",
+                "terminalColors",
+                "letMeDoItFile",
+                "letMeDoItAIFolder",
+                "open",
+                "inputSuggestions", # used with plugins; user input suggestions
+                "chatGPTTransformers", # used with plugins; transform ChatGPT response message
+                "predefinedInstructions", # used with plugins; pre-defined instructions
+                "predefinedContexts", # used with plugins; pre-defined contexts
+                # used with plugins; function call
+                "execute_python_code_signature",
+                "execute_termux_command_signature",
+                "integrate_google_searches_signature",
+                "heal_python_signature",
+                "chatGPTApiFunctionSignatures",
+                "chatGPTApiAvailableFunctions",
+                "pythonFunctionResponse", # used with plugins; function call when function name is 'python'
+                # LetMeDoItAI methods shared from Class LetMeDoItAI
+                "getFiles",
+                "stopSpinning",
+                "toggleMultiline",
+                "print",
+                "print2",
+                "print3",
+                "getWrappedHTMLText",
+                "fineTuneUserInput",
+                "launchPager",
+                "addPagerText",
+                "getFunctionMessageAndResponse",
+                "isTermux",
+            ]
+            excludeConfigList = excludeConfigList + config.excludeConfigList
+            if not name.startswith("__") and not name in excludeConfigList:
+                try:
+                    value = eval(f"config.{name}")
+                    if not callable(value) and not str(value).startswith("<"):
+                        fileObj.write("{0} = {1}\n".format(name, pprint.pformat(value)))
+                except:
+                    pass
+config.saveConfig = saveConfig
+
 def set_log_file_max_lines(log_file, max_lines):
     if os.path.isfile(log_file):
         # Read the contents of the log file
         with open(log_file, "r", encoding="utf-8") as fileObj:
             lines = fileObj.readlines()
         # Count the number of lines in the file
         num_lines = len(lines)
@@ -202,29 +308,27 @@
         config.defaultEntry = args.default.strip()
         config.accept_default = False
     else:
         config.defaultEntry = ""
         config.accept_default = False
 
     set_title(config.letMeDoItName)
-    SharedUtil.setOsOpenCmd(thisPlatform)
+    setOsOpenCmd()
     createShortcuts()
     config.excludeConfigList = []
     config.isVlcPlayerInstalled = VlcUtil.isVlcPlayerInstalled()
-    # save loaded configs
-    config.saveConfig()
     # check log files; remove old lines if more than 3000 lines is found in a log file
     for i in ("chats", "paths", "commands"):
         filepath = os.path.join(config.historyParentFolder if config.historyParentFolder else config.letMeDoItAIFolder, "history", i)
         set_log_file_max_lines(filepath, 3000)
     LetMeDoItAI().startChats()
     # Do the following tasks before exit
     # backup configurations
-    config.saveConfig()
-    storageDir = SharedUtil.getLocalStorage()
+    saveConfig()
+    storageDir = getStorageDir()
     if os.path.isdir(storageDir):
         shutil.copy(configFile, os.path.join(storageDir, "config_backup.py"))
     # delete temporary content
     try:
         tempFolder = os.path.join(config.letMeDoItAIFolder, "temp")
         shutil.rmtree(tempFolder, ignore_errors=True)
         Path(tempFolder).mkdir(parents=True, exist_ok=True)
```

### Comparing `letmedoit-2.1.84/letmedoit/palm2.py` & `letmedoit-2.1.9/letmedoit/palm2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import vertexai, os, traceback, argparse, threading
 from vertexai.language_models import ChatModel, ChatMessage
 from letmedoit import config
 from letmedoit.utils.streaming_word_wrapper import StreamingWordWrapper
 from letmedoit.health_check import HealthCheck
-if not hasattr(config, "currentMessages"):
+if not hasattr(config, "exit_entry"):
     HealthCheck.setBasicConfig()
-    config.saveConfig()
-    #print("Configurations updated!")
+    HealthCheck.saveConfig()
+    print("Configurations updated!")
+HealthCheck.setPrint()
 from prompt_toolkit.styles import Style
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.shortcuts import clear
 from pathlib import Path
 
 
@@ -18,26 +19,28 @@
 #!pip install --upgrade google-cloud-aiplatform
 
 
 class Palm2:
 
     def __init__(self, name="PaLM 2"):
         # authentication
-        if os.environ["GOOGLE_APPLICATION_CREDENTIALS"] and "Vertex AI" in config.enabledGoogleAPIs:
+        authpath1 = os.path.join(HealthCheck.getFiles(), "credentials_googleaistudio.json")
+        if os.path.isfile(authpath1):
+            os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = authpath1
             self.runnable = True
         else:
-            print("Vertex AI is disabled!")
+            print(f"API key json file '{authpath1}' not found!")
             print("Read https://github.com/eliranwong/letmedoit/wiki/Google-API-Setup for setting up Google API.")
             self.runnable = False
         # initiation
         vertexai.init()
         self.name = name
 
     def run(self, prompt="", model="chat-bison-32k", temperature=0.0, max_output_tokens=2048):
-        historyFolder = os.path.join(HealthCheck.getLocalStorage(), "history")
+        historyFolder = os.path.join(HealthCheck.getFiles(), "history")
         Path(historyFolder).mkdir(parents=True, exist_ok=True)
         chat_history = os.path.join(historyFolder, self.name.replace(" ", "_"))
         chat_session = PromptSession(history=FileHistory(chat_history))
 
         promptStyle = Style.from_dict({
             # User input (default text).
             "": config.terminalCommandEntryColor2,
@@ -68,28 +71,28 @@
                 history = history[:-1]
             elif not history:
                 history = None
         else:
             history = None
         # start chat
         chat = model.start_chat(
-            context=config.systemMessage_palm2,
+            context=f"You're {self.name}, a helpful AI assistant.",
             message_history=history,
             #examples=[
             #    InputOutputTextPair(
             #        input_text="How many moons does Mars have?",
             #        output_text="The planet Mars has two moons, Phobos and Deimos.",
             #    ),
             #],
         )
         HealthCheck.print2(f"\n{self.name} loaded!")
         if hasattr(config, "currentMessages"):
-            bottom_toolbar = f""" {str(config.hotkey_exit).replace("'", "")} {config.exit_entry}"""
+            bottom_toolbar = f" [ctrl+q] {config.exit_entry}"
         else:
-            bottom_toolbar = f""" {str(config.hotkey_exit).replace("'", "")} {config.exit_entry} {str(config.hotkey_new).replace("'", "")} .new"""
+            bottom_toolbar = f" [ctrl+q] {config.exit_entry} [ctrl+n] .new"
             print("(To start a new chart, enter '.new')")
         print(f"(To exit, enter '{config.exit_entry}')\n")
         while True:
             if not prompt:
                 prompt = HealthCheck.simplePrompt(style=promptStyle, promptSession=chat_session, bottom_toolbar=bottom_toolbar)
                 if prompt and not prompt in (".new", config.exit_entry) and hasattr(config, "currentMessages"):
                     config.currentMessages.append({"content": prompt, "role": "user"})
@@ -122,15 +125,15 @@
                     self.streaming_thread.join()
                     HealthCheck.print2(traceback.format_exc())
 
             prompt = ""
 
         HealthCheck.print2(f"\n{self.name} closed!")
         if hasattr(config, "currentMessages"):
-            HealthCheck.print2(f"Return back to {config.letMeDoItName} prompt ...")
+            HealthCheck.print2(f"Going back to {config.letMeDoItName} prompt ...")
 
 def main():
     # Create the parser
     parser = argparse.ArgumentParser(description="palm2 cli options")
     # Add arguments
     parser.add_argument("default", nargs="?", default=None, help="default entry")
     parser.add_argument('-m', '--model', action='store', dest='model', help="specify language model with -m flag; default: chat-bison-32k")
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/add calendar event.py` & `letmedoit-2.1.9/letmedoit/plugins/add calendar event.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,21 +119,14 @@
         return link
 
     SharedUtil.openURL(getOutlookLink() if calendar == "outlook" else getGoogleLink())
 
     return "Done!"
 
 functionSignature = {
-    "intent": [
-        "arrange activities",
-        "access to internet real-time information",
-    ],
-    "examples": [
-        "Add a calender event",
-    ],
     "name": "add_calendar_event",
     "description": "add calendar event",
     "parameters": {
         "type": "object",
         "properties": {
             "calendar": {
                 "type": "string",
@@ -165,8 +158,10 @@
                 "description": "The location or venue of the event.",
             },
         },
         "required": ["calendar", "title", "description", "start_time", "end_time"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=add_calendar_event)
+config.pluginsWithFunctionCall.append("add_calendar_event")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["add_calendar_event"] = add_calendar_event
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/analyze files.py` & `letmedoit-2.1.9/letmedoit/plugins/analyze files.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,28 +34,22 @@
                 "query": query,
                 "files": [files],
             }
             config.print3("Running function: 'analyze_images'")
             return config.chatGPTApiAvailableFunctions["analyze_images"](function_args)
         config.stopSpinning()
         config.print2("AutoGen Retriever launched!")
-        last_message = AutoGenRetriever().getResponse(files, query, True)
+        last_message = AutoGenRetriever().getResponse(files, query)
         config.currentMessages += last_message
         config.print2("AutoGen Retriever closed!")
         return ""
 
     return "[INVALID]"
 
 functionSignature = {
-    "intent": [
-        "analyze files",
-    ],
-    "examples": [
-        "analyze files",
-    ],
     "name": "analyze_files",
     "description": "retrieve information from files",
     "parameters": {
         "type": "object",
         "properties": {
             "query": {
                 "type": "string",
@@ -66,8 +60,10 @@
                 "description": """Return a directory or non-image file path. Return an empty string '' if it is not given.""",
             },
         },
         "required": ["query", "files"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=analyze_files)
+config.pluginsWithFunctionCall.append("analyze_files")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["analyze_files"] = analyze_files
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/analyze images with gemini.py` & `letmedoit-2.1.9/letmedoit/plugins/analyze images with gemini.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,20 +14,14 @@
 def analyze_images_with_gemini(function_args):
     answer = GeminiProVision(temperature=config.llmTemperature).analyze_images(function_args)
     if answer:
         config.tempContent = answer
     return "[INVALID]" if not answer else ""
 
 functionSignature = {
-    "intent": [
-        "analyze files",
-    ],
-    "examples": [
-        "analyze image with Gemini",
-    ],
     "name": "analyze_images_with_gemini",
     "description": "Use Gemini Pro Vision to describe or analyze images",
     "parameters": {
         "type": "object",
         "properties": {
             "query": {
                 "type": "string",
@@ -38,9 +32,11 @@
                 "description": """Return a list of image paths or urls, e.g. '["image1.png", "/tmp/image2.png", "https://letmedoit.ai/image.png"]'. Return '[]' if image path is not provided.""",
             },
         },
         "required": ["query", "files"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=analyze_images_with_gemini)
+config.pluginsWithFunctionCall.append("analyze_images_with_gemini")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["analyze_images_with_gemini"] = analyze_images_with_gemini
 config.inputSuggestions.append("Ask Gemini Pro Vision to describe this image in detail: ")
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/analyze web content.py` & `letmedoit-2.1.9/letmedoit/plugins/analyze web content.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,21 +35,14 @@
     last_message = AutoGenRetriever().getResponse(filename, query)
     config.currentMessages += last_message
     config.print2("AutoGen Retriever closed!")
 
     return ""
 
 functionSignature = {
-    "intent": [
-        "analyze files",
-        "access to internet real-time information",
-    ],
-    "examples": [
-        "summarize this webpage",
-    ],
     "name": "analyze_web_content",
     "description": "retrieve information from a webpage if an url is provided",
     "parameters": {
         "type": "object",
         "properties": {
             "query": {
                 "type": "string",
@@ -60,8 +53,10 @@
                 "description": """Return the given url. Return an empty string '' if it is not given.""",
             },
         },
         "required": ["query", "url"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=analyze_web_content)
+config.pluginsWithFunctionCall.append("analyze_web_content")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["analyze_web_content"] = analyze_web_content
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/ask chatgpt.py` & `letmedoit-2.1.9/letmedoit/plugins/ask palm2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 """
-LetMeDoIt AI Plugin - ask chatgpt
+LetMeDoIt AI Plugin - ask PaLM 2
 
-Ask ChatGPT for conversation only; no function calling
+Ask Google PaLM 2 for information
 
 [FUNCTION_CALL]
 """
 
 
 from letmedoit import config
-from letmedoit.chatgpt import ChatGPT
+from letmedoit.palm2 import Palm2
 
-def ask_chatgpt(function_args):
-    config.stopSpinning()
+def ask_palm2(function_args):
     query = function_args.get("query") # required
-    config.currentMessages = config.currentMessages[:-1]
-    ChatGPT().run(query)
+    config.stopSpinning()
+    Palm2().run(query, temperature=config.llmTemperature)
     return ""
 
 functionSignature = {
-    "intent": [
-        "ask a chatbot",
-    ],
-    "examples": [
-        "Ask ChatGPT about",
-    ],
-    "name": "ask_chatgpt",
-    "description": "Ask ChatGPT to chat or provide information",
+    "name": "ask_palm2",
+    "description": "Ask PaLM 2 to chat or provide information",
     "parameters": {
         "type": "object",
         "properties": {
             "query": {
                 "type": "string",
-                "description": "The original request in detail, including any supplementary information",
+                "description": "The request in detail, including any supplementary information",
             },
         },
         "required": ["query"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=ask_chatgpt)
-config.inputSuggestions.append("Ask ChatGPT: ")
+config.pluginsWithFunctionCall.append("ask_palm2")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["ask_palm2"] = ask_palm2
+config.inputSuggestions.append("Ask PaLM 2: ")
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/ask codey.py` & `letmedoit-2.1.9/letmedoit/plugins/ask codey.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,29 +13,25 @@
 def ask_codey(function_args):
     query = function_args.get("query") # required
     config.stopSpinning()
     Codey().run(query, temperature=config.llmTemperature)
     return ""
 
 functionSignature = {
-    "intent": [
-        "ask a chatbot",
-    ],
-    "examples": [
-        "Ask Codey about",
-    ],
     "name": "ask_codey",
     "description": "Ask Codey for information about coding",
     "parameters": {
         "type": "object",
         "properties": {
             "query": {
                 "type": "string",
                 "description": "The request in detail, including any supplementary information",
             },
         },
         "required": ["query"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=ask_codey)
+config.pluginsWithFunctionCall.append("ask_codey")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["ask_codey"] = ask_codey
 config.inputSuggestions.append("Ask Codey: ")
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/ask gemini pro.py` & `letmedoit-2.1.9/letmedoit/plugins/ask gemini pro.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,29 +13,25 @@
 def ask_gemini_pro(function_args):
     config.stopSpinning()
     query = function_args.get("query") # required
     GeminiPro(temperature=config.llmTemperature).run(query)
     return ""
 
 functionSignature = {
-    "intent": [
-        "ask a chatbot",
-    ],
-    "examples": [
-        "Ask Gemini about",
-    ],
     "name": "ask_gemini_pro",
     "description": "Ask Gemini Pro to chat or provide information",
     "parameters": {
         "type": "object",
         "properties": {
             "query": {
                 "type": "string",
                 "description": "The original request in detail, including any supplementary information",
             },
         },
         "required": ["query"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=ask_gemini_pro)
+config.pluginsWithFunctionCall.append("ask_gemini_pro")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["ask_gemini_pro"] = ask_gemini_pro
 config.inputSuggestions.append("Ask Gemini Pro: ")
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/ask mistral.py` & `letmedoit-2.1.9/letmedoit/plugins/solve math problems.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 """
-LetMeDoIt AI Plugin - ask Mistral
+LetMeDoIt AI Plugin - solve math problems
 
-Ask Mistral for information
+solve math problems with integrated "AutoGen Math Solver"
 
 [FUNCTION_CALL]
 """
 
 
 from letmedoit import config
-from letmedoit.ollamachat import OllamaChat
+from letmedoit.automath import AutoGenMath
 
-def ask_mistral(function_args):
+def solve_math(function_args):
     query = function_args.get("query") # required
     config.stopSpinning()
-    OllamaChat().run(query, model="mistral")
+    config.print2("AutoGen Math Solver launched!")
+    last_message = AutoGenMath().getResponse(query)
+    config.currentMessages += last_message
+    config.print2("AutoGen Math Solver closed!")
     return ""
 
 functionSignature = {
-    "intent": [
-        "ask a chatbot",
-    ],
-    "examples": [
-        "Ask Mistral about",
-    ],
-    "name": "ask_mistral",
-    "description": "Ask Mistral to chat or provide information",
+    "name": "solve_math",
+    "description": "solve math problems",
     "parameters": {
         "type": "object",
         "properties": {
             "query": {
                 "type": "string",
-                "description": "The request in detail, including any supplementary information",
+                "description": "Math problem in detail",
             },
         },
         "required": ["query"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=ask_mistral)
-config.inputSuggestions.append("Ask Mistral: ")
+config.pluginsWithFunctionCall.append("solve_math")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["solve_math"] = solve_math
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/ask palm2.py` & `letmedoit-2.1.9/letmedoit/plugins/dates and times.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 """
-LetMeDoIt AI Plugin - ask PaLM 2
+LetMeDoIt AI Plugin - dates and times
 
-Ask Google PaLM 2 for information
+Retrieve information about dates and times
 
 [FUNCTION_CALL]
 """
 
-
 from letmedoit import config
-from letmedoit.palm2 import Palm2
+from letmedoit.utils.shared_utils import SharedUtil
 
-def ask_palm2(function_args):
-    query = function_args.get("query") # required
-    config.stopSpinning()
-    Palm2().run(query, temperature=config.llmTemperature)
-    return ""
+def datetimes(function_args):
+    code = function_args.get("code") # required
+    information = SharedUtil.showAndExecutePythonCode(code)
+    return information
 
 functionSignature = {
-    "intent": [
-        "ask a chatbot",
-    ],
-    "examples": [
-        "Ask PaLM about",
-    ],
-    "name": "ask_palm2",
-    "description": "Ask PaLM 2 to chat or provide information",
+    "name": "datetimes",
+    "description": f'''Get information about dates and times''',
     "parameters": {
         "type": "object",
         "properties": {
-            "query": {
+            "code": {
                 "type": "string",
-                "description": "The request in detail, including any supplementary information",
+                "description": "Python code that integrates package pendulum to resolve my query",
             },
         },
-        "required": ["query"],
+        "required": ["code"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=ask_palm2)
-config.inputSuggestions.append("Ask PaLM 2: ")
+config.pluginsWithFunctionCall.append("datetimes")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["datetimes"] = datetimes
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/auto heal python code.py` & `letmedoit-2.1.9/letmedoit/plugins/auto heal python code.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,20 +36,14 @@
             SharedUtil.displayPythonCode(fix)
         exec(SharedUtil.fineTunePythonCode(fix), globals())
         return "EXECUTED"
     except:
         return traceback.format_exc()
 
 functionSignature = {
-    "intent": [
-        "generate code",
-    ],
-    "examples": [
-        "Fix python code",
-    ],
     "name": "heal_python",
     "description": "Fix python code if both original code and traceback error are provided",
     "parameters": {
         "type": "object",
         "properties": {
             "fix": {
                 "type": "string",
@@ -71,8 +65,11 @@
 # configs particular to this plugin
 # persistent
 persistentConfigs = (
     ("max_consecutive_auto_heal", 5),
 )
 config.setConfig(persistentConfigs)
 
-config.addFunctionCall(signature=functionSignature, method=heal_python)
+config.pluginsWithFunctionCall.append("heal_python")
+config.heal_python_signature = [functionSignature]
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["heal_python"] = heal_python
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/awesome prompts.py` & `letmedoit-2.1.9/letmedoit/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/plugins/character analysis.py` & `letmedoit-2.1.9/letmedoit/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/plugins/contexts.py` & `letmedoit-2.1.9/letmedoit/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/plugins/counselling.py` & `letmedoit-2.1.9/letmedoit/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/plugins/create ai assistants.py` & `letmedoit-2.1.9/letmedoit/plugins/create ai assistants.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,22 +21,14 @@
         del messages[-1]
     # add context to the message chain
     config.currentMessages += messages
     config.print2("\nAutoGen Agent Builder closed!")
     return ""
 
 functionSignature = {
-    "intent": [
-        "ask an auto assistant",
-        "create content",
-    ],
-    "examples": [
-        "Ask autobuilder to",
-        "Create a team of agents / assistants to",
-    ],
     "name": "build_agents",
     "description": "build a group of AI assistants or agents to execute a complicated task that other functions cannot resolve",
     "parameters": {
         "type": "object",
         "properties": {
             "task": {
                 "type": "string",
@@ -47,8 +39,10 @@
                 "description": "A short title to describe the task",
             },
         },
         "required": ["task", "title"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=build_agents)
+config.pluginsWithFunctionCall.append("build_agents")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["build_agents"] = build_agents
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/create maps.py` & `letmedoit-2.1.9/letmedoit/plugins/create maps.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,28 +20,24 @@
         os.system(f"{config.open} {htmlFile}")
         return f"Saved as '{htmlFile}'"
     elif information:
         return information
     return ""
 
 functionSignature = {
-    "intent": [
-        "create content",
-    ],
-    "examples": [
-        "Create a map",
-    ],
     "name": "create_map",
     "description": f'''Create maps''',
     "parameters": {
         "type": "object",
         "properties": {
             "code": {
                 "type": "string",
                 "description": "Python code that integrates package folium to resolve my request. Created maps are saved in html format",
             },
         },
         "required": ["code"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=create_map)
+config.pluginsWithFunctionCall.append("create_map")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["create_map"] = create_map
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/create qrcode.py` & `letmedoit-2.1.9/letmedoit/plugins/create qrcode.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,28 +20,24 @@
             try:
                 os.system(f'''{config.open} "{filepath}"''')
             except:
                 pass
     return ""
 
 functionSignature = {
-    "intent": [
-        "create content",
-    ],
-    "examples": [
-        "Create a QR code",
-    ],
     "name": "create_qrcode",
     "description": f'''Create QR code''',
     "parameters": {
         "type": "object",
         "properties": {
             "code": {
                 "type": "string",
                 "description": "Python code that integrates package qrcode to resolve my request. Always save the qr code image in png format and use 'print' function to print its full path only, without additional description or comment, in the last line of your code.",
             },
         },
         "required": ["code"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=create_qrcode)
+config.pluginsWithFunctionCall.append("create_qrcode")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["create_qrcode"] = create_qrcode
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/download youtube or web content.py` & `letmedoit-2.1.9/letmedoit/plugins/download youtube or web content.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,42 +49,34 @@
 
     url = function_args.get("url") # required
     if is_youtube_url(url):
         config.print("Loading youtube downloader ...")
         format = function_args.get("format") # required
         location = function_args.get("location", "") # optional
         if not (location and os.path.isdir(location)):
-            location = os.path.join(config.getLocalStorage(), "audio" if format == "audio" else "video")
+            location = os.path.join(config.getFiles(), "audio" if format == "audio" else "video")
             Path(location).mkdir(parents=True, exist_ok=True)
         downloadCommand = "yt-dlp -x --audio-format mp3" if format == "audio" else "yt-dlp -f bestvideo[ext=mp4]+bestaudio[ext=m4a]/mp4"
         terminalDownloadYoutubeFile(downloadCommand, url, location)
         return "Finished! Youtube downloader closed!"
     elif SharedUtil.is_valid_url(url):
         try:
-            folder = config.getLocalStorage()
+            folder = config.getFiles()
             folder = os.path.join(folder, "Downloads")
             Path(folder).mkdir(parents=True, exist_ok=True)
             SharedUtil.downloadWebContent(url, folder=folder, ignoreKind=True)
             return "Downloaded!"
         except:
             SharedUtil.showErrors()
             return "[INVALID]"
     else:
         config.print("invalid link given")
         return "[INVALID]"
 
 functionSignature = {
-    "intent": [
-        "access to internet real-time information",
-    ],
-    "examples": [
-        "Download Youtube video",
-        "Download Youtube audio into mp3 format",
-        "Download this webpage",
-    ],
     "name": "download_web_content",
     "description": "download Youtube video into mp4 file or download audio into mp3 file or download webcontent",
     "parameters": {
         "type": "object",
         "properties": {
             "url": {
                 "type": "string",
@@ -100,8 +92,10 @@
                 "description": "Output folder where downloaded file is to be saved",
             },
         },
         "required": ["url", "format"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=download_web_content)
+config.pluginsWithFunctionCall.append("download_web_content")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["download_web_content"] = download_web_content
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/edit text.py` & `letmedoit-2.1.9/letmedoit/plugins/edit text.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,28 +33,24 @@
     else:
         command = f"{customTextEditor} {filename}" if filename else customTextEditor
         config.stopSpinning()
         os.system(command)
         return "Finished! Text editor closed!"
 
 functionSignature = {
-    "intent": [
-        "change files",
-    ],
-    "examples": [
-        "Edit test.txt",
-    ],
     "name": "edit_text",
     "description": f'''Edit text files with extensions: '*.{"', '*.".join(config.textFileExtensions)}'.''',
     "parameters": {
         "type": "object",
         "properties": {
             "filename": {
                 "type": "string",
                 "description": "Text file path given by user. Return an empty string if not given.",
             },
         },
         "required": ["filename"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=edit_text)
+config.pluginsWithFunctionCall.append("edit_text")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["edit_text"] = edit_text
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/global finance.py` & `letmedoit-2.1.9/letmedoit/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/plugins/improve British English.py` & `letmedoit-2.1.9/letmedoit/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/plugins/input suggestions.py` & `letmedoit-2.1.9/letmedoit/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/plugins/integrate google searches.py` & `letmedoit-2.1.9/letmedoit/plugins/integrate google searches.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,28 +28,25 @@
         }
 
     config.print("Loaded!\n")
 
     return json.dumps(info)
 
 functionSignature = {
-    "intent": [
-        "access to internet real-time information",
-    ],
-    "examples": [
-        "Search internet",
-    ],
     "name": "integrate_google_searches",
     "description": "Search internet for keywords when ChatGPT lacks information or when user ask about latest updates",
     "parameters": {
         "type": "object",
         "properties": {
             "keywords": {
                 "type": "string",
                 "description": "keywords for searches, e.g. ChatGPT",
             },
         },
         "required": ["keywords"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=integrate_google_searches)
+config.pluginsWithFunctionCall.append("integrate_google_searches")
+config.integrate_google_searches_signature = [functionSignature]
+config.chatGPTApiFunctionSignatures.insert(0, functionSignature)
+config.chatGPTApiAvailableFunctions["integrate_google_searches"] = integrate_google_searches
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/manipulate files.py` & `letmedoit-2.1.9/letmedoit/plugins/manipulate files.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,28 +13,24 @@
 import re, os
 
 def manipulate_files(function_args):
     code = function_args.get("code") # required
     return SharedUtil.showAndExecutePythonCode(code)
 
 functionSignature = {
-    "intent": [
-        "change files",
-    ],
-    "examples": [
-        "Edit test.txt",
-    ],
     "name": "manipulate_files",
     "description": f'''Manipulate files, such as opening, launching, navigation, renaming, editing, removal, conversion, etc.''',
     "parameters": {
         "type": "object",
         "properties": {
             "code": {
                 "type": "string",
                 "description": "Python code that integrates any relevant packages to resolve my request",
             },
         },
         "required": ["code"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=manipulate_files)
+config.pluginsWithFunctionCall.append("manipulate_files")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["manipulate_files"] = manipulate_files
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/memory.py` & `letmedoit-2.1.9/letmedoit/plugins/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,15 @@
 
 from letmedoit import config
 from letmedoit.health_check import HealthCheck
 from pathlib import Path
 from chromadb.config import Settings
 import uuid, os, chromadb, getpass, geocoder, datetime, json
 
-persistentConfigs = (
-    ("memory_categories", ["general", "instruction", "fact", "event", "concept"]),
-)
-config.setConfig(persistentConfigs)
-
-memory_store = os.path.join(config.getLocalStorage(), "memory")
+memory_store = os.path.join(config.getFiles(), "memory")
 Path(memory_store).mkdir(parents=True, exist_ok=True)
 chroma_client = chromadb.PersistentClient(memory_store, Settings(anonymized_telemetry=False))
 
 #import numpy as np
 #from numpy.linalg import norm
 #def cosine_similarity(A, B):
 #    cosine = np.dot(A, B) / (norm(A) * norm(B))
@@ -47,15 +42,14 @@
 
 def save_memory(function_args):
     memory = function_args.get("memory") # required
     memory_title = function_args.get("title") # required
     memory_type = function_args.get("type") # required
     memory_tags = function_args.get("tags") # required
     if not isinstance(memory_tags, str):
-        print(type(memory_tags), memory_tags)
         memory_tags = str(memory_tags)
     collection = get_or_create_collection("memories")
     g = geocoder.ip('me')
     metadata = {
         "timestamp": str(datetime.datetime.now()),
         "tags": memory_tags,
         "title": memory_title,
@@ -77,15 +71,15 @@
     #query_embedding = get_embedding(query)
     return collection.query(
         #query_embeddings = [query_embedding],
         query_texts=[query],
         n_results = n,
     )
 
-def retrieve_memory(function_args):
+def retrieve_memories(function_args):
     query = function_args.get("query") # required
     collection = get_or_create_collection("memories")
     res = query_vectors(collection, query, config.memoryClosestMatches)
     if config.developer:
         config.print(config.divider)
         print(">>> retrieved memories: ") 
         print(res["documents"])
@@ -95,65 +89,52 @@
         info[f"memory {index}"] = {
             "description": description,
         }
     config.stopSpinning()
     return json.dumps(info)
 
 functionSignature1 = {
-    "intent": [
-        "memory / record access",
-        "arrange activities",
-    ],
-    "examples": [
-        "Remember that",
-    ],
     "name": "save_memory",
     "description": """Use this function if I mention something which you think would be useful in the future and should be saved as a memory. Saved memories will allow you to retrieve snippets of past conversations when needed.""",
     "parameters": {
         "type": "object",
         "properties": {
             "memory": {
                 "type": "string",
-                "description": "Full description of the memory to be saved. I would like you to help me with converting relative dates and times, if any, into exact dates and times based on the given current date and time.",
+                "description": "Full description of the memory to be saved. I would like you to help me with converting relative dates and times, if any, into exact dates and times based on the given current date and time."
             },
             "title": {
                 "type": "string",
-                "description": "Title of the memory",
+                "description": "Title of the memory"
             },
             "type": {
                 "type": "string",
-                "description": "Type of the memory, return either 'general', 'instruction', 'fact', 'event', or 'concept'",
-                "enum": config.memory_categories,
+                "description": "Type of the memory, return either 'general', 'instruction', 'fact', 'event', or 'concept'"
             },
             "tags": {
                 "type": "string",
-                "description": """Return a list of tags about the memory, e.g. '["work", "to_do", "follow_up"]'""",
+                "description": """Return a list of tags about the memory, e.g. '["work", "to_do", "follow_up"]'"""
             },
         },
         "required": ["memory", "title", "type", "tags"]
     }
 }
 functionSignature2 = {
-    "intent": [
-        "memory / record access",
-        "arrange activities",
-    ],
-    "examples": [
-        "Do you remember that",
-    ],
-    "name": "retrieve_memory",
+    "name": "retrieve_memories",
     "description": """Use this function to query and retrieve memories of important conversation snippets that we had in the past. Use this function if the information you require is not in the current prompt or you need additional information to refresh your memory.""",
     "parameters": {
         "type": "object",
         "properties": {
             "query": {
                 "type": "string",
                 "description": "The query to be used to look up memories from a vector database"
             },
         },
         "required": ["query"]
     }
 }
 
 config.inputSuggestions += ["Remember, ", "Do you remember?"]
-config.addFunctionCall(signature=functionSignature1, method=save_memory)
-config.addFunctionCall(signature=functionSignature2, method=retrieve_memory)
+config.pluginsWithFunctionCall += ["save_memory", "retrieve_memories"]
+config.chatGPTApiFunctionSignatures += [functionSignature1, functionSignature2]
+config.chatGPTApiAvailableFunctions["save_memory"] = save_memory
+config.chatGPTApiAvailableFunctions["retrieve_memories"] = retrieve_memories
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/open web browser.py` & `letmedoit-2.1.9/letmedoit/plugins/open web browser.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,22 +14,14 @@
     url = function_args.get("url") # required
     if url:
         SharedUtil.openURL(url)
     return ""
 
 # Function Signature
 functionSignature = {
-    "intent": [
-        "access to internet real-time information",
-    ],
-    "examples": [
-        "Open web browser",
-        "Open website",
-        "Open https://letmedoit.ai",
-    ],
     "name": "open_browser",
     "description": f'''Open an url with default web browser''',
     "parameters": {
         "type": "object",
         "properties": {
             "url": {
                 "type": "string",
@@ -37,9 +29,11 @@
             },
         },
         "required": ["url"],
     },
 }
 
 # Integrate the signature and method into LetMeDoIt AI
-config.addFunctionCall(signature=functionSignature, method=open_browser)
+config.pluginsWithFunctionCall.append("open_browser")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["open_browser"] = open_browser
 config.inputSuggestions.append("Open url: ")
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/pronounce words.py` & `letmedoit-2.1.9/letmedoit/plugins/pronounce words.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,20 +22,14 @@
     words = function_args.get("words") # required
     language = function_args.get("language") # required
     config.print("Loading speech feature ...")
     TTSUtil.play(words, language)
     return "Finished! Speech engine closed!"
 
 functionSignature = {
-    "intent": [
-        "interact with user",
-    ],
-    "examples": [
-        "Pronunce",
-    ],
     "name": "pronunce_words",
     "description": "pronounce words or sentences",
     "parameters": {
         "type": "object",
         "properties": {
             "words": {
                 "type": "string",
@@ -47,9 +41,11 @@
                 "enum": config.ttsLanguages,
             },
         },
         "required": ["words", "language"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=pronunce_words)
+config.pluginsWithFunctionCall.append("pronunce_words")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["pronunce_words"] = pronunce_words
 config.inputSuggestions.append("pronunce ")
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/remove image background.py` & `letmedoit-2.1.9/letmedoit/plugins/remove image background.py`

 * *Files 26% similar despite different names*

```diff
@@ -51,28 +51,24 @@
             try:
                 os.system(f'''{config.open} "{filepath}"''')
             except:
                 pass
     return ""
 
 functionSignature = {
-    "intent": [
-        "change files",
-    ],
-    "examples": [
-        "Remove image background",
-    ],
     "name": "remove_image_background",
     "description": f'''Remove image background''',
     "parameters": {
         "type": "object",
         "properties": {
             "files": {
                 "type": "string",
                 "description": """Return a list of image paths, e.g. '["image1.png", "/tmp/image2.png"]'. Return '[]' if image path is not provided.""",
             },
         },
         "required": ["files"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=remove_image_background)
+config.pluginsWithFunctionCall.append("remove_image_background")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["remove_image_background"] = remove_image_background
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/search chat records.py` & `letmedoit-2.1.9/letmedoit/plugins/search chat records.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from letmedoit.health_check import HealthCheck
 from pathlib import Path
 from chromadb.config import Settings
 import uuid, os, chromadb, re
 from letmedoit.utils.shared_utils import SharedUtil
 from prompt_toolkit import print_formatted_text, HTML
 
-chat_store = os.path.join(config.getLocalStorage(), "chats")
+chat_store = os.path.join(config.getFiles(), "chats")
 Path(chat_store).mkdir(parents=True, exist_ok=True)
 chroma_client = chromadb.PersistentClient(chat_store, Settings(anonymized_telemetry=False))
 
 def get_or_create_collection(collection_name):
     collection = chroma_client.get_or_create_collection(
         name=collection_name,
         metadata={"hnsw:space": "cosine"},
@@ -82,15 +82,15 @@
 
     def validateChatFile(chatFile):
         chatFile = os.path.expanduser(chatFile)
         if os.path.isfile(chatFile):
             isfile = True
         elif re.search("^[0-9][0-9][0-9][0-9]-[0-9][0-9]-[0-9][0-9]_[0-9][0-9]_[0-9][0-9]_[0-9][0-9]$", chatFile):
             # match chat id format
-            folderPath = os.path.join(config.getLocalStorage(), "chats", re.sub("^([0-9]+?\-[0-9]+?)\-.*?$", r"\1", chatFile))
+            folderPath = os.path.join(config.getFiles(), "chats", re.sub("^([0-9]+?\-[0-9]+?)\-.*?$", r"\1", chatFile))
             chatFile = os.path.join(folderPath, f"{chatFile}.txt")
             if os.path.isfile(chatFile):
                 isfile = True
             else:
                 isfile = False
         else:
             isfile = False
@@ -128,20 +128,14 @@
             config.print3(f"Failed to load chat records '{timestamp}' due to invalid format!")
     except:
         config.print3(f"Failed to load chat records: {timestamp}\n")
         SharedUtil.showErrors()
     return "[INVALID]"
 
 functionSignature1 = {
-    "intent": [
-        "memory / record access",
-    ],
-    "examples": [
-        "Save chat record",
-    ],
     "name": "search_chats",
     "description": """Search chat records""",
     "parameters": {
         "type": "object",
         "properties": {
             "query": {
                 "type": "string",
@@ -149,20 +143,14 @@
             },
         },
         "required": ["query"]
     }
 }
 
 functionSignature2 = {
-    "intent": [
-        "memory / record access",
-    ],
-    "examples": [
-        "Load chat record",
-    ],
     "name": "load_chats",
     "description": """Load or open old saved chat records if chat ID / timestamp / file path is given""",
     "parameters": {
         "type": "object",
         "properties": {
             "id": {
                 "type": "string",
@@ -170,9 +158,11 @@
             },
         },
         "required": ["id"]
     }
 }
 
 config.inputSuggestions += ["Search chat records: ", "Load chat records with this ID: ", "Load chat records in this file: "]
-config.addFunctionCall(signature=functionSignature1, method=search_chats)
-config.addFunctionCall(signature=functionSignature2, method=load_chats)
+config.pluginsWithFunctionCall += ["search_chats", "load_chats"]
+config.chatGPTApiFunctionSignatures += [functionSignature1, functionSignature2]
+config.chatGPTApiAvailableFunctions["search_chats"] = search_chats
+config.chatGPTApiAvailableFunctions["load_chats"] = load_chats
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/search financial data.py` & `letmedoit-2.1.9/letmedoit/plugins/search financial data.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,28 +17,24 @@
         info = {
             "information": information,
         }
         return json.dumps(info)
     return ""
 
 functionSignature = {
-    "intent": [
-        "access to internet real-time information",
-    ],
-    "examples": [
-        "Check stock price",
-    ],
     "name": "search_finance",
     "description": f'''Search or analyze financial data. Use this function ONLY WHEN package yfinance is useful to resolve my request''',
     "parameters": {
         "type": "object",
         "properties": {
             "code": {
                 "type": "string",
                 "description": "Python code that integrates package yfinance to resolve my request. Integrate package matplotlib to visualize data, if applicable.",
             },
         },
         "required": ["code"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=search_finance)
+config.pluginsWithFunctionCall.append("search_finance")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["search_finance"] = search_finance
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/search latest news.py` & `letmedoit-2.1.9/letmedoit/plugins/search latest news.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 search latest news
 
 [FUNCTION_CALL]
 """
 
 from letmedoit import config
-import feedparser, re
+import feedparser
 
 # Function method to get the latest news from a specific RSS feed
 def search_latest_news(function_args: dict) -> str:
-    keywords = function_args.get("keywords").replace(" ", "+")
+    keywords = function_args.get("keywords")
     feed_url = f"https://news.google.com/rss/search?q={keywords}&hl=en-US&gl=US&ceid=US:en"
     feed = feedparser.parse(feed_url)
 
     # Print the title and link of each news item
     config.stopSpinning()
     config.print2(config.divider)
     for index, entry in enumerate(feed.entries):
@@ -29,32 +29,32 @@
             link = re.sub("<[^<>]*?>", "", entry.link)
             config.print3(f"Link: {link}")
     config.print2(config.divider)
     return ""
 
 # Function signature to work with ChatGPT function calling
 functionSignature = {
-    "intent": [
-        "access to internet real-time information",
-    ],
-    "examples": [
-        "Tell me latest news about",
-    ],
     "name": "search_latest_news",
     "description": "Search the latest news with given keywords",
     "parameters": {
         "type": "object",
         "properties": {
             "keywords": {
                 "type": "string",
                 "description": "The keywords for searching the latest news, delimited by plus sign '+'.  For example, return 'London+UK' if keywords are 'London' and 'UK'.",
             },
         },
         "required": ["keywords"],
     },
 }
 
-# The following line integrate the function method and signature into LetMeDoIt AI
-config.addFunctionCall(signature=functionSignature, method=search_latest_news)
+# Add the following line to tell LetMeDoIt AI that this plugin work with function calling feature.
+config.pluginsWithFunctionCall.append("search_latest_news")
+
+# The following line adds the function signature, that we prepared in STEP 3, to the full list of all function signatures that work with LetMeDoIt AI.
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+
+# The following line tells LetMeDoIt AI to call the method "search_latest_news" that we added in this plugin when the function signature "search_latest_news" is loaded.
+config.chatGPTApiAvailableFunctions["search_latest_news"] = search_latest_news
 
 # The following line is optional. It adds an input suggestion to LetMeDoIt AI user input prompt
 config.inputSuggestions.append("Tell me the latest news about ")
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/search sqlite.py` & `letmedoit-2.1.9/letmedoit/plugins/ask sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [FUNCTION_CALL]
 """
 
 from letmedoit import config
 from letmedoit.utils.shared_utils import SharedUtil
 import os, sqlite3, json, pprint
 
-def search_sqlite(function_args):
+def ask_sqlite(function_args):
     db = function_args.get("path") # required
     request = function_args.get("request") # required
     if not os.path.isfile(db):
         return "[INVALID]"
     try:
         info = {}
         config.print2("Reading table information ...")
@@ -55,30 +55,22 @@
 
         userInput = f"""Connect this sqlite file: sqlite file: {db}
 
 And run python code to resolve my request: {request}
 
 Please consider individual table information below for code generation:
 {info}"""
-        _, function_call_response = SharedUtil.getSingleFunctionResponse(userInput, [config.chatGPTApiFunctionSignatures["execute_python_code"]], "execute_python_code")
+        _, function_call_response = SharedUtil.getSingleFunctionResponse(userInput, config.execute_python_code_signature, "execute_python_code")
         return function_call_response
     except:
         SharedUtil.showErrors()
         return "[INVALID]"
 
 functionSignature = {
-    "intent": [
-        "database access",
-        "analyze files",
-    ],
-    "examples": [
-        "Connect to SQLite file",
-        "Search SQLite file",
-    ],
-    "name": "search_sqlite",
+    "name": "ask_sqlite",
     "description": f'''Ask SQLite file. To retrieve information from or make changes in a sqlite file, e.g. fetch data, update records, etc. Remember, use this function ONLY IF I provide you with a sqlite file path.''',
     "parameters": {
         "type": "object",
         "properties": {
             "path": {
                 "type": "string",
                 "description": "File path of the sqlite file",
@@ -88,12 +80,14 @@
                 "description": "The request about fetching data or making changes in the sqlite file, including all available supplementary information in detail, if any.  If there is no specific request apart from connection or query about table schema / information, return 'Describe tables' without extra comment or information.",
             },
         },
         "required": ["code", "request"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=search_sqlite)
+config.pluginsWithFunctionCall.append("ask_sqlite")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["ask_sqlite"] = ask_sqlite
 
 config.inputSuggestions.append("""Connect the following SQLite file and tell me about the tables that it contains:
-[CALL_search_sqlite]
+[CALL_ask_sqlite]
 \n""")
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/search weather info.py` & `letmedoit-2.1.9/letmedoit/plugins/search weather info.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,49 +2,42 @@
 LetMeDoIt AI Plugin - search weather info
 
 search for weather information
 
 [FUNCTION_CALL]
 """
 
-if not config.openweathermapApi:
-    config.changeOpenweathermapApi()
-
 if config.openweathermapApi:
     from letmedoit import config
     from letmedoit.utils.shared_utils import SharedUtil
     import json
 
     def search_weather_info(function_args):
         code = function_args.get("code") # required
         information = SharedUtil.showAndExecutePythonCode(code)
         if information:
             return json.loads(information)["information"]
         return "Not found!"
 
     functionSignature = {
-        "intent": [
-            "access to internet real-time information",
-        ],
-        "examples": [
-            "What's the current weather",
-        ],
         "name": "search_weather_info",
         "description": f'''Answer query about weather''',
         "parameters": {
             "type": "object",
             "properties": {
                 "code": {
                     "type": "string",
                     "description": f"""Python code that use my OpenWeatherMap API key '{config.openweathermapApi}' to resolve my request.
-To work with OpenWeatherMap API key, you may integrate python package geocoder in the code to find the required Latitude and Longitude.
+To work with OpenWeatherMap API key, you may integrWhat is the current weather in New York?ate python package geocoder in the code to find the required Latitude and Longitude.
 In the last line of your code, use 'print' function to print the requested information, without additional description or comment.""",
                 },
             },
             "required": ["code"],
         },
     }
 
-    config.addFunctionCall(signature=functionSignature, method=search_weather_info)
+    config.pluginsWithFunctionCall.append("search_weather_info")
+    config.chatGPTApiFunctionSignatures.append(functionSignature)
+    config.chatGPTApiAvailableFunctions["search_weather_info"] = search_weather_info
 else:
     config.print("To use plugin 'search weather info', you need to set up an OpenWeatherMap API key first.")
     config.print3("Read: https://github.com/eliranwong/letmedoit/wiki/OpenWeatherMap-API-Setup")
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/send email.py` & `letmedoit-2.1.9/letmedoit/plugins/send email.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,21 +89,14 @@
         return link
 
     SharedUtil.openURL(getOutlookLink() if email == "outlook" else getGoogleLink())
 
     return "Done!"
 
 functionSignature = {
-    "intent": [
-        "arrange activities",
-        "access to internet real-time information",
-    ],
-    "examples": [
-        "Send email",
-    ],
     "name": "send_email",
     "description": "send email",
     "parameters": {
         "type": "object",
         "properties": {
             "email": {
                 "type": "string",
@@ -123,8 +116,10 @@
                 "description": "The body or content of the email.",
             },
         },
         "required": ["email", "subject"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=send_email)
+config.pluginsWithFunctionCall.append("send_email")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["send_email"] = send_email
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/send whatsapp messages.py` & `letmedoit-2.1.9/letmedoit/plugins/send whatsapp messages.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,21 +16,14 @@
     if re.search("^[\+\(\)0-9]+?$", recipient):
         pywhatkit.sendwhatmsg_instantly(recipient, message)
     else:
         pywhatkit.sendwhatmsg_to_group_instantly(recipient, message)
     return "Done!"
 
 functionSignature = {
-    "intent": [
-        "arrange activities",
-        "access to internet real-time information",
-    ],
-    "examples": [
-        "Send WhatsApp",
-    ],
     "name": "send_whatsapp",
     "description": f'''Send WhatsApp messages''',
     "parameters": {
         "type": "object",
         "properties": {
             "recipient": {
                 "type": "string",
@@ -41,8 +34,10 @@
                 "description": "The message that is to be sent to the recipient",
             },
         },
         "required": ["recipient", "message"],
     },
 }
 
-config.addFunctionCall(signature=functionSignature, method=send_whatsapp)
+config.pluginsWithFunctionCall.append("send_whatsapp")
+config.chatGPTApiFunctionSignatures.append(functionSignature)
+config.chatGPTApiAvailableFunctions["send_whatsapp"] = send_whatsapp
```

### Comparing `letmedoit-2.1.84/letmedoit/plugins/simplified Chinese to traditional Chinese.py` & `letmedoit-2.1.9/letmedoit/plugins/simplified Chinese to traditional Chinese.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 
 def convertToTraditionalChinese(text):
     if text:
         return OpenCC('s2t').convert(text)
     else:
         return text
 
-config.outputTransformers.append(convertToTraditionalChinese)
+config.chatGPTTransformers.append(convertToTraditionalChinese)
```

### Comparing `letmedoit-2.1.84/letmedoit/utils/assistant.py` & `letmedoit-2.1.9/letmedoit/utils/assistant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,97 @@
 from letmedoit import config
-import openai, threading, os, time, traceback, re, subprocess, json, pydoc, textwrap, shutil, datetime, pprint, sys
+import openai, threading, os, time, traceback, re, subprocess, json, pydoc, textwrap, shutil, datetime, pprint
+try:
+    import tiktoken
+    tiktokenImported = True
+except:
+    tiktokenImported = False
 from pathlib import Path
 import pygments
 from pygments.lexers.python import PythonLexer
-#from pygments.lexers.shell import BashLexer
+from pygments.lexers.shell import BashLexer
 #from pygments.lexers.markup import MarkdownLexer
 from prompt_toolkit.formatted_text import PygmentsTokens
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.completion import WordCompleter, FuzzyCompleter
-from prompt_toolkit.shortcuts import clear, set_title
+from prompt_toolkit.shortcuts import clear
 from prompt_toolkit.application import run_in_terminal
 from prompt_toolkit import print_formatted_text, HTML
 from letmedoit.utils.terminal_mode_dialogs import TerminalModeDialogs
 from letmedoit.utils.prompts import Prompts
 from letmedoit.utils.promptValidator import FloatValidator, TokenValidator
 from letmedoit.utils.get_path_prompt import GetPath
 from letmedoit.utils.prompt_shared_key_bindings import swapTerminalColors
 from letmedoit.utils.file_utils import FileUtil
 from letmedoit.utils.terminal_system_command_prompt import SystemCommandPrompt
 from letmedoit.utils.shared_utils import SharedUtil
 from letmedoit.utils.tts_utils import TTSUtil
-from letmedoit.utils.ttsLanguages import TtsLanguages
 from letmedoit.utils.streaming_word_wrapper import StreamingWordWrapper
 from letmedoit.utils.text_utils import TextUtil
-from letmedoit.utils.sttLanguages import googleSpeeckToTextLanguages, whisperSpeeckToTextLanguages
 from letmedoit.chatgpt import ChatGPT
-from letmedoit.utils.install import installmodule
 if not config.isTermux:
     from letmedoit.autobuilder import AutoGenBuilder
     from letmedoit.geminipro import GeminiPro
     from letmedoit.palm2 import Palm2
     from letmedoit.codey import Codey
-from elevenlabs import generate, voices
+from letmedoit.utils.install import installmodule
 
 
 class LetMeDoItAI:
 
     def __init__(self):
         #config.letMeDoItAI = self
         self.prompts = Prompts()
         self.dialogs = TerminalModeDialogs(self)
         self.setup()
-        SharedUtil.runPlugins()
+        self.runPlugins()
 
     def setup(self):
         self.models = list(SharedUtil.tokenLimits.keys())
         config.divider = self.divider = "--------------------"
-        config.runPython = True
+        self.runPython = True
         if not hasattr(config, "accept_default"):
             config.accept_default = False
         if not hasattr(config, "defaultEntry"):
             config.defaultEntry = ""
         config.tempContent = ""
         config.tempChunk = ""
         if not hasattr(config, "predefinedContextTemp"):
             config.predefinedContextTemp = ""
         config.systemCommandPromptEntry = ""
         config.pagerContent = ""
         #self.addPagerContent = False
         # share the following methods in config so that they are accessible via plugins
-        config.addFunctionCall = SharedUtil.addFunctionCall
-        config.getLocalStorage = SharedUtil.getLocalStorage
+        config.getFiles = self.getFiles
         config.stopSpinning = self.stopSpinning
         config.toggleMultiline = self.toggleMultiline
         config.print = self.print
         config.print2 = self.print2
         config.print3 = self.print3
         config.getWrappedHTMLText = self.getWrappedHTMLText
         config.fineTuneUserInput = self.fineTuneUserInput
         config.launchPager = self.launchPager
         config.addPagerText = self.addPagerText
-        config.changeOpenweathermapApi = self.changeOpenweathermapApi
+        config.getFunctionMessageAndResponse = self.getFunctionMessageAndResponse
         config.runSpecificFuntion = ""
         # env variables
         os.environ["QT_QPA_PLATFORM_PLUGIN_PATH"] = config.env_QT_QPA_PLATFORM_PLUGIN_PATH
 
         # get path
         config.addPathAt = None
         self.getPath = GetPath(
             cancel_entry="",
             promptIndicatorColor=config.terminalPromptIndicatorColor2,
             promptEntryColor=config.terminalCommandEntryColor2,
             subHeadingColor=config.terminalColors[config.terminalPromptIndicatorColor2],
             itemColor=config.terminalColors[config.terminalCommandEntryColor2],
         )
 
-        # local storage directory
-        self.storageDir = SharedUtil.getLocalStorage()
-        # hisotry directory
+        self.storageDir = self.getStorageDir()
         if (not config.historyParentFolder or not os.path.isdir(config.historyParentFolder)) and self.storageDir:
             try:
                 historyParentFolder = os.path.join(self.storageDir, "history")
                 Path(historyParentFolder).mkdir(parents=True, exist_ok=True)
                 for i in ("chats", "paths", "commands"):
                     historyFile = os.path.join(historyParentFolder, i)
                     if not os.path.isfile(historyFile):
@@ -116,21 +115,26 @@
         else:
             SharedUtil.setAPIkey()
 
         chat_history = os.path.join(config.historyParentFolder if config.historyParentFolder else config.letMeDoItAIFolder, "history", "chats")
         self.terminal_chat_session = PromptSession(history=FileHistory(chat_history))
 
         # check if tts is ready
+        if not config.isVlcPlayerInstalled and not config.isPygameInstalled and not config.ttsCommand:
+            config.tts = False
+        else:
+            config.tts = True
         self.isTtsAvailable()
 
         self.actions = {
-            ".new": (f"start a new chat {str(config.hotkey_new)}", None),
+            ".new": ("start a new chat [ctrl+n]", None),
             ".save": ("save content", lambda: self.saveChat(config.currentMessages)),
-            ".export": (f"export content {str(config.hotkey_export)}", lambda: self.exportChat(config.currentMessages)),
-            ".context": (f"change chat context {str(config.hotkey_select_context)}", None),
+            ".export": ("export content [ctrl+s]", lambda: self.exportChat(config.currentMessages)),
+            #".instruction": ("run a predefined instruction", self.runInstruction),
+            ".context": ("change chat context [ctrl+o]", None),
             ".contextintegration": ("change chat context integration", self.setContextIntegration),
             ".changeapikey": ("change OpenAI API key", self.changeAPIkey),
             ".functionmodel": ("change function call model", self.setLlmModel),
             ".chatmodel": ("change chat-only model", self.setChatbot),
             ".embeddingmodel": ("change embedding model", self.setEmbeddingModel),
             ".temperature": ("change temperature", self.setTemperature),
             ".maxtokens": ("change maximum response tokens", self.setMaxTokens),
@@ -144,208 +148,138 @@
             ".functioncallintegration": ("change function call integration", self.setFunctionResponse),
             ".latestSearches": ("change online searches", self.setLatestSearches),
             ".userconfirmation": ("change code confirmation protocol", self.setUserConfirmation),
             ".codedisplay": ("change code display", self.setCodeDisplay),
             ".pagerview": ("change pager view", self.setPagerView),
             ".assistantname": ("change assistant name", self.setAssistantName),
             ".systemmessage": ("change custom system message", self.setCustomSystemMessage),
+            ".openweathermapapi": ("change OpenWeatherMap API key", self.changeOpenweathermapApi),
             ".ipinfo": ("change ip information integration", self.setIncludeIpInSystemMessage),
             ".storagedirectory": ("change storage directory", self.setStorageDirectory),
-            ".voicetypingconfig": ("change voice typing config", self.setVoiceTypingConfig),
-            ".texttospeechconfig": ("change text-to-speech config", self.setTextToSpeechConfig),
-            ".googleapiservice": ("change Google API service", self.selectGoogleAPIs),
-            ".openweathermapapi": ("change OpenWeatherMap API key", self.changeOpenweathermapApi),
-            ".elevenlabsapi": ("change ElevenLabs API key", self.changeElevenlabsApi),
             ".autobuilderconfig": ("change auto builder config", self.setAutoGenBuilderConfig),
             ".customtexteditor": ("change custom text editor", self.setCustomTextEditor),
             ".termuxapi": ("change Termux API integration", self.setTermuxApi),
             ".autoupgrade": ("change automatic upgrade", self.setAutoUpgrade),
-            ".developer": (f"change developer mode {str(config.hotkey_toggle_developer_mode)}", self.setDeveloperMode),
-            ".togglemultiline": (f"toggle multi-line input {str(config.hotkey_toggle_multiline_entry)}", self.toggleMultiline),
-            ".togglemousesupport": (f"toogle mouse support {str(config.hotkey_toggle_mouse_support)}", self.toggleMouseSupport),
-            ".toggletextbrightness": (f"swap text brightness {str(config.hotkey_swap_text_brightness)}", swapTerminalColors),
-            ".togglewordwrap": (f"toggle word wrap {str(config.hotkey_toggle_word_wrap)}", self.toggleWordWrap),
-            ".toggleimprovedwriting": (f"toggle improved writing {str(config.hotkey_toggle_writing_improvement)}", self.toggleImprovedWriting),
-            ".toggleinputaudio": (f"toggle input audio {str(config.hotkey_toggle_input_audio)}", self.toggleinputaudio),
-            ".toggleresponseaudio": (f"toggle response audio {str(config.hotkey_toggle_response_audio)}", self.toggleresponseaudio),
-            ".editresponse": (f"edit the last response {str(config.hotkey_edit_last_response)}", self.editLastResponse),
-            ".editconfigs": ("edit configuration settings", self.editConfigs),
+            ".developer": ("change developer mode [ctrl+d]", self.setDeveloperMode),
+            ".togglemultiline": ("toggle multi-line input [ctrl+l]", self.toggleMultiline),
+            ".togglemousesupport": ("toogle mouse support [esc+m]", self.toggleMouseSupport),
+            ".toggletextbrightness": ("swap text brightness [esc+s]", swapTerminalColors),
+            ".togglewordwrap": ("toggle word wrap [ctrl+w]", self.toggleWordWrap),
+            ".toggleimprovedwriting": ("toggle improved writing [esc+i]", self.toggleImprovedWriting),
+            ".toggleinputaudio": ("toggle input audio [ctrl+b]", self.toggleinputaudio),
+            ".toggleresponseaudio": ("toggle response audio [ctrl+p]", self.toggleresponseaudio),
+            ".ttscommand": ("configure text-to-speech command", self.defineTtsCommand),
             ".install": ("install python package", self.installPythonPackage),
-            ".system": (f"open system command prompt {str(config.hotkey_launch_system_prompt)}", lambda: SystemCommandPrompt().run(allowPathChanges=True)),
-            ".content": ("display current directory content", self.getPath.displayDirectoryContent),
-            ".keys": (f"display key bindings {str(config.hotkey_display_key_combo)}", config.showKeyBindings),
+            ".system": ("open system command prompt", lambda: SystemCommandPrompt().run(allowPathChanges=True)),
             ".help": ("open LetMeDoIt wiki", lambda: SharedUtil.openURL('https://github.com/eliranwong/letmedoit/wiki')),
-            ".donate": ("donate and support LetMeDoIt AI", lambda: SharedUtil.openURL('https://www.paypal.com/paypalme/letmedoitai')),
+            ".keys": ("display key bindings", config.showKeyBindings),
         }
 
         config.actionHelp = f"# Quick Actions\n(entries that start with '.')\n"
         for key, value in self.actions.items():
             config.actionHelp += f"{key}: {value[0]}\n"
         config.actionHelp += "\n## Read more at:\nhttps://github.com/eliranwong/letmedoit/wiki/Action-Menu"
 
+    def getStorageDir(self):
+        storageDir = os.path.join(os.path.expanduser('~'), config.letMeDoItName.split()[0].lower())
+        try:
+            Path(storageDir).mkdir(parents=True, exist_ok=True)
+        except:
+            pass
+        return storageDir if os.path.isdir(storageDir) else ""
+
+    def getFiles(self):
+        if config.storagedirectory and not os.path.isdir(config.storagedirectory):
+            config.storagedirectory = ""
+        storageDir = self.storageDir if self.storageDir else os.path.join(config.letMeDoItAIFolder, "files")
+        return config.storagedirectory if config.storagedirectory else storageDir
+
     def getFolderPath(self, default=""):
         return self.getPath.getFolderPath(
             check_isdir=True,
             display_dir_only=True,
             create_dirs_if_not_exist=True,
             empty_to_cancel=True,
             list_content_on_directory_change=True,
             keep_startup_directory=True,
             message=f"{self.divider}\nSetting a startup directory ...\nEnter a folder name or path below:",
             bottom_toolbar="",
             promptIndicator = "",
-            default=default,
+            default="",
         )
 
-    # Voice Typing Language
-    def setSpeechToTextLanguage(self):
-        # record in history for easy retrieval by moving arrows upwards / downwards
-        voice_typing_language_history = os.path.join(config.historyParentFolder if config.historyParentFolder else config.letMeDoItAIFolder, "history", "voice_typing_language")
-        voice_typing_language_session = PromptSession(history=FileHistory(voice_typing_language_history))
-        # input suggestion for languages
-        languages = tuple(googleSpeeckToTextLanguages.keys()) if config.voiceTypingPlatform in ("google", "googlecloud") else whisperSpeeckToTextLanguages
-        # default
-        default = ""
-        for i in languages:
-            if config.voiceTypingPlatform in ("google", "googlecloud") and googleSpeeckToTextLanguages[i] == config.voiceTypingLanguage:
-                default = i
-            elif i == config.voiceTypingLanguage:
-                default = i
-        if not default:
-            default = "English (United States)" if config.voiceTypingPlatform in ("google", "googlecloud") else "english"
-        # completer
-        completer = FuzzyCompleter(WordCompleter(languages, ignore_case=True))
-        self.print("Please specify the voice typing language:")
-        language = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default=default, promptSession=voice_typing_language_session, completer=completer)
-        if language and not language in (config.exit_entry, config.cancel_entry):
-            config.voiceTypingLanguage = language
-        if not config.voiceTypingLanguage in languages:
-            config.voiceTypingLanguage = "en-US" if config.voiceTypingPlatform in ("google", "googlecloud") else "english"
-        if config.voiceTypingPlatform in ("google", "googlecloud") and config.voiceTypingLanguage in languages:
-            config.voiceTypingLanguage = googleSpeeckToTextLanguages[config.voiceTypingLanguage]
-
-    # ElevenLabs Text-to-Speech Voice
-    def setElevenlabsVoice(self):
-        # record in history for easy retrieval by moving arrows upwards / downwards
-        elevenlabsVoice_history = os.path.join(config.historyParentFolder if config.historyParentFolder else config.letMeDoItAIFolder, "history", "elevenlabsVoice")
-        elevenlabsVoice_session = PromptSession(history=FileHistory(elevenlabsVoice_history))
-        # input suggestion for options
-        options = [voice.name for voice in voices()]
-        # default
-        default = config.elevenlabsVoice if config.elevenlabsVoice in options else "Rachel"
-        # completer
-        completer = FuzzyCompleter(WordCompleter(options, ignore_case=True))
-        self.print("Please specify ElevenLabs Text-to-Speech Voice:")
-        option = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default=default, promptSession=elevenlabsVoice_session, completer=completer)
-        if option and not option in (config.exit_entry, config.cancel_entry):
-            config.elevenlabsVoice = option if option in options else "Rachel"
-
-    # Google Text-to-Speech (Generic)
-    def setGttsLanguage(self):
-        # record in history for easy retrieval by moving arrows upwards / downwards
-        gtts_language_history = os.path.join(config.historyParentFolder if config.historyParentFolder else config.letMeDoItAIFolder, "history", "gtts_language")
-        gtts_language_session = PromptSession(history=FileHistory(gtts_language_history))
-        # input suggestion for languages
-        languages = tuple(TtsLanguages.gtts.keys())
-        # default
-        default = ""
-        for i in languages:
-            if TtsLanguages.gtts[i] == config.gttsLang:
-                default = i
-        if not default:
-            default = "en"
-        # completer
-        completer = FuzzyCompleter(WordCompleter(languages, ignore_case=True))
-        self.print("Please specify Google Text-to-Speech language:")
-        language = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default=default, promptSession=gtts_language_session, completer=completer)
-        if language and not language in (config.exit_entry, config.cancel_entry):
-            config.gttsLang = language
-        if config.gttsLang in languages:
-            config.gttsLang = TtsLanguages.gtts[config.gttsLang]
-        else:
-            config.gttsLang = "en"
+    def execPythonFile(self, script="", content=""):
+        if script or content:
+            try:
+                def runCode(text):
+                    code = compile(text, script, 'exec')
+                    exec(code, globals())
+                if content:
+                    runCode(content)
+                else:
+                    with open(script, 'r', encoding='utf8') as f:
+                        runCode(f.read())
+                return True
+            except:
+                self.print("Failed to run '{0}'!".format(os.path.basename(script)))
+                SharedUtil.showErrors()
+        return False
 
-    # Google Cloud Text-to-Speech (API)
-    def setGcttsLanguage(self):
-        # record in history for easy retrieval by moving arrows upwards / downwards
-        gctts_language_history = os.path.join(config.historyParentFolder if config.historyParentFolder else config.letMeDoItAIFolder, "history", "gctts_language")
-        gctts_language_session = PromptSession(history=FileHistory(gctts_language_history))
-        # input suggestion for languages
-        languages = tuple(TtsLanguages.gctts.keys())
-        # default
-        default = ""
-        for i in languages:
-            if TtsLanguages.gctts[i] == config.gcttsLang:
-                default = i
-        if not default:
-            default = "en-US"
-        # completer
-        completer = FuzzyCompleter(WordCompleter(languages, ignore_case=True))
-        self.print("Please specify Google Cloud Text-to-Speech language:")
-        language = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default=default, promptSession=gctts_language_session, completer=completer)
-        if language and not language in (config.exit_entry, config.cancel_entry):
-            config.gcttsLang = language
-        if config.gcttsLang in languages:
-            config.gcttsLang = TtsLanguages.gctts[config.gcttsLang]
-        else:
-            config.gcttsLang = "en-US"
+    def runPlugins(self):
+        # The following config values can be modified with plugins, to extend functionalities
+        config.pluginsWithFunctionCall = []
+        config.aliases = {}
+        config.predefinedContexts = {
+            "[none]": "",
+            "[custom]": "",
+        }
+        config.predefinedInstructions = {}
+        config.inputSuggestions = []
+        config.chatGPTTransformers = []
+        config.chatGPTApiFunctionSignatures = []
+        config.chatGPTApiAvailableFunctions = {}
+
+        # built-in functions
+        config.pluginsWithFunctionCall.append("execute_python_code")
+        if config.terminalEnableTermuxAPI:
+            config.pluginsWithFunctionCall.append("execute_termux_command")
 
-    def setVlcSpeed(self):
-        if config.isVlcPlayerInstalled and not config.usePygame:
-            self.print("Specify VLC player playback speed:")
-            self.print("(between 0.1 and 2.0)")
-            vlcSpeed = self.prompts.simplePrompt(style=self.prompts.promptStyle2, validator=FloatValidator(), default=str(config.vlcSpeed))
-            if vlcSpeed and not vlcSpeed.strip().lower() == config.exit_entry:
-                vlcSpeed = float(vlcSpeed)
-                if vlcSpeed < 0.1:
-                    vlcSpeed = 0.1
-                elif vlcSpeed > 2:
-                    vlcSpeed = 2
-                config.vlcSpeed = round(vlcSpeed, 1)
-                self.print3(f"VLC player playback speed: {vlcSpeed}")
-
-    def setGcttsSpeed(self):
-        self.print("Specify Google Cloud Text-to-Speech playback speed:")
-        self.print("(between 0.1 and 2.0)")
-        gcttsSpeed = self.prompts.simplePrompt(style=self.prompts.promptStyle2, validator=FloatValidator(), default=str(config.gcttsSpeed))
-        if gcttsSpeed and not gcttsSpeed.strip().lower() == config.exit_entry:
-            gcttsSpeed = float(gcttsSpeed)
-            if gcttsSpeed < 0.1:
-                gcttsSpeed = 0.1
-            elif gcttsSpeed > 2:
-                gcttsSpeed = 2
-            config.gcttsSpeed = round(gcttsSpeed, 1)
-            self.print3(f"Google Cloud Text-to-Speech playback speed: {gcttsSpeed}")
-
-    def selectGoogleAPIs(self):
-        if os.environ["GOOGLE_APPLICATION_CREDENTIALS"]:
-            enabledGoogleAPIs = self.dialogs.getMultipleSelection(
-                title="Google Cloud Service",
-                text="Select to enable Google Cloud Service in LetMeDoIt AI:",
-                options=("Vertex AI", "Speech-to-Text", "Text-to-Speech"),
-                default_values=config.enabledGoogleAPIs,
-            )
-            if enabledGoogleAPIs is not None:
-                config.enabledGoogleAPIs = enabledGoogleAPIs
+        pluginFolder = os.path.join(config.letMeDoItAIFolder, "plugins")
+        if self.storageDir:
+            customPluginFoler = os.path.join(self.storageDir, "plugins")
+            Path(customPluginFoler).mkdir(parents=True, exist_ok=True)
+            pluginFolders = (pluginFolder, customPluginFoler)
         else:
-            config.enabledGoogleAPIs = ["Vertex AI"]
-            self.print(f"API key json file '{config.google_cloud_credentials_file}' not found!")
-            self.print("Read https://github.com/eliranwong/letmedoit/wiki/Google-API-Setup for setting up Google API.")
-        if "Speech-to-Text" in config.enabledGoogleAPIs:
-            if not config.voiceTypingPlatform == "googlecloud":
-                config.voiceTypingPlatform = "googlecloud"
-                self.print3("Voice typing platform changed to: Google Text-to-Speech (API)")
-            self.setSpeechToTextLanguage()
-        if "Text-to-Speech" in config.enabledGoogleAPIs:
-            if not config.ttsPlatform == "googlecloud":
-                config.ttsPlatform = "googlecloud"
-                self.print3("Text-to-Speech platform changed to: Google Text-to-Speech (API)")
-            self.setGcttsLanguage()
-            self.setGcttsSpeed()
-        config.saveConfig()
+            pluginFolders = (pluginFolder,)
+        # always run 'integrate google searches'
+        internetSeraches = "integrate google searches"
+        script = os.path.join(pluginFolder, "{0}.py".format(internetSeraches))
+        self.execPythonFile(script)
+        # always include the following plugins
+        requiredPlugins = ("auto heal python code",)
+        for i in requiredPlugins:
+            if i in config.pluginExcludeList:
+                config.pluginExcludeList.remove(i)
+        # execute enabled plugins
+        for folder in pluginFolders:
+            for plugin in FileUtil.fileNamesWithoutExtension(folder, "py"):
+                if not plugin in config.pluginExcludeList:
+                    script = os.path.join(folder, "{0}.py".format(plugin))
+                    run = self.execPythonFile(script)
+                    if not run:
+                        config.pluginExcludeList.append(plugin)
+        if internetSeraches in config.pluginExcludeList:
+            del config.chatGPTApiFunctionSignatures[0]
+        self.setupPythonExecution()
+        if config.terminalEnableTermuxAPI:
+            self.setupTermuxExecution()
+        for i in config.pluginsWithFunctionCall:
+            callEntry = f"[CALL_{i}]"
+            if not callEntry in config.inputSuggestions:
+                config.inputSuggestions.append(callEntry)
 
     def selectPlugins(self):
         plugins = []
         enabledPlugins = []
         pluginFolder = os.path.join(config.letMeDoItAIFolder, "plugins")
         if self.storageDir:
             customPluginFoler = os.path.join(self.storageDir, "plugins")
@@ -366,15 +300,15 @@
         )
         if enabledPlugins is not None:
             for p in plugins:
                 if p in enabledPlugins and p in config.pluginExcludeList:
                     config.pluginExcludeList.remove(p)
                 elif not p in enabledPlugins and not p in config.pluginExcludeList:
                     config.pluginExcludeList.append(p)
-            SharedUtil.runPlugins()
+            self.runPlugins()
             config.saveConfig()
             self.print("Plugin selection updated!")
 
     def getCliOutput(self, cli):
         try:
             process = subprocess.Popen(cli, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             stdout, *_ = process.communicate()
@@ -414,36 +348,14 @@
             if SharedUtil.getWeather() is not None:
                 config.saveConfig()
                 self.print2("Configurations updated!")
             else:
                 config.openweathermapApi = ""
                 self.print2("Invalid API key entered!")
 
-    def changeElevenlabsApi(self):
-        if not config.terminalEnableTermuxAPI or (config.terminalEnableTermuxAPI and self.fingerprint()):
-            self.print("To set up ElevenLabs API Key, read:\nhttps://elevenlabs.io/docs/api-reference/text-to-speech#authentication\n")
-            self.print("Enter your ElevenLabs API Key:")
-            print()
-            apikey = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default=config.elevenlabsApi, is_password=True)
-            if apikey and not apikey.strip().lower() in (config.cancel_entry, config.exit_entry):
-                config.elevenlabsApi = apikey
-            try:
-                # testing
-                generate(
-                    api_key=config.elevenlabsApi, # Defaults to os.getenv(ELEVEN_API_KEY)
-                    text="test",
-                    voice="Rachel",
-                    model="eleven_multilingual_v2"
-                )
-                config.saveConfig()
-                self.print2("Configurations updated!")
-            except:
-                config.elevenlabsApi = ""
-                self.print2("Invalid API key entered!")
-
     def exitAction(self):
         message = "closing ..."
         self.print2(message)
         self.print(self.divider)
         return ""
 
     def print(self, content):
@@ -473,14 +385,429 @@
         while not stop_event.is_set():
             for symbol in "|/-\\":
                 print(symbol, end="\r")
                 time.sleep(0.1)
         #print("\r", end="")
         #print(" ", end="")
 
+#    def getChatResponse(self, completion):
+#        chat_response = completion["choices"][0]["message"]["content"]
+#        # transform response with plugins
+#        if chat_response:
+#            for t in config.chatGPTTransformers:
+#                chat_response = t(chat_response)
+#        return chat_response
+
+    def confirmExecution(self, risk):
+        if config.confirmExecution == "always" or (risk == "high" and config.confirmExecution == "high_risk_only") or (not risk == "low" and config.confirmExecution == "medium_risk_or_above"):
+            return True
+        else:
+            return False
+
+    def showRisk(self, risk):
+        if not config.confirmExecution in ("always", "medium_risk_or_above", "high_risk_only", "none"):
+            config.confirmExecution = "always"
+        self.print(f"[risk level: {risk}]")
+
+    def setupTermuxExecution(self):
+        def execute_termux_command(function_args):
+            # retrieve argument values from a dictionary
+            risk = function_args.get("risk") # required
+            title = function_args.get("title") # required
+            #sharedText = function_args.get("message", "") # optional
+            function_args = textwrap.dedent(function_args.get("code")).strip() # required
+            sharedText = re.sub("^termux-share .*?'([^']+?)'$", r"\1", function_args)
+            sharedText = re.sub('^termux-share .*?"([^"]+?)"$', r"\1", sharedText)
+            sharedText = re.sub("""^[\d\D]*?subprocess.run\(\['termux-share'[^\[\]]*?'([^']+?)'\]\)[\d\D]*?$""", r"\1", sharedText)
+            sharedText = re.sub('''^[\d\D]*?subprocess.run\(\["termux-share"[^\[\]]*?"([^']+?)"\]\)[\d\D]*?$''', r"\1", sharedText)
+            function_args = function_args if sharedText == function_args else f'''termux-share -a send "{sharedText}"'''
+
+            # show Termux command for developer
+            self.print(self.divider)
+            self.print(f"Termux: {title}")
+            self.showRisk(risk)
+            if config.developer or config.codeDisplay:
+                self.print("```")
+                #print(function_args)
+                tokens = list(pygments.lex(function_args, lexer=BashLexer()))
+                print_formatted_text(PygmentsTokens(tokens), style=SharedUtil.getPygmentsStyle())
+                self.print("```")
+            self.print(self.divider)
+
+            self.stopSpinning()
+            if self.confirmExecution(risk):
+                self.print("Do you want to execute it? [y]es / [N]o")
+                confirmation = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default="y")
+                if not confirmation.lower() in ("y", "yes"):
+                    return "[INVALID]"
+
+            try:
+                if not sharedText == function_args:
+                    pydoc.pipepager(sharedText, cmd="termux-share -a send")
+                    function_response = "Done!"
+                else:
+                    # display both output and error
+                    function_response = SharedUtil.runSystemCommand(function_args)
+                self.print(function_response)
+            except:
+                SharedUtil.showErrors()
+                self.print(self.divider)
+                return "[INVALID]"
+            info = {"information": function_response}
+            function_response = json.dumps(info)
+            return json.dumps(info)
+
+        functionSignature = {
+            "name": "execute_termux_command",
+            "description": "Execute Termux command on Android",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "code": {
+                        "type": "string",
+                        "description": "Termux command, e.g. am start -n com.android.chrome/com.google.android.apps.chrome.Main",
+                    },
+                    "title": {
+                        "type": "string",
+                        "description": "title for the termux command",
+                    },
+                    "risk": {
+                        "type": "string",
+                        "description": "Assess the risk level of damaging my device upon executing the task. e.g. file deletions or similar significant impacts are regarded as 'high' level.",
+                        "enum": ["high", "medium", "low"],
+                    },
+                },
+                "required": ["code", "title", "risk"],
+            },
+        }
+
+        config.execute_termux_command_signature = [functionSignature]
+        # useful when enhanced mode is disabled
+        config.chatGPTApiFunctionSignatures.append(functionSignature)
+        config.chatGPTApiAvailableFunctions["execute_termux_command"] = execute_termux_command
+
+    def setupPythonExecution(self):
+        def execute_python_code(function_args):
+            # retrieve argument values from a dictionary
+            risk = function_args.get("risk") # required
+            title = function_args.get("title") # required
+            python_code = function_args.get("code") # required
+            refinedCode = SharedUtil.fineTunePythonCode(python_code)
+
+            # show pyton code for developer
+            self.print(self.divider)
+            self.print(f"Python: {title}")
+            self.showRisk(risk)
+            if config.developer or config.codeDisplay:
+                self.print("```")
+                #print(python_code)
+                # pygments python style
+                tokens = list(pygments.lex(python_code, lexer=PythonLexer()))
+                print_formatted_text(PygmentsTokens(tokens), style=SharedUtil.getPygmentsStyle())
+                self.print("```")
+            self.print(self.divider)
+
+            self.stopSpinning()
+            if not self.runPython:
+                return "[INVALID]"
+            elif self.confirmExecution(risk):
+                self.print("Do you want to execute it? [y]es / [N]o")
+                confirmation = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default="y")
+                if not confirmation.lower() in ("y", "yes"):
+                    self.runPython = False
+                    return "[INVALID]"
+            return SharedUtil.executePythonCode(refinedCode)
+
+        functionSignature = {
+            "name": "execute_python_code",
+            "description": "Execute python code to resolve a computing task",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "code": {
+                        "type": "string",
+                        "description": "Python code that integrates any relevant packages to resolve my request",
+                    },
+                    "title": {
+                        "type": "string",
+                        "description": "title for the python code",
+                    },
+                    "risk": {
+                        "type": "string",
+                        "description": "Assess the risk level of damaging my device upon executing the task. e.g. file deletions or similar significant impacts are regarded as 'high' level.",
+                        "enum": ["high", "medium", "low"],
+                    },
+                },
+                "required": ["code", "title", "risk"],
+            },
+        }
+
+        config.execute_python_code_signature = [functionSignature]
+        # useful when enhanced mode is disabled
+        config.chatGPTApiFunctionSignatures.append(functionSignature)
+        config.chatGPTApiAvailableFunctions["execute_python_code"] = execute_python_code
+
+        ### A dummy function to redirect q&a task about python, otherwise, it may be mistaken by execute_python_code
+        def python_qa(function_args):
+            return "[INVALID]"
+        functionSignature = {
+            "name": "python_qa",
+            "description": f'''Answer questions or provide information about python''',
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "qa": {
+                        "type": "string",
+                        "description": "empty string ''",
+                    },
+                },
+            },
+        }
+        #config.pluginsWithFunctionCall.append("python_qa")
+        config.chatGPTApiFunctionSignatures.append(functionSignature)
+        config.chatGPTApiAvailableFunctions["python_qa"] = python_qa
+
+    # call a specific function and return messages
+    def runFunction(self, messages, functionSignatures, function_name):
+        messagesCopy = messages[:]
+        try:
+            function_call_message, function_call_response = self.getFunctionMessageAndResponse(messages, functionSignatures, function_name)
+            messages.append(function_call_message)
+            messages.append(
+                {
+                    "role": "function",
+                    "name": function_name,
+                    "content": function_call_response if function_call_response else config.tempContent,
+                }
+            )
+            config.tempContent = ""
+        except:
+            SharedUtil.showErrors()
+            return messagesCopy
+        return messages
+
+    def getFunctionMessageAndResponse(self, messages, functionSignatures, function_name, temperature=None):
+        completion = config.oai_client.chat.completions.create(
+            model=config.chatGPTApiModel,
+            messages=messages,
+            max_tokens=SharedUtil.getDynamicTokens(messages, functionSignatures),
+            temperature=temperature if temperature is not None else config.llmTemperature,
+            n=1,
+            tools=SharedUtil.convertFunctionSignaturesIntoTools(functionSignatures),
+            tool_choice={"type": "function", "function": {"name": function_name}},
+        )
+        function_call_message = completion.choices[0].message
+        tool_call = function_call_message.tool_calls[0]
+        func_arguments = tool_call.function.arguments
+        function_call_message_mini = {
+            "role": "assistant",
+            "content": "",
+            "function_call": {
+                "name": tool_call.function.name,
+                "arguments": func_arguments,
+            }
+        }
+        function_call_response = self.getFunctionResponse(func_arguments, function_name)
+        return function_call_message_mini, function_call_response
+
+    def getFunctionResponse(self, func_arguments, function_name):
+        def notifyDeveloper(func_name):
+            if config.developer:
+                #self.print(f"running function '{func_name}' ...")
+                print_formatted_text(HTML(f"<{config.terminalPromptIndicatorColor2}>Running function</{config.terminalPromptIndicatorColor2}> <{config.terminalCommandEntryColor2}>'{func_name}'</{config.terminalCommandEntryColor2}> <{config.terminalPromptIndicatorColor2}>...</{config.terminalPromptIndicatorColor2}>"))
+        # ChatGPT's built-in function named "python"
+        if function_name == "python":
+            notifyDeveloper(function_name)
+            python_code = textwrap.dedent(func_arguments)
+            refinedCode = SharedUtil.fineTunePythonCode(python_code)
+
+            self.print(self.divider)
+            self.print2("running python code ...")
+            risk = SharedUtil.riskAssessment(python_code)
+            self.showRisk(risk)
+            if config.developer or config.codeDisplay:
+                print("```")
+                #print(python_code)
+                # pygments python style
+                tokens = list(pygments.lex(python_code, lexer=PythonLexer()))
+                print_formatted_text(PygmentsTokens(tokens), style=SharedUtil.getPygmentsStyle())
+                print("```")
+            self.print(self.divider)
+
+            self.stopSpinning()
+            if not self.runPython:
+                info = {"information": python_code}
+                return json.dumps(info)
+            elif self.confirmExecution(risk):
+                self.print("Do you want to continue? [y]es / [N]o")
+                confirmation = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default="y")
+                if not confirmation.lower() in ("y", "yes"):
+                    info = {"information": python_code}
+                    return json.dumps(info)
+            try:
+                exec(refinedCode, globals())
+                function_response = SharedUtil.getPythonFunctionResponse(refinedCode)
+            except:
+                trace = SharedUtil.showErrors()
+                self.print(self.divider)
+                if config.max_consecutive_auto_heal > 0:
+                    return SharedUtil.autoHealPythonCode(refinedCode, trace)
+                else:
+                    return "[INVALID]"
+            if function_response:
+                info = {"information": function_response}
+                function_response = json.dumps(info)
+        # known unwanted functions are handled here
+        elif function_name in ("translate_text",):
+            # "translate_text" has two arguments, "text", "target_language"
+            # handle known and unwanted function
+            function_response = "[INVALID]" 
+        # handle unexpected function
+        elif not function_name in config.chatGPTApiAvailableFunctions:
+            if config.developer:
+                self.print(f"Unexpected function: {function_name}")
+                self.print(self.divider)
+                print(func_arguments)
+                self.print(self.divider)
+            function_response = "[INVALID]"
+        else:
+            notifyDeveloper(function_name)
+            fuction_to_call = config.chatGPTApiAvailableFunctions[function_name]
+            # convert the arguments from json into a dict
+            function_args = json.loads(func_arguments)
+            function_response = fuction_to_call(function_args)
+        return function_response
+
+    def runCompletion(self, thisMessage, noFunctionCall=False):
+        self.functionJustCalled = False
+        def runThisCompletion(thisThisMessage):
+            if config.chatGPTApiFunctionSignatures and not self.functionJustCalled and not noFunctionCall:
+                return config.oai_client.chat.completions.create(
+                    model=config.chatGPTApiModel,
+                    messages=thisThisMessage,
+                    n=1,
+                    temperature=config.llmTemperature,
+                    max_tokens=SharedUtil.getDynamicTokens(thisThisMessage, config.chatGPTApiFunctionSignatures),
+                    tools=SharedUtil.convertFunctionSignaturesIntoTools(config.chatGPTApiFunctionSignatures),
+                    tool_choice={"type": "function", "function": {"name": config.runSpecificFuntion}} if config.runSpecificFuntion else config.chatGPTApiFunctionCall,
+                    stream=True,
+                )
+            return config.oai_client.chat.completions.create(
+                model=config.chatGPTApiModel,
+                messages=thisThisMessage,
+                n=1,
+                temperature=config.llmTemperature,
+                max_tokens=SharedUtil.getDynamicTokens(thisThisMessage),
+                stream=True,
+            )
+
+        while True:
+            completion = runThisCompletion(thisMessage)
+            config.runSpecificFuntion = ""
+            try:
+                # consume the first delta
+                for event in completion:
+                    first_delta = event.choices[0].delta
+                    # check if a tool is called
+                    if first_delta.tool_calls: # a tool is called
+                        function_calls = [i for i in first_delta.tool_calls if i.type == "function"]
+                        # non_function_calls = [i for i in first_delta.tool_calls if not i.type == "function"]
+                    else: # no tool is called; same handling as tools finished calling; which break the loop later
+                        self.functionJustCalled = True
+                    # consume the first delta only at this point
+                    break
+                # Continue only when a function is called
+                if self.functionJustCalled:
+                    break
+
+                # get all tool arguments, both of functions and non-functions
+                toolArguments = SharedUtil.getToolArgumentsFromStreams(completion)
+
+                func_responses = ""
+                bypassFunctionCall = False
+                # handle function calls
+                for func in function_calls:
+                    func_index = func.index
+                    func_id = func.id
+                    func_name = func.function.name
+                    func_arguments = toolArguments[func_index]
+
+                    # get function response
+                    func_response = self.getFunctionResponse(func_arguments, func_name)
+
+                    # "[INVALID]" practically mean that it ignores previously called function and continues chat without function calling
+                    if func_response == "[INVALID]":
+                        bypassFunctionCall = True
+                    elif func_response or config.tempContent:
+                        # send the function call info and response to GPT
+                        function_call_message = {
+                            "role": "assistant",
+                            "content": "",
+                            "function_call": {
+                                "name": func_name,
+                                "arguments": func_arguments,
+                            }
+                        }
+                        thisMessage.append(function_call_message) # extend conversation with assistant's reply
+                        thisMessage.append(
+                            {
+                                "tool_call_id": func_id,
+                                "role": "function",
+                                "name": func_name,
+                                "content": func_response if func_response else config.tempContent,
+                            }
+                        )  # extend conversation with function response
+                        config.tempContent = ""
+                        if func_response:
+                            func_responses += f"\n{func_response}\n{config.divider}"
+
+                self.functionJustCalled = True
+
+                # bypassFunctionCall is set to True, usually when a function is called by mistake
+                if bypassFunctionCall:
+                    pass
+                # two cases that breaks the loop at this point
+                # 1. func_responses == ""
+                # 2. config.passFunctionCallReturnToChatGPT = False
+                elif not config.passFunctionCallReturnToChatGPT or not func_responses:
+                    if func_responses:
+                        self.print(f"{config.divider}\n{func_responses}")
+                    # A break here means that no information from the called function is passed back to ChatGPT
+                    # 1. config.passFunctionCallReturnToChatGPT is set to True
+                    # 2. func_responses = "" or None; can be specified in plugins
+                    break
+            except:
+                SharedUtil.showErrors()
+                break
+
+        return completion
+
+    # reset message when a new chart is started or context is changed
+    def resetMessages(self):
+        systemMessage = config.customSystemMessage if config.customSystemMessage else f'''You’re {config.letMeDoItName}, an advanced AI assistant, capable of both engaging in conversations and executing codes on my device.
+I am providing the basic information of my device below in case you need it:
+```
+{SharedUtil.getDeviceInfo()}
+```
+Please use the current time and date that I have provided above as a reference point for any relative dates and times mentioned in my prompt.
+You have all the necessary permissions to execute system commands and Python code on my behalf. Your functionality expands as I add more plugins to you. You respond to my prompts and perform tasks based on your own knowledge, the context I provide, as well as the additional knowledge and capabilities provided by plugins.
+
+When replying to my requests, please follow these steps:
+Step 1: Consider our previous conversations, particularly your last response, if any, as the context for these requests.
+Step 2: Estimate my intent based on the request and context. The intent can be a code generation task, an executable computing task, a math-solving task, a translation task, or a question answering task.
+Step 3: Reply based on the estimated intent.
+Remember, do not use function call if it is a translation task.
+
+Always remember that you are much more than a text-based AI. You possess both vision and speech capabilities and have direct access to my device's system, enabling you to execute tasks at my command. Please do not state otherwise.
+'''
+        messages = [
+            {"role": "system", "content": systemMessage}
+        ]
+        return messages
+
     # update system message
     def updateSystemMessage(self, messages):
         for index, message in enumerate(messages):
             try:
                 if message.get("role", "") == "system":
                     # update system mess
                     dayOfWeek = SharedUtil.getDayOfWeek()
@@ -663,15 +990,15 @@
                 config.chatGPTApiFunctionCall = "auto"
                 if "integrate google searches" in config.pluginExcludeList:
                     config.pluginExcludeList.remove("integrate google searches")
             elif config.loadingInternetSearches == "none":
                 if not "integrate google searches" in config.pluginExcludeList:
                     config.pluginExcludeList.append("integrate google searches")
             # reset plugins
-            SharedUtil.runPlugins()
+            self.runPlugins()
             # notify
             config.saveConfig()
             self.print3(f"Latest Online Searches: {option}")
 
     def setUserConfirmation(self):
         options = ("always", "medium_risk_or_above", "high_risk_only", "none")
         if not config.confirmExecution in options:
@@ -691,20 +1018,19 @@
         )
         if option:
             config.confirmExecution = option
             config.saveConfig()
             self.print3(f"Command Confirmation Protocol: {option}")
 
     def setPagerView(self):
-        manuel = f"""manual '{str(config.hotkey_launch_pager_view).replace("'", "")}'"""
-        options = ("auto", manuel)
+        options = ("auto", "manual [ctrl+g]")
         option = self.dialogs.getValidOptions(
             options=options,
             title="Pager View",
-            default="auto" if config.pagerView else manuel,
+            default="auto" if config.pagerView else "manual [ctrl+g]",
         )
         if option:
             config.pagerView = (option == "auto")
             config.saveConfig()
             self.print3(f"Pager View: {option}!")
 
     def setDeveloperMode(self):
@@ -736,15 +1062,15 @@
             if config.terminalEnableTermuxAPI:
                 # Check if Termux API package is installed
                 result = subprocess.run(['pkg', 'list-installed', 'termux-api'], capture_output=True, text=True)
                 # Check if the package is installed
                 if not "termux-api" in result.stdout:
                     self.print("Termux:API is not installed!")
             # reset plugins
-            SharedUtil.runPlugins()
+            self.runPlugins()
             config.saveConfig()
             self.print3(f"""Termux API Integration: {"enable" if config.terminalEnableTermuxAPI else "disable"}d!""")
 
     def setFunctionCall(self):
         calls = ("auto", "none")
         call = self.dialogs.getValidOptions(
             options=calls,
@@ -766,46 +1092,14 @@
             text="Enabling this feature allows\npassing function call responses, if any,\nto extend conversation with ChatGPT.\nDisabling this feature allows\nrunning function calls\nwithout generating further responses."
         )
         if call:
             config.passFunctionCallReturnToChatGPT = (call == "enable")
             config.saveConfig()
             self.print3(f"Pass Function Call Response to ChatGPT: {'enabled' if config.passFunctionCallReturnToChatGPT else 'disabled'}!")
 
-    def editLastResponse(self):
-        customTextEditor = config.customTextEditor if config.customTextEditor else f"{sys.executable} {os.path.join(config.letMeDoItAIFolder, 'eTextEdit.py')}"
-        pydoc.pipepager(config.pagerContent, cmd=customTextEditor)
-        set_title(config.letMeDoItName)
-
-    # change configs
-    def editConfigs(self):
-        # file paths
-        configFile = os.path.join(config.letMeDoItAIFolder, "config.py")
-        backupFile = os.path.join(config.getLocalStorage(), "config_backup.py")
-        # backup configs
-        config.saveConfig()
-        shutil.copy(configFile, backupFile)
-        # open current configs with built-in text editor
-        customTextEditor = config.customTextEditor if config.customTextEditor else f"{sys.executable} {os.path.join(config.letMeDoItAIFolder, 'eTextEdit.py')}"
-        os.system(f"{customTextEditor} {configFile}")
-        set_title(config.letMeDoItName)
-        # re-load configs
-        try:
-            config.loadConfig(configFile)
-            self.print2("Changes loaded!")
-        except:
-            self.print2("Failed to load your changes!")
-            print(traceback.format_exc())
-            try:
-                self.print2("Restoring backup ...")
-                config.loadConfig(backupFile)
-                shutil.copy(backupFile, configFile)
-                self.print2("Restored!")
-            except:
-                self.print2("Failed to restore backup!")
-
     def installPythonPackage(self):
         self.print("Enter a python package name:")
         package = self.prompts.simplePrompt(style=self.prompts.promptStyle2)
         if package:
             self.print(f"Installing '{package}' ...")
             installmodule(f"--upgrade {package}")
 
@@ -823,22 +1117,28 @@
             config.saveConfig()
             self.print3(f"LLM Temperature: {temperature}")
 
     def setLlmModel(self):
         model = self.dialogs.getValidOptions(
             options=self.models,
             title="Function Calling Model",
-            default=config.chatGPTApiModel if config.chatGPTApiModel in self.models else self.models[0],
+            default=config.chatGPTApiModel,
             text="Select a function call model:\n(for both chat and task execution)",
         )
         if model:
             config.chatGPTApiModel = model
             self.print3(f"ChatGPT model: {model}")
-            # set max tokens
-            config.chatGPTApiMaxTokens = self.getMaxTokens()[-1]
+            # handle max tokens
+            if tiktokenImported:
+                functionTokens = SharedUtil.count_tokens_from_functions(config.chatGPTApiFunctionSignatures)
+                tokenLimit = SharedUtil.tokenLimits[config.chatGPTApiModel] - functionTokens
+            else:
+                tokenLimit = SharedUtil.tokenLimits[config.chatGPTApiModel]
+            suggestedMaxToken = int(tokenLimit / 2)
+            config.chatGPTApiMaxTokens = 4096 if config.chatGPTApiModel in ("gpt-4-turbo-preview", "gpt-4-0125-preview", "gpt-4-1106-preview") else suggestedMaxToken # 'gpt-4-1106-preview' supports at most 4096 completion tokens
             config.saveConfig()
             self.print3(f"Maximum response tokens: {config.chatGPTApiMaxTokens}")
 
     def setChatbot(self):
         model = self.dialogs.getValidOptions(
             options=("chatgpt", "geminipro", "palm2", "codey"),
             title="Chat-only model",
@@ -848,15 +1148,15 @@
         if model:
             config.chatbot = model
             self.print3(f"Chat-only model: {model}")
 
     def setEmbeddingModel(self):
         oldEmbeddingModel = config.embeddingModel
         model = self.dialogs.getValidOptions(
-            options=("text-embedding-3-large", "text-embedding-3-small", "text-embedding-ada-002", "paraphrase-multilingual-mpnet-base-v2", "all-mpnet-base-v2", "all-MiniLM-L6-v2", "custom"),
+            options=("text-embedding-ada-002", "paraphrase-multilingual-mpnet-base-v2", "all-mpnet-base-v2", "all-MiniLM-L6-v2", "custom"),
             title="Embedding model",
             default=config.embeddingModel,
             text="Select an embedding model:",
         )
         if model:
             if model == "custom":
                 self.print("Enter OpenAI or Sentence Transformer Embedding model:")
@@ -869,16 +1169,16 @@
             self.print3(f"Embedding model: {model}")
         if not oldEmbeddingModel == config.embeddingModel:
             self.print(f"You've change the embedding model from '{oldEmbeddingModel}' to '{config.embeddingModel}'.")
             self.print("To work with the newly selected model, previous memory store and retrieved collections need to be deleted.")
             self.print("Do you want to delete them now? [y]es / [N]o")
             confirmation = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default="yes")
             if confirmation.lower() in ("y", "yes"):
-                memory_store = os.path.join(config.getLocalStorage(), "memory")
-                retrieved_collections = os.path.join(config.getLocalStorage(), "autogen", "retriever")
+                memory_store = os.path.join(config.getFiles(), "memory")
+                retrieved_collections = os.path.join(config.getFiles(), "autogen", "retriever")
                 for folder in (memory_store, retrieved_collections):
                     shutil.rmtree(folder, ignore_errors=True)
             else:
                 self.print(f"Do you want to change back the embedding model from '{config.embeddingModel}' to '{oldEmbeddingModel}'? [y]es / [N]o")
                 confirmation = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default="yes")
                 if not confirmation.lower() in ("y", "yes"):
                     config.embeddingModel = oldEmbeddingModel
@@ -891,26 +1191,26 @@
             AutoGenBuilder().promptConfig()
 
     def setAssistantName(self):
         self.print("You may modify my name below:")
         letMeDoItName = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default=config.letMeDoItName)
         if letMeDoItName and not letMeDoItName.strip().lower() == config.exit_entry:
             config.letMeDoItName = letMeDoItName
-            self.storageDir = SharedUtil.getLocalStorage()
+            self.storageDir = self.getStorageDir()
             config.saveConfig()
             self.print3(f"You have changed my name to: {config.letMeDoItName}")
 
     def setCustomSystemMessage(self):
         self.print("You can modify the system message to furnish me with details about my capabilities, constraints, or any pertinent context that may inform our interactions. This will guide me in managing and responding to your requests appropriately.")
         self.print("Please note that altering my system message directly affects my functionality. Handle with care.")
         self.print("Enter custom system message below:")
         self.print(f"(Keep it blank to use {config.letMeDoItName} default system message.)")
-        message = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default=config.systemMessage_letmedoit)
+        message = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default=config.customSystemMessage)
         if message and not message.strip().lower() == config.exit_entry:
-            config.systemMessage_letmedoit = message
+            config.customSystemMessage = message
             config.saveConfig()
             self.print3(f"Custom system message: {config.letMeDoItName}")
 
     def setCustomTextEditor(self):
         self.print("Please specify custom text editor command below:")
         self.print("e.g. 'micro -softwrap true -wordwrap true'")
         self.print("Leave it blank to use our built-in text editor 'eTextEdit' by default.")
@@ -956,87 +1256,88 @@
         if mintokens and not mintokens.strip().lower() == config.exit_entry and int(mintokens) > 0:
             config.chatGPTApiMinTokens = int(mintokens)
             if config.chatGPTApiMinTokens > config.chatGPTApiMaxTokens:
                 config.chatGPTApiMinTokens = config.chatGPTApiMaxTokens
             config.saveConfig()
             self.print3(f"Minimum tokens: {config.chatGPTApiMinTokens}")
 
-    def getMaxTokens(self):
-        contextWindowLimit = SharedUtil.tokenLimits[config.chatGPTApiModel]
-        functionTokens = SharedUtil.count_tokens_from_functions(config.chatGPTApiFunctionSignatures.values())
-        maxToken = contextWindowLimit - functionTokens - config.chatGPTApiMinTokens
-        if maxToken > 4096 and config.chatGPTApiModel in (
-            "gpt-4-turbo-preview",
-            "gpt-4-0125-preview",
-            "gpt-4-1106-preview",
-            "gpt-3.5-turbo",
-        ):
-            maxToken = 4096
-        return contextWindowLimit, functionTokens, maxToken
-
     def setMaxTokens(self):
-        contextWindowLimit, functionTokens, tokenLimit = self.getMaxTokens()
-        if tokenLimit < config.chatGPTApiMinTokens:
-            self.print2(f"Function tokens [{functionTokens}] exceed {config.chatGPTApiModel} response token limit.")
-            self.print("Either change to a model with higher token limit or disable unused function-call plguins.")
+        contextWindowLimit = SharedUtil.tokenLimits[config.chatGPTApiModel]
+        if tiktokenImported:
+            functionTokens = SharedUtil.count_tokens_from_functions(config.chatGPTApiFunctionSignatures)
+            tokenLimit = contextWindowLimit - functionTokens - config.chatGPTApiMinTokens
+        else:
+            tokenLimit = contextWindowLimit
+        if tiktokenImported and tokenLimit < config.chatGPTApiMinTokens:
+            self.print(f"Availble functions have already taken up too many tokens [{functionTokens}] to work with selected model '{config.chatGPTApiModel}'. You may either changing to a model that supports more tokens or deactivating some of the plugins that you don't need to reduce the number of tokens in total.")
         else:
             self.print(self.divider)
-            self.print("GPT and embeddings models process text in chunks called tokens. As a rough rule of thumb, 1 token is approximately 4 characters or 0.75 words for English text. One limitation to keep in mind is that for a GPT model the prompt and the generated output combined must be no more than the model's maximum context length.")
-            self.print3(f"Current GPT model: {config.chatGPTApiModel}")
-            self.print3(f"Maximum context length: {contextWindowLimit}")
-            self.print3(f"Current function tokens: {functionTokens}")
-            self.print3(f"Maximum response token allowed (excl. functions): {tokenLimit}")
+            self.print(f"You are now using ChatGPT model '{config.chatGPTApiModel}'. Its context window limit is {contextWindowLimit} tokens.")
+            if tiktokenImported:
+                self.print(f"Current enabled functions have taken up {functionTokens} tokens.")
+            self.print(f"You can have no more than {tokenLimit} tokens, for both prompts and responses, in a single chain of messages.")
+            self.print("(GPT and embeddings models process text in chunks called tokens. As a rough rule of thumb, 1 token is approximately 4 characters or 0.75 words for English text. One limitation to keep in mind is that for a GPT model the prompt and the generated output combined must be no more than the model's maximum context length.)")
             self.print(self.divider)
             self.print("Please specify maximum response tokens below:")
+            self.print("(Remarks: If the entered value exceeds the maximum number of completion tokens allowed in your selected model, it will be modified.)")
             maxtokens = self.prompts.simplePrompt(style=self.prompts.promptStyle2, numberOnly=True, default=str(config.chatGPTApiMaxTokens))
             if maxtokens and not maxtokens.strip().lower() == config.exit_entry and int(maxtokens) > 0:
                 config.chatGPTApiMaxTokens = int(maxtokens)
-                if config.chatGPTApiMaxTokens > tokenLimit:
-                    config.chatGPTApiMaxTokens = tokenLimit
+                if config.chatGPTApiMaxTokens > 4096 if config.chatGPTApiModel in ("gpt-4-turbo-preview", "gpt-4-0125-preview", "gpt-4-1106-preview") else tokenLimit: # 'gpt-4-1106-preview' supports at most 4096 completion tokens
+                    config.chatGPTApiMaxTokens = 4096 if config.chatGPTApiModel in ("gpt-4-turbo-preview", "gpt-4-0125-preview", "gpt-4-1106-preview") else tokenLimit
                 config.saveConfig()
                 self.print3(f"Maximum tokens: {config.chatGPTApiMaxTokens}")
 
+    def runPythonScript(self, script):
+        script = script.strip()[3:-3]
+        try:
+            exec(script, globals())
+        except:
+            trace = traceback.format_exc()
+            print(trace if config.developer else "Error encountered!")
+            self.print(self.divider)
+            if config.max_consecutive_auto_heal > 0:
+                SharedUtil.autoHealPythonCode(script, trace)
+
     def runSystemCommand(self, command):
         command = command.strip()[1:]
-        if "\n" in command:
+        if config.multilineInput:
             command = ";".join(command.split("\n"))
         if config.thisPlatform == "Windows":
             os.system(command)
         else:
             os.system(f"env QT_QPA_PLATFORM_PLUGIN_PATH='{config.env_QT_QPA_PLATFORM_PLUGIN_PATH}' {command}")
 
     def toggleMultiline(self):
         config.multilineInput = not config.multilineInput
         run_in_terminal(lambda: self.print(f"Multi-line input {'enabled' if config.multilineInput else 'disabled'}!"))
         if config.multilineInput:
             run_in_terminal(lambda: self.print("Use 'escape + enter' to complete your entry."))
 
     def isTtsAvailable(self):
-        if not config.isVlcPlayerInstalled and not config.isPygameInstalled and not config.ttsCommand and not config.elevenlabsApi:
-            self.print2("Text-to-speech feature is not enabled!")
-            self.print3("Read: https://github.com/eliranwong/letmedoit/wiki/letMeDoIt-Speaks")
-            config.tts = False
-        else:
-            config.tts = True
-        return config.tts
+        if config.tts:
+            return True
+        self.print("Text-to-speech feature not ready!\nTo, set up, either:\n* install 'VLC player'\n* install 'pygame'\n* define 'ttsCommand' in config.py")
+        self.print("Read more at:\nhttps://github.com/eliranwong/letmedoit/wiki/letMeDoIt-Speaks")
+        return False
 
     def toggleinputaudio(self):
         if self.isTtsAvailable:
             config.ttsInput = not config.ttsInput
             config.saveConfig()
             self.print3(f"Input Audio: '{'enabled' if config.ttsInput else 'disabled'}'!")
 
     def toggleresponseaudio(self):
         if self.isTtsAvailable:
             config.ttsOutput = not config.ttsOutput
             config.saveConfig()
             self.print3(f"Response Audio: '{'enabled' if config.ttsOutput else 'disabled'}'!")
 
     def defineTtsCommand(self):
-        self.print("Define custom text-to-speech command below:")
+        self.print("Define text-to-speech command below:")
         self.print("""* on macOS ['say -v "?"' to check voices], e.g.:\n'say' or 'say -r 200 -v Daniel'""")
         self.print("* on Ubuntu ['espeak --voices' to check voices], e.g.:\n'espeak' or 'espeak -s 175 -v en-gb'")
         self.print("* on Windows, simply enter 'windows' here to use Windows built-in speech engine") # letmedoit.ai will handle the command for Windows users
         self.print("remarks: always place the voice option, if any, at the end")
         ttsCommand = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default=config.ttsCommand)
         if ttsCommand:
             self.print("Specify command suffix below, if any [leave it blank if N/A]:")
@@ -1071,145 +1372,25 @@
             self.print("Please specify the writing style below:")
             style = self.prompts.simplePrompt(style=self.prompts.promptStyle2, default=config.improvedWritingSytle)
             if style and not style in (config.exit_entry, config.cancel_entry):
                 config.improvedWritingSytle = style
                 config.saveConfig()
         self.print3(f"Improved Writing Display: '{'enabled' if config.displayImprovedWriting else 'disabled'}'!")
 
-    def setAudioPlaybackTool(self):
-        playback = self.dialogs.getValidOptions(
-            options=("pygame", "vlc"),
-            descriptions=("PyGame", f"VLC Player (w/ speed control){' [installation required]' if not config.isVlcPlayerInstalled else ''}"),
-            title="Text-to-Speech Playback",
-            text="Select a text-to-speech plackback tool:",
-            default="vlc" if config.isVlcPlayerInstalled and not config.usePygame else "pygame",
-        )
-        if playback:
-            if playback == "vlc":
-                if not config.isVlcPlayerInstalled:
-                    self.print("VLC player not found! Install it first!")
-                    self.print3("Text-to-Speech Playback changed to: PyGame")
-                    config.usePygame = True
-                else:
-                    config.usePygame = False
-            else:
-                config.usePygame = True
-
-    def setTextToSpeechConfig(self):
-        ttsPlatform = self.dialogs.getValidOptions(
-            options=("google", "googlecloud", "elevenlabs", "custom"),
-            descriptions=("Google Text-to-Speech (Generic)", "Google Text-to-Speech (API)", "ElevenLabs (API)", "Custom Text-to-Speech Command [advanced]"),
-            title="Text-to-Speech Configurations",
-            text="Select a text-to-speech platform:",
-            default=config.ttsPlatform,
-        )
-        if ttsPlatform:
-            if ttsPlatform == "googlecloud" and not (os.environ["GOOGLE_APPLICATION_CREDENTIALS"] and "Text-to-Speech" in config.enabledGoogleAPIs):
-                self.print2("Google Cloud Text-to-Speech feature is not enabled!")
-                self.print3("Read: https://github.com/eliranwong/letmedoit/wiki/Google-API-Setup")
-                self.print3("Text-to-Speech platform changed to: Google Text-to-Speech (Generic)")
-                config.ttsPlatform = "google"
-            else:
-                config.ttsPlatform = ttsPlatform
-        # further options
-        if config.ttsPlatform == "google":
-            self.setGttsLanguage()
-            self.setAudioPlaybackTool()
-            self.setVlcSpeed()
-        elif config.ttsPlatform == "googlecloud":
-            self.setGcttsLanguage()
-            self.setGcttsSpeed()
-            self.setAudioPlaybackTool()
-            self.setVlcSpeed()
-        elif config.ttsPlatform == "elevenlabs":
-            if not config.elevenlabsApi:
-                self.changeElevenlabsApi()
-            if not config.elevenlabsApi:
-                self.print("ElevenLabs API key not found!")
-                self.print3("Text-to-Speech platform changed to: Google Text-to-Speech (Generic)")
-                config.ttsPlatform = "google"
-            else:
-                self.setElevenlabsVoice()
-        elif config.ttsPlatform == "custom":
-            self.defineTtsCommand()
-        # save configs
-        config.saveConfig()
-
-    def setVoiceTypingConfig(self):
-        voiceTypingPlatform = self.dialogs.getValidOptions(
-            options=("google", "googlecloud", "whisper"),
-            descriptions=("Google Speech-to-Text (Generic) [online]", "Google Speech-to-Text (API) [online]", "OpenAI Whisper [offline; slower with non-English voices]"),
-            title="Voice Typing Configurations",
-            text="Select a voice typing platform:",
-            default=config.voiceTypingPlatform,
-        )
-        if voiceTypingPlatform:
-            if voiceTypingPlatform == "googlecloud" and not (os.environ["GOOGLE_APPLICATION_CREDENTIALS"] and "Speech-to-Text" in config.enabledGoogleAPIs):
-                self.print2("Google Cloud Speech-to-Text feature is not enabled!")
-                self.print3("Read: https://github.com/eliranwong/letmedoit/wiki/Google-API-Setup")
-                self.print3("Voice typing platform changed to: Google Speech-to-Text (Generic)")
-                config.voiceTypingPlatform = "google"
-            elif voiceTypingPlatform == "whisper" and not SharedUtil.isPackageInstalled("ffmpeg"):
-                self.print2("Install 'ffmpeg' first to use offline openai whisper model!")
-                self.print3("Read: https://github.com/openai/whisper#setup")
-                self.print3("Voice typing platform changed to: Google Speech-to-Text (Generic)")
-                config.voiceTypingPlatform = "google"
-            else:
-                config.voiceTypingPlatform = voiceTypingPlatform
-        # language
-        self.setSpeechToTextLanguage()
-        # configure config.voiceTypingAdjustAmbientNoise
-        voiceTypingAdjustAmbientNoise = self.dialogs.getValidOptions(
-            options=("Yes", "No"),
-            descriptions=("Yes [slower]", "No"),
-            title="Adjust Ambient Noise",
-            text="Do you want to adjust ambient noise?",
-            default="Yes" if config.voiceTypingAdjustAmbientNoise else "No",
-        )
-        if voiceTypingAdjustAmbientNoise:
-            config.voiceTypingAdjustAmbientNoise = True if voiceTypingAdjustAmbientNoise == "Yes" else False
-        # audio notification
-        voiceTypingNotification = self.dialogs.getValidOptions(
-            options=("Yes", "No"),
-            title="Audio Notification",
-            text="Do you want audio notification when you use microphone?",
-            default="Yes" if config.voiceTypingNotification else "No",
-        )
-        if voiceTypingNotification:
-            config.voiceTypingNotification = True if voiceTypingNotification == "Yes" else False
-        # auto completion: voiceTypingAutoComplete
-        voiceTypingAutoComplete = self.dialogs.getValidOptions(
-            options=("Yes", "No"),
-            title="Audio Entry Auto Completion",
-            text="Do you want to automatically complete your entry when microphone stops?",
-            default="Yes" if config.voiceTypingAutoComplete else "No",
-        )
-        if voiceTypingAutoComplete:
-            config.voiceTypingAutoComplete = True if voiceTypingAutoComplete == "Yes" else False
-        # notify
-        print("")
-        self.print3(f"Voice Typing Model: {config.voiceTypingPlatform}")
-        self.print3(f"Voice Typing Language: {config.voiceTypingLanguage}")
-        self.print3(f"Ambient Noise Adjustment: {config.voiceTypingAdjustAmbientNoise}")
-        self.print3(f"Audio Notification: {config.voiceTypingNotification}")
-        self.print3(f"Auto Completion: {config.voiceTypingAutoComplete}")
-        # save configs
-        config.saveConfig()
-
     def saveChat(self, messages):
         if config.conversationStarted:
             timestamp = SharedUtil.getCurrentDateTime()
 
             if hasattr(config, "save_chat_record"):
                 # when plugin "save chat records" is enabled
                 for order, i in enumerate(messages):
                     config.save_chat_record(timestamp, order, i)
 
             try:
-                folderPath = os.path.join(SharedUtil.getLocalStorage(), "chats", re.sub("^([0-9]+?\-[0-9]+?)\-.*?$", r"\1", timestamp))
+                folderPath = os.path.join(self.getFiles(), "chats", re.sub("^([0-9]+?\-[0-9]+?)\-.*?$", r"\1", timestamp))
                 Path(folderPath).mkdir(parents=True, exist_ok=True)
                 if os.path.isdir(folderPath):
                     chatFile = os.path.join(folderPath, f"{timestamp}.txt")
                     with open(chatFile, "w", encoding="utf-8") as fileObj:
                         fileObj.write(pprint.pformat(messages))
             except:
                 self.print2("Failed to save chat!\n")
@@ -1238,15 +1419,15 @@
                             plainText += "\n\n"
                         plainText += f"{content}\n\n"
             plainText = plainText.strip()
             if config.terminalEnableTermuxAPI:
                 pydoc.pipepager(plainText, cmd="termux-share -a send")
             else:
                 try:
-                    folderPath = os.path.join(SharedUtil.getLocalStorage(), "chats", "export")
+                    folderPath = os.path.join(self.getFiles(), "chats", "export")
                     Path(folderPath).mkdir(parents=True, exist_ok=True)
                     if os.path.isdir(folderPath):
                         chatFile = os.path.join(folderPath, f"{timestamp}.txt")
                         with open(chatFile, "w", encoding="utf-8") as fileObj:
                             fileObj.write(plainText)
                         if openFile and os.path.isfile(chatFile):
                             os.system(f'''{config.open} "{chatFile}"''')
@@ -1325,33 +1506,32 @@
             return config.dynamicToolBarText
         def startChat():
             clear()
             self.print(self.divider)
             self.showLogo()
             self.showCurrentContext()
             # go to startup directory
-            storagedirectory = SharedUtil.getLocalStorage()
+            storagedirectory = self.getFiles()
             os.chdir(storagedirectory)
-            messages = SharedUtil.resetMessages()
+            messages = self.resetMessages()
             #self.print(f"startup directory:\n{storagedirectory}")
             print_formatted_text(HTML(f"<{config.terminalPromptIndicatorColor2}>Directory:</{config.terminalPromptIndicatorColor2}> {storagedirectory}"))
             self.print(self.divider)
 
             config.conversationStarted = False
             return (storagedirectory, messages)
         storagedirectory, config.currentMessages = startChat()
         config.multilineInput = False
         featuresLower = list(self.actions.keys()) + ["..."]
-        # input suggestions
         config.inputSuggestions += featuresLower
-        completer = FuzzyCompleter(WordCompleter(config.inputSuggestions, ignore_case=True)) if config.inputSuggestions else None
-        completer_developer = FuzzyCompleter(WordCompleter(config.inputSuggestions[:] + [f"config.{i}" for i in dir(config) if not i.startswith("__")] + self.getDirectoryList(), ignore_case=True))
+        if config.developer:
+            config.inputSuggestions += [f"config.{i}" for i in dir(config) if not i.startswith("__")]
         while True:
             # default toolbar text
-            config.dynamicToolBarText = f""" {str(config.hotkey_exit).replace("'", "")} exit {str(config.hotkey_display_key_combo).replace("'", "")} shortcuts """
+            config.dynamicToolBarText = " [ctrl+q] exit [ctrl+k] shortcuts "
             # display current directory if changed
             currentDirectory = os.getcwd()
             if not currentDirectory == storagedirectory:
                 #self.print(self.divider)
                 self.print3(f"Current directory: {currentDirectory}")
                 self.print(self.divider)
                 storagedirectory = currentDirectory
@@ -1360,17 +1540,18 @@
             config.accept_default = False
             defaultEntry = config.defaultEntry
             if os.path.isfile(defaultEntry):
                 defaultEntry = f'File: "{defaultEntry}"\n'
             elif os.path.isdir(defaultEntry):
                 defaultEntry = f'Folder: "{defaultEntry}"\n'
             config.defaultEntry = ""
-
-            # user input
-            userInput = self.prompts.simplePrompt(promptSession=self.terminal_chat_session, completer=completer_developer if config.developer else completer, default=defaultEntry, accept_default=accept_default, validator=tokenValidator, bottom_toolbar=getDynamicToolBar)
+            # input suggestions
+            inputSuggestions = config.inputSuggestions[:] + self.getDirectoryList() if config.developer else config.inputSuggestions
+            completer = FuzzyCompleter(WordCompleter(inputSuggestions, ignore_case=True)) if inputSuggestions else None
+            userInput = self.prompts.simplePrompt(promptSession=self.terminal_chat_session, completer=completer, default=defaultEntry, accept_default=accept_default, validator=tokenValidator, bottom_toolbar=getDynamicToolBar)
             
             # update system message when user enter a new input
             config.currentMessages = self.updateSystemMessage(config.currentMessages)
             
             # display options when empty string is entered
             userInputLower = userInput.lower()
             if config.addPathAt is not None:
@@ -1413,42 +1594,41 @@
                     self.print3(f"Directory changed to: {docs_path}")
                     self.getPath.displayDirectoryContent()
                     continue
                 except:
                     pass
 
             # try eval
-            if config.developer and not userInput == "...":
+            if not userInput == "...":
                 try:
                     value = eval(userInput) # it solve simple math, e.g. 1+1, or read variables, e.g. dir(config)
                     if value is not None:
                         #print(value)
                         pprint.pprint(value)
                         print("")
                         continue
                     elif re.search("^print\([^\)\)]+?\)$", userInput):
                         print("")
                         continue
                 except:
                     pass
             # try to run as a python script first
-            if config.developer:
-                try:
-                    exec(userInput, globals())
-                    print("")
-                    continue
-                except:
-                    pass
+            try:
+                exec(userInput, globals())
+                print("")
+                continue
+            except:
+                pass
 
             if userInput.startswith("!"):
                 self.runSystemCommand(userInput)
                 print("")
-            elif config.developer and userInput.startswith("```") and userInput.endswith("```") and not userInput == "``````":
+            elif userInput.startswith("```") and userInput.endswith("```") and not userInput == "``````":
                 userInput = re.sub("```python", "```", userInput)
-                SharedUtil.runPythonScript(userInput)
+                self.runPythonScript(userInput)
                 print("")
             elif userInputLower == config.exit_entry:
                 self.saveChat(config.currentMessages)
                 return self.exitAction()
             elif userInputLower == config.cancel_entry:
                 pass
             elif userInputLower == ".context":
@@ -1517,37 +1697,37 @@
                         # call the spcified chatbot to continue the conversation
                         fineTunedUserInput = re.sub("\[CHAT\]|\[CHAT_[^\[\]]+?\]", "", fineTunedUserInput)
                         self.launchChatbot(chatbot, fineTunedUserInput)
                         continue
                     # if user don't want function call or a particular function call
                     noFunctionCall = ("[NO_FUNCTION_CALL]" in fineTunedUserInput)
                     checkCallSpecificFunction = re.search("\[CALL_([^\[\]]+?)\]", fineTunedUserInput)
-                    config.runSpecificFuntion = checkCallSpecificFunction.group(1) if checkCallSpecificFunction and checkCallSpecificFunction.group(1) in config.chatGPTApiAvailableFunctions else ""
+                    config.runSpecificFuntion = checkCallSpecificFunction.group(1) if checkCallSpecificFunction and checkCallSpecificFunction.group(1) in config.pluginsWithFunctionCall else ""
                     if config.developer and config.runSpecificFuntion:
                         #self.print(f"calling function '{config.runSpecificFuntion}' ...")
                         print_formatted_text(HTML(f"<{config.terminalPromptIndicatorColor2}>Calling function</{config.terminalPromptIndicatorColor2}> <{config.terminalCommandEntryColor2}>'{config.runSpecificFuntion}'</{config.terminalCommandEntryColor2}> <{config.terminalPromptIndicatorColor2}>...</{config.terminalPromptIndicatorColor2}>"))
                     fineTunedUserInput = re.sub(specialEntryPattern, "", fineTunedUserInput)
                     config.currentMessages.append({"role": "user", "content": fineTunedUserInput})
 
                     # start spinning
                     config.stop_event = threading.Event()
                     config.spinner_thread = threading.Thread(target=self.spinning_animation, args=(config.stop_event,))
                     config.spinner_thread.start()
 
                     # force loading internet searches
                     if config.loadingInternetSearches == "always":
                         try:
-                            config.currentMessages = SharedUtil.runFunction(config.currentMessages, [config.chatGPTApiFunctionSignatures["integrate_google_searches"]], "integrate_google_searches")
+                            config.currentMessages = self.runFunction(config.currentMessages, config.integrate_google_searches_signature, "integrate_google_searches")
                         except:
                             self.print("Unable to load internet resources.")
                             SharedUtil.showErrors()
 
-                    completion = SharedUtil.runCompletion(config.currentMessages, noFunctionCall)
+                    completion = self.runCompletion(config.currentMessages, noFunctionCall)
                     # stop spinning
-                    config.runPython = True
+                    self.runPython = True
                     self.stopSpinning()
 
                     # Create a new thread for the streaming task
                     streamingWordWrapper = StreamingWordWrapper()
                     streaming_event = threading.Event()
                     self.streaming_thread = threading.Thread(target=streamingWordWrapper.streamOutputs, args=(streaming_event, completion, True))
                     # Start the streaming thread
```

### Comparing `letmedoit-2.1.84/letmedoit/utils/get_path_prompt.py` & `letmedoit-2.1.9/letmedoit/utils/get_path_prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,32 +151,37 @@
                 from prompt_toolkit.filters import Condition
 
                 filePathHistory = os.path.join(config.historyParentFolder if config.historyParentFolder else config.letMeDoItAIFolder, "history", "paths")
                 filePathSession = PromptSession(history=FileHistory(filePathHistory))
 
                 # key bindings
                 this_key_bindings = KeyBindings()
-
-                @this_key_bindings.add(*config.hotkey_exit)
+                """
+                if self.ctrl_s_to_system:
+                    @this_key_bindings.add("c-s")
+                    def _(event):
+                        event.app.current_buffer.text = ".system"
+                        event.app.current_buffer.validate_and_handle()"""
+                @this_key_bindings.add("c-q")
                 def _(event):
                     #if self.ctrl_q_to_exit:
                     #    event.app.current_buffer.text = ".quit"
                     #else:
                     #    event.app.current_buffer.text = self.cancel_entry
                     event.app.current_buffer.text = self.cancel_entry
                     event.app.current_buffer.validate_and_handle()
-                @this_key_bindings.add(*config.hotkey_cancel)
+                @this_key_bindings.add("c-z")
                 def _(event):
                     buffer = event.app.current_buffer
                     buffer.reset()
-                @this_key_bindings.add(*config.hotkey_list_directory_content)
+                @this_key_bindings.add("c-l")
                 def _(_):
                     # list directories and files
                     run_in_terminal(lambda: self.displayDirectoryContent(display_dir_only=display_dir_only))
-                @this_key_bindings.add(*config.hotkey_toggle_mouse_support)
+                @this_key_bindings.add("escape", "m")
                 def _(_):
                     config.mouseSupport = not config.mouseSupport
                     run_in_terminal(lambda: config.print(f"Entry Mouse Support '{'enabled' if config.mouseSupport else 'disabled'}'!"))
 
                 inputIndicator = [("class:indicator", indicator)]
                 completer = PathCompleter()
                 auto_suggestion=AutoSuggestFromHistory()
@@ -187,15 +192,15 @@
                     "indicator": self.promptIndicatorColor,
                 })
                 this_key_bindings = merge_key_bindings([
                     this_key_bindings,
                     #prompt_shared_key_bindings,
                 ])
                 if not bottom_toolbar:
-                    bottom_toolbar = f""" {str(config.hotkey_exit).replace("'", "")} exit {str(config.hotkey_list_directory_content).replace("'", "")} list content [cd <dir>] change dir """
+                    bottom_toolbar = " [ctrl+q] exit [ctrl+l] list content [cd <dir>] change dir "
                 userInput = filePathSession.prompt(
                     inputIndicator,
                     default=default,
                     style=promptStyle,
                     key_bindings=this_key_bindings,
                     auto_suggest=auto_suggestion,
                     completer=completer,
```

### Comparing `letmedoit-2.1.84/letmedoit/utils/install.py` & `letmedoit-2.1.9/letmedoit/utils/install.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/utils/promptValidator.py` & `letmedoit-2.1.9/letmedoit/utils/promptValidator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from letmedoit import config
 from letmedoit.utils.shared_utils import SharedUtil
 from prompt_toolkit.validation import Validator, ValidationError
 from prompt_toolkit.application import run_in_terminal
-import tiktoken
+#from prompt_toolkit.application import get_app
+try:
+    import tiktoken
+    tiktokenImported = True
+except:
+    tiktokenImported = False
 import re
 
 class TokenValidator(Validator):
     def validate(self, document):
         #current_buffer = get_app().current_buffer
         currentInput = document.text
         if not config.dynamicTokenCount or not currentInput or currentInput.lower() in (config.exit_entry, config.cancel_entry, ".new", ".share", ".save"):
             pass
-        else:
+        elif tiktokenImported:
             try:
                 encoding = tiktoken.encoding_for_model(config.chatGPTApiModel)
             except:
                 encoding = tiktoken.get_encoding("cl100k_base")
             no_function_call_pattern = "\[NO_FUNCTION_CALL\]|\[CHAT\]|\[CHAT_[^\[\]]+?\]"
             #if "[NO_FUNCTION_CALL]" in currentInput:
             if re.search(no_function_call_pattern, currentInput):
@@ -25,22 +30,24 @@
             else:
                 availableFunctionTokens = SharedUtil.count_tokens_from_functions(config.chatGPTApiFunctionSignatures)
             currentInputTokens = len(encoding.encode(config.fineTuneUserInput(currentInput)))
             loadedMessageTokens = SharedUtil.count_tokens_from_messages(config.currentMessages)
             selectedModelLimit = SharedUtil.tokenLimits[config.chatGPTApiModel]
             #estimatedAvailableTokens = selectedModelLimit - availableFunctionTokens - loadedMessageTokens - currentInputTokens
 
-            config.dynamicToolBarText = f""" Tokens: {(availableFunctionTokens + loadedMessageTokens + currentInputTokens)}/{selectedModelLimit} {str(config.hotkey_display_key_combo).replace("'", "")} shortcuts """
+            config.dynamicToolBarText = f" Tokens: {(availableFunctionTokens + loadedMessageTokens + currentInputTokens)}/{selectedModelLimit} [ctrl+k] shortcuts "
             #if config.conversationStarted:
             #    config.dynamicToolBarText = config.dynamicToolBarText + " [ctrl+n] new"
             if selectedModelLimit - (availableFunctionTokens + loadedMessageTokens + currentInputTokens) >= config.chatGPTApiMinTokens:
                 pass
             else:
-                run_in_terminal(lambda: print(f"""Press '{str(config.hotkey_new).replace("'", "")[1:-1]}' to start a new chat!"""))
+                run_in_terminal(lambda: print("Press 'ctrl+n' to start a new chat!"))
                 raise ValidationError(message='Token limit reached!', cursor_position=document.cursor_position)
+        else:
+            pass
 
 class NumberValidator(Validator):
     def validate(self, document):
         text = document.text
 
         if text.lower() in (config.exit_entry, config.cancel_entry):
             pass
```

### Comparing `letmedoit-2.1.84/letmedoit/utils/prompt_multiline_shared_key_bindings.py` & `letmedoit-2.1.9/letmedoit/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/utils/prompt_shared_key_bindings.py` & `letmedoit-2.1.9/letmedoit/utils/prompt_shared_key_bindings.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,21 +50,18 @@
 @prompt_shared_key_bindings.add("c-x")
 def _(event):
     buffer = event.app.current_buffer
     data = buffer.cut_selection()
     # remarks: set_data does not work
     config.clipboard.set_text(data.text)
 # insert linebreak
-@prompt_shared_key_bindings.add(*config.hotkey_insert_newline)
+@prompt_shared_key_bindings.add("c-r")
 def _(event):
     buffer = event.app.current_buffer
-    if config.multilineInput:
-        buffer.validate_and_handle()
-    else:
-        buffer.newline()
+    buffer.insert_text("\n")
 
 # navigation
 
 # go to current line starting position
 @prompt_shared_key_bindings.add("escape", "b")
 def _(event):
     buffer = event.app.current_buffer
@@ -92,23 +89,23 @@
 # go to the beginning of the text
 @prompt_shared_key_bindings.add("escape", "a")
 def _(event):
     buffer = event.app.current_buffer
     buffer.cursor_position = 0
 
 # reset buffer
-@prompt_shared_key_bindings.add(*config.hotkey_cancel)
+@prompt_shared_key_bindings.add("c-z")
 def _(event):
     buffer = event.app.current_buffer
     buffer.reset()
 
 # open current input in built-in or custom text editor
 # place this method here so that terminal or other input can share this binding
 #@prompt_shared_key_bindings.add("escape", "o")
-@prompt_shared_key_bindings.add(*config.hotkey_edit_current_entry)
+@prompt_shared_key_bindings.add("c-e")
 def _(event):
     customTextEditor = config.customTextEditor if config.customTextEditor else f"{sys.executable} {os.path.join(config.letMeDoItAIFolder, 'eTextEdit.py')}"
     current_buffer = event.app.current_buffer
     text = current_buffer.text
     filename = os.path.join(config.letMeDoItAIFolder, "temp", "current_input.txt")
     with open(filename, "w", encoding="utf-8") as fileObj:
         fileObj.write(text)
@@ -117,15 +114,15 @@
         editedText = fileObj.read()
     editedText = re.sub("\n$", "", editedText)
     current_buffer.text = editedText
     current_buffer.cursor_position = len(editedText)
     set_title(config.letMeDoItName)
 
 # swap color theme
-@prompt_shared_key_bindings.add(*config.hotkey_swap_text_brightness)
+@prompt_shared_key_bindings.add("escape", "s")
 def _(_):
     swapTerminalColors()
 
 @staticmethod
 def swapTerminalColors():
     if config.terminalResourceLinkColor in config.terminalColors:
         config.terminalResourceLinkColor = config.terminalColors[config.terminalResourceLinkColor]
```

### Comparing `letmedoit-2.1.84/letmedoit/utils/shortcuts.py` & `letmedoit-2.1.9/letmedoit/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/utils/streaming_word_wrapper.py` & `letmedoit-2.1.9/letmedoit/utils/streaming_word_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from letmedoit import config
 from letmedoit.health_check import HealthCheck
 from letmedoit.utils.tts_utils import TTSUtil
+if not hasattr(config, "exit_entry"):
+    HealthCheck.setBasicConfig()
+    HealthCheck.saveConfig()
+    print("Configurations updated!")
+HealthCheck.setPrint()
 #import pygments
 #from pygments.lexers.markup import MarkdownLexer
 #from prompt_toolkit.formatted_text import PygmentsTokens
 #from prompt_toolkit import print_formatted_text
 from prompt_toolkit.keys import Keys
 from prompt_toolkit.input import create_input
-import asyncio, shutil, textwrap, re
+import asyncio, shutil, textwrap, string
 
 
 class StreamingWordWrapper:
 
     def __init__(self):
         self.streaming_finished = False
         config.tempChunk = ""
@@ -113,26 +118,19 @@
         self.lineWidth = 0
         blockStart = False
         wrapWords = config.wrapWords
         firstEvent = True
         for event in completion:
             if not streaming_event.is_set() and not self.streaming_finished:
                 # RETRIEVE THE TEXT FROM THE RESPONSE
-                if openai:
-                    # openai
-                    answer = event.choices[0].delta.content
-                elif isinstance(event, dict):
-                    # ollama chat
-                    answer = event['message']['content']
-                else:
-                    # vertex ai
-                    answer = event.text
+                # openai or vertex
+                answer = event.choices[0].delta.content if openai else event.text
                 # transform
-                if hasattr(config, "outputTransformers"):
-                    for transformer in config.outputTransformers:
+                if hasattr(config, "chatGPTTransformers"):
+                    for transformer in config.chatGPTTransformers:
                         answer = transformer(answer)
                 # STREAM THE ANSWER
                 if answer is not None:
                     if firstEvent:
                         firstEvent = False
                         answer = answer.lstrip()
                     # display the chunk
@@ -159,23 +157,19 @@
                         print(answer, end='', flush=True) # Print the response
                     # speak streaming words
                     self.readAnswer(answer)
             else:
                 finishOutputs(wrapWords, chat_response)
                 return None
         
-        if config.ttsOutput and config.tempChunk:
-            TTSUtil.play(config.tempChunk)
-            config.tempChunk = ""
         finishOutputs(wrapWords, chat_response)
 
     def readAnswer(self, answer):
         # read the chunk when there is a punctuation
-        #if answer in string.punctuation and config.tempChunk:
-        if re.search(config.tts_readWhenStreamContains, answer) and config.tempChunk:
+        if answer in string.punctuation and config.tempChunk:
             # read words when there a punctuation
             chunk = config.tempChunk + answer
             # reset config.tempChunk
             config.tempChunk = ""
             # play with tts
             if config.ttsOutput:
                 TTSUtil.play(chunk)
```

### Comparing `letmedoit-2.1.84/letmedoit/utils/terminal_mode_dialogs.py` & `letmedoit-2.1.9/letmedoit/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/utils/terminal_system_command_prompt.py` & `letmedoit-2.1.9/letmedoit/utils/terminal_system_command_prompt.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             "indicator": config.terminalPromptIndicatorColor2,
         })
         system_command_history = os.path.join(config.historyParentFolder if config.historyParentFolder else config.letMeDoItAIFolder, "history", "commands")
         self.terminal_system_command_session = PromptSession(history=FileHistory(system_command_history))
         self.openCommand = config.open
 
     def getToolBar(self):
-        return f""" {str(config.hotkey_exit).replace("'", "")} exit {str(config.hotkey_list_directory_content).replace("'", "")} list content {str(config.hotkey_insert_filepath).replace("'", "")} insert path """
+        return " [ctrl+q] exit [ctrl+l] list content [ctrl+i] insert path "
 
     def getSystemCommands(self):
         try:
             options = subprocess.Popen("bash -c 'compgen -ac | sort'", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             stdout, *_ = options.communicate()
             options = stdout.decode("utf-8").split("\n")
             options = [option for option in options if option and not option in ("{", "}", ".", "!", ":")]
@@ -47,45 +47,40 @@
         except:
             return []
 
     def run(self, allowPathChanges=False):
         self.runSystemCommandPrompt = True
         # initial message
         print_formatted_text(HTML(f"<{config.terminalCommandEntryColor1}>You are currently running system command prompt!</{config.terminalCommandEntryColor1}>"))
-        config.print(f"""To exit, either press '{str(config.hotkey_exit).replace("'", "")[1:-1]}' or enter '{config.exit_entry}'.""")
+        config.print(f"To exit, either press 'ctrl+q' or enter '{config.exit_entry}'.")
         # keep current path in case users change directory
         startupDirectory = self.previousDirectory = self.currentDirectory = os.getcwd()
 
         this_key_bindings = KeyBindings()
 
-        @this_key_bindings.add(*config.hotkey_exit)
+        @this_key_bindings.add("c-q")
         def _(event):
-            buffer = event.app.current_buffer
-            buffer.text = config.exit_entry
-            buffer.validate_and_handle()
-        @this_key_bindings.add(*config.hotkey_cancel)
-        def _(event):
-            buffer = event.app.current_buffer
-            buffer.reset()
-        @this_key_bindings.add(*config.hotkey_list_directory_content)
+            event.app.current_buffer.text = config.exit_entry
+            event.app.current_buffer.validate_and_handle()
+        @this_key_bindings.add("c-l")
         def _(_):
             config.print("")
             run_in_terminal(lambda: self.getPath.displayDirectoryContent())
-        @this_key_bindings.add(*config.hotkey_insert_filepath)
+        @this_key_bindings.add("c-i")
         def _(event):
             self.addPath = True
             buffer = event.app.current_buffer
             self.systemCommandPromptEntry = buffer.text
             self.systemCommandPromptPosition = buffer.cursor_position
             buffer.validate_and_handle()
-        @this_key_bindings.add(*config.hotkey_insert_newline)
+        @this_key_bindings.add("c-r")
         def _(event):
             buffer = event.app.current_buffer
-            buffer.newline()
-        @this_key_bindings.add(*config.hotkey_toggle_mouse_support)
+            buffer.insert_text("\n")
+        @this_key_bindings.add("escape", "m")
         def _(_):
             config.mouseSupport = not config.mouseSupport
             run_in_terminal(lambda: config.print(f"Entry Mouse Support '{'enabled' if config.mouseSupport else 'disabled'}'!"))
 
         this_key_bindings = merge_key_bindings([
             this_key_bindings,
             prompt_shared_key_bindings,
```

### Comparing `letmedoit-2.1.84/letmedoit/utils/text_utils.py` & `letmedoit-2.1.9/letmedoit/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit/utils/tts_utils.py` & `letmedoit-2.1.9/letmedoit/utils/tts_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 from letmedoit import config
-import os, traceback, subprocess, re, sounddevice, soundfile
+import os, traceback, subprocess, re
 from gtts import gTTS
-from elevenlabs import generate, play
 from letmedoit.utils.vlc_utils import VlcUtil
 try:
     from google.cloud import texttospeech
 except:
     pass
 try:
     # hide pygame welcome message
     os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
     import pygame
-    if pygame.mixer.get_init() is None:
-        pygame.mixer.init()
-    config.isPygameInstalled = True
 except:
     config.usePygame = False
-    config.isPygameInstalled = True
 
 class TTSUtil:
 
     @staticmethod
     def play(content, language=""):
         if config.tts:
             try:
+                credentials_GoogleCloudTextToSpeech = os.path.join(config.letMeDoItAIFolder, "credentials_GoogleCloudTextToSpeech.json")
                 # official google-cloud-texttospeech
-                if config.ttsPlatform == "googlecloud" and os.environ["GOOGLE_APPLICATION_CREDENTIALS"] and "Text-to-Speech" in config.enabledGoogleAPIs:
+                if os.path.isfile(credentials_GoogleCloudTextToSpeech):
+                    os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = credentials_GoogleCloudTextToSpeech
                     audioFile = os.path.join(config.letMeDoItAIFolder, "temp", "gctts.mp3")
                     if not language:
                         language = config.gcttsLang
                     elif language == "yue":
                         language = "yue-HK"
                     elif "-" in language:
                         language, accent = language.split("-", 1)
                         language = f"{language}-{accent.upper()}"
                     TTSUtil.saveCloudTTSAudio(content, language, filename=audioFile)
                     TTSUtil.playAudioFile(audioFile)
-                elif config.ttsPlatform == "custom" and config.ttsCommand:
+                elif config.ttsCommand:
                     # remove '"' from the content
                     content = re.sub('"', "", content)
 
                     # Windows users
                     # https://stackoverflow.com/questions/1040655/ms-speech-from-command-lines
                     # https://www.powerofpowershell.com/post/powershell-can-speak-too#:~:text=The%20Add%2DType%20cmdlet%20is,want%20to%20convert%20into%20speech.
                     windows = (config.ttsCommand.lower() == "windows")
@@ -55,26 +52,15 @@
                             command = f'''{ttsCommand} "{content}"{config.ttsCommandSuffix}'''
                     else:
                         if windows:
                             command = f'''PowerShell -Command "Add-Type –AssemblyName System.Speech; (New-Object System.Speech.Synthesis.SpeechSynthesizer).Speak('{content}');"'''
                         else:
                             command = f'''{config.ttsCommand} "{content}"{config.ttsCommandSuffix}'''
                     subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE).communicate()
-                elif config.ttsPlatform == "elevenlabs" and config.elevenlabsApi:
-                    audio = generate(
-                        api_key=config.elevenlabsApi, # Defaults to os.getenv(ELEVEN_API_KEY)
-                        text=content,
-                        voice="Rachel",
-                        model="eleven_multilingual_v2"
-                    )
-                    play(audio)
                 else:
-                    if not config.ttsPlatform == "google":
-                        config.ttsPlatform == "google"
-                        config.saveConfig()
                     # use gTTS as default as config.ttsCommand is empty by default
                     if not language:
                         language = config.gttsLang
                     elif language == "yue":
                         language = "zh"
                     elif "-" in language:
                         language = re.sub("^(.*?)\-.*?$", r"\1", language)
@@ -90,20 +76,17 @@
 
     @staticmethod
     def playAudioFile(audioFile):
         try:
             if config.isVlcPlayerInstalled and not config.usePygame:
                 # vlc is preferred as it allows speed control with config.vlcSpeed
                 VlcUtil.playMediaFile(audioFile)
-            elif config.isPygameInstalled:
+            else:
                 # use pygame if config.usePygame or vlc player is not installed
                 TTSUtil.playAudioFilePygame(audioFile)
-            else:
-                sounddevice.play(*soundfile.read(audioFile)) 
-                sounddevice.wait()
         except:
             command = f"{config.open} {audioFile}"
             subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE).communicate()
 
     @staticmethod
     def playAudioFilePygame(audioFile):
         pygame.mixer.music.load(audioFile)
```

### Comparing `letmedoit-2.1.84/letmedoit/utils/vlc_utils.py` & `letmedoit-2.1.9/letmedoit/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `letmedoit-2.1.84/letmedoit.egg-info/PKG-INFO` & `letmedoit-2.1.9/letmedoit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,156 +1,69 @@
 Metadata-Version: 2.1
 Name: letmedoit
-Version: 2.1.84
+Version: 2.1.9
 Summary: LetMeDoIt AI, an advanced AI assistant, leveraging the capabilities of ChatGPT API, Gemini Pro and AutoGen, capable of engaging in conversations, executing codes with auto-healing, and assisting you with a wide range of tasks on your local devices.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
 Project-URL: Documentation, https://github.com/eliranwong/letmedoit/wiki
-Project-URL: Funding, https://www.paypal.me/letmedoitai
+Project-URL: Funding, https://www.paypal.me/MarvelBible
 Keywords: ai assistant openai chatgpt gemini autogen rag interpreter auto-heal
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <3.12
-Requires-Dist: openai==1.19.0
-Requires-Dist: groq==0.5.0
-Requires-Dist: requests
-Requires-Dist: argparse
-Requires-Dist: pendulum
-Requires-Dist: folium
-Requires-Dist: seaborn[stats]
-Requires-Dist: sympy
-Requires-Dist: numpy
-Requires-Dist: prompt_toolkit
-Requires-Dist: Pygments
-Requires-Dist: datetime
-Requires-Dist: netifaces
-Requires-Dist: geocoder
-Requires-Dist: googlesearch-python
-Requires-Dist: art
-Requires-Dist: apsw
-Requires-Dist: gTTS
-Requires-Dist: google-cloud-speech
-Requires-Dist: google-cloud-texttospeech
-Requires-Dist: google-cloud-aiplatform==1.47.0
-Requires-Dist: pywhatkit
-Requires-Dist: yt-dlp
-Requires-Dist: rembg
-Requires-Dist: qrcode
-Requires-Dist: pyperclip
-Requires-Dist: colorama
-Requires-Dist: pillow
-Requires-Dist: docker
-Requires-Dist: einops
-Requires-Dist: transformers==4.40.1
-Requires-Dist: torch==2.2.2
-Requires-Dist: torchvision==0.17.2
-Requires-Dist: sentence-transformers
-Requires-Dist: chromadb==0.4.24
-Requires-Dist: unstructured[all-docs]
-Requires-Dist: pyautogen[autobuild,retrievechat]==0.2.24
-Requires-Dist: autogenstudio==0.0.56
-Requires-Dist: tiktoken
-Requires-Dist: pygame
-Requires-Dist: PySide6
-Requires-Dist: feedparser
-Requires-Dist: html2text
-Requires-Dist: pypdf
-Requires-Dist: PyMuPDF
-Requires-Dist: yfinance
-Requires-Dist: setuptools-rust
-Requires-Dist: SpeechRecognition
-Requires-Dist: openai-whisper
-Requires-Dist: soundfile==0.12.1
-Requires-Dist: sounddevice==0.4.6
-Requires-Dist: elevenlabs==1.0.3
-Requires-Dist: ollama==0.1.8
-Requires-Dist: llama-cpp-python[server]==0.2.61
-Requires-Dist: huggingface-hub
-Requires-Dist: langchain==0.1.13
-Requires-Dist: langchain_openai==0.1.3
-Requires-Dist: pydub
-Requires-Dist: stable-diffusion-cpp-python
-Requires-Dist: pytz
-Requires-Dist: geopy
-Requires-Dist: guidance==0.1.13
 
 # LetMeDoIt AI
 
 Welcome to LetMeDoIt AI, your premier virtual assistant designed to revolutionize the way you work! More than a mere chatbot, I am equipped with the capability to conduct meaningful interactions and actively carry out computing tasks as per your directives. My real-time code generation and execution prowess guarantees not only effectiveness but also efficiency in task fulfillment. With an advanced auto-correction feature, I autonomously repair any malfunctioning code segments and automatically install necessary libraries, ensuring uninterrupted workflow. My commitment to your digital safety is paramount, with inbuilt risk assessments and tailored user confirmation protocols to protect your data and device.
 
-With LetMeDoIt AI, you can access OpenAI ChatGPT-4, Google Gemini Pro, and Microsoft AutoGen, local LLMs, all in one place, to enhance your productivity. [Read more ...](https://github.com/eliranwong/letmedoit/wiki#letmedoit-ai)
+With LetMeDoIt AI, you can access OpenAI ChatGPT-4, Google Gemini Pro, and Microsoft AutoGen, all in one place, to enhance your productivity. [Read more ...](https://github.com/eliranwong/letmedoit/wiki#letmedoit-ai)
 
 Developer: [Eliran Wong](https://github.com/eliranwong)
 
 Website: https://LetMeDoIt.ai
 
 Source: https://github.com/eliranwong/letmedoit
 
 Installation: https://github.com/eliranwong/letmedoit/wiki/Installation
 
 Quick-Guide: https://github.com/eliranwong/letmedoit/wiki/Quick-Guide
 
 Wiki: https://github.com/eliranwong/letmedoit/wiki
 
-Video Demo: https://www.youtube.com/watch?v=Eeat6h_ktbQ&list=PLo4xQ5NqC8SEMM71xC4NNhOHJCFlW-jaJ
+Support this project: https://www.paypal.me/MarvelBible
 
-Support this project: https://www.paypal.me/letmedoitai
+# An Interview
 
-# Video Demo
+[![Watch the video](https://img.youtube.com/vi/Dfsl-Cxx0bQ/maxresdefault.jpg)](https://youtu.be/Dfsl-Cxx0bQ)
 
-[![Watch the video](https://img.youtube.com/vi/Eeat6h_ktbQ/maxresdefault.jpg)](https://youtu.be/Eeat6h_ktbQ)
-
-Youtube Playlist: https://www.youtube.com/watch?v=Eeat6h_ktbQ&list=PLo4xQ5NqC8SEMM71xC4NNhOHJCFlW-jaJ
-
-# LetMeDoIt Features without OpenAI?
-
-You can utilize Google Gemini or open-source LLMs through Ollama for chat features in the LetMeDoIt AI.
-
-If you're seeking the complete functionality of LetMeDoIt, which includes both chat and task execution features, without the need for an Open AI API key, we offer support for Gemini Pro, Ollama, and Llama.cpp in our related project, FreeGenius AI:
-
-https://github.com/eliranwong/freegenius
+Read more at: https://github.com/eliranwong/letmedoit/wiki#an-interview
 
 # Requirements
 
 1. ChatGPT API key (read https://github.com/eliranwong/letmedoit/wiki/ChatGPT-API-Key)
 
 2. [Python](https://www.python.org) version 3.8-3.11; read [Install a Supported Python Version](https://github.com/eliranwong/letmedoit/wiki/Install-a-Supported-Python-Version)
 
 3. Supported OS: Windows / macOS / Linux / ChromeOS / Android (Termux)
 
 # Recent Additions
 
-[Generate tweets](https://github.com/eliranwong/letmedoit/wiki/Social-Media)
-
-<img width="798" alt="twitter" src="https://github.com/eliranwong/letmedoit/assets/25262722/d19c7bca-3bdc-48be-a907-b75afb34615b">
-
-[Run Local LLM Offline](https://github.com/eliranwong/letmedoit/wiki/Run-Local-LLM-Offline)
-
-<img width="832" alt="support_localllm" src="https://github.com/eliranwong/letmedoit/assets/25262722/587aba21-7f89-4b78-bfc4-3b32b442b287">
-
-[Talk to LetMeDoIt in Multiple Languages](https://github.com/eliranwong/letmedoit/wiki/Speak-to-LetMeDoIt-AI)
-
-![talk_to_letmedoit](https://github.com/eliranwong/letmedoit/assets/25262722/6aa33f2d-8971-45ad-b5ac-e8f4e290bff5)
-
-[Analyze audio](https://github.com/eliranwong/letmedoit/wiki/Analyze-Audio)
-
-<img width="1440" alt="analyze_audio" src="https://github.com/eliranwong/letmedoit/assets/25262722/24e49f3b-289d-40f6-bf9c-45ed1e0eeed6">
-
 [Search / Analyze Financial Data](https://github.com/eliranwong/letmedoit/wiki/Search-Financial-Data)
 
 <img width="1312" alt="search_financial_data" src="https://github.com/eliranwong/letmedoit/assets/25262722/9976f15b-85e1-4c5b-97a0-5124c04ffa8a">
 
 [Access Weather Information](https://github.com/eliranwong/letmedoit/wiki/Search-Weather-Information)
 
 ![test_weather_plugin](https://github.com/eliranwong/letmedoit/assets/25262722/e9fd4376-1579-40e0-b1b2-a2b7c5583f0c)
@@ -237,22 +150,14 @@
 
 * developer mode available
 
 # Examples of Plugin Features (selective only):
 
 Latest LetMeDoIt Plugins allow you to acheive variety of tasks with natural language:
 
-* [NEW] generate tweets
-
-> Post a short tweet about LetMeDoIt AI
-
-* [NEW] analyze audio
-
-> transcribe "meeting_records.mp3"
-
 * [NEW] search / analyze financial data
 
 > What was the average stock price of Apple Inc. in 2023?
 
 > Analyze Apple Inc's stock price over last 5 years.
 
 * [NEW] search weather information
@@ -604,8 +509,10 @@
 
 > share text "Hello World!" on Android
 
 Read more at: https://github.com/eliranwong/letmedoit/wiki/Android-Support
 
 # Donations
 
-https://www.paypal.me/letmedoitai
+https://www.paypal.me/MarvelBible
+
+
```

### Comparing `letmedoit-2.1.84/letmedoit.egg-info/SOURCES.txt` & `letmedoit-2.1.9/letmedoit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,34 +10,25 @@
 letmedoit/commandprompt.py
 letmedoit/config.py
 letmedoit/eTextEdit.py
 letmedoit/geminipro.py
 letmedoit/geminiprovision.py
 letmedoit/health_check.py
 letmedoit/main.py
-letmedoit/ollamachat.py
 letmedoit/package_name.txt
 letmedoit/palm2.py
-letmedoit/qt.py
 letmedoit/requirements.txt
 letmedoit/systemtray.py
 letmedoit.egg-info/PKG-INFO
 letmedoit.egg-info/SOURCES.txt
 letmedoit.egg-info/dependency_links.txt
 letmedoit.egg-info/entry_points.txt
 letmedoit.egg-info/requires.txt
 letmedoit.egg-info/top_level.txt
-letmedoit/audio/notification1.mp3
-letmedoit/audio/notification1_mild.mp3
-letmedoit/audio/notification2.mp3
-letmedoit/audio/notification2_mild.mp3
 letmedoit/files/Readme.md
-letmedoit/gui/chatgui.py
-letmedoit/gui/quicktask.py
-letmedoit/gui/worker.py
 letmedoit/history/Readme.md
 letmedoit/icons/CyberTask.ico
 letmedoit/icons/CyberTask.png
 letmedoit/icons/GeminiPro.ico
 letmedoit/icons/GeminiPro.png
 letmedoit/icons/LetMeDoIt.ico
 letmedoit/icons/LetMeDoIt.png
@@ -67,85 +58,70 @@
 letmedoit/macOS_service/LetMeDoIt_Text_workflow/Contents/QuickLook/Thumbnail.png
 letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/Info.plist
 letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/document.wflow
 letmedoit/macOS_service/LetMeDoIt_Translation_workflow/Contents/QuickLook/Thumbnail.png
 letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/Info.plist
 letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/document.wflow
 letmedoit/macOS_service/LetMeDoIt_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
-letmedoit/plugins/000_check_ffmpeg.py
-letmedoit/plugins/000_check_pyaudio.py
-letmedoit/plugins/000_check_vlc.py
 letmedoit/plugins/Readme.md
 letmedoit/plugins/add calendar event.py
 letmedoit/plugins/aliases.py
-letmedoit/plugins/analyze audio.py
 letmedoit/plugins/analyze files.py
 letmedoit/plugins/analyze images with gemini.py
 letmedoit/plugins/analyze images.py
 letmedoit/plugins/analyze web content.py
 letmedoit/plugins/ask chatgpt.py
 letmedoit/plugins/ask codey.py
 letmedoit/plugins/ask gemini pro.py
-letmedoit/plugins/ask gemma.py
-letmedoit/plugins/ask llama2.py
-letmedoit/plugins/ask llava.py
-letmedoit/plugins/ask mistral.py
-letmedoit/plugins/ask ollama.py
 letmedoit/plugins/ask palm2.py
+letmedoit/plugins/ask sqlite.py
 letmedoit/plugins/auto heal python code.py
 letmedoit/plugins/awesome prompts.py
 letmedoit/plugins/character analysis.py
 letmedoit/plugins/contexts.py
 letmedoit/plugins/counselling.py
 letmedoit/plugins/create ai assistants.py
 letmedoit/plugins/create images.py
 letmedoit/plugins/create maps.py
 letmedoit/plugins/create qrcode.py
 letmedoit/plugins/create statistical graphics.py
 letmedoit/plugins/dates and times.py
 letmedoit/plugins/download youtube or web content.py
 letmedoit/plugins/edit text.py
-letmedoit/plugins/execute python code.py
-letmedoit/plugins/execute termux command.py
 letmedoit/plugins/global finance.py
 letmedoit/plugins/improve British English.py
 letmedoit/plugins/input suggestions.py
 letmedoit/plugins/install python package.py
 letmedoit/plugins/integrate google searches.py
 letmedoit/plugins/manipulate files.py
 letmedoit/plugins/memory.py
 letmedoit/plugins/modify images.py
 letmedoit/plugins/open web browser.py
 letmedoit/plugins/pronounce words.py
 letmedoit/plugins/remove image background.py
 letmedoit/plugins/search chat records.py
 letmedoit/plugins/search financial data.py
 letmedoit/plugins/search latest news.py
-letmedoit/plugins/search sqlite.py
 letmedoit/plugins/search weather info.py
 letmedoit/plugins/send email.py
-letmedoit/plugins/send tweet.py
 letmedoit/plugins/send whatsapp messages.py
 letmedoit/plugins/simplified Chinese to traditional Chinese.py
 letmedoit/plugins/solve math problems.py
 letmedoit/temp/Readme.md
 letmedoit/utils/assistant.py
-letmedoit/utils/config_essential.py
-letmedoit/utils/config_tools.py
+letmedoit/utils/configDefault.py
 letmedoit/utils/file_utils.py
 letmedoit/utils/get_path_prompt.py
 letmedoit/utils/install.py
-letmedoit/utils/ollama_models.py
 letmedoit/utils/promptValidator.py
 letmedoit/utils/prompt_multiline_shared_key_bindings.py
 letmedoit/utils/prompt_shared_key_bindings.py
 letmedoit/utils/prompts.py
 letmedoit/utils/shared_utils.py
 letmedoit/utils/shortcuts.py
 letmedoit/utils/streaming_word_wrapper.py
-letmedoit/utils/sttLanguages.py
 letmedoit/utils/terminal_mode_dialogs.py
 letmedoit/utils/terminal_system_command_prompt.py
 letmedoit/utils/text_utils.py
 letmedoit/utils/ttsLanguages.py
 letmedoit/utils/tts_utils.py
 letmedoit/utils/vlc_utils.py
```

### Comparing `letmedoit-2.1.84/setup.py` & `letmedoit-2.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,30 +44,28 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="2.1.84",
+    version="2.1.9",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant, leveraging the capabilities of ChatGPT API, Gemini Pro and AutoGen, capable of engaging in conversations, executing codes with auto-healing, and assisting you with a wide range of tasks on your local devices.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     packages=[
         package,
-        f"{package}.audio",
         f"{package}.files",
         f"{package}.history",
         f"{package}.icons",
         f"{package}.plugins",
         f"{package}.temp",
         f"{package}.utils",
-        f"{package}.gui",
         f"{package}.macOS_service",
         f"{package}.macOS_service.LetMeDoIt_Files_workflow",
         f"{package}.macOS_service.LetMeDoIt_Files_workflow.Contents",
         f"{package}.macOS_service.LetMeDoIt_Files_workflow.Contents.QuickLook",
         f"{package}.macOS_service.LetMeDoIt_Text_workflow",
         f"{package}.macOS_service.LetMeDoIt_Text_workflow.Contents",
         f"{package}.macOS_service.LetMeDoIt_Text_workflow.Contents.QuickLook",
@@ -88,22 +86,20 @@
         f"{package}.macOS_service.LetMeDoIt_YoutubeMP3_workflow.Contents.QuickLook",
         f"{package}.macOS_service.LetMeDoIt_Download_workflow",
         f"{package}.macOS_service.LetMeDoIt_Download_workflow.Contents",
         f"{package}.macOS_service.LetMeDoIt_Download_workflow.Contents.QuickLook",
     ],
     package_data={
         package: ["*.*"],
-        f"{package}.audio": ["*.*"],
         f"{package}.files": ["*.*"],
         f"{package}.history": ["*.*"],
         f"{package}.icons": ["*.*"],
         f"{package}.plugins": ["*.*"],
         f"{package}.temp": ["*.*"],
         f"{package}.utils": ["*.*"],
-        f"{package}.gui": ["*.*"],
         f"{package}.macOS_service": ["*.*"],
         f"{package}.macOS_service.LetMeDoIt_Files_workflow": ["*.*"],
         f"{package}.macOS_service.LetMeDoIt_Files_workflow.Contents": ["*.*"],
         f"{package}.macOS_service.LetMeDoIt_Files_workflow.Contents.QuickLook": ["*.*"],
         f"{package}.macOS_service.LetMeDoIt_Text_workflow": ["*.*"],
         f"{package}.macOS_service.LetMeDoIt_Text_workflow.Contents": ["*.*"],
         f"{package}.macOS_service.LetMeDoIt_Text_workflow.Contents.QuickLook": ["*.*"],
@@ -128,49 +124,34 @@
     },
     license="GNU General Public License (GPL)",
     install_requires=install_requires,
     entry_points={
         "console_scripts": [
             f"{package}={package}.main:main",
             f"{package}tray={package}.systemtray:main",
-            f"{package}gui={package}.qt:main",
             f"commandprompt={package}.commandprompt:main",
             f"etextedit={package}.eTextEdit:main",
             f"autoassist={package}.autoassist:main",
             f"autoretriever={package}.autoretriever:main",
             f"automath={package}.automath:main",
             f"autobuilder={package}.autobuilder:main",
             f"geminipro={package}.geminipro:main",
             f"geminiprovision={package}.geminiprovision:main",
             f"palm2={package}.palm2:main",
             f"codey={package}.codey:main",
             f"chatgpt={package}.chatgpt:main",
-            f"ollamachat={package}.ollamachat:main",
-            f"mistral={package}.ollamachat:mistral",
-            f"mixtral={package}.ollamachat:mixtral",
-            f"llama2={package}.ollamachat:llama2",
-            f"llama213b={package}.ollamachat:llama213b",
-            f"llama270b={package}.ollamachat:llama270b",
-            f"gemma2b={package}.ollamachat:gemma2b",
-            f"gemma7b={package}.ollamachat:gemma7b",
-            f"llava={package}.ollamachat:llava",
-            f"phi={package}.ollamachat:phi",
-            f"vicuna={package}.ollamachat:vicuna",
-            f"codellama={package}.ollamachat:codellama",
-            f"starlinglm={package}.ollamachat:starlinglm",
-            f"orca2={package}.ollamachat:orca2",
         ],
     },
     keywords="ai assistant openai chatgpt gemini autogen rag interpreter auto-heal",
     url="https://letmedoit.ai",
     project_urls={
         "Source": "https://github.com/eliranwong/letmedoit",
         "Tracker": "https://github.com/eliranwong/letmedoit/issues",
         "Documentation": "https://github.com/eliranwong/letmedoit/wiki",
-        "Funding": "https://www.paypal.me/letmedoitai",
+        "Funding": "https://www.paypal.me/MarvelBible",
     },
     classifiers=[
         # Reference: https://pypi.org/classifiers/
 
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
```

