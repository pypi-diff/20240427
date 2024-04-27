# Comparing `tmp/tweety_ns-1.1.3.tar.gz` & `tmp/tweety_ns-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety_ns-1.1.3.tar", last modified: Tue Apr 23 08:18:05 2024, max compression
+gzip compressed data, was "tweety_ns-1.1.4.tar", last modified: Sat Apr 27 09:52:55 2024, max compression
```

## Comparing `tweety_ns-1.1.3.tar` & `tweety_ns-1.1.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.705319 tweety_ns-1.1.3/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-23 08:18:05.705319 tweety_ns-1.1.3/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety_ns-1.1.3/README.md
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety_ns-1.1.3/pyproject.toml
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      671 2024-04-23 08:18:05.705319 tweety_ns-1.1.3/setup.cfg
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      785 2024-04-23 07:11:33.000000 tweety_ns-1.1.3/setup.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.697319 tweety_ns-1.1.3/src/
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.701319 tweety_ns-1.1.3/src/tweety/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      276 2024-04-23 07:11:42.000000 tweety_ns-1.1.3/src/tweety/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     7486 2024-04-12 13:05:42.000000 tweety_ns-1.1.3/src/tweety/auth.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    31953 2024-04-23 07:05:13.000000 tweety_ns-1.1.3/src/tweety/bot.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    96143 2024-04-23 07:05:23.000000 tweety_ns-1.1.3/src/tweety/builder.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.701319 tweety_ns-1.1.3/src/tweety/events/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety_ns-1.1.3/src/tweety/events/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2119 2024-03-31 11:29:17.000000 tweety_ns-1.1.3/src/tweety/events/newmessage.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    22029 2024-04-14 08:52:30.000000 tweety_ns-1.1.3/src/tweety/exceptions_.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2343 2024-04-23 07:03:34.000000 tweety_ns-1.1.3/src/tweety/filters.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    20431 2024-04-23 06:55:33.000000 tweety_ns-1.1.3/src/tweety/http.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2362 2024-04-10 16:34:41.000000 tweety_ns-1.1.3/src/tweety/session.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.701319 tweety_ns-1.1.3/src/tweety/types/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1249 2024-03-20 05:30:39.000000 tweety_ns-1.1.3/src/tweety/types/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3039 2024-02-12 12:06:11.000000 tweety_ns-1.1.3/src/tweety/types/base.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1172 2024-01-20 09:02:27.000000 tweety_ns-1.1.3/src/tweety/types/bookmarks.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3256 2024-01-20 09:00:34.000000 tweety_ns-1.1.3/src/tweety/types/community.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4054 2024-02-22 14:22:03.000000 tweety_ns-1.1.3/src/tweety/types/follow.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      987 2024-01-20 08:43:34.000000 tweety_ns-1.1.3/src/tweety/types/gifs.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    17540 2024-04-04 20:48:50.000000 tweety_ns-1.1.3/src/tweety/types/inbox.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1444 2024-03-03 17:35:17.000000 tweety_ns-1.1.3/src/tweety/types/likes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4302 2024-01-20 08:28:50.000000 tweety_ns-1.1.3/src/tweety/types/lists.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1511 2024-01-19 19:19:11.000000 tweety_ns-1.1.3/src/tweety/types/mentions.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     9022 2024-04-10 16:29:13.000000 tweety_ns-1.1.3/src/tweety/types/n_types.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1351 2024-01-19 19:15:58.000000 tweety_ns-1.1.3/src/tweety/types/notification.py
--rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1103 2024-03-20 05:31:04.000000 tweety_ns-1.1.3/src/tweety/types/places.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-01-19 19:12:37.000000 tweety_ns-1.1.3/src/tweety/types/retweets.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3806 2024-02-03 16:37:11.000000 tweety_ns-1.1.3/src/tweety/types/search.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1216 2024-01-31 06:59:29.000000 tweety_ns-1.1.3/src/tweety/types/topic.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    58815 2024-04-14 08:56:44.000000 tweety_ns-1.1.3/src/tweety/types/twDataTypes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12236 2024-04-12 07:15:06.000000 tweety_ns-1.1.3/src/tweety/types/usertweet.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety_ns-1.1.3/src/tweety/updates.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    36382 2024-04-23 03:37:43.000000 tweety_ns-1.1.3/src/tweety/user.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     6531 2024-04-23 07:05:23.000000 tweety_ns-1.1.3/src/tweety/utils.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.705319 tweety_ns-1.1.3/src/tweety_ns.egg-info/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-23 08:18:05.000000 tweety_ns-1.1.3/src/tweety_ns.egg-info/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1026 2024-04-23 08:18:05.000000 tweety_ns-1.1.3/src/tweety_ns.egg-info/SOURCES.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-04-23 08:18:05.000000 tweety_ns-1.1.3/src/tweety_ns.egg-info/dependency_links.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-04-23 08:18:05.000000 tweety_ns-1.1.3/src/tweety_ns.egg-info/requires.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-04-23 08:18:05.000000 tweety_ns-1.1.3/src/tweety_ns.egg-info/top_level.txt
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 09:52:55.816221 tweety_ns-1.1.4/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-27 09:52:55.816221 tweety_ns-1.1.4/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety_ns-1.1.4/README.md
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety_ns-1.1.4/pyproject.toml
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      671 2024-04-27 09:52:55.816221 tweety_ns-1.1.4/setup.cfg
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      785 2024-04-27 09:47:22.000000 tweety_ns-1.1.4/setup.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 09:52:55.808221 tweety_ns-1.1.4/src/
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 09:52:55.812221 tweety_ns-1.1.4/src/tweety/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      276 2024-04-27 09:47:29.000000 tweety_ns-1.1.4/src/tweety/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     7526 2024-04-27 08:15:36.000000 tweety_ns-1.1.4/src/tweety/auth.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    31976 2024-04-27 09:34:06.000000 tweety_ns-1.1.4/src/tweety/bot.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    98004 2024-04-27 09:42:49.000000 tweety_ns-1.1.4/src/tweety/builder.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 09:52:55.812221 tweety_ns-1.1.4/src/tweety/events/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety_ns-1.1.4/src/tweety/events/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2083 2024-04-27 09:38:42.000000 tweety_ns-1.1.4/src/tweety/events/newmessage.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    22029 2024-04-14 08:52:30.000000 tweety_ns-1.1.4/src/tweety/exceptions_.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2343 2024-04-23 07:03:34.000000 tweety_ns-1.1.4/src/tweety/filters.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    20593 2024-04-27 09:09:11.000000 tweety_ns-1.1.4/src/tweety/http.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2362 2024-04-10 16:34:41.000000 tweety_ns-1.1.4/src/tweety/session.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 09:52:55.812221 tweety_ns-1.1.4/src/tweety/types/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1249 2024-03-20 05:30:39.000000 tweety_ns-1.1.4/src/tweety/types/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3094 2024-04-27 09:46:41.000000 tweety_ns-1.1.4/src/tweety/types/base.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1172 2024-01-20 09:02:27.000000 tweety_ns-1.1.4/src/tweety/types/bookmarks.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3256 2024-01-20 09:00:34.000000 tweety_ns-1.1.4/src/tweety/types/community.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4054 2024-02-22 14:22:03.000000 tweety_ns-1.1.4/src/tweety/types/follow.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      987 2024-01-20 08:43:34.000000 tweety_ns-1.1.4/src/tweety/types/gifs.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    20744 2024-04-27 09:46:46.000000 tweety_ns-1.1.4/src/tweety/types/inbox.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1444 2024-03-03 17:35:17.000000 tweety_ns-1.1.4/src/tweety/types/likes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4302 2024-01-20 08:28:50.000000 tweety_ns-1.1.4/src/tweety/types/lists.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1511 2024-01-19 19:19:11.000000 tweety_ns-1.1.4/src/tweety/types/mentions.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     9022 2024-04-10 16:29:13.000000 tweety_ns-1.1.4/src/tweety/types/n_types.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1351 2024-01-19 19:15:58.000000 tweety_ns-1.1.4/src/tweety/types/notification.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1103 2024-03-20 05:31:04.000000 tweety_ns-1.1.4/src/tweety/types/places.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-01-19 19:12:37.000000 tweety_ns-1.1.4/src/tweety/types/retweets.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3806 2024-02-03 16:37:11.000000 tweety_ns-1.1.4/src/tweety/types/search.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1216 2024-01-31 06:59:29.000000 tweety_ns-1.1.4/src/tweety/types/topic.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    58815 2024-04-14 08:56:44.000000 tweety_ns-1.1.4/src/tweety/types/twDataTypes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12236 2024-04-12 07:15:06.000000 tweety_ns-1.1.4/src/tweety/types/usertweet.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety_ns-1.1.4/src/tweety/updates.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    36810 2024-04-27 09:40:36.000000 tweety_ns-1.1.4/src/tweety/user.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     6586 2024-04-25 11:56:51.000000 tweety_ns-1.1.4/src/tweety/utils.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 09:52:55.816221 tweety_ns-1.1.4/src/tweety_ns.egg-info/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-27 09:52:55.000000 tweety_ns-1.1.4/src/tweety_ns.egg-info/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1026 2024-04-27 09:52:55.000000 tweety_ns-1.1.4/src/tweety_ns.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-04-27 09:52:55.000000 tweety_ns-1.1.4/src/tweety_ns.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-04-27 09:52:55.000000 tweety_ns-1.1.4/src/tweety_ns.egg-info/requires.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-04-27 09:52:55.000000 tweety_ns-1.1.4/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety_ns-1.1.3/PKG-INFO` & `tweety_ns-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.3
+Version: 1.1.4
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety_ns-1.1.3/README.md` & `tweety_ns-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/setup.cfg` & `tweety_ns-1.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tweety-ns
-version = 1.1.3
+version = 1.1.4
 author = Tayyab Kharl
 author_email = tayyabmahr@gmail.com
 description = An easy Twitter Scraper
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mahrtayyab/tweety
 project_urls =
