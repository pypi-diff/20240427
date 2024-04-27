# Comparing `tmp/otpcr-7.tar.gz` & `tmp/otpcr-8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otpcr-7.tar", last modified: Wed Apr 24 23:08:22 2024, max compression
+gzip compressed data, was "otpcr-8.tar", last modified: Sat Apr 27 14:21:51 2024, max compression
```

## Comparing `otpcr-7.tar` & `otpcr-8.tar`

### file list

```diff
@@ -1,62 +1,58 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 23:08:22.337195 otpcr-7/
--rw-r--r--   0 bart      (1000) bart      (1000)     2395 2024-04-24 23:08:22.333196 otpcr-7/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1868 2024-04-24 18:38:19.000000 otpcr-7/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 23:08:22.329195 otpcr-7/docs/
--rw-r--r--   0 bart      (1000) bart      (1000)     3451 2024-04-24 18:38:19.000000 otpcr-7/docs/MANUAL.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 23:08:22.329195 otpcr-7/files/
--rw-r--r--   0 bart      (1000) bart      (1000)   225470 2024-04-24 18:38:19.000000 otpcr-7/files/EM_Ack_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   238330 2024-04-24 18:38:19.000000 otpcr-7/files/EM_T04_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   236671 2024-04-24 18:38:19.000000 otpcr-7/files/EM_T07_OTP-CR-117_19_001.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)  1685507 2023-06-10 19:59:00.000000 otpcr-7/files/bevestigd.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    50044 2023-06-10 19:59:02.000000 otpcr-7/files/bevestigd.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)    69979 2023-06-10 19:59:02.000000 otpcr-7/files/informed.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)     7738 2024-04-24 20:30:12.000000 otpcr-7/files/otpcrsmile.png
--rw-r--r--   0 bart      (1000) bart      (1000)    56642 2024-04-24 20:30:12.000000 otpcr-7/files/otpcrwall.png
--rw-r--r--   0 bart      (1000) bart      (1000)   242205 2024-04-24 18:38:19.000000 otpcr-7/files/verbatim5.png
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 23:08:22.333196 otpcr-7/otpcr/
--rw-r--r--   0 bart      (1000) bart      (1000)     1220 2024-04-24 18:38:19.000000 otpcr-7/otpcr/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4325 2024-04-24 20:29:24.000000 otpcr-7/otpcr/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      654 2024-04-24 18:38:19.000000 otpcr-7/otpcr/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3863 2024-04-24 18:38:19.000000 otpcr-7/otpcr/client.py
--rw-r--r--   0 bart      (1000) bart      (1000)      276 2024-04-24 18:38:19.000000 otpcr-7/otpcr/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)      232 2024-04-24 18:38:19.000000 otpcr-7/otpcr/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1223 2024-04-24 18:38:19.000000 otpcr-7/otpcr/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)      762 2024-04-24 18:38:19.000000 otpcr-7/otpcr/event.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1904 2024-04-24 18:38:19.000000 otpcr-7/otpcr/find.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1352 2024-04-24 18:38:19.000000 otpcr-7/otpcr/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 23:08:22.333196 otpcr-7/otpcr/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      423 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      213 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      376 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      425 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      841 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    18951 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      805 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3641 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17429 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)      238 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2408 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)    11003 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3211 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/rst.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1252 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1020 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5322 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3186 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5784 2024-04-24 18:38:19.000000 otpcr-7/otpcr/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6139 2024-04-24 18:38:19.000000 otpcr-7/otpcr/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)      748 2024-04-24 18:38:19.000000 otpcr-7/otpcr/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)      226 2024-04-24 18:38:19.000000 otpcr-7/otpcr/repeater.py
--rw-r--r--   0 bart      (1000) bart      (1000)      109 2024-04-24 18:38:19.000000 otpcr-7/otpcr/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1871 2024-04-24 18:38:19.000000 otpcr-7/otpcr/thread.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1036 2024-04-24 18:38:19.000000 otpcr-7/otpcr/timer.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1093 2024-04-24 18:38:19.000000 otpcr-7/otpcr/workdir.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 23:08:22.333196 otpcr-7/otpcr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2395 2024-04-24 23:08:22.000000 otpcr-7/otpcr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1102 2024-04-24 23:08:22.000000 otpcr-7/otpcr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-24 23:08:22.000000 otpcr-7/otpcr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       49 2024-04-24 23:08:22.000000 otpcr-7/otpcr.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        6 2024-04-24 23:08:22.000000 otpcr-7/otpcr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-24 23:08:22.000000 otpcr-7/otpcr.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)     1152 2024-04-24 20:30:56.000000 otpcr-7/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-24 23:08:22.337195 otpcr-7/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-24 18:38:19.000000 otpcr-7/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.433202 otpcr-8/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2496 2024-04-27 14:21:51.433202 otpcr-8/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1868 2024-04-26 20:04:47.000000 otpcr-8/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.425202 otpcr-8/docs/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3722 2024-04-27 11:24:31.000000 otpcr-8/docs/MANUAL.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.425202 otpcr-8/files/
+-rw-r--r--   0 bart      (1000) bart      (1000)   225470 2024-04-26 20:04:47.000000 otpcr-8/files/EM_Ack_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   238330 2024-04-26 20:04:47.000000 otpcr-8/files/EM_T04_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   236671 2024-04-26 20:04:47.000000 otpcr-8/files/EM_T07_OTP-CR-117_19_001.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)  1685507 2024-04-26 20:04:47.000000 otpcr-8/files/bevestigd.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    50044 2024-04-26 20:04:47.000000 otpcr-8/files/bevestigd.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)    69979 2024-04-26 20:04:47.000000 otpcr-8/files/informed.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   242205 2024-04-26 20:04:47.000000 otpcr-8/files/verbatim5.png
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.429202 otpcr-8/otpcr/
+-rw-r--r--   0 bart      (1000) bart      (1000)       53 2024-04-26 20:04:47.000000 otpcr-8/otpcr/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4795 2024-04-27 14:14:13.000000 otpcr-8/otpcr/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      704 2024-04-26 22:47:25.000000 otpcr-8/otpcr/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4002 2024-04-26 20:04:47.000000 otpcr-8/otpcr/client.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      581 2024-04-27 14:13:19.000000 otpcr-8/otpcr/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      285 2024-04-26 20:04:47.000000 otpcr-8/otpcr/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1397 2024-04-27 12:24:03.000000 otpcr-8/otpcr/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      813 2024-04-26 20:04:47.000000 otpcr-8/otpcr/event.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2008 2024-04-26 20:04:47.000000 otpcr-8/otpcr/find.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1405 2024-04-26 20:04:47.000000 otpcr-8/otpcr/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.429202 otpcr-8/otpcr/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      311 2024-04-27 14:15:12.000000 otpcr-8/otpcr/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      216 2024-04-27 14:12:24.000000 otpcr-8/otpcr/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      344 2024-04-27 12:21:57.000000 otpcr-8/otpcr/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      372 2024-04-27 11:40:49.000000 otpcr-8/otpcr/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      764 2024-04-27 11:41:03.000000 otpcr-8/otpcr/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    18837 2024-04-27 12:41:01.000000 otpcr-8/otpcr/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      706 2024-04-27 11:41:44.000000 otpcr-8/otpcr/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3577 2024-04-27 11:42:03.000000 otpcr-8/otpcr/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      183 2024-04-27 11:42:13.000000 otpcr-8/otpcr/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2354 2024-04-27 11:42:25.000000 otpcr-8/otpcr/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    10834 2024-04-27 14:11:08.000000 otpcr-8/otpcr/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3169 2024-04-26 20:04:47.000000 otpcr-8/otpcr/modules/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1159 2024-04-27 14:11:44.000000 otpcr-8/otpcr/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      988 2024-04-27 11:43:30.000000 otpcr-8/otpcr/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5200 2024-04-27 11:44:01.000000 otpcr-8/otpcr/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3062 2024-04-27 14:10:56.000000 otpcr-8/otpcr/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6085 2024-04-27 12:21:16.000000 otpcr-8/otpcr/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      278 2024-04-26 20:04:47.000000 otpcr-8/otpcr/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      161 2024-04-27 12:54:45.000000 otpcr-8/otpcr/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1956 2024-04-26 20:04:47.000000 otpcr-8/otpcr/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1085 2024-04-26 20:04:47.000000 otpcr-8/otpcr/timer.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1120 2024-04-27 11:55:38.000000 otpcr-8/otpcr/whitelist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1266 2024-04-27 10:40:11.000000 otpcr-8/otpcr/workdir.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.429202 otpcr-8/otpcr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2496 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1021 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       49 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        6 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)     1197 2024-04-27 14:04:29.000000 otpcr-8/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-27 14:21:51.433202 otpcr-8/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-26 20:04:47.000000 otpcr-8/setup.py
```

### Comparing `otpcr-7/PKG-INFO` & `otpcr-8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: otpcr
-Version: 7
-Summary: OTP-CR-117/19
+Version: 8
+Summary: The 117 communication record of the year 2019 to the Office of the Prosecutor of the International Criminal Court.
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/otpcr
 Project-URL: bugs, https://github.com/xobjectz/otpcr/issues
 Project-URL: source, https://github.com/xobjectz/otpcr
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
```

### Comparing `otpcr-7/README.rst` & `otpcr-8/README.rst`

 * *Files identical despite different names*

### Comparing `otpcr-7/docs/MANUAL.rst` & `otpcr-8/docs/MANUAL.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 NAME
 
 ::
 
