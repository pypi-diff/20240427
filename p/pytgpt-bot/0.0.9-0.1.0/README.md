# Comparing `tmp/pytgpt_bot-0.0.9.tar.gz` & `tmp/pytgpt_bot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.0.9.tar", last modified: Fri Apr 26 03:06:32 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.1.0.tar", last modified: Fri Apr 26 21:48:09 2024, max compression
```

## Comparing `pytgpt_bot-0.0.9.tar` & `pytgpt_bot-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:06:32.588867 pytgpt_bot-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 03:06:32.588867 pytgpt_bot-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:06:32.588867 pytgpt_bot-0.0.9/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    17267 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:06:32.588867 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 03:06:32.588867 pytgpt_bot-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:48:09.104422 pytgpt_bot-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 21:47:49.000000 pytgpt_bot-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 21:48:09.104422 pytgpt_bot-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-04-26 21:47:49.000000 pytgpt_bot-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:48:09.100422 pytgpt_bot-0.1.0/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 21:47:49.000000 pytgpt_bot-0.1.0/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 21:47:49.000000 pytgpt_bot-0.1.0/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-26 21:47:49.000000 pytgpt_bot-0.1.0/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-26 21:47:49.000000 pytgpt_bot-0.1.0/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-26 21:47:49.000000 pytgpt_bot-0.1.0/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19875 2024-04-26 21:47:49.000000 pytgpt_bot-0.1.0/pytgpt_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-26 21:47:49.000000 pytgpt_bot-0.1.0/pytgpt_bot/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-26 21:47:49.000000 pytgpt_bot-0.1.0/pytgpt_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:48:09.104422 pytgpt_bot-0.1.0/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 21:48:09.000000 pytgpt_bot-0.1.0/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-26 21:48:09.000000 pytgpt_bot-0.1.0/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:48:09.000000 pytgpt_bot-0.1.0/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 21:48:09.000000 pytgpt_bot-0.1.0/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-26 21:48:09.000000 pytgpt_bot-0.1.0/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 21:48:09.000000 pytgpt_bot-0.1.0/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:48:09.104422 pytgpt_bot-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-26 21:47:49.000000 pytgpt_bot-0.1.0/setup.py
```

### Comparing `pytgpt_bot-0.0.9/LICENSE` & `pytgpt_bot-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.9/PKG-INFO` & `pytgpt_bot-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.9
-Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
+Version: 0.1.0
+Summary: Telegram bot for chatting, text-to-image and text-to-voice conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/pytgpt-bot
@@ -31,18 +31,19 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytelegrambotapi==4.17.0
 Requires-Dist: python-tgpt==0.6.6
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: click==8.1.3
+Requires-Dist: SQLAlchemy==2.0.29
 
 <p align="center">
 <a href="https://github.com/Simatwa/pytgpt-bot/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=MIT&color=Blue&message=MIT&label=License"/></a>
-<a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt"/></a>
+<a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt-bot"/></a>
 <a href="https://pypi.org/project/pytgpt-bot"><img alt="PyPi" src="https://img.shields.io/pypi/v/pytgpt-bot?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
 <a href="https://pepy.tech/project/pytgpt-bot"><img src="https://static.pepy.tech/personalized-badge/pytgpt-bot?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <!--
 <a href="https://github.com/Simatwa/pytgpt-bot/releases"><img src="https://img.shields.io/github/v/release/Simatwa/pytgpt-bot?color=success&label=Release&logo=github" alt="Latest release"></img></a> 
 -->
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/pytgpt-bot"/></a>
@@ -77,17 +78,17 @@
 pip install pytgpt-bot
 ```
 
 ## Usage
 
 Before getting started, ensure you've your Telegram bot token. If that's not the case then purpose to secure one from [@BotFather](https://telegram.me/BotFather).
 
-Proceed to fill the [env](env) configuration file as per the needs and then rename it `.env` before firing up the server `python3 run.py`.
+Proceed to fill the [env](env) configuration file as per the needs and then rename it `.env` before firing up the bot `python3 run.py`.
 
-Alternatively, using CLI interface::
+Alternatively, using CLI:
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
 ### Commands
 
@@ -112,21 +113,21 @@
 
 - **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
 
 - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of them.
 
 - **/history**: Provides users with the ability to view the history of their chats with the bot. This command is useful for reviewing past interactions or finding specific information from previous conversations.
 
-- **/settings**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
+- **/check**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
 
 - **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
 
 - **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
 
-- `any other text or command>`: An alias for `/chat`, allowing users to continue with text chat.
+- `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
 
 ### Administrative Commands
 
 
 ### Administrative Commands
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.9 Summary: Telegram bot for
-text generation, text-to-image and text-to-audio conversions. Home-page: https:
-//github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.0 Summary: Telegram bot for
+chatting, text-to-image and text-to-voice conversions Home-page: https://
+github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
 pytgpt-bot/releases Project-URL: Documentation, https://github.com/Simatwa/
 pytgpt-bot/blob/main/README.md Keywords:
@@ -17,15 +17,16 @@
 Python Modules Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pytelegrambotapi==4.17.0 Requires-Dist: python-tgpt==0.6.6 Requires-Dist:
-python-dotenv==1.0.0 Requires-Dist: click==8.1.3
+python-dotenv==1.0.0 Requires-Dist: click==8.1.3 Requires-Dist:
+SQLAlchemy==2.0.29
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/
    _a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_g_p_t_-_b_o_t_]
                                   _[_w_a_k_a_t_i_m_e_]
                       ************ WWeellccoommee ttoo _pp_yy_tt_gg_pp_tt_--_bb_oo_tt ************
 This is a Telegram bot based on [python-tgpt](https://github.com/Simatwa/
 python-tgpt), a powerful tool designed to enhance your interactions with AI.
 This bot is built on the robust foundation of the `pyTelegramBotAPI` and offers
