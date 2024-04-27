# Comparing `tmp/feedsbot-0.4.3.tar.gz` & `tmp/feedsbot-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedsbot-0.4.3.tar", last modified: Fri Mar 22 07:29:14 2024, max compression
+gzip compressed data, was "feedsbot-0.5.0.tar", last modified: Sat Apr 27 20:40:16 2024, max compression
```

## Comparing `feedsbot-0.4.3.tar` & `feedsbot-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 07:29:14.208446 feedsbot-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 07:29:14.204446 feedsbot-0.4.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-22 07:29:04.000000 feedsbot-0.4.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 07:29:14.204446 feedsbot-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-22 07:29:04.000000 feedsbot-0.4.3/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-22 07:29:04.000000 feedsbot-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-03-22 07:29:04.000000 feedsbot-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-22 07:29:14.208446 feedsbot-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-22 07:29:04.000000 feedsbot-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-03-22 07:29:04.000000 feedsbot-0.4.3/avatar.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 07:29:14.208446 feedsbot-0.4.3/feedsbot/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-22 07:29:04.000000 feedsbot-0.4.3/feedsbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-03-22 07:29:04.000000 feedsbot-0.4.3/feedsbot/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-22 07:29:04.000000 feedsbot-0.4.3/feedsbot/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-03-22 07:29:04.000000 feedsbot-0.4.3/feedsbot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 07:29:14.208446 feedsbot-0.4.3/feedsbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-22 07:29:14.000000 feedsbot-0.4.3/feedsbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-22 07:29:14.000000 feedsbot-0.4.3/feedsbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 07:29:14.000000 feedsbot-0.4.3/feedsbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-22 07:29:14.000000 feedsbot-0.4.3/feedsbot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-22 07:29:14.000000 feedsbot-0.4.3/feedsbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-22 07:29:14.000000 feedsbot-0.4.3/feedsbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-22 07:29:04.000000 feedsbot-0.4.3/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-22 07:29:04.000000 feedsbot-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 07:29:14.208446 feedsbot-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:40:16.446969 feedsbot-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:40:16.442969 feedsbot-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-27 20:40:07.000000 feedsbot-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:40:16.442969 feedsbot-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-27 20:40:07.000000 feedsbot-0.5.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-27 20:40:07.000000 feedsbot-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-27 20:40:07.000000 feedsbot-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-27 20:40:16.446969 feedsbot-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-27 20:40:07.000000 feedsbot-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-27 20:40:07.000000 feedsbot-0.5.0/avatar.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:40:16.442969 feedsbot-0.5.0/feedsbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-27 20:40:07.000000 feedsbot-0.5.0/feedsbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-04-27 20:40:07.000000 feedsbot-0.5.0/feedsbot/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-27 20:40:07.000000 feedsbot-0.5.0/feedsbot/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-27 20:40:07.000000 feedsbot-0.5.0/feedsbot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:40:16.446969 feedsbot-0.5.0/feedsbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-27 20:40:07.000000 feedsbot-0.5.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-27 20:40:07.000000 feedsbot-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 20:40:16.446969 feedsbot-0.5.0/setup.cfg
```

### Comparing `feedsbot-0.4.3/.github/dependabot.yml` & `feedsbot-0.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `feedsbot-0.4.3/.github/workflows/python-ci.yml` & `feedsbot-0.5.0/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `feedsbot-0.4.3/LICENSE` & `feedsbot-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feedsbot-0.4.3/PKG-INFO` & `feedsbot-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: feedsbot
-Version: 0.4.3
+Version: 0.5.0
 Summary: Subscribe to RSS/Atom feeds in Delta Chat
 Author-email: adbenitez <adb@merlinux.eu>