-    OTPCR - 117/19
+    OTPCR - The 117 communication record of the year 2019 to the Office
+            of the Prosecutor of the International Criminal Court.
 
 
 SYNOPSIS
 
 ::
 
     otpcr <cmd> [key=val] [key==val]
@@ -45,27 +46,65 @@
     OTPCR has a demo bot, it can connect to IRC, fetch and display RSS
     feeds, take todo notes, keep a shopping list and log text. You can
     also copy/paste the service file and run it under systemd for 24/7
     presence in a IRC channel.
 
     OTPCR is Public Domain.
 
+
+INSTALL
+
+::
+
+    use pipx to install otpcr as a local installed program
+
+    $ pipx install otpcr
+    $ pipx ensurepath
+    $ mkdir ~/.otpcr
+
+
+CONFIGURATION
+
+::
+
+    $ otpcr cfg 
+    channel=#otpcr commands=True nick=otpcr port=6667 server=localhost
+
+    irc
+
+    $ otpcr cfg server=<server>
+    $ otpcr cfg channel=<channel>
+    $ otpcr cfg nick=<nick>
+
+    sasl
+
+    $ otpcr pwd <nsvnick> <nspass>
+    $ otpcr cfg password=<frompwd>
+
+    rss
+
+    $ otpcr rss <url>
+    $ otpcr dpl <url> <item1,item2>
+    $ otpcr rem <url>
+    $ otpcr nme <url> <name>
+
+
 USAGE
 
 ::
 
     without any argument the program does nothing
 
     $ otpcr
     $
 
     see list of commands
 
     $ otpcr cmd
-    cmd,err,mod,req,thr,ver
+    cfg,cmd,dne,dpl,exp,log,mre,nme,pwd,rem,req,res,rss,tdo,ver
 
     list of modules
 
     $ otpcr mod
     cmd,err,fnd,irc,log,mod,req,rss,tdo,thr
 
     use -c to start a console