```

### Comparing `tweety_ns-1.1.3/setup.py` & `tweety_ns-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='tweety-ns',
     packages=['tweety', 'tweety.types', 'tweety.events'],
-    version='1.1.3',
+    version='1.1.4',
     license='MIT',
     description='An easy Twitter Scraper',
     author='Tayyab Kharl',
     author_email='tayyabmahr@gmail.com',
     url='https://github.com/mahrtayyab/tweety',
     keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
     install_requires=[
```

### Comparing `tweety_ns-1.1.3/src/tweety/auth.py` & `tweety_ns-1.1.4/src/tweety/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
             return
 
         self.request.set_cookies(str(self.session))
         self.user = self.get_user_info(self.request.username)
         self.request.set_user(self.user)
         self.session.set_session_user(self.user)
         self._is_connected = True
+        self.is_user_authorized = True
         return self.user
 
     def start(
             self,
             username=None,
             password=None,
             *,
```

### Comparing `tweety_ns-1.1.3/src/tweety/bot.py` & `tweety_ns-1.1.4/src/tweety/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import traceback
 import warnings
 from typing import Union
 from .utils import find_objects, AuthRequired, get_user_from_typehead, get_tweet_id, check_translation_lang
 from .types import (Proxy, TweetComments, UserTweets, Search, User, Tweet, Trends, Community, CommunityTweets,
                     CommunityMembers, UserFollowers, UserFollowings, TweetHistory, UserMedia, GifSearch,
                     ShortUser, TypeHeadSearch, TweetTranslate, AudioSpace, UserHighlights, UserLikes, Places)
 from .exceptions_ import *
@@ -36,14 +35,15 @@
             self.session = session_name(self)
         elif isinstance(session_name, FileSession):
             self.session = session_name
         else:
             self.session = FileSession(self, session_name)
 
         self.logged_in = False
+        self.is_user_authorized = False
         self.request = self.http = Request(self, max_retries=10, proxy=self._proxy, **httpx_kwargs)
         self.user = None
 
     def get_user_info(self, username: Union[str, int, list] = None):
         """
         Get the User Info of the specified username
```

### Comparing `tweety_ns-1.1.3/src/tweety/builder.py` & `tweety_ns-1.1.4/src/tweety/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     URL_AUDIO_SPACE_BY_ID = "https://twitter.com/i/api/graphql/gpc0LEdR6URXZ7HOo42_bQ/AudioSpaceById"
     URL_AUDIO_SPACE_STREAM = "https://twitter.com/i/api/1.1/live_video_stream/status/{}"
     URL_TWEET_DETAILS = "https://twitter.com/i/api/graphql/3XDB26fBve-MmjHaWTUZxA/TweetDetail"
     URL_TWEET_ANALYTICS = "https://twitter.com/i/api/graphql/vnwexpl0q33_Bky-SROVww/TweetActivityQuery"
     URL_TWEET_TRANSLATE = "https://twitter.com/i/api/1.1/strato/column/None/tweetId={},destinationLanguage={},translationSource=Some(Google),feature=None,timeout=None,onlyCached=None/translation/service/translateTweet"
     URL_TWEET_DETAILS_AS_GUEST = "https://api.twitter.com/graphql/5GOHgZe-8U2j5sVHQzEm9A/TweetResultByRestId"
     URL_TWEET_HISTORY = "https://twitter.com/i/api/graphql/MYJ08HcXJuxtXMXWMP-63w/TweetEditHistory"
-    URL_AUSER_INBOX = "https://twitter.com/i/api/1.1/dm/user_updates.json"  # noqa
+    URL_AUSER_INITIAL_INBOX = "https://twitter.com/i/api/1.1/dm/inbox_initial_state.json"  # noqa
+    URL_AUSER_INBOX_UPDATES = "https://twitter.com/i/api/1.1/dm/user_updates.json"  # noqa
     URL_AUSER_TRUSTED_INBOX = "https://twitter.com/i/api/1.1/dm/inbox_timeline/trusted.json"  # noqa
     URL_AUSER_NOTIFICATION_MENTIONS = "https://twitter.com/i/api/2/notifications/mentions.json"  # noqa
     URL_AUSER_SETTINGS = "https://api.twitter.com/1.1/account/settings.json"  # noqa
     URL_AUSER_ADD_GROUP_MEMBER = "https://twitter.com/i/api/graphql/oBwyQ0_xVbAQ8FAyG0pCRA/AddParticipantsMutation"  # noqa
     URL_AUSER_SEND_MESSAGE = "https://twitter.com/i/api/1.1/dm/new2.json"  # noqa
     URL_AUSER_CONVERSATION = "https://twitter.com/i/api/1.1/dm/conversation/{}.json"  # noqa
     URL_AUSER_CREATE_TWEET = "https://twitter.com/i/api/graphql/tTsjMKyhajZvK4q76mpIBg/CreateTweet"  # noqa
@@ -618,53 +619,90 @@
 
         if cursor:
             params['cursor'] = cursor
 
         return "GET", self._build(self.URL_AUSER_NOTIFICATION_MENTIONS, urlencode(params))
 
     @return_with_headers
-    def get_inbox(self, cursor, active_conversation=None):
+    def get_initial_inbox(self):
         params = {
-            'nsfw_filtering_enabled': False,
-            'filter_low_quality': True,
+            'nsfw_filtering_enabled': 'false',
+            'filter_low_quality': 'false',
             'include_quality': 'all',
-            'dm_secret_conversations_enabled': False,
-            'krs_registration_enabled': True,
+            'include_profile_interstitial_type': '1',
+            'include_blocking': '1',
+            'include_blocked_by': '1',
+            'include_followed_by': '1',
+            'include_want_retweets': '1',
+            'include_mute_edge': '1',
+            'include_can_dm': '1',
+            'include_can_media_tag': '1',
+            'include_ext_is_blue_verified': '1',
+            'include_ext_verified_type': '1',
+            'include_ext_profile_image_shape': '1',
+            'skip_status': '1',
+            'dm_secret_conversations_enabled': 'false',
+            'krs_registration_enabled': 'true',
             'cards_platform': 'Web-12',
             'include_cards': '1',
-            'include_ext_alt_text': True,
-            'include_ext_limited_action_results': True,
-            'include_quote_count': True,
+            'include_ext_alt_text': 'true',
+            'include_ext_limited_action_results': 'true',
+            'include_quote_count': 'true',
             'include_reply_count': '1',
             'tweet_mode': 'extended',
-            'include_ext_views': True,
-            'dm_users': False,
-            'include_groups': True,
-            'include_inbox_timelines': True,
-            'include_ext_media_color': True,
-            'supports_reactions': True,
-            'include_ext_edit_control': True,
-            'include_ext_business_affiliations_label': True,
-            'ext': 'mediaColor,altText,businessAffiliationsLabel,mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,superFollowMetadata,unmentionInfo,editControl',
+            'include_ext_views': 'true',
+            'dm_users': 'true',
+            'include_groups': 'true',
+            'include_inbox_timelines': 'true',
+            'include_ext_media_color': 'true',
+            'supports_reactions': 'true',
+            'include_ext_edit_control': 'true',
+            'include_ext_business_affiliations_label': 'true',
+            'ext': 'mediaColor,altText,mediaStats,highlightedLabel,voiceInfo,birdwatchPivot,superFollowMetadata,unmentionInfo,editControl,article',
+        }
+
+        return "GET", self._build(self.URL_AUSER_INITIAL_INBOX, urlencode(params))
+
+    @return_with_headers
+    def get_inbox_updates(self, cursor, active_conversation=None):
+        params = {
+            'nsfw_filtering_enabled': 'false',
+            'filter_low_quality': 'false',
+            'include_quality': 'all',
+            'dm_secret_conversations_enabled': 'false',
+            'krs_registration_enabled': 'true',
+            'cards_platform': 'Web-12',
+            'include_cards': '1',
+            'include_ext_alt_text': 'true',
+            'include_ext_limited_action_results': 'true',
+            'include_quote_count': 'true',
+            'include_reply_count': '1',
+            'tweet_mode': 'extended',
+            'include_ext_views': 'true',
+            'dm_users': 'true',
+            'include_groups': 'true',
+            'include_inbox_timelines': 'true',
+            'include_ext_media_color': 'true',
+            'supports_reactions': 'true',
+            'include_ext_edit_control': 'true',
+            'include_ext_business_affiliations_label': 'true',
+            'ext': 'mediaColor,altText,businessAffiliationsLabel,mediaStats,highlightedLabel,voiceInfo,birdwatchPivot,superFollowMetadata,unmentionInfo,editControl,article',
+            'cursor': cursor
         }
 
         if active_conversation:
             params['active_conversation_id'] = active_conversation
 
-        if cursor:
-            params['cursor'] = cursor
-
-        return "GET", self._build(self.URL_AUSER_INBOX, urlencode(params))
+        return "GET", self._build(self.URL_AUSER_INBOX_UPDATES, urlencode(params))
 
     @return_with_headers
-    def get_trusted_inbox(self, max_id):
+    def get_trusted_inbox(self, max_id=None):
         params = {
             'filter_low_quality': True,
             'include_quality': 'all',
-            'max_id': max_id,
             'nsfw_filtering_enabled': False,
             'include_profile_interstitial_type': '1',
             'include_blocking': '1',
             'include_blocked_by': '1',
             'include_followed_by': '1',
             'include_want_retweets': '1',
             'include_mute_edge': '1',
@@ -681,22 +719,24 @@
             'include_cards': '1',
             'include_ext_alt_text': True,
             'include_ext_limited_action_results': True,
             'include_quote_count': True,
             'include_reply_count': '1',
             'tweet_mode': 'extended',
             'include_ext_views': True,
-            'dm_users': False,
+            'dm_users': True,
             'include_groups': True,
             'include_inbox_timelines': True,
             'include_ext_media_color': True,
             'supports_reactions': True,
             'include_ext_edit_control': True,
             'ext': 'mediaColor,altText,mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,superFollowMetadata,unmentionInfo,editControl',
         }
+        if max_id:
+            params['max_id'] = max_id
 
         return "GET", self._build(self.URL_AUSER_TRUSTED_INBOX, urlencode(params))
 
     @return_with_headers
     def get_untrusted_inbox(self, max_id, low_quality=False):
         params = {
             'filter_low_quality': True if not low_quality else False,
@@ -722,15 +762,15 @@
             'include_cards': '1',
             'include_ext_alt_text': True,
             'include_ext_limited_action_results': True,
             'include_quote_count': True,
             'include_reply_count': '1',
             'tweet_mode': 'extended',
             'include_ext_views': True,
-            'dm_users': False,
+            'dm_users': True,
             'include_groups': True,
             'include_inbox_timelines': True,
             'include_ext_media_color': True,
             'supports_reactions': True,
             'include_ext_edit_control': True,
             'ext': 'mediaColor,altText,mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,superFollowMetadata,unmentionInfo,editControl',
         }
```

### Comparing `tweety_ns-1.1.3/src/tweety/events/newmessage.py` & `tweety_ns-1.1.4/src/tweety/events/newmessage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import threading
 import time
 from ..types.inbox import Inbox, Message
 
 
 class NewMessageUpdate:
-    def __init__(self, request, callback):
-        self.request = request
+    def __init__(self, client, callback):
+        self.client = client
         self.callback_func = callback
-        self.inbox = Inbox(self.request.user.id, self.request)
+        self.inbox = Inbox(self.client.user.id, self.client, 1)
+        list(self.inbox.generator())
         self.cursor = self.inbox.cursor
         self.wait_for_message()
 
     class NewMessage:
         def __init__(self, conversation, message):
             self.conversation = conversation
             self.message = message
@@ -20,32 +21,31 @@
             self.sender = self.message.sender
             self.receiver = self.message.receiver
             self.text = self.message.text if hasattr(self.message, "text") else None
             self.time = self.message.time
             self.id = self.message.id
             self.media = self.message.media if hasattr(self.message, "media") else None
 
-        def respond(self, text):
-            return self.conversation.send_message(text)
+        def respond(self, text, file=None):
+            return self.conversation.send_message(text, file)
 
         def __repr__(self):
             return "NewMessage(id={}, sender={}, receiver={}, time={}, text={})".format(
                 self.id, self.sender, self.receiver, self.time, self.text
             )
 
     def wait_for_message(self):
         while True:
-            new_chats = Inbox(None, self.request, cursor=self.cursor)
-            self.cursor = new_chats.cursor
-            if new_chats.conversations:
-                for conv in new_chats.conversations:
+            new_chats = self.inbox.get_new_messages()
+            if new_chats:
+                for conv in new_chats:
                     for message in conv.messages:
                         event = None
                         if isinstance(message, Message):
-                            if not message.sender or str(message.sender.id) != str(self.request.user.id):
+                            if not message.sender or str(message.sender.id) != str(self.client.user.id):
                                 event = self.NewMessage(conv, message)
                         else:
                             event = message
 
                         if event:
                             threading.Thread(target=self.callback_func, args=(event,)).start()
```

### Comparing `tweety_ns-1.1.3/src/tweety/exceptions_.py` & `tweety_ns-1.1.4/src/tweety/exceptions_.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/filters.py` & `tweety_ns-1.1.4/src/tweety/filters.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/http.py` & `tweety_ns-1.1.4/src/tweety/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from urllib.parse import quote
 import httpx
 from .exceptions_ import GuestTokenNotFound, UnknownError, UserNotFound, InvalidCredentials
 from .types.n_types import GenericError
 from .utils import custom_json, GUEST_TOKEN_REGEX
 from .builder import UrlBuilder
 
-httpx.Response.original_json = httpx.Response.json
 httpx.Response.json = custom_json
 
 
 class Request:
     def __init__(self, client, max_retries=10, proxy=None, **kwargs):
 
         timeout = kwargs.pop("timeout", 60)
@@ -68,14 +67,15 @@
                 limit_remaining=int(headers['x-rate-limit-remaining'])
             )
 
     def __get_response__(self, return_raw=False, ignore_none_data=False, is_document=False, **request_data):
 
         response = self.__session.request(**request_data)
         self._update_rate_limit(response, inspect.stack()[1][3])
+
         if is_document:
             return response
 
         response_json = response.json()  # noqa
         if ignore_none_data and len(response.text) == 0:
             return None
 
@@ -241,16 +241,21 @@
         response = self.__get_response__(**self.__builder.bookmark_tweet(tweet_id))
         return response
 
     def delete_bookmark_tweet(self, tweet_id):
         response = self.__get_response__(**self.__builder.delete_tweet_bookmark(tweet_id))
         return response
 
-    def get_inbox(self, user_id, cursor=None):
-        request = self.__builder.get_inbox(cursor)
+    def get_initial_inbox(self):
+        request = self.__builder.get_initial_inbox()
+        response = self.__get_response__(**request)
+        return response
+
+    def get_inbox_updates(self, cursor, active_conversation=None):
+        request = self.__builder.get_inbox_updates(cursor, active_conversation)
         response = self.__get_response__(**request)
         return response
 
     def get_trusted_inbox(self, max_id):
         response = self.__get_response__(**self.__builder.get_trusted_inbox(max_id))
         return response
```

### Comparing `tweety_ns-1.1.3/src/tweety/session.py` & `tweety_ns-1.1.4/src/tweety/session.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/__init__.py` & `tweety_ns-1.1.4/src/tweety/types/__init__.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/base.py` & `tweety_ns-1.1.4/src/tweety/types/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,28 +54,33 @@
 
                 if result.is_retweet and result.retweeted_tweet:
                     self.client._cached_users[str(result.retweeted_tweet.author.username).lower()] = result.retweeted_tweet.author.id
 
         return results
 
     def generator(self):
-        for page in range(1, int(self.pages) + 1):
+        this_page = 0
+        while this_page != int(self.pages):
             results = self.get_next_page()
 
             if len(results) == 0:
                 break
 
             yield self, results
 
             if not self.is_next_page:
                 break
 
-            if page != self.pages:
+            this_page += 1
+
+            if this_page != self.pages:
                 time.sleep(parse_wait_time(self.wait_time))
 
+
+
         return self
 
     def __repr__(self):
         class_name = self.__class__.__name__
         return "{}(user_id={}, count={})".format(
             class_name, self.user_id, self.__len__()
         )
```

### Comparing `tweety_ns-1.1.3/src/tweety/types/bookmarks.py` & `tweety_ns-1.1.4/src/tweety/types/bookmarks.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/community.py` & `tweety_ns-1.1.4/src/tweety/types/community.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/follow.py` & `tweety_ns-1.1.4/src/tweety/types/follow.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/gifs.py` & `tweety_ns-1.1.4/src/tweety/types/gifs.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/inbox.py` & `tweety_ns-1.1.4/src/tweety/types/inbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,171 @@
 import re
 import threading
 import time
+import traceback
 from . import User, Media, URL, Hashtag, ShortUser, Symbol
 from ..utils import parse_time, parse_wait_time
 
 
 class Inbox(dict):
     HAS_MORE_STATUS = "HAS_MORE"
     AT_END_STATUS = "AT_END"
 
-    def __init__(self, user_id, client, cursor=None):
+    def __init__(self, user_id, client, pages, wait_time=2):
         super().__init__()
         self._client = client
-        self._tmp_conv_id = []
+        self._got_initial = False
+        self._inbox_timelines = {}
+        self.pages = pages
+        self.wait_time = wait_time
         self.conversations = []
         self.messages = []
-        self.cursor = cursor
+        self.cursor = None
         self.last_seen_event_id = None
         self.trusted_last_seen_event_id = None
         self.untrusted_last_seen_event_id = None
         self.user_id = user_id
-        self.get_initial()
 
     def _parse_response(self, response):
+        this_page = []
         _initial_inbox = response.get('inbox_initial_state') or response.get('user_events') or response.get('inbox_timeline')
+        _conversations = _initial_inbox.get("conversations", {})
 
-        if _initial_inbox.get('conversations'):
-            for conservation in _initial_inbox['conversations'].values():
-                _conversation = Conversation(conservation, _initial_inbox, self._client)
-                if str(_conversation.id) not in self._tmp_conv_id:
-                    self.conversations.append(_conversation)
+        for conservation in _conversations.values():
+            _conversation = Conversation(conservation, _initial_inbox, self._client)
+            this_page.append(_conversation)
 
-        for conv in self.conversations:
-            self._tmp_conv_id.append(str(conv.id))
+            to_edit = None
+
+            for conv_index, pre_conv in enumerate(self.conversations):
+                if str(pre_conv.id) == str(_conversation.id):
+                    to_edit = conv_index
+                    break
+
+            if to_edit:
+                self.conversations.insert(to_edit, _conversation)
+            else:
+                self.conversations.append(_conversation)
 
-        return _initial_inbox or {}
+        self._parse_messages(this_page)
+        return this_page, _initial_inbox
 
-    def get_initial(self):
-        _threads = []
-        response = self._client.http.get_inbox(self.user_id, cursor=self.cursor)
+    def get_page(self, min_entry_id=None, page_type="trusted"):
+        if not self._got_initial:
+            if not self.cursor:
+                response = self._client.http.get_initial_inbox()
+            else:
+                response = self._client.http.get_inbox_updates(cursor=self.cursor)
 
-        _initial_inbox = self._parse_response(response)
+            page, inbox = self._parse_response(response)
+            self.cursor = self['cursor'] = inbox.get('cursor')
+            self.last_seen_event_id = self['last_seen_event_id'] = inbox.get('last_seen_event_id')
+            self.trusted_last_seen_event_id = self['trusted_last_seen_event_id'] = inbox.get('trusted_last_seen_event_id')
+            self.untrusted_last_seen_event_id = self['untrusted_last_seen_event_id'] = inbox.get('untrusted_last_seen_event_id')
 
-        self.cursor = self['cursor'] = _initial_inbox.get('cursor')
-        self.last_seen_event_id = self['last_seen_event_id'] = _initial_inbox.get('last_seen_event_id')
-        self.trusted_last_seen_event_id = self['trusted_last_seen_event_id'] = _initial_inbox.get('trusted_last_seen_event_id')
-        self.untrusted_last_seen_event_id = self['untrusted_last_seen_event_id'] = _initial_inbox.get('untrusted_last_seen_event_id')
+            if inbox.get("inbox_timelines"):
+                self._inbox_timelines = inbox.get("inbox_timelines", {})
 
-        if _initial_inbox.get("inbox_timelines"):
-            for key, value in _initial_inbox['inbox_timelines'].items():
-                new_thread = threading.Thread(target=self.get_more, args=(value,))
-                _threads.append(new_thread)
-                new_thread.start()
+            self._got_initial = True
+            return page, self.cursor, None
+        else:
+            if page_type not in ("trusted", "untrusted"):
+                page_type = "trusted"
 
-            for _ in _threads:
-                _.join()
+            if not min_entry_id:
+                raise ValueError("'min_entry_id' is required after initial request.")
 
-        self._parse_messages()
-        return self, self.conversations
+            if page_type == "untrusted":
+                response = self._client.http.get_untrusted_inbox(min_entry_id)
+            else:
+                response = self._client.http.get_trusted_inbox(min_entry_id)
 
-    def _parse_messages(self):
-        for conv in self.conversations:
+            page, inbox = self._parse_response(response)
+
+            return page, inbox.get('min_entry_id', 0), inbox.get('status', self.AT_END_STATUS)
+
+    def get_new_messages(self, cursor=None):
+        if not cursor:
+            cursor = self.cursor
+
+        response = self._client.http.get_inbox_updates(cursor=cursor)
+        page, inbox = self._parse_response(response)
+        self.cursor = self['cursor'] = inbox.get('cursor')
+        self.last_seen_event_id = self['last_seen_event_id'] = inbox.get('last_seen_event_id')
+        self.trusted_last_seen_event_id = self['trusted_last_seen_event_id'] = inbox.get('trusted_last_seen_event_id')
+        self.untrusted_last_seen_event_id = self['untrusted_last_seen_event_id'] = inbox.get('untrusted_last_seen_event_id')
+
+        if inbox.get("inbox_timelines"):
+            self._inbox_timelines = inbox.get("inbox_timelines", {})
+
+        return page
+
+    def get_next_page(self):
+        if not self._got_initial:
+            page, cursor, _ = self.get_page()
+            self.cursor = self['cursor'] = cursor
+            return page
+        else:
+            page_type = "trusted"
+
+            if self._inbox_timelines[page_type]['status'] == self.AT_END_STATUS:
+                page_type = "untrusted"
+
+            page_attrs = self._inbox_timelines.get(page_type, {})
+            min_entry_id = page_attrs.get('min_entry_id', 0)
+            status = page_attrs.get('status', self.AT_END_STATUS)
+
+            if status == self.AT_END_STATUS:
+                return []
+
+            page, new_min_entry_id, new_status = self.get_page(min_entry_id=min_entry_id, page_type=page_type)
+            self._inbox_timelines[page_type]["min_entry_id"] = new_min_entry_id
+            self._inbox_timelines[page_type]["status"] = new_status
+            return page
+
+    def generator(self):
+        this_page = 0
+        while this_page != int(self.pages):
+            results = self.get_next_page()
+
+            if len(results) == 0:
+                break
+
+            yield self, results
+
+            this_page += 1
+            if this_page != self.pages:
+                time.sleep(parse_wait_time(self.wait_time))
+
+        return self
+
+    def _parse_messages(self, conversations):
+        for conv in conversations:
             for message in conv.messages:
                 self.messages.append(message)
 
         self['conversations'] = self.conversations
         self['messages'] = self.messages
 
-    def get_more(self, status):
-        stage = status.get('status', self.AT_END_STATUS)
-        min_entry_id = status.get('min_entry_id', 0)
-        while stage != self.AT_END_STATUS:
-            response = self._client.http.get_trusted_inbox(min_entry_id)
-            inbox = self._parse_response(response)
-            min_entry_id = inbox.get('min_entry_id', 0)
-            stage = inbox.get('status', self.AT_END_STATUS)
-
     def get_conversation(self, conversation_id):
         for conv in self.conversations:
             if str(conv.id) == conversation_id:
                 return conv
 
         return None
 
     def __getitem__(self, index):
         if isinstance(index, str):
             return getattr(self, index)
 
         return self.conversations[index]
 
     def __iter__(self):
-        for __tweet in self.conversations:
-            yield __tweet
+        for _conversation_ in self.conversations:
+            yield _conversation_
 
     def __len__(self):
         return len(self.conversations)
 
     def __repr__(self):
         return f"Inbox(user_id={self.user_id}, count={self.__len__()})"
 
@@ -137,21 +207,24 @@
                     return participant.name
         return ""
 
     def get_participants(self):
         users = []
         participants = self._raw['participants']
         for participant in participants:
-            this_user = None
             try:
                 user = self._inbox['users'].get(str(participant['user_id']))
+
                 if user:
                     user['__typename'] = "User"
                     this_user = User(self._client, user)
+                else:
+                    this_user = str(participant["user_id"])
             except Exception as e:
+                traceback.print_exc()
                 this_user = str(participant["user_id"])
 
             if participant.get("is_admin") is True:
                 self.admin = this_user
 
             users.append(this_user)
 
@@ -159,21 +232,30 @@
 
     def _get_key(self, keyName, default=None):
         return self._raw.get(keyName, default)
 
     def _parse_message(self, entry):
         if entry.get('message') and str(entry['message']['conversation_id']) == str(self.id):
             return Message(entry['message'], self._inbox, self._client)
+        elif entry.get('welcome_message_create') and str(entry['welcome_message_create']['conversation_id']) == str(self.id):
+            return Message(entry['welcome_message_create'], self._inbox, self._client)
         elif entry.get('participants_join') and str(entry['participants_join']['conversation_id']) == str(self.id):
             return MessageParticipantUpdate(
                 'participants_join',
                 entry.get('participants_join'),
                 self._inbox,
                 self._client
             )
+        elif entry.get('join_conversation') and str(entry['join_conversation']['conversation_id']) == str(self.id):
+            return MessageParticipantUpdate(
+                'participants_join',
+                entry.get('join_conversation'),
+                self._inbox,
+                self._client
+            )
         elif entry.get('participants_leave') and str(entry['participants_leave']['conversation_id']) == str(self.id):
             return MessageParticipantUpdate(
                 'participants_leave',
                 entry.get('participants_leave'),
                 self._inbox,
                 self._client
             )
@@ -360,18 +442,18 @@
         self._entities = self._get_message_data('entities', {})
         self.conversation_id = self['conversation_id'] = self._raw.get('conversation_id')
         self.id = self['id'] = self._raw.get('id')
         self.epoch_time = self['epoch_time'] = self._get_message_data('time')
         self.time = self['time'] = parse_time(self.epoch_time)
         self.request_id = self['request_id'] = self._raw.get('request_id')
         self.text = self['text'] = self._get_text()
-        self.receiver_id = self._get_message_data('recipient_id')
+        self.receiver_id = self._client.user.id
         self.sender_id = self._get_message_data("sender_id")
-        self.receiver = self['receiver'] = self.get_recipient(self.receiver_id)
-        self.sender = self['sender'] = self.get_recipient(self.sender_id)
+        self.receiver = self['receiver'] = self._client.user
+        self.sender = self['sender'] = self.get_recipient("sender_id")
         self.media = self['media'] = self._get_media()
         self.urls = self['urls'] = self._get_urls()
         self.symbols = self['symbols'] = self._get_symbols()
         self.hashtags = self['hashtags'] = self._get_hashtags()
         self.user_mentions = self['user_mentions'] = self._get_user_mentions()
 
     def _get_urls(self):
@@ -387,14 +469,15 @@
         return [ShortUser(self._client, i) for i in self._entities.get('user_mentions', [])]
 
     def _get_message_data(self, dataKey, default=None):
         return self._raw['message_data'].get(dataKey, default)
 
     def get_recipient(self, target):
         user = self._get_message_data(target)
+
         if not user:
             return None
 
         user = self._inbox.get('users', {}).get(str(user))
         if user:
             user['__typename'] = "User"
             return User(self._client, user)
```

### Comparing `tweety_ns-1.1.3/src/tweety/types/likes.py` & `tweety_ns-1.1.4/src/tweety/types/likes.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/lists.py` & `tweety_ns-1.1.4/src/tweety/types/lists.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/mentions.py` & `tweety_ns-1.1.4/src/tweety/types/mentions.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/n_types.py` & `tweety_ns-1.1.4/src/tweety/types/n_types.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/notification.py` & `tweety_ns-1.1.4/src/tweety/types/notification.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/places.py` & `tweety_ns-1.1.4/src/tweety/types/places.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/retweets.py` & `tweety_ns-1.1.4/src/tweety/types/retweets.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/search.py` & `tweety_ns-1.1.4/src/tweety/types/search.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/topic.py` & `tweety_ns-1.1.4/src/tweety/types/topic.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/twDataTypes.py` & `tweety_ns-1.1.4/src/tweety/types/twDataTypes.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/types/usertweet.py` & `tweety_ns-1.1.4/src/tweety/types/usertweet.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.3/src/tweety/user.py` & `tweety_ns-1.1.4/src/tweety/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,29 +329,43 @@
         notifications = TweetNotifications(self.me.id, self, pages, wait_time, cursor)
 
         return notifications.generator()
 
     def get_inbox(
             self,
             user_id: Union[int, str, User] = None,
-            cursor: str = None
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
     ) -> Inbox:
         """
-        :param user_id : (`str`, `int`, `User`) User id or username of the user whom to get the messages of. Default is ALL
-        :param cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-                                It is used to get the messages updates
+        :param user_id : (`str`, `int`, `User`) Not Implemented
+        :param pages: (`int`) The number of pages to get
+        :param wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
         :return:
         """
 
-        if user_id:
-            user_id = self._get_user_id(user_id)
+        inbox = Inbox(self.user.id, self, pages, wait_time)
+        list(inbox.generator())
+        return inbox
 
-        inbox = Inbox(user_id, self, cursor)
+    def iter_inbox(
+            self,
+            user_id: Union[int, str, User] = None,
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
+    ) -> Inbox:
+        """
+        :param user_id : (`str`, `int`, `User`) Not Implemented
+        :param pages: (`int`) The number of pages to get
+        :param wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :return:
+        """
 
-        return inbox
+        inbox = Inbox(self.user.id, self, pages, wait_time)
+        return inbox.generator()
 
     def add_member_to_group(
             self,
             members: Union[str, int, list],
             group_id: Union[str, int, Conversation]
     ):
```

### Comparing `tweety_ns-1.1.3/src/tweety/utils.py` & `tweety_ns-1.1.4/src/tweety/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import base64
 import datetime
 import hashlib
 import inspect
+import json
 import os.path
 import random
 import re
 import string
 import sys
+import traceback
 import uuid
 from dateutil import parser as date_parser
 from urllib.parse import urlparse
 from .exceptions_ import AuthenticationRequired
 from .filters import Language
 
 GUEST_TOKEN_REGEX = re.compile("gt=(.*?);")
@@ -71,17 +73,17 @@
 
     if isinstance(wait_time, (tuple, list)):
         return random.randint(*wait_time)
 
     return int(wait_time)
 
 
-def custom_json(self):
+def custom_json(self, **kwargs):
     try:
-        return self.original_json()
+        return json.loads(self.content, **kwargs)
     except:
         return None
 
 
 def create_request_id():
     return str(uuid.uuid1())
```

### Comparing `tweety_ns-1.1.3/src/tweety_ns.egg-info/PKG-INFO` & `tweety_ns-1.1.4/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.3
+Version: 1.1.4
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety_ns-1.1.3/src/tweety_ns.egg-info/SOURCES.txt` & `tweety_ns-1.1.4/src/tweety_ns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

