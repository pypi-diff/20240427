# Comparing `tmp/alicebot_plugin_template-0.1.0.3.tar.gz` & `tmp/alicebot_plugin_template-0.1.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "alicebot_plugin_template-0.1.10.tar", last modified: Sat Apr 27 13:29:20 2024, max compression
```

## Comparing `alicebot_plugin_template-0.1.0.3.tar` & `alicebot_plugin_template-0.1.10.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0    78991 2020-02-02 00:00:00.000000 alicebot_plugin_template-0.1.0.3/pdm.lock
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 alicebot_plugin_template-0.1.0.3/alicebot_plugin_template/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 alicebot_plugin_template-0.1.0.3/alicebot_plugin_template/config.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 alicebot_plugin_template-0.1.0.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 alicebot_plugin_template-0.1.0.3/LICENSE
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 alicebot_plugin_template-0.1.0.3/README.md
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 alicebot_plugin_template-0.1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 alicebot_plugin_template-0.1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-03-18 03:29:10.213703 alicebot_plugin_template-0.1.10/LICENSE
+-rw-r--r--   0        0        0      262 2024-03-18 03:29:15.742605 alicebot_plugin_template-0.1.10/README.md
+-rw-r--r--   0        0        0      502 2024-03-26 08:10:41.477223 alicebot_plugin_template-0.1.10/alicebot_plugin_template/__init__.py
+-rw-r--r--   0        0        0      256 2024-03-20 13:07:41.146377 alicebot_plugin_template-0.1.10/alicebot_plugin_template/config.py
+-rw-r--r--   0        0        0     1592 2024-04-27 13:29:20.464513 alicebot_plugin_template-0.1.10/pyproject.toml
+-rw-r--r--   0        0        0     1180 1970-01-01 00:00:00.000000 alicebot_plugin_template-0.1.10/PKG-INFO
```

### Comparing `alicebot_plugin_template-0.1.0.3/LICENSE` & `alicebot_plugin_template-0.1.10/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 The MIT License (MIT)
-Copyright (c) 2021 st1020
+Copyright (c) 2021 AliceBotProject
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `alicebot_plugin_template-0.1.0.3/PKG-INFO` & `alicebot_plugin_template-0.1.10/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: alicebot-plugin-template
-Version: 0.1.0.3
+Version: 0.1.10
 Summary: AliceBot Plugin Template.
-Project-URL: Homepage, https://docs.alicebot.dev/
-Project-URL: Documentation, https://docs.alicebot.dev/
-Project-URL: Repository, https://github.com/AliceBotProject/alicebot-plugin-template
-Project-URL: Changelog, https://docs.alicebot.dev/changelog.html
-Author-email: st1020 <stone_1020@qq.com>
+Keywords: bot,chatbot,alicebot,tag1,tag2
+Author-Email: AliceBot <concontact@alicebot.dev>
 License: MIT
-License-File: LICENSE
-Keywords: alicebot,bot,chatbot,tag1,tag2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications :: Chat
+Project-URL: Homepage, https://docs.alicebot.dev/
+Project-URL: Documentation, https://docs.alicebot.dev/
+Project-URL: Repository, https://github.com/AliceBotProject/alicebot-plugin-template
+Project-URL: Changelog, https://docs.alicebot.dev/changelog.html
 Requires-Python: >=3.8
-Requires-Dist: alicebot==0.8.1
+Requires-Dist: alicebot>=0.10.0
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/AliceBotProject/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
 
 # AliceBot-Plugin-Template
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: alicebot-plugin-template Version: 0.1.0.3 Summary:
-AliceBot Plugin Template. Project-URL: Homepage, https://docs.alicebot.dev/
-Project-URL: Documentation, https://docs.alicebot.dev/ Project-URL: Repository,
-https://github.com/AliceBotProject/alicebot-plugin-template Project-URL:
-Changelog, https://docs.alicebot.dev/changelog.html Author-email: st1020
-qq.com> License: MIT License-File: LICENSE Keywords:
-alicebot,bot,chatbot,tag1,tag2 Classifier: Development Status :: 3 - Alpha
+Metadata-Version: 2.1 Name: alicebot-plugin-template Version: 0.1.10 Summary:
+AliceBot Plugin Template. Keywords: bot,chatbot,alicebot,tag1,tag2 Author-
+Email: AliceBot
+alicebot.dev> License: MIT Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
-Communications :: Chat Requires-Python: >=3.8 Requires-Dist: alicebot==0.8.1
-Description-Content-Type: text/markdown
+Communications :: Chat Project-URL: Homepage, https://docs.alicebot.dev/
+Project-URL: Documentation, https://docs.alicebot.dev/ Project-URL: Repository,
+https://github.com/AliceBotProject/alicebot-plugin-template Project-URL:
+Changelog, https://docs.alicebot.dev/changelog.html Requires-Python: >=3.8
+Requires-Dist: alicebot>=0.10.0 Description-Content-Type: text/markdown
           _[_l_o_g_o_]# AliceBot-Plugin-Template **AliceBot æä»¶æ¨¡æ¿**
```

