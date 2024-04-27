# Comparing `tmp/stickersbot-4.0.1.tar.gz` & `tmp/stickersbot-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stickersbot-4.0.1.tar", last modified: Mon Apr 15 23:26:12 2024, max compression
+gzip compressed data, was "stickersbot-4.1.1.tar", last modified: Sat Apr 27 18:23:57 2024, max compression
```

## Comparing `stickersbot-4.0.1.tar` & `stickersbot-4.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:26:12.372801 stickersbot-4.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:26:12.368801 stickersbot-4.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-15 23:26:02.000000 stickersbot-4.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:26:12.368801 stickersbot-4.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-15 23:26:02.000000 stickersbot-4.0.1/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 23:26:02.000000 stickersbot-4.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-15 23:26:02.000000 stickersbot-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-15 23:26:12.368801 stickersbot-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-15 23:26:02.000000 stickersbot-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-15 23:26:02.000000 stickersbot-4.0.1/avatar.png
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 23:26:02.000000 stickersbot-4.0.1/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-15 23:26:02.000000 stickersbot-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:26:12.372801 stickersbot-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:26:12.368801 stickersbot-4.0.1/stickersbot/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-15 23:26:02.000000 stickersbot-4.0.1/stickersbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 23:26:02.000000 stickersbot-4.0.1/stickersbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-15 23:26:02.000000 stickersbot-4.0.1/stickersbot/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-15 23:26:02.000000 stickersbot-4.0.1/stickersbot/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-15 23:26:02.000000 stickersbot-4.0.1/stickersbot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:26:12.368801 stickersbot-4.0.1/stickersbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-15 23:26:12.000000 stickersbot-4.0.1/stickersbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-15 23:26:12.000000 stickersbot-4.0.1/stickersbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:26:12.000000 stickersbot-4.0.1/stickersbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 23:26:12.000000 stickersbot-4.0.1/stickersbot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 23:26:12.000000 stickersbot-4.0.1/stickersbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 23:26:12.000000 stickersbot-4.0.1/stickersbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:23:57.695646 stickersbot-4.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:23:57.691646 stickersbot-4.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-27 18:23:44.000000 stickersbot-4.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:23:57.691646 stickersbot-4.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-27 18:23:44.000000 stickersbot-4.1.1/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-27 18:23:44.000000 stickersbot-4.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-27 18:23:44.000000 stickersbot-4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-27 18:23:57.695646 stickersbot-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-27 18:23:44.000000 stickersbot-4.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-27 18:23:44.000000 stickersbot-4.1.1/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-27 18:23:44.000000 stickersbot-4.1.1/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-27 18:23:44.000000 stickersbot-4.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 18:23:57.695646 stickersbot-4.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:23:57.691646 stickersbot-4.1.1/stickersbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-27 18:23:44.000000 stickersbot-4.1.1/stickersbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 18:23:44.000000 stickersbot-4.1.1/stickersbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-27 18:23:44.000000 stickersbot-4.1.1/stickersbot/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-27 18:23:44.000000 stickersbot-4.1.1/stickersbot/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-27 18:23:44.000000 stickersbot-4.1.1/stickersbot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:23:57.695646 stickersbot-4.1.1/stickersbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/top_level.txt
```

### Comparing `stickersbot-4.0.1/.github/workflows/python-ci.yml` & `stickersbot-4.1.1/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `stickersbot-4.0.1/LICENSE` & `stickersbot-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stickersbot-4.0.1/PKG-INFO` & `stickersbot-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: stickersbot
-Version: 4.0.1
+Version: 4.1.1
 Summary: Sticker packs for all your Delta Chat needs
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/stickersbot
 Keywords: deltachat,bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deltabot-cli<7.0,>=6.0.0
+Requires-Dist: deltabot-cli<7.0,>=6.1.0
 Requires-Dist: signalstickers-client>=3.1.0
 Requires-Dist: emoji>=1.6.1
 Requires-Dist: cachelib>=0.7.0
 Requires-Dist: requests>=2.26.0
 Requires-Dist: pillow>=10.3.0
 Requires-Dist: rembg>=2.0.56
 Provides-Extra: dev
```