@@ -80,39 +119,14 @@
     use -v for verbose
 
     $ otpcr -cv mod=irc
     OTPCR started CV started Sat Dec 2 17:53:24 2023
     >
 
 
-CONFIGURATION
-
-::
-
-    $ otpcr cfg 
-    channel=#otpcr commands=True nick=otpcr port=6667 server=localhost
-
-    irc
-
-    $ otpcr cfg server=<server>
-    $ otpcr cfg channel=<channel>
-    $ otpcr cfg nick=<nick>
-
-    sasl
-
-    $ otpcr pwd <nsvnick> <nspass>
-    $ otpcr cfg password=<frompwd>
-
-    rss
-
-    $ otpcr rss <url>
-    $ otpcr dpl <url> <item1,item2>
-    $ otpcr rem <url>
-    $ otpcr nme <url> <name>
-
 COMMANDS
 
 ::
 
     cmd - commands
     cfg - irc configuration
     dlt - remove a user
@@ -122,20 +136,22 @@
     met - add a user
     mre - displays cached output
     pwd - sasl nickserv name/pass
     rem - removes a rss feed
     rss - add a feed
     thr - show the running threads
 
+
 SYSTEMD
 
-::
 
-    save the following it in /etc/systemd/system/otpcr.service and
-    replace "<user>" with the user running pipx
+save the following it in /etc/systemd/system/otpcr.service and
+replace "<user>" with the user running pipx
+
+::
 
     [Unit]
     Description=OTP-CR-117/19
     Requires=network-online.target
     After=network-online.target
 
     [Service]
@@ -145,20 +161,22 @@
     WorkingDirectory=/home/<user>/.otpcr
     ExecStart=/home/<user>/.local/pipx/venvs/otpcr/bin/otpcr -d
     RemainAfterExit=yes
 
     [Install]
     WantedBy=default.target
 
-    then run this
+then run this
+
+::
 
-    $ mkdir ~/.otpcr
     $ sudo systemctl enable otpcr --now
 
-    default channel/server is #otpcr on localhost
+
+default channel/server is #otpcr on localhost
 
 FILES
 
 ::
 
     ~/.otpcr
     ~/.local/bin/otpcr
```

### Comparing `otpcr-7/files/EM_Ack_OTP-CR-117_19.pdf` & `otpcr-8/files/EM_Ack_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `otpcr-7/files/EM_T04_OTP-CR-117_19.pdf` & `otpcr-8/files/EM_T04_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `otpcr-7/files/EM_T07_OTP-CR-117_19_001.pdf` & `otpcr-8/files/EM_T07_OTP-CR-117_19_001.pdf`

 * *Files identical despite different names*

### Comparing `otpcr-7/files/bevestigd.jpg` & `otpcr-8/files/bevestigd.jpg`

 * *Files identical despite different names*

### Comparing `otpcr-7/files/bevestigd.pdf` & `otpcr-8/files/bevestigd.pdf`

 * *Files identical despite different names*

### Comparing `otpcr-7/files/informed.jpg` & `otpcr-8/files/informed.jpg`

 * *Files identical despite different names*

### Comparing `otpcr-7/files/verbatim5.png` & `otpcr-8/files/verbatim5.png`

 * *Files identical despite different names*

### Comparing `otpcr-7/otpcr/__main__.py` & `otpcr-8/otpcr/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=W0212
-# ruff: noqa: E402
 
 
 "main"
 
 
 import getpass
 import os
@@ -13,32 +10,35 @@
 import readline
 import sys
 import termios
 import time
 
 
 from .client  import Client, cmnd, parse_cmd, spl
-from .command import Command
 from .default import Default
-from .errors  import debug, enable, errors
+from .errors  import debug, enable, errors, later
 from .event   import Event
 from .object  import cdir
 from .runtime import broker
 from .workdir import Workdir, skel
 
 
+from .command   import scan as scancmd
+from .whitelist import scan as scancls
+
+
 from . import modules
 
 
 Cfg             = Default()
-Cfg.dis         = "mbx,mdl,rst,udp"
-Cfg.mod         = "cmd,mod"
+Cfg.dis         = ""
+Cfg.mod         = ""
 Cfg.opts        = ""
-Cfg.name        = "otpcr"
-Cfg.version     = "6"
+Cfg.name        = __file__.split(os.sep)[-2]
+Cfg.version     = "8"
 Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
 Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
 
 
 Workdir.workdir = Cfg.wdr
 
 
@@ -73,14 +73,15 @@
         "print to console"
         txt = txt.encode('utf-8', 'replace').decode()
         print(txt)
 
 
 def daemon(pidfile, verbose=False):
     "switch to background."
+    # pylint: disable=W0212
     pid = os.fork()
     if pid != 0:
         os._exit(0)
     os.setsid()
     pid2 = os.fork()
     if pid2 != 0:
         os._exit(0)
@@ -106,16 +107,33 @@
     for modname in spl(modstr):
         if skip(modname, disable):
             continue
         module = getattr(pkg, modname, None)
         if not module:
             continue
         if "init" in dir(module):
-            module.init()
-            mds.append(module)
+            try:
+                module.init()
+                mds.append(module)
+            except Exception as ex: # pylint: disable=W0718
+                later(ex)
+    return mds
+
+
+def scan(pkg, modstr, disable=""):
+    "scan modules for commands and classes"
+    mds = []
+    for modname in spl(modstr):
+        if skip(modname, disable):
+            continue
+        module = getattr(pkg, modname, None)
+        if not module:
+            continue
+        scancmd(module)
+        scancls(module)
     return mds
 
 
 def privileges(username):
     "drop privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
@@ -149,24 +167,23 @@
 def ver(event):
     "show version."
     event.reply(f"{Cfg.name.upper()} {Cfg.version}")
 
 
 def main():
     "main"
