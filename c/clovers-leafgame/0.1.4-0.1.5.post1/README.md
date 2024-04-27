# Comparing `tmp/clovers_leafgame-0.1.4.tar.gz` & `tmp/clovers_leafgame-0.1.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_leafgame-0.1.4.tar", max compression
+gzip compressed data, was "clovers_leafgame-0.1.5.post1.tar", max compression
```

## Comparing `clovers_leafgame-0.1.4.tar` & `clovers_leafgame-0.1.5.post1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      300 2024-04-15 02:23:00.888180 clovers_leafgame-0.1.4/clovers_leafgame/__init__.py
--rw-r--r--   0        0        0      682 2024-04-16 00:16:47.844659 clovers_leafgame-0.1.4/clovers_leafgame/config.py
--rw-r--r--   0        0        0     4000 2024-04-16 13:40:14.090678 clovers_leafgame-0.1.4/clovers_leafgame/core/clovers.py
--rw-r--r--   0        0        0     5568 2024-04-16 13:05:38.537666 clovers_leafgame-0.1.4/clovers_leafgame/core/data.py
--rw-r--r--   0        0        0     1617 2024-04-15 02:23:00.889680 clovers_leafgame-0.1.4/clovers_leafgame/item.py
--rw-r--r--   0        0        0     1151 2024-04-16 00:26:16.638079 clovers_leafgame-0.1.4/clovers_leafgame/main.py
--rw-r--r--   0        0        0     6480 2024-04-16 12:19:33.503496 clovers_leafgame-0.1.4/clovers_leafgame/manager.py
--rw-r--r--   0        0        0    14551 2024-04-23 13:53:09.577894 clovers_leafgame-0.1.4/clovers_leafgame/modules/account/__init__.py
--rw-r--r--   0        0        0      347 2024-04-16 00:17:06.391821 clovers_leafgame-0.1.4/clovers_leafgame/modules/account/config.py
--rw-r--r--   0        0        0    44539 2024-04-17 09:36:06.166199 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/__init__.py
--rw-r--r--   0        0        0      153 2024-04-15 07:55:35.192417 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/config.py
--rw-r--r--   0        0        0     8755 2024-04-23 13:54:15.236319 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/core.py
--rw-r--r--   0        0        0    10104 2024-04-15 02:23:00.894179 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/fortress/core.py
--rw-r--r--   0        0        0    12802 2024-04-16 00:25:10.251581 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/__init__.py
--rw-r--r--   0        0        0      447 2024-04-16 00:17:40.700801 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/config.py
--rw-r--r--   0        0        0     5817 2024-02-25 09:48:38.952874 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
--rw-r--r--   0        0        0     5728 2024-02-25 09:48:38.952874 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
--rw-r--r--   0        0        0     2174 2024-02-25 09:48:38.953876 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
--rw-r--r--   0        0        0     1231 2024-02-25 09:48:38.953876 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
--rw-r--r--   0        0        0     2742 2024-02-25 09:48:38.954376 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
--rw-r--r--   0        0        0     1606 2024-02-25 09:48:38.954376 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
--rw-r--r--   0        0        0    25830 2024-02-25 09:48:38.954877 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
--rw-r--r--   0        0        0     5180 2024-02-25 09:48:38.955377 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
--rw-r--r--   0        0        0     1072 2024-02-25 09:48:38.955878 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
--rw-r--r--   0        0        0     2294 2024-02-25 09:48:38.955878 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
--rw-r--r--   0        0        0     7488 2024-04-13 05:59:32.008464 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/horse.py
--rw-r--r--   0        0        0      933 2024-04-17 03:48:34.370378 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/start.py
--rw-r--r--   0        0        0      754 2024-03-28 05:01:34.333218 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/tools.py
--rw-r--r--   0        0        0    18177 2024-04-23 13:51:57.075986 clovers_leafgame-0.1.4/clovers_leafgame/modules/market/__init__.py
--rw-r--r--   0        0        0      457 2024-04-16 09:18:01.778879 clovers_leafgame-0.1.4/clovers_leafgame/modules/market/config.py
--rw-r--r--   0        0        0    12241 2024-04-23 13:50:43.306529 clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/__init__.py
--rw-r--r--   0        0        0      271 2024-04-16 00:19:07.783118 clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/config.py
--rw-r--r--   0        0        0     2085 2024-04-15 02:23:00.897679 clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/core.py
--rw-r--r--   0        0        0     2681 2024-03-20 09:21:29.211881 clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/output.py
--rw-r--r--   0        0        0     4516 2024-04-15 09:58:44.129537 clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/props_library.json
--rw-r--r--   0        0        0     3958 2024-04-17 03:48:34.371878 clovers_leafgame-0.1.4/clovers_leafgame/modules/ranklist/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-15 02:23:00.898679 clovers_leafgame-0.1.4/clovers_leafgame/modules/ranklist/output.py
--rw-r--r--   0        0        0     3587 2024-04-15 09:04:34.774669 clovers_leafgame-0.1.4/clovers_leafgame/modules/task/__init__.py
--rw-r--r--   0        0        0     6592 2024-04-15 11:17:50.623418 clovers_leafgame-0.1.4/clovers_leafgame/output.py
--rw-r--r--   0        0        0     1806 2024-03-15 10:15:49.531286 clovers_leafgame-0.1.4/clovers_leafgame/props_library.json
--rw-r--r--   0        0        0     1086 2024-04-15 07:17:11.700550 clovers_leafgame-0.1.4/LICENSE
--rw-r--r--   0        0        0      428 2024-04-23 13:53:54.885214 clovers_leafgame-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    18355 2024-04-15 11:14:25.199623 clovers_leafgame-0.1.4/README.md
--rw-r--r--   0        0        0    18184 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      300 2024-04-26 12:07:06.142903 clovers_leafgame-0.1.5.post1/clovers_leafgame/__init__.py
+-rw-r--r--   0        0        0      682 2024-04-26 12:07:06.142903 clovers_leafgame-0.1.5.post1/clovers_leafgame/config.py
+-rw-r--r--   0        0        0     4000 2024-04-26 12:07:06.143403 clovers_leafgame-0.1.5.post1/clovers_leafgame/core/clovers.py
+-rw-r--r--   0        0        0     5568 2024-04-26 12:07:06.143903 clovers_leafgame-0.1.5.post1/clovers_leafgame/core/data.py
+-rw-r--r--   0        0        0     1617 2024-04-26 12:07:06.143903 clovers_leafgame-0.1.5.post1/clovers_leafgame/item.py
+-rw-r--r--   0        0        0     1151 2024-04-26 12:07:06.144403 clovers_leafgame-0.1.5.post1/clovers_leafgame/main.py
+-rw-r--r--   0        0        0     6491 2024-04-26 12:44:35.983423 clovers_leafgame-0.1.5.post1/clovers_leafgame/manager.py
+-rw-r--r--   0        0        0    14551 2024-04-26 12:07:06.145403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/account/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-26 12:07:06.145403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/account/config.py
+-rw-r--r--   0        0        0    44539 2024-04-26 12:07:06.146403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-26 12:07:06.146403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/config.py
+-rw-r--r--   0        0        0     8755 2024-04-26 12:07:06.146907 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/core.py
+-rw-r--r--   0        0        0    10104 2024-04-26 12:07:06.147402 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/fortress/core.py
+-rw-r--r--   0        0        0    12802 2024-04-26 12:07:06.147902 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-26 12:07:06.148404 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/config.py
+-rw-r--r--   0        0        0     5817 2024-04-26 12:07:06.148903 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
+-rw-r--r--   0        0        0     5728 2024-04-26 12:07:06.149402 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
+-rw-r--r--   0        0        0     2174 2024-04-26 12:07:06.149402 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
+-rw-r--r--   0        0        0     1231 2024-04-26 12:07:06.149902 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
+-rw-r--r--   0        0        0     2742 2024-04-26 12:07:06.149902 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
+-rw-r--r--   0        0        0     1606 2024-04-26 12:07:06.150413 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
+-rw-r--r--   0        0        0    25830 2024-04-26 12:07:06.150903 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
+-rw-r--r--   0        0        0     5180 2024-04-26 12:07:06.150903 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
+-rw-r--r--   0        0        0     1072 2024-04-26 12:07:06.151403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
+-rw-r--r--   0        0        0     2294 2024-04-26 12:07:06.151403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
+-rw-r--r--   0        0        0     7488 2024-04-26 12:07:06.151903 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/horse.py
+-rw-r--r--   0        0        0      933 2024-04-26 12:07:06.152402 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/start.py
+-rw-r--r--   0        0        0      754 2024-04-26 12:07:06.152748 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/tools.py
+-rw-r--r--   0        0        0    18182 2024-04-26 12:54:46.015963 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/market/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-26 12:07:06.153499 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/market/config.py
+-rw-r--r--   0        0        0    12241 2024-04-26 12:07:06.154055 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-26 12:07:06.154055 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/config.py
+-rw-r--r--   0        0        0     2085 2024-04-26 12:07:06.154565 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/core.py
+-rw-r--r--   0        0        0     2681 2024-04-26 12:07:06.154565 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/output.py
+-rw-r--r--   0        0        0     4516 2024-04-26 12:07:06.155065 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/props_library.json
+-rw-r--r--   0        0        0     3958 2024-04-26 12:07:06.155565 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/ranklist/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-26 12:07:06.155565 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/ranklist/output.py
+-rw-r--r--   0        0        0     3587 2024-04-26 12:07:06.156065 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/task/__init__.py
+-rw-r--r--   0        0        0     6592 2024-04-26 12:07:06.156565 clovers_leafgame-0.1.5.post1/clovers_leafgame/output.py
+-rw-r--r--   0        0        0     1806 2024-04-26 12:07:06.156565 clovers_leafgame-0.1.5.post1/clovers_leafgame/props_library.json
+-rw-r--r--   0        0        0     1086 2024-04-26 12:07:06.141902 clovers_leafgame-0.1.5.post1/LICENSE
+-rw-r--r--   0        0        0      430 2024-04-26 12:55:58.270310 clovers_leafgame-0.1.5.post1/pyproject.toml
+-rw-r--r--   0        0        0    18355 2024-04-26 12:07:06.142403 clovers_leafgame-0.1.5.post1/README.md
+-rw-r--r--   0        0        0    18190 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.5.post1/PKG-INFO
```

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/config.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/config.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/core/clovers.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/core/clovers.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/core/data.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/core/data.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/item.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/item.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/main.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/main.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/manager.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         now = datetime.now().strftime("%Y-%m-%d %H-%M-%S")
         date_today, now_time = now.split()
         backup_today = self.backup_path / date_today
         if not backup_today.exists():
             backup_today.mkdir()
         self.save()
         file = backup_today / f"russian_data {now_time}.json"
-        file.write_text(self.data.json(indent=4))
+        file.write_text(self.data.model_dump_json(indent=4))
 
     def clean_backup(self, delta: int | float):
         folders = [f for f in self.backup_path.iterdir() if f.is_dir()]
         info = []
         for folder in folders:
             if datetime.now().timestamp() - folder.stat().st_birthtime > delta:
                 folder.unlink(True)
```

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/account/__init__.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/account/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/__init__.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/core.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/fortress/core.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/fortress/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/__init__.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/Stand.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/Stand.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/horse.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/horse.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/start.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/start.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/tools.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/tools.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/market/__init__.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/market/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,20 +92,20 @@
             n_in = int(user.bank[STD_GOLD.id] / level)
         else:
             n_in = n
         user.bank[STD_GOLD.id] -= n_out
         account.bank[GOLD.id] += n_in
         return f"你成功将{n_out}枚标准金币兑换为{n_in}枚金币"
     else:
