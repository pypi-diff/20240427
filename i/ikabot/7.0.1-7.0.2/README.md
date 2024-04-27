# Comparing `tmp/ikabot-7.0.1.tar.gz` & `tmp/ikabot-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikabot-7.0.1.tar", last modified: Thu Apr 25 18:20:54 2024, max compression
+gzip compressed data, was "ikabot-7.0.2.tar", last modified: Sat Apr 27 17:56:14 2024, max compression
```

## Comparing `ikabot-7.0.1.tar` & `ikabot-7.0.2.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.899791 ikabot-7.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 18:20:51.000000 ikabot-7.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 18:20:51.000000 ikabot-7.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-25 18:20:54.899791 ikabot-7.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-25 18:20:51.000000 ikabot-7.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.883791 ikabot-7.0.1/ikabot/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10483 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.891791 ikabot-7.0.1/ikabot/function/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/activateMiracle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/alertAttacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/alertLowWine.py
--rw-r--r--   0 runner    (1001) docker     (127)    22648 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/attackBarbarians.py
--rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/autoPirate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/buyResources.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/checkForUpdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/constructBuilding.py
--rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/constructionList.py
--rw-r--r--   0 runner    (1001) docker     (127)    52825 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/decaptchaConf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/distributeResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/donate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/donationBot.py
--rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/dumpWorld.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/getStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/importExportCookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/investigate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/killTasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/loadCustomModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/loginDaily.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/proxyConf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/searchForIslandSpaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/sellResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/sendResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/shipMovements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/stationArmy.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/testTelegramBot.py
--rw-r--r--   0 runner    (1001) docker     (127)    17449 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/trainArmy.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/vacationMode.py
--rw-r--r--   0 runner    (1001) docker     (127)    64399 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/webServer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.891791 ikabot-7.0.1/ikabot/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/aesCipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/apiComm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/botComm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/getJson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/market.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/naval.py
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/pedirInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/planRoutes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/varios.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.883791 ikabot-7.0.1/ikabot/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.883791 ikabot-7.0.1/ikabot/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.899791 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/activateMiracle.po
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/aesCipher.po
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/alertAttacks.po
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/alertLowWine.po
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/botComm.po
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/buyResources.po
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/command_line.po
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/config.po
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/constructBuilding.po
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/constructionList.po
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/distributeResources.po
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/donate.po
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/donationBot.po
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/getStatus.po
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/gui.mo
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/gui.po
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/loginDaily.po
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.po
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/sellResources.po
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/sendResources.po
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/session.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/session.po
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/shipMovements.po
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/signals.mo
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/signals.po
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainArmy.pot
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainFleets.po
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainTroops.po
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/update.po
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/vacationMode.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.899791 ikabot-7.0.1/ikabot/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59884 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/web/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.899791 ikabot-7.0.1/ikabot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:20:54.899791 ikabot-7.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-25 18:20:51.000000 ikabot-7.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.692282 ikabot-7.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-27 17:56:10.000000 ikabot-7.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-27 17:56:10.000000 ikabot-7.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-27 17:56:14.692282 ikabot-7.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-27 17:56:10.000000 ikabot-7.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.676282 ikabot-7.0.2/ikabot/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10909 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.684282 ikabot-7.0.2/ikabot/function/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/activateMiracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/activateShrine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/alertAttacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/alertLowWine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22648 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/attackBarbarians.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/autoPirate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/buyResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/checkForUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/constructBuilding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22509 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/constructionList.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52825 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/decaptchaConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/distributeResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/donate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/donationBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/dumpWorld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/getStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/importExportCookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/investigate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/killTasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/loadCustomModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/loginDaily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/proxyConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/searchForIslandSpaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/sellResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/sendResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/shipMovements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/stationArmy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/testTelegramBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17449 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/trainArmy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/vacationMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64399 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/webServer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.684282 ikabot-7.0.2/ikabot/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/aesCipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/apiComm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/botComm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/getJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/naval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/pedirInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/planRoutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/varios.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.676282 ikabot-7.0.2/ikabot/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.676282 ikabot-7.0.2/ikabot/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.688282 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/activateMiracle.po
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/aesCipher.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/alertAttacks.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/alertLowWine.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/botComm.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/buyResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/command_line.po
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/config.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/constructBuilding.po
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/constructionList.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/distributeResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/donate.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/donationBot.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/getStatus.po
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/gui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/gui.po
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/loginDaily.po
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/sellResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/sendResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/session.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/session.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/shipMovements.po
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/signals.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/signals.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainArmy.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainFleets.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainTroops.po
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/update.po
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/vacationMode.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.688282 ikabot-7.0.2/ikabot/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59889 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/web/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.692282 ikabot-7.0.2/ikabot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 17:56:14.692282 ikabot-7.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-27 17:56:10.000000 ikabot-7.0.2/setup.py
```

### Comparing `ikabot-7.0.1/LICENSE` & `ikabot-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/PKG-INFO` & `ikabot-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikabot
-Version: 7.0.1
+Version: 7.0.2
 Home-page: https://github.com/Ikabot-Collective/ikabot
 Author: physics-sp
 Author-email: physics-sp@protonmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ikabot Version: 7.0.1 Home-page: https://
