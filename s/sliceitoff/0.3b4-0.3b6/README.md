# Comparing `tmp/sliceitoff-0.3b4.tar.gz` & `tmp/sliceitoff-0.3b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceitoff-0.3b4.tar", max compression
+gzip compressed data, was "sliceitoff-0.3b6.tar", max compression
```

## Comparing `sliceitoff-0.3b4.tar` & `sliceitoff-0.3b6.tar`

### file list

```diff
@@ -1,115 +1,119 @@
--rw-r--r--   0        0        0    18092 2010-03-23 23:34:05.000000 sliceitoff-0.3b4/LICENSE.txt
--rw-r--r--   0        0        0     1065 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/README.txt
--rw-r--r--   0        0        0     1092 2024-04-10 15:07:05.073339 sliceitoff-0.3b4/pyproject.toml
--rw-r--r--   0        0        0      105 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/__main__.py
--rw-r--r--   0        0        0       84 2024-04-07 23:52:43.859530 sliceitoff-0.3b4/src/sliceitoff/assets/fonts.lst
--rw-r--r--   0        0        0      213 2021-12-26 13:36:06.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.DE
--rw-r--r--   0        0        0      208 2021-12-26 13:36:08.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.FR
--rw-r--r--   0        0        0      606 2022-02-17 10:26:58.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM
--rw-r--r--   0        0        0      207 2022-01-30 21:46:46.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.SV
--rw-r--r--   0        0        0      211 2021-12-26 13:36:08.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.TR
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT
--rw-r--r--   0        0        0     4096 2013-05-13 14:32:08.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT
--rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT
--rw-r--r--   0        0        0      186 2024-03-29 13:01:53.951084 sliceitoff-0.3b4/src/sliceitoff/display/__init__.py
--rw-r--r--   0        0        0     1661 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/display/display.py
--rw-r--r--   0        0        0     3234 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/display/scaling.py
--rw-r--r--   0        0        0      680 2024-04-04 07:17:58.865661 sliceitoff-0.3b4/src/sliceitoff/display/static.py
--rw-r--r--   0        0        0       77 2024-03-29 16:01:18.249398 sliceitoff-0.3b4/src/sliceitoff/enemies/__init__.py
--rw-r--r--   0        0        0      995 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/enemies/ball.py
--rw-r--r--   0        0        0     1386 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/enemies/bouncher.py
--rw-r--r--   0        0        0     1301 2024-03-31 17:25:53.250046 sliceitoff-0.3b4/src/sliceitoff/enemies/enemies.py
--rw-r--r--   0        0        0     1310 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/enemies/enemy.py
--rw-r--r--   0        0        0       72 2024-03-31 17:25:53.250046 sliceitoff-0.3b4/src/sliceitoff/field/__init__.py
--rw-r--r--   0        0        0     5022 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/field/field.py
--rw-r--r--   0        0        0      113 2024-04-07 20:07:44.458257 sliceitoff-0.3b4/src/sliceitoff/game/__init__.py
--rw-r--r--   0        0        0      302 2024-03-28 21:20:33.439547 sliceitoff-0.3b4/src/sliceitoff/game/anykey.py
--rw-r--r--   0        0        0     1019 2024-04-07 20:02:27.007590 sliceitoff-0.3b4/src/sliceitoff/game/explodeout.py
--rw-r--r--   0        0        0     3009 2024-04-10 13:45:29.932810 sliceitoff-0.3b4/src/sliceitoff/game/game.py
--rw-r--r--   0        0        0     2163 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/game/gameplay.py
--rw-r--r--   0        0        0     1826 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/game/initials.py
--rw-r--r--   0        0        0     2218 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/game/level.py
--rw-r--r--   0        0        0     2433 2024-04-10 13:44:59.608502 sliceitoff-0.3b4/src/sliceitoff/game/mainmenu.py
--rw-r--r--   0        0        0      809 2024-04-07 20:51:11.974454 sliceitoff-0.3b4/src/sliceitoff/game/show.py
--rw-r--r--   0        0        0       83 2024-03-31 17:25:53.250046 sliceitoff-0.3b4/src/sliceitoff/hiscores/__init__.py
--rw-r--r--   0        0        0     2874 2024-04-10 14:57:12.122945 sliceitoff-0.3b4/src/sliceitoff/hiscores/hiscores.py
--rw-r--r--   0        0        0      493 2024-04-10 14:57:27.003047 sliceitoff-0.3b4/src/sliceitoff/hiscores/static.py
--rw-r--r--   0        0        0      170 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/main.py
--rw-r--r--   0        0        0       98 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/player/__init__.py
--rw-r--r--   0        0        0     1562 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/player/life.py
--rw-r--r--   0        0        0     1985 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/player/player.py
--rw-r--r--   0        0        0     1079 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/player/static.py
--rw-r--r--   0        0        0      412 2024-04-07 23:54:32.780119 sliceitoff-0.3b4/src/sliceitoff/screens/__init__.py
--rw-r--r--   0        0        0      338 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/screens/gameover.py
--rw-r--r--   0        0        0      391 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/screens/hiscores.py
--rw-r--r--   0        0        0      516 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/screens/initials.py
--rw-r--r--   0        0        0      769 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/screens/instructions1.py
--rw-r--r--   0        0        0      848 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/screens/instructions2.py
--rw-r--r--   0        0        0      327 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/screens/level.py
--rw-r--r--   0        0        0     1127 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/screens/levelup.py
--rw-r--r--   0        0        0      822 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/screens/mainmenu.py
--rw-r--r--   0        0        0       98 2024-03-31 17:25:53.250046 sliceitoff-0.3b4/src/sliceitoff/stats/__init__.py
--rw-r--r--   0        0        0     1435 2024-03-31 17:25:53.250046 sliceitoff-0.3b4/src/sliceitoff/stats/stats.py
--rw-r--r--   0        0        0       95 2024-03-31 17:25:53.250046 sliceitoff-0.3b4/src/sliceitoff/status/__init__.py
--rw-r--r--   0        0        0     1166 2024-04-10 13:59:33.481717 sliceitoff-0.3b4/src/sliceitoff/status/status.py
--rw-r--r--   0        0        0      178 2024-04-07 19:26:34.325877 sliceitoff-0.3b4/src/sliceitoff/text/__init__.py
--rw-r--r--   0        0        0      940 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/text/explode.py
--rw-r--r--   0        0        0     1520 2024-03-31 17:25:53.250046 sliceitoff-0.3b4/src/sliceitoff/text/fonts.py
--rw-r--r--   0        0        0     2682 2024-04-09 09:37:04.363558 sliceitoff-0.3b4/src/sliceitoff/text/text.py
--rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 sliceitoff-0.3b4/PKG-INFO
+-rw-r--r--   0        0        0    18092 2010-03-23 23:34:05.000000 sliceitoff-0.3b6/LICENSE.txt
+-rw-r--r--   0        0        0     1065 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/README.txt
+-rw-r--r--   0        0        0     1092 2024-04-20 19:32:08.368507 sliceitoff-0.3b6/pyproject.toml
+-rw-r--r--   0        0        0      105 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/__main__.py
+-rw-r--r--   0        0        0       70 2024-04-20 18:33:46.167308 sliceitoff-0.3b6/src/sliceitoff/assets/fonts.lst
+-rw-r--r--   0        0        0      213 2021-12-26 13:36:06.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.DE
+-rw-r--r--   0        0        0      208 2021-12-26 13:36:08.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.FR
+-rw-r--r--   0        0        0      606 2022-02-17 10:26:58.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM
+-rw-r--r--   0        0        0      207 2022-01-30 21:46:46.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.SV
+-rw-r--r--   0        0        0      211 2021-12-26 13:36:08.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.TR
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 12:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT
+-rw-r--r--   0        0        0     4096 2013-05-13 14:32:08.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT
+-rw-r--r--   0        0        0     4096 1994-03-28 06:00:02.000000 sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT
+-rw-r--r--   0        0        0    84622 2024-04-20 18:59:41.426924 sliceitoff-0.3b6/src/sliceitoff/assets/laser.mp3
+-rw-r--r--   0        0        0   497256 2024-04-20 17:48:25.409906 sliceitoff-0.3b6/src/sliceitoff/assets/laser.wav
+-rw-r--r--   0        0        0      186 2024-03-29 13:01:53.951084 sliceitoff-0.3b6/src/sliceitoff/display/__init__.py
+-rw-r--r--   0        0        0     1661 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/display/display.py
+-rw-r--r--   0        0        0     3234 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/display/scaling.py
+-rw-r--r--   0        0        0      680 2024-04-04 07:17:58.865661 sliceitoff-0.3b6/src/sliceitoff/display/static.py
+-rw-r--r--   0        0        0       77 2024-03-29 16:01:18.249398 sliceitoff-0.3b6/src/sliceitoff/enemies/__init__.py
+-rw-r--r--   0        0        0      995 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/enemies/ball.py
+-rw-r--r--   0        0        0     1386 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/enemies/bouncher.py
+-rw-r--r--   0        0        0     1301 2024-03-31 17:25:53.250046 sliceitoff-0.3b6/src/sliceitoff/enemies/enemies.py
+-rw-r--r--   0        0        0     1310 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/enemies/enemy.py
+-rw-r--r--   0        0        0       72 2024-03-31 17:25:53.250046 sliceitoff-0.3b6/src/sliceitoff/field/__init__.py
+-rw-r--r--   0        0        0     5022 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/field/field.py
+-rw-r--r--   0        0        0      113 2024-04-07 20:07:44.458257 sliceitoff-0.3b6/src/sliceitoff/game/__init__.py
+-rw-r--r--   0        0        0      302 2024-03-28 21:20:33.439547 sliceitoff-0.3b6/src/sliceitoff/game/anykey.py
+-rw-r--r--   0        0        0     1019 2024-04-07 20:02:27.007590 sliceitoff-0.3b6/src/sliceitoff/game/explodeout.py
+-rw-r--r--   0        0        0     3121 2024-04-20 18:32:45.444334 sliceitoff-0.3b6/src/sliceitoff/game/game.py
+-rw-r--r--   0        0        0     2220 2024-04-20 19:06:42.538581 sliceitoff-0.3b6/src/sliceitoff/game/gameplay.py
+-rw-r--r--   0        0        0     1826 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/game/initials.py
+-rw-r--r--   0        0        0     2218 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/game/level.py
+-rw-r--r--   0        0        0     2433 2024-04-10 13:44:59.608502 sliceitoff-0.3b6/src/sliceitoff/game/mainmenu.py
+-rw-r--r--   0        0        0      809 2024-04-07 20:51:11.974454 sliceitoff-0.3b6/src/sliceitoff/game/show.py
+-rw-r--r--   0        0        0       83 2024-03-31 17:25:53.250046 sliceitoff-0.3b6/src/sliceitoff/hiscores/__init__.py
+-rw-r--r--   0        0        0     2874 2024-04-10 14:57:12.122945 sliceitoff-0.3b6/src/sliceitoff/hiscores/hiscores.py
+-rw-r--r--   0        0        0      493 2024-04-10 14:57:27.003047 sliceitoff-0.3b6/src/sliceitoff/hiscores/static.py
+-rw-r--r--   0        0        0      170 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/main.py
+-rw-r--r--   0        0        0       98 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/player/__init__.py
+-rw-r--r--   0        0        0     1562 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/player/life.py
+-rw-r--r--   0        0        0     1985 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/player/player.py
+-rw-r--r--   0        0        0     1079 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/player/static.py
+-rw-r--r--   0        0        0      412 2024-04-07 23:54:32.780119 sliceitoff-0.3b6/src/sliceitoff/screens/__init__.py
+-rw-r--r--   0        0        0      338 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/screens/gameover.py
+-rw-r--r--   0        0        0      391 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/screens/hiscores.py
+-rw-r--r--   0        0        0      516 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/screens/initials.py
+-rw-r--r--   0        0        0      769 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/screens/instructions1.py
+-rw-r--r--   0        0        0      848 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/screens/instructions2.py
+-rw-r--r--   0        0        0      327 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/screens/level.py
+-rw-r--r--   0        0        0     1127 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/screens/levelup.py
+-rw-r--r--   0        0        0      822 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/screens/mainmenu.py
+-rw-r--r--   0        0        0       69 2024-04-20 18:38:32.696645 sliceitoff-0.3b6/src/sliceitoff/sfx/__init__.py
+-rw-r--r--   0        0        0     1112 2024-04-20 19:05:06.674447 sliceitoff-0.3b6/src/sliceitoff/sfx/sfx.py
+-rw-r--r--   0        0        0       98 2024-03-31 17:25:53.250046 sliceitoff-0.3b6/src/sliceitoff/stats/__init__.py
+-rw-r--r--   0        0        0     1435 2024-03-31 17:25:53.250046 sliceitoff-0.3b6/src/sliceitoff/stats/stats.py
+-rw-r--r--   0        0        0       95 2024-03-31 17:25:53.250046 sliceitoff-0.3b6/src/sliceitoff/status/__init__.py
+-rw-r--r--   0        0        0     1166 2024-04-10 13:59:33.481717 sliceitoff-0.3b6/src/sliceitoff/status/status.py
+-rw-r--r--   0        0        0      178 2024-04-07 19:26:34.325877 sliceitoff-0.3b6/src/sliceitoff/text/__init__.py
+-rw-r--r--   0        0        0      940 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/text/explode.py
+-rw-r--r--   0        0        0     1510 2024-04-20 18:33:11.667867 sliceitoff-0.3b6/src/sliceitoff/text/fonts.py
+-rw-r--r--   0        0        0     2682 2024-04-09 09:37:04.363558 sliceitoff-0.3b6/src/sliceitoff/text/text.py
+-rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 sliceitoff-0.3b6/PKG-INFO
```

### Comparing `sliceitoff-0.3b4/LICENSE.txt` & `sliceitoff-0.3b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/README.txt` & `sliceitoff-0.3b6/README.txt`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/pyproject.toml` & `sliceitoff-0.3b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sliceitoff"
-version = "0.3-beta.4"
+version = "0.3-beta.6"
 description = "Arcade game where one slices play area off while avoiding slicing happy faces."
 repository = "https://git.hix.fi/sliceitoff.git/"
 authors = ["Viljami Ilola <+@hix.fi>"]
 readme = "README.txt"
 packages = [{include = "sliceitoff", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT` & `sliceitoff-0.3b6/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/display/display.py` & `sliceitoff-0.3b6/src/sliceitoff/display/display.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/display/scaling.py` & `sliceitoff-0.3b6/src/sliceitoff/display/scaling.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/display/static.py` & `sliceitoff-0.3b6/src/sliceitoff/display/static.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/enemies/ball.py` & `sliceitoff-0.3b6/src/sliceitoff/enemies/ball.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/enemies/bouncher.py` & `sliceitoff-0.3b6/src/sliceitoff/enemies/bouncher.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/enemies/enemies.py` & `sliceitoff-0.3b6/src/sliceitoff/enemies/enemies.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/enemies/enemy.py` & `sliceitoff-0.3b6/src/sliceitoff/enemies/enemy.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/field/field.py` & `sliceitoff-0.3b6/src/sliceitoff/field/field.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/game/explodeout.py` & `sliceitoff-0.3b6/src/sliceitoff/game/explodeout.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/game/game.py` & `sliceitoff-0.3b6/src/sliceitoff/game/game.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,29 +10,32 @@
 from sliceitoff.text import Fonts
 from sliceitoff.stats import Stats
 from sliceitoff.screens import (
     hiscores_screen,
     instructions1_screen,
     instructions2_screen)
 from sliceitoff.hiscores import HiScores
+from sliceitoff.sfx import sfx
 
 from .mainmenu import Mainmenu, MenuItems
 from .level import Level
 from .show import Show
 from .initials import Initials
 
 class Game:
     """ This is the whole game. """
     def __init__(self):
+        assets_path = Path(__file__).parent.parent.resolve().joinpath('assets')
         pygame.init()
+        sfx.init(assets_path)
         self.clock = pygame.time.Clock()
         self.display = Display()
         self.stats = None
         self.hiscores = HiScores()
-        Fonts.load_fonts( Path(__file__).parent.parent.resolve() )
+        Fonts.load_fonts(assets_path)
         pygame.mouse.set_visible(False)
 
     def __del__(self):
         pygame.quit()
 
     def instructions(self):
         """ displays instruction and waits a key """
```

