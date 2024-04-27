# Comparing `tmp/clovers_leafgame-0.1.5.post1.tar.gz` & `tmp/clovers_leafgame-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_leafgame-0.1.5.post1.tar", max compression
+gzip compressed data, was "clovers_leafgame-0.1.6.tar", max compression
```

## Comparing `clovers_leafgame-0.1.5.post1.tar` & `clovers_leafgame-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      300 2024-04-26 12:07:06.142903 clovers_leafgame-0.1.5.post1/clovers_leafgame/__init__.py
--rw-r--r--   0        0        0      682 2024-04-26 12:07:06.142903 clovers_leafgame-0.1.5.post1/clovers_leafgame/config.py
--rw-r--r--   0        0        0     4000 2024-04-26 12:07:06.143403 clovers_leafgame-0.1.5.post1/clovers_leafgame/core/clovers.py
--rw-r--r--   0        0        0     5568 2024-04-26 12:07:06.143903 clovers_leafgame-0.1.5.post1/clovers_leafgame/core/data.py
--rw-r--r--   0        0        0     1617 2024-04-26 12:07:06.143903 clovers_leafgame-0.1.5.post1/clovers_leafgame/item.py
--rw-r--r--   0        0        0     1151 2024-04-26 12:07:06.144403 clovers_leafgame-0.1.5.post1/clovers_leafgame/main.py
--rw-r--r--   0        0        0     6491 2024-04-26 12:44:35.983423 clovers_leafgame-0.1.5.post1/clovers_leafgame/manager.py
--rw-r--r--   0        0        0    14551 2024-04-26 12:07:06.145403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/account/__init__.py
--rw-r--r--   0        0        0      347 2024-04-26 12:07:06.145403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/account/config.py
--rw-r--r--   0        0        0    44539 2024-04-26 12:07:06.146403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/__init__.py
--rw-r--r--   0        0        0      153 2024-04-26 12:07:06.146403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/config.py
--rw-r--r--   0        0        0     8755 2024-04-26 12:07:06.146907 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/core.py
--rw-r--r--   0        0        0    10104 2024-04-26 12:07:06.147402 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/fortress/core.py
--rw-r--r--   0        0        0    12802 2024-04-26 12:07:06.147902 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/__init__.py
--rw-r--r--   0        0        0      447 2024-04-26 12:07:06.148404 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/config.py
--rw-r--r--   0        0        0     5817 2024-04-26 12:07:06.148903 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
--rw-r--r--   0        0        0     5728 2024-04-26 12:07:06.149402 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
--rw-r--r--   0        0        0     2174 2024-04-26 12:07:06.149402 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
--rw-r--r--   0        0        0     1231 2024-04-26 12:07:06.149902 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
--rw-r--r--   0        0        0     2742 2024-04-26 12:07:06.149902 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
--rw-r--r--   0        0        0     1606 2024-04-26 12:07:06.150413 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
--rw-r--r--   0        0        0    25830 2024-04-26 12:07:06.150903 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
--rw-r--r--   0        0        0     5180 2024-04-26 12:07:06.150903 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
--rw-r--r--   0        0        0     1072 2024-04-26 12:07:06.151403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
--rw-r--r--   0        0        0     2294 2024-04-26 12:07:06.151403 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
--rw-r--r--   0        0        0     7488 2024-04-26 12:07:06.151903 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/horse.py
--rw-r--r--   0        0        0      933 2024-04-26 12:07:06.152402 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/start.py
--rw-r--r--   0        0        0      754 2024-04-26 12:07:06.152748 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/tools.py
--rw-r--r--   0        0        0    18182 2024-04-26 12:54:46.015963 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/market/__init__.py
--rw-r--r--   0        0        0      457 2024-04-26 12:07:06.153499 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/market/config.py
--rw-r--r--   0        0        0    12241 2024-04-26 12:07:06.154055 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/__init__.py
--rw-r--r--   0        0        0      271 2024-04-26 12:07:06.154055 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/config.py
--rw-r--r--   0        0        0     2085 2024-04-26 12:07:06.154565 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/core.py
--rw-r--r--   0        0        0     2681 2024-04-26 12:07:06.154565 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/output.py
--rw-r--r--   0        0        0     4516 2024-04-26 12:07:06.155065 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/props_library.json
--rw-r--r--   0        0        0     3958 2024-04-26 12:07:06.155565 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/ranklist/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-26 12:07:06.155565 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/ranklist/output.py
--rw-r--r--   0        0        0     3587 2024-04-26 12:07:06.156065 clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/task/__init__.py
--rw-r--r--   0        0        0     6592 2024-04-26 12:07:06.156565 clovers_leafgame-0.1.5.post1/clovers_leafgame/output.py
--rw-r--r--   0        0        0     1806 2024-04-26 12:07:06.156565 clovers_leafgame-0.1.5.post1/clovers_leafgame/props_library.json
--rw-r--r--   0        0        0     1086 2024-04-26 12:07:06.141902 clovers_leafgame-0.1.5.post1/LICENSE
--rw-r--r--   0        0        0      430 2024-04-26 12:55:58.270310 clovers_leafgame-0.1.5.post1/pyproject.toml
--rw-r--r--   0        0        0    18355 2024-04-26 12:07:06.142403 clovers_leafgame-0.1.5.post1/README.md
--rw-r--r--   0        0        0    18190 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.5.post1/PKG-INFO
+-rw-r--r--   0        0        0      300 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.6/clovers_leafgame/__init__.py
+-rw-r--r--   0        0        0      682 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.6/clovers_leafgame/config.py
+-rw-r--r--   0        0        0     4000 2024-04-27 08:49:20.730733 clovers_leafgame-0.1.6/clovers_leafgame/core/clovers.py
+-rw-r--r--   0        0        0     5568 2024-04-27 09:13:40.955639 clovers_leafgame-0.1.6/clovers_leafgame/core/data.py
+-rw-r--r--   0        0        0     1617 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.6/clovers_leafgame/item.py
+-rw-r--r--   0        0        0     1151 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.6/clovers_leafgame/main.py
+-rw-r--r--   0        0        0     6491 2024-04-27 08:49:20.732220 clovers_leafgame-0.1.6/clovers_leafgame/manager.py
+-rw-r--r--   0        0        0    14551 2024-04-27 08:49:20.732603 clovers_leafgame-0.1.6/clovers_leafgame/modules/account/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-27 08:49:20.733113 clovers_leafgame-0.1.6/clovers_leafgame/modules/account/config.py
+-rw-r--r--   0        0        0    44539 2024-04-27 08:49:20.733802 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-27 08:49:20.733802 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/config.py
+-rw-r--r--   0        0        0     8755 2024-04-27 08:49:20.734312 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/core.py
+-rw-r--r--   0        0        0    10104 2024-04-27 08:49:20.734812 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/fortress/core.py
+-rw-r--r--   0        0        0    12802 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/config.py
+-rw-r--r--   0        0        0     5817 2024-04-27 08:49:20.735812 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
+-rw-r--r--   0        0        0     5728 2024-04-27 08:49:20.736312 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
+-rw-r--r--   0        0        0     2174 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
+-rw-r--r--   0        0        0     1231 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
+-rw-r--r--   0        0        0     2742 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
+-rw-r--r--   0        0        0     1606 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
+-rw-r--r--   0        0        0    25830 2024-04-27 08:49:20.737811 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
+-rw-r--r--   0        0        0     5180 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
+-rw-r--r--   0        0        0     1072 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
+-rw-r--r--   0        0        0     2294 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
+-rw-r--r--   0        0        0     7488 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/horse.py
+-rw-r--r--   0        0        0      933 2024-04-27 08:49:20.739312 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/start.py
+-rw-r--r--   0        0        0      754 2024-04-27 08:49:20.739812 clovers_leafgame-0.1.6/clovers_leafgame/modules/game/tools.py
+-rw-r--r--   0        0        0    18182 2024-04-27 08:49:20.740312 clovers_leafgame-0.1.6/clovers_leafgame/modules/market/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-27 08:49:20.740820 clovers_leafgame-0.1.6/clovers_leafgame/modules/market/config.py
+-rw-r--r--   0        0        0    12241 2024-04-27 08:49:20.740820 clovers_leafgame-0.1.6/clovers_leafgame/modules/prop/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-27 08:49:20.741311 clovers_leafgame-0.1.6/clovers_leafgame/modules/prop/config.py
+-rw-r--r--   0        0        0     2085 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.6/clovers_leafgame/modules/prop/core.py
+-rw-r--r--   0        0        0     2681 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.6/clovers_leafgame/modules/prop/output.py
+-rw-r--r--   0        0        0     4516 2024-04-27 08:49:20.742312 clovers_leafgame-0.1.6/clovers_leafgame/modules/prop/props_library.json
+-rw-r--r--   0        0        0     3958 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.6/clovers_leafgame/modules/ranklist/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.6/clovers_leafgame/modules/ranklist/output.py
+-rw-r--r--   0        0        0     3587 2024-04-27 09:15:30.718836 clovers_leafgame-0.1.6/clovers_leafgame/modules/task/__init__.py
+-rw-r--r--   0        0        0     6592 2024-04-27 08:49:20.743811 clovers_leafgame-0.1.6/clovers_leafgame/output.py
+-rw-r--r--   0        0        0     1806 2024-04-27 09:12:59.164148 clovers_leafgame-0.1.6/clovers_leafgame/props_library.json
+-rw-r--r--   0        0        0     1086 2024-04-27 08:49:20.729233 clovers_leafgame-0.1.6/LICENSE
+-rw-r--r--   0        0        0      428 2024-04-27 08:50:29.743590 clovers_leafgame-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    18953 2024-04-27 09:09:36.331086 clovers_leafgame-0.1.6/README.md
+-rw-r--r--   0        0        0    18662 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.6/PKG-INFO
```

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/config.py` & `clovers_leafgame-0.1.6/clovers_leafgame/config.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/core/clovers.py` & `clovers_leafgame-0.1.6/clovers_leafgame/core/clovers.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/core/data.py` & `clovers_leafgame-0.1.6/clovers_leafgame/core/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
         0:无(空气)
         1:群内
         2:全局
     """
     flow: int
     """
     道具时效
-        0:永久道具
-        1:时效道具
+        0:时效道具
+        1:永久道具
     """
     number: int
     """道具编号"""
     color: str = "black"
     intro: str = ""
     tip: str = ""
```

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/item.py` & `clovers_leafgame-0.1.6/clovers_leafgame/item.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/main.py` & `clovers_leafgame-0.1.6/clovers_leafgame/main.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/manager.py` & `clovers_leafgame-0.1.6/clovers_leafgame/manager.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/account/__init__.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/account/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/__init__.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/core.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/fortress/core.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/fortress/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/__init__.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/Stand.json` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/Stand.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/horse.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/horse.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/horse_race/start.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/horse_race/start.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/game/tools.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/game/tools.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/market/__init__.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/market/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/__init__.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/prop/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/core.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/prop/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/output.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/prop/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/prop/props_library.json` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/prop/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/ranklist/__init__.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/ranklist/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/ranklist/output.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/ranklist/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/modules/task/__init__.py` & `clovers_leafgame-0.1.6/clovers_leafgame/modules/task/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,21 +66,21 @@
 
 @plugin.handle({"刷新每日"}, {"permission"})
 @Check().superuser().check
 @scheduler.scheduled_job("cron", hour=0, misfire_grace_time=120)
 async def _():
     revolution_today = datetime.today().weekday() in {4, 5, 6}
     for user in manager.data.user_dict.values():
