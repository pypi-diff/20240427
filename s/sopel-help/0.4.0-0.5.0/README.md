# Comparing `tmp/sopel-help-0.4.0.tar.gz` & `tmp/sopel_help-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-help-0.4.0.tar", last modified: Sat Jul 23 19:49:32 2022, max compression
+gzip compressed data, was "sopel_help-0.5.0.tar", last modified: Sat Apr 27 14:25:32 2024, max compression
```

## Comparing `sopel-help-0.4.0.tar` & `sopel_help-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,32 @@
-drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-07-23 19:49:32.382586 sopel-help-0.4.0/
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1021 2020-04-12 14:48:07.000000 sopel-help-0.4.0/LICENSE.txt
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      222 2020-04-12 14:48:07.000000 sopel-help-0.4.0/MANIFEST.in
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2248 2022-07-23 19:49:32.382586 sopel-help-0.4.0/PKG-INFO
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1023 2022-07-23 19:48:17.000000 sopel-help-0.4.0/README.rst
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1578 2022-07-23 19:49:32.386586 sopel-help-0.4.0/setup.cfg
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       38 2020-04-12 14:18:56.000000 sopel-help-0.4.0/setup.py
-drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-07-23 19:49:32.382586 sopel-help-0.4.0/sopel_help/
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2020-04-12 14:18:56.000000 sopel-help-0.4.0/sopel_help/__init__.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1818 2022-07-23 19:30:26.000000 sopel-help-0.4.0/sopel_help/config.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2593 2021-07-09 14:33:37.000000 sopel-help-0.4.0/sopel_help/managers.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     3170 2021-07-06 21:25:32.000000 sopel-help-0.4.0/sopel_help/mixins.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1584 2022-07-23 19:48:17.000000 sopel-help-0.4.0/sopel_help/plugin.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)    15635 2022-07-23 19:48:17.000000 sopel-help-0.4.0/sopel_help/providers.py
-drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-07-23 19:49:32.382586 sopel-help-0.4.0/sopel_help.egg-info/
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2248 2022-07-23 19:49:32.000000 sopel-help-0.4.0/sopel_help.egg-info/PKG-INFO
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      425 2022-07-23 19:49:32.000000 sopel-help-0.4.0/sopel_help.egg-info/SOURCES.txt
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)        1 2022-07-23 19:49:32.000000 sopel-help-0.4.0/sopel_help.egg-info/dependency_links.txt
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      278 2022-07-23 19:49:32.000000 sopel-help-0.4.0/sopel_help.egg-info/entry_points.txt
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)        1 2020-03-22 13:31:04.000000 sopel-help-0.4.0/sopel_help.egg-info/not-zip-safe
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       20 2022-07-23 19:49:32.000000 sopel-help-0.4.0/sopel_help.egg-info/requires.txt
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       11 2022-07-23 19:49:32.000000 sopel-help-0.4.0/sopel_help.egg-info/top_level.txt
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2024-04-27 14:25:32.680027 sopel_help-0.5.0/
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1021 2020-04-12 14:48:07.000000 sopel_help-0.5.0/LICENSE.txt
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      222 2020-04-12 14:48:07.000000 sopel_help-0.5.0/MANIFEST.in
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2263 2024-04-27 14:25:32.680027 sopel_help-0.5.0/PKG-INFO
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1023 2024-04-27 14:18:14.000000 sopel_help-0.5.0/README.rst
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1811 2024-04-27 14:20:27.000000 sopel_help-0.5.0/pyproject.toml
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      267 2024-04-27 14:25:32.680027 sopel_help-0.5.0/setup.cfg
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2024-04-27 14:25:32.676027 sopel_help-0.5.0/sopel_help/
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2020-04-12 14:18:56.000000 sopel_help-0.5.0/sopel_help/__init__.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1819 2024-04-27 14:18:14.000000 sopel_help-0.5.0/sopel_help/config.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2593 2021-07-09 14:33:37.000000 sopel_help-0.5.0/sopel_help/managers.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     3170 2021-07-06 21:25:32.000000 sopel_help-0.5.0/sopel_help/mixins.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1584 2022-07-23 19:48:17.000000 sopel_help-0.5.0/sopel_help/plugin.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)    15837 2024-04-27 14:18:14.000000 sopel_help-0.5.0/sopel_help/providers.py
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2024-04-27 14:25:32.680027 sopel_help-0.5.0/sopel_help.egg-info/
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2263 2024-04-27 14:25:32.000000 sopel_help-0.5.0/sopel_help.egg-info/PKG-INFO
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      694 2024-04-27 14:25:32.000000 sopel_help-0.5.0/sopel_help.egg-info/SOURCES.txt
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)        1 2024-04-27 14:25:32.000000 sopel_help-0.5.0/sopel_help.egg-info/dependency_links.txt
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      277 2024-04-27 14:25:32.000000 sopel_help-0.5.0/sopel_help.egg-info/entry_points.txt
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       20 2024-04-27 14:25:32.000000 sopel_help-0.5.0/sopel_help.egg-info/requires.txt
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)        1 2024-04-27 14:25:32.000000 sopel_help-0.5.0/sopel_help.egg-info/top_level.txt
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2024-04-27 14:25:32.680027 sopel_help-0.5.0/tests/
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     4233 2023-11-11 13:20:22.000000 sopel_help-0.5.0/tests/test_integrations.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1412 2022-07-23 19:48:17.000000 sopel_help-0.5.0/tests/test_managers.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      777 2021-07-06 21:25:32.000000 sopel_help-0.5.0/tests/test_mixins.py
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      912 2020-04-12 14:18:56.000000 sopel_help-0.5.0/tests/test_providers_0x0.py
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      925 2020-04-12 14:18:56.000000 sopel_help-0.5.0/tests/test_providers_abstract.py
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     3097 2020-04-12 14:18:56.000000 sopel_help-0.5.0/tests/test_providers_abstract_publisher.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)    14240 2024-04-27 14:18:14.000000 sopel_help-0.5.0/tests/test_providers_base.py
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      905 2020-04-12 14:18:56.000000 sopel_help-0.5.0/tests/test_providers_clbin.py
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1216 2020-04-12 14:18:56.000000 sopel_help-0.5.0/tests/test_providers_local.py
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1050 2020-04-12 14:18:56.000000 sopel_help-0.5.0/tests/test_providers_termbin.py
```

### Comparing `sopel-help-0.4.0/LICENSE.txt` & `sopel_help-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sopel-help-0.4.0/README.rst` & `sopel_help-0.5.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Install
 =======
 
 The recommanded way to install this plugin is to use ``pip``::
 
     $ pip install sopel-help
 