@@ -34,63 +35,63 @@
 from text, `pytgpt-bot` has got you covered. ## Prerequisites - [x]
 [Python>=3.10](https://python.org) ## Installation 1. From Source Clone repo
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
-file as per the needs and then rename it `.env` before firing up the server
-`python3 run.py`. Alternatively, using CLI interface:: `$ pytgpt-bot run ` ##
-Features ### Commands ### Usage Information This section provides detailed
-instructions on how to use the various commands available in the bot. - **/
-start**: Displays the help information, offering a comprehensive list of
-available commands and their functionalities. This command is essential for
-users to quickly understand how to interact with the bot. - **/chat**: Initiate
-a natural language conversation with the AI. This command allows users to
-engage in interactive dialogues, ask questions, or make requests. - **/image**:
-Generates images from textual descriptions using the default provider. This
-feature enables users to visualize ideas or concepts through images. - **/
-prodia**: Generates images from textual descriptions using the Prodia provider.
-This command offers a unique style or interpretation of the text descriptions
+file as per the needs and then rename it `.env` before firing up the bot
+`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features ###
+Commands ### Usage Information This section provides detailed instructions on
+how to use the various commands available in the bot. - **/start**: Displays
+the help information, offering a comprehensive list of available commands and
+their functionalities. This command is essential for users to quickly
+understand how to interact with the bot. - **/chat**: Initiate a natural
+language conversation with the AI. This command allows users to engage in
+interactive dialogues, ask questions, or make requests. - **/image**: Generates
+images from textual descriptions using the default provider. This feature
+enables users to visualize ideas or concepts through images. - **/prodia**:
+Generates images from textual descriptions using the Prodia provider. This
+command offers a unique style or interpretation of the text descriptions
 compared to the default method. - **/audio**: Converts text to speech,
 providing users with the ability to listen to descriptions, instructions, or
 any text content read out by the AI. - **/intro**: Sets a new text for the chat
 intro. This command allows users to customize the chat introductory prompt
 which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
 voice for speech synthesis. This command enables users to choose from different
 voices for the AI to use when generating audio from text. - **/provider**: Sets
 a new chat provider. This command allows users to switch between different
 providers for various functionalities, such as `phind`, `llama2`, `koboldai`
 etc. - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of
 them. - **/history**: Provides users with the ability to view the history of
 their chats with the bot. This command is useful for reviewing past
 interactions or finding specific information from previous conversations. - **/
-settings**: Offers an overview of the bot's current configuration, including
-any custom settings applied by the user. - **/reset**: Resets the chat history
-and starts a new conversation thread. This command is useful for users who wish
-to start fresh or clear their chat history for privacy reasons. - **/myid**:
+check**: Offers an overview of the bot's current configuration, including any
+custom settings applied by the user. - **/reset**: Resets the chat history and
+starts a new conversation thread. This command is useful for users who wish to
+start fresh or clear their chat history for privacy reasons. - **/myid**:
 Echoes the user's Telegram ID. This command is useful for users who need to
 know their Telegram ID for various purposes, such as setting up bot admin. -
-`any other text or command>`: An alias for `/chat`, allowing users to continue
-with text chat. ### Administrative Commands ### Administrative Commands - `/
-clear`: Clears all chats. This command is used to remove all chat data from the
-bot's database. It's a powerful command that should be used with caution, as it
-will delete all chat history. - `/total`: Shows the total number of chats
-available. This command provides an overview of the current chat data stored in
-the bot's database, helping administrators understand the volume of
-interactions the bot has had. - `/drop`: Clears the entire chat table and bot
-logs. Similar to `/clear`, this command removes all data from the chat table in
-the database. It's a more drastic measure than `/clear`, as it completely wipes
-out all chat data and current contents of log file. - `/sql`: Allows running
-SQL statements against the database. This command provides a way for
-administrators to directly interact with the bot's database using SQL queries.
-It's a powerful tool for managing and analyzing the bot's data but should be
-used with caution to avoid unintended data loss or corruption. - `/logs`:
-Checks the logs. This command is used to access the bot's logs, which can
-provide insights into the bot's activity, errors, and user interactions. It's a
-valuable tool for monitoring and troubleshooting the bot's performance. ##
-Support and Feedback If you have any questions, feedback, or suggestions for
-`pytgpt`, please feel free to reach out. Your input is valuable in helping us
-improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
-source and available under the [MIT License](LICENSE). Feel free to use,
-modify, and distribute the code as you see fit. --- Thank you for using
-`pytgpt-bot`. Enjoy your AI-powered interactions!
+`any other text`: An alias for `/chat`, allowing users to continue with
+chatting. ### Administrative Commands ### Administrative Commands - `/clear`:
+Clears all chats. This command is used to remove all chat data from the bot's
+database. It's a powerful command that should be used with caution, as it will
+delete all chat history. - `/total`: Shows the total number of chats available.
+This command provides an overview of the current chat data stored in the bot's
+database, helping administrators understand the volume of interactions the bot
+has had. - `/drop`: Clears the entire chat table and bot logs. Similar to `/
+clear`, this command removes all data from the chat table in the database. It's
+a more drastic measure than `/clear`, as it completely wipes out all chat data
+and current contents of log file. - `/sql`: Allows running SQL statements
+against the database. This command provides a way for administrators to
+directly interact with the bot's database using SQL queries. It's a powerful
+tool for managing and analyzing the bot's data but should be used with caution
+to avoid unintended data loss or corruption. - `/logs`: Checks the logs. This
+command is used to access the bot's logs, which can provide insights into the
+bot's activity, errors, and user interactions. It's a valuable tool for
+monitoring and troubleshooting the bot's performance. ## Support and Feedback
+If you have any questions, feedback, or suggestions for `pytgpt`, please feel
+free to reach out. Your input is valuable in helping us improve and expand the
+bot's capabilities. ## License `pytgpt-bot` is open-source and available under
+the [MIT License](LICENSE). Feel free to use, modify, and distribute the code
+as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy your AI-powered
+interactions!
```

### Comparing `pytgpt_bot-0.0.9/README.md` & `pytgpt_bot-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <p align="center">
 <a href="https://github.com/Simatwa/pytgpt-bot/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=MIT&color=Blue&message=MIT&label=License"/></a>
-<a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt"/></a>
+<a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt-bot"/></a>
 <a href="https://pypi.org/project/pytgpt-bot"><img alt="PyPi" src="https://img.shields.io/pypi/v/pytgpt-bot?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
 <a href="https://pepy.tech/project/pytgpt-bot"><img src="https://static.pepy.tech/personalized-badge/pytgpt-bot?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <!--
 <a href="https://github.com/Simatwa/pytgpt-bot/releases"><img src="https://img.shields.io/github/v/release/Simatwa/pytgpt-bot?color=success&label=Release&logo=github" alt="Latest release"></img></a> 
 -->
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/pytgpt-bot"/></a>
@@ -39,17 +39,17 @@
 pip install pytgpt-bot
 ```
 
 ## Usage
 
 Before getting started, ensure you've your Telegram bot token. If that's not the case then purpose to secure one from [@BotFather](https://telegram.me/BotFather).
 
-Proceed to fill the [env](env) configuration file as per the needs and then rename it `.env` before firing up the server `python3 run.py`.
+Proceed to fill the [env](env) configuration file as per the needs and then rename it `.env` before firing up the bot `python3 run.py`.
 
-Alternatively, using CLI interface::
+Alternatively, using CLI:
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
 ### Commands
 
@@ -74,21 +74,21 @@
 
 - **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
 
 - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of them.
 
 - **/history**: Provides users with the ability to view the history of their chats with the bot. This command is useful for reviewing past interactions or finding specific information from previous conversations.
 
-- **/settings**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
+- **/check**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
 
 - **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
 
 - **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
 
-- `any other text or command>`: An alias for `/chat`, allowing users to continue with text chat.
+- `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
 
 ### Administrative Commands
 
 
 ### Administrative Commands
```

#### html2text {}

```diff
@@ -10,63 +10,63 @@
 from text, `pytgpt-bot` has got you covered. ## Prerequisites - [x]
 [Python>=3.10](https://python.org) ## Installation 1. From Source Clone repo
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
-file as per the needs and then rename it `.env` before firing up the server
-`python3 run.py`. Alternatively, using CLI interface:: `$ pytgpt-bot run ` ##
-Features ### Commands ### Usage Information This section provides detailed
-instructions on how to use the various commands available in the bot. - **/
-start**: Displays the help information, offering a comprehensive list of
-available commands and their functionalities. This command is essential for
-users to quickly understand how to interact with the bot. - **/chat**: Initiate
-a natural language conversation with the AI. This command allows users to
-engage in interactive dialogues, ask questions, or make requests. - **/image**:
-Generates images from textual descriptions using the default provider. This
-feature enables users to visualize ideas or concepts through images. - **/
-prodia**: Generates images from textual descriptions using the Prodia provider.
-This command offers a unique style or interpretation of the text descriptions
+file as per the needs and then rename it `.env` before firing up the bot
+`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features ###
+Commands ### Usage Information This section provides detailed instructions on
+how to use the various commands available in the bot. - **/start**: Displays
+the help information, offering a comprehensive list of available commands and
+their functionalities. This command is essential for users to quickly
+understand how to interact with the bot. - **/chat**: Initiate a natural
+language conversation with the AI. This command allows users to engage in
+interactive dialogues, ask questions, or make requests. - **/image**: Generates
+images from textual descriptions using the default provider. This feature
+enables users to visualize ideas or concepts through images. - **/prodia**:
+Generates images from textual descriptions using the Prodia provider. This
+command offers a unique style or interpretation of the text descriptions
 compared to the default method. - **/audio**: Converts text to speech,
 providing users with the ability to listen to descriptions, instructions, or
 any text content read out by the AI. - **/intro**: Sets a new text for the chat
 intro. This command allows users to customize the chat introductory prompt
 which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
 voice for speech synthesis. This command enables users to choose from different
 voices for the AI to use when generating audio from text. - **/provider**: Sets
 a new chat provider. This command allows users to switch between different
 providers for various functionalities, such as `phind`, `llama2`, `koboldai`
 etc. - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of
 them. - **/history**: Provides users with the ability to view the history of
 their chats with the bot. This command is useful for reviewing past
 interactions or finding specific information from previous conversations. - **/
-settings**: Offers an overview of the bot's current configuration, including
-any custom settings applied by the user. - **/reset**: Resets the chat history
-and starts a new conversation thread. This command is useful for users who wish
-to start fresh or clear their chat history for privacy reasons. - **/myid**:
+check**: Offers an overview of the bot's current configuration, including any
+custom settings applied by the user. - **/reset**: Resets the chat history and
+starts a new conversation thread. This command is useful for users who wish to
+start fresh or clear their chat history for privacy reasons. - **/myid**:
 Echoes the user's Telegram ID. This command is useful for users who need to
 know their Telegram ID for various purposes, such as setting up bot admin. -
-`any other text or command>`: An alias for `/chat`, allowing users to continue
-with text chat. ### Administrative Commands ### Administrative Commands - `/
-clear`: Clears all chats. This command is used to remove all chat data from the
-bot's database. It's a powerful command that should be used with caution, as it
-will delete all chat history. - `/total`: Shows the total number of chats
-available. This command provides an overview of the current chat data stored in
-the bot's database, helping administrators understand the volume of
-interactions the bot has had. - `/drop`: Clears the entire chat table and bot
-logs. Similar to `/clear`, this command removes all data from the chat table in
-the database. It's a more drastic measure than `/clear`, as it completely wipes
-out all chat data and current contents of log file. - `/sql`: Allows running
-SQL statements against the database. This command provides a way for
-administrators to directly interact with the bot's database using SQL queries.
-It's a powerful tool for managing and analyzing the bot's data but should be
-used with caution to avoid unintended data loss or corruption. - `/logs`:
-Checks the logs. This command is used to access the bot's logs, which can
-provide insights into the bot's activity, errors, and user interactions. It's a
-valuable tool for monitoring and troubleshooting the bot's performance. ##
-Support and Feedback If you have any questions, feedback, or suggestions for
-`pytgpt`, please feel free to reach out. Your input is valuable in helping us
-improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
-source and available under the [MIT License](LICENSE). Feel free to use,
-modify, and distribute the code as you see fit. --- Thank you for using
-`pytgpt-bot`. Enjoy your AI-powered interactions!
+`any other text`: An alias for `/chat`, allowing users to continue with
+chatting. ### Administrative Commands ### Administrative Commands - `/clear`:
+Clears all chats. This command is used to remove all chat data from the bot's
+database. It's a powerful command that should be used with caution, as it will
+delete all chat history. - `/total`: Shows the total number of chats available.
+This command provides an overview of the current chat data stored in the bot's
+database, helping administrators understand the volume of interactions the bot
+has had. - `/drop`: Clears the entire chat table and bot logs. Similar to `/
+clear`, this command removes all data from the chat table in the database. It's
+a more drastic measure than `/clear`, as it completely wipes out all chat data
+and current contents of log file. - `/sql`: Allows running SQL statements
+against the database. This command provides a way for administrators to
+directly interact with the bot's database using SQL queries. It's a powerful
+tool for managing and analyzing the bot's data but should be used with caution
+to avoid unintended data loss or corruption. - `/logs`: Checks the logs. This
+command is used to access the bot's logs, which can provide insights into the
+bot's activity, errors, and user interactions. It's a valuable tool for
+monitoring and troubleshooting the bot's performance. ## Support and Feedback
+If you have any questions, feedback, or suggestions for `pytgpt`, please feel
+free to reach out. Your input is valuable in helping us improve and expand the
+bot's capabilities. ## License `pytgpt-bot` is open-source and available under
+the [MIT License](LICENSE). Feel free to use, modify, and distribute the code
+as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy your AI-powered
+interactions!
```

### Comparing `pytgpt_bot-0.0.9/pytgpt_bot/cli.py` & `pytgpt_bot-0.1.0/pytgpt_bot/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,14 +66,19 @@
 @click.option(
     "-p",
     "--provider",
     type=click.Choice(provider_keys),
     help="Default tgpt-based llm provider",
     default="auto",
 )
+@click.option(
+    "-d",
+    "--database",
+    help="Database engine URL e.g sqlite:////:memory:",
+)
 @click.help_option("-h", "--help")
 def run(**kwargs):
     """Start the bot"""
     click.secho("[*] Firing up bot - [pytgpt-bot]", fg="cyan")
 
     modded_kwargs: dict = {}
```

### Comparing `pytgpt_bot-0.0.9/pytgpt_bot/config.py` & `pytgpt_bot-0.1.0/pytgpt_bot/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .utils import provider_keys
 
 load_dotenv()
 
 assert environ.get("token"), "Export bot's token to the environment 😠"
 
 bot_token: str = environ.get("token")
+database: str = environ.get("database")
 provider: str = environ.get("provider", "auto")
 admin_id: int = int(environ.get("admin-id", 1234567))
 max_tokens: int = int(environ.get("max-tokens", 600))
 timeout: int = int(environ.get("timeout", 30))
 loglevel: int = int(environ.get("loglevel", 20))
 logfile = environ.get("logfile", "")
 voice: str = environ.get("voice", "Brian")
```

### Comparing `pytgpt_bot-0.0.9/pytgpt_bot/main.py` & `pytgpt_bot-0.1.0/pytgpt_bot/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,133 @@
 import telebot
+import json
+import logging
 import pytgpt.imager as image_generator
 from pytgpt.utils import Audio as audio_generator
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
 from functools import wraps
-import logging
-import json
+from sqlalchemy import text
+
+from . import __version__, __repo__
 
 from .config import (
     bot_token,
     max_tokens,
     timeout,
     loglevel,
     logfile,
     admin_id,
     provider,
 )
-from .db import User, Chat
+from .db import User
 from .utils import provider_keys
 from .utils import provider_map
+from .utils import get_random_emoji
+from .models import session, Chat, create_all, drop_all
 
 chosen_provider: str = provider_map.get(provider)
 
 log_params = dict(
     format="%(asctime)s : %(levelname)s - %(message)s",
     datefmt="%d-%b-%Y %H:%M:%S",
     level=loglevel,
 )
 
-awesome_prompts: dict = AwesomePrompts().get_acts()
-awesome_prompts_keys: list = list(awesome_prompts.keys())
+awesome_prompts_dict: dict = AwesomePrompts().get_acts()
+awesome_prompts_keys: list = list(awesome_prompts_dict.keys())
 
 if logfile:
     log_params["filename"] = logfile
 
 logging.basicConfig(**log_params)
 
-bot = telebot.TeleBot(bot_token, parse_mode="Markdown")
+bot = telebot.TeleBot(bot_token, disable_web_page_preview=True)
 
 bot.remove_webhook()
 
-logging.info(f"Bot started sucessfully. Admin ID - [{admin_id}]")
+logging.info(f"Bot started sucessfully {get_random_emoji('happy')}. Admin ID - [{admin_id}]")
+
+usage_info = (
+    "Welcome to [PYTGPT-BOT](https://github.com/Simatwa/pytgpt-bot) ✨.\n"
+    "For chatting, text-to-image and text-to-voice conversions.\n\n"
+    "Usage commands:\n"
+    "1. /start : Show this help info 📚\n"
+    "2. /chat : Chat with AI 🤖\n"
+    "3. /image : Generate image from text 🖼️ (default)\n"
+    "4. /prodia : Generate image from text 🎨 (Prodia)\n"
+    "5. /audio : Generate audio from text 🎧\n"
+    "6. /intro : Set new text for chat intro 📝\n"
+    "7. /voice : Set new voice for speech synthesis 🎙️\n"
+    "8. /provider : Set new chat provider 🌐\n"
+    "9. /awesome : Set awesome prompt as intro 💥\n"
+    "10. /history : Check chat history 🕰️\n"
+    "11. /check : Check current settings ⚙️\n"
+    "12. /reset : Start new chat thread 🔄\n"
+    "13. /myid : Echo your Telegram ID 🆔\n"
+    "default : Chat with AI.\n\n"
+    f"For instances {get_random_emoji('love')}:\n"
+    "\t\t\t/chat Hello there.\n"
+    "\t\t\t/image Peaceful desert scene\n"
+    "\t\t\t/prodia Clear cool shore view\n"
+    "\t\t\t/audio I am better than you.\n\n"
+    f"[🌟 Star me on Github]({__repo__}) pytgpt-bot v{__version__}"
+)
 
-admin_commands = """
-    /clear : Clear all chats.
-    /total : Total chats available.
-    /drop : Clear entire chat table and bot logs.
-    /sql : Run sql statements against database.
-    /logs : View bot logs.
-"""
+admin_commands = (
+    "\n\nAdmin Commands\n"
+    "/clear : Clear all chats 🧹\n"
+    "/total : Total chats available 📊\n"
+    "/drop : Clear entire chat table and bot logs 🗑️\n"
+    "/sql : Run sql statements against database ⏳\n"
+    "/logs : View bot logs 📜"
+)
 
 
-def handler_formatter(text: bool = False, admin: bool = False):
+def handler_formatter(text: bool = False, admin: bool = False, preserve: bool = False):
     """Handles common message handler verification and execptions
 
     Args:
         text (bool, optional): Command must contain text?. Defaults to False.
         admin (bool, optional): Needs admin privileges?. Defaults to False.
+        preserve (bool, optional): Do not alter text?. Default to False.
     """
 
     def main(func):
 
         @wraps(func)
         def decorator(message: telebot.types.Message):
             try:
                 logging.info(
                     f"Serving user [{message.from_user.id}] ({message.from_user.full_name}) - Function [{func.__name__}]"
                 )
-                if admin and not User(message.from_user.id).is_admin:
+                if admin and not User(message).is_admin:
                     return bot.reply_to(
                         message,
-                        "Action restricted to admins only❗️",
+                        f"{get_random_emoji("angry")} Action restricted to admins only❗️",
                         reply_markup=make_delete_markup(message),
                     )
 
-                if message.text and message.text.startswith("/"):
+                if message.text and message.text.startswith("/") and not preserve:
                     message.text = " ".join(message.text.split(" ")[1:])
 
                 if text and not message.text:
                     return bot.reply_to(
                         message,
-                        "Text is required❗️❗️.",
+                        f"{get_random_emoji()} Text is required❗️❗️.",
                         reply_markup=make_delete_markup(message),
                     )
 
                 return func(message)
             except Exception as e:
                 logging.error(f"Error on function - {func.__name__} - {e}")
-                logging.exception(e)
+                logging.debug(str(e))
                 bot.reply_to(
                     message,
-                    text="😔 An error occured and I could't complete that request ❗️❗️❗️",
+                    text=f"{get_random_emoji('angry')} An error occured and I could't complete that request ❗️❗️❗️",
                     reply_markup=make_delete_markup(message),
                 )
 
         return decorator
 
     return main
 
@@ -112,106 +145,105 @@
         text="🗑️", callback_data=f"delete:{message.chat.id}:{message.id}"
     )
     markup.add(callback_button)
     return markup
 
 
 def send_and_add_delete_button(
-    message: telebot.types.Message, text: str, as_reply: bool = False
+    message: telebot.types.Message,
+    text: str,
+    as_reply: bool = False,
+    parse_mode="Markdown",
 ):
     """Add send text and add delete inlineKeyboard item
 
     Args:
         message (telebot.types.Message):
         text (str): Tag
         as_reply (bool): Respond as a reply_to. Defaults to False.
+        parse_mode (str): __. Defaults to Markdown.
 
     Returns:
         _type_: _description_
     """
     markup = make_delete_markup(message)
     return (
-        bot.reply_to(message, text=text, reply_markup=markup)
+        bot.reply_to(message, text=text, reply_markup=markup, parse_mode=parse_mode)
         if as_reply
-        else bot.send_message(message.chat.id, text, reply_markup=markup)
+        else bot.send_message(
+            message.chat.id, text, reply_markup=markup, parse_mode=parse_mode
+        )
     )
 
 
-def send_long_text(message: telebot.types.Message, text: str, add_delete: bool = False):
+def send_long_text(
+    message: telebot.types.Message,
+    text: str,
+    add_delete: bool = False,
+    parse_mode="Markdown",
+):
     """Send texts longer than 4096 long
 
     Args:
         message (telebot.types.Message): Message object.
         text (str): Text to be sent.
         add_delete (bool). Add delete button. Defaults to False.
+        parse_mode (str): __. Defaults to Markdown.
     """
     max_length = 4096
     take_action = send_and_add_delete_button if add_delete else bot.send_message
     if len(text) <= max_length:
         # bot.send_message(message.chat.id, text)
-        take_action(message if add_delete else message.chat.id, text)
+        take_action(
+            message if add_delete else message.chat.id, text, parse_mode=parse_mode
+        )
     else:
         parts = [text[i : i + max_length] for i in range(0, len(text), max_length)]
         for part in parts:
-            take_action(message if add_delete else message.chat.id, part)
+            take_action(
+                message if add_delete else message.chat.id, part, parse_mode=parse_mode
+            )
 
 
 @bot.message_handler(commands=["help", "start"])
 @handler_formatter()
 def home(message: telebot.types.Message):
-    """
-    Welcome to [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot). Freely interact with multiple LLM providers.
-    /start : Show this help info.
-    /chat : Chat with AI.
-    /image : Generate image from text. (default)
-    /prodia : Generate image from text. (Prodia)
-    /audio : Generate audio from text.
-    /intro : Set new text for chat intro.
-    /voice : Set new voice for speech synthesis.
-    /provider : Set new chat provider.
-    /awesome : Set awesome prompt as intro.
-    /history : Check chat history.
-    /settings : Check current settings.
-    /reset : Start new chat thread.
-    /myid : Echo your Telegram ID.
-    /default : Chat with AI.
-    """
+    """Show help"""
 
     return bot.send_message(
         message.chat.id,
-        text=(
-            home.__doc__ + admin_commands if User(message.from_user.id).is_admin else ""
-        ),
+        text=(usage_info + admin_commands if User(message).is_admin else usage_info),
         reply_markup=make_delete_markup(message),
+        parse_mode="Markdown",
     )
 
 
 @bot.message_handler(commands=["myid"])
 @handler_formatter()
 def echo_user_id(message: telebot.types.Message):
     return bot.reply_to(
         message,
-        f"Greetings {message.from_user.first_name}. Your Telegram ID is {message.from_user.id}.",
+        f"Greetings {message.from_user.first_name} {get_random_emoji('love')}. Your Telegram ID is {message.from_user.id}.",
         reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["intro"])
 @handler_formatter(text=True)
 def set_chat_intro(message: telebot.types.Message):
     """Set new value for chat intro"""
-    intro = AwesomePrompts().get_act(message.text) or message.text
+    intro = awesome_prompts_dict.get(message.text,message.text)
     if not len(intro) > 10:
         return bot.reply_to(
             message,
-            "The chat introduction must be at least 10 characters long.",
+            f"{get_random_emoji('sad')} The chat introduction must be at least 10 characters long.",
             reply_markup=make_delete_markup(message),
         )
-    user = User(message.from_user.id)
-    user.update_intro(intro)
+    user = User(message)
+    user.chat.intro = intro
     return bot.reply_to(
         message, "New intro set successfully.", reply_markup=make_delete_markup(message)
     )
 
 
 @bot.message_handler(commands=["voice"])
 @handler_formatter(text=False)
@@ -220,125 +252,130 @@
     user_id: str = message.from_user.id
     markup = telebot.types.InlineKeyboardMarkup(row_width=4)
     make_item = lambda voice: telebot.types.InlineKeyboardButton(
         voice, callback_data=f"{voice}:{user_id}"
     )
     markup.add(*map(make_item, audio_generator.all_voices))
     bot.delete_message(message.chat.id, message.id)
-    return bot.send_message(message.chat.id, "Choose a voice:", reply_markup=markup)
+    return bot.send_message(message.chat.id, f"Choose a voice {get_random_emoji('happy')}:", reply_markup=markup)
 
 
 @bot.callback_query_handler(
     func=lambda call: call.data.split(":")[0] in audio_generator.all_voices
 )
 def set_new_speech_voice_callback(call: telebot.types.CallbackQuery):
     """Set new voice for speech synthesis callback handler"""
     bot.delete_message(call.message.chat.id, call.message.id)
     voice, user_id = call.data.split(":")
     message = call.message
     markup = make_delete_markup(call.message)
-    user = User(int(user_id))
-    user.update_voice(voice)
+    user = User(user_id=int(user_id))
+    user.chat.voice = voice
     return bot.send_message(
-        message.chat.id, f"New voice set : `{voice}`", reply_markup=markup
+        message.chat.id, f"{get_random_emoji('happy')} New voice set : `{voice}`", reply_markup=markup, parse_mode="Markdown"
     )
 
 
 @bot.message_handler(commands=["provider"])
 @handler_formatter(text=False)
 def set_new_text_provider(message: telebot.types.Message):
     """Set new text provider"""
     user_id: str = message.from_user.id
     markup = telebot.types.InlineKeyboardMarkup(row_width=2)
     make_item = lambda provider: telebot.types.InlineKeyboardButton(
         provider, callback_data=f"{provider}:{user_id}"
     )
     markup.add(*map(make_item, provider_keys))
     bot.delete_message(message.chat.id, message.id)
-    return bot.send_message(message.chat.id, "Choose a provider:", reply_markup=markup)
+    return bot.send_message(message.chat.id, f"Choose a provider {get_random_emoji('love')}:", reply_markup=markup)
 
 
 @bot.callback_query_handler(func=lambda call: call.data.split(":")[0] in provider_keys)
 def set_new_text_provider_callback(call: telebot.types.CallbackQuery):
     """Set new text provider callback handler"""
     bot.delete_message(call.message.chat.id, call.message.id)
     provider, user_id = call.data.split(":")
     message = call.message
     markup = make_delete_markup(call.message)
-    user = User(int(user_id))
-    user.update_provider(provider)
+    user = User(user_id=int(user_id))
+    user.chat.provider = provider
     return bot.send_message(
-        message.chat.id, f"New text provider set : `{provider}`", reply_markup=markup
+        message.chat.id, f"New text provider set {get_random_emoji('love')}: `{provider}`", reply_markup=markup, parse_mode="Markdown"
     )
 
 
 @bot.message_handler(commands=["awesome"])
 @handler_formatter(text=False)
 def set_awesome_prompt_as_chat_intro(message: telebot.types.Message):
     """Set awesome prompt as intro"""
     user_id: str = message.from_user.id
     markup = telebot.types.InlineKeyboardMarkup(row_width=4)
     make_item = lambda awesome: telebot.types.InlineKeyboardButton(
         awesome, callback_data=f"{awesome}:{user_id}"
     )
     markup.add(*map(make_item, awesome_prompts_keys))
     bot.delete_message(message.chat.id, message.id)
-    return bot.send_message(message.chat.id, "Choose awesome:", reply_markup=markup)
+    return bot.send_message(message.chat.id, f"Choose awesome {get_random_emoji('love')}:", reply_markup=markup)
 
 
 @bot.callback_query_handler(
     func=lambda call: call.data.split(":")[0] in awesome_prompts_keys
 )
 def set_awesome_prompt_as_chat_intro_callback_handler(
     call: telebot.types.CallbackQuery,
 ):
     """Set awesome prompt as intro callback handler"""
     bot.delete_message(call.message.chat.id, call.message.id)
     awesome_prompt, user_id = call.data.split(":")
-    user = User(int(user_id))
-    user.update_intro(awesome_prompts.get(awesome_prompt))
+    user = User(user_id=int(user_id))
+    user.chat.intro = awesome_prompts_dict.get(awesome_prompt)
     return bot.send_message(
         call.message.chat.id,
-        f"""New awesome-intro set:
-```
-{awesome_prompts.get(awesome_prompt)}
-```.""",
+        f"""New awesome-intro set:\n```{user.chat.intro}\n```.""",
         reply_markup=make_delete_markup(call.message),
+        parse_mode="Markdown"
     )
 
 
-@bot.message_handler(commands=["settings"])
+@bot.message_handler(commands=["check"])
 @handler_formatter()
 def check_current_settings(message: telebot.types.Message):
     """Check current user settings"""
-    user_record: dict = User(message.from_user.id).record
+    chat = User(message).chat
     current_user_settings = (
-        f"Chat Length : `{len(user_record.get('history'))}`\n"
-        f"Speech Voice : `{user_record.get('voice')}`\n"
-        f"Chat Provider : `{user_record.get('provider')}`\n"
-        f"Chat Intro : `{user_record.get('intro')}`"
+        f"Chat Length : `{len(chat.history)}`\n"
+        f"Speech Voice : `{chat.voice}`\n"
+        f"Chat Provider : `{chat.provider}`\n"
+        f"Chat Intro : `{chat.intro}`"
     )
     return bot.reply_to(
-        message, current_user_settings, reply_markup=make_delete_markup(message)
+        message,
+        current_user_settings,
+        reply_markup=make_delete_markup(message),
+        parse_mode="Markdown",
     )
 
 
 @bot.message_handler(commands=["history"])
 @handler_formatter()
 def check_chat_history(message: telebot.types.Message):
-    user = User(message.from_user.id)
+    user = User(message)
     return send_long_text(
-        message, user.chat_history or "Your chat history is empty ❗️", add_delete=True
+        message,
+        user.chat.history or f"{get_random_emoji()} Your chat history is empty ❗️",
+        add_delete=True,
+        parse_mode="Markdown",
     )
 
 
 @bot.message_handler(commands=["image", "img"])
 @handler_formatter(text=True)
 def text_to_image_default(message: telebot.types.Message):
     """Generate image using `image`"""
+    bot.send_chat_action(message.chat.id, "upload_photo", timeout=timeout)
     generator_obj = image_generator.Imager(
         timeout=timeout,
     )
     return bot.send_photo(
         message.chat.id,
         photo=generator_obj.generate(
             message.text,
@@ -348,28 +385,30 @@
     )
 
 
 @bot.message_handler(commands=["prodia", "prod"])
 @handler_formatter(text=True)
 def text_to_image_prodia(message: telebot.types.Message):
     """Generate image using `prodia`"""
+    bot.send_chat_action(message.chat.id, "upload_photo", timeout=timeout)
     generator_obj = image_generator.Prodia(timeout=timeout)
     return bot.send_photo(
         message.chat.id,
         photo=generator_obj.generate(message.text)[0],
         caption=message.text,
         reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["audio", "aud"])
 @handler_formatter(text=True)
 def text_to_audio(message: telebot.types.Message):
     """Convert text to audio"""
-    voice = User(message.chat.id).chat_voice
+    bot.send_chat_action(message.chat.id, "upload_audio", timeout=timeout)
+    voice = User(message).chat.voice
     audio_chunk = audio_generator.text_to_audio(
         message=message.text,
         voice=voice,
         timeout=timeout,
     )
     return bot.send_audio(
         message.chat.id,
@@ -381,45 +420,45 @@
     )
 
 
 @bot.message_handler(commands=["reset"])
 @handler_formatter()
 def reset_chat(message: telebot.types.Message):
     """Reset current chat thread"""
-    user = User(message.from_user.id)
+    user = User(message)
     user.delete()
     return bot.reply_to(
-        message, "New chat instance created.", reply_markup=make_delete_markup(message)
+        message, f"New chat instance created. {get_random_emoji('happy')}", reply_markup=make_delete_markup(message)
     )
 
 
 @bot.message_handler(commands=["clear", "clear_chats"])
 @handler_formatter(admin=True)
 def clear_chats(message: telebot.types.Message):
     """Delete all chat entries"""
-    Chat.query("DELETE FROM Chat")
+    session.query(Chat).delete()
     logging.warning(
         f"Clearing Chats - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
     return bot.reply_to(
-        message, "Chats cleared successfully.", reply_markup=make_delete_markup(message)
+        message, f"{get_random_emoji('love')} Chats cleared successfully.", reply_markup=make_delete_markup(message)
     )
 
 
 @bot.message_handler(commands=["total", "total_chats"])
 @handler_formatter(admin=True)
 def total_chats_query(message: telebot.types.Message):
     """Query total chats"""
-    total_chats = Chat.query("SELECT COUNT(id) FROM Chat")[0][0]
+    total_chats = session.query(Chat).count()
     logging.warning(
         f"Total Chats query - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
     return bot.reply_to(
         message,
-        f"Total Chats **{total_chats}**",
+        f"Total Chats {total_chats}",
         reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["drop", "drop_chats"])
 @handler_formatter(admin=True)
 def total_chats_table_and_logs(message: telebot.types.Message):
@@ -428,81 +467,107 @@
         with open(logfile, "w") as fh:
             fh.write(
                 f"ADMIN CLEARED LOGS & DROPPED CHAT TABLE [{message.from_user.id}] - ({message.from_user.full_name})\n"
             )
     logging.warning(
         f"Dropping Chat table and reinitialize - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
-    Chat.query("DROP TABLE CHAT")
-    Chat.initialize()
+    drop_all()
+    create_all()
     return bot.reply_to(
         message,
-        f"Chat table and bot logs dropped and new one created.",
+        f"{get_random_emoji('love')} Chat table and bot logs dropped and new one created.",
         reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["sql"])
-@handler_formatter(admin=True)
+@handler_formatter(admin=True, text=True)
 def run_sql_statement(message: telebot.types.Message):
     """Run sql statements against database"""
     logging.warning(
         f"Running SQL statements - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
     try:
-        response = f"""
-        ```
-        {Chat.query(message.text)}
-        ```
-        """
+        results = session.execute(text(message.text))
+        response: dict[str, list] = {}
+        if results:
+            for count, row in enumerate(results):
+                response[count] = str(row)
+            jsonified_response = json.dumps(
+                response,
+                indent=3,
+            )
+            response = f"```json\n{jsonified_response}\n```"
+        else:
+            response = f"```\n{results}\n```"
+        session.commit()
 
     except Exception as e:
-        response = f"ERROR : {e.args[1] if e.args and len(e.args)>1 else e}"
+        response = f"{e.args[1] if e.args and len(e.args)>1 else e}"
 
     finally:
-        return send_long_text(message, response, add_delete=True)
+        return send_long_text(
+            message,
+            response,
+            add_delete=True,
+        )
 
 
 @bot.message_handler(commands=["logs"])
 @handler_formatter(admin=True)
 def check_current_settings(message: telebot.types.Message):
     """View bot logs"""
     if not logfile:
-        return bot.reply_to(message, "Logfile not specified!")
+        return bot.reply_to(message, f"{get_random_emoji()} Logfile not specified ❗️",reply_markup=make_delete_markup(message))
     with open(logfile, encoding="utf-8") as fh:
         contents: str = fh.read()
-    return send_long_text(message, contents, add_delete=True)
+    return send_long_text(message, contents, add_delete=True, parse_mode=None)
+
 
+def is_action_for_chat(message: telebot.types.Message) -> bool:
+    splitted_text = message.text.split(" ")
+    if splitted_text[0].startswith("/"):
+        if splitted_text[0] == "/chat":
+            return True
+        else:
+            return False
+    return True
 
-@bot.message_handler(content_types=["text"])
+
+@bot.message_handler(content_types=["text"], func=is_action_for_chat)
 @handler_formatter(text=True)
 def text_chat(message: telebot.types.Message):
     """Text generation"""
-    user = User(message.from_user.id)
-    chat_record = user.record
+    user = User(message)
     conversation = Conversation(max_tokens=max_tokens)
-    conversation.chat_history = chat_record.get("history")
-    user_provider = provider_map.get(chat_record.get("provider"))
+    conversation.chat_history = user.chat.history
+    user_provider = provider_map.get(user.chat.provider)
     conversation_prompt = conversation.gen_complete_prompt(
-        message.text, intro=chat_record.get("intro")
+        message.text, intro=user.chat.intro
     )
     bot.send_chat_action(message.chat.id, "typing")
     ai_response = user_provider(is_conversation=False, timeout=timeout).chat(
         conversation_prompt
     )
     conversation.update_chat_history(
         prompt=message.text, response=ai_response, force=True
     )
-    user.update_history(conversation.chat_history)
-    return send_long_text(message, ai_response)
+    user.chat.history = conversation.chat_history
+    send_long_text(message, ai_response)
 
 
 @bot.message_handler(func=lambda val: True)
 def any_other_action(message):
-    return bot.reply_to(message, home.__doc__, reply_markup=make_delete_markup(message))
+    return bot.reply_to(
+        message,
+        usage_info,
+        reply_markup=make_delete_markup(message),
+        parse_mode="Markdown",
+    )
 
 
 @bot.callback_query_handler(func=lambda call: call.data.startswith("delete:"))
 def delete_callback_handler(
     call: telebot.types.CallbackQuery,
 ):
     """Delete callback handler"""
```

### Comparing `pytgpt_bot-0.0.9/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.1.0/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.9
-Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
+Version: 0.1.0
+Summary: Telegram bot for chatting, text-to-image and text-to-voice conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/pytgpt-bot
@@ -31,18 +31,19 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytelegrambotapi==4.17.0
 Requires-Dist: python-tgpt==0.6.6
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: click==8.1.3
+Requires-Dist: SQLAlchemy==2.0.29
 
 <p align="center">
 <a href="https://github.com/Simatwa/pytgpt-bot/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=MIT&color=Blue&message=MIT&label=License"/></a>
-<a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt"/></a>
+<a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt-bot"/></a>
 <a href="https://pypi.org/project/pytgpt-bot"><img alt="PyPi" src="https://img.shields.io/pypi/v/pytgpt-bot?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
 <a href="https://pepy.tech/project/pytgpt-bot"><img src="https://static.pepy.tech/personalized-badge/pytgpt-bot?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <!--
 <a href="https://github.com/Simatwa/pytgpt-bot/releases"><img src="https://img.shields.io/github/v/release/Simatwa/pytgpt-bot?color=success&label=Release&logo=github" alt="Latest release"></img></a> 
 -->
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/pytgpt-bot"/></a>
@@ -77,17 +78,17 @@
 pip install pytgpt-bot
 ```
 
 ## Usage
 
 Before getting started, ensure you've your Telegram bot token. If that's not the case then purpose to secure one from [@BotFather](https://telegram.me/BotFather).
 
-Proceed to fill the [env](env) configuration file as per the needs and then rename it `.env` before firing up the server `python3 run.py`.
+Proceed to fill the [env](env) configuration file as per the needs and then rename it `.env` before firing up the bot `python3 run.py`.
 
-Alternatively, using CLI interface::
+Alternatively, using CLI:
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
 ### Commands
 
@@ -112,21 +113,21 @@
 
 - **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
 
 - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of them.
 
 - **/history**: Provides users with the ability to view the history of their chats with the bot. This command is useful for reviewing past interactions or finding specific information from previous conversations.
 
-- **/settings**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
+- **/check**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
 
 - **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
 
 - **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
 
-- `any other text or command>`: An alias for `/chat`, allowing users to continue with text chat.
+- `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
 
 ### Administrative Commands
 
 
 ### Administrative Commands
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.9 Summary: Telegram bot for
-text generation, text-to-image and text-to-audio conversions. Home-page: https:
-//github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.0 Summary: Telegram bot for
+chatting, text-to-image and text-to-voice conversions Home-page: https://
+github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
 pytgpt-bot/releases Project-URL: Documentation, https://github.com/Simatwa/
 pytgpt-bot/blob/main/README.md Keywords:
@@ -17,15 +17,16 @@
 Python Modules Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pytelegrambotapi==4.17.0 Requires-Dist: python-tgpt==0.6.6 Requires-Dist:
-python-dotenv==1.0.0 Requires-Dist: click==8.1.3
+python-dotenv==1.0.0 Requires-Dist: click==8.1.3 Requires-Dist:
+SQLAlchemy==2.0.29
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/
    _a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_g_p_t_-_b_o_t_]
                                   _[_w_a_k_a_t_i_m_e_]
                       ************ WWeellccoommee ttoo _pp_yy_tt_gg_pp_tt_--_bb_oo_tt ************
 This is a Telegram bot based on [python-tgpt](https://github.com/Simatwa/
 python-tgpt), a powerful tool designed to enhance your interactions with AI.
 This bot is built on the robust foundation of the `pyTelegramBotAPI` and offers
@@ -34,63 +35,63 @@
 from text, `pytgpt-bot` has got you covered. ## Prerequisites - [x]
 [Python>=3.10](https://python.org) ## Installation 1. From Source Clone repo
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
-file as per the needs and then rename it `.env` before firing up the server
-`python3 run.py`. Alternatively, using CLI interface:: `$ pytgpt-bot run ` ##
-Features ### Commands ### Usage Information This section provides detailed
-instructions on how to use the various commands available in the bot. - **/
-start**: Displays the help information, offering a comprehensive list of
-available commands and their functionalities. This command is essential for
-users to quickly understand how to interact with the bot. - **/chat**: Initiate
-a natural language conversation with the AI. This command allows users to
-engage in interactive dialogues, ask questions, or make requests. - **/image**:
-Generates images from textual descriptions using the default provider. This
-feature enables users to visualize ideas or concepts through images. - **/
-prodia**: Generates images from textual descriptions using the Prodia provider.
-This command offers a unique style or interpretation of the text descriptions
+file as per the needs and then rename it `.env` before firing up the bot
+`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features ###
+Commands ### Usage Information This section provides detailed instructions on
+how to use the various commands available in the bot. - **/start**: Displays
+the help information, offering a comprehensive list of available commands and
+their functionalities. This command is essential for users to quickly
+understand how to interact with the bot. - **/chat**: Initiate a natural
+language conversation with the AI. This command allows users to engage in
+interactive dialogues, ask questions, or make requests. - **/image**: Generates
+images from textual descriptions using the default provider. This feature
+enables users to visualize ideas or concepts through images. - **/prodia**:
+Generates images from textual descriptions using the Prodia provider. This
+command offers a unique style or interpretation of the text descriptions
 compared to the default method. - **/audio**: Converts text to speech,
 providing users with the ability to listen to descriptions, instructions, or
 any text content read out by the AI. - **/intro**: Sets a new text for the chat
 intro. This command allows users to customize the chat introductory prompt
 which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
 voice for speech synthesis. This command enables users to choose from different
 voices for the AI to use when generating audio from text. - **/provider**: Sets
 a new chat provider. This command allows users to switch between different
 providers for various functionalities, such as `phind`, `llama2`, `koboldai`
 etc. - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of
 them. - **/history**: Provides users with the ability to view the history of
 their chats with the bot. This command is useful for reviewing past
 interactions or finding specific information from previous conversations. - **/
-settings**: Offers an overview of the bot's current configuration, including
-any custom settings applied by the user. - **/reset**: Resets the chat history
-and starts a new conversation thread. This command is useful for users who wish
-to start fresh or clear their chat history for privacy reasons. - **/myid**:
+check**: Offers an overview of the bot's current configuration, including any
+custom settings applied by the user. - **/reset**: Resets the chat history and
+starts a new conversation thread. This command is useful for users who wish to
+start fresh or clear their chat history for privacy reasons. - **/myid**:
 Echoes the user's Telegram ID. This command is useful for users who need to
 know their Telegram ID for various purposes, such as setting up bot admin. -
-`any other text or command>`: An alias for `/chat`, allowing users to continue
-with text chat. ### Administrative Commands ### Administrative Commands - `/
-clear`: Clears all chats. This command is used to remove all chat data from the
-bot's database. It's a powerful command that should be used with caution, as it
-will delete all chat history. - `/total`: Shows the total number of chats
-available. This command provides an overview of the current chat data stored in
-the bot's database, helping administrators understand the volume of
-interactions the bot has had. - `/drop`: Clears the entire chat table and bot
-logs. Similar to `/clear`, this command removes all data from the chat table in
-the database. It's a more drastic measure than `/clear`, as it completely wipes
-out all chat data and current contents of log file. - `/sql`: Allows running
-SQL statements against the database. This command provides a way for
-administrators to directly interact with the bot's database using SQL queries.
-It's a powerful tool for managing and analyzing the bot's data but should be
-used with caution to avoid unintended data loss or corruption. - `/logs`:
-Checks the logs. This command is used to access the bot's logs, which can
-provide insights into the bot's activity, errors, and user interactions. It's a
-valuable tool for monitoring and troubleshooting the bot's performance. ##
-Support and Feedback If you have any questions, feedback, or suggestions for
-`pytgpt`, please feel free to reach out. Your input is valuable in helping us
-improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
-source and available under the [MIT License](LICENSE). Feel free to use,
-modify, and distribute the code as you see fit. --- Thank you for using
-`pytgpt-bot`. Enjoy your AI-powered interactions!
+`any other text`: An alias for `/chat`, allowing users to continue with
+chatting. ### Administrative Commands ### Administrative Commands - `/clear`:
+Clears all chats. This command is used to remove all chat data from the bot's
+database. It's a powerful command that should be used with caution, as it will
+delete all chat history. - `/total`: Shows the total number of chats available.
+This command provides an overview of the current chat data stored in the bot's
+database, helping administrators understand the volume of interactions the bot
+has had. - `/drop`: Clears the entire chat table and bot logs. Similar to `/
+clear`, this command removes all data from the chat table in the database. It's
+a more drastic measure than `/clear`, as it completely wipes out all chat data
+and current contents of log file. - `/sql`: Allows running SQL statements
+against the database. This command provides a way for administrators to
+directly interact with the bot's database using SQL queries. It's a powerful
+tool for managing and analyzing the bot's data but should be used with caution
+to avoid unintended data loss or corruption. - `/logs`: Checks the logs. This
+command is used to access the bot's logs, which can provide insights into the
+bot's activity, errors, and user interactions. It's a valuable tool for
+monitoring and troubleshooting the bot's performance. ## Support and Feedback
+If you have any questions, feedback, or suggestions for `pytgpt`, please feel
+free to reach out. Your input is valuable in helping us improve and expand the
+bot's capabilities. ## License `pytgpt-bot` is open-source and available under
+the [MIT License](LICENSE). Feel free to use, modify, and distribute the code
+as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy your AI-powered
+interactions!
```

### Comparing `pytgpt_bot-0.0.9/setup.py` & `pytgpt_bot-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.0.9",
+    version="0.1.0",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
-    description="Telegram bot for text generation, text-to-image and text-to-audio conversions.",
+    description="Telegram bot for chatting, text-to-image and text-to-voice conversions",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
         "Bug Report": "https://github.com/Simatwa/pytgpt-bot/issues/new",
         "Homepage": "https://github.com/Simatwa/pytgpt-bot",
         "Source Code": "https://github.com/Simatwa/pytgpt-bot",
         "Issue Tracker": "https://github.com/Simatwa/pytgpt-bot/issues",
         "Download": "https://github.com/Simatwa/pytgpt-bot/releases",
@@ -34,14 +34,15 @@
         ],
     },
     install_requires=[
         "pytelegrambotapi==4.17.0",
         "python-tgpt==0.6.6",
         "python-dotenv==1.0.0",
         "click==8.1.3",
+        "SQLAlchemy==2.0.29",
     ],
     python_requires=">=3.10",
     keywords=[
         "ai",
         "tgpt",
         "pytgpt",
         "chatbot",
```

