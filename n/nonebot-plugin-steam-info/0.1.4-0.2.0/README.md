# Comparing `tmp/nonebot_plugin_steam_info-0.1.4.tar.gz` & `tmp/nonebot_plugin_steam_info-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_steam_info-0.1.4.tar", last modified: Mon Apr 22 14:42:05 2024, max compression
+gzip compressed data, was "nonebot_plugin_steam_info-0.2.0.tar", last modified: Sat Apr 27 05:27:48 2024, max compression
```

## Comparing `nonebot_plugin_steam_info-0.1.4.tar` & `nonebot_plugin_steam_info-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1062 2024-04-22 14:41:36.218760 nonebot_plugin_steam_info-0.1.4/LICENSE
--rw-r--r--   0        0        0     2089 2024-04-22 14:41:36.218760 nonebot_plugin_steam_info-0.1.4/README.md
--rw-r--r--   0        0        0     8016 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/__init__.py
--rw-r--r--   0        0        0      152 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/config.py
--rw-r--r--   0        0        0     5091 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/data_source.py
--rw-r--r--   0        0        0    12428 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/draw.py
--rw-r--r--   0        0        0      572 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/models.py
--rw-r--r--   0        0        0      552 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/busy.png
--rw-r--r--   0        0        0     1847 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/friends_search.png
--rw-r--r--   0        0        0     7467 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/parent_status.png
--rw-r--r--   0        0        0     3409 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/unknown_avatar.jpg
--rw-r--r--   0        0        0      533 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/zzz_gaming.png
--rw-r--r--   0        0        0      536 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/zzz_online.png
--rw-r--r--   0        0        0     1209 2024-04-22 14:41:36.374761 nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/steam.py
--rw-r--r--   0        0        0      580 2024-04-22 14:42:05.319066 nonebot_plugin_steam_info-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 nonebot_plugin_steam_info-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-27 05:27:23.457559 nonebot_plugin_steam_info-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2380 2024-04-27 05:27:23.457559 nonebot_plugin_steam_info-0.2.0/README.md
+-rw-r--r--   0        0        0     9520 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/config.py
+-rw-r--r--   0        0        0     6254 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/data_source.py
+-rw-r--r--   0        0        0    12428 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/draw.py
+-rw-r--r--   0        0        0      572 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/models.py
+-rw-r--r--   0        0        0      552 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/busy.png
+-rw-r--r--   0        0        0     1847 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/friends_search.png
+-rw-r--r--   0        0        0     7467 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/parent_status.png
+-rw-r--r--   0        0        0     3409 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/unknown_avatar.jpg
+-rw-r--r--   0        0        0      533 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/zzz_gaming.png
+-rw-r--r--   0        0        0      536 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/zzz_online.png
+-rw-r--r--   0        0        0     1209 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/steam.py
+-rw-r--r--   0        0        0      580 2024-04-27 05:27:48.861264 nonebot_plugin_steam_info-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 nonebot_plugin_steam_info-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_steam_info-0.1.4/LICENSE` & `nonebot_plugin_steam_info-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/__init__.py` & `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,39 +17,42 @@
 
 import nonebot_plugin_localstore as store
 from nonebot_plugin_apscheduler import scheduler
 from nonebot_plugin_alconna import Text, Image, UniMessage, Target
 
 from .config import Config
 from .models import PlayerSummaries
-from .data_source import BindData, SteamInfoData, ParentData
 from .steam import get_steam_id, get_steam_users_info, STEAM_ID_OFFSET
+from .data_source import BindData, SteamInfoData, ParentData, DisableParentData
 from .draw import (
+    check_font,
+    image_to_bytes,
     draw_friends_status,
     simplize_steam_player_data,
-    image_to_bytes,
-    check_font,
 )
 
 
 __plugin_meta__ = PluginMetadata(
     name="Steam Info",
     description="播报绑定的 Steam 好友状态",
-    usage="steambind [Steam ID 或 Steam好友代码] -绑定 Steam\nsteaminfo -查看绑定信息\nsteamcheck -查询群友 Steam 状态\nsteamupdate [名称] [图片] -更新群聊头像和名称",
+    usage="绑定 Steam ID: steambind [Steam ID 或 Steam好友代码]\n解绑 Steam ID: steamunbind\n查看 Steam ID: steaminfo\n查看 Steam 好友状态: steamcheck\n启用 Steam 播报: steamenable\n禁用 Steam 播报: steamdisable\n更新群信息: steamupdate",
     type="application",
     homepage="https://github.com/zhaomaoniu/nonebot-plugin-steam-info",
     config=Config,
     supported_adapters=inherit_supported_adapters("nonebot_plugin_alconna"),
 )
 
 
 bind = on_command("steambind", aliases={"绑定steam"}, priority=10)
