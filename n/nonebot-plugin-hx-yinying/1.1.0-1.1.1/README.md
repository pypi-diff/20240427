# Comparing `tmp/nonebot-plugin-hx-yinying-1.1.0.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.1.0.tar", last modified: Sat Apr 27 15:23:38 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.1.1.tar", last modified: Sat Apr 27 19:46:47 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.1.0.tar` & `nonebot-plugin-hx-yinying-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 15:23:38.393370 nonebot-plugin-hx-yinying-1.1.0/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     5087 2024-04-27 15:23:38.393370 nonebot-plugin-hx-yinying-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4647 2024-04-25 16:11:37.000000 nonebot-plugin-hx-yinying-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 15:23:38.151995 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    56726 2024-04-27 15:15:42.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    95541 2024-04-27 15:16:04.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      396 2024-04-27 15:10:23.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/config.py
--rw-rw-rw-   0        0        0     2998 2024-04-27 15:19:03.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/report.py
-drwxrwxrwx   0        0        0        0 2024-04-27 15:23:38.393370 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     5087 2024-04-27 15:23:37.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-04-27 15:23:37.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 15:23:37.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      222 2024-04-27 15:23:37.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-27 15:23:37.000000 nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-27 15:23:38.406330 nonebot-plugin-hx-yinying-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      946 2024-04-27 15:22:00.000000 nonebot-plugin-hx-yinying-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:46:47.305420 nonebot-plugin-hx-yinying-1.1.1/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5087 2024-04-27 19:46:47.306568 nonebot-plugin-hx-yinying-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4647 2024-04-25 16:11:37.000000 nonebot-plugin-hx-yinying-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 19:46:47.084036 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    56840 2024-04-27 19:45:25.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    95553 2024-04-27 18:12:21.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      396 2024-04-27 19:46:39.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/config.py
+-rw-rw-rw-   0        0        0     4060 2024-04-27 18:25:28.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/report.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:46:47.289339 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     5087 2024-04-27 19:46:46.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-04-27 19:46:46.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 19:46:46.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2024-04-27 19:46:46.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-27 19:46:46.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-27 19:46:47.354296 nonebot-plugin-hx-yinying-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      961 2024-04-27 18:26:26.000000 nonebot-plugin-hx-yinying-1.1.1/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.1.0/LICENSE` & `nonebot-plugin-hx-yinying-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.0/PKG-INFO` & `nonebot-plugin-hx-yinying-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.1.0
+Version: 1.1.1
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
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.1 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.1.0/README.md` & `nonebot-plugin-hx-yinying-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,16 +105,17 @@
 model_handoff = on_command("切换模型", aliases={"qhmodel","切换chat模型","模型切换"},rule=Rule(chek_rule_base),  priority=0, block=True)
 easycyber_set = on_command("easycyber", aliases={"easycyber设置","hxworld"},rule=Rule(chek_rule_base),  priority=0, block=True)
 cyber_set = on_command("cyber", aliases={"cyber设置","Hxworld"},rule=Rule(chek_rule_base),  priority=0, block=True)
 admin_set = on_command("控制台操作", aliases={"管理控制台","setstart"},rule=Rule(chek_rule_admin),  priority=0, block=True)
 verision = on_command("确认版本", aliases={"旅行伙伴确认","版本确认"},rule=Rule(chek_rule_base),  priority=0, block=True)
 character = on_command("sd", aliases={"旅行伙伴加入","设定加入"},rule=Rule(chek_rule_base),  priority=0, block=True)
 chat_ne = on_command("加入订阅", aliases={"旅行伙伴觉醒","订阅加入"},rule=Rule(chek_rule_base),  priority=0, block=True)
-ces = on_command("ces", aliases={"测试"},rule=Rule(chek_rule_base), priority=0, block=True)
+ces = on_command("测试服务", aliases={"测试报错"},rule=Rule(chek_rule_base), priority=0, block=True)
 
+#自定义自己的设定
 @character.handle()
 async def character(matcher: Matcher,bot:Bot, event: MessageEvent, msg: Message = CommandArg()):
     user = get_id(event)
     nick = await get_nick(bot,event)
     config = config_in_user(user,nick)
     config_get = json_get(config,user)
     text = msg.extract_plain_text()
@@ -140,15 +141,16 @@
                     msg = f"{msg[0]}加入成功！"
             else:
                 msg = "没有获取到要加入伙伴的设定哦"
             await send_msg(matcher, event, msg)
         except Exception as e:
             msg = False
             logger.opt(colors=True).error(f"{e}")