### Comparing `stickersbot-4.0.1/README.md` & `stickersbot-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `stickersbot-4.0.1/avatar.png` & `stickersbot-4.1.1/avatar.png`

 * *Files identical despite different names*

### Comparing `stickersbot-4.0.1/pyproject.toml` & `stickersbot-4.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 ]
 dependencies = [
-    "deltabot-cli>=6.0.0,<7.0",
+    "deltabot-cli>=6.1.0,<7.0",
     "signalstickers-client>=3.1.0",
     "emoji>=1.6.1",
     "cachelib>=0.7.0",
     "requests>=2.26.0",
     "pillow>=10.3.0",
     "rembg>=2.0.56",
 ]
@@ -43,14 +43,15 @@
 ]
 
 [project.scripts]
 stickersbot = "stickersbot:main"
 
 [tool.setuptools_scm]
 # can be empty if no extra settings are needed, presence enables setuptools_scm
+version_file = "stickersbot/_version.py"
 
 [tool.setuptools]
 packages = ["stickersbot"]
 
 [tool.isort]
 profile = "black"
```

### Comparing `stickersbot-4.0.1/stickersbot/hooks.py` & `stickersbot-4.1.1/stickersbot/hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,21 @@
     NewMsgEvent,
     events,
 )
 from emoji import emoji_count
 from PIL import Image
 from rembg import remove
 
+from ._version import __version__
 from .signal import SignalStickers
 from .util import sizeof_fmt, upload
 
 signal = SignalStickers()
 cli = BotCli("stickersbot")
+cli.add_generic_option("-v", "--version", action="version", version=__version__)
 
 
 @cli.on_init
 def on_init(bot: Bot, _args: Namespace) -> None:
     for accid in bot.rpc.get_all_account_ids():
         if not bot.rpc.get_config(accid, "displayname"):
             bot.rpc.set_config(accid, "displayname", "StickersBot")
@@ -128,17 +130,16 @@
             reply = MsgData(text=text, file=filename, quoted_message_id=msg.id)
             bot.rpc.send_msg(accid, msg.chat_id, reply)
     else:
         reply = MsgData(text="❌ Unknow pack URL", quoted_message_id=msg.id)
         bot.rpc.send_msg(accid, msg.chat_id, reply)
 
 
-@cli.on(events.NewMessage)
+@cli.after(events.NewMessage)
 def delete_msgs(bot: Bot, accid: int, event: NewMsgEvent) -> None:
-    """NOTE: This hook must be added at the end so it is not executed before other commands and hooks"""
     bot.rpc.delete_messages(accid, [event.msg.id])
 
 
 def process_signal_pack(bot: Bot, accid: int, msg: Message) -> None:
     title, path = signal.download_pack(bot.account.get_blobdir(), msg.text)
     size = os.stat(path).st_size
     if size > 1024**2 * 15:
```

### Comparing `stickersbot-4.0.1/stickersbot/signal.py` & `stickersbot-4.1.1/stickersbot/signal.py`

 * *Files identical despite different names*

### Comparing `stickersbot-4.0.1/stickersbot/util.py` & `stickersbot-4.1.1/stickersbot/util.py`

 * *Files identical despite different names*

### Comparing `stickersbot-4.0.1/stickersbot.egg-info/PKG-INFO` & `stickersbot-4.1.1/stickersbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: stickersbot
-Version: 4.0.1
+Version: 4.1.1
 Summary: Sticker packs for all your Delta Chat needs
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/stickersbot
 Keywords: deltachat,bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deltabot-cli<7.0,>=6.0.0
+Requires-Dist: deltabot-cli<7.0,>=6.1.0
 Requires-Dist: signalstickers-client>=3.1.0
 Requires-Dist: emoji>=1.6.1
 Requires-Dist: cachelib>=0.7.0
 Requires-Dist: requests>=2.26.0
 Requires-Dist: pillow>=10.3.0
 Requires-Dist: rembg>=2.0.56
 Provides-Extra: dev
```

