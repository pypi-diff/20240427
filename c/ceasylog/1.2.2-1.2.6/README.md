# Comparing `tmp/ceasylog-1.2.2.tar.gz` & `tmp/ceasylog-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ceasylog-1.2.2.tar", last modified: Fri Apr  5 06:41:57 2024, max compression
+gzip compressed data, was "ceasylog-1.2.6.tar", last modified: Fri Apr 26 15:25:33 2024, max compression
```

## Comparing `ceasylog-1.2.2.tar` & `ceasylog-1.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-05 06:41:57.668830 ceasylog-1.2.2/
--rw-r--r--   0 adminhuang   (501) staff       (20)    11339 2024-03-24 13:12:02.000000 ceasylog-1.2.2/LICENSE
--rw-r--r--   0 adminhuang   (501) staff       (20)      254 2024-04-05 06:41:57.668219 ceasylog-1.2.2/PKG-INFO
--rw-r--r--   0 adminhuang   (501) staff       (20)     6854 2024-04-05 06:39:16.000000 ceasylog-1.2.2/README.md
-drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-05 06:41:57.664754 ceasylog-1.2.2/ceasylog/
--rw-r--r--   0 adminhuang   (501) staff       (20)     8801 2024-04-05 06:24:07.000000 ceasylog-1.2.2/ceasylog/Logger.py
--rw-r--r--   0 adminhuang   (501) staff       (20)    11433 2024-04-04 12:19:51.000000 ceasylog-1.2.2/ceasylog/LoggerConfiger.py
--rw-r--r--   0 adminhuang   (501) staff       (20)      737 2024-03-31 05:32:26.000000 ceasylog-1.2.2/ceasylog/LoggerLevel.py
--rw-r--r--   0 adminhuang   (501) staff       (20)      633 2024-04-04 11:52:17.000000 ceasylog-1.2.2/ceasylog/LoggerNetworkConfiger.py
--rw-r--r--   0 adminhuang   (501) staff       (20)      430 2024-04-05 06:40:02.000000 ceasylog-1.2.2/ceasylog/LoggerStatic.py
--rw-r--r--   0 adminhuang   (501) staff       (20)      257 2024-04-04 14:16:03.000000 ceasylog-1.2.2/ceasylog/__init__.py
-drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-05 06:41:57.667645 ceasylog-1.2.2/ceasylog.egg-info/
--rw-r--r--   0 adminhuang   (501) staff       (20)      254 2024-04-05 06:41:57.000000 ceasylog-1.2.2/ceasylog.egg-info/PKG-INFO
--rw-r--r--   0 adminhuang   (501) staff       (20)      335 2024-04-05 06:41:57.000000 ceasylog-1.2.2/ceasylog.egg-info/SOURCES.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)        1 2024-04-05 06:41:57.000000 ceasylog-1.2.2/ceasylog.egg-info/dependency_links.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)       18 2024-04-05 06:41:57.000000 ceasylog-1.2.2/ceasylog.egg-info/requires.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)        9 2024-04-05 06:41:57.000000 ceasylog-1.2.2/ceasylog.egg-info/top_level.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)       38 2024-04-05 06:41:57.668894 ceasylog-1.2.2/setup.cfg
--rw-r--r--   0 adminhuang   (501) staff       (20)      371 2024-04-04 14:16:03.000000 ceasylog-1.2.2/setup.py
+drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-26 15:25:33.263875 ceasylog-1.2.6/
+-rw-r--r--   0 adminhuang   (501) staff       (20)    11339 2024-03-24 13:12:02.000000 ceasylog-1.2.6/LICENSE
+-rw-r--r--   0 adminhuang   (501) staff       (20)      254 2024-04-26 15:25:33.263414 ceasylog-1.2.6/PKG-INFO
+-rw-r--r--   0 adminhuang   (501) staff       (20)     6850 2024-04-05 15:18:09.000000 ceasylog-1.2.6/README.md
+drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-26 15:25:33.260684 ceasylog-1.2.6/ceasylog/
+-rw-r--r--   0 adminhuang   (501) staff       (20)    10016 2024-04-26 15:07:49.000000 ceasylog-1.2.6/ceasylog/Logger.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)    12331 2024-04-26 15:23:34.000000 ceasylog-1.2.6/ceasylog/LoggerConfiger.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)      737 2024-03-31 05:32:26.000000 ceasylog-1.2.6/ceasylog/LoggerLevel.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)      633 2024-04-04 11:52:17.000000 ceasylog-1.2.6/ceasylog/LoggerNetworkConfiger.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)      452 2024-04-26 15:24:15.000000 ceasylog-1.2.6/ceasylog/LoggerStatic.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)      257 2024-04-26 15:25:30.000000 ceasylog-1.2.6/ceasylog/__init__.py
+drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-26 15:25:33.262623 ceasylog-1.2.6/ceasylog.egg-info/
+-rw-r--r--   0 adminhuang   (501) staff       (20)      254 2024-04-26 15:25:33.000000 ceasylog-1.2.6/ceasylog.egg-info/PKG-INFO
+-rw-r--r--   0 adminhuang   (501) staff       (20)      335 2024-04-26 15:25:33.000000 ceasylog-1.2.6/ceasylog.egg-info/SOURCES.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)        1 2024-04-26 15:25:33.000000 ceasylog-1.2.6/ceasylog.egg-info/dependency_links.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)       18 2024-04-26 15:25:33.000000 ceasylog-1.2.6/ceasylog.egg-info/requires.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)        9 2024-04-26 15:25:33.000000 ceasylog-1.2.6/ceasylog.egg-info/top_level.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)       38 2024-04-26 15:25:33.263956 ceasylog-1.2.6/setup.cfg
+-rw-r--r--   0 adminhuang   (501) staff       (20)      371 2024-04-26 15:25:30.000000 ceasylog-1.2.6/setup.py
```

### Comparing `ceasylog-1.2.2/LICENSE` & `ceasylog-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ceasylog-1.2.2/README.md` & `ceasylog-1.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 * INFO 一般日志
 * WARN 警告日志
 * ERROR 错误日志
 * CRITICAL 严重错误日志
 
 ## 安装
 