-        n_out = n
+        n_out = -n
         if n_out > account.bank[GOLD.id]:
             n_out = account.bank[GOLD.id]
             n_in = account.bank[GOLD.id] * level
         else:
-            n_in = n * level
+            n_in = n_out * level
         user.bank[STD_GOLD.id] += n_in
         account.bank[GOLD.id] -= n_out
         return f"你成功将{n_out}枚金币兑换为{n_in}枚标准金币"
 
 
 @plugin.handle({"金币转移"}, {"user_id", "group_id"})
 async def _(event: Event):
```

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/__init__.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/core.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/output.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/props_library.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/ranklist/__init__.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/ranklist/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/ranklist/output.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/ranklist/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/modules/task/__init__.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/task/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/output.py` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/clovers_leafgame/props_library.json` & `clovers_leafgame-0.1.5.post1/clovers_leafgame/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/LICENSE` & `clovers_leafgame-0.1.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/README.md` & `clovers_leafgame-0.1.5.post1/README.md`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.4/PKG-INFO` & `clovers_leafgame-0.1.5.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: clovers-leafgame
-Version: 0.1.4
+Version: 0.1.5.post1
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0)
-Requires-Dist: clovers[linecard,tools] (>=0.1.3,<0.2.0)
+Requires-Dist: clovers[linecard,tools] (>=0.1.6,<0.2.0)
 Requires-Dist: mplfinance (>=0.12.10b0,<0.13.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 # clovers_leafgame
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.4 Summary: Author:
-KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.10,<4.0
+Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.5.post1 Summary:
+Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0) Requires-Dist: clovers
-[linecard,tools] (>=0.1.3,<0.2.0) Requires-Dist: mplfinance
+[linecard,tools] (>=0.1.6,<0.2.0) Requires-Dist: mplfinance
 (>=0.12.10b0,<0.13.0) Requires-Dist: pydantic (>=2.7.0,<3.0.0) Description-
 Content-Type: text/markdown # clovers_leafgame _â¨ æ¹èª
 [nonebot_plugin_russian](https://github.com/HibiKier/nonebot_plugin_russian)
 å [nonebot_plugin_horserace](https://github.com/shinianj/
 nonebot_plugin_horserace) çå°æ¸¸æåé â¨_
                     [python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ pip ```bash pip install clovers_leafgame ``` poetry ```bash
```