-        bank = {k: (v - 1) if prop.flow == 1 else v for k, v in user.bank.items() if (prop := manager.props_library.get(k))}
+        bank = {k: (v - 1) if prop.flow == 0 else v for k, v in user.bank.items() if (prop := manager.props_library.get(k))}
         user.bank = Counter(bank)
     for account in manager.data.account_dict.values():
         # 周末刷新重置签到
         account.extra["revolution"] = revolution_today
         # 群内道具有效期 - 1天
-        bank = {k: (v - 1) if prop.flow == 1 else v for k, v in account.bank.items() if (prop := manager.props_library.get(k))}
+        bank = {k: (v - 1) if prop.flow == 0 else v for k, v in account.bank.items() if (prop := manager.props_library.get(k))}
         account.bank = Counter(bank)
     verification()
     print("每日签到已刷新")
 
 
 # 数据备份
 @plugin.handle({"数据备份"}, {"permission"})
```

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/output.py` & `clovers_leafgame-0.1.6/clovers_leafgame/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/clovers_leafgame/props_library.json` & `clovers_leafgame-0.1.6/clovers_leafgame/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/LICENSE` & `clovers_leafgame-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.5.post1/README.md` & `clovers_leafgame-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,32 @@
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
+<div align="center">
 
-# clovers_leafgame
+# clovers-leafgame
 
 _✨ 改自 [nonebot_plugin_russian](https://github.com/HibiKier/nonebot_plugin_russian) 和 [nonebot_plugin_horserace](https://github.com/shinianj/nonebot_plugin_horserace) 的小游戏合集 ✨_
-
-<div align="center">
 <img src="https://img.shields.io/badge/python-3.12+-blue.svg" alt="python">
 <a href="./LICENSE">
-  <img src="https://img.shields.io/github/license/KarisAya/clovers_leafgame.svg" alt="license">
+<img src="https://img.shields.io/github/license/KarisAya/clovers_leafgame.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/clovers_leafgame">
-  <img src="https://img.shields.io/pypi/v/clovers_leafgame.svg" alt="pypi">
+<img src="https://img.shields.io/pypi/v/clovers_leafgame.svg" alt="pypi">
 </a>
 <a href="https://pypi.python.org/pypi/clovers_leafgame">
-  <img src="https://img.shields.io/pypi/dm/clovers_leafgame" alt="pypi download">
+<img src="https://img.shields.io/pypi/dm/clovers_leafgame" alt="pypi download">
 </a>
 
 </div>
 
 ## 💿 安装
 
-<details open>
-
-<summary>pip</summary>
-
 ```bash
 pip install clovers_leafgame
 ```
 
-</details>
-
-<details>
-
-<summary>poetry</summary>
-
-```bash
-poetry add clovers_leafgame
-```
-
-</details>
-
 ## ⚙️ 配置
 
 <details>
 
 <summary>在 clovers 配置文件内按需添加下面的配置项</summary>
 
 ```toml
@@ -104,23 +87,20 @@
 
 **默认资料卡背景**
 
 首次运行本插件之后，会出现 `/data/LeafGames/BG_image/` (或者你指定的) 这个路径。
 
 你需要往这个文件夹下添加一个 `default.png` 的图片，所有人的默认资料卡背景图片就是这张图了。
 
-如果不配置的话，就是纯色（~~高性能模式~~）。
+如果不配置的话，就是纯色 ~~高性能模式~~
 
 改图片的时候不用关 bot 也会生效
 
 ## 🎉 使用
 
-游戏可以使用道具作为赌注！
-注：同一时间群内只能有一场对决
-
 <details>
   
 <summary>管理员指令</summary>
 
 `获取 【道具名】 【数量】`
 
 获取相应数量的道具
@@ -407,14 +387,18 @@
 
 </details>
 
 <details>
 
 <summary>开始游戏</summary>
 
+游戏可以使用道具作为赌注！
+
+注：同一时间群内只能有一场对决
+
 所有游戏都可以通过下方的指令发起
 
 `发起游戏指令 【下注道具】 【下注数量】 【其它参数】@someone`
 
 发起游戏指令的所有参数都可忽略
 
 `下注道具` 默认为金币
@@ -572,16 +556,14 @@
 
 `双倍下注`
 
 抽一张牌并停牌，赌注翻倍。
 
 **规则**
 
-赌注上限为单次 5 倍赌注上限
-
 通过 21 点 来对其他人对战，手牌点数大的获胜。
 
 游戏中点数超过 21 会直接失败。
 
 </details>
 
 <details>
@@ -596,16 +578,14 @@
 
 **进行（私聊 bot）**
 
 `装弹` `开枪` `闪避` `闪枪` `预判开枪`
 
 **规则**
 