-```bash
+```
 pip install ceasylog
 ```
 
 ## 使用方法
 
 ### 引入相关的库
```

### Comparing `ceasylog-1.2.2/ceasylog/Logger.py` & `ceasylog-1.2.6/ceasylog/Logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import threading
 import time
 import traceback
 import uuid
 from datetime import datetime
 
 import requests
-from colorama import Fore, Style
+from colorama import Style
 from colorama import init as coloramaInit
 
 from ceasylog.LoggerConfiger import *
 
 coloramaInit(autoreset=True)
 
 # Surprise Mother F**K LMX
@@ -25,14 +25,30 @@
     Fore.LIGHTGREEN_EX,
     Fore.LIGHTMAGENTA_EX,
 ]
 
 MAX_BLANK = 35
 
 
+def getStyle(name: str):
+    """获取样式"""
+    styleMap = {
+        LOG_STYLE[0]: ["a", "b", "c", "d", "u", "0", "8", "9"],
+        LOG_STYLE[1]: ["e", "f", "g", "h", "v", "1", "7"],
+        LOG_STYLE[2]: ["i", "j", "k", "l", "w", "2", "6"],
+        LOG_STYLE[3]: ["m", "n", "o", "p", "x", "3", "5"],
+        LOG_STYLE[4]: ["q", "r", "s", "t", "y", "z", "4"],
+    }
+    startWith = name[:1].lower()
+    for i in styleMap.keys():
+        if startWith in styleMap[i]:
+            return i
+    return LOG_STYLE[random.randint(0, len(LOG_STYLE) - 1)]
+
+
 def getTime(timeFormat1: str, timeFormat2: str) -> tuple[str, str, str]:
     """
     获取时间
     :param timeFormat2:
     :param timeFormat1:
     :return:
     """
@@ -145,63 +161,85 @@
         """
         :param config: 配置信息
         """
         self.config = config
         # 超过长度的名称省略
         if len(self.config.name) > MAX_BLANK:
             self.config.setName(self.config.name[:(MAX_BLANK - 13)] + "..." + self.config.name[-10:])
-        self.logStyle = LOG_STYLE[random.randint(0, len(LOG_STYLE) - 1)]
+        # self.logStyle = LOG_STYLE[random.randint(0, len(LOG_STYLE) - 1)]
+        self.logStyle = getStyle(self.config.name)
 
     def debug(self, msg: str):
         uid = getUID()
         nowTimePrint, nowTimeRecord, timeStamp = getTime(self.config.printTimeFormat, self.config.recordTimeFormat)
         logPrint(msg, LoggerLevel.DEBUG, self.config, uid, self.logStyle, nowTimePrint)
         logRecord(msg, LoggerLevel.DEBUG, self.config, uid, nowTimeRecord)
+        self.config.handleFunc(LoggerLevel.DEBUG, msg)
         logNetworkSender(msg, LoggerLevel.DEBUG, self.config, uid, timeStamp)
