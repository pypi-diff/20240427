# Comparing `tmp/deltachat_faqbot-0.5.1-py3-none-any.whl.zip` & `tmp/deltachat_faqbot-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 18209 bytes, number of entries: 11
--rw-r--r--  2.0 unx      164 b- defN 24-Apr-06 23:17 faqbot/__init__.py
--rw-r--r--  2.0 unx       65 b- defN 24-Apr-06 23:17 faqbot/__main__.py
--rw-r--r--  2.0 unx     7026 b- defN 24-Apr-06 23:17 faqbot/hooks.py
--rw-r--r--  2.0 unx     1250 b- defN 24-Apr-06 23:17 faqbot/orm.py
--rw-r--r--  2.0 unx      957 b- defN 24-Apr-06 23:17 faqbot/utils.py
--rw-r--r--  2.0 unx    35141 b- defN 24-Apr-06 23:17 deltachat_faqbot-0.5.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1504 b- defN 24-Apr-06 23:17 deltachat_faqbot-0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 23:17 deltachat_faqbot-0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       39 b- defN 24-Apr-06 23:17 deltachat_faqbot-0.5.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-06 23:17 deltachat_faqbot-0.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      899 b- defN 24-Apr-06 23:17 deltachat_faqbot-0.5.1.dist-info/RECORD
-11 files, 47144 bytes uncompressed, 16679 bytes compressed:  64.6%
+Zip file size: 18641 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      164 b- defN 24-Apr-27 20:51 faqbot/__init__.py
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-27 20:51 faqbot/__main__.py
+-rw-r--r--  2.0 unx      411 b- defN 24-Apr-27 20:51 faqbot/_version.py
+-rw-r--r--  2.0 unx     7028 b- defN 24-Apr-27 20:51 faqbot/hooks.py
+-rw-r--r--  2.0 unx     1250 b- defN 24-Apr-27 20:51 faqbot/orm.py
+-rw-r--r--  2.0 unx      957 b- defN 24-Apr-27 20:51 faqbot/utils.py
+-rw-r--r--  2.0 unx    35141 b- defN 24-Apr-27 20:51 deltachat_faqbot-0.6.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1504 b- defN 24-Apr-27 20:51 deltachat_faqbot-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-27 20:51 deltachat_faqbot-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 24-Apr-27 20:51 deltachat_faqbot-0.6.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-27 20:51 deltachat_faqbot-0.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      973 b- defN 24-Apr-27 20:51 deltachat_faqbot-0.6.0.dist-info/RECORD
+12 files, 47631 bytes uncompressed, 16999 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,34 +1,37 @@
 Filename: faqbot/__init__.py
 Comment: 
 
 Filename: faqbot/__main__.py
 Comment: 
 
+Filename: faqbot/_version.py
+Comment: 
+
 Filename: faqbot/hooks.py
 Comment: 
 
 Filename: faqbot/orm.py
 Comment: 
 
 Filename: faqbot/utils.py
 Comment: 
 
-Filename: deltachat_faqbot-0.5.1.dist-info/LICENSE.txt
+Filename: deltachat_faqbot-0.6.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: deltachat_faqbot-0.5.1.dist-info/METADATA
+Filename: deltachat_faqbot-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: deltachat_faqbot-0.5.1.dist-info/WHEEL
+Filename: deltachat_faqbot-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: deltachat_faqbot-0.5.1.dist-info/entry_points.txt
+Filename: deltachat_faqbot-0.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: deltachat_faqbot-0.5.1.dist-info/top_level.txt
+Filename: deltachat_faqbot-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: deltachat_faqbot-0.5.1.dist-info/RECORD
+Filename: deltachat_faqbot-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## faqbot/hooks.py

