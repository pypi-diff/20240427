# Comparing `tmp/sopel_modules_genius_answer-0.0.17.tar.gz` & `tmp/sopel_modules_genius_answer-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel_modules_genius_answer-0.0.17.tar", last modified: Fri Apr 26 16:33:58 2024, max compression
+gzip compressed data, was "sopel_modules_genius_answer-0.0.18.tar", last modified: Fri Apr 26 17:57:35 2024, max compression
```

## Comparing `sopel_modules_genius_answer-0.0.17.tar` & `sopel_modules_genius_answer-0.0.18.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 16:33:58.917505 sopel_modules_genius_answer-0.0.17/
--rw-rw-r--   0 user      (1000) user      (1000)      702 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.17/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)      111 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.17/NOTE.md
--rw-r--r--   0 user      (1000) user      (1000)     1000 2024-04-26 16:33:58.916505 sopel_modules_genius_answer-0.0.17/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      592 2024-04-26 15:48:30.000000 sopel_modules_genius_answer-0.0.17/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      674 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.17/TODO
--rw-rw-r--   0 user      (1000) user      (1000)      642 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.17/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-26 16:33:58.917505 sopel_modules_genius_answer-0.0.17/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 16:33:58.915505 sopel_modules_genius_answer-0.0.17/sopel_modules/
--rw-rw-r--   0 user      (1000) user      (1000)       56 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.17/sopel_modules/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 16:33:58.916505 sopel_modules_genius_answer-0.0.17/sopel_modules/genius-answer/
--rw-rw-r--   0 user      (1000) user      (1000)     2180 2024-04-26 16:28:27.000000 sopel_modules_genius_answer-0.0.17/sopel_modules/genius-answer/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 16:33:58.916505 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1000 2024-04-26 16:33:58.000000 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      368 2024-04-26 16:33:58.000000 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-26 16:33:58.000000 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-26 16:33:58.000000 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       14 2024-04-26 16:33:58.000000 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 17:57:35.631374 sopel_modules_genius_answer-0.0.18/
+-rw-rw-r--   0 user      (1000) user      (1000)      702 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.18/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)      135 2024-04-26 17:11:45.000000 sopel_modules_genius_answer-0.0.18/NOTE.md
+-rw-r--r--   0 user      (1000) user      (1000)     1144 2024-04-26 17:57:35.631374 sopel_modules_genius_answer-0.0.18/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      736 2024-04-26 16:54:45.000000 sopel_modules_genius_answer-0.0.18/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      674 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.18/TODO
+-rw-rw-r--   0 user      (1000) user      (1000)      642 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.18/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-26 17:57:35.631374 sopel_modules_genius_answer-0.0.18/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 17:57:35.629375 sopel_modules_genius_answer-0.0.18/sopel_modules/
+-rw-rw-r--   0 user      (1000) user      (1000)       56 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.18/sopel_modules/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 17:57:35.630375 sopel_modules_genius_answer-0.0.18/sopel_modules/genius-answer/
+-rw-rw-r--   0 user      (1000) user      (1000)     2933 2024-04-26 17:55:10.000000 sopel_modules_genius_answer-0.0.18/sopel_modules/genius-answer/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 17:57:35.630375 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1144 2024-04-26 17:57:35.000000 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      368 2024-04-26 17:57:35.000000 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-26 17:57:35.000000 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-26 17:57:35.000000 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       14 2024-04-26 17:57:35.000000 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/top_level.txt
```

### Comparing `sopel_modules_genius_answer-0.0.17/.gitignore` & `sopel_modules_genius_answer-0.0.18/.gitignore`

 * *Files identical despite different names*

### Comparing `sopel_modules_genius_answer-0.0.17/PKG-INFO` & `sopel_modules_genius_answer-0.0.18/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel_modules.genius-answer
-Version: 0.0.17
+Version: 0.0.18
 Summary: A sopel plugin (irc-bot) to answer with a quote from rapgenius.com 
 Author-email: eoli3n <eoli3n@runbox.com>
 License: WTFPL
 Project-URL: Source code, https://github.com/eoli3n/sopel-genius-answer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sopel<8,>=7.1