+        return uid
 
     def info(self, msg: str):
         uid = getUID()
         nowTimePrint, nowTimeRecord, timeStamp = getTime(self.config.printTimeFormat, self.config.recordTimeFormat)
         logPrint(msg, LoggerLevel.INFO, self.config, uid, self.logStyle, nowTimePrint)
         logRecord(msg, LoggerLevel.INFO, self.config, uid, nowTimeRecord)
+        self.config.handleFunc(LoggerLevel.INFO, msg)
         logNetworkSender(msg, LoggerLevel.INFO, self.config, uid, timeStamp)
+        return uid
 
     def warn(self, msg: str):
         uid = getUID()
         nowTimePrint, nowTimeRecord, timeStamp = getTime(self.config.printTimeFormat, self.config.recordTimeFormat)
         logPrint(msg, LoggerLevel.WARN, self.config, uid, self.logStyle, nowTimePrint)
         logRecord(msg, LoggerLevel.WARN, self.config, uid, nowTimeRecord)
+        self.config.handleFunc(LoggerLevel.WARN, msg)
         logNetworkSender(msg, LoggerLevel.WARN, self.config, uid, timeStamp)
+        return uid
 
     def error(self, msg: str):
         uid = getUID()
         nowTimePrint, nowTimeRecord, timeStamp = getTime(self.config.printTimeFormat, self.config.recordTimeFormat)
         logPrint(msg, LoggerLevel.ERROR, self.config, uid, self.logStyle, nowTimePrint)
         logRecord(msg, LoggerLevel.ERROR, self.config, uid, nowTimeRecord)
+        self.config.handleFunc(LoggerLevel.ERROR, msg)
         logNetworkSender(msg, LoggerLevel.ERROR, self.config, uid, timeStamp)
+        return uid
 
     def critical(self, msg: str):
         uid = getUID()
         nowTimePrint, nowTimeRecord, timeStamp = getTime(self.config.printTimeFormat, self.config.recordTimeFormat)
         logPrint(msg, LoggerLevel.CRITICAL, self.config, uid, self.logStyle, nowTimePrint)
         logRecord(msg, LoggerLevel.CRITICAL, self.config, uid, nowTimeRecord)
+        self.config.handleFunc(LoggerLevel.CRITICAL, msg)
         logNetworkSender(msg, LoggerLevel.CRITICAL, self.config, uid, timeStamp)
+        return uid
 
     def exception(self, e: BaseException, level: LoggerLevel = LoggerLevel.ERROR):
         if not isinstance(e, BaseException):
             return
         exceptionBaseInfo = traceback.format_exc(limit=None, chain=True)
         exceptionBaseInfoList = exceptionBaseInfo.split("\n")
         exceptionInfo = ""
         for i in range(len(exceptionBaseInfoList)):
             i -= 1
             if i == 0:
                 exceptionInfo = exceptionBaseInfoList[i]
                 continue
-            exceptionInfo = exceptionInfo + "\n" + " " * (len(getTime(self.config.printTimeFormat, self.config.recordTimeFormat)[0]) + 1 + len(getUID()) + 1 + MAX_BLANK + 8) + exceptionBaseInfoList[i]
+            exceptionInfo = (exceptionInfo + "\n" + " " * (
+                    len(
+                        getTime(
+                            self.config.printTimeFormat,
+                            self.config.recordTimeFormat
+                        )[0]
+                    ) + 1
+                    + len(getUID())
+                    + 1
+                    + MAX_BLANK
+                    + 8
+            ) + exceptionBaseInfoList[i])
         exceptionLoggerCfg = LoggerConfiger()
         exceptionLoggerCfg.extendBy(self.config)
         exceptionLoggerCfg.setName(self.config.name)
         exceptionLoggerCfg.setMaxPrintLevel(level)
         exceptionLoggerCfg.setMinPrintLevel(level)
         exceptionLoggerCfg.setMaxRecordLevel(level)
         exceptionLoggerCfg.setMinRecordLevel(level)
@@ -213,15 +251,14 @@
         elif level == LoggerLevel.WARN:
             exceptionLogger.warn(exceptionInfo)
         elif level == LoggerLevel.ERROR:
             exceptionLogger.error(exceptionInfo)
         elif level == LoggerLevel.CRITICAL:
             exceptionLogger.critical(exceptionInfo)
 
-
     # def d(self, msg):
     #     self.debug(msg)
     #
     # def i(self, msg):
     #     self.info(msg)
     #
     # def w(self, msg):