-    Command.add(ver)
     enable(print)
     skel()
     parse_cmd(Cfg, " ".join(sys.argv[1:]))
     if Cfg.sets.dis:
         Cfg.dis += "," + Cfg.sets.dis
-    if 'a' in Cfg.opts:
-        Cfg.mod = ",".join(modules.__dir__())
+    Cfg.mod = ",".join(modules.__dir__())
     if "v" in Cfg.opts:
         debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
+    scan(modules, Cfg.mod, Cfg.dis)
     if "h" in Cfg.opts:
         print(__doc__)
     elif "d" in Cfg.opts:
         Cfg.mod = ",".join(modules.__dir__())
         Cfg.user = getpass.getuser()
         daemon(Cfg.pidfile, "v" in Cfg.opts)
         privileges(Cfg.user)
```

### Comparing `otpcr-7/otpcr/broker.py` & `otpcr-8/otpcr/broker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-#
 
 
 "broker"
 
 
 from .object import Object, keys
 
@@ -31,7 +29,13 @@
     def get(self, orig):
         "return object by origin (repr)"
         return getattr(self.objs, orig, None)
 
     def remove(self, obj):
         "remove object from broker"
         delattr(self.objs, rpr(obj))
+
+
+def __dir__():
+    return (
+        'Broker',
+    )
```

### Comparing `otpcr-7/otpcr/client.py` & `otpcr-8/otpcr/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=W0718
 
 
 "client"
 
 
 from .command import Command
 from .default import Default
@@ -53,15 +51,15 @@
 def command(bot, evt):
     "check for and run a command."
     parse_cmd(evt)
     func = getattr(Command.cmds, evt.cmd, None)
     if func:
         try:
             func(evt)
-        except Exception as exc:
+        except Exception as exc: # pylint: disable=W0718
             later(exc)
     bot.show(evt)
     evt.ready()
 
 
 def laps(seconds, short=True):
     "show elapsed time."
@@ -160,7 +158,18 @@
 def spl(txt):
     "split comma separated string into a list."
     try:
         res = txt.split(',')
     except (TypeError, ValueError):
         res = txt
     return [x for x in res if x]
+
+
+def __dir__():
+    return (
+        'Client',
+        'cmnd',
+        'command',
+        'lapse',
+        'parse_cmd',
+        'spl'
+    )
```

### Comparing `otpcr-7/otpcr/event.py` & `otpcr-8/otpcr/event.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=R0902
 
 
 "event"
 
 
 import threading
 
 
 from .default import Default
 
 
-class Event(Default):
+class Event(Default): # pylint: disable=R0902
 
     "Event"
 
     def __init__(self):
         Default.__init__(self)
         self._thr    = None
         self._ready  = threading.Event()
@@ -36,7 +34,13 @@
 
     def wait(self):
         "wait for event to be ready."
         if self._thr:
             self._thr.join()
         self._ready.wait()
         return self.result
+
+
+def __dir__():
+    return (
+        'Event',
+    )
```

### Comparing `otpcr-7/otpcr/find.py` & `otpcr-8/otpcr/find.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # This file is placed in the Public Domain.
-#
-#
 
 
 "locate"
 
 
 import os
 import time
 
 
-from .default import Default
-from .object  import fqn, search, update
-from .persist import long
-from .workdir import fetch, store, strip
+from .default   import Default
+from .object    import fqn, search, update
+from .whitelist import long
+from .workdir   import fetch, store, strip
 
 
 def fns(mtc=""):
     "show list of files."
     dname = ''
     pth = store(mtc)
     for rootdir, dirs, _files in os.walk(pth, topdown=False):
@@ -71,7 +69,16 @@
                    )
     res = None
     if result:
         inp = result[-1]
         update(obj, inp[-1])
         res = inp[0]
     return res
+
+
+def __dir__():
+    return (
+        'fns',
+        'fntime',
+        'find',
+        'last'
+    )
```

### Comparing `otpcr-7/otpcr/handler.py` & `otpcr-8/otpcr/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=W0212
 
 
 "handler"
 
 
 import queue
 import threading
@@ -27,15 +25,15 @@
 
     def callback(self, evt):
         "call callback based on event type."
         func = getattr(self.cbs, evt.type, None)
         if not func:
             evt.ready()
             return
-        evt._thr = launch(func, self, evt)
+        evt._thr = launch(func, self, evt) # pylint: disable=W0212
 
     def loop(self):
         "proces events until interrupted."
         while not self.stopped.is_set():
             try:
                 evt = self.poll()
                 self.callback(evt)
@@ -57,7 +55,13 @@
     def start(self):
         "start the event loop."
         launch(self.loop)
 
     def stop(self):
         "stop the event loop."
         self.stopped.set()
+
+
+def __dir__():
+    return (
+        'Handler',
+    )
```

### Comparing `otpcr-7/otpcr/modules/fnd.py` & `otpcr-8/otpcr/modules/fnd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0611,E0402
 
 
 "locate"
 
 
-from ..command import Command
-from ..find    import find
-from ..object  import fmt
-from ..persist import long
-from ..workdir import liststore, skel
+from ..find      import find
+from ..object    import fmt
+from ..whitelist import long
+from ..workdir   import liststore, skel
 
 
 def fnd(event):
     "locate objects."
     skel()
     if not event.rest:
         res = sorted([x.split('.')[-1].lower() for x in liststore()])
@@ -30,10 +27,7 @@
                 clz = fnm
     nmr = 0
     for fnm, obj in find(clz, event.gets):
         event.reply(f"{nmr} {fmt(obj)}")
         nmr += 1
     if not nmr:
         event.reply("no result")
-
-
-#Command.add(fnd)
```

### Comparing `otpcr-7/otpcr/modules/irc.py` & `otpcr-8/otpcr/modules/irc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0718
-# ruff: noqa: F841
 
 
 "internet relay chat"
 
 
 import base64
 import os
