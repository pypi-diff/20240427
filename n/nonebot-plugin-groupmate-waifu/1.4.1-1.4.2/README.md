# Comparing `tmp/nonebot_plugin_groupmate_waifu-1.4.1.tar.gz` & `tmp/nonebot_plugin_groupmate_waifu-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.4.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.4.2.tar", max compression
```

## Comparing `nonebot_plugin_groupmate_waifu-1.4.1.tar` & `nonebot_plugin_groupmate_waifu-1.4.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1086 2023-11-06 04:36:06.280670 nonebot_plugin_groupmate_waifu-1.4.1/LICENSE
--rw-r--r--   0        0        0      867 2024-04-25 17:20:52.736619 nonebot_plugin_groupmate_waifu-1.4.1/nonebot_plugin_groupmate_waifu/__init__.py
--rw-r--r--   0        0        0      409 2024-04-25 17:22:13.753605 nonebot_plugin_groupmate_waifu-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2520 2024-04-23 16:36:28.534422 nonebot_plugin_groupmate_waifu-1.4.1/README.md
--rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 nonebot_plugin_groupmate_waifu-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-27 08:15:12.420341 nonebot_plugin_groupmate_waifu-1.4.2/LICENSE
+-rw-r--r--   0        0        0      479 2024-04-27 08:27:52.520106 nonebot_plugin_groupmate_waifu-1.4.2/nonebot_plugin_groupmate_waifu/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-27 08:26:15.839081 nonebot_plugin_groupmate_waifu-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2520 2024-04-27 08:15:12.420341 nonebot_plugin_groupmate_waifu-1.4.2/README.md
+-rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 nonebot_plugin_groupmate_waifu-1.4.2/PKG-INFO
```

### Comparing `nonebot_plugin_groupmate_waifu-1.4.1/LICENSE` & `nonebot_plugin_groupmate_waifu-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.4.1/README.md` & `nonebot_plugin_groupmate_waifu-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.4.1/PKG-INFO` & `nonebot_plugin_groupmate_waifu-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-groupmate-waifu
-Version: 1.4.1
+Version: 1.4.2
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: clovers (>=0.1.7,<0.2.0)
 Requires-Dist: clovers-groupmate-waifu (>=0.1.0.post3,<0.2.0)
 Requires-Dist: nonebot-plugin-clovers[nonebot] (>=0.1.4,<0.2.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-groupmate-waifu Version: 1.4.1
+Metadata-Version: 2.1 Name: nonebot-plugin-groupmate-waifu Version: 1.4.2
 Summary: Author: KarisAya Author-email: 1048827424@qq.com Requires-Python:
->=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: clovers-groupmate-waifu (>=0.1.0.post3,<0.2.0)
-Requires-Dist: nonebot-plugin-clovers[nonebot] (>=0.1.4,<0.2.0) Description-
-Content-Type: text/markdown
+>=3.12,<4.0 Classifier: Programming Language :: Python :: 3 Requires-Dist:
+clovers (>=0.1.7,<0.2.0) Requires-Dist: clovers-groupmate-waifu
+(>=0.1.0.post3,<0.2.0) Requires-Dist: nonebot-plugin-clovers[nonebot]
+(>=0.1.4,<0.2.0) Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
     # nonebot-plugin-groupmate-waifu å¨¶ç¾¤å[python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i
                                    _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯ [æ¨è] ä½¿ç¨
 nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install
```

