# Comparing `tmp/nonebot_plugin_game_collection-3.0.4.tar.gz` & `tmp/nonebot_plugin_game_collection-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-3.0.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_game_collection-3.0.5.tar", max compression
```

## Comparing `nonebot_plugin_game_collection-3.0.4.tar` & `nonebot_plugin_game_collection-3.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1086 2023-10-28 21:32:04.942263 nonebot_plugin_game_collection-3.0.4/LICENSE
--rw-r--r--   0        0        0      854 2024-04-25 17:17:19.355663 nonebot_plugin_game_collection-3.0.4/nonebot_plugin_game_collection/__init__.py
--rw-r--r--   0        0        0      394 2024-04-25 17:18:24.127869 nonebot_plugin_game_collection-3.0.4/pyproject.toml
--rw-r--r--   0        0        0     2984 2024-04-15 12:09:00.697493 nonebot_plugin_game_collection-3.0.4/README.md
--rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 nonebot_plugin_game_collection-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-27 08:33:06.936238 nonebot_plugin_game_collection-3.0.5/LICENSE
+-rw-r--r--   0        0        0      468 2024-04-27 08:37:28.520047 nonebot_plugin_game_collection-3.0.5/nonebot_plugin_game_collection/__init__.py
+-rw-r--r--   0        0        0      420 2024-04-27 08:36:54.711331 nonebot_plugin_game_collection-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2984 2024-04-27 08:33:06.936738 nonebot_plugin_game_collection-3.0.5/README.md
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 nonebot_plugin_game_collection-3.0.5/PKG-INFO
```

### Comparing `nonebot_plugin_game_collection-3.0.4/LICENSE` & `nonebot_plugin_game_collection-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-3.0.4/README.md` & `nonebot_plugin_game_collection-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-3.0.4/PKG-INFO` & `nonebot_plugin_game_collection-3.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-game-collection
-Version: 3.0.4
+Version: 3.0.5
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: clovers-leafgame (>=0.1.4,<0.2.0)
+Requires-Dist: clovers (>=0.1.7,<0.2.0)
+Requires-Dist: clovers-leafgame (>=0.1.5.post1,<0.2.0)
 Requires-Dist: nonebot-plugin-clovers[nonebot] (>=0.1.4,<0.2.0)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-game-collection Version: 3.0.4
+Metadata-Version: 2.1 Name: nonebot-plugin-game-collection Version: 3.0.5
 Summary: Author: KarisAya Author-email: 1048827424@qq.com Requires-Python:
->=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: clovers-leafgame (>=0.1.4,<0.2.0) Requires-Dist:
-nonebot-plugin-clovers[nonebot] (>=0.1.4,<0.2.0) Description-Content-Type:
-text/markdown
+>=3.12,<4.0 Classifier: Programming Language :: Python :: 3 Requires-Dist:
+clovers (>=0.1.7,<0.2.0) Requires-Dist: clovers-leafgame (>=0.1.5.post1,<0.2.0)
+Requires-Dist: nonebot-plugin-clovers[nonebot] (>=0.1.4,<0.2.0) Description-
+Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
 # nonebot-plugin-game-collection _â¨ æ¹èª [nonebot_plugin_russian](https://
   github.com/HibiKier/nonebot_plugin_russian) å [nonebot_plugin_horserace]
 (https://github.com/shinianj/nonebot_plugin_horserace) çå°æ¸¸æåé â¨_
                     [python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯ [æ¨è] ä½¿ç¨
```