@@ -14,29 +11,27 @@
 import ssl
 import textwrap
 import threading
 import time
 import _thread
 
 
-from ..client  import Client, command
-from ..command import Command
-from ..default import Default
-from ..event   import Event
-from ..errors  import Errors, debug, later
-from ..find    import last
-from ..object  import Object, edit, fmt, keys, values
-from ..persist import whitelist
-from ..runtime import broker
-from ..thread  import launch
-from ..workdir import sync
+from ..client    import Client, command
+from ..default   import Default
+from ..event     import Event
+from ..errors    import Errors, debug, later
+from ..find      import last
+from ..object    import Object, edit, fmt, keys, values
+from ..runtime   import broker
+from ..thread    import launch
+from ..whitelist import whitelist
+from ..workdir   import sync
 
 
 NAME    = __file__.split(os.sep)[-3]
-get     = broker.get
 saylock = _thread.allocate_lock()
 
 
 Errors.filter = ["PING", "PONG", "PRIVMSG"]
 
 
 def init():
@@ -46,24 +41,24 @@
     irc.events.joined.wait()
     return irc
 
 
 def shutdown():
     "shutdown irc bot."
     for bot in values(broker.objs):
-        if "irc" not in type(bot):
+        if "irc" not in str(type(bot)).lower():
             continue
         debug(f"IRC stopping {repr(bot)}")
         bot.state.pongcheck = True
         bot.state.keeprunning = False
         bot.events.connected.clear()
         bot.stop()
 
 
-class Config(Default):
+class Config(Default): # pylint: disable=R0902,R0903
 
     "Config"
 
     channel = f'#{NAME}'
     commands = True
     control = '!'
     edited = time.time()
@@ -276,15 +271,15 @@
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
                ) as _ex:
             pass
-        except Exception as ex:
+        except Exception as ex: # pylint: disable=W0718
             later(ex)
 
     def doconnect(self, server, nck, port=6667):
         "loop until connected."
         while 1:
             try:
                 if self.connect(server, port):
@@ -359,14 +354,15 @@
         self.events.authed.wait()
         self.direct(f'NICK {nck}')
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
         "parse text into an event."