+unbind = on_command("steamunbind", aliases={"解绑steam"}, priority=10)
 info = on_command("steaminfo", aliases={"steam信息"}, priority=10)
 check = on_command("steamcheck", aliases={"查看steam", "查steam"}, priority=10)
-update_parent_info = on_command("steamupdate", priority=10)
+enable = on_command("steamenable", aliases={"启用steam"}, priority=10)
+disable = on_command("steamdisable", aliases={"禁用steam"}, priority=10)
+update_parent_info = on_command("steamupdate", aliases={"更新群信息"}, priority=10)
 
 
 if hasattr(nonebot, "get_plugin_config"):
     config = nonebot.get_plugin_config(Config)
 else:
     from nonebot import get_driver
 
@@ -57,19 +60,23 @@
 
 
 bind_data_path = store.get_data_file("nonebot_plugin_steam_info", "bind_data.json")
 steam_info_data_path = store.get_data_file(
     "nonebot_plugin_steam_info", "steam_info.json"
 )
 parent_data_path = store.get_data_file("nonebot_plugin_steam_info", "parent_data.json")
+disable_parent_data_path = store.get_data_file(
+    "nonebot_plugin_steam_info", "disable_parent_data.json"
+)
 avatar_path = store.get_cache_dir("nonebot_plugin_steam_info")
 
 bind_data = BindData(bind_data_path)
 steam_info_data = SteamInfoData(steam_info_data_path)
 parent_data = ParentData(parent_data_path)
+disable_parent_data = DisableParentData(disable_parent_data_path)
 
 try:
     check_font()
 except FileNotFoundError as e:
     logger.error(
         f"{e}, nonebot_plugin_steam_info 无法使用，请参照 `https://github.com/zhaomaoniu/nonebot-plugin-steam-info` 配置字体文件"
     )
@@ -99,14 +106,17 @@
                     raise ValueError(f"无法获取图片数据: {resp.status}")
                 return await resp.read()
 
     raise ValueError("无法获取图片数据")
 
 
 async def broadcast_steam_info(parent_id: str, steam_info: PlayerSummaries):
+    if disable_parent_data.is_disabled(parent_id):
+        return None
+
     bot = nonebot.get_bot()
 
     msg = steam_info_data.compare(parent_id, steam_info["response"])
 
     if msg == []:
         return None
 
@@ -177,14 +187,28 @@
     else:
         bind_data.add(parent_id, {"user_id": event.get_user_id(), "steam_id": steam_id})
         bind_data.save()
 
         await bind.finish(f"已绑定你的 Steam ID 为 {steam_id}")
 
 
+@unbind.handle()
+async def unbind_handle(event: Event, target: Target = Depends(get_target)):
+    parent_id = target.parent_id or target.id
+    user_id = event.get_user_id()
+
+    if bind_data.get(parent_id, user_id) is not None:
+        bind_data.remove(parent_id, user_id)
+        bind_data.save()
+
+        await unbind.finish("已解绑 Steam ID")
+    else:
+        await unbind.finish("未绑定 Steam ID")
+
+
 @info.handle()
 async def info_handle(event: Event, target: Target = Depends(get_target)):
     parent_id = target.parent_id or target.id
 
     if user_data := bind_data.get(parent_id, event.get_user_id()):
         steam_id = user_data["steam_id"]
         steam_friend_code = str(int(steam_id) - STEAM_ID_OFFSET)
@@ -243,7 +267,27 @@
             info["name"] = seg.text
 
     if "avatar" not in info or "name" not in info:
         await update_parent_info.finish("文本中应包含图片和文字")
 
     parent_data.update(target.parent_id or target.id, info["avatar"], info["name"])
     await update_parent_info.finish("更新成功")
+
+
+@enable.handle()
+async def enable_handle(target: Target = Depends(get_target)):
+    parent_id = target.parent_id or target.id
+
+    disable_parent_data.remove(parent_id)
+    disable_parent_data.save()
+
+    await enable.finish("已启用 Steam 播报")
+
+
+@disable.handle()
+async def disable_handle(target: Target = Depends(get_target)):
+    parent_id = target.parent_id or target.id
+
+    disable_parent_data.add(parent_id)
+    disable_parent_data.save()
+
+    await disable.finish("已禁用 Steam 播报")
```

### Comparing `nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/data_source.py` & `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/data_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,22 @@
             json.dump(self.content, f, indent=4)
 
     def add(self, parent_id: str, content: Dict[str, str]) -> None:
         if parent_id not in self.content:
             self.content[parent_id] = [content]
         else:
             self.content[parent_id].append(content)