```

### Comparing `ceasylog-1.2.2/ceasylog/LoggerConfiger.py` & `ceasylog-1.2.6/ceasylog/LoggerConfiger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,34 @@
+import types
+from random import randint
+
+from colorama import Fore
+
 import ceasylog
 import ceasylog.LoggerLevel as LoggerLevel
 from ceasylog.LoggerNetworkConfiger import LoggerNetworkConfiger
 
+LOG_STYLE = [
+    Fore.LIGHTYELLOW_EX,
+    Fore.LIGHTBLUE_EX,
+    Fore.LIGHTCYAN_EX,
+    Fore.LIGHTGREEN_EX,
+    Fore.LIGHTMAGENTA_EX,
+]
+
 
 class LoggerConfiger(object):
 
     def __init__(self):
         self.__name = "default"
 
+        self.__style = LOG_STYLE[randint(0, len(LOG_STYLE) - 1)]
+
+        self.handleFunc = lambda: None
+
         self.__maxPrintLevel = LoggerLevel.CRITICAL
         self.__minPrintLevel = LoggerLevel.DEBUG
         self.__maxRecordLevel = LoggerLevel.CRITICAL
         self.__minRecordLevel = LoggerLevel.WARN
 
         self.__printTimeFormat = "%Y-%m-%d %H:%M:%S.%f"
         self.__recordTimeFormat = "%Y-%m-%d %H:%M:%S.%f"
@@ -24,14 +41,18 @@
         self.__networkRecordCfg: LoggerNetworkConfiger = LoggerNetworkConfiger()
 
     @property
     def name(self):
         return self.__name
 
     @property
+    def style(self):
+        return self.__style
+
+    @property
     def maxPrintLevel(self):
         return self.__maxPrintLevel
 
     @property
     def minPrintLevel(self):
         return self.__minPrintLevel
 
@@ -67,14 +88,25 @@
     def isRecordNetworkB(self):
         return self.__isRecordNetworkB
 
     @property
     def networkRecordCfg(self):
         return self.__networkRecordCfg
 
+    def refreshStyle(self):
+        lastStyle = self.__style
+        self.__style = LOG_STYLE[randint(0, len(LOG_STYLE) - 1)]
+        while lastStyle != self.__style:
+            self.__style = LOG_STYLE[randint(0, len(LOG_STYLE) - 1)]
+
+    def setHandleFunc(self, func) -> None:
+        if not isinstance(func, types.FunctionType):
+            raise ValueError("Handler must be a function")
+        self.handleFunc = func
+
     def loadFromFile(self, path: str):
         import os
         import json
         if not os.path.isabs(path):
             # 拼接解释器运行路径作为绝对路径
             path = os.path.join(os.path.dirname(os.path.abspath(__file__)), path)
         if not os.path.exists(path):
@@ -90,15 +122,15 @@
             if key == "name":
                 self.setName(value)
             elif key == "version":
                 fileVersion = float(str(value).split(".")[0] + "." + str(value).split(".")[1])
                 version = float(str(ceasylog.VERSION).split(".")[0] + "." + str(ceasylog.VERSION).split(".")[1])
                 if fileVersion > version:
                     raise Exception(f"LoggerConfiger file version {fileVersion} is higher than ceasylog "
-                                    f"version {version}")
+                                    f"version {version}, Please update ceasylog version to {fileVersion}")
             elif key == "maxPrintLevel":
                 if value == "CRITICAL":
                     value = LoggerLevel.CRITICAL
                 elif value == "ERROR":
                     value = LoggerLevel.ERROR
                 elif value == "WARN":
                     value = LoggerLevel.WARN
@@ -250,14 +282,16 @@
             self.__maxRecordLevel = father.maxRecordLevel
             self.__minRecordLevel = father.minRecordLevel
 
             self.__printTimeFormat = father.printTimeFormat
             self.__recordTimeFormat = father.recordTimeFormat
             self.__recordPathNameFormat = father.recordPathNameFormat
 
+            self.handleFunc = father.handleFunc
+
             self.__isRecordB = father.isRecordB
             self.__recordPath = father.recordPath
 
     def setName(self, name: str):
         self.__name = name.strip()
 
     def setMaxPrintLevel(self, maxPrintLevel):
```

### Comparing `ceasylog-1.2.2/ceasylog/LoggerLevel.py` & `ceasylog-1.2.6/ceasylog/LoggerLevel.py`

 * *Files identical despite different names*

### Comparing `ceasylog-1.2.2/ceasylog/LoggerNetworkConfiger.py` & `ceasylog-1.2.6/ceasylog/LoggerNetworkConfiger.py`

 * *Files identical despite different names*