+        # pylint: disable=R0912,R0915
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         debug(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
@@ -538,17 +534,14 @@
         Client.stop(self)
 
     def wait(self):
         "wait for ready."
         self.events.ready.wait()
 
 
-"callbacks"
-
-
 def cb_auth(bot, evt):
     "auth callback."
     bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
 
 
 def cb_cap(bot, evt):
     "capabilities callback."
@@ -585,17 +578,15 @@
 
 def cb_log(bot, evt):
     "log callback."
 
 
 def cb_ready(bot, evt):
     "bot is ready callback."
-    bot = get(evt.orig)
-    if bot:
-        bot.events.ready.set()
+    bot.events.ready.set()
 
 
 def cb_001(bot, evt):
     "first line received callback."
     bot.logon()
 
 
@@ -626,17 +617,14 @@
 def cb_quit(bot, evt):
     "quit callback."
     debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
-"commands"
-
-
 def cfg(event):
     "configure command."
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
@@ -679,15 +667,7 @@
     arg1 = event.args[0]
     arg2 = event.args[1]
     txt = f'\x00{arg1}\x00{arg2}'
     enc = txt.encode('ascii')
     base = base64.b64encode(enc)
     dcd = base.decode('ascii')
     event.reply(dcd)
-
-
-"register"
-
-
-Command.add(cfg)
-Command.add(mre)
-Command.add(pwd)
```

### Comparing `otpcr-7/otpcr/modules/mbx.py` & `otpcr-8/otpcr/modules/mbx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0212
+# pylint: disable=C,R
+
 
 "mailbox"
 
 
 import mailbox
 import os
 import time
 
 
-from ..object  import Object, fmt, update
-from ..client  import laps
-from ..command import Command
-from ..find    import find, fntime
-from ..persist import whitelist
-from ..workdir import sync
+from ..object    import Object, fmt, update
+from ..client    import laps
+from ..find      import find, fntime
+from ..whitelist import whitelist
+from ..workdir   import sync
 
 
 MONTH = {
     'Jan': 1,
     'Feb': 2,
     'Mar': 3,
     'Apr': 4,
@@ -95,32 +95,26 @@
         if len(event.args) > 1:
             txt = ",".join(event.args[1:])
         else:
             txt = "From,Subject"
         event.reply("%s %s %s" % (nr, fmt(email, txt, plain=True), laps(time.time() - fntime(email.__stp__))))
 
 
-Command.add(cor)
-
-
 def eml(event):
     "emnail"
     if not event.args:
         event.reply("eml <searchtxtinemail>")
         return
     nr = -1
     for fn, o in find("email"):
         if event.rest in o.text:
             nr += 1
             event.reply("%s %s %s" % (nr, fmt(o, "From,Subject"), laps(time.time() - fntime(fn))))
 
 
-Command.add(eml)
-
-
 def mbx(event):
     "mailbox"
     if not event.args:
         return
     fn = os.path.expanduser(event.args[0])
     event.reply("reading from %s" % fn)
     nr = 0
@@ -132,20 +126,17 @@
         return
     try:
         thing.lock()
     except FileNotFoundError:
         pass
     for m in thing:
         o = Email()
-        update(o, m._headers)
+        update(o, m._headers) # pylint: disable=W0212
         o.text = ""
         for payload in m.walk():
             if payload.get_content_type() == 'text/plain':
                 o.text += payload.get_payload()
         o.text = o.text.replace("\\n", "\n")
         sync(o)
         nr += 1
     if nr:
         event.reply("ok %s" % nr)
-
-
-Command.add(mbx)
```

### Comparing `otpcr-7/otpcr/modules/req.py` & `otpcr-8/otpcr/modules/req.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # This file is placed in the Public Domain.
-#
-#
+
 
 """| **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
@@ -75,16 +74,10 @@
 
 
 (1) provided are the confirmation letters of both the chamber and the king.
 (2) your reference: OTP-CR-117/19
 """
 
 
-from ..command import Command
-
-
 def req(event):
     "reconsider"
     event.reply(__doc__)
-
-
-Command.add(req)
```

### Comparing `otpcr-7/otpcr/modules/rss.py` & `otpcr-8/otpcr/modules/rss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=R0903,W0105
 
 
 "rich site syndicate"
 
 
 import html.parser
 import re
@@ -14,24 +12,22 @@
 import _thread
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 
 
-from ..client   import laps, spl
-from ..command  import Command
-from ..default  import Default
-from ..find     import find, fntime, last
-from ..object   import Object, fmt, update, values
-from ..persist  import whitelist
-from ..repeater import Repeater
-from ..runtime  import broker
-from ..thread   import launch
-from ..workdir  import sync
+from ..client     import laps, spl
+from ..default    import Default
+from ..find       import find, fntime, last
+from ..object     import Object, fmt, update, values
+from ..repeater   import Repeater
+from ..runtime    import broker
+from ..thread     import launch
+from ..workdir    import sync
 
 
 def init():
     "start fetcher."
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
@@ -47,30 +43,30 @@
     <head>
         <title>rssbot opml</title>
     </head>
     <body>
         <outline title="rssbot opml" text="24/7 feed fetcher">"""
 
 
-class Feed(Default):
+class Feed(Default): # pylint: disable=R0903
 
     "Feed"
 
 
-class Rss(Default):
+class Rss(Default): # pylint: disable=R0903
 
     "Rss"
 
     def __init__(self):
         Default.__init__(self)
         self.display_list = 'title,link,author'
         self.rss          = ''
 
 
-class Seen(Default):
+class Seen(Default): # pylint: disable=R0903
 
     "Seen"
 
     def __init__(self):
         Default.__init__(self)
         self.urls = []
 
@@ -320,17 +316,14 @@
 
 
 def useragent(txt):
     "return useragent."
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
-"commands"
-
-
 def dpl(event):
     "set display items."
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
     for _fn, feed in find('rss', {'rss': event.args[0]}):
@@ -413,20 +406,7 @@
         if result:
             event.reply(f'already got {url}')
             return
     feed = Rss()
     feed.rss = event.args[0]
     sync(feed)
     event.reply('ok')
-
-
-"register"
-
-
-Command.add(dpl)
-Command.add(exp)
-Command.add(nme)
-Command.add(rem)
-Command.add(res)
-Command.add(rss)
-whitelist(Rss)
-whitelist(Seen)
```

### Comparing `otpcr-7/otpcr/modules/rst.py` & `otpcr-8/otpcr/modules/rst.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=R,C,W0105
 
 
 "rest"
 
 
 import os
 import sys
@@ -18,14 +16,26 @@
 from ..errors  import debug, later
 from ..find    import fns
 from ..object  import Object
 from ..thread  import launch
 from ..workdir import Workdir
 
 
+def init():
+    "start object server."
+    result = None
+    try:
+        result = REST((Config.hostname, int(Config.port)), RESTHandler)
+    except OSError:
+        pass
+    if result:
+        launch(result.start)
+    return result
+
+
 class Config(Default):
 
     "Config"
 
     hostname = "localhost"
     port     = 10102
 
@@ -121,22 +131,7 @@
         "log access."
         debug(f"{self.address_string()} code {code} path {self.path}")
 
 
 def html(txt):
     "html template."
     return f"<!doctype html><html>{txt}</html>"
-
-
-"runtime"
-
-
-def init():
-    "start object server."
-    result = None
-    try:
-        result = REST((Config.hostname, int(Config.port)), RESTHandler)
-    except OSError:
-        pass
-    if result:
-        launch(result.start)
-    return result
```

### Comparing `otpcr-7/otpcr/modules/tdo.py` & `otpcr-8/otpcr/modules/tdo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,E0402
 
 
 "todo list"
 
 
 import time
 
 
-from ..client  import laps
-from ..object  import Object
-from ..command import Command
-from ..find    import fntime, find
-from ..persist import whitelist
-from ..workdir import sync
+from ..client    import laps
+from ..object    import Object
+from ..find      import fntime, find
+from ..workdir   import sync
 
 
-class NoDate(Exception):
+class NoDate(Exception): # pylint: disable=R0903
 
     "no matching date"
 
 
-class Todo(Object):
+class Todo(Object): # pylint: disable=R0903
 
     "Todo"
- 
+
     def __init__(self):
         Object.__init__(self)
         self.txt = ''
 
 
-whitelist(Todo)
-
-
 def dne(event):
     "flag todo as done."
     if not event.args:
         event.reply("dne <txt>")
         return
     selector = {'txt': event.args[0]}
     nmr = 0
@@ -47,17 +40,14 @@
         sync(obj, fnm)
         event.reply('ok')
         break
     if not nmr:
         event.reply("nothing todo")
 
 
-Command.add(dne)
-
-
 def tdo(event):
     "add todo."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('todo'):
             lap = laps(time.time()-fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
@@ -65,10 +55,7 @@
         if not nmr:
             event.reply("no todo")
         return
     obj = Todo()
     obj.txt = event.rest
     sync(obj)
     event.reply('ok')
-
-
-Command.add(tdo)
```

### Comparing `otpcr-7/otpcr/modules/thr.py` & `otpcr-8/otpcr/modules/thr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # This file is placed in the Public Domain.
-#
-#
 
 
 "show running threads"
 
 
 import threading
 import time
 
 
-from ..client import Command, laps
+from ..client import laps
 from ..object import Object, update
 
 
 STARTTIME = time.time()
 
 
 def thr(event):
@@ -36,10 +34,7 @@
     for uptime, txt in sorted(result, key=lambda x: x[1]):
         lap = laps(uptime)
         res.append(f'{txt}/{lap}')
     if res:
         event.reply(' '.join(res))
     else:
         event.reply('no threads')
-
-
-Command.add(thr)
```

### Comparing `otpcr-7/otpcr/modules/tmr.py` & `otpcr-8/otpcr/modules/tmr.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=W0105
 
 
 "timer"
 
 
 import datetime
 import re
 import time as ttime
 
 
-from ..client  import laps
-from ..command import Command
-from ..event   import Event
-from ..find    import find
-from ..object  import update
-from ..persist import whitelist
-from ..runtime import broker
-from ..thread  import launch
-from ..timer   import Timer
-from ..workdir import sync
+from ..client    import laps
+from ..event     import Event
+from ..find      import find
+from ..object    import update
+from ..runtime   import broker
+from ..thread    import launch
+from ..timer     import Timer
+from ..workdir   import sync
+
+
+def init():
+    "start timers."
+    for _fn, obj in find("timer"):
+        if "time" not in obj:
+            continue
+        diff = float(obj.time) - ttime.time()
+        if diff > 0:
+            bot = broker.first()
+            evt = Event()
+            update(evt, obj)
+            evt.orig = object.__repr__(bot)
+            timer = Timer(diff, evt.show)
+            launch(timer.start)
 
 
 MONTHS = [
     'Bo',
     'Jan',
     'Feb',
     'Mar',
@@ -76,15 +87,15 @@
             (day, month, yea) = ymdre.groups()
     except ValueError:
         try:
             ymre = re.search(r'(\d+)-(\d+)', daystr)
             if ymre:
                 (day, month) = ymre.groups()
                 yea = ttime.strftime("%Y", ttime.localtime())
-        except Exception as ex:
+        except Exception as ex: # pylint: disable=W0212
             raise NoDate(daystr) from ex
     if day:
         day = int(day)
         month = int(month)
         yea = int(yea)
         date = f"{day} {MONTHS[month]} {yea}"
         return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
@@ -167,17 +178,14 @@
 
 
 def today():
     "return date."
     return str(datetime.datetime.today()).split()[0]
 
 
-"commands"
-
-
 def tmr(event):
     "add a timer."
     result = ""
     if not event.rest:
         nmr = 0
         for _fn, obj in find('timer'):
             lap = float(obj.time) - ttime.time()
@@ -215,32 +223,7 @@
     event.result = []
     event.result.append(event.rest)
     timer = Timer(diff, event.show, thrname=event.cmd)
     update(timer, event)
     sync(timer)
     launch(timer.start)
     return result
-
-
-"runtime"
-
-
-def init():
-    "start timers."
-    for _fn, obj in find("timer"):
-        if "time" not in obj:
-            continue
-        diff = float(obj.time) - ttime.time()
-        if diff > 0:
-            bot = broker.first()
-            evt = Event()
-            update(evt, obj)
-            evt.orig = object.__repr__(bot)
-            timer = Timer(diff, evt.show)
-            launch(timer.start)
-
-
-"register"
-
-
-Command.add(tmr)
-whitelist(Timer)
```

### Comparing `otpcr-7/otpcr/modules/udp.py` & `otpcr-8/otpcr/modules/udp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=W0105
 
 
 "udp to irc relay"
 
 
 import select
 import socket
 import sys
 import threading
 import time
 
 
-from dataclasses import dataclass
-
-
-from ..command import Command
 from ..object  import Object, values
 from ..thread  import launch
 from ..runtime import broker
 
 
 def init():
     "start udp to irc relay."
     udpd = UDP()
     udpd.start()
     return udpd
 
 
-@dataclass
-class Cfg(Object):
+class Cfg(Object): # pylint: disable=R0903
 
     "Cfg"
 
     addr = ""
     host = "localhost"
     port = 5500
 
@@ -92,17 +85,14 @@
 
 def toudp(host, port, txt):
     "send udp packet to bot."
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     sock.sendto(bytes(txt.strip(), "utf-8"), (host, port))
 
 
-"commands"
-
-
 def udp(event):
     "send udp command."
     if event.rest:
         toudp(Cfg.host, Cfg.port, event.rest)
         event.reply(f"{len(event.rest)} characters sent")
         return
     if not select.select(
@@ -130,13 +120,7 @@
             if not txt:
                 stop = True
                 break
             size += len(txt)
             toudp(Cfg.host, Cfg.port, txt)
         if stop:
             break
-
-
-"register"
-
-
-Command.add(udp)
```

### Comparing `otpcr-7/otpcr/object.py` & `otpcr-8/otpcr/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=W0105
 
 
-"objects"
+"clean namespace"
 
 
 import json
 import os
 import pathlib
 import _thread
 
@@ -248,17 +246,14 @@
     "create directory."
     if os.path.exists(pth):
         return
     pth = pathlib.Path(pth)
     os.makedirs(pth, exist_ok=True)
 
 
-"interface"
-
-
 def __dir__():
     return (
         'Object',
         'construct',
         'dump',
         'dumps',
         'edit',
@@ -271,10 +266,7 @@
         'loads',
         'read',
         'search',
         'update',
         'values',
         'write'
     )
-
-
-__all__ = __dir__()
```

### Comparing `otpcr-7/otpcr/thread.py` & `otpcr-8/otpcr/thread.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=W0718
 
 
 "thread"
 
 
 import queue
 import threading
@@ -40,15 +38,15 @@
         return self._result
 
     def run(self):
         "run this thread's payload."
         func, args = self.queue.get()
         try:
             self._result = func(*args)
-        except Exception as ex:
+        except Exception as ex: # pylint: disable=W0718
             later(ex)
             if args and "Event" in str(type(args[0])):
                 args[0].ready()
 
 
 def launch(func, *args, **kwargs):
     "launch a thread."
@@ -68,7 +66,15 @@
     if '__class__' in dir(obj) and '__name__' in dir(obj):
         return f'{obj.__class__.__name__}.{obj.__name__}'
     if '__class__' in dir(obj):
         return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
     if '__name__' in dir(obj):
         return f'{obj.__class__.__name__}.{obj.__name__}'
     return None
+
+
+def __dir__():
+    return (
+        'Thread',
+        'launch',
+        'name'
+    )
```

### Comparing `otpcr-7/otpcr/timer.py` & `otpcr-8/otpcr/timer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-#
 
 
 "timer"
 
 
 import threading
 import time
@@ -43,7 +41,13 @@
         timer.start()
         self.timer   = timer
 
     def stop(self):
         "stop timer."
         if self.timer:
             self.timer.cancel()
+
+
+def __dir__():
+    return (
+        'Timer',
+    )
```

### Comparing `otpcr-7/otpcr/workdir.py` & `otpcr-8/otpcr/workdir.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=R0903
 
 
 "workdir"
 
 
 import datetime
 import os
 
 
 from .object import Object, cdir, fqn, read, write
 
 
-class Workdir(Object):
+class Workdir(Object): # pylint: disable=R0903
 
     "Workdir"
 
     workdir = ""
 
 
 def fetch(obj, pth):
@@ -58,7 +56,20 @@
 def sync(obj, pth=None):
     "sync object to disk."
     if pth is None:
         pth = ident(obj)
     pth2 = store(pth)
     write(obj, pth2)
     return pth
+
+
+def __dir__():
+    return (
+        'Workdir',
+        'fetch',
+        'ident',
+        'liststore',
+        'skel',
+        'store',
+        'strip',
+        'sync'
+    )
```

### Comparing `otpcr-7/otpcr.egg-info/PKG-INFO` & `otpcr-8/otpcr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: otpcr
-Version: 7
-Summary: OTP-CR-117/19
+Version: 8
+Summary: The 117 communication record of the year 2019 to the Office of the Prosecutor of the International Criminal Court.
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/otpcr
 Project-URL: bugs, https://github.com/xobjectz/otpcr/issues
 Project-URL: source, https://github.com/xobjectz/otpcr
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
```

### Comparing `otpcr-7/otpcr.egg-info/SOURCES.txt` & `otpcr-8/otpcr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,33 +4,31 @@
 docs/MANUAL.rst
 files/EM_Ack_OTP-CR-117_19.pdf
 files/EM_T04_OTP-CR-117_19.pdf
 files/EM_T07_OTP-CR-117_19_001.pdf
 files/bevestigd.jpg
 files/bevestigd.pdf
 files/informed.jpg
-files/otpcrsmile.png
-files/otpcrwall.png
 files/verbatim5.png
 otpcr/__init__.py
 otpcr/__main__.py
 otpcr/broker.py
 otpcr/client.py
 otpcr/command.py
 otpcr/default.py
 otpcr/errors.py
 otpcr/event.py
 otpcr/find.py
 otpcr/handler.py
 otpcr/object.py
-otpcr/persist.py
 otpcr/repeater.py
 otpcr/runtime.py
 otpcr/thread.py
 otpcr/timer.py
+otpcr/whitelist.py
 otpcr/workdir.py
 otpcr.egg-info/PKG-INFO
 otpcr.egg-info/SOURCES.txt
 otpcr.egg-info/dependency_links.txt
 otpcr.egg-info/entry_points.txt
 otpcr.egg-info/top_level.txt
 otpcr.egg-info/zip-safe
@@ -38,17 +36,15 @@
 otpcr/modules/cmd.py
 otpcr/modules/err.py
 otpcr/modules/flt.py
 otpcr/modules/fnd.py
 otpcr/modules/irc.py
 otpcr/modules/log.py
 otpcr/modules/mbx.py
-otpcr/modules/mdl.py
 otpcr/modules/mod.py
 otpcr/modules/req.py
 otpcr/modules/rss.py
 otpcr/modules/rst.py
 otpcr/modules/tdo.py
 otpcr/modules/thr.py
 otpcr/modules/tmr.py
-otpcr/modules/udp.py
-otpcr/modules/wsd.py
+otpcr/modules/udp.py
```

### Comparing `otpcr-7/pyproject.toml` & `otpcr-8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
     "setuptools>=43.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otpcr"
-description = "OTP-CR-117/19"
-version = "7"
+description = "The 117 communication record of the year 2019 to the Office of the Prosecutor of the International Criminal Court."
+version = "8"
 authors = [
     {name = "Bart Thate", email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
@@ -29,25 +29,23 @@
 "home" = "https://pypi.org/project/otpcr"
 "bugs" = "https://github.com/xobjectz/otpcr/issues"
 "source" = "https://github.com/xobjectz/otpcr"
 
 [tool.setuptools]
 packages = [
     'otpcr',
-    'otpcr.modules',
+    'otpcr.modules'
 ]
 zip-safe=true
 
 
 [tool.setuptools.data-files]
 "share/doc/otpcr" = [
     "README.rst",
     "docs/MANUAL.rst",
-    "files/otpcrsmile.png",
-    "files/otpcrwall.png",
     "files/bevestigd.jpg",
     "files/bevestigd.pdf",
     "files/informed.jpg",
     "files/verbatim5.png",
     "files/EM_Ack_OTP-CR-117_19.pdf",
     "files/EM_T07_OTP-CR-117_19_001.pdf",
     "files/EM_T04_OTP-CR-117_19.pdf"
```

