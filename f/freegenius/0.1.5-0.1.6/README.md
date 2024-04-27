# Comparing `tmp/freegenius-0.1.5.tar.gz` & `tmp/freegenius-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.1.5.tar", last modified: Sat Apr 27 15:20:53 2024, max compression
+gzip compressed data, was "freegenius-0.1.6.tar", last modified: Sat Apr 27 15:27:09 2024, max compression
```

## Comparing `freegenius-0.1.5.tar` & `freegenius-0.1.6.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.190566 freegenius-0.1.5/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-04-27 15:20:53.190566 freegenius-0.1.5/PKG-INFO
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.170566 freegenius-0.1.5/freegenius/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11766 2024-04-27 15:20:52.000000 freegenius-0.1.5/freegenius/README.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.1.5/freegenius/__init__.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.170566 freegenius-0.1.5/freegenius/audio/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.1.5/freegenius/audio/notification1.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.1.5/freegenius/audio/notification1_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.1.5/freegenius/audio/notification2.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.1.5/freegenius/audio/notification2_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6646 2024-04-11 14:37:13.000000 freegenius-0.1.5/freegenius/autoassist.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.1.5/freegenius/autobuilder.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10727 2024-04-11 14:37:13.000000 freegenius-0.1.5/freegenius/autoretriever.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.1.5/freegenius/chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.1.5/freegenius/codey.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.1.5/freegenius/commandprompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:52.000000 freegenius-0.1.5/freegenius/config.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.1.5/freegenius/eTextEdit.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.170566 freegenius-0.1.5/freegenius/files/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.1.5/freegenius/files/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.1.5/freegenius/geminipro.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.1.5/freegenius/geminiprovision.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6515 2024-04-27 12:11:29.000000 freegenius-0.1.5/freegenius/groqchat.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.170566 freegenius-0.1.5/freegenius/gui/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.1.5/freegenius/gui/chatgui.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.1.5/freegenius/gui/worker.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.170566 freegenius-0.1.5/freegenius/history/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.1.5/freegenius/history/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.178566 freegenius-0.1.5/freegenius/icons/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.1.5/freegenius/icons/FreeGenius.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.1.5/freegenius/icons/FreeGenius.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.1.5/freegenius/icons/FreeGenius_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.1.5/freegenius/icons/ai.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.1.5/freegenius/icons/ai_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.1.5/freegenius/llamacpp.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.166566 freegenius-0.1.5/freegenius/macOS_service/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.166566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.166566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.166566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.166566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.166566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.166566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.166566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.166566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.182566 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.1.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.1.5/freegenius/main.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.1.5/freegenius/ollamachat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-27 15:20:52.000000 freegenius-0.1.5/freegenius/package_name.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.1.5/freegenius/palm2.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.186566 freegenius-0.1.5/freegenius/plugins/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.1.5/freegenius/plugins/000_check_ffmpeg.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.1.5/freegenius/plugins/000_check_pyaudio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.1.5/freegenius/plugins/000_check_vlc.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.1.5/freegenius/plugins/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.1.5/freegenius/plugins/add calendar event.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.1.5/freegenius/plugins/aliases.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.1.5/freegenius/plugins/analyze audio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.1.5/freegenius/plugins/analyze files.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.1.5/freegenius/plugins/analyze images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.1.5/freegenius/plugins/analyze web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.1.5/freegenius/plugins/auto correct python code.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.1.5/freegenius/plugins/awesome prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.1.5/freegenius/plugins/character analysis.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.1.5/freegenius/plugins/chat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.1.5/freegenius/plugins/contexts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.1.5/freegenius/plugins/counselling.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.1.5/freegenius/plugins/create ai assistants.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.1.5/freegenius/plugins/create images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.1.5/freegenius/plugins/create maps.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.1.5/freegenius/plugins/create qrcode.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.1.5/freegenius/plugins/create statistical graphics.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.1.5/freegenius/plugins/dates and times.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.1.5/freegenius/plugins/download youtube or web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.1.5/freegenius/plugins/edit text.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.1.5/freegenius/plugins/execute computing tasks.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.1.5/freegenius/plugins/execute termux command.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.1.5/freegenius/plugins/global finance.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.1.5/freegenius/plugins/improve British English.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.1.5/freegenius/plugins/input suggestions.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.1.5/freegenius/plugins/install python package.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.1.5/freegenius/plugins/integrate google searches.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.1.5/freegenius/plugins/memory.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.1.5/freegenius/plugins/modify images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.1.5/freegenius/plugins/open web browser.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.1.5/freegenius/plugins/pronounce words.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.1.5/freegenius/plugins/remove image background.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.1.5/freegenius/plugins/search chat records.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.1.5/freegenius/plugins/search financial data.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.1.5/freegenius/plugins/search latest news.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.1.5/freegenius/plugins/search sqlite.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.1.5/freegenius/plugins/search weather info.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.1.5/freegenius/plugins/send email.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.1.5/freegenius/plugins/send tweet.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.1.5/freegenius/plugins/send whatsapp messages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.1.5/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.1.5/freegenius/qt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.1.5/freegenius/rag.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-04-26 22:24:44.000000 freegenius-0.1.5/freegenius/requirements.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.1.5/freegenius/servers.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.1.5/freegenius/systemtray.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.186566 freegenius-0.1.5/freegenius/temp/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.1.5/freegenius/temp/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.190566 freegenius-0.1.5/freegenius/utils/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   112155 2024-04-27 15:16:32.000000 freegenius-0.1.5/freegenius/utils/assistant.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29734 2024-04-26 22:27:56.000000 freegenius-0.1.5/freegenius/utils/call_chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17269 2024-04-25 20:53:07.000000 freegenius-0.1.5/freegenius/utils/call_gemini.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17313 2024-04-27 14:53:19.000000 freegenius-0.1.5/freegenius/utils/call_groq.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    24612 2024-04-25 20:52:45.000000 freegenius-0.1.5/freegenius/utils/call_llamacpp.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.1.5/freegenius/utils/call_llm.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18713 2024-04-25 20:53:07.000000 freegenius-0.1.5/freegenius/utils/call_ollama.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18391 2024-04-27 12:12:56.000000 freegenius-0.1.5/freegenius/utils/config_essential.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.1.5/freegenius/utils/config_tools.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.1.5/freegenius/utils/download.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.1.5/freegenius/utils/get_path_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.1.5/freegenius/utils/ollama_models.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.1.5/freegenius/utils/promptValidator.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.1.5/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.1.5/freegenius/utils/prompt_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.1.5/freegenius/utils/prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.1.5/freegenius/utils/python_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    50100 2024-04-27 15:07:24.000000 freegenius-0.1.5/freegenius/utils/shared_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.1.5/freegenius/utils/shortcuts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.1.5/freegenius/utils/single_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.1.5/freegenius/utils/streaming_word_wrapper.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.1.5/freegenius/utils/sttLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.1.5/freegenius/utils/terminal_mode_dialogs.py
--rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.1.5/freegenius/utils/terminal_system_command_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.1.5/freegenius/utils/text_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4352 2024-04-12 22:26:19.000000 freegenius-0.1.5/freegenius/utils/tool_plugins.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.1.5/freegenius/utils/ttsLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.1.5/freegenius/utils/tts_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.1.5/freegenius/utils/vlc_utils.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:20:53.190566 freegenius-0.1.5/freegenius.egg-info/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-04-27 15:20:53.000000 freegenius-0.1.5/freegenius.egg-info/PKG-INFO
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-04-27 15:20:53.000000 freegenius-0.1.5/freegenius.egg-info/SOURCES.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-27 15:20:53.000000 freegenius-0.1.5/freegenius.egg-info/dependency_links.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1258 2024-04-27 15:20:53.000000 freegenius-0.1.5/freegenius.egg-info/entry_points.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-04-27 15:20:53.000000 freegenius-0.1.5/freegenius.egg-info/requires.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-04-27 15:20:53.000000 freegenius-0.1.5/freegenius.egg-info/top_level.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-27 15:20:53.190566 freegenius-0.1.5/setup.cfg
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10445 2024-04-27 15:20:43.000000 freegenius-0.1.5/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.777488 freegenius-0.1.6/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-04-27 15:27:09.777488 freegenius-0.1.6/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.745489 freegenius-0.1.6/freegenius/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11766 2024-04-27 15:27:09.000000 freegenius-0.1.6/freegenius/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.1.6/freegenius/__init__.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.745489 freegenius-0.1.6/freegenius/audio/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.1.6/freegenius/audio/notification1.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.1.6/freegenius/audio/notification1_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.1.6/freegenius/audio/notification2.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.1.6/freegenius/audio/notification2_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6646 2024-04-11 14:37:13.000000 freegenius-0.1.6/freegenius/autoassist.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.1.6/freegenius/autobuilder.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10727 2024-04-11 14:37:13.000000 freegenius-0.1.6/freegenius/autoretriever.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.1.6/freegenius/chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.1.6/freegenius/codey.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.1.6/freegenius/commandprompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.000000 freegenius-0.1.6/freegenius/config.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.1.6/freegenius/eTextEdit.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.745489 freegenius-0.1.6/freegenius/files/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.1.6/freegenius/files/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.1.6/freegenius/geminipro.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.1.6/freegenius/geminiprovision.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6515 2024-04-27 12:11:29.000000 freegenius-0.1.6/freegenius/groqchat.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.745489 freegenius-0.1.6/freegenius/gui/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.1.6/freegenius/gui/chatgui.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.1.6/freegenius/gui/worker.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.749488 freegenius-0.1.6/freegenius/history/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.1.6/freegenius/history/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.757488 freegenius-0.1.6/freegenius/icons/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.1.6/freegenius/icons/FreeGenius.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.1.6/freegenius/icons/FreeGenius.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.1.6/freegenius/icons/FreeGenius_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.1.6/freegenius/icons/ai.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.1.6/freegenius/icons/ai_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.1.6/freegenius/llamacpp.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.741489 freegenius-0.1.6/freegenius/macOS_service/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.741489 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.761488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.761488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.741489 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.761488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.761488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.741489 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.761488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.761488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.741489 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.761488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.761488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.741489 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.761488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.761488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.741489 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.765488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.765488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.741489 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.765488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.765488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.741489 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.765488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.765488 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.1.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.1.6/freegenius/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.1.6/freegenius/ollamachat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-27 15:27:09.000000 freegenius-0.1.6/freegenius/package_name.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.1.6/freegenius/palm2.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.769488 freegenius-0.1.6/freegenius/plugins/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.1.6/freegenius/plugins/000_check_ffmpeg.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.1.6/freegenius/plugins/000_check_pyaudio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.1.6/freegenius/plugins/000_check_vlc.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.1.6/freegenius/plugins/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.1.6/freegenius/plugins/add calendar event.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.1.6/freegenius/plugins/aliases.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.1.6/freegenius/plugins/analyze audio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.1.6/freegenius/plugins/analyze files.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.1.6/freegenius/plugins/analyze images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.1.6/freegenius/plugins/analyze web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.1.6/freegenius/plugins/auto correct python code.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.1.6/freegenius/plugins/awesome prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.1.6/freegenius/plugins/character analysis.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.1.6/freegenius/plugins/chat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.1.6/freegenius/plugins/contexts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.1.6/freegenius/plugins/counselling.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.1.6/freegenius/plugins/create ai assistants.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.1.6/freegenius/plugins/create images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.1.6/freegenius/plugins/create maps.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.1.6/freegenius/plugins/create qrcode.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.1.6/freegenius/plugins/create statistical graphics.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.1.6/freegenius/plugins/dates and times.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.1.6/freegenius/plugins/download youtube or web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.1.6/freegenius/plugins/edit text.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.1.6/freegenius/plugins/execute computing tasks.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.1.6/freegenius/plugins/execute termux command.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.1.6/freegenius/plugins/global finance.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.1.6/freegenius/plugins/improve British English.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.1.6/freegenius/plugins/input suggestions.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.1.6/freegenius/plugins/install python package.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.1.6/freegenius/plugins/integrate google searches.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.1.6/freegenius/plugins/memory.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.1.6/freegenius/plugins/modify images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.1.6/freegenius/plugins/open web browser.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.1.6/freegenius/plugins/pronounce words.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.1.6/freegenius/plugins/remove image background.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.1.6/freegenius/plugins/search chat records.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.1.6/freegenius/plugins/search financial data.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.1.6/freegenius/plugins/search latest news.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.1.6/freegenius/plugins/search sqlite.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.1.6/freegenius/plugins/search weather info.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.1.6/freegenius/plugins/send email.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.1.6/freegenius/plugins/send tweet.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.1.6/freegenius/plugins/send whatsapp messages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.1.6/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.1.6/freegenius/qt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.1.6/freegenius/rag.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-04-26 22:24:44.000000 freegenius-0.1.6/freegenius/requirements.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.1.6/freegenius/servers.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.1.6/freegenius/systemtray.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.769488 freegenius-0.1.6/freegenius/temp/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.1.6/freegenius/temp/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.773488 freegenius-0.1.6/freegenius/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   112155 2024-04-27 15:16:32.000000 freegenius-0.1.6/freegenius/utils/assistant.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29734 2024-04-26 22:27:56.000000 freegenius-0.1.6/freegenius/utils/call_chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17269 2024-04-25 20:53:07.000000 freegenius-0.1.6/freegenius/utils/call_gemini.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17313 2024-04-27 14:53:19.000000 freegenius-0.1.6/freegenius/utils/call_groq.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    24612 2024-04-25 20:52:45.000000 freegenius-0.1.6/freegenius/utils/call_llamacpp.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.1.6/freegenius/utils/call_llm.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18713 2024-04-25 20:53:07.000000 freegenius-0.1.6/freegenius/utils/call_ollama.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18391 2024-04-27 12:12:56.000000 freegenius-0.1.6/freegenius/utils/config_essential.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.1.6/freegenius/utils/config_tools.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.1.6/freegenius/utils/download.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.1.6/freegenius/utils/get_path_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.1.6/freegenius/utils/ollama_models.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.1.6/freegenius/utils/promptValidator.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.1.6/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.1.6/freegenius/utils/prompt_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.1.6/freegenius/utils/prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.1.6/freegenius/utils/python_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    50100 2024-04-27 15:07:24.000000 freegenius-0.1.6/freegenius/utils/shared_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.1.6/freegenius/utils/shortcuts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.1.6/freegenius/utils/single_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.1.6/freegenius/utils/streaming_word_wrapper.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.1.6/freegenius/utils/sttLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.1.6/freegenius/utils/terminal_mode_dialogs.py
+-rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.1.6/freegenius/utils/terminal_system_command_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.1.6/freegenius/utils/text_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4352 2024-04-12 22:26:19.000000 freegenius-0.1.6/freegenius/utils/tool_plugins.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.1.6/freegenius/utils/ttsLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.1.6/freegenius/utils/tts_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.1.6/freegenius/utils/vlc_utils.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 15:27:09.773488 freegenius-0.1.6/freegenius.egg-info/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-04-27 15:27:09.000000 freegenius-0.1.6/freegenius.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-04-27 15:27:09.000000 freegenius-0.1.6/freegenius.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-27 15:27:09.000000 freegenius-0.1.6/freegenius.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-27 15:27:09.000000 freegenius-0.1.6/freegenius.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-04-27 15:27:09.000000 freegenius-0.1.6/freegenius.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-04-27 15:27:09.000000 freegenius-0.1.6/freegenius.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-27 15:27:09.777488 freegenius-0.1.6/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10449 2024-04-27 15:26:42.000000 freegenius-0.1.6/setup.py
```

### Comparing `freegenius-0.1.5/PKG-INFO` & `freegenius-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.1.5
+Version: 0.1.6
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.1.5/freegenius/README.md` & `freegenius-0.1.6/freegenius/README.md`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/__init__.py` & `freegenius-0.1.6/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/audio/notification1.mp3` & `freegenius-0.1.6/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/audio/notification1_mild.mp3` & `freegenius-0.1.6/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/audio/notification2.mp3` & `freegenius-0.1.6/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/audio/notification2_mild.mp3` & `freegenius-0.1.6/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/autoassist.py` & `freegenius-0.1.6/freegenius/autoassist.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/autobuilder.py` & `freegenius-0.1.6/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/autoretriever.py` & `freegenius-0.1.6/freegenius/autoretriever.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/chatgpt.py` & `freegenius-0.1.6/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/codey.py` & `freegenius-0.1.6/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/commandprompt.py` & `freegenius-0.1.6/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/eTextEdit.py` & `freegenius-0.1.6/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/geminipro.py` & `freegenius-0.1.6/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/geminiprovision.py` & `freegenius-0.1.6/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/groqchat.py` & `freegenius-0.1.6/freegenius/groqchat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/gui/chatgui.py` & `freegenius-0.1.6/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/gui/worker.py` & `freegenius-0.1.6/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/icons/FreeGenius.ico` & `freegenius-0.1.6/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/icons/FreeGenius.png` & `freegenius-0.1.6/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/icons/FreeGenius_original.png` & `freegenius-0.1.6/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/icons/ai.png` & `freegenius-0.1.6/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/icons/ai_original.png` & `freegenius-0.1.6/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/llamacpp.py` & `freegenius-0.1.6/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.1.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/main.py` & `freegenius-0.1.6/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/ollamachat.py` & `freegenius-0.1.6/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/palm2.py` & `freegenius-0.1.6/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.1.6/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.1.6/freegenius/plugins/000_check_pyaudio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/000_check_vlc.py` & `freegenius-0.1.6/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/add calendar event.py` & `freegenius-0.1.6/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/aliases.py` & `freegenius-0.1.6/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/analyze audio.py` & `freegenius-0.1.6/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/analyze files.py` & `freegenius-0.1.6/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/analyze images.py` & `freegenius-0.1.6/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/analyze web content.py` & `freegenius-0.1.6/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/auto correct python code.py` & `freegenius-0.1.6/freegenius/plugins/auto correct python code.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/awesome prompts.py` & `freegenius-0.1.6/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/character analysis.py` & `freegenius-0.1.6/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/chat.py` & `freegenius-0.1.6/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/contexts.py` & `freegenius-0.1.6/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/counselling.py` & `freegenius-0.1.6/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/create ai assistants.py` & `freegenius-0.1.6/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/create images.py` & `freegenius-0.1.6/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/create maps.py` & `freegenius-0.1.6/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/create qrcode.py` & `freegenius-0.1.6/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/create statistical graphics.py` & `freegenius-0.1.6/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/dates and times.py` & `freegenius-0.1.6/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/download youtube or web content.py` & `freegenius-0.1.6/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/edit text.py` & `freegenius-0.1.6/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/execute computing tasks.py` & `freegenius-0.1.6/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/execute termux command.py` & `freegenius-0.1.6/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/global finance.py` & `freegenius-0.1.6/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/improve British English.py` & `freegenius-0.1.6/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/input suggestions.py` & `freegenius-0.1.6/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/install python package.py` & `freegenius-0.1.6/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/integrate google searches.py` & `freegenius-0.1.6/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/memory.py` & `freegenius-0.1.6/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/modify images.py` & `freegenius-0.1.6/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/open web browser.py` & `freegenius-0.1.6/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/pronounce words.py` & `freegenius-0.1.6/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/remove image background.py` & `freegenius-0.1.6/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/search chat records.py` & `freegenius-0.1.6/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/search financial data.py` & `freegenius-0.1.6/freegenius/plugins/search financial data.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/search latest news.py` & `freegenius-0.1.6/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/search sqlite.py` & `freegenius-0.1.6/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/search weather info.py` & `freegenius-0.1.6/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/send email.py` & `freegenius-0.1.6/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/send tweet.py` & `freegenius-0.1.6/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.1.6/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.1.6/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/rag.py` & `freegenius-0.1.6/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/requirements.txt` & `freegenius-0.1.6/freegenius/requirements.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/servers.py` & `freegenius-0.1.6/freegenius/servers.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/systemtray.py` & `freegenius-0.1.6/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/assistant.py` & `freegenius-0.1.6/freegenius/utils/assistant.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/call_chatgpt.py` & `freegenius-0.1.6/freegenius/utils/call_chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/call_gemini.py` & `freegenius-0.1.6/freegenius/utils/call_gemini.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/call_groq.py` & `freegenius-0.1.6/freegenius/utils/call_groq.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/call_llamacpp.py` & `freegenius-0.1.6/freegenius/utils/call_llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/call_llm.py` & `freegenius-0.1.6/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/call_ollama.py` & `freegenius-0.1.6/freegenius/utils/call_ollama.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/config_essential.py` & `freegenius-0.1.6/freegenius/utils/config_essential.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/config_tools.py` & `freegenius-0.1.6/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/download.py` & `freegenius-0.1.6/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/get_path_prompt.py` & `freegenius-0.1.6/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/ollama_models.py` & `freegenius-0.1.6/freegenius/utils/ollama_models.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/promptValidator.py` & `freegenius-0.1.6/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.1.6/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.1.6/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/prompts.py` & `freegenius-0.1.6/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/python_utils.py` & `freegenius-0.1.6/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/shared_utils.py` & `freegenius-0.1.6/freegenius/utils/shared_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/shortcuts.py` & `freegenius-0.1.6/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/single_prompt.py` & `freegenius-0.1.6/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.1.6/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/sttLanguages.py` & `freegenius-0.1.6/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.1.6/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.1.6/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/text_utils.py` & `freegenius-0.1.6/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/tool_plugins.py` & `freegenius-0.1.6/freegenius/utils/tool_plugins.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/ttsLanguages.py` & `freegenius-0.1.6/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/tts_utils.py` & `freegenius-0.1.6/freegenius/utils/tts_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius/utils/vlc_utils.py` & `freegenius-0.1.6/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius.egg-info/PKG-INFO` & `freegenius-0.1.6/freegenius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.1.5
+Version: 0.1.6
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.1.5/freegenius.egg-info/SOURCES.txt` & `freegenius-0.1.6/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/freegenius.egg-info/entry_points.txt` & `freegenius-0.1.6/freegenius.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 etextedit = freegenius.eTextEdit:main
 freegenius = freegenius.main:main
 freegeniustray = freegenius.systemtray:main
 geminipro = freegenius.geminipro:main
 geminiprovision = freegenius.geminiprovision:main
 gemma2b = freegenius.ollamachat:gemma2b
 gemma7b = freegenius.ollamachat:gemma7b
-groqchat = freegenius.groq:main
+groqchat = freegenius.groqchat:main
 letmedoit = freegenius.main:letmedoit
 llama2 = freegenius.ollamachat:llama2
 llama213b = freegenius.ollamachat:llama213b
 llama270b = freegenius.ollamachat:llama270b
 llamacpp = freegenius.llamacpp:main
 llava = freegenius.ollamachat:llava
 mistral = freegenius.ollamachat:mistral
```

### Comparing `freegenius-0.1.5/freegenius.egg-info/requires.txt` & `freegenius-0.1.6/freegenius.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.5/setup.py` & `freegenius-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.1.5",
+    version="0.1.6",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
@@ -149,15 +149,15 @@
             f"autoretriever={package}.autoretriever:main",
             #f"automath={package}.automath:main",
             f"autobuilder={package}.autobuilder:main",
             f"geminipro={package}.geminipro:main",
             f"geminiprovision={package}.geminiprovision:main",
             f"palm2={package}.palm2:main",
             f"codey={package}.codey:main",
-            f"groqchat={package}.groq:main",
+            f"groqchat={package}.groqchat:main",
             f"chatgpt={package}.chatgpt:main",
             f"llamacpp={package}.llamacpp:main",
             f"ollamachat={package}.ollamachat:main",
             f"mistral={package}.ollamachat:mistral",
             f"mixtral={package}.ollamachat:mixtral",
             f"llama2={package}.ollamachat:llama2",
             f"llama213b={package}.ollamachat:llama213b",
```

