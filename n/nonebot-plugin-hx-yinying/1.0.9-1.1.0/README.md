# Comparing `tmp/nonebot-plugin-hx-yinying-1.0.9.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.0.9.tar", last modified: Fri Apr 26 07:24:31 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.1.0.tar", last modified: Sat Apr 27 15:23:38 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.0.9.tar` & `nonebot-plugin-hx-yinying-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:31.484044 nonebot-plugin-hx-yinying-1.0.9/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     5087 2024-04-26 07:24:31.484044 nonebot-plugin-hx-yinying-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4647 2024-04-25 16:11:37.000000 nonebot-plugin-hx-yinying-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:31.309713 nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    65155 2024-04-26 06:55:26.000000 nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    90994 2024-04-26 06:44:51.000000 nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      396 2024-04-26 06:52:41.000000 nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying/config.py
--rw-rw-rw-   0        0        0       92 2024-04-26 07:22:58.000000 nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying/report.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:31.484044 nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     5087 2024-04-26 07:24:30.000000 nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-04-26 07:24:30.000000 nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 07:24:30.000000 nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      175 2024-04-26 07:24:30.000000 nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-26 07:24:30.000000 nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-26 07:24:31.509175 nonebot-plugin-hx-yinying-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      895 2024-04-26 07:23:51.000000 nonebot-plugin-hx-yinying-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 15:23:38.393370 nonebot-plugin-hx-yinying-1.1.0/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5087 2024-04-27 15:23:38.393370 nonebot-plugin-hx-yinying-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4647 2024-04-25 16:11:37.000000 nonebot-plugin-hx-yinying-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 15:23:38.151995 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    56726 2024-04-27 15:15:42.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    95541 2024-04-27 15:16:04.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      396 2024-04-27 15:10:23.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/config.py
+-rw-rw-rw-   0        0        0     2998 2024-04-27 15:19:03.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/report.py
+drwxrwxrwx   0        0        0        0 2024-04-27 15:23:38.393370 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     5087 2024-04-27 15:23:37.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-04-27 15:23:37.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 15:23:37.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      222 2024-04-27 15:23:37.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-27 15:23:37.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-27 15:23:38.406330 nonebot-plugin-hx-yinying-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-04-27 15:22:00.000000 nonebot-plugin-hx-yinying-1.1.0/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.0.9/LICENSE` & `nonebot-plugin-hx-yinying-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.0.9/PKG-INFO` & `nonebot-plugin-hx-yinying-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.0.9
+Version: 1.1.0
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.9 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.0 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.0.9/README.md` & `nonebot-plugin-hx-yinying-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from nonebot.plugin import PluginMetadata
-from .config import Config
 from nonebot import on_command, on_message ,get_plugin_config,require
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import (
     Bot,
     GroupMessageEvent,
@@ -11,17 +10,19 @@
     Message,
     Event,
 )
 from html import unescape
 from nonebot.typing import T_State
 from nonebot.log import logger
 from nonebot.matcher import Matcher
-from nonebot.rule import to_me
+from nonebot.rule import to_me,Rule
 import json,os,random
+from .config import Config
 from .chat import *