+    
+    def remove(self, parent_id: str, user_id: str) -> None:
+        if parent_id not in self.content:
+            return
+        for data in self.content[parent_id]:
+            if data["user_id"] == user_id:
+                self.content[parent_id].remove(data)
+                break
 
     def update(self, parent_id: str, content: Dict[str, str]) -> None:
         self.content[parent_id] = content
 
     def get(self, parent_id: str, user_id: str) -> Optional[Dict[str, str]]:
         if parent_id not in self.content:
             return None
@@ -134,7 +142,37 @@
         if parent_id not in self.content:
             return (
                 Image.open(Path(__file__).parent / "res/unknown_avatar.jpg"),
                 parent_id,
             )
         avatar_path = self._save_path.parent / f"{parent_id}.png"
         return Image.open(avatar_path), self.content[parent_id]
+
+
+class DisableParentData:
+    """储存禁用 Steam 通知的 parent"""
+
+    def __init__(self, save_path: Path) -> None:
+        self.content: List[str] = []
+        self._save_path = save_path
+
+        if save_path.exists():
+            self.content = json.loads(save_path.read_text("utf-8"))
+        else:
+            self.save()
+
+    def save(self) -> None:
+        with open(self._save_path, "w", encoding="utf-8") as f:
+            json.dump(self.content, f, indent=4)
+
+    def add(self, parent_id: str) -> None:
+        if parent_id not in self.content:
+            self.content.append(parent_id)
+            self.save()
+
+    def remove(self, parent_id: str) -> None:
+        if parent_id in self.content:
+            self.content.remove(parent_id)
+            self.save()
+
+    def is_disabled(self, parent_id: str) -> bool:
+        return parent_id in self.content
```

### Comparing `nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/draw.py` & `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/models.py` & `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/busy.png` & `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/busy.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/friends_search.png` & `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/friends_search.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/parent_status.png` & `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/parent_status.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/unknown_avatar.jpg` & `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/unknown_avatar.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/zzz_gaming.png` & `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/zzz_gaming.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/res/zzz_online.png` & `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/zzz_online.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.4/nonebot_plugin_steam_info/steam.py` & `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.4/pyproject.toml` & `nonebot_plugin_steam_info-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-steam-info"
-version = "0.1.4"
+version = "0.2.0"
 description = "Default template for PDM package"
 authors = [
     { name = "zhaomaoniu", email = "2667292003@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.0",
     "nonebot-plugin-alconna>=0.37.0",
```

### Comparing `nonebot_plugin_steam_info-0.1.4/PKG-INFO` & `nonebot_plugin_steam_info-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,30 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-steam-info
-Version: 0.1.4
-Summary: Default template for PDM package
-Author-Email: zhaomaoniu <2667292003@qq.com>
-License: MIT
-Requires-Python: >=3.8
-Requires-Dist: nonebot2>=2.2.0
-Requires-Dist: nonebot-plugin-alconna>=0.37.0
-Requires-Dist: aiohttp>=3.9.3
-Requires-Dist: Pillow>=10.2.0
-Requires-Dist: nonebot-plugin-apscheduler>=0.4.0
-Requires-Dist: nonebot-plugin-localstore>=0.6.0
-Description-Content-Type: text/markdown
-
 # Nonebot-Plugin-Steam-Info
 ✨ Steam 好友状态播报 NoneBot 插件 ✨
 
 ## 功能
 - [x] 绑定 Steam ID
 - [x] 群友状态变更播报
 - [x] 主动查询群友状态
 
 ## 预览
 仿照了 Steam 好友列表的样式
 
 ![image](./preview.png)
 
 ## 使用
-steambind [Steam ID 或 Steam好友代码] -绑定 Steam   
-steaminfo -查看绑定信息   
-steamcheck -查询群友 Steam 状态   
-steamupdate [名称] [图片] -更新群聊头像和名称
+| 命令 | 别名 |  说明 |
+| --- | --- | --- |
+| steambind [Steam ID 或 Steam好友代码] | 绑定steam | 绑定 Steam |
+| steamunbind | 解绑steam | 解绑 Steam |
+| steaminfo | steam信息 | 查看绑定信息 |
+| steamcheck | 查看steam, 查steam | 查询群友 Steam 状态 |
+| steamupdate [名称] [图片] | 更新群信息 | 更新群聊头像和名称 |
+| steamenable | 启用steam | 启用群友状态播报 |
+| steamdisable | 禁用steam | 禁用群友状态播报 |
 
 > 记得加上你配置的命令头哦
 
 ## 安装方法
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
```