-        
+
+#版本确认
 @verision.handle()
 async def verision_get(matcher: Matcher, event: MessageEvent):
     new_verision, time = update_hx()
     if get_groupid(event):
         id = get_groupid(event)
         e_config = config_in_group(id)
         config = json_get(e_config,id)
@@ -205,117 +207,121 @@
                 if model_in:
                     msg =f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
                 msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
             else:
                 msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
         await send_msg(matcher, event, msg)
 
+#@对话
 @msg_at.handle()
 async def at(matcher: Matcher, event: MessageEvent, bot: Bot):
     await get_answer_at(matcher, event, bot)
 
+#指令对话
 @msg_ml.handle()
 async def ml(matcher: Matcher, event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
     await get_answer_ml(matcher, event, bot ,msg)
 
+#刷新对话
 @clear.handle()
 async def clear(matcher: Matcher,bot:Bot, event: MessageEvent):
     id = get_id(event)
     nick = await get_nick(bot,event)
     if clear_id(id,nick):
         msg = "已刷新对话！"
         await send_msg(matcher, event, msg)
     else:
         msg = "刷新对话失败，请检查后台输出或联系开发者！"
         await send_msg(matcher, event, msg)
 
+#设置全局配置
 @set_global_config.got(
     "msg",
     prompt=f"发送以下选项执行相应功能\n修改 #修改全局配置项\n查看 #查看全局配置项\n追加 #向全局配置里追加配置项，通常用于插件更新后配置不存在导致的出错\n查看所有配置 #列出所有全局配置\n发送非预期命令则退出",
 )
 async def set_global(matcher: Matcher, bot:Bot, event: MessageEvent,events: Event, s: T_State):
     id = get_id(event)
     text = unescape(event.get_plaintext().strip())
     if "last" not in s:
         s["last"] = ""
     if s["last"]:
         if s["last"] == "查看":
             config = config_in_global()
-            get_config = json_get_text(config,text)
+            get_config = await json_get_text(config,text)
             if get_config == 0:
                 s["last"] = True
                 msg = f"无法查找到该配置项！，请检查其是否为正确的配置名{text}"
                 await send_msg(matcher,event,msg)
             else:
                 s["last"] = True
                 msg = f"{text}状态为:{get_config}"
                 await send_msg(matcher,event,msg)
 
         if s["last"] == "修改":
             config = config_in_global()
-            get_config = json_get_text(config,text)
-            if get_config == 0:
+            if text == "退出":
                 s["last"] = True
-                msg = "无法查找到该配置项！，请检查其是否为正确的配置名"
+                msg = "已退出"
                 await send_msg(matcher,event,msg)
             else:
-                TFkey, Wkey, Listkey = config_list(config)
+                TFkey, Wkey, Listkey = await config_list(config)
                 if text in TFkey:
                     s["last"] = "修改TF"
                     s["set"] = text
                     msg = "请发送开启或关闭【也可以是on或者off或者开和关】"
                     await send_msg_reject(matcher,event,msg)
                 elif text in Wkey:
                     s["last"] = "修改w"
                     s["set"] = text
-                    msg = "请发送id（群号或者QQ号，看你改哪个配置项）"
+                    msg = "请发送id（群号或者QQ号或者是对话限制次数，看你改哪个配置项）"
                     await send_msg_reject(matcher,event,msg)
                 elif text in Listkey:
                     s["last"] = "updata_LK"
                     s["set"] = text
                     msg = "请发送添加或删除【也可以是增加或者移除】"
                     await send_msg_reject(matcher,event,msg)
                 else:
+                    s["last"] = "修改"
+                    msg = "无法查找到该配置项！，请检查其是否为正确的配置名,请重新输入！\n如需退出请发送退出"
+                    await send_msg_reject(matcher,event,msg)
                     return
         
         if s["last"] == "修改TF":
             config = config_in_global()
             config_name = s["set"]
-            get_config = json_get_text(config,config_name)
+            get_config = await json_get_text(config,config_name)
+            logger.debug(f"{get_config}")
             key = {"on":False,"off":False,"开":True,"关":False,"开启":True,"关闭":False}
             if text in key:
                 s["last"] = True
                 text = key[f"{text}"]
                 if get_config and text:
                     msg = f"该配置项[{config_name}]已经开启了，不需要重复开启噢"
-                    await send_msg(matcher,event,msg)
                 elif not get_config and not text:
                     msg = f"该配置项[{config_name}]已经关闭了，不需要重复关闭噢"
-                    await send_msg(matcher,event,msg)
                 elif text:
                     config[f"{config_name}"] = True
                     with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
                     msg = f"{config_name}的状态已更改为{text}"
-                    await send_msg(matcher,event,msg)
                 elif not text:
                     config[f"{config_name}"] = False
                     with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
                     msg = f"{config_name}的状态已更改为{text}"
             else:
                 msg = "未知"
             await send_msg(matcher,event,msg) 
                 
      
         
         if s["last"] == "修改w":
             config = config_in_global()
             config_name = s["set"]
-            get_config = json_get_text(config,config_name)
+            get_config = await json_get_text(config,config_name)
             config[f"{config_name}"] = int(text)
             with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                 json.dump(config,file)
             msg = f"{config_name}的id已更改为{text}"
             s["last"] = True
             await send_msg(matcher,event,msg)
 
@@ -386,28 +392,31 @@
     # 退出
     if s["last"]:
         return
     else:
         msg = f"未知命令“{text}”，已退出"
         await send_msg(matcher,event,msg)
 
+#导出历史记录（私人消息转发
 @history_get.handle()
 async def history(bot: Bot, event: MessageEvent,events: Event):
     id = get_id(event)
     msg_list = await get_history(id,bot,event)
     if isinstance(events, GroupMessageEvent):
         await bot.send_group_forward_msg(group_id=event.group_id, messages=msg_list)  # type: ignore
     else:
         await bot.send_private_forward_msg(user_id=id, messages=msg_list)  # type: ignore
 
+#获取模型列表
 @model_list.handle()
 async def list(matcher: Matcher, event: MessageEvent):
         msg = "1.yinyingllm-v1\n2.yinyingllm-v2\n3.yinyingllm-v3\n4.cyberfurry-001\n5.easycyberfurry-001\n切换模型请发送:切换模型(序号)"
         await send_msg(matcher, event, msg)
 
+#模型切换方面
 @model_handoff.handle()
 async def handoff(matcher: Matcher, bot: Bot, event: MessageEvent,events: Event, msg: Message = CommandArg()):
     text = msg.extract_plain_text()
     nick = await get_nick(bot,event)
     id = get_id(event)
     model = model_got(text)
     if not text == "" or text == None:
@@ -442,14 +451,15 @@
                     clear_id(id,nick)
                     msg =f"切换成功（当前模型已切换为{model})"
                     await send_msg(matcher,event,msg)
     else:
         msg = "请注意，切换模型后不能为空哦"
         await send_msg(matcher,event,msg)
 
+#easycyber操作（投稿和载入和查看）
 @easycyber_set.got(
     "msg",
     prompt=f"发送以下选项执行相应功能\n投稿 #投稿自定义预设(不允许同名)\n载入 #载入自定义预设(不允许不存在)\n查看列表 #列出所有公开的自定义预设\n退出 #退出设置\n发送非预期命令则退出",
 )
 async def _(matcher: Matcher, bot:Bot, event: MessageEvent, s: T_State,events: Event):
     id = get_id(event)
     text = unescape(event.get_plaintext().strip())
@@ -458,14 +468,22 @@
         s["last"] = ""
     if s["last"]:
         if s["last"] == "增加":
             if text == "Hx" or text == "HX" or text == "幻歆":
                 s["last"] = True
                 msg = "easycyber预设“Hx”不能删除或修改，如要改动请改源码"
                 await send_msg(matcher,event,msg)
+            elif text == "退出":
+                s["last"] = True
+                msg = "已退出"
+                await send_msg(matcher,event,msg)
+            elif text in easycyber_in_tg(text,False) or text in easycyber_in(text,False):
+                s["last"] = "增加"
+                msg = "该预设角色名称已经存在，请不要重复使用该昵称，请重新输入，如需退出请发送退出"
+                await send_msg_reject(matcher,event,msg)
             else:
                 s["cfnickname"] = text
                 s["last"] = "cfSpecies"
                 msg = "请输入角色物种"
                 await send_msg_reject(matcher,event,msg)
         if s["last"] == "cfSpecies":
             if text == "退出":
@@ -549,51 +567,35 @@
                     easycyber_package["creator"] = int(id)
                     s["last"] = True
                     cybernick = s["cfnickname"]
                     g = json_get(config_in_global(),"admin_group")
                     u = json_get(config_in_global(),"admin_pro")
                     g_k = json_get(config_in_global(),"admin_group_switch")
                     u_k = json_get(config_in_global(),"admin_user_switch")
-                    if not g and u:
-                        logger.opt(colors=True).success(f"{g},{u}")
-                        msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
-                    elif u == None and g == None:
-                        logger.opt(colors=True).success("false")
+                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                    if not g and not u:
                         msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
-                    elif u == None and g_k:
+                    elif not u and g:
                         easycyber_in_tg(cybernick,easycyber_package)
-                        groupid = json_get(config_in_global(),"admin_group")
-                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-                    elif g == None and u_k:
+                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
+                    elif not g and u:
                         easycyber_in_tg(cybernick,easycyber_package)
-                        adminid = json_get(config_in_global(),"admin_pro")
-                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
-                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
                     elif u_k and g_k:
                         easycyber_in_tg(cybernick,easycyber_package)
-                        groupid = json_get(config_in_global(),"admin_group")
-                        adminid = json_get(config_in_global(),"admin_pro")
-                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
-                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-                    elif g_k:
+                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
+                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
+                    elif u_k:
                         easycyber_in_tg(cybernick,easycyber_package)
                         adminid = json_get(config_in_global(),"admin_pro")
-                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
+                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
                     else:
                         easycyber_in_tg(cybernick,easycyber_package)
-                        groupid = json_get(config_in_global(),"admin_group")
-                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
                     await send_msg(matcher,event,msg)
 
 
         if s["last"] == "载入":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
@@ -672,14 +674,15 @@
     # 退出
     if s["last"]:
         return
     else:
         msg = f"未知命令“{text}”，已退出"
         await send_msg(matcher,event,msg)
 
+#cyber操作（投稿和载入和查看）
 @cyber_set.got(
     "msg",
     prompt=f"发送以下选项执行相应功能\n投稿 #投稿自定义预设(不允许同名)\n载入 #载入自定义预设(不允许不存在)\n查看列表 #列出所有公开的自定义预设\n退出 #退出设置\n发送非预期命令则退出",
 )
 async def _(matcher: Matcher, bot:Bot, event: MessageEvent, s: T_State,events: Event):
     id = get_id(event)
     text = unescape(event.get_plaintext().strip())
@@ -688,16 +691,20 @@
         s["last"] = ""
     if s["last"]:
         if s["last"] == "增加":
             if text == "Hx" or text == "HX" or text == "幻歆":
                 s["last"] = True
                 msg = "cyber预设“Hx”不能删除或修改，如要改动请改源码"
                 await send_msg(matcher,event,msg)
+            elif text in cyber_in_tg(text,False) or text in cyber_in(text,False):
+                s["last"] = True
+                msg = "该预设角色名称已经存在，请不要重复使用该昵称."
+                await send_msg(matcher,event,msg)
             else:
-                s["cynickname"] = text
+                s["name"] = text
                 s["last"] = "system"
                 msg = "该角色的systempromote是？"
                 await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "system":
             if text == "退出":
                 s["last"] = True
@@ -717,62 +724,47 @@
             else:
                 key = {"是":True,"否":False,"公开":True,"不公开":False}
                 if not text in key:
                     s["last"] = "public"
                     msg = "非正确格式！请重新输入，如需退出请发送：退出"
                     await send_msg_reject(matcher,event,msg)
                 else:
-                    name = s["cfnickname"]
+                    name = s["name"]
                     systempromote = s["systempromote"]
                     easycyber_package["system"] = s["systempromote"]
                     easycyber_package["public"] = key[f"{text}"]
                     easycyber_package["creator"] = int(id)
                     s["last"] = True
                     g = json_get(config_in_global(),"admin_group")
                     u = json_get(config_in_global(),"admin_pro")
                     g_k = json_get(config_in_global(),"admin_group_switch")
                     u_k = json_get(config_in_global(),"admin_user_switch")
-                    if not g and u:
+                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
+                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                    if not g and not u:
                         logger.opt(colors=True).success(f"{g},{u}")
                         msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
-                    elif u == None and g == None:
-                        logger.opt(colors=True).success("false")
-                        msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
-                    elif u == None and g_k:
+                    elif not u and g:
                         cyber_in_tg(name,easycyber_package)
-                        groupid = json_get(config_in_global(),"admin_group")
-                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
-                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-                    elif g == None and u_k:
+                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
+                    elif not g and u:
                         cyber_in_tg(name,easycyber_package)
-                        adminid = json_get(config_in_global(),"admin_pro")
-                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
-                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
-                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
                     elif u_k and g_k:
                         cyber_in_tg(name,easycyber_package)
-                        groupid = json_get(config_in_global(),"admin_group")
-                        adminid = json_get(config_in_global(),"admin_pro")
-                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
-                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
-                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-                    elif g_k:
+                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
+                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
+                    elif u_k:
                         cyber_in_tg(name,easycyber_package)
-                        adminid = json_get(config_in_global(),"admin_pro")
-                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
-                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
+                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
                     else:
                         cyber_in_tg(name,easycyber_package)
-                        groupid = json_get(config_in_global(),"admin_group")
-                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
-                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
                     await send_msg(matcher,event,msg)
+
         if s["last"] == "载入":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
             else:
                 s["last"] = True
@@ -847,78 +839,131 @@
     # 退出
     if s["last"]:
         return
     else:
         msg = f"未知命令“{text}”，已退出"
         await send_msg(matcher,event,msg)
 
+#所有投稿管理处理
 @admin_set.got(
     "msg",
-    prompt=f"发送以下选项执行相应功能\n通过 #通过投稿的自定义预设(不允许同名)\n拒绝 #拒绝投稿的自定义预设(不允许同名)\n查看 #查看投稿预设详情(不允许不存在)\n查看投稿列表 #列出所有投稿的自定义预设\n添加admin #添加bot管理者\n退出 #退出\n仅支持bot管理员使用！\n发送非预期命令则退出",
+    prompt=f"发送以下选项执行相应功能\n通过 #通过投稿的预设(不允许同名)\n拒绝 #拒绝投稿的自定义预设(不允许同名)\n查看 #查看投稿预设详情(不允许不存在)\n查看投稿列表 #列出所有投稿的自定义预设\n添加admin #添加bot管理者\n退出 #退出\n仅支持bot管理员使用！\n发送非预期命令则退出",
 )
 async def _(matcher: Matcher, bot:Bot, event: MessageEvent, s: T_State):
     id = get_id(event)
     text = unescape(event.get_plaintext().strip())
     place_user = place(id)
     if place_user >= 9:
         if "last" not in s:
             s["last"] = ""
         if s["last"]:
-            if s["last"] == "通过1":
+            if s["last"] == "通过":
+                msg = "请输入要通过的预设名称，如果不知道建议先get下列表"
+                if text == "easycyber":
+                    s["last"] == "easyber"
+                    await send_msg_reject(matcher,event,msg)
+                elif text == "cyber":
+                    s["last"] == "cyber"
+                    await send_msg_reject(matcher,event,msg)
+
+            if s["last"] == "easyber":
                 json_1 = easycyber_in_tg(False,False)
                 json_data = json_get(json_1,text)
                 json_data["tg_admin"] = id
                 user = json_data["creator"]
                 in_ok = easycyber_in(text,json_data)
                 end_json = json_1.pop(f"{text}")
                 with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
                     json.dump(json_1,file)
                     s["last"] = True
-                    msg = f"已通过投稿用户为{user}关于角色{text}的投稿"
+                    msg = f"[easycyber]已通过投稿用户为{user}关于角色{text}的投稿"
+                await send_msg(matcher,event,msg)
+
+            if s["last"] == "cyber":
+                json_1 = cyber_in_tg(False,False)
+                json_data = json_get(json_1,text)
+                json_data["tg_admin"] = id
+                user = json_data["creator"]
+                in_ok = cyber_in(text,json_data)
+                end_json = json_1.pop(f"{text}")
+                with open(f'{log_dir}/file/cyber_tg.json','w',encoding='utf-8') as file:
+                    json.dump(json_1,file)
+                    s["last"] = True
+                    msg = f"[cyber]已通过投稿用户为{user}关于角色{text}的投稿"
                 await send_msg(matcher,event,msg)
 
             if s["last"] == "拒绝":
+                msg = "请输入要拒绝的预设名称，如果不知道建议先get下列表"
+                if text == "easycyber":
+                    s["last"] == "badeasyber"
+                    await send_msg_reject(matcher,event,msg)
+                elif text == "cyber":
+                    s["last"] == "badcyber"
+                    await send_msg_reject(matcher,event,msg)
+            
+            if s["last"] == "badeasyber":
                 s["last"] = True
                 json_1 = easycyber_in_tg(False,False)
                 json_data = json_get(json_1,text)
                 user = json_data["creator"]
                 end_json = json_1.pop(f"{text}")
                 with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
                     json.dump(json_1,file)
                     msg = f"已拒绝投稿用户为{user}关于角色{text}的投稿"
                 await send_msg(matcher,event,msg)
 
+            if s["last"] == "badcyber":
+                s["last"] = True
+                json_1 = cyber_in_tg(False,False)
+                json_data = json_get(json_1,text)
+                user = json_data["creator"]
+                end_json = json_1.pop(f"{text}")
+                with open(f'{log_dir}/file/cyber_tg.json','w',encoding='utf-8') as file:
+                    json.dump(json_1,file)
+                    msg = f"已拒绝投稿用户为{user}关于角色{text}的投稿"
+                await send_msg(matcher,event,msg)
+
         if text == "通过":
-            s["last"] = "通过1"
-            msg = "请输入要加入角色昵称"
+            s["last"] = "通过"
+            msg = "请输入要通过的预设类型\n例如：cyber或者easycyber"
             await send_msg_reject(matcher,event,msg)
 
+
         if text == "查看投稿列表":
             s["last"] = True
             list_in = easycyber_in_tg(False,False)
             msg_list = []
             for key in list_in:
                 msg_list.append(format(key))
-            await send_msg(matcher,event,f"{msg_list}")
+            msg = f"[easycyber]投稿角色列表：\n"
+            msg += "\n".join(msg_list)
+            list_in = cyber_in_tg(False,False)
+            msg_list = []
+            for key in list_in:
+                msg_list.append(format(key))
+            msg += f"\n\n[cyber]投稿角色列表：\n"
+            msg += "\n".join(msg_list)
+            await send_msg(matcher,event,f"{msg}")
 
         if text == "拒绝":
             s["last"] = "拒绝"
-            msg = "请输入要离开角色昵称"
+            msg = "请输入要的预设类型\n例如：cyber或者easycyber"
             await send_msg_reject(matcher,event,msg)
 
         if s["last"]:
             return
         else:
             msg = f"未知命令“{text}”，已退出"
             await send_msg(matcher,event,msg)
 
     else:
         msg = f"你的权限为{place_user},权限不足，无法操作"
         await send_msg(matcher, event, msg)
 
+#订阅系统
 @chat_ne.got(
     "msg",
     prompt=f"发送以下选项执行相应功能\n加入 #银影将会主动来找你聊天》？\n退出 #呜呜呜，真的要赶银影走吗\n查看加入列表 #字如其意(仅限管理员使用)\n发送非预期命令则退出",
 )
 async def _(matcher: Matcher,event: MessageEvent, s: T_State):
     id = get_id(event)
     text = unescape(event.get_plaintext().strip())
@@ -1007,11 +1052,12 @@
     # 退出
     if s["last"]:
         return
     else:
         msg = f"未知命令“{text}”，已退出"
         await send_msg(matcher,event,msg)
 
+#测试函数
 @ces.handle()
-async def _(event: MessageEvent,msg: Message = CommandArg()):
+async def _(event: MessageEvent):
     id = get_id(event)
     await get_id()
```

### Comparing `nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 def json_get(json,key) -> str:
     try:
         back = json[f"{key}"]
     except Exception as e:
         back = False
     return back
 
-def json_get_text(json,key) -> str:
+async def json_get_text(json,key) -> str:
     try:
         back = json[f"{key}"]
     except Exception as e:
         back = 0
     return back
 
 def json_get_time(json,key) -> str:
@@ -858,15 +858,15 @@
                 id_package['last_chattime'] = t
                 json_data[f"{id}"] = id_package
                 json.dump(json_data,file)
                 back = json_data
     return back
 
 #获取配置内键值并列表化
-def config_list(config):
+async def config_list(config):
     try:
         tf_key = []
         w_key = []
         list_key = []
         if config:
             for key in config:
                 get_config = json_get(config,format(key))
```

### Comparing `nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying/report.py` & `nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/report.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,51 @@
 from io import BytesIO
-import os
+import traceback,requests,zipfile,sys,os
 from PIL import Image,ImageFilter
 from .chat import(
     file_get,
     path_in,
     create_dir_usr,
 )
 from nonebot import get_plugin_config
 from nonebot_plugin_htmlrender import template_to_pic
-from pathlib import Path
 from loguru import logger
-import traceback
-import sys
+from tqdm import tqdm
 from nonebot.message import run_postprocessor
 from nonebot.adapters.onebot.v11 import (
    Bot,  MessageEvent ,MessageSegment
 )
 from .config import Config
+file = path_in()
+def get_file():
+    url = "https://skin.huanxinbot.com/api/lzy.php?url=https://wwp.lanzoup.com/iGH5K1wrn1wh&type=down"
+    file_get = requests.get(url=url,stream=True)
+    total = int(file_get.headers.get('Content-Length',0))
+    with open(f"{file}/error.zip","wb") as f,tqdm(desc="error.zip",total=total,unit="iB",unit_scale=True,unit_divisor=1024,) as bar: 
+        for data in file_get.iter_content(chunk_size=1024): 
+            size = f.write(data)
+            bar.update(len(data))
+    if os.path.exists(f"{file}/error.zip"):
+        logger.success("[Hx]尝试下载补全文件成功")
+        with zipfile.ZipFile(f"{file}/error.zip", 'r') as zip_ref:
+            zip_ref.extractall(f"{file}/file/error_report")
+            logger.success("[Hx]尝试补全成功")
+            logger.success("已加载错误报告模块")
+        os.remove(f"{file}/error.zip")
+    else:
+        logger.error("尝试下载失败！")
+
+if os.path.exists(f"{file}/file/error_report/hx_error.html"):
+    logger.success("已加载错误报告模块")
+else:
+    logger.error("未找到错误报告模块的文件，尝试下载。。。")
+    get_file()
 
 ##由星佑的oops修改而来
-file = path_in()
-image_dir = str(Path(__file__).parent / "error_report")
+image_dir = str(f"{file}/error_report")
 hx_config = get_plugin_config(Config)
 
 #背景图片尝试模糊处理（下一步更新）
 async def pictures_bj(file, radius)-> BytesIO:
     if not file:
         return False
     else:
@@ -57,15 +78,15 @@
         error = traceback.format_exception(exc_type, exc_value, exc_traceback)[-1]
         error_values = error.split(":",1)[-1]
         data = data.replace('\n','<br>')
     else:
         error_values=err_values
         newline_char = '<br>'
         data = f'{newline_char.join(err_values.args)}'
-    template_path = str(Path(__file__).parent / "error_report") #同文件夹下面的
+    template_path = str(f"{file}/error_report")
     htmlimage = await template_to_pic(
                 template_path=template_path,
                 template_name="hx_error.html",
                 templates={
                     "verision":hx_config.hx_version,
                     "error":error_values,
                     "data": data,
@@ -75,9 +96,8 @@
 @run_postprocessor
 async def post_run(bot: Bot, event: MessageEvent, e: Exception) -> None:
     img = await crash_oops(e)
     try:
         id = event.group_id
         await bot.call_api("send_group_msg",group_id=id,message=MessageSegment.image(img))
     except:
-        raise BotRunTimeError("遇到未知错误,请自行扒拉日志!")
-    logger.info(f"[Hx]:报错处理：{e}")
+        raise BotRunTimeError("遇到未知错误,请自行扒拉日志!")
```

### Comparing `nonebot-plugin-hx-yinying-1.1.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.1.0
+Version: 1.1.1
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
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.1 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.1.0/setup.py` & `nonebot-plugin-hx-yinying-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.1.0",
+    version="1.1.1",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
-    install_requires=['nonebot2>=2.2.1', 'ujson>=5.9.0', 'httpx>=0.27.0', 'nonebot-adapter-onebot>=2.4.3', 'nonebot_plugin_localstore>=0.6.0', 'pydantic>=1.10.12','requests>=2.31.0','nonebot_plugin_apscheduler>=0.4.0','nonebot_plugin_htmlrender>=0.3.0','pillow>=9.3.0'],
+    install_requires=['nonebot2>=2.2.1', 'ujson>=5.9.0', 'httpx>=0.27.0', 'nonebot-adapter-onebot>=2.4.3', 'nonebot_plugin_localstore>=0.6.0', 'pydantic>=1.10.12','requests>=2.31.0','nonebot_plugin_apscheduler>=0.4.0','nonebot_plugin_htmlrender>=0.3.0','pillow>=9.3.0','tqdm>=4.65.0'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

