# Comparing `tmp/matterdelta-1.3.0.tar.gz` & `tmp/matterdelta-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matterdelta-1.3.0.tar", last modified: Tue Mar 19 05:47:15 2024, max compression
+gzip compressed data, was "matterdelta-1.4.0.tar", last modified: Sat Apr 27 21:12:05 2024, max compression
```

## Comparing `matterdelta-1.3.0.tar` & `matterdelta-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:15.347379 matterdelta-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:15.343379 matterdelta-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:15.343379 matterdelta-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-19 05:47:05.000000 matterdelta-1.3.0/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-19 05:47:05.000000 matterdelta-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-03-19 05:47:05.000000 matterdelta-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-19 05:47:15.347379 matterdelta-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-19 05:47:05.000000 matterdelta-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:15.343379 matterdelta-1.3.0/matterdelta/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-19 05:47:05.000000 matterdelta-1.3.0/matterdelta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-19 05:47:05.000000 matterdelta-1.3.0/matterdelta/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-19 05:47:05.000000 matterdelta-1.3.0/matterdelta/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-19 05:47:05.000000 matterdelta-1.3.0/matterdelta/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:15.347379 matterdelta-1.3.0/matterdelta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-19 05:47:15.000000 matterdelta-1.3.0/matterdelta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-19 05:47:15.000000 matterdelta-1.3.0/matterdelta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 05:47:15.000000 matterdelta-1.3.0/matterdelta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-19 05:47:15.000000 matterdelta-1.3.0/matterdelta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 05:47:15.000000 matterdelta-1.3.0/matterdelta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-19 05:47:15.000000 matterdelta-1.3.0/matterdelta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-19 05:47:05.000000 matterdelta-1.3.0/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-19 05:47:05.000000 matterdelta-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 05:47:15.347379 matterdelta-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:05.066473 matterdelta-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:05.062473 matterdelta-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:05.066473 matterdelta-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-27 21:11:53.000000 matterdelta-1.4.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-27 21:11:53.000000 matterdelta-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-27 21:11:53.000000 matterdelta-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-27 21:12:05.066473 matterdelta-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-27 21:11:53.000000 matterdelta-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:05.066473 matterdelta-1.4.0/matterdelta/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 21:11:53.000000 matterdelta-1.4.0/matterdelta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 21:11:53.000000 matterdelta-1.4.0/matterdelta/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 21:12:04.000000 matterdelta-1.4.0/matterdelta/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-27 21:11:53.000000 matterdelta-1.4.0/matterdelta/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-27 21:11:53.000000 matterdelta-1.4.0/matterdelta/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:05.066473 matterdelta-1.4.0/matterdelta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 21:11:53.000000 matterdelta-1.4.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-27 21:11:53.000000 matterdelta-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 21:12:05.066473 matterdelta-1.4.0/setup.cfg
```

### Comparing `matterdelta-1.3.0/.github/workflows/python-ci.yml` & `matterdelta-1.4.0/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `matterdelta-1.3.0/LICENSE.txt` & `matterdelta-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `matterdelta-1.3.0/PKG-INFO` & `matterdelta-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: matterdelta
-Version: 1.3.0
+Version: 1.4.0
 Summary: Matterbridge API plugin for Delta Chat
 Author-email: adbenitez <adb@merlinux.eu>
+Project-URL: Homepage, https://github.com/deltachat-bot/matterdelta
 Keywords: deltachat,bot,matterbridge,bridge
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: deltabot-cli<6.0,>=5.0.0
+Requires-Dist: deltabot-cli<7.0,>=6.1.0
 Requires-Dist: requests
 Provides-Extra: fast
 Requires-Dist: cchardet>=2.1.7; extra == "fast"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `matterdelta-1.3.0/README.md` & `matterdelta-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `matterdelta-1.3.0/matterdelta/api.py` & `matterdelta-1.4.0/matterdelta/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tempfile
 import time
 from pathlib import Path
 from threading import Thread
 from typing import Dict, List, Tuple
 
 import requests
-from deltabot_cli import AttrDict, Bot, JsonRpcError, ViewType
+from deltachat2 import Bot, JsonRpcError, Message, MessageViewtype, MsgData
 
 mb_config = {}
 chat2gateway: Dict[Tuple[int, int], List[str]] = {}
 gateway2chat: Dict[str, List[Tuple[int, int]]] = {}
 
 
 def init_api(bot: Bot, config_dir: str) -> None:
@@ -29,15 +29,15 @@
         gateway2chat.setdefault(gateway["gateway"], []).append(chat)
         chat2gateway.setdefault(chat, []).append(gateway["gateway"])
 
     if mb_config["api"]["url"] and len(gateways):
         Thread(target=listen_to_matterbridge, args=(bot,), daemon=True).start()
 
 
-def dc2mb(bot: Bot, accid: int, msg: AttrDict) -> None:
+def dc2mb(bot: Bot, accid: int, msg: Message) -> None:
     """Send a Delta Chat message to the matterbridge side."""
     if not msg.text and not msg.file:  # ignore buggy empty messages
         return
     gateways = chat2gateway.get((accid, msg.chat_id), [])
     if gateways:
         username = (
             msg.override_sender_name
@@ -84,29 +84,29 @@
         return
     chats = [c for c in gateway2chat.get(msg["gateway"], []) if c != exclude]
     if not chats:
         return
     text = msg.get("text") or ""
     if msg["event"] == "user_action":
         text = "/me " + text
-    reply = {
-        "text": text,
-        "overrideSenderName": msg["username"],
-    }
+    reply = MsgData(
+        text=text,
+        override_sender_name=msg["username"],
+    )
     file = ((msg.get("Extra") or {}).get("file") or [{}])[0]
     if file:
         if text == file["Name"]:
             text = ""
         with tempfile.TemporaryDirectory() as tmp_dir:
-            reply["file"] = str(Path(tmp_dir, file["Name"]))
+            reply.file = str(Path(tmp_dir, file["Name"]))
             data = base64.decodebytes(file["Data"].encode())
-            with open(reply["file"], mode="wb") as attachment:
+            with open(reply.file, mode="wb") as attachment:
                 attachment.write(data)
             if file["Name"].endswith((".tgs", ".webp")):
-                reply["viewtype"] = ViewType.STICKER
+                reply.viewtype = MessageViewtype.STICKER
             for accid, chat_id in chats:
                 try:
                     bot.rpc.send_msg(accid, chat_id, reply)
                 except JsonRpcError as ex:
                     bot.logger.exception(ex)
     elif text:
         for accid, chat_id in chats:
```

### Comparing `matterdelta-1.3.0/matterdelta/hooks.py` & `matterdelta-1.4.0/matterdelta/hooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 """Event Hooks"""
 
 from argparse import Namespace
 
-from deltabot_cli import (
-    AttrDict,
-    Bot,
-    BotCli,
-    ChatType,
-    EventType,
-    events,
-    is_not_known_command,
-)
+from deltabot_cli import BotCli
+from deltachat2 import Bot, ChatType, CoreEvent, EventType, MsgData, NewMsgEvent, events
 from rich.logging import RichHandler
 
+from ._version import __version__
 from .api import dc2mb, init_api
 
 cli = BotCli("matterdelta")
+cli.add_generic_option("-v", "--version", action="version", version=__version__)
 cli.add_generic_option(
     "--no-time",
     help="do not display date timestamp in log messages",
     action="store_false",
 )
 
 
@@ -29,63 +24,65 @@
         RichHandler(show_path=False, omit_repeated_times=False, show_time=args.no_time)
     ]
     for accid in bot.rpc.get_all_account_ids():
         if not bot.rpc.get_config(accid, "displayname"):
             bot.rpc.set_config(accid, "displayname", "Matterbridge Bot")
             status = "I am a Delta Chat bot, send me /help for more info"
             bot.rpc.set_config(accid, "selfstatus", status)
-            bot.rpc.set_config(accid, "delete_server_after", "1")
             bot.rpc.set_config(accid, "delete_device_after", str(60 * 60 * 24 * 30))
 
 
 @cli.on_start
 def _on_start(bot: Bot, args: Namespace) -> None:
     init_api(bot, args.config_dir)
 
 
 @cli.on(events.RawEvent)