-Note that this plugin requires Python 3.7+ and Sopel 7.1+.
+Note that this plugin requires Python 3.8+ and Sopel 7.1+.
 
 Configure
 =========
 
 As with many other plugins, you can use ``sopel-config`` to launch the
 configuration wizard, like so::
```

### Comparing `sopel-help-0.4.0/sopel_help/config.py` & `sopel_help-0.5.0/sopel_help/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Configuration for the help plugin."""
+
 from sopel import config
 
 from sopel_help.managers import manager
 
 
 class HelpSection(config.types.StaticSection):
     """Configuration section for this module."""
```

### Comparing `sopel-help-0.4.0/sopel_help/managers.py` & `sopel_help-0.5.0/sopel_help/managers.py`

 * *Files identical despite different names*

### Comparing `sopel-help-0.4.0/sopel_help/mixins.py` & `sopel_help-0.5.0/sopel_help/mixins.py`

 * *Files identical despite different names*

### Comparing `sopel-help-0.4.0/sopel_help/plugin.py` & `sopel_help-0.5.0/sopel_help/plugin.py`

 * *Files identical despite different names*

### Comparing `sopel-help-0.4.0/sopel_help/providers.py` & `sopel_help-0.5.0/sopel_help/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 
 
 class UnknownCommand(Exception):
     """Command is unknown."""
 
 
 def _post_content(*args, **kwargs):
+    # ensure we always timeout
+    timeout = kwargs.pop('timeout', 30)
     try:
-        response = requests.post(*args, **kwargs)
+        response = requests.post(*args, timeout=timeout, **kwargs)
         response.raise_for_status()
     except (
             requests.exceptions.Timeout,
             requests.exceptions.TooManyRedirects,
             requests.exceptions.RequestException,
             requests.exceptions.HTTPError
     ) as err:
@@ -139,17 +141,19 @@
                 "The help for command %s is too long; "
                 "I'm sending it to you in a private message." % command)
             reply = bot.say
             recipient = trigger.nick
 
         reply(head, recipient)
         for line in body:
-            bot.say(line, recipient)
+            if line:
+                bot.say(line, recipient)
         for line in usages:
-            bot.say(line, recipient)
+            if line:
+                bot.say(line, recipient)
 
     def get_reply_method(self, bot, trigger):
         """Define the reply method and its recipient.
 
         :param bot: Wrapped bot object
         :type bot: :class:`sopel.bot.SopelWrapper`
         :param trigger: Trigger to reply to
@@ -289,14 +293,15 @@
         :param list lines: lines of help
         """
         template = """<!DOCTYPE html>
         <html>
             <head>
                 <title>Sopel Help</title>
                 <meta charset="utf-8">
+                <meta content="light dark" name="color-scheme">
             </head>
             <body>
             <h1>Sopel Help</h1>
             {content}
             </body>
         </html>
         """
```