+from .report import post_run
 
 __plugin_meta__ = PluginMetadata(
     name="Hx_YinYing",
     description="快来和可爱的赛博狼狼聊天！",
     usage=(
         "通过QQ艾特机器人来进行对话"
     ),
@@ -58,15 +59,15 @@
 
 #检查关键配置
 if hx_config.yinying_appid == None or hx_config.yinying_token == None:
     logger.opt(colors=True).error("未设置核心配置？！,请检查你配置里的yinying_appid和yinying_token")
 else:
     logger.opt(colors=True).success("【Hx】加载核心配置成功")
 
-#根据订阅信息注册定身任务
+#根据订阅信息注册定时任务
 try:
     extent = int(len(dy_list))
     for key in dy_list:
         config_1 = config_in_user(key,False)
         user_config = json_get(config_1,key)
         config_time = json_get_time(user_config,"dy_time")
         config_minute = json_get_time(user_config,"dy_minute")
@@ -91,36 +92,31 @@
     <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
 """)
 except Exception as e:
     logger.opt(colors=True).error(f"【Hx】:错误捕获{e}，联系开发者！")
     logger.opt(colors=True).error("【Hx】定时任务加载失败！！，联系开发者！")
 
 #主要命令列表
-msg_at = on_message(rule=to_me(), priority=10, block=True)
-msg_ml = on_command("hx", aliases={"chat"}, priority=10, block=True)
-clear =  on_command("刷新对话", aliases={"clear"}, priority=0, block=True)
-history_get = on_command("导出对话", aliases={"getchat"}, priority=0, block=True)
-set_global_config = on_command("设置全局配置", aliases={"设置配置全局","globalset"}, priority=0, block=True)
-set_get_global = on_command("导出全局设置", aliases={"getset_global"}, priority=0, block=True)
-model_list = on_command("模型列表", aliases={"modellist","chat模型列表"}, priority=0, block=True)
-model_handoff = on_command("切换模型", aliases={"qhmodel","切换chat模型","模型切换"}, priority=0, block=True)
-rule_reply = on_command("对话回复", aliases={"chat回复"}, priority=0, block=True)
-rule_reply_at = on_command("回复艾特", aliases={"chat回复艾特"}, priority=0, block=True)
-private = on_command("私聊回复", aliases={"私聊chat"}, priority=0, block=True)
-at_reply = on_command("艾特回复", aliases={"bot艾特回复"}, priority=0, block=True)
-easycyber_set = on_command("easycyber", aliases={"easycyber设置","hxworld"}, priority=0, block=True)
-cyber_set = on_command("cyber", aliases={"cyber设置","Hxworld"}, priority=0, block=True)
-admin_set = on_command("控制台操作", aliases={"管理控制台","setstart"}, priority=0, block=True)
-verision = on_command("确认版本", aliases={"旅行伙伴确认","版本确认"}, priority=0, block=True)
-character = on_command("sd", aliases={"旅行伙伴加入","设定加入"}, priority=0, block=True)
-chat_ne = on_command("加入订阅", aliases={"旅行伙伴觉醒","订阅加入"}, priority=0, block=True)
-ces = on_command("ces", aliases={"测试"}, priority=0, block=True)
+msg_at = on_message(rule=Rule(chek_rule_base)&to_me(), priority=10,  block=True)
+msg_ml = on_command("hx", aliases={"chat"},rule=Rule(chek_rule_base),  priority=10, block=True)
+clear =  on_command("刷新对话", aliases={"clear"},rule=Rule(chek_rule_base),  priority=0, block=True)
+history_get = on_command("导出对话", aliases={"getchat"},rule=Rule(chek_rule_base),  priority=0, block=True)
+set_global_config = on_command("设置全局配置", aliases={"设置配置全局","globalset"},rule=Rule(chek_rule_admin),  priority=0, block=True)
+model_list = on_command("模型列表", aliases={"modellist","chat模型列表"},rule=Rule(chek_rule_base),  priority=0, block=True)
+model_handoff = on_command("切换模型", aliases={"qhmodel","切换chat模型","模型切换"},rule=Rule(chek_rule_base),  priority=0, block=True)
+easycyber_set = on_command("easycyber", aliases={"easycyber设置","hxworld"},rule=Rule(chek_rule_base),  priority=0, block=True)
+cyber_set = on_command("cyber", aliases={"cyber设置","Hxworld"},rule=Rule(chek_rule_base),  priority=0, block=True)
+admin_set = on_command("控制台操作", aliases={"管理控制台","setstart"},rule=Rule(chek_rule_admin),  priority=0, block=True)
+verision = on_command("确认版本", aliases={"旅行伙伴确认","版本确认"},rule=Rule(chek_rule_base),  priority=0, block=True)
+character = on_command("sd", aliases={"旅行伙伴加入","设定加入"},rule=Rule(chek_rule_base),  priority=0, block=True)
+chat_ne = on_command("加入订阅", aliases={"旅行伙伴觉醒","订阅加入"},rule=Rule(chek_rule_base),  priority=0, block=True)
+ces = on_command("ces", aliases={"测试"},rule=Rule(chek_rule_base), priority=0, block=True)
 
 @character.handle()
-async def character(matcher: Matcher,bot:Bot, event: MessageEvent, events:Event, msg: Message = CommandArg()):
+async def character(matcher: Matcher,bot:Bot, event: MessageEvent, msg: Message = CommandArg()):
     user = get_id(event)
     nick = await get_nick(bot,event)
     config = config_in_user(user,nick)
     config_get = json_get(config,user)
     text = msg.extract_plain_text()
     if text == "" or text == None:
         msg = "没有获取到要加入伙伴的设定哦"
@@ -146,17 +142,17 @@
                 msg = "没有获取到要加入伙伴的设定哦"
             await send_msg(matcher, event, msg)
         except Exception as e:
             msg = False
             logger.opt(colors=True).error(f"{e}")
         
 @verision.handle()
-async def verision_get(matcher: Matcher, event: MessageEvent, events:Event):
+async def verision_get(matcher: Matcher, event: MessageEvent):
     new_verision, time = update_hx()
-    if isinstance(events, GroupMessageEvent):
+    if get_groupid(event):
         id = get_groupid(event)
         e_config = config_in_group(id)
         config = json_get(e_config,id)
         model = json_get(config,"use_model")
         if not new_verision and not hx_config.hx_version:
             if model == "easycyberfurry-001":
                 model_in = json_get(config,"easycharacter_in")
@@ -210,30 +206,20 @@
                     msg =f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
                 msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
             else:
                 msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
         await send_msg(matcher, event, msg)
 
 @msg_at.handle()
-async def at(matcher: Matcher, event: MessageEvent, bot: Bot, events:Event):
-    config_global = config_in_global()
-    at_reply = json_get(config_global,"at_reply")
-    if not at_reply:
-        logger.opt(colors=True).warning("由于艾特回复被设置为false，此条消息忽略")
-    elif isinstance(events, GroupMessageEvent):
-        await get_answer_at(matcher, event, bot)
-    elif json_get(config_in_global(),"private"):
-        await get_answer_at(matcher, event, bot)
+async def at(matcher: Matcher, event: MessageEvent, bot: Bot):
+    await get_answer_at(matcher, event, bot)
 
 @msg_ml.handle()
-async def ml(matcher: Matcher, event: MessageEvent, bot: Bot, events:Event, msg: Message = CommandArg()):
-    if isinstance(events, GroupMessageEvent):
-        await get_answer_ml(matcher, event, bot ,msg)
-    elif json_get(config_in_global(),"private"):
-        await get_answer_ml(matcher, event, bot ,msg)
+async def ml(matcher: Matcher, event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
+    await get_answer_ml(matcher, event, bot ,msg)
 
 @clear.handle()
 async def clear(matcher: Matcher,bot:Bot, event: MessageEvent):
     id = get_id(event)
     nick = await get_nick(bot,event)
     if clear_id(id,nick):
         msg = "已刷新对话！"
@@ -291,36 +277,40 @@
                 else:
                     return
         
         if s["last"] == "修改TF":
             config = config_in_global()
             config_name = s["set"]
             get_config = json_get_text(config,config_name)
-            if text == "on" or text == "开" or text == True:
-                text = True
-            elif text == "off" or text == "关" or text == False:
-                text = False
+            key = {"on":False,"off":False,"开":True,"关":False,"开启":True,"关闭":False}
+            if text in key:
+                s["last"] = True
+                text = key[f"{text}"]
                 if get_config and text:
                     msg = f"该配置项[{config_name}]已经开启了，不需要重复开启噢"
+                    await send_msg(matcher,event,msg)
                 elif not get_config and not text:
                     msg = f"该配置项[{config_name}]已经关闭了，不需要重复关闭噢"
+                    await send_msg(matcher,event,msg)
                 elif text:
                     config[f"{config_name}"] = True
                     with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
                     msg = f"{config_name}的状态已更改为{text}"
+                    await send_msg(matcher,event,msg)
                 elif not text:
                     config[f"{config_name}"] = False
                     with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
                     msg = f"{config_name}的状态已更改为{text}"
-            s["last"] = True
-            if text == "退出":
-                msg = "已退出"
-            await send_msg(matcher,event,msg)        
+            else:
+                msg = "未知"
+            await send_msg(matcher,event,msg) 
+                
+     
         
         if s["last"] == "修改w":
             config = config_in_global()
             config_name = s["set"]
             get_config = json_get_text(config,config_name)
             config[f"{config_name}"] = int(text)
             with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
@@ -398,19 +388,19 @@
         return
     else:
         msg = f"未知命令“{text}”，已退出"
         await send_msg(matcher,event,msg)
 
 @history_get.handle()
 async def history(bot: Bot, event: MessageEvent,events: Event):
-    id = get_id(events)
+    id = get_id(event)
     msg_list = await get_history(id,bot,event)
     if isinstance(events, GroupMessageEvent):
         await bot.send_group_forward_msg(group_id=event.group_id, messages=msg_list)  # type: ignore
-    elif json_get(config_in_global(),"private"):
+    else:
         await bot.send_private_forward_msg(user_id=id, messages=msg_list)  # type: ignore
 
 @model_list.handle()
 async def list(matcher: Matcher, event: MessageEvent):
         msg = "1.yinyingllm-v1\n2.yinyingllm-v2\n3.yinyingllm-v3\n4.cyberfurry-001\n5.easycyberfurry-001\n切换模型请发送:切换模型(序号)"
         await send_msg(matcher, event, msg)
 
@@ -452,167 +442,14 @@
                     clear_id(id,nick)
                     msg =f"切换成功（当前模型已切换为{model})"
                     await send_msg(matcher,event,msg)
     else:
         msg = "请注意，切换模型后不能为空哦"
         await send_msg(matcher,event,msg)
 
-@rule_reply.handle()
-async def reply(matcher: Matcher, event: MessageEvent, msg: Message = CommandArg()):
-    text = msg.extract_plain_text()
-    if not text == "" or text == None:
-        if text == "开启" or text == "on" or text == "开":
-            config_global = config_in_global()
-            zt_reply = json_get(config_global,"reply")
-            if zt_reply == True:
-                msg = "请勿重复开启对话回复哦"
-                await send_msg(matcher,event,msg)
-            else:
-                config_global["reply"] = True
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                    json.dump(config_global,file) 
-                msg = "对话回复已开启"
-                await send_msg(matcher,event,msg)
-        elif text == "关闭" or text == "off" or text == "关":
-            config_global = config_in_global()
-            zt_reply = json_get(config_global,"reply")
-            if zt_reply == False:
-                msg = "请勿重复关闭对话回复哦"
-                await send_msg(matcher,event,msg)
-            else:
-                config_global["reply"] = False
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                    json.dump(config_global,file)
-                msg = "对话回复已关闭"
-                await send_msg(matcher,event,msg)
-    else:
-        msg = f"请注意，正确的格式应该是\n对话回复{text}"
-        await send_msg(matcher,event,msg)
-
-@rule_reply_at.handle()
-async def reply_at(matcher: Matcher, event: MessageEvent, msg: Message = CommandArg()):
-    text = msg.extract_plain_text()
-    if not text == "" or text == None:
-        if json_get(config_in_global(),"reply") == False:
-            if text == "开启" or text == "on" or text == "开":
-                config_global = config_in_global()
-                zt_reply = json_get(config_global,"reply_at")
-                if zt_reply == True:
-                    msg = "请勿重复开启回复艾特哦"
-                    await send_msg(matcher,event,msg)
-                else:
-                    config_global["reply_at"] = True
-                    with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                        json.dump(config_global,file) 
-                    msg = "回复艾特已开启"
-                    await send_msg(matcher,event,msg)
-            elif text == "关闭" or text == "off" or text == "关":
-                config_global = config_in_global()
-                zt_reply = json_get(config_global,"reply_at")
-                if zt_reply == False:
-                    msg = "请勿重复关闭对话回复哦"
-                    await send_msg(matcher,event,msg)
-                else:
-                    config_global["reply_at"] = False
-                    with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                        json.dump(config_global,file)
-                    msg = "回复艾特已关闭"
-                    await send_msg(matcher,event,msg)
-        else:
-            msg = "在对话回复开启的状况下（,回复艾特无效"
-            await send_msg(matcher,event,msg)
-    else:
-        msg = f"请注意，正确的格式应该是\n回复艾特{text}"
-        await send_msg(matcher,event,msg)
-
-@set_get_global.handle()
-async def get_config(bot:Bot, event: MessageEvent,events: Event):
-    id = get_id(events)
-    msg_list = await get_config_global()
-    if isinstance(events, GroupMessageEvent):
-        await bot.send_group_forward_msg(group_id=event.group_id, messages=msg_list)  # type: ignore
-    elif json_get(config_in_global(),"private"):
-        await bot.send_private_forward_msg(user_id=id, messages=msg_list)  # type: ignore
-
-@private.handle()
-async def reply(matcher: Matcher, bot: Bot, event: MessageEvent, msg: Message = CommandArg()):
-    text = msg.extract_plain_text()
-    if not text == "" or text == None:
-        if text == "开启" or text == "on" or text == "开":
-            config_global = config_in_global()
-            zt_reply = json_get(config_global,"private")
-            if zt_reply == True:
-                msg = "请勿重复开启私聊回复哦"
-                await send_msg(matcher,event,msg)
-            else:
-                config_global["private"] = True
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                    json.dump(config_global,file) 
-                msg = "私聊回复已启用"
-                await send_msg(matcher,event,msg)
-        elif text == "关闭" or text == "off" or text == "关":
-            config_global = config_in_global()
-            zt_reply = json_get(config_global,"private")
-            if zt_reply == False:
-                msg = "请勿重复关闭私聊回复哦"
-                await send_msg(matcher,event,msg)
-            else:
-                config_global["private"] = False
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                    json.dump(config_global,file)
-                msg = "私聊回复已停用"
-                await send_msg(matcher,event,msg)
-    else:
-        msg = f"请注意，正确的格式应该是\n私聊回复{text}"
-        await send_msg(matcher,event,msg)
-
-@at_reply.handle()
-async def reply(matcher: Matcher, bot: Bot, event: MessageEvent, msg: Message = CommandArg()):
-    text = msg.extract_plain_text()
-    if not text == "" or text == None:
-        if text == "开启" or text == "on" or text == "开":
-            config_global = config_in_global()
-            at_reply = json_get(config_global,"at_reply")
-            if not at_reply:
-                config_global["at_reply"] = True
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                    json.dump(config_global,file) 
-                msg = "艾特回复已启用【bot被@将会回复】"
-                await send_msg(matcher,event,msg)
-            elif at_reply == True:
-                msg = "请勿重复开启艾特回复哦【bot被@已经会回复了】"
-                await send_msg(matcher,event,msg)
-            else:
-                config_global["at_reply"] = True
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                    json.dump(config_global,file) 
-                msg = "艾特回复已启用【bot被@将会回复】"
-                await send_msg(matcher,event,msg)
-        elif text == "关闭" or text == "off" or text == "关":
-            config_global = config_in_global()
-            at_reply = json_get(config_global,"at_reply")
-            if not at_reply:
-                config_global["at_reply"] = False
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                    json.dump(config_global,file)
-                msg = "艾特回复已停用【bot被@回复已停用】"
-                await send_msg(matcher,event,msg)
-            elif at_reply == False:
-                msg = "请勿重复关闭艾特回复哦【bot被@已经不会回复了】"
-                await send_msg(matcher,event,msg)
-            else:
-                config_global["at_reply"] = False
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                    json.dump(config_global,file) 
-                msg = "艾特回复已停用【bot被@回复已停用】"
-                await send_msg(matcher,event,msg)
-    else:
-        msg = f"请注意，正确的格式应该是\n私聊回复{text}"
-        await send_msg(matcher,event,msg)
-
 @easycyber_set.got(
     "msg",
     prompt=f"发送以下选项执行相应功能\n投稿 #投稿自定义预设(不允许同名)\n载入 #载入自定义预设(不允许不存在)\n查看列表 #列出所有公开的自定义预设\n退出 #退出设置\n发送非预期命令则退出",
 )
 async def _(matcher: Matcher, bot:Bot, event: MessageEvent, s: T_State,events: Event):
     id = get_id(event)
     text = unescape(event.get_plaintext().strip())
@@ -1171,10 +1008,10 @@
     if s["last"]:
         return
     else:
         msg = f"未知命令“{text}”，已退出"
         await send_msg(matcher,event,msg)
 
 @ces.handle()
-async def _(event: MessageEvent):
+async def _(event: MessageEvent,msg: Message = CommandArg()):
     id = get_id(event)
-    await get_chat(id)
+    await get_id()
```

### Comparing `nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -- coding: utf-8 --**
-from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent ,MessageSegment ,Message
+from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent ,MessageSegment ,Message,MessageEvent,Event
 from html import unescape
 from typing import List
 import os,httpx, json, time, requests,loguru,platform
 from loguru import logger as lg
 from .config import Config
 import operator,nonebot
+from nonebot.params import EventToMe,EventParam
 from nonebot import get_plugin_config, logger, require,get_driver
 from pathlib import Path
 require("nonebot_plugin_localstore")
+from nonebot.rule import to_me
 import nonebot_plugin_localstore as store
 
 
 hx_config = get_plugin_config(Config)
 
-
 #判断主要配置文件夹是否存在！
 sys = platform.system()
 if sys == "Windows":
     if hx_config.hx_path == None:
         logger.warning("找不到配置里的路径，将使用默认配置[Windows]")
         lg.opt(colors=True).success( f"""
         <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
@@ -225,14 +226,37 @@
         await matcher.reject(content, at_sender=reply_at)
 
 #创建用户文件夹
 def create_dir_usr(path):
     if not os.path.exists(path):
         os.mkdir(path)
 
+#获取json函数
+def json_get(json,key) -> str:
+    try:
+        back = json[f"{key}"]
+    except Exception as e:
+        back = False
+    return back
+
+def json_get_text(json,key) -> str:
+    try:
+        back = json[f"{key}"]
+    except Exception as e:
+        back = 0
+    return back
+
+def json_get_time(json,key) -> str:
+    try:
+        back = json[f"{key}"]
+    except Exception as e:
+        back = 1
+    return back
+
+
 #json转义防止爆炸（）
 def json_replace(text) -> str:
     text = text.replace('\n','/n')
     text = text.replace('\t','/t')
     text = text.replace("'","/'")
     text = text.replace('"','/"')
     return text
@@ -619,30 +643,31 @@
             create_dir_usr(f"{log_dir}/config")
             with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                 json_data = {}
                 admin_user = []
                 black_user = []
                 black_group = []
                 black_world = []
-                write_group = []
+                white_group = []
                 dy_list_r = []
-                write_user = []
+                white_user = []
                 json_data['global_switch'] = True
                 json_data['admin_pro'] = None
                 json_data['admin_group'] = None
                 json_data['admin_group_switch'] = True
                 json_data['admin_user_switch'] = False
                 json_data['limit'] = 12
                 json_data['at_reply'] = True
                 json_data['reply'] = False
                 json_data['reply_at'] = False
                 json_data['private'] = True
                 json_data['dy_list'] = dy_list_r
-                json_data['write_user'] = write_user
-                json_data['write_group'] = write_group
+                json_data['rule_model'] = "black"
+                json_data['white_user'] = white_user
+                json_data['white_group'] = white_group
                 json_data['admin_user'] = admin_user
                 json_data['blacklist_user'] = black_user
                 json_data['blacklist_group'] = black_group
                 json_data['blacklist_world'] = black_world
                 json.dump(json_data,file)
                 back = json_data
     except Exception as e:
@@ -652,30 +677,31 @@
             logger.warning(f"报错捕获{e}")
             with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                 json_data = {}
                 admin_user = []
                 black_user = []
                 black_group = []
                 black_world = []
-                write_group = []
+                white_group = []
                 dy_list_r = []
-                write_user = []
+                white_user = []
                 json_data['global_switch'] = True
                 json_data['admin_pro'] = None
                 json_data['admin_group'] = None
                 json_data['admin_group_switch'] = True
                 json_data['admin_user_switch'] = False
                 json_data['limit'] = 12
                 json_data['at_reply'] = True
                 json_data['reply'] = False
                 json_data['reply_at'] = False
                 json_data['private'] = True
                 json_data['dy_list'] = dy_list_r
-                json_data['write_user'] = write_user
-                json_data['write_group'] = write_group
+                json_data['rule_model'] = "black"
+                json_data['white_user'] = white_user
+                json_data['white_group'] = white_group
                 json_data['admin_user'] = admin_user
                 json_data['blacklist_user'] = black_user
                 json_data['blacklist_group'] = black_group
                 json_data['blacklist_world'] = black_world
                 json.dump(json_data,file)
                 back = json_data
     return back
@@ -855,43 +881,150 @@
         else:
             logger.error(f"配置文件不存在！")
     except Exception as e:
         logger.warning(f"报错捕获{e}")
         logger.error(f"报错定位于获取配置内鉴值")
     return tf_key, w_key, list_key
 
+#获取nonebot超级管理组
+def get_superuser() -> list:
+    list_superuser = get_driver().config.superusers
+    try:
+        if list_superuser == None or not list_superuser:
+            superuser = ["3485462167"]
+        else:
+            superuser = get_driver().config.superusers
+    except Exception as e:
+            logger.warning(f"报错捕获{e}")
+            superuser = ["3485462167"]
+    return superuser
+
 #全局权限检查！！！！！（总算写出来了）
 def place(id) -> int:
     try:
         config = config_in_global()
         admin_pro = json_get(config,"admin_pro")
         admin_user = json_get(config,"admin_user")
         black_list = json_get(config,"blacklist_user")
-        superuser = get_driver().config.superusers
+        superuser = get_superuser()
         logger.warning(f"user捕获{superuser}")
-        if id in superuser:
+        if f"{id}" in superuser:
             place_user = 10
         elif id == admin_pro:
             place_user = 10
         elif id in admin_user:
             place_user = 9
         elif id in black_list:
             place_user = 1
         else:
             place_user = 5
     except Exception as e:
             logger.warning(f"报错捕获{e}")
             place_user = 5
     return place_user
 
+#rule---管理组
+async def chek_rule_admin(event:MessageEvent):
+    id = get_id(event)
+    config = config_in_global()
+    admin_list = json_get(config,"admin_user")
+    admin_pro = json_get(config,"admin_pro")
+    supuser = get_superuser()
+    try:
+        if id in admin_list or id == admin_pro or id in supuser:
+            return True
+        else:
+            return False
+    except Exception as e:
+            logger.error(f"报错捕获{e}")
+            logger.error(f"你的配置文件错误或已过时！！，权限控制失效！")
+            return True
+
+#rule---用户组
+async def chek_rule_base(bot:Bot,event:MessageEvent,eve:Event):
+    id = get_id(event)
+    groupid = get_groupid(event)
+    config = config_in_global()
+    admin_list = json_get(config, "admin_user")
+    admin_pro = json_get(config, "admin_pro")
+    supuser = get_superuser()
+    white_group = json_get(config, "white_group")
+    white_user = json_get(config, "white_user")
+    black_group = json_get(config, "blacklist_group")
+    black_user = json_get(config, "blacklist_user")
+    rule_mode = json_get(config, "rule_model")
+    at_reply = json_get(config, "at_reply")
+    private = json_get(config, "private")
+    try:
+        if isinstance(eve, GroupMessageEvent):
+            to_bot = event.to_me
+            if rule_mode == "black":
+                if id in admin_list or id == admin_pro or id in supuser:
+                    return True
+                elif groupid in white_group or id in white_user:
+                    return True
+                elif groupid in black_group:
+                    return False
+                elif id in black_user:
+                    return False
+                elif at_reply is False and to_bot:
+                    logger.warning(f"配置文件中该项配置为False，该消息不予处理")
+                    return False
+                else:
+                    return True
+            elif rule_mode == "white":
+                if id in admin_list or id == admin_pro or id in supuser:
+                    return True
+                elif at_reply is False and to_bot:
+                    return False
+                elif groupid in white_group or id in white_user:
+                    return True
+                else:
+                    return False
+            else:
+                logger.error(f"你的配置文件错误或已过时！！，权限控制失效！")
+                return True
+        elif not isinstance(eve, GroupMessageEvent) and private is False:
+            return False
+        else:
+            if rule_mode == "black":
+                if id in admin_list or id == admin_pro or id in supuser:
+                    return True
+                elif groupid in white_group or id in white_user:
+                    return True
+                elif groupid in black_group:
+                    return False
+                elif id in black_user:
+                    return False
+                elif at_reply is False:
+                    return False
+                else:
+                    return True
+            elif rule_mode == "white":
+                if id in admin_list or id == admin_pro or id in supuser or id in white_user:
+                    return True
+                elif at_reply is False:
+                    return False
+                elif groupid in json_get(config,"white_group"):
+                    return True
+                else:
+                    return False
+            else:
+                logger.error(f"你的配置文件错误或已过时！！，权限控制失效！")
+                return True
+    except Exception as e:
+            logger.error(f"报错捕获{e}")
+            logger.error(f"你的配置文件错5654误或已过时！！，权限控制失效！")
+            return True
+
 #尝试获取bot本地文件夹文件
 def file_get(file) -> str:
     try:
         if os.path.exists(f"{log_dir}/file/{file}"):
-            back = True
+            back = f"{log_dir}/file/{file}"
         else:
             back = False
     except Exception as e:
         back = False
     return back
 
 #历史消息卡片构建
@@ -931,14 +1064,15 @@
                 user_id=3485462167,
                 nickname="AAA星佑批发（幻歆限定）",
                 content=Message("合并消息时出错！"),
             )
         ]
     return msg_list
 