-def _log_event(bot: Bot, accid: int, event: AttrDict) -> None:
+def _log_event(bot: Bot, accid: int, event: CoreEvent) -> None:
     if event.kind == EventType.INFO:
         bot.logger.debug(event.msg)
     elif event.kind == EventType.WARNING:
         bot.logger.warning(event.msg)
     elif event.kind == EventType.ERROR:
         bot.logger.error(event.msg)
     elif event.kind == EventType.SECUREJOIN_INVITER_PROGRESS:
         if event.progress == 1000:
-            bot.logger.debug("QR scanned by contact id=%s", event.contact_id)
-            chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
-            _send_help(bot, accid, chatid)
+            if not bot.rpc.get_contact(accid, event.contact_id).is_bot:
+                bot.logger.debug("QR scanned by contact id=%s", event.contact_id)
+                chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
+                _send_help(bot, accid, chatid)
 
 
-@cli.on(events.NewMessage(is_info=False, is_bot=None, func=is_not_known_command))
-def _bridge(bot: Bot, accid: int, event: AttrDict) -> None:
+@cli.on(events.NewMessage(is_info=False, is_bot=None))
+def _bridge(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    if bot.has_command(event.command):
+        return
     msg = event.msg
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
     if chat.chat_type == ChatType.SINGLE and not msg.is_bot:
         bot.rpc.markseen_msgs(accid, [msg.id])
         _send_help(bot, accid, msg.chat_id)
     else:
         dc2mb(bot, accid, msg)
 
 
 @cli.on(events.NewMessage(command="/id"))
-def _id(bot: Bot, accid: int, event: AttrDict) -> None:
+def _id(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     msg = event.msg
     bot.rpc.markseen_msgs(accid, [msg.id])
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
     if chat.chat_type == ChatType.SINGLE:
         text = "You can't use /id command here, add me to a group and use the command there"
-        bot.rpc.send_msg(accid, msg.chat_id, {"text": text, "quotedMessageId": msg.id})
+        reply = MsgData(text=text, quoted_message_id=msg.id)
     else:
-        reply = {"text": f"accountId: {accid}\nchatId: {msg.chat_id}"}
-        bot.rpc.send_msg(accid, msg.chat_id, reply)
+        reply = MsgData(text=f"accountId: {accid}\nchatId: {msg.chat_id}")
+    bot.rpc.send_msg(accid, msg.chat_id, reply)
 
 
 def _send_help(bot: Bot, accid: int, chatid: int) -> None:
     text = (
         "I'm a bot, I allow to bridge Delta Chat groups with groups in other platforms."
         " Only the bot administrator can bridge groups.\n\n"
         "**Available commands**\n\n"
         "/id - send me this command in a group to get its ID."
     )
-    bot.rpc.send_msg(accid, chatid, {"text": text})
+    bot.rpc.send_msg(accid, chatid, MsgData(text=text))
```

### Comparing `matterdelta-1.3.0/matterdelta.egg-info/PKG-INFO` & `matterdelta-1.4.0/matterdelta.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: matterdelta
-Version: 1.3.0
+Version: 1.4.0
 Summary: Matterbridge API plugin for Delta Chat
 Author-email: adbenitez <adb@merlinux.eu>
+Project-URL: Homepage, https://github.com/deltachat-bot/matterdelta
 Keywords: deltachat,bot,matterbridge,bridge
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: deltabot-cli<6.0,>=5.0.0
+Requires-Dist: deltabot-cli<7.0,>=6.1.0
 Requires-Dist: requests
 Provides-Extra: fast
 Requires-Dist: cchardet>=2.1.7; extra == "fast"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `matterdelta-1.3.0/pyproject.toml` & `matterdelta-1.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,21 @@
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
 dependencies = [
-    "deltabot-cli>=5.0.0,<6.0",
+    "deltabot-cli>=6.1.0,<7.0",
     "requests",
 ]
 
+[project.urls]
+Homepage = "https://github.com/deltachat-bot/matterdelta"
+
 [project.optional-dependencies]
 fast = [
     "cchardet>=2.1.7",
 ]
 dev = [
   "black",
   "mypy",
@@ -37,13 +40,14 @@
 ]
 
 [project.scripts]
 matterdelta = "matterdelta:main"
 
 [tool.setuptools_scm]
 # can be empty if no extra settings are needed, presence enables setuptools_scm
+version_file = "matterdelta/_version.py"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 ignore_missing_imports = "True"
```