### Comparing `sliceitoff-0.3b4/src/sliceitoff/game/gameplay.py` & `sliceitoff-0.3b6/src/sliceitoff/game/gameplay.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Reads user input and does actions when game play is on. """
 import pygame
+from sliceitoff.sfx import sfx
 
 class Gameplay:
     """ Logic of the playfield """
     def __init__(
             self,
             player = None,
             field = None,
@@ -21,14 +22,15 @@
         zap_sprite = self.field.slice(
                 self.player.position,
                 self.player.direction,
                 4_000)
         if not zap_sprite:
             return False
         self.stats.add_score(-500)
+        sfx.play("laser")
         if pygame.sprite.spritecollideany(zap_sprite, self.enemies):
             self.life.lose_life()
             if self.stats.lose_life():
                 return True
         self.field.kill_if_not_colliding(self.enemies.sprites())
         self.field.update_stats()
         return self.stats.percent < 20
```

### Comparing `sliceitoff-0.3b4/src/sliceitoff/game/initials.py` & `sliceitoff-0.3b6/src/sliceitoff/game/initials.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/game/level.py` & `sliceitoff-0.3b6/src/sliceitoff/game/level.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/game/mainmenu.py` & `sliceitoff-0.3b6/src/sliceitoff/game/mainmenu.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/game/show.py` & `sliceitoff-0.3b6/src/sliceitoff/game/show.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/hiscores/hiscores.py` & `sliceitoff-0.3b6/src/sliceitoff/hiscores/hiscores.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/player/life.py` & `sliceitoff-0.3b6/src/sliceitoff/player/life.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/player/player.py` & `sliceitoff-0.3b6/src/sliceitoff/player/player.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/player/static.py` & `sliceitoff-0.3b6/src/sliceitoff/player/static.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/screens/initials.py` & `sliceitoff-0.3b6/src/sliceitoff/screens/initials.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/screens/instructions1.py` & `sliceitoff-0.3b6/src/sliceitoff/screens/instructions1.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/screens/instructions2.py` & `sliceitoff-0.3b6/src/sliceitoff/screens/instructions2.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/screens/levelup.py` & `sliceitoff-0.3b6/src/sliceitoff/screens/levelup.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/screens/mainmenu.py` & `sliceitoff-0.3b6/src/sliceitoff/screens/mainmenu.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/stats/stats.py` & `sliceitoff-0.3b6/src/sliceitoff/stats/stats.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/status/status.py` & `sliceitoff-0.3b6/src/sliceitoff/status/status.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/text/explode.py` & `sliceitoff-0.3b6/src/sliceitoff/text/explode.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/src/sliceitoff/text/fonts.py` & `sliceitoff-0.3b6/src/sliceitoff/text/fonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class Fonts:
     """ Fonts - static class to store loaded fonts """
     fonts = {}
 
     @staticmethod
     def load_fonts(base_path):
         """ loads fonts from list """
-        filename_fontlist = os.path.join(base_path, "assets", "fonts.lst")
+        filename_fontlist = os.path.join(base_path, "fonts.lst")
         with open(filename_fontlist, "r", encoding="utf-8") as fontlist_file:
             for line in fontlist_file:
                 name, *path = line.strip().split()
                 filename = os.path.join(base_path, *path)
                 __class__.fonts[name] = Font(filename)
         return True
```

### Comparing `sliceitoff-0.3b4/src/sliceitoff/text/text.py` & `sliceitoff-0.3b6/src/sliceitoff/text/text.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b4/PKG-INFO` & `sliceitoff-0.3b6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceitoff
-Version: 0.3b4
+Version: 0.3b6
 Summary: Arcade game where one slices play area off while avoiding slicing happy faces.
 Home-page: https://git.hix.fi/sliceitoff.git/
 Author: Viljami Ilola
 Author-email: +@hix.fi
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