```diff
@@ -14,18 +14,20 @@
     MsgData,
     NewMsgEvent,
     events,
 )
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.future import select
 
+from ._version import __version__
 from .orm import FAQ, init, session_scope
 from .utils import get_answer_text, get_faq
 
 cli = BotCli("faqbot")
+cli.add_generic_option("-v", "--version", action="version", version=__version__)
 
 
 @cli.on_init
 def on_init(bot: Bot, _args: Namespace) -> None:
     for accid in bot.rpc.get_all_account_ids():
         if not bot.rpc.get_config(accid, "displayname"):
             bot.rpc.set_config(accid, "displayname", "FAQ Bot")
@@ -54,14 +56,15 @@
                 bot.logger.debug("QR scanned by contact=%s", event.contact_id)
                 chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
                 send_help(bot, accid, chatid)
 
 
 @cli.on(events.NewMessage(command="/help"))
 def _help(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    bot.rpc.markseen_msgs(accid, [event.msg.id])
     send_help(bot, accid, event.msg.chat_id)
 
 
 def send_help(bot: Bot, accid: int, chat_id: int) -> None:
     text = """**Available commands**
 
 /faq - sends available topics.
@@ -149,20 +152,14 @@
             " use /remove first to remove the old reply",
             quoted_message_id=msg.id,
         )
     bot.rpc.send_msg(accid, msg.chat_id, reply)
 
 
 @cli.on(events.NewMessage(is_info=False))
-def markseen_commands(bot: Bot, accid: int, event: NewMsgEvent) -> None:
-    if bot.has_command(event.command):
-        bot.rpc.markseen_msgs(accid, [event.msg.id])
-
-
-@cli.on(events.NewMessage(is_info=False))
 def _answer(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     if bot.has_command(event.command):
         return
     msg = event.msg
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
     if chat.chat_type == ChatType.SINGLE:
         bot.rpc.markseen_msgs(accid, [msg.id])
@@ -190,14 +187,15 @@
             else:
                 bot.rpc.send_msg(accid, msg.chat_id, reply)
 
 
 def reply_to_command_in_dm(bot: Bot, accid: int, msg: Message) -> bool:
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
     if chat.chat_type == ChatType.SINGLE:
+        bot.rpc.markseen_msgs(accid, [msg.id])
         reply = MsgData(
             text="Can't save notes in private, add me to a group and use the command there",
             quoted_message_id=msg.id,
         )
         bot.rpc.send_msg(accid, msg.chat_id, reply)
         return True
     return False
```

## Comparing `deltachat_faqbot-0.5.1.dist-info/LICENSE.txt` & `deltachat_faqbot-0.6.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `deltachat_faqbot-0.5.1.dist-info/METADATA` & `deltachat_faqbot-0.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: deltachat-faqbot
-Version: 0.5.1
+Version: 0.6.0
 Summary: FAQ bot, help to answer common questions in support groups
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/faqbot
 Keywords: deltachat,bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: SQLAlchemy <3.0,>=2.0.25
-Requires-Dist: deltabot-cli <7.0,>=6.0.0
+Requires-Dist: deltabot-cli <7.0,>=6.1.0
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: pylint ; extra == 'dev'
 Requires-Dist: pylama ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
```

## Comparing `deltachat_faqbot-0.5.1.dist-info/RECORD` & `deltachat_faqbot-0.6.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 faqbot/__init__.py,sha256=HQDDaYy2LJKcpbyq3SCzQ6LLYe8elUMIC6ORVAgMt_4,164
 faqbot/__main__.py,sha256=M7jcIQ0wYwLot7bzOqMQUEJv_190nXbdctI6hrTINbA,65
-faqbot/hooks.py,sha256=dC6q9wI4iAsXGN56CrAH13aG55kotAw8vg5pkxoeHPA,7026
+faqbot/_version.py,sha256=2JKwcA-YQ0okV2N-gwTWy_n51igWrPcsKQFm0cnqsvw,411
+faqbot/hooks.py,sha256=8juttTQ6WjIWiOXUBxeyfSXt_zElvVFWHGZd1ysYmNo,7028
 faqbot/orm.py,sha256=01QrRfYB3nk6nx9V0CEWkBhrebz3nC0O06q-6aHUu9U,1250
 faqbot/utils.py,sha256=HPMshutjdZMoUnwiUUqQ2CGMqyCqfR6aSMlzsB8DP8U,957
-deltachat_faqbot-0.5.1.dist-info/LICENSE.txt,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
-deltachat_faqbot-0.5.1.dist-info/METADATA,sha256=Cnbq0OvObxyJvXmiYbeoi_OeOvuG1l3K8bq1s2jOrQg,1504
-deltachat_faqbot-0.5.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-deltachat_faqbot-0.5.1.dist-info/entry_points.txt,sha256=LPihtLfVtOY_74CMHDuB2b-o-S4mxY8J32JNubC7uVc,39
-deltachat_faqbot-0.5.1.dist-info/top_level.txt,sha256=owc81PC21g6sHQ1ESOzXn8ZV_85OmuEq4RplpAErzd8,7
-deltachat_faqbot-0.5.1.dist-info/RECORD,,
+deltachat_faqbot-0.6.0.dist-info/LICENSE.txt,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
+deltachat_faqbot-0.6.0.dist-info/METADATA,sha256=1mQ6SEWzxWgiz9bH_-8CigYNZuY6f4TsIulasGPTOdc,1504
+deltachat_faqbot-0.6.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+deltachat_faqbot-0.6.0.dist-info/entry_points.txt,sha256=LPihtLfVtOY_74CMHDuB2b-o-S4mxY8J32JNubC7uVc,39
+deltachat_faqbot-0.6.0.dist-info/top_level.txt,sha256=owc81PC21g6sHQ1ESOzXn8ZV_85OmuEq4RplpAErzd8,7
+deltachat_faqbot-0.6.0.dist-info/RECORD,,
```