+Metadata-Version: 2.1 Name: ikabot Version: 7.0.2 Home-page: https://
 github.com/Ikabot-Collective/ikabot Author: physics-sp Author-email: physics-
 sp@protonmail.com License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: requests Requires-Dist:
 requests[socks] Requires-Dist: cryptography Requires-Dist: psutil
   ![Ikabot Banner](assets/banner.png) [![Downloads](https://static.pepy.tech/
 badge/ikabot)](https://pepy.tech/project/ikabot) ![GitHub Repo stars](https://
```

### Comparing `ikabot-7.0.1/README.md` & `ikabot-7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/command_line.py` & `ikabot-7.0.2/ikabot/command_line.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from ikabot.function.stationArmy import stationArmy
 from ikabot.function.testTelegramBot import testTelegramBot
 from ikabot.function.trainArmy import trainArmy
 from ikabot.function.update import update
 from ikabot.function.vacationMode import vacationMode
 from ikabot.function.webServer import webServer
 from ikabot.function.loadCustomModule import loadCustomModule
+from ikabot.function.activateShrine import activateShrine
 from ikabot.helpers.botComm import telegramDataIsValid, updateTelegramData
 from ikabot.helpers.gui import *
 from ikabot.helpers.pedirInfo import read
 from ikabot.helpers.process import updateProcessList
 from ikabot.web.session import *
 
 t = gettext.translation("command_line", localedir, languages=languages, fallback=True)
@@ -113,65 +114,66 @@
         print("")
 
     menu_actions = {
         1: constructionList,
         2: sendResources,
         3: distributeResources,
         4: getStatus,
-        5: searchForIslandSpaces,
+        5: activateShrine,
         6: loginDaily,
-        101: alertAttacks,
-        102: alertLowWine,
-        111: buyResources,
-        112: sellResources,
-        121: donate,
-        122: donationBot,
+        701: alertAttacks,
+        702: alertLowWine,
+        801: buyResources,
+        802: sellResources,
+        901: donate,
+        902: donationBot,
         10: vacationMode,
         11: activateMiracle,
-        131: trainArmy,
-        132: stationArmy,
+        1201: trainArmy,
+        1202: stationArmy,
         13: shipMovements,
         14: constructBuilding,
         15: update,
         16: webServer,
         17: autoPirate,
         18: investigate,
         19: attackBarbarians,
-        20: dumpWorld,
-        141: proxyConf,
-        142: updateTelegramData,
-        143: killTasks,
-        144: decaptchaConf,
-        145: logs,
-        146: testTelegramBot,
-        147: importExportCookie,
-        148: loadCustomModule
+        2001: searchForIslandSpaces,
+        2002: dumpWorld,
+        2101: proxyConf,
+        2102: updateTelegramData,
+        2103: killTasks,
+        2104: decaptchaConf,
+        2105: logs,
+        2106: testTelegramBot,
+        2107: importExportCookie,
+        2108: loadCustomModule
     }
 
     print(_("(0)  Exit"))
     print(_("(1)  Construction list"))
     print(_("(2)  Send resources"))
     print(_("(3)  Distribute resources"))
     print(_("(4)  Account status"))
-    print(_("(5)  Monitor islands"))
+    print(_("(5)  Activate Shrine"))
     print(_("(6)  Login daily"))
     print(_("(7)  Alerts / Notifications"))
     print(_("(8)  Marketplace"))
     print(_("(9)  Donate"))
     print(_("(10) Activate vacation mode"))
     print(_("(11) Activate miracle"))
     print(_("(12) Military actions"))
     print(_("(13) See movements"))
     print(_("(14) Construct building"))
     print(_("(15) Update Ikabot"))
     print(_("(16) Ikabot Web Server"))
     print(_("(17) Auto-Pirate"))
     print(_("(18) Investigate"))
     print(_("(19) Attack barbarians"))
-    print(_("(20) Dump / View world"))
+    print(_("(20) Dump / Monitor world"))
     print(_("(21) Options / Settings"))
     total_options = len(menu_actions) + 1
     selected = read(min=0, max=total_options, digit=True, empty=True)
     
     # refresh main menu on hitting enter
     if selected == '':
         return menu(session)
@@ -183,53 +185,65 @@
         print(_("(2) Alert wine running out"))
 
         selected = read(min=0, max=2, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
-            selected += 100
+            selected += 700
 
     if selected == 8:
         banner()
         print(_("(0) Back"))
         print(_("(1) Buy resources"))
         print(_("(2) Sell resources"))
 
         selected = read(min=0, max=2, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
-            selected += 110
+            selected += 800
 
     if selected == 9:
         banner()
         print(_("(0) Back"))
         print(_("(1) Donate once"))
         print(_("(2) Donate automatically"))
 
         selected = read(min=0, max=2, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
-            selected += 120
+            selected += 900
 
     if selected == 12:
         banner()
         print(_("(0) Back"))
         print(_("(1) Train Army"))
         print(_("(2) Send Troops/Ships"))
         selected = read(min=0, max=2, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
-            selected += 130
+            selected += 1200
+
+    if selected == 20:
+        print(_("(0) Back"))
+        print(_("(1) Monitor islands"))
+        print(_("(2) Dump & Search world"))
+        
+        selected = read(min=0, max=8, digit=True)
+        if selected == 0:
+            menu(session)
+            return
+        if selected > 0:
+            selected += 2100
 
     if selected == 21:
         banner()
         print(_("(0) Back"))
         print(_("(1) Configure Proxy"))
         if telegramDataIsValid(session):
             print(_("(2) Change the Telegram data"))
@@ -243,15 +257,15 @@
         print(_("(8) Load custom ikabot module"))
 
         selected = read(min=0, max=8, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
-            selected += 140
+            selected += 2100
 
     if selected != 0:
         try:
             event = multiprocessing.Event()  # creates a new event
             config.has_params = len(config.predetermined_input) > 0
             process = multiprocessing.Process(
                 target=menu_actions[selected],
```

### Comparing `ikabot-7.0.1/ikabot/config.py` & `ikabot-7.0.2/ikabot/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import gettext
 import locale
 import os
 import random
 
 # Version changed automatically by the release pipeline
-IKABOT_VERSION = "7.0.1"
+IKABOT_VERSION = "7.0.2"
 
 IKABOT_VERSION_TAG = "v" + IKABOT_VERSION
 
 local = locale.setlocale(locale.LC_ALL, "")
 if "es_" in local:
     languages = ["es"]
 else:
```

### Comparing `ikabot-7.0.1/ikabot/function/activateMiracle.py` & `ikabot-7.0.2/ikabot/function/activateMiracle.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/alertAttacks.py` & `ikabot-7.0.2/ikabot/function/alertAttacks.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/alertLowWine.py` & `ikabot-7.0.2/ikabot/function/alertLowWine.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/attackBarbarians.py` & `ikabot-7.0.2/ikabot/function/attackBarbarians.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/autoPirate.py` & `ikabot-7.0.2/ikabot/function/autoPirate.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/buyResources.py` & `ikabot-7.0.2/ikabot/function/buyResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/checkForUpdate.py` & `ikabot-7.0.2/ikabot/function/checkForUpdate.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/constructBuilding.py` & `ikabot-7.0.2/ikabot/function/constructBuilding.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/constructionList.py` & `ikabot-7.0.2/ikabot/function/constructionList.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import re
 import threading
 import time
 import traceback
 from decimal import *
 
 import requests
+from functools import cache
 
 from ikabot.config import *
 from ikabot.helpers.botComm import *
 from ikabot.helpers.getJson import getCity
 from ikabot.helpers.gui import *
 from ikabot.helpers.pedirInfo import *
 from ikabot.helpers.planRoutes import *
@@ -553,15 +554,15 @@
     print(_("current level:{}").format(current_level))
 
     final_level = read(min=current_level, msg=_("increase to level:"))
     building["upgradeTo"] = final_level
 
     return building
 
-
+@cache
 def checkhash(url):
     m = hashlib.md5()
     r = requests.get(url)
     for data in r.iter_content(8192):
         m.update(data)
         if m.hexdigest() == config.material_img_hash[0]:
             material = "wood"
```

### Comparing `ikabot-7.0.1/ikabot/function/decaptchaConf.py` & `ikabot-7.0.2/ikabot/function/decaptchaConf.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/distributeResources.py` & `ikabot-7.0.2/ikabot/function/distributeResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/donate.py` & `ikabot-7.0.2/ikabot/function/donate.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/donationBot.py` & `ikabot-7.0.2/ikabot/function/donationBot.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,41 +71,41 @@
                 donation_type = "tradegood"
             elif rta.lower() == b:
                 donation_type = "both"
             else:
                 donation_type = None
                 percentage = None
 
-            if donation_type is not None and donate_method is 1:
+            if donation_type is not None and donate_method == 1:
                 print(
                     _(
                         "What is the maximum percentage of your storage capacity that you wish to keep occupied? (the resources that exceed it, will be donated) (default: 80%)"
                     )
                 )
                 percentage = read(min=0, max=100, empty=True)
                 if percentage == "":
                     percentage = 80
                 elif (
                     percentage == 100
                 ):  # if the user is ok with the storage beeing totally full, don't donate at all
                     donation_type = None
-            elif donation_type is not None and donate_method is 2:
+            elif donation_type is not None and donate_method == 2:
                 print(
                     _(
                         "What is the percentage of your production that you wish to donate? (enter 0 to disable donation for the town) (default: 50%)"
                     )
                 )
                 percentage = read(
                     min=0, max=100, empty=True
                 )  # max_random_waiting_time increases inaccuracy
                 if percentage == "":
                     percentage = 50
                 elif percentage == 0:
                     donation_type = None
-            elif donation_type is not None and donate_method is 3:
+            elif donation_type is not None and donate_method == 3:
                 print(
                     _(
                         "What is the amount would you like to donate? (enter 0 to disable donation for the town) (default: 10000)"
                     )
                 )
                 percentage = read(
                     min=0, max=1000000, empty=True
@@ -179,41 +179,41 @@
             # get the storageCapacity and the wood this city has
             html = session.get(city_url + cityId)
             city = getCity(html)
             wood = city["availableResources"][0]
             storageCapacity = city["storageCapacity"]
 
             # get the percentage
-            if donate_method is 1:
+            if donate_method == 1:
                 percentage = cities_dict[cityId]["percentage"]
                 percentage /= 100
 
                 # calculate what is the amount of wood that should be preserved
                 max_wood = storageCapacity * percentage
                 max_wood = int(max_wood)
 
                 # calculate the wood that is exceeding the percentage
                 to_donate = wood - max_wood
                 if to_donate <= 0:
                     continue
 
-            elif donate_method is 2:
+            elif donate_method == 2:
                 # get current production rate if changed since starting the bot
                 (wood_prod, good_prod, typeGood) = getProductionPerSecond(
                     session, cityId
                 )
                 percentage = cities_dict[cityId]["percentage"]
 
                 # calculate the amount of wood to be donated from production, based on the given donation frequency
                 to_donate = int((wood_prod * percentage / 100) * (waiting_time * 60))
                 # Note: Connection delay can/will cause "inaccurate" donations especially with low waiting_time
                 if to_donate <= 0:
                     continue
 
-            elif donate_method is 3:
+            elif donate_method == 3:
                 percentage = cities_dict[cityId]["percentage"]
                 # make sure the donation amount is never lower than resources available
                 max_wood = wood - percentage
                 max_wood = int(max_wood)
 
                 to_donate = percentage
                 if max_wood <= 0:
```

### Comparing `ikabot-7.0.1/ikabot/function/dumpWorld.py` & `ikabot-7.0.2/ikabot/function/dumpWorld.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/getStatus.py` & `ikabot-7.0.2/ikabot/function/getStatus.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/importExportCookie.py` & `ikabot-7.0.2/ikabot/function/importExportCookie.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/investigate.py` & `ikabot-7.0.2/ikabot/function/investigate.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,37 +39,62 @@
     ].split("=")[-1]
     url = "action=Advisor&function=doResearch&actionRequest={}&type={}&backgroundView=city&currentCityId={}&templateView=researchAdvisor&ajax=1".format(
         actionRequest, research_type, city_id
     )
     session.post(url)
 
 
-def experiment(session, experiments):
+def experiment(session, experiments, automatic):
     while experiments["qty"] > 0:
+        if automatic is True: experiments["qty"] = 999999
         # Validate if material is still there..oterwhise log it and send it via bot
         session.get("view=city&cityId={}".format(experiments["cityID"]), noIndex=True)
         data = session.get("view=updateGlobalData&ajax=1", noIndex=True)
         json_data = json.loads(data, strict=False)
         json_data = json_data[0][1]["headerData"]
         current_glass = int(json_data["currentResources"]["3"])
 
         if current_glass < 300000:
-            sendToBot(
-                session,
-                f"Experiment process ended on {experiments['cityName']} due lack of glass ({addThousandSeparator(current_glass)})",
-            )
-            break
+            if automatic is False:
+                sendToBot(
+                    session,
+                    f"Experiment process ended on {experiments['cityName']}, not enough crystal ({addThousandSeparator(current_glass)})",
+                )
+                break
+            else:
+                session.setStatus(
+                    f"Experiment skipped in {experiments['cityName']}, not enough crystal ({addThousandSeparator(current_glass)}) @{getDateTime()}"
+                )
+                time.sleep(241 * 60)# Re-try after 4h1m
+                continue
+
+        while True:
+            cooldown_url = f'view=academy&cityId={experiments["cityID"]}&position={experiments["pos"]}&backgroundView=city&currentCityId={experiments["cityID"]}&templateView=academy&actionRequest={actionRequest}&ajax=1'
+            cooldown_html = session.get(cooldown_url)
+            if 'experimentCooldown' in cooldown_html: # Check if a cooldown is still in effect
+                session.setStatus(
+                    f"Cooldown is still in effect in {experiments['cityName']} @{getDateTime()}",
+                )
+                time.sleep(300) # Check again after 5 minutes
+                continue
+            else:
+                break
 
         url = f'action=CityScreen&function=buyResearch&cityId={experiments["cityID"]}&position={experiments["pos"]}&backgroundView=city&currentCityId={experiments["cityID"]}&templateView=academy&actionRequest={actionRequest}&ajax=1'
         session.post(url)
+
         experiments["qty"] = experiments["qty"] - 1
-        sendToBot(
-            session,
-            f"Experiment done on {experiments['cityName']}, left = {experiments['qty']} time (s)",
-        )
+        if automatic is False:
+            session.setStatus(
+                f"Experiment done in {experiments['cityName']} @{getDateTime()}, left = {experiments['qty']} time (s)",
+            )
+        else:
+            session.setStatus(
+                f"Experiment done in {experiments['cityName']} @{getDateTime()}"
+            )
 
         # Terminate it if no of experiments = 0
         if experiments["qty"] == 0:
             break
 
         # Every 4h, added 1m extra
         time.sleep(241 * 60)
@@ -88,15 +113,16 @@
     config.predetermined_input = predetermined_input
     try:
         banner()
 
         print("\nSelect an option:")
         print("1) Study")
         print("2) Conduct experiment")
-        option = read(min=1, max=2)
+        print("3) Conduct automatically")
+        option = read(min=1, max=3)
 
         if option == 1:
             studies = get_studies(session)
             keys = list(studies.keys())
             num_studies = len(
                 [
                     key
@@ -134,67 +160,81 @@
                 return
 
             study(session, studies, available[choice - 1])
             print(_("Done."))
             enter()
             event.set()
         else:
+            if option == 3:
+                max_experiments = 9999999
+                automatic = True
+            else:
+                automatic = False
             # Experiment
             experiments = {}
             total_glass = 0
             found_academy = -1
 
             # while (total_glass < 300000 or found_academy < 0):
             banner()
             print("Pick city: ")
             city = chooseCity(session)
             total_glass = int(city["availableResources"][3])
 
             # Check if enough glass
-            if total_glass < 300000:
-                print(
-                    f"Not enough glass ({addThousandSeparator(total_glass)}), try another city. Min=300k"
-                )
-                time.sleep(2)
-                enter()
-                event.set()
-                return
+            if automatic is False:
+                if total_glass < 300000:
+                    print(
+                        f"Not enough glass ({addThousandSeparator(total_glass)}), try another city. Min=300k"
+                    )
+                    time.sleep(2)
+                    enter()
+                    event.set()
+                    return
 
             # Search for Academy
             for building in city["position"]:
                 if building["building"] == "academy":
                     found_academy = building["position"]
 
             if found_academy < 0:
                 print(f"No academy in this town, pick another one")
                 time.sleep(2)
                 enter()
                 event.set()
                 return
 
-            max_experiments = total_glass // 300000
-            banner()
-            print(f"How many experiments? Min=1, Max={max_experiments}")
-            choice = read(min=1, max=max_experiments)
+            if automatic is False:
+                max_experiments = total_glass // 300000
+                automatic = False
+                banner()
+                print(f"How many experiments? Min=1, Max={max_experiments}")
+                choice = read(min=1, max=max_experiments)
+
+            if automatic is True:
+                choice = 999999
 
             # Build experiments dict
             experiments["cityID"] = city["id"]
             experiments["cityName"] = city["name"]
             experiments["pos"] = found_academy
             experiments["qty"] = choice
 
             # Process
             set_child_mode(session)
             event.set()
 
-            info = f"Process: Experiments\n\nWill excecute {choice} times every 4h"
+            if automatic is False:
+                info = f"Process: Experiments\n\nWill excecute {choice} times every 4h"
+            else:
+                info = f"Process: Experiments\n\nWill excecute every 4h"
 
             try:
                 sendToBot(session, info)
-                experiment(session, experiments)
+                experiment(session, experiments, automatic)
             except Exception as e:
                 error_msg = f"Error in:\n{info}\nCause:\n{traceback.format_exc()}"
                 sendToBot(session, error_msg)
             finally:
                 session.logout()
 
     except KeyboardInterrupt:
```

### Comparing `ikabot-7.0.1/ikabot/function/killTasks.py` & `ikabot-7.0.2/ikabot/function/killTasks.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/loadCustomModule.py` & `ikabot-7.0.2/ikabot/function/loadCustomModule.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/loginDaily.py` & `ikabot-7.0.2/ikabot/function/loginDaily.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/logs.py` & `ikabot-7.0.2/ikabot/function/logs.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/proxyConf.py` & `ikabot-7.0.2/ikabot/function/proxyConf.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/searchForIslandSpaces.py` & `ikabot-7.0.2/ikabot/function/searchForIslandSpaces.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/sellResources.py` & `ikabot-7.0.2/ikabot/function/sellResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/sendResources.py` & `ikabot-7.0.2/ikabot/function/sendResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/shipMovements.py` & `ikabot-7.0.2/ikabot/function/shipMovements.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/stationArmy.py` & `ikabot-7.0.2/ikabot/function/stationArmy.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/testTelegramBot.py` & `ikabot-7.0.2/ikabot/function/testTelegramBot.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/trainArmy.py` & `ikabot-7.0.2/ikabot/function/trainArmy.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/update.py` & `ikabot-7.0.2/ikabot/function/update.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/vacationMode.py` & `ikabot-7.0.2/ikabot/function/vacationMode.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/function/webServer.py` & `ikabot-7.0.2/ikabot/function/webServer.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/aesCipher.py` & `ikabot-7.0.2/ikabot/helpers/aesCipher.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/apiComm.py` & `ikabot-7.0.2/ikabot/helpers/apiComm.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/botComm.py` & `ikabot-7.0.2/ikabot/helpers/botComm.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/dns.py` & `ikabot-7.0.2/ikabot/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/getJson.py` & `ikabot-7.0.2/ikabot/helpers/getJson.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/gui.py` & `ikabot-7.0.2/ikabot/helpers/gui.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/market.py` & `ikabot-7.0.2/ikabot/helpers/market.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/naval.py` & `ikabot-7.0.2/ikabot/helpers/naval.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/pedirInfo.py` & `ikabot-7.0.2/ikabot/helpers/pedirInfo.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/planRoutes.py` & `ikabot-7.0.2/ikabot/helpers/planRoutes.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/process.py` & `ikabot-7.0.2/ikabot/helpers/process.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/resources.py` & `ikabot-7.0.2/ikabot/helpers/resources.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/signals.py` & `ikabot-7.0.2/ikabot/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/helpers/varios.py` & `ikabot-7.0.2/ikabot/helpers/varios.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/activateMiracle.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/activateMiracle.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/aesCipher.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/aesCipher.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/alertAttacks.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/alertAttacks.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/alertLowWine.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/alertLowWine.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/botComm.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/botComm.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/buyResources.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/buyResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/command_line.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/command_line.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/config.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/config.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/constructBuilding.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/constructBuilding.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/constructionList.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/constructionList.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/distributeResources.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/distributeResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/donate.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/donate.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/donationBot.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/donationBot.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/getStatus.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/getStatus.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/gui.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/gui.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/loginDaily.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/loginDaily.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/sellResources.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/sellResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/sendResources.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/sendResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/session.mo` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/session.mo`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/session.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/session.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/shipMovements.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/shipMovements.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/signals.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/signals.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainArmy.pot` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainArmy.pot`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainFleets.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainFleets.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainTroops.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainTroops.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/update.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/update.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/vacationMode.po` & `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/vacationMode.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.1/ikabot/web/session.py` & `ikabot-7.0.2/ikabot/web/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -605,15 +605,15 @@
                     drop_target = self.s.get(
                         "https://image-drop-challenge.gameforge.com/challenge/{}/en-GB/drop-target?{}".format(
                             challenge_id, captcha_time
                         )
                     ).content
                     data = {}
                     try:
-                        captcha = getInteractiveCaptchaSolution(self, text_image, drag_icons)
+                        captcha = str(getInteractiveCaptchaSolution(self, text_image, drag_icons))
                         if not captcha.isnumeric():
                             raise Exception(
                                 "Failed to resolve interactive captcha automatically. Server returned bad data: {}".format(
                                     captcha
                                 )
                             )
                         data = {"answer": int(captcha)}
```

### Comparing `ikabot-7.0.1/ikabot.egg-info/PKG-INFO` & `ikabot-7.0.2/ikabot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikabot
-Version: 7.0.1
+Version: 7.0.2
 Home-page: https://github.com/Ikabot-Collective/ikabot
 Author: physics-sp
 Author-email: physics-sp@protonmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ikabot Version: 7.0.1 Home-page: https://
+Metadata-Version: 2.1 Name: ikabot Version: 7.0.2 Home-page: https://
 github.com/Ikabot-Collective/ikabot Author: physics-sp Author-email: physics-
 sp@protonmail.com License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: requests Requires-Dist:
 requests[socks] Requires-Dist: cryptography Requires-Dist: psutil
   ![Ikabot Banner](assets/banner.png) [![Downloads](https://static.pepy.tech/
 badge/ikabot)](https://pepy.tech/project/ikabot) ![GitHub Repo stars](https://
```

### Comparing `ikabot-7.0.1/ikabot.egg-info/SOURCES.txt` & `ikabot-7.0.2/ikabot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ikabot.egg-info/SOURCES.txt
 ikabot.egg-info/dependency_links.txt
 ikabot.egg-info/entry_points.txt
 ikabot.egg-info/requires.txt
 ikabot.egg-info/top_level.txt
 ikabot/function/__init__.py
 ikabot/function/activateMiracle.py
+ikabot/function/activateShrine.py
 ikabot/function/alertAttacks.py
 ikabot/function/alertLowWine.py
 ikabot/function/attackBarbarians.py
 ikabot/function/autoPirate.py
 ikabot/function/buyResources.py
 ikabot/function/checkForUpdate.py
 ikabot/function/constructBuilding.py
```

### Comparing `ikabot-7.0.1/setup.py` & `ikabot-7.0.2/setup.py`

 * *Files identical despite different names*