@@ -33,7 +33,15 @@
 Bot will ``say``, not ``answer``.
 
 ```ini
 [fallback]
 default="I don't know dude."
 channel="#channel is such a great place !"
 ```
+
+### Per nickname serial answer limitation
+To be able to limit how many answers to give to the same nickname.
+
+```ini
+[limitation]
+pinpin=3
+```
```

### Comparing `sopel_modules_genius_answer-0.0.17/README.md` & `sopel_modules_genius_answer-0.0.18/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -21,7 +21,15 @@
 Bot will ``say``, not ``answer``.
 
 ```ini
 [fallback]
 default="I don't know dude."
 channel="#channel is such a great place !"
 ```
+
+### Per nickname serial answer limitation
+To be able to limit how many answers to give to the same nickname.
+
+```ini
+[limitation]
+pinpin=3
+```
```

### Comparing `sopel_modules_genius_answer-0.0.17/TODO` & `sopel_modules_genius_answer-0.0.18/TODO`

 * *Files identical despite different names*

### Comparing `sopel_modules_genius_answer-0.0.17/pyproject.toml` & `sopel_modules_genius_answer-0.0.18/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sopel_modules_genius_answer-0.0.17/sopel_modules/genius-answer/__init__.py` & `sopel_modules_genius_answer-0.0.18/sopel_modules/genius-answer/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 #! /usr/bin/env python3
 
 import random
 import re
+import logging
 import lyricsgenius
 from sopel import plugin
 
+logger = logging.getLogger(__name__)
+
 def setup(bot):
+    if "last_nick" not in bot.memory:
+        bot.memory["last_nick"] = ""
+    if "last_nick_count" not in bot.memory:
+        bot.memory["last_nick_count"] = 0
     genius_token = bot.config.genius.api_key
     global genius
     genius = lyricsgenius.Genius(genius_token)
     genius.remove_section_headers = True
+    global fallback
+    if bot.config.fallback.default:
+        fallback = bot.config.fallback.default
+    else:
+        fallback = ""
 
 def get_two_words_in_text(text):
     splitted = text.split()
     for word in splitted:
         if not re.match("^[A-Za-zÀ-ÿ-']*$", word):
             splitted.remove(word)
     length = len(splitted)
@@ -57,18 +69,32 @@
     except:
         return False
     return answer
 
 @plugin.rule(r'(.*\b)($nickname)[ :,](.*)')
 
 def sentence_responder(bot, trigger):
+
+    # limitation serial msg per nick
+    if bot.memory["last_nick"] != trigger.nick:  
+        bot.memory["last_nick"] = trigger.nick
+        bot.memory["last_nick_count"] = 1
+    else:
+        bot.memory["last_nick_count"] += 1
+
+    if getattr(bot.config.limitation, trigger.nick):
+        if bot.memory["last_nick_count"] > int(getattr(bot.config.limitation, trigger.nick)):
+            logger.info(trigger.nick + " is now blocked")
+            return
+
     message = trigger.group(1) + trigger.group(3)
     response = genius_bot_answer(message)
+
     channel = bot.channels[trigger.sender].name.replace('#','')
     if getattr(bot.config.fallback, channel):
         fallback = getattr(bot.config.fallback, channel)
-    elif bot.config.fallback.default:
-        fallback = bot.config.fallback.default
+    # answer
     if response:
         bot.reply(response)
+    # fallback msg
     elif fallback:
         bot.say(fallback)
```

### Comparing `sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/PKG-INFO` & `sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel_modules.genius-answer
-Version: 0.0.17
+Version: 0.0.18
 Summary: A sopel plugin (irc-bot) to answer with a quote from rapgenius.com 
 Author-email: eoli3n <eoli3n@runbox.com>
 License: WTFPL
 Project-URL: Source code, https://github.com/eoli3n/sopel-genius-answer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sopel<8,>=7.1
@@ -33,7 +33,15 @@
 Bot will ``say``, not ``answer``.
 
 ```ini
 [fallback]
 default="I don't know dude."
 channel="#channel is such a great place !"
 ```
+
+### Per nickname serial answer limitation
+To be able to limit how many answers to give to the same nickname.
+
+```ini
+[limitation]
+pinpin=3
+```
```