+Project-URL: Homepage, https://github.com/deltachat-bot/feedsbot
 Keywords: deltachat,bot,feeds,rss,atom
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deltabot-cli<6.0,>=5.0.0
+Requires-Dist: deltabot-cli<7.0,>=6.1.0
 Requires-Dist: SQLAlchemy<3.0,>=2.0.25
 Requires-Dist: feedparser<7.0,>=6.0.11
 Requires-Dist: requests<3.0,>=2.28.1
 Requires-Dist: beautifulsoup4<5.0,>=4.11.1
 Requires-Dist: html5lib>=1.1
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
```

### Comparing `feedsbot-0.4.3/README.md` & `feedsbot-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `feedsbot-0.4.3/avatar.png` & `feedsbot-0.5.0/avatar.png`

 * *Files identical despite different names*

### Comparing `feedsbot-0.4.3/feedsbot/hooks.py` & `feedsbot-0.5.0/feedsbot/hooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 """Event Hooks"""
 
 from argparse import Namespace
 from pathlib import Path
 from threading import Thread
 
-from deltabot_cli import (
-    AttrDict,
+from deltabot_cli import BotCli
+from deltachat2 import (
     Bot,
-    BotCli,
     ChatType,
+    CoreEvent,
     EventType,
+    MsgData,
+    NewMsgEvent,
     SpecialContactId,
+    SystemMessageType,
     events,
-    is_not_known_command,
 )
 from feedparser import FeedParserDict
 from rich.logging import RichHandler
 from sqlalchemy import delete, func, select
 
+from ._version import __version__
 from .orm import Fchat, Feed, init, session_scope
 from .util import (
     check_feeds,
     format_entries,
     get_latest_date,
     get_old_entries,
     normalize_url,
     parse_feed,
     set_group_image,
 )
 
 cli = BotCli("feedsbot")
+cli.add_generic_option("-v", "--version", action="version", version=__version__)
 cli.add_generic_option(
     "--interval",
     type=int,
     default=60 * 5,
     help="how many seconds to sleep before checking the feeds again (default: %(default)s)",
 )
 cli.add_generic_option(
@@ -80,60 +84,66 @@
         target=check_feeds,
         args=(bot, args.interval, args.parallel, config_dir),
         daemon=True,
     ).start()
 
 
 @cli.on(events.RawEvent)
-def log_event(bot: Bot, accid: int, event: AttrDict) -> None:
+def log_event(bot: Bot, accid: int, event: CoreEvent) -> None:
     if event.kind == EventType.INFO:
         bot.logger.debug(event.msg)
     elif event.kind == EventType.WARNING:
         bot.logger.warning(event.msg)
     elif event.kind == EventType.ERROR:
         bot.logger.error(event.msg)
+    elif event.kind == EventType.MSG_DELIVERED:
+        bot.rpc.delete_messages(accid, [event.msg_id])
     elif event.kind == EventType.SECUREJOIN_INVITER_PROGRESS:
         if event.progress == 1000:
-            bot.logger.debug("QR scanned by contact id=%s", event.contact_id)
-            chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
-            send_help(bot, accid, chatid)
+            if not bot.rpc.get_contact(accid, event.contact_id).is_bot:
+                bot.logger.debug("QR scanned by contact id=%s", event.contact_id)
+                chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
+                send_help(bot, accid, chatid)
 
 
-@cli.on(events.MemberListChanged)
-def on_memberlist_change(bot: Bot, accid: int, event: AttrDict) -> None:
-    if event.member_added:
+@cli.on(events.NewMessage(is_info=True))
+def on_memberlist_change(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    if event.msg.system_message_type != SystemMessageType.MEMBER_REMOVED_FROM_GROUP:
         return
     chat_id = event.msg.chat_id
     chat = bot.rpc.get_full_chat_by_id(accid, chat_id)
     if SpecialContactId.SELF not in chat.contact_ids or len(chat.contact_ids) <= 1:
         with session_scope() as session:
             stmt = delete(Fchat).where(Fchat.accid == accid, Fchat.gid == chat_id)
             session.execute(stmt)
             bot.logger.debug(
                 f"group(id={chat_id}) subscriptions were deleted due to member-removed event"
             )
 
 
-@cli.on(events.NewMessage(is_info=False))
-def markseen_commands(bot: Bot, accid: int, event: AttrDict) -> None:
-    if not is_not_known_command(bot, event):
-        bot.rpc.markseen_msgs(accid, [event.msg.id])
+@cli.after(events.NewMessage)
+def delete_msgs(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    bot.rpc.delete_messages(accid, [event.msg.id])
+
 
+@cli.on(events.NewMessage(is_info=False))
+def on_message(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    if bot.has_command(event.command):
+        return
 
-@cli.on(events.NewMessage(is_info=False, func=is_not_known_command))
-def on_unknown_cmd(bot: Bot, accid: int, event: AttrDict) -> None:
     msg = event.msg
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
     if chat.chat_type == ChatType.SINGLE:
         bot.rpc.markseen_msgs(accid, [msg.id])
         send_help(bot, accid, event.msg.chat_id)
 
 
 @cli.on(events.NewMessage(command="/help"))
-def _help(bot: Bot, accid: int, event: AttrDict) -> None:
+def _help(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    bot.rpc.markseen_msgs(accid, [event.msg.id])
     send_help(bot, accid, event.msg.chat_id)
 
 
 def send_help(bot: Bot, accid: int, chat_id: int) -> None:
     text = """Hello, I'm a bot 🤖, with me you can subscribe group chats to RSS/Atom feeds.
 
 **Available commands**
@@ -150,58 +160,59 @@
 /list - List feed subscriptions in the group the command is sent.
 
 
 **How to use me?**
 
 Add me to a group then you can use the /sub command there to subscribe the group to RSS/Atom feeds.
     """
-    bot.rpc.send_msg(accid, chat_id, {"text": text})
+    bot.rpc.send_msg(accid, chat_id, MsgData(text=text))
 
 
-def _sub(max_feed_count: int, bot: Bot, accid: int, event: AttrDict) -> None:
+def _sub(max_feed_count: int, bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    bot.rpc.markseen_msgs(accid, [event.msg.id])
     chat = bot.rpc.get_basic_chat_info(accid, event.msg.chat_id)
     args = event.payload.split(maxsplit=1)
     url = normalize_url(args[0]) if args else ""
     filter_ = args[1] if len(args) == 2 else ""
 
     with session_scope() as session:
         feed = session.execute(select(Feed).where(Feed.url == url)).scalar()
         if feed:
             try:
                 d = parse_feed(feed.url)
             except Exception as ex:
-                reply = {
-                    "text": "❌ Invalid feed url.",
-                    "quotedMessageId": event.msg.id,
-                }
+                reply = MsgData(
+                    text="❌ Invalid feed url.",
+                    quoted_message_id=event.msg.id,
+                )
                 bot.rpc.send_msg(accid, event.msg.chat_id, reply)
                 bot.logger.exception("Invalid feed %s: %s", url, ex)
                 return
         else:
             stmt = select(func.count()).select_from(  # noqa: func.count is callable
                 Feed
             )
             if 0 <= max_feed_count <= session.execute(stmt).scalar_one():
-                reply = {"text": "❌ Sorry, maximum number of feeds reached"}
+                reply = MsgData(text="❌ Sorry, maximum number of feeds reached")
                 bot.rpc.send_msg(accid, event.msg.chat_id, reply)
                 return
             try:
                 d = parse_feed(url)
                 feed = Feed(
                     url=url,
                     etag=d.get("etag"),
                     modified=d.get("modified") or d.get("updated"),
                     latest=get_latest_date(d.entries),
                 )
                 session.add(feed)
             except Exception as ex:
-                reply = {
-                    "text": "❌ Invalid feed url.",
-                    "quotedMessageId": event.msg.id,
-                }
+                reply = MsgData(
+                    text="❌ Invalid feed url.",
+                    quoted_message_id=event.msg.id,
+                )
                 bot.rpc.send_msg(accid, event.msg.chat_id, reply)
                 bot.logger.exception("Invalid feed %s: %s", url, ex)
                 return
 
         if chat.chat_type == ChatType.SINGLE:
             chat_id = bot.rpc.create_group_chat(
                 accid, d.feed.get("title") or url, False
@@ -212,27 +223,27 @@
                 set_group_image(bot, url, accid, chat_id)
         else:
             chat_id = event.msg.chat_id
             stmt = select(Fchat).where(
                 Fchat.accid == accid, Fchat.gid == chat.id, Fchat.feed_url == feed.url
             )
             if session.execute(stmt).scalar():
-                reply = {
-                    "text": "❌ Chat already subscribed to that feed.",
-                    "quotedMessageId": event.msg.id,
-                }
+                reply = MsgData(
+                    text="❌ Chat already subscribed to that feed.",
+                    quoted_message_id=event.msg.id,
+                )
                 bot.rpc.send_msg(accid, chat_id, reply)
                 return
 
         session.add(Fchat(accid=accid, gid=chat_id, feed_url=feed.url, filter=filter_))
 
-    reply = {"text": _format_feed_info(d, feed.url, filter_)}
+    reply = MsgData(text=_format_feed_info(d, feed.url, filter_))
 
     if d.entries and feed.latest:
-        reply["html"] = format_entries(
+        reply.html = format_entries(
             get_old_entries(d.entries, tuple(map(int, feed.latest.split())))[:15],
             filter_,
         )
 
     bot.rpc.send_msg(accid, chat_id, reply)
 
 
@@ -240,15 +251,16 @@
     url = f"{url} ({filter_})" if filter_ else url
     title = d.feed.get("title") or "-"
     desc = d.feed.get("description") or "-"
     return f"Title: {title}\n\nURL: {url}\n\nDescription: {desc}"
 
 
 @cli.on(events.NewMessage(command="/unsub"))
-def _unsub(bot: Bot, accid: int, event: AttrDict) -> None:
+def _unsub(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    bot.rpc.markseen_msgs(accid, [event.msg.id])
     if not event.payload:
         _list(bot, accid, event)
         return
 
     msg = event.msg
     with session_scope() as session:
         stmt = select(Feed).where(Feed.url == normalize_url(event.payload))
@@ -259,34 +271,35 @@
                 Fchat.accid == accid,
                 Fchat.gid == msg.chat_id,
                 Fchat.feed_url == feed.url,
             )
             fchat = session.execute(stmt).scalar()
         if fchat:
             session.delete(fchat)
-            reply = {"text": f"Chat unsubscribed from: {feed.url}"}
+            reply = MsgData(text=f"Chat unsubscribed from: {feed.url}")
             bot.rpc.send_msg(accid, msg.chat_id, reply)
         else:
-            reply = {
-                "text": "❌ This chat is not subscribed to that feed",
-                "quotedMessageId": msg.id,
-            }
+            reply = MsgData(
+                text="❌ This chat is not subscribed to that feed",
+                quoted_message_id=msg.id,
+            )
             bot.rpc.send_msg(accid, msg.chat_id, reply)
 
 
 @cli.on(events.NewMessage(command="/list"))
-def _list(bot: Bot, accid: int, event: AttrDict) -> None:
+def _list(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    bot.rpc.markseen_msgs(accid, [event.msg.id])
     msg = event.msg
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
     if chat.chat_type == ChatType.SINGLE:
         text = (
             "❌ You must send that command in the group where you have the subscriptions.\n"
             "You can check the groups you share with me in my profile"
         )
-        reply = {"text": text, "quotedMessageId": msg.id}
+        reply = MsgData(text=text, quoted_message_id=msg.id)
     else:
         with session_scope() as session:
             stmt = select(Fchat).where(Fchat.accid == accid, Fchat.gid == msg.chat_id)
             fchats = session.execute(stmt).scalars()
             text = "\n\n".join(fchat.feed_url for fchat in fchats)
-        reply = {"text": text or "❌ No feed subscriptions in this chat"}
+        reply = MsgData(text=text or "❌ No feed subscriptions in this chat")
     bot.rpc.send_msg(accid, msg.chat_id, reply)
```

### Comparing `feedsbot-0.4.3/feedsbot/orm.py` & `feedsbot-0.5.0/feedsbot/orm.py`

 * *Files identical despite different names*

### Comparing `feedsbot-0.4.3/feedsbot/util.py` & `feedsbot-0.5.0/feedsbot/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Optional
 
 import bs4
 import feedparser
 import requests
-from deltabot_cli import Bot, JsonRpcError
+from deltachat2 import Bot, JsonRpcError, MsgData
 from feedparser.datetimes import _parse_date
 from feedparser.exceptions import CharacterEncodingOverride
 from sqlalchemy import delete, select, update
 
 from .orm import Fchat, Feed, session_scope
 
 www = requests.Session()
@@ -76,17 +76,17 @@
                 stmt = update(Feed).where(Feed.url == feed.url)
                 session.execute(stmt.values(errors=feed.errors + 1))
         else:
             with session_scope() as session:
                 stmt = select(Fchat.accid, Fchat.gid).where(Fchat.feed_url == feed.url)
                 fchats = session.execute(stmt).all()
                 session.execute(delete(Feed).where(Feed.url == feed.url))
-            reply = {
-                "text": f"❌ Due to errors, this chat was unsubscribed from feed: {feed.url}"
-            }
+            reply = MsgData(
+                text=f"❌ Due to errors, this chat was unsubscribed from feed: {feed.url}"
+            )
             for accid, gid in fchats:
                 try:
                     bot.rpc.send_msg(accid, gid, reply)
                 except JsonRpcError:
                     pass
     bot.logger.debug(f"Done checking feed: {feed.url}")
 
@@ -110,15 +110,15 @@
     for fchat in fchats:
         if fchat.filter:
             html = format_entries(d.entries[:100], fchat.filter)
             if not html:
                 continue
         else:
             html = full_html
-        reply = {"html": html, "OverrideSenderName": d.feed.get("title") or feed.url}
+        reply = MsgData(html=html, override_sender_name=d.feed.get("title") or feed.url)
         try:
             bot.rpc.send_msg(fchat.accid, fchat.gid, reply)
         except JsonRpcError:
             with session_scope() as session:
                 stmt = delete(Fchat).where(
                     Fchat.accid == fchat.accid, Fchat.gid == fchat.gid
                 )
```

### Comparing `feedsbot-0.4.3/feedsbot.egg-info/PKG-INFO` & `feedsbot-0.5.0/feedsbot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: feedsbot
-Version: 0.4.3
+Version: 0.5.0
 Summary: Subscribe to RSS/Atom feeds in Delta Chat
 Author-email: adbenitez <adb@merlinux.eu>
+Project-URL: Homepage, https://github.com/deltachat-bot/feedsbot
 Keywords: deltachat,bot,feeds,rss,atom
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deltabot-cli<6.0,>=5.0.0
+Requires-Dist: deltabot-cli<7.0,>=6.1.0
 Requires-Dist: SQLAlchemy<3.0,>=2.0.25
 Requires-Dist: feedparser<7.0,>=6.0.11
 Requires-Dist: requests<3.0,>=2.28.1
 Requires-Dist: beautifulsoup4<5.0,>=4.11.1
 Requires-Dist: html5lib>=1.1
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
```

### Comparing `feedsbot-0.4.3/pyproject.toml` & `feedsbot-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,25 @@
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 ]
 dependencies = [
-    "deltabot-cli>=5.0.0,<6.0",
+    "deltabot-cli>=6.1.0,<7.0",
     "SQLAlchemy>=2.0.25,<3.0",
     "feedparser>=6.0.11,<7.0",
     "requests>=2.28.1,<3.0",
     "beautifulsoup4>=4.11.1,<5.0",
     "html5lib>=1.1",
 ]
 
+[project.urls]
+Homepage = "https://github.com/deltachat-bot/feedsbot"
+
 [project.optional-dependencies]
 dev = [
   "black",
   "mypy",
   "isort",
   "pylint",
   "pylama",
@@ -38,13 +41,14 @@
 ]
 
 [project.scripts]
 feedsbot = "feedsbot:main"
 
 [tool.setuptools_scm]
 # can be empty if no extra settings are needed, presence enables setuptools_scm
+version_file = "feedsbot/_version.py"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 ignore_missing_imports = "True"
```