-赌注上限为 5 倍赌注上限
-
 双方私聊 bot 本轮的行动
 
 双方初始 1 发子弹，装弹上限为 6 发子弹（6 发可以继续装弹，但是子弹数不会再增加了）。
 
 如果双方同时`开枪`，那么子弹会发生碰撞。本轮平局
 
 `装弹` 在 **初始位置** 行动，剩余子弹数+1。会被 `开枪` `闪枪` 击杀
@@ -620,14 +600,52 @@
 
 注：预判开枪不会与闪枪发生子弹碰撞，因为预判开枪速度比闪避开枪速度快。
 
 </details>
 
 <details>
 
+<summary>恶魔轮盘</summary>
+
+**发起**
+
+`恶魔轮盘`
+
+**进行**
+
+`向对方开枪`,`向自己开枪`
+
+如果向自己开枪是空弹，那么下一回合仍是自己行动。
+
+`使用道具 道具名`
+
+开枪前可以使用道具。
+
+需要注意的是使用肾上腺素时需要同时指定对方道具
+
+例如 `使用道具 肾上腺素 手铐` 这样就会使用对方的手铐
+
+如果不指定道具或指定了对方没有的道具你会使用失败（肾上腺素仍会扣除）
+
+**规则**
+
+参考 [buckshot roulette](https://store.steampowered.com/app/2835570/_/) 规则
+
+一些修改：
+
+在子弹打光之后的下一回合会同时清空双方 buff 并切换玩家，而不是闲家回合
+
+手铐可以永动
+
+新增了道具 箱子 可以给两个人各刷一个道具
+
+</details>
+
+<details>
+
 <summary>赛马小游戏</summary>
 
 ~~抄~~改自 [nonebot_plugin_horserace](https://github.com/shinianj/nonebot_plugin_horserace)
 
 ~~发言复刻~~ 请不要在使用此插件时出现报错去找原作者（冲我来，发 issue，我已经准备好赴死了）
 
 `赛马创建`
```

#### html2text {}

```diff
@@ -1,44 +1,42 @@
-# clovers_leafgame _â¨ æ¹èª [nonebot_plugin_russian](https://github.com/
-HibiKier/nonebot_plugin_russian) å [nonebot_plugin_horserace](https://
-github.com/shinianj/nonebot_plugin_horserace) çå°æ¸¸æåé â¨_
-                    [python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
-## ð¿ å®è£ pip ```bash pip install clovers_leafgame ``` poetry ```bash
-poetry add clovers_leafgame ``` ## âï¸ éç½® å¨ clovers
-éç½®æä»¶åæéæ·»å ä¸é¢çéç½®é¡¹ ```toml [clovers_leafgame] #
-ä¸»è·¯å¾ main_path = "D:\\linbot\\LiteGames" # é»è®¤æ¾ç¤ºå­ä½ fontname =
-"simsun" # é»è®¤å¤ç¨å­ä½ fallback_fonts = [ "Arial", "Tahoma", "Microsoft
-YaHei", "Segoe UI", "Segoe UI Emoji", "Segoe UI Symbol", "Helvetica Neue",
-"PingFang SC", "Hiragino Sans GB", "Source Han Sans SC", "Noto Sans SC", "Noto
-Sans CJK JP", "WenQuanYi Micro Hei", "Apple Color Emoji", "Noto Color Emoji",]
-["clovers_leafgame.modules.account"] # æ¯æ¥ç­¾å°çèå´ sign_gold = [ 200,
-500,] # æ è®°å­ç¬¦ä¸²ï¼ä¸è¦å¨ï¼ clovers_marking = "ï¼¬ï¼µï¼£ï¼«ï¼¹
-ï¼£ï¼¬ï¼¯ï¼¶ï¼¥ï¼²" revolution_marking = " ï¼£ï¼¡ï¼°ï¼©ï¼´ï¼¡ï¼¬ï¼©ï¼³ï¼´ "
-debug_marking = " ï¼¯ï¼¦ï¼¦ï¼©ï¼£ï¼©ï¼¡ï¼¬ " ["clovers_leafgame.modules.game"]
-# è¶æ¶æ¶é´ timeout = 60 # é»è®¤èµæ³¨ default_bet = 200
-["clovers_leafgame.modules.game.horse_race"] # ç©å®¶äººæ°èå´
-range_of_player_numbers = [ 2, 8,] # è·éé¿åº¦ setting_track_length = 30 #
-éæºä½ç½®äºä»¶ï¼è½å¤éæºå°çè·éèå´ random_move_range = [ 0,
-0.8,] # æ¯åååºç¡ç§»å¨èå´ base_move_range = [ 1, 3,] # äºä»¶æ¦ç
-event_randvalue = 450 ["clovers_leafgame.modules.market"] #
+  # clovers-leafgame _â¨ æ¹èª [nonebot_plugin_russian](https://github.com/
+   HibiKier/nonebot_plugin_russian) å [nonebot_plugin_horserace](https://
+ github.com/shinianj/nonebot_plugin_horserace) çå°æ¸¸æåé â¨_[python]
+                        _[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
+## ð¿ å®è£ ```bash pip install clovers_leafgame ``` ## âï¸ éç½® å¨
+clovers éç½®æä»¶åæéæ·»å ä¸é¢çéç½®é¡¹ ```toml
+[clovers_leafgame] # ä¸»è·¯å¾ main_path = "D:\\linbot\\LiteGames" #
+é»è®¤æ¾ç¤ºå­ä½ fontname = "simsun" # é»è®¤å¤ç¨å­ä½ fallback_fonts =
+[ "Arial", "Tahoma", "Microsoft YaHei", "Segoe UI", "Segoe UI Emoji", "Segoe UI
+Symbol", "Helvetica Neue", "PingFang SC", "Hiragino Sans GB", "Source Han Sans
+SC", "Noto Sans SC", "Noto Sans CJK JP", "WenQuanYi Micro Hei", "Apple Color
+Emoji", "Noto Color Emoji",] ["clovers_leafgame.modules.account"] #
+æ¯æ¥ç­¾å°çèå´ sign_gold = [ 200, 500,] # æ è®°å­ç¬¦ä¸²ï¼ä¸è¦å¨ï¼
+clovers_marking = "ï¼¬ï¼µï¼£ï¼«ï¼¹ ï¼£ï¼¬ï¼¯ï¼¶ï¼¥ï¼²" revolution_marking = "
+ï¼£ï¼¡ï¼°ï¼©ï¼´ï¼¡ï¼¬ï¼©ï¼³ï¼´ " debug_marking = " ï¼¯ï¼¦ï¼¦ï¼©ï¼£ï¼©ï¼¡ï¼¬ "
+["clovers_leafgame.modules.game"] # è¶æ¶æ¶é´ timeout = 60 # é»è®¤èµæ³¨
+default_bet = 200 ["clovers_leafgame.modules.game.horse_race"] #
+ç©å®¶äººæ°èå´ range_of_player_numbers = [ 2, 8,] # è·éé¿åº¦
+setting_track_length = 30 # éæºä½ç½®äºä»¶ï¼è½å¤éæºå°çè·éèå´
+random_move_range = [ 0, 0.8,] # æ¯åååºç¡ç§»å¨èå´ base_move_range =
+[ 1, 3,] # äºä»¶æ¦ç event_randvalue = 450
+["clovers_leafgame.modules.market"] #
 éç½®å·å´æ¶é´ï¼è®¾ç½®ä¸º0ç¦ç¨åèµ·éç½® revolt_cd = 28800 #
 éç½®çåºå°¼ç³»æ° revolt_gini = 0.68 # éç½®ç­¾å°çèå´ revolt_gold =
 [ 1000, 2000,] # æ³¨åå¬å¸éå¸æ° company_public_gold = 20000
 ["clovers_leafgame.modules.prop"] # æ½å¡æééå¸ gacha_gold = 50 #
 ç¤¼åéå¸èå´ packet_gold = [ 200, 2000,] # å¹¸è¿ç¡¬å¸èµæ³¨èå´
 luckey_coin = [ 2000, 100000,] ``` **é»è®¤èµæå¡èæ¯**
 é¦æ¬¡è¿è¡æ¬æä»¶ä¹åï¼ä¼åºç° `/data/LeafGames/BG_image/`
 (æèä½ æå®ç) è¿ä¸ªè·¯å¾ã ä½ éè¦å¾è¿ä¸ªæä»¶å¤¹ä¸æ·»å ä¸ä¸ª
 `default.png`
 çå¾çï¼ææäººçé»è®¤èµæå¡èæ¯å¾çå°±æ¯è¿å¼ å¾äºã
-å¦æä¸éç½®çè¯ï¼å°±æ¯çº¯è²ï¼~~é«æ§è½æ¨¡å¼~~ï¼ã
-æ¹å¾ççæ¶åä¸ç¨å³ bot ä¹ä¼çæ ## ð ä½¿ç¨
-æ¸¸æå¯ä»¥ä½¿ç¨éå·ä½ä¸ºèµæ³¨ï¼
-æ³¨ï¼åä¸æ¶é´ç¾¤ååªè½æä¸åºå¯¹å³ ç®¡çåæä»¤ `è·å
-ãéå·åã ãæ°éã` è·åç¸åºæ°éçéå·
+å¦æä¸éç½®çè¯ï¼å°±æ¯çº¯è² ~~é«æ§è½æ¨¡å¼~~
+æ¹å¾ççæ¶åä¸ç¨å³ bot ä¹ä¼çæ ## ð ä½¿ç¨ ç®¡çåæä»¤
+`è·å ãéå·åã ãæ°éã` è·åç¸åºæ°éçéå·
 `å»ç»èµäº§@someone` æ¥å° at çç¾¤åçå¨é¨èµäº§ã
 ç±äºæ¸¸æå¸åºæºå¶è¿äºç®åå¯¼è´è¿è¥æ¶é´é¿äºä»¥åä¼åºç°éå¸æ°éç¦»è°±çç©å®¶
 å¦æéå¸ææéè¿äºç¦»è°±ï¼å¯ä»¥ä½¿ç¨`å»ç»èµäº§`æ¥å°ã
 `ç»§æ¿ç¾¤è´¦æ· ãè¢«ç»§æ¿ç¾¤ã -> ãç»§æ¿ç¾¤ã`
 æç¾¤è¢«ç»§æ¿ç¾¤å¨é¨çèµäº§è½¬ç§»å°ç»§æ¿ç¾¤ `æ°æ®éªè¯`
 ä¿®å¤å­æ¡£æ°æ® `ä¿å­æ°æ®` å¨å³ bot
 åéè¦ä¿å­æ°æ®ï¼ä¸ç¶ä¼åæ¡£å°ä¸æ¬¡èªå¨ä¿å­çæ¶é´ç¹
@@ -125,18 +123,20 @@
 åï¼ææ¸ç©ºã_ æè¡ç³»ç» `ãéå·åææåæ é¢ãæè¡`
 æ¥çæ¬ç¾¤ç©å®¶å¨æ¬ç¾¤ææéå·çæ°éï¼ææåæ°æ®ï¼æè¡ å¦
 `éå¸æè¡` æ¥çæ¬ç¾¤éå¸æ°æè¡
 `ãéå·åææåæ é¢ãæ»æè¡`
 æ¥çææç©å®¶çå¨é¨è´¦æ·çéå·æ»æ°éï¼ææåæ°æ®ï¼æè¡
 å¦ææå®çéå·åæ¯ç¾¤åéå·ï¼é£ä¹è®¡ç®æ»æ°æ¶ä¼è®¡ç®éå·æå¨ç¾¤æ±ç
 **æåæ é¢** `èåº`,`è¿è`,`è´¥åº`,`è¿è´¥`,`è·¯ç¯æä»¶`
-å¼å§æ¸¸æ æææ¸¸æé½å¯ä»¥éè¿ä¸æ¹çæä»¤åèµ·
-`åèµ·æ¸¸ææä»¤ ãä¸æ³¨éå·ã ãä¸æ³¨æ°éã
-ãå¶å®åæ°ã@someone` åèµ·æ¸¸ææä»¤çææåæ°é½å¯å¿½ç¥
-`ä¸æ³¨éå·` é»è®¤ä¸ºéå¸ `ä¸æ³¨æ°é` é»è®¤ä¸º 0 `å¶å®åæ°`
+å¼å§æ¸¸æ æ¸¸æå¯ä»¥ä½¿ç¨éå·ä½ä¸ºèµæ³¨ï¼
+æ³¨ï¼åä¸æ¶é´ç¾¤ååªè½æä¸åºå¯¹å³
+æææ¸¸æé½å¯ä»¥éè¿ä¸æ¹çæä»¤åèµ· `åèµ·æ¸¸ææä»¤
+ãä¸æ³¨éå·ã ãä¸æ³¨æ°éã ãå¶å®åæ°ã@someone`
+åèµ·æ¸¸ææä»¤çææåæ°é½å¯å¿½ç¥ `ä¸æ³¨éå·` é»è®¤ä¸ºéå¸
+`ä¸æ³¨æ°é` é»è®¤ä¸º 0 `å¶å®åæ°`
 é»è®¤ä¸ºç©ºãå¦ææ³è¦ç»å¶å®åæ°ä¼ å¥ä¸ä¸ªå¯ä»¥è¢«æ ¼å¼åä¸ºæ°å­çå­ç¬¦ä¸²ï¼é£ä¹å¿é¡»è¦æä¸æ³¨æ°éã
 `at` æå®æ¥åææå¯¹è±¡ æ¸¸æå¯¹å±å¯ä»¥ä½¿ç¨å¦ä¸æä»¤å¤ç
 `æ¥åææ` `æç»ææ` `è®¤è¾` `è¶æ¶ç»ç®` ï¼60 ç§ï¼
 `æ¸¸æéç½®` ï¼éè¦æ¸¸æå¯¹å±è¶æ¶ï¼ **åèµ·æ¸¸ææä»¤**
 ä¿ç½æ¯è½®ç **åèµ·** `ä¿ç½æ¯è½®ç` å¶å®åæ°ä¸ºè£å¼¹æ°
 **è¿è¡** `å¼æª ãNã` **è§å** éè¿ è£å¼¹
 æ¥å¯¹å¶ä»äººåèµ·å³æï¼è½®æµå¼æªï¼ç´å°è¿æ°ä¸å¥½çäººåå»ä¸ã
@@ -167,33 +167,43 @@
 å¨å¼çåå¯ä»¥ç¡®è®¤èªå·±çæçãå¯ç§èççï¼éè¦æ·»å  bot
 å¥½åï¼ `å¼ç` **è§å** éè¿ åè±é¡º
 æ¥å¯¹å¶ä»äººå¯¹æï¼åæççå¼çï¼åæççå¼çï¼ç´å°ä¸æ¹è®¤è¾æç¹æ°å¤§çè·èã
 ç»åï¼åè±é¡º > åæ¡ > è«è¦ > åè± > é¡ºå­ > ä¸æ¡ > ä¸¤å¯¹ >
 ä¸å¯¹ > æ£ç è±è²ï¼é»æ¡ > çº¢æ¡ > æ¢è± > æ¹ç 21ç¹ **åèµ·**
 `21ç¹` å¯¹æåæ¹éè¦æ·»å  bot å¥½å **è¿è¡** `æ½ç` æ½ä¸å¼ ç
 `åç` åæ­¢æ½ç `ååä¸æ³¨` æ½ä¸å¼ çå¹¶åçï¼èµæ³¨ç¿»åã
-**è§å** èµæ³¨ä¸éä¸ºåæ¬¡ 5 åèµæ³¨ä¸é éè¿ 21 ç¹
-æ¥å¯¹å¶ä»äººå¯¹æï¼æçç¹æ°å¤§çè·èã æ¸¸æä¸­ç¹æ°è¶è¿ 21
-ä¼ç´æ¥å¤±è´¥ã è¥¿é¨å¯¹æ **åèµ·** `è¥¿é¨å¯¹æ éé¢ at`
-å¯¹æåæ¹éè¦æ·»å  bot å¥½å **è¿è¡ï¼ç§è botï¼** `è£å¼¹`
-`å¼æª` `éªé¿` `éªæª` `é¢å¤å¼æª` **è§å** èµæ³¨ä¸éä¸º 5
-åèµæ³¨ä¸é åæ¹ç§è bot æ¬è½®çè¡å¨ åæ¹åå§ 1
-åå­å¼¹ï¼è£å¼¹ä¸éä¸º 6 åå­å¼¹ï¼6
-åå¯ä»¥ç»§ç»­è£å¼¹ï¼ä½æ¯å­å¼¹æ°ä¸ä¼åå¢å äºï¼ã
+**è§å** éè¿ 21 ç¹ æ¥å¯¹å¶ä»äººå¯¹æï¼æçç¹æ°å¤§çè·èã
+æ¸¸æä¸­ç¹æ°è¶è¿ 21 ä¼ç´æ¥å¤±è´¥ã è¥¿é¨å¯¹æ **åèµ·**
+`è¥¿é¨å¯¹æ éé¢ at` å¯¹æåæ¹éè¦æ·»å  bot å¥½å **è¿è¡ï¼ç§è
+botï¼** `è£å¼¹` `å¼æª` `éªé¿` `éªæª` `é¢å¤å¼æª` **è§å**
+åæ¹ç§è bot æ¬è½®çè¡å¨ åæ¹åå§ 1 åå­å¼¹ï¼è£å¼¹ä¸éä¸º 6
+åå­å¼¹ï¼6 åå¯ä»¥ç»§ç»­è£å¼¹ï¼ä½æ¯å­å¼¹æ°ä¸ä¼åå¢å äºï¼ã
 å¦æåæ¹åæ¶`å¼æª`ï¼é£ä¹å­å¼¹ä¼åçç¢°æãæ¬è½®å¹³å±
 `è£å¼¹` å¨ **åå§ä½ç½®** è¡å¨ï¼å©ä½å­å¼¹æ°+1ãä¼è¢« `å¼æª`
 `éªæª` å»æ `éªé¿` å» **éªé¿ä½ç½®** ï¼ä¸ä¼æ¶èå­å¼¹ãä¼è¢«
 `é¢å¤å¼æª` å»æ `å¼æª` å¨ **åå§ä½ç½®** è¡å¨ï¼æå¯¹æ¹
 **åå§ä½ç½®** ï¼å©ä½å­å¼¹æ°-1 å»æ `è£å¼¹` `é¢å¤å¼æª` `éªæª`
 å» **éªé¿ä½ç½®** ï¼æå¯¹æ¹ **åå§ä½ç½®** ï¼å©ä½å­å¼¹æ°-1 å»æ
 `è£å¼¹` `å¼æª` `é¢å¤å¼æª` å¨ **åå§ä½ç½®** è¡å¨ï¼æå¯¹æ¹
 **éªé¿ä½ç½®** ï¼å©ä½å­å¼¹æ°-1 å»æ `éªé¿` `éªæª`
 æ³¨ï¼é¢å¤å¼æªä¸ä¼ä¸éªæªåçå­å¼¹ç¢°æï¼å ä¸ºé¢å¤å¼æªéåº¦æ¯éªé¿å¼æªéåº¦å¿«ã
-èµé©¬å°æ¸¸æ ~~æ~~æ¹èª [nonebot_plugin_horserace](https://github.com/
-shinianj/nonebot_plugin_horserace) ~~åè¨å¤å»~~
+æ¶é­è½®ç **åèµ·** `æ¶é­è½®ç` **è¿è¡**
+`åå¯¹æ¹å¼æª`,`åèªå·±å¼æª`
+å¦æåèªå·±å¼æªæ¯ç©ºå¼¹ï¼é£ä¹ä¸ä¸ååä»æ¯èªå·±è¡å¨ã
+`ä½¿ç¨éå· éå·å` å¼æªåå¯ä»¥ä½¿ç¨éå·ã
+éè¦æ³¨æçæ¯ä½¿ç¨è¾ä¸èºç´ æ¶éè¦åæ¶æå®å¯¹æ¹éå· ä¾å¦
+`ä½¿ç¨éå· è¾ä¸èºç´  æé` è¿æ ·å°±ä¼ä½¿ç¨å¯¹æ¹çæé
+å¦æä¸æå®éå·ææå®äºå¯¹æ¹æ²¡æçéå·ä½ ä¼ä½¿ç¨å¤±è´¥ï¼è¾ä¸èºç´ ä»ä¼æ£é¤ï¼
+**è§å** åè [buckshot roulette](https://store.steampowered.com/app/
+2835570/_/) è§å ä¸äºä¿®æ¹ï¼
+å¨å­å¼¹æåä¹åçä¸ä¸ååä¼åæ¶æ¸ç©ºåæ¹ buff
+å¹¶åæ¢ç©å®¶ï¼èä¸æ¯é²å®¶åå æéå¯ä»¥æ°¸å¨ æ°å¢äºéå·
+ç®±å­ å¯ä»¥ç»ä¸¤ä¸ªäººåå·ä¸ä¸ªéå· èµé©¬å°æ¸¸æ ~~æ~~æ¹èª
+[nonebot_plugin_horserace](https://github.com/shinianj/
+nonebot_plugin_horserace) ~~åè¨å¤å»~~
 è¯·ä¸è¦å¨ä½¿ç¨æ­¤æä»¶æ¶åºç°æ¥éå»æ¾åä½èï¼å²ææ¥ï¼å
 issueï¼æå·²ç»åå¤å¥½èµ´æ­»äºï¼ `èµé©¬åå»º`
 ç¬¬ä¸ä½ç©å®¶åèµ·æ´»å¨ `èµé©¬å å¥ ä½ çé©¬å¿åç§°`
 è±è´¹æ¥åè´¹ï¼å å¥ä½ çèµé©¬ `èµé©¬å¼å§`
 å¦ææè¶³å¤çäººå å¥äºæ¸¸æï¼é£ä¹å¯ä»¥éè¿æ¬æä»¤å¼å§æ¸¸æ
 `èµé©¬æå`
 æåæ¬ç¾¤çèµé©¬ï¼ç¨åå¯ä»¥ç¨`èµé©¬å¼å§`ç»§ç»­æ¸¸æ
```

### Comparing `clovers_leafgame-0.1.5.post1/PKG-INFO` & `clovers_leafgame-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,46 @@
 Metadata-Version: 2.1
 Name: clovers-leafgame
-Version: 0.1.5.post1
+Version: 0.1.6
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0)
-Requires-Dist: clovers[linecard,tools] (>=0.1.6,<0.2.0)
+Requires-Dist: clovers[linecard,tools] (>=0.1.7,<0.2.0)
 Requires-Dist: mplfinance (>=0.12.10b0,<0.13.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
+<div align="center">
 
-# clovers_leafgame
+# clovers-leafgame
 
 _✨ 改自 [nonebot_plugin_russian](https://github.com/HibiKier/nonebot_plugin_russian) 和 [nonebot_plugin_horserace](https://github.com/shinianj/nonebot_plugin_horserace) 的小游戏合集 ✨_
-
-<div align="center">
 <img src="https://img.shields.io/badge/python-3.12+-blue.svg" alt="python">
 <a href="./LICENSE">
-  <img src="https://img.shields.io/github/license/KarisAya/clovers_leafgame.svg" alt="license">
+<img src="https://img.shields.io/github/license/KarisAya/clovers_leafgame.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/clovers_leafgame">
-  <img src="https://img.shields.io/pypi/v/clovers_leafgame.svg" alt="pypi">
+<img src="https://img.shields.io/pypi/v/clovers_leafgame.svg" alt="pypi">
 </a>
 <a href="https://pypi.python.org/pypi/clovers_leafgame">
-  <img src="https://img.shields.io/pypi/dm/clovers_leafgame" alt="pypi download">
+<img src="https://img.shields.io/pypi/dm/clovers_leafgame" alt="pypi download">
 </a>
 
 </div>
 
 ## 💿 安装
 
-<details open>
-
-<summary>pip</summary>
-
 ```bash
 pip install clovers_leafgame
 ```
 
-</details>
-
-<details>
-
-<summary>poetry</summary>
-
-```bash
-poetry add clovers_leafgame
-```
-
-</details>
-
 ## ⚙️ 配置
 
 <details>
 
 <summary>在 clovers 配置文件内按需添加下面的配置项</summary>
 
 ```toml
@@ -120,23 +101,20 @@
 
 **默认资料卡背景**
 
 首次运行本插件之后，会出现 `/data/LeafGames/BG_image/` (或者你指定的) 这个路径。
 
 你需要往这个文件夹下添加一个 `default.png` 的图片，所有人的默认资料卡背景图片就是这张图了。
 
-如果不配置的话，就是纯色（~~高性能模式~~）。
+如果不配置的话，就是纯色 ~~高性能模式~~
 
 改图片的时候不用关 bot 也会生效
 
 ## 🎉 使用
 
-游戏可以使用道具作为赌注！
-注：同一时间群内只能有一场对决
-
 <details>
   
 <summary>管理员指令</summary>
 
 `获取 【道具名】 【数量】`
 
 获取相应数量的道具
@@ -423,14 +401,18 @@
 
 </details>
 
 <details>
 
 <summary>开始游戏</summary>
 
+游戏可以使用道具作为赌注！
+
+注：同一时间群内只能有一场对决
+
 所有游戏都可以通过下方的指令发起
 
 `发起游戏指令 【下注道具】 【下注数量】 【其它参数】@someone`
 
 发起游戏指令的所有参数都可忽略
 
 `下注道具` 默认为金币
@@ -588,16 +570,14 @@
 
 `双倍下注`
 
 抽一张牌并停牌，赌注翻倍。
 
 **规则**
 
-赌注上限为单次 5 倍赌注上限
-
 通过 21 点 来对其他人对战，手牌点数大的获胜。
 
 游戏中点数超过 21 会直接失败。
 
 </details>
 
 <details>
@@ -612,16 +592,14 @@
 
 **进行（私聊 bot）**
 
 `装弹` `开枪` `闪避` `闪枪` `预判开枪`
 
 **规则**
 
-赌注上限为 5 倍赌注上限
-
 双方私聊 bot 本轮的行动
 
 双方初始 1 发子弹，装弹上限为 6 发子弹（6 发可以继续装弹，但是子弹数不会再增加了）。
 
 如果双方同时`开枪`，那么子弹会发生碰撞。本轮平局
 
 `装弹` 在 **初始位置** 行动，剩余子弹数+1。会被 `开枪` `闪枪` 击杀
@@ -636,14 +614,52 @@
 
 注：预判开枪不会与闪枪发生子弹碰撞，因为预判开枪速度比闪避开枪速度快。
 
 </details>
 
 <details>
 
+<summary>恶魔轮盘</summary>
+
+**发起**
+
+`恶魔轮盘`
+
+**进行**
+
+`向对方开枪`,`向自己开枪`
+
+如果向自己开枪是空弹，那么下一回合仍是自己行动。
+
+`使用道具 道具名`
+
+开枪前可以使用道具。
+
+需要注意的是使用肾上腺素时需要同时指定对方道具
+
+例如 `使用道具 肾上腺素 手铐` 这样就会使用对方的手铐
+
+如果不指定道具或指定了对方没有的道具你会使用失败（肾上腺素仍会扣除）
+
+**规则**
+
+参考 [buckshot roulette](https://store.steampowered.com/app/2835570/_/) 规则
+
+一些修改：
+
+在子弹打光之后的下一回合会同时清空双方 buff 并切换玩家，而不是闲家回合
+
+手铐可以永动
+
+新增了道具 箱子 可以给两个人各刷一个道具
+
+</details>
+
+<details>
+
 <summary>赛马小游戏</summary>
 
 ~~抄~~改自 [nonebot_plugin_horserace](https://github.com/shinianj/nonebot_plugin_horserace)
 
 ~~发言复刻~~ 请不要在使用此插件时出现报错去找原作者（冲我来，发 issue，我已经准备好赴死了）
 
 `赛马创建`
```

#### html2text {}

```diff
@@ -1,52 +1,48 @@
-Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.5.post1 Summary:
-Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0) Requires-Dist: clovers
-[linecard,tools] (>=0.1.6,<0.2.0) Requires-Dist: mplfinance
-(>=0.12.10b0,<0.13.0) Requires-Dist: pydantic (>=2.7.0,<3.0.0) Description-
-Content-Type: text/markdown # clovers_leafgame _â¨ æ¹èª
-[nonebot_plugin_russian](https://github.com/HibiKier/nonebot_plugin_russian)
-å [nonebot_plugin_horserace](https://github.com/shinianj/
-nonebot_plugin_horserace) çå°æ¸¸æåé â¨_
-                    [python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
-## ð¿ å®è£ pip ```bash pip install clovers_leafgame ``` poetry ```bash
-poetry add clovers_leafgame ``` ## âï¸ éç½® å¨ clovers
-éç½®æä»¶åæéæ·»å ä¸é¢çéç½®é¡¹ ```toml [clovers_leafgame] #
-ä¸»è·¯å¾ main_path = "D:\\linbot\\LiteGames" # é»è®¤æ¾ç¤ºå­ä½ fontname =
-"simsun" # é»è®¤å¤ç¨å­ä½ fallback_fonts = [ "Arial", "Tahoma", "Microsoft
-YaHei", "Segoe UI", "Segoe UI Emoji", "Segoe UI Symbol", "Helvetica Neue",
-"PingFang SC", "Hiragino Sans GB", "Source Han Sans SC", "Noto Sans SC", "Noto
-Sans CJK JP", "WenQuanYi Micro Hei", "Apple Color Emoji", "Noto Color Emoji",]
-["clovers_leafgame.modules.account"] # æ¯æ¥ç­¾å°çèå´ sign_gold = [ 200,
-500,] # æ è®°å­ç¬¦ä¸²ï¼ä¸è¦å¨ï¼ clovers_marking = "ï¼¬ï¼µï¼£ï¼«ï¼¹
-ï¼£ï¼¬ï¼¯ï¼¶ï¼¥ï¼²" revolution_marking = " ï¼£ï¼¡ï¼°ï¼©ï¼´ï¼¡ï¼¬ï¼©ï¼³ï¼´ "
-debug_marking = " ï¼¯ï¼¦ï¼¦ï¼©ï¼£ï¼©ï¼¡ï¼¬ " ["clovers_leafgame.modules.game"]
-# è¶æ¶æ¶é´ timeout = 60 # é»è®¤èµæ³¨ default_bet = 200
-["clovers_leafgame.modules.game.horse_race"] # ç©å®¶äººæ°èå´
-range_of_player_numbers = [ 2, 8,] # è·éé¿åº¦ setting_track_length = 30 #
-éæºä½ç½®äºä»¶ï¼è½å¤éæºå°çè·éèå´ random_move_range = [ 0,
-0.8,] # æ¯åååºç¡ç§»å¨èå´ base_move_range = [ 1, 3,] # äºä»¶æ¦ç
-event_randvalue = 450 ["clovers_leafgame.modules.market"] #
+Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.6 Summary: Author:
+KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.12,<4.0
+Classifier: Programming Language :: Python :: 3 Requires-Dist: clovers-
+apscheduler (>=0.1.3,<0.2.0) Requires-Dist: clovers[linecard,tools]
+(>=0.1.7,<0.2.0) Requires-Dist: mplfinance (>=0.12.10b0,<0.13.0) Requires-Dist:
+pydantic (>=2.7.0,<3.0.0) Description-Content-Type: text/markdown
+  # clovers-leafgame _â¨ æ¹èª [nonebot_plugin_russian](https://github.com/
+   HibiKier/nonebot_plugin_russian) å [nonebot_plugin_horserace](https://
+ github.com/shinianj/nonebot_plugin_horserace) çå°æ¸¸æåé â¨_[python]
+                        _[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
+## ð¿ å®è£ ```bash pip install clovers_leafgame ``` ## âï¸ éç½® å¨
+clovers éç½®æä»¶åæéæ·»å ä¸é¢çéç½®é¡¹ ```toml
+[clovers_leafgame] # ä¸»è·¯å¾ main_path = "D:\\linbot\\LiteGames" #
+é»è®¤æ¾ç¤ºå­ä½ fontname = "simsun" # é»è®¤å¤ç¨å­ä½ fallback_fonts =
+[ "Arial", "Tahoma", "Microsoft YaHei", "Segoe UI", "Segoe UI Emoji", "Segoe UI
+Symbol", "Helvetica Neue", "PingFang SC", "Hiragino Sans GB", "Source Han Sans
+SC", "Noto Sans SC", "Noto Sans CJK JP", "WenQuanYi Micro Hei", "Apple Color
+Emoji", "Noto Color Emoji",] ["clovers_leafgame.modules.account"] #
+æ¯æ¥ç­¾å°çèå´ sign_gold = [ 200, 500,] # æ è®°å­ç¬¦ä¸²ï¼ä¸è¦å¨ï¼
+clovers_marking = "ï¼¬ï¼µï¼£ï¼«ï¼¹ ï¼£ï¼¬ï¼¯ï¼¶ï¼¥ï¼²" revolution_marking = "
+ï¼£ï¼¡ï¼°ï¼©ï¼´ï¼¡ï¼¬ï¼©ï¼³ï¼´ " debug_marking = " ï¼¯ï¼¦ï¼¦ï¼©ï¼£ï¼©ï¼¡ï¼¬ "
+["clovers_leafgame.modules.game"] # è¶æ¶æ¶é´ timeout = 60 # é»è®¤èµæ³¨
+default_bet = 200 ["clovers_leafgame.modules.game.horse_race"] #
+ç©å®¶äººæ°èå´ range_of_player_numbers = [ 2, 8,] # è·éé¿åº¦
+setting_track_length = 30 # éæºä½ç½®äºä»¶ï¼è½å¤éæºå°çè·éèå´
+random_move_range = [ 0, 0.8,] # æ¯åååºç¡ç§»å¨èå´ base_move_range =
+[ 1, 3,] # äºä»¶æ¦ç event_randvalue = 450
+["clovers_leafgame.modules.market"] #
 éç½®å·å´æ¶é´ï¼è®¾ç½®ä¸º0ç¦ç¨åèµ·éç½® revolt_cd = 28800 #
 éç½®çåºå°¼ç³»æ° revolt_gini = 0.68 # éç½®ç­¾å°çèå´ revolt_gold =
 [ 1000, 2000,] # æ³¨åå¬å¸éå¸æ° company_public_gold = 20000
 ["clovers_leafgame.modules.prop"] # æ½å¡æééå¸ gacha_gold = 50 #
 ç¤¼åéå¸èå´ packet_gold = [ 200, 2000,] # å¹¸è¿ç¡¬å¸èµæ³¨èå´
 luckey_coin = [ 2000, 100000,] ``` **é»è®¤èµæå¡èæ¯**
 é¦æ¬¡è¿è¡æ¬æä»¶ä¹åï¼ä¼åºç° `/data/LeafGames/BG_image/`
 (æèä½ æå®ç) è¿ä¸ªè·¯å¾ã ä½ éè¦å¾è¿ä¸ªæä»¶å¤¹ä¸æ·»å ä¸ä¸ª
 `default.png`
 çå¾çï¼ææäººçé»è®¤èµæå¡èæ¯å¾çå°±æ¯è¿å¼ å¾äºã
-å¦æä¸éç½®çè¯ï¼å°±æ¯çº¯è²ï¼~~é«æ§è½æ¨¡å¼~~ï¼ã
-æ¹å¾ççæ¶åä¸ç¨å³ bot ä¹ä¼çæ ## ð ä½¿ç¨
-æ¸¸æå¯ä»¥ä½¿ç¨éå·ä½ä¸ºèµæ³¨ï¼
-æ³¨ï¼åä¸æ¶é´ç¾¤ååªè½æä¸åºå¯¹å³ ç®¡çåæä»¤ `è·å
-ãéå·åã ãæ°éã` è·åç¸åºæ°éçéå·
+å¦æä¸éç½®çè¯ï¼å°±æ¯çº¯è² ~~é«æ§è½æ¨¡å¼~~
+æ¹å¾ççæ¶åä¸ç¨å³ bot ä¹ä¼çæ ## ð ä½¿ç¨ ç®¡çåæä»¤
+`è·å ãéå·åã ãæ°éã` è·åç¸åºæ°éçéå·
 `å»ç»èµäº§@someone` æ¥å° at çç¾¤åçå¨é¨èµäº§ã
 ç±äºæ¸¸æå¸åºæºå¶è¿äºç®åå¯¼è´è¿è¥æ¶é´é¿äºä»¥åä¼åºç°éå¸æ°éç¦»è°±çç©å®¶
 å¦æéå¸ææéè¿äºç¦»è°±ï¼å¯ä»¥ä½¿ç¨`å»ç»èµäº§`æ¥å°ã
 `ç»§æ¿ç¾¤è´¦æ· ãè¢«ç»§æ¿ç¾¤ã -> ãç»§æ¿ç¾¤ã`
 æç¾¤è¢«ç»§æ¿ç¾¤å¨é¨çèµäº§è½¬ç§»å°ç»§æ¿ç¾¤ `æ°æ®éªè¯`
 ä¿®å¤å­æ¡£æ°æ® `ä¿å­æ°æ®` å¨å³ bot
 åéè¦ä¿å­æ°æ®ï¼ä¸ç¶ä¼åæ¡£å°ä¸æ¬¡èªå¨ä¿å­çæ¶é´ç¹
@@ -133,18 +129,20 @@
 åï¼ææ¸ç©ºã_ æè¡ç³»ç» `ãéå·åææåæ é¢ãæè¡`
 æ¥çæ¬ç¾¤ç©å®¶å¨æ¬ç¾¤ææéå·çæ°éï¼ææåæ°æ®ï¼æè¡ å¦
 `éå¸æè¡` æ¥çæ¬ç¾¤éå¸æ°æè¡
 `ãéå·åææåæ é¢ãæ»æè¡`
 æ¥çææç©å®¶çå¨é¨è´¦æ·çéå·æ»æ°éï¼ææåæ°æ®ï¼æè¡
 å¦ææå®çéå·åæ¯ç¾¤åéå·ï¼é£ä¹è®¡ç®æ»æ°æ¶ä¼è®¡ç®éå·æå¨ç¾¤æ±ç
 **æåæ é¢** `èåº`,`è¿è`,`è´¥åº`,`è¿è´¥`,`è·¯ç¯æä»¶`
-å¼å§æ¸¸æ æææ¸¸æé½å¯ä»¥éè¿ä¸æ¹çæä»¤åèµ·
-`åèµ·æ¸¸ææä»¤ ãä¸æ³¨éå·ã ãä¸æ³¨æ°éã
-ãå¶å®åæ°ã@someone` åèµ·æ¸¸ææä»¤çææåæ°é½å¯å¿½ç¥
-`ä¸æ³¨éå·` é»è®¤ä¸ºéå¸ `ä¸æ³¨æ°é` é»è®¤ä¸º 0 `å¶å®åæ°`
+å¼å§æ¸¸æ æ¸¸æå¯ä»¥ä½¿ç¨éå·ä½ä¸ºèµæ³¨ï¼
+æ³¨ï¼åä¸æ¶é´ç¾¤ååªè½æä¸åºå¯¹å³
+æææ¸¸æé½å¯ä»¥éè¿ä¸æ¹çæä»¤åèµ· `åèµ·æ¸¸ææä»¤
+ãä¸æ³¨éå·ã ãä¸æ³¨æ°éã ãå¶å®åæ°ã@someone`
+åèµ·æ¸¸ææä»¤çææåæ°é½å¯å¿½ç¥ `ä¸æ³¨éå·` é»è®¤ä¸ºéå¸
+`ä¸æ³¨æ°é` é»è®¤ä¸º 0 `å¶å®åæ°`
 é»è®¤ä¸ºç©ºãå¦ææ³è¦ç»å¶å®åæ°ä¼ å¥ä¸ä¸ªå¯ä»¥è¢«æ ¼å¼åä¸ºæ°å­çå­ç¬¦ä¸²ï¼é£ä¹å¿é¡»è¦æä¸æ³¨æ°éã
 `at` æå®æ¥åææå¯¹è±¡ æ¸¸æå¯¹å±å¯ä»¥ä½¿ç¨å¦ä¸æä»¤å¤ç
 `æ¥åææ` `æç»ææ` `è®¤è¾` `è¶æ¶ç»ç®` ï¼60 ç§ï¼
 `æ¸¸æéç½®` ï¼éè¦æ¸¸æå¯¹å±è¶æ¶ï¼ **åèµ·æ¸¸ææä»¤**
 ä¿ç½æ¯è½®ç **åèµ·** `ä¿ç½æ¯è½®ç` å¶å®åæ°ä¸ºè£å¼¹æ°
 **è¿è¡** `å¼æª ãNã` **è§å** éè¿ è£å¼¹
 æ¥å¯¹å¶ä»äººåèµ·å³æï¼è½®æµå¼æªï¼ç´å°è¿æ°ä¸å¥½çäººåå»ä¸ã
@@ -175,33 +173,43 @@
 å¨å¼çåå¯ä»¥ç¡®è®¤èªå·±çæçãå¯ç§èççï¼éè¦æ·»å  bot
 å¥½åï¼ `å¼ç` **è§å** éè¿ åè±é¡º
 æ¥å¯¹å¶ä»äººå¯¹æï¼åæççå¼çï¼åæççå¼çï¼ç´å°ä¸æ¹è®¤è¾æç¹æ°å¤§çè·èã
 ç»åï¼åè±é¡º > åæ¡ > è«è¦ > åè± > é¡ºå­ > ä¸æ¡ > ä¸¤å¯¹ >
 ä¸å¯¹ > æ£ç è±è²ï¼é»æ¡ > çº¢æ¡ > æ¢è± > æ¹ç 21ç¹ **åèµ·**
 `21ç¹` å¯¹æåæ¹éè¦æ·»å  bot å¥½å **è¿è¡** `æ½ç` æ½ä¸å¼ ç
 `åç` åæ­¢æ½ç `ååä¸æ³¨` æ½ä¸å¼ çå¹¶åçï¼èµæ³¨ç¿»åã
-**è§å** èµæ³¨ä¸éä¸ºåæ¬¡ 5 åèµæ³¨ä¸é éè¿ 21 ç¹
-æ¥å¯¹å¶ä»äººå¯¹æï¼æçç¹æ°å¤§çè·èã æ¸¸æä¸­ç¹æ°è¶è¿ 21
-ä¼ç´æ¥å¤±è´¥ã è¥¿é¨å¯¹æ **åèµ·** `è¥¿é¨å¯¹æ éé¢ at`
-å¯¹æåæ¹éè¦æ·»å  bot å¥½å **è¿è¡ï¼ç§è botï¼** `è£å¼¹`
-`å¼æª` `éªé¿` `éªæª` `é¢å¤å¼æª` **è§å** èµæ³¨ä¸éä¸º 5
-åèµæ³¨ä¸é åæ¹ç§è bot æ¬è½®çè¡å¨ åæ¹åå§ 1
-åå­å¼¹ï¼è£å¼¹ä¸éä¸º 6 åå­å¼¹ï¼6
-åå¯ä»¥ç»§ç»­è£å¼¹ï¼ä½æ¯å­å¼¹æ°ä¸ä¼åå¢å äºï¼ã
+**è§å** éè¿ 21 ç¹ æ¥å¯¹å¶ä»äººå¯¹æï¼æçç¹æ°å¤§çè·èã
+æ¸¸æä¸­ç¹æ°è¶è¿ 21 ä¼ç´æ¥å¤±è´¥ã è¥¿é¨å¯¹æ **åèµ·**
+`è¥¿é¨å¯¹æ éé¢ at` å¯¹æåæ¹éè¦æ·»å  bot å¥½å **è¿è¡ï¼ç§è
+botï¼** `è£å¼¹` `å¼æª` `éªé¿` `éªæª` `é¢å¤å¼æª` **è§å**
+åæ¹ç§è bot æ¬è½®çè¡å¨ åæ¹åå§ 1 åå­å¼¹ï¼è£å¼¹ä¸éä¸º 6
+åå­å¼¹ï¼6 åå¯ä»¥ç»§ç»­è£å¼¹ï¼ä½æ¯å­å¼¹æ°ä¸ä¼åå¢å äºï¼ã
 å¦æåæ¹åæ¶`å¼æª`ï¼é£ä¹å­å¼¹ä¼åçç¢°æãæ¬è½®å¹³å±
 `è£å¼¹` å¨ **åå§ä½ç½®** è¡å¨ï¼å©ä½å­å¼¹æ°+1ãä¼è¢« `å¼æª`
 `éªæª` å»æ `éªé¿` å» **éªé¿ä½ç½®** ï¼ä¸ä¼æ¶èå­å¼¹ãä¼è¢«
 `é¢å¤å¼æª` å»æ `å¼æª` å¨ **åå§ä½ç½®** è¡å¨ï¼æå¯¹æ¹
 **åå§ä½ç½®** ï¼å©ä½å­å¼¹æ°-1 å»æ `è£å¼¹` `é¢å¤å¼æª` `éªæª`
 å» **éªé¿ä½ç½®** ï¼æå¯¹æ¹ **åå§ä½ç½®** ï¼å©ä½å­å¼¹æ°-1 å»æ
 `è£å¼¹` `å¼æª` `é¢å¤å¼æª` å¨ **åå§ä½ç½®** è¡å¨ï¼æå¯¹æ¹
 **éªé¿ä½ç½®** ï¼å©ä½å­å¼¹æ°-1 å»æ `éªé¿` `éªæª`
 æ³¨ï¼é¢å¤å¼æªä¸ä¼ä¸éªæªåçå­å¼¹ç¢°æï¼å ä¸ºé¢å¤å¼æªéåº¦æ¯éªé¿å¼æªéåº¦å¿«ã
-èµé©¬å°æ¸¸æ ~~æ~~æ¹èª [nonebot_plugin_horserace](https://github.com/
-shinianj/nonebot_plugin_horserace) ~~åè¨å¤å»~~
+æ¶é­è½®ç **åèµ·** `æ¶é­è½®ç` **è¿è¡**
+`åå¯¹æ¹å¼æª`,`åèªå·±å¼æª`
+å¦æåèªå·±å¼æªæ¯ç©ºå¼¹ï¼é£ä¹ä¸ä¸ååä»æ¯èªå·±è¡å¨ã
+`ä½¿ç¨éå· éå·å` å¼æªåå¯ä»¥ä½¿ç¨éå·ã
+éè¦æ³¨æçæ¯ä½¿ç¨è¾ä¸èºç´ æ¶éè¦åæ¶æå®å¯¹æ¹éå· ä¾å¦
+`ä½¿ç¨éå· è¾ä¸èºç´  æé` è¿æ ·å°±ä¼ä½¿ç¨å¯¹æ¹çæé
+å¦æä¸æå®éå·ææå®äºå¯¹æ¹æ²¡æçéå·ä½ ä¼ä½¿ç¨å¤±è´¥ï¼è¾ä¸èºç´ ä»ä¼æ£é¤ï¼
+**è§å** åè [buckshot roulette](https://store.steampowered.com/app/
+2835570/_/) è§å ä¸äºä¿®æ¹ï¼
+å¨å­å¼¹æåä¹åçä¸ä¸ååä¼åæ¶æ¸ç©ºåæ¹ buff
+å¹¶åæ¢ç©å®¶ï¼èä¸æ¯é²å®¶åå æéå¯ä»¥æ°¸å¨ æ°å¢äºéå·
+ç®±å­ å¯ä»¥ç»ä¸¤ä¸ªäººåå·ä¸ä¸ªéå· èµé©¬å°æ¸¸æ ~~æ~~æ¹èª
+[nonebot_plugin_horserace](https://github.com/shinianj/
+nonebot_plugin_horserace) ~~åè¨å¤å»~~
 è¯·ä¸è¦å¨ä½¿ç¨æ­¤æä»¶æ¶åºç°æ¥éå»æ¾åä½èï¼å²ææ¥ï¼å
 issueï¼æå·²ç»åå¤å¥½èµ´æ­»äºï¼ `èµé©¬åå»º`
 ç¬¬ä¸ä½ç©å®¶åèµ·æ´»å¨ `èµé©¬å å¥ ä½ çé©¬å¿åç§°`
 è±è´¹æ¥åè´¹ï¼å å¥ä½ çèµé©¬ `èµé©¬å¼å§`
 å¦ææè¶³å¤çäººå å¥äºæ¸¸æï¼é£ä¹å¯ä»¥éè¿æ¬æä»¤å¼å§æ¸¸æ
 `èµé©¬æå`
 æåæ¬ç¾¤çèµé©¬ï¼ç¨åå¯ä»¥ç¨`èµé©¬å¼å§`ç»§ç»­æ¸¸æ
```