+
 #全局配置卡片构建
 async def get_config_global() -> List[MessageSegment]:
     config = config_in_global()
     msg_list = []
     try:
         reply = config["reply"]
         reply_at = config["reply_at"]
@@ -1078,35 +1212,14 @@
                     user_name = user_info.get("card", None) or user_info.get(
                         "nickname", None
                     )
                     if user_name:
                         msg
     return msg
 
-#获取json函数
-def json_get(json,key) -> str:
-    try:
-        back = json[f"{key}"]
-    except Exception as e:
-        back = False
-    return back
-
-def json_get_text(json,key) -> str:
-    try:
-        back = json[f"{key}"]
-    except Exception as e:
-        back = 0
-    return back
-
-def json_get_time(json,key) -> str:
-    try:
-        back = json[f"{key}"]
-    except Exception as e:
-        back = 1
-    return back
 
 #手动刷新对话
 def clear_id(id,nick) -> str:
     data = log_in()
     dt = time.time()
     t = int(dt)
     data[f'{id}']['time'] = t
```

### Comparing `nonebot-plugin-hx-yinying-1.0.9/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.0.9
+Version: 1.1.0
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.9 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.0 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.0.9/setup.py` & `nonebot-plugin-hx-yinying-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.0.9",
+    version="1.1.0",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
-    install_requires=['nonebot2>=2.2.1', 'ujson>=5.9.0', 'httpx>=0.27.0', 'nonebot-adapter-onebot>=2.4.3', 'nonebot_plugin_localstore>=0.6.0', 'pydantic>=1.10.12','requests>=2.31.0','nonebot_plugin_apscheduler>=0.4.0'],
+    install_requires=['nonebot2>=2.2.1', 'ujson>=5.9.0', 'httpx>=0.27.0', 'nonebot-adapter-onebot>=2.4.3', 'nonebot_plugin_localstore>=0.6.0', 'pydantic>=1.10.12','requests>=2.31.0','nonebot_plugin_apscheduler>=0.4.0','nonebot_plugin_htmlrender>=0.3.0','pillow>=9.3.0'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

