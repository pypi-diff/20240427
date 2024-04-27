# Comparing `tmp/zanthor-1.2.3.tar.gz` & `tmp/zanthor-1.2.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zanthor-1.2.3.tar", last modified: Thu Mar  3 12:29:23 2011, max compression, from Unix
+gzip compressed data, was "zanthor-1.2.4a2.tar", last modified: Sat Apr 27 20:09:55 2024, max compression
```

## Comparing `zanthor-1.2.3.tar` & `zanthor-1.2.4a2.tar`

### file list

```diff
@@ -1,319 +1,328 @@
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/
--rw-r--r--   0 rene      (1000) rene      (1000)      111 2011-03-03 11:01:19.000000 zanthor-1.2.3/run_game.py
--rwxr-xr-x   0 rene      (1000) rene      (1000)     7699 2011-03-03 12:28:40.000000 zanthor-1.2.3/setup.py
--rw-r--r--   0 rene      (1000) rene      (1000)     1081 2011-03-03 12:29:22.000000 zanthor-1.2.3/PKG-INFO
--rw-r--r--   0 rene      (1000) rene      (1000)     1852 2011-03-03 11:01:19.000000 zanthor-1.2.3/BUGS.txt
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/
--rw-r--r--   0 rene      (1000) rene      (1000)       59 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/__init__.py
--rw-r--r--   0 rene      (1000) rene      (1000)     9496 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/sounds.py
--rw-r--r--   0 rene      (1000) rene      (1000)     1342 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/factory.py
--rw-r--r--   0 rene      (1000) rene      (1000)      344 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/util.py
--rw-r--r--   0 rene      (1000) rene      (1000)      926 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/sound_info.py
--rw-r--r--   0 rene      (1000) rene      (1000)     4386 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/messages.py
--rw-r--r--   0 rene      (1000) rene      (1000)     1275 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/cyclic_list.py
--rw-r--r--   0 rene      (1000) rene      (1000)    16489 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/html.py
--rw-r--r--   0 rene      (1000) rene      (1000)     9810 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/states.py
--rw-r--r--   0 rene      (1000) rene      (1000)    18818 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/level.py
--rw-r--r--   0 rene      (1000) rene      (1000)     4998 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/explode.py
--rw-r--r--   0 rene      (1000) rene      (1000)     3843 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/intro.py
--rw-r--r--   0 rene      (1000) rene      (1000)    13294 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/units.py
--rw-r--r--   0 rene      (1000) rene      (1000)     4003 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/items.py
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/data/
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/data/gfx/
--rw-r--r--   0 rene      (1000) rene      (1000)   487584 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/caastles.png
--rw-r--r--   0 rene      (1000) rene      (1000)    32375 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/background_illustration.png
--rw-r--r--   0 rene      (1000) rene      (1000)    13069 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/heart.xcf.bz2
--rw-r--r--   0 rene      (1000) rene      (1000)      249 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/tileedit.ini
--rw-r--r--   0 rene      (1000) rene      (1000)    87812 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/tiles.tga
--rw-r--r--   0 rene      (1000) rene      (1000)    30627 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/background_equipment.png
--rw-r--r--   0 rene      (1000) rene      (1000)     1463 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/hairs.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      852 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/coal.png
--rw-r--r--   0 rene      (1000) rene      (1000)    76032 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/background_bottom.png
--rw-r--r--   0 rene      (1000) rene      (1000)     1013 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/hole2.png
--rw-r--r--   0 rene      (1000) rene      (1000)    81736 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/tiles2.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      655 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/hole.png
--rw-r--r--   0 rene      (1000) rene      (1000)      402 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/castle1.png
--rw-r--r--   0 rene      (1000) rene      (1000)    27136 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/background_status_left.png
--rw-r--r--   0 rene      (1000) rene      (1000)     2147 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/heart_pulse.png
--rw-r--r--   0 rene      (1000) rene      (1000)     8236 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/castle1.tga
--rwxr-xr-x   0 rene      (1000) rene      (1000)    34808 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/tileedit.py
--rw-r--r--   0 rene      (1000) rene      (1000)     2206 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/hole4.png
--rw-r--r--   0 rene      (1000) rene      (1000)     1476 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/heart.png
--rw-r--r--   0 rene      (1000) rene      (1000)     3750 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/gfx/hole3.png
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/data/intro/
--rw-r--r--   0 rene      (1000) rene      (1000)    31304 2011-03-03 11:01:17.000000 zanthor-1.2.3/zanthor/data/intro/ETHNOCEN.TTF
--rw-r--r--   0 rene      (1000) rene      (1000)   656299 2011-03-03 11:01:18.000000 zanthor-1.2.3/zanthor/data/intro/soundtrack2.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)   804138 2011-03-03 11:01:18.000000 zanthor-1.2.3/zanthor/data/intro/grass.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    91644 2011-03-03 11:01:17.000000 zanthor-1.2.3/zanthor/data/intro/dazzlesh.ttf
--rw-r--r--   0 rene      (1000) rene      (1000)     9848 2011-03-03 11:01:17.000000 zanthor-1.2.3/zanthor/data/intro/read_me.html
--rw-r--r--   0 rene      (1000) rene      (1000)   101753 2011-03-03 11:01:17.000000 zanthor-1.2.3/zanthor/data/intro/intro1.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    54509 2011-03-03 11:01:18.000000 zanthor-1.2.3/zanthor/data/intro/mybkgr.png
--rw-r--r--   0 rene      (1000) rene      (1000)    32033 2011-03-03 11:01:17.000000 zanthor-1.2.3/zanthor/data/intro/title.jpg
--rw-r--r--   0 rene      (1000) rene      (1000)   596043 2011-03-03 11:01:18.000000 zanthor-1.2.3/zanthor/data/intro/soundtrack1.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)   457195 2011-03-03 11:01:17.000000 zanthor-1.2.3/zanthor/data/intro/zanthor.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    36748 2011-03-03 11:01:17.000000 zanthor-1.2.3/zanthor/data/intro/WALSHES.TTF
--rw-r--r--   0 rene      (1000) rene      (1000)    87309 2011-03-03 11:01:17.000000 zanthor-1.2.3/zanthor/data/intro/introbg.png
--rw-r--r--   0 rene      (1000) rene      (1000)   633397 2011-03-03 11:01:18.000000 zanthor-1.2.3/zanthor/data/intro/soundtrack3.ogg
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/data/sounds/
--rw-r--r--   0 rene      (1000) rene      (1000)    48976 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/peasants1.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    17739 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/cannon2.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    11336 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/hitground.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    11079 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/squish2.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    30450 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/water.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    31104 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/peasants2.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    46232 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/peasants3.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    28681 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/birds1.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    23243 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/ouch2.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    20374 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/upgrade.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    12053 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/hitenemy.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    82275 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/birds2.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    24014 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/hitwall2.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    17630 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/cannon3.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)   272104 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/engine-fast.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    17430 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/cannon.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    18019 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/coal.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    24075 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/ouch1.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)     5437 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/squish1.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)   405886 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/engine-slow.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    23130 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/destroyenemy.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    17332 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/hitwall.ogg
--rw-r--r--   0 rene      (1000) rene      (1000)    33840 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/data/sounds/release.ogg
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/data/themes/
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/data/themes/default/
--rw-r--r--   0 rene      (1000) rene      (1000)      864 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/vslider.up.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      172 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/list.item.hover.png
--rw-r--r--   0 rene      (1000) rene      (1000)     1278 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/scroller.slide.v.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1278 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/scroller.slide.h.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      634 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/filebrowser.folder.png
--rw-r--r--   0 rene      (1000) rene      (1000)     1412 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/vslider.bar.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      172 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/select.option.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      363 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/select.arrow.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1412 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/vslider.bar.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      320 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/checkbox.off.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      338 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/select.selected.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      529 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/rdot.hover.png
--rw-r--r--   0 rene      (1000) rene      (1000)      190 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/list.item.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      354 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/vdot.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      205 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/check.png
--rw-r--r--   0 rene      (1000) rene      (1000)      242 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/box.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      324 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/box.hover.png
--rw-r--r--   0 rene      (1000) rene      (1000)      441 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/menu.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      372 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/hslider.right.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      129 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/list.png
--rw-r--r--   0 rene      (1000) rene      (1000)      582 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/dialog.close.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      181 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/desktop.png
--rw-r--r--   0 rene      (1000) rene      (1000)      370 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/rdot.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      322 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/dialog.png
--rw-r--r--   0 rene      (1000) rene      (1000)      776 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/slider.bar.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      563 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/progressbar.bar.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      528 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/tool.down.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      108 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/notes.txt
--rw-r--r--   0 rene      (1000) rene      (1000)      322 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/select.selected.down.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      199 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/x.png
--rw-r--r--   0 rene      (1000) rene      (1000)      412 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/progressbar.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      206 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/right.png
--rw-r--r--   0 rene      (1000) rene      (1000)      181 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/input.focus.png
--rw-r--r--   0 rene      (1000) rene      (1000)      363 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/select.arrow.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      528 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/menu.down.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      181 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/select.options.png
--rw-r--r--   0 rene      (1000) rene      (1000)      232 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/sbox.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      776 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/hslider.bar.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      172 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/list.item.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      776 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/button.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      342 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/scroller.slide.bar.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      729 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/hslider.bar.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      156 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/select.arrow.png
--rw-r--r--   0 rene      (1000) rene      (1000)      197 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/radio.png
--rw-r--r--   0 rene      (1000) rene      (1000)      233 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/vbox.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      190 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/select.option.hover.png
--rw-r--r--   0 rene      (1000) rene      (1000)      500 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/checkbox.on.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      668 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/dialog.close.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     2004 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/box.xcf
--rw-r--r--   0 rene      (1000) rene      (1000)      224 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/console.input.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      786 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/button.down.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      282 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/select.selected.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      344 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/select.arrow.down.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      224 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/console.input.focus.png
--rw-r--r--   0 rene      (1000) rene      (1000)      366 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/dot.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      442 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/checkbox.off.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1231 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/hslider.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      582 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/radio.off.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      202 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      195 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/up.png
--rw-r--r--   0 rene      (1000) rene      (1000)      864 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/vslider.down.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      372 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/hslider.left.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      563 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/tool.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      329 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/dialog.bar.png
--rw-r--r--   0 rene      (1000) rene      (1000)       78 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/menu.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      540 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/vdot.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)     1231 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/slider.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      527 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/vdot.hover.png
--rw-r--r--   0 rene      (1000) rene      (1000)      677 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/dialog.close.down.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      537 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/radio.off.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     3501 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/generate.py
--rw-r--r--   0 rene      (1000) rene      (1000)      525 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/rdot.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      795 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/out.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      729 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/button.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     2226 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/listitem.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      637 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/radio.on.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     2226 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/listitem.down.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      342 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/scroller.slide.bar.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     2322 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/listitem.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)    65932 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/Vera.ttf
--rw-r--r--   0 rene      (1000) rene      (1000)      408 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/idot.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      208 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/input.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)     1231 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/vslider.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     7676 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/config.txt
--rw-r--r--   0 rene      (1000) rene      (1000)      441 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/tool.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      646 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/radio.on.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      312 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/box.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      209 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/left.png
--rw-r--r--   0 rene      (1000) rene      (1000)      224 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/vsbox.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      548 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/dot.hover.png
--rw-r--r--   0 rene      (1000) rene      (1000)     1930 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/dot.xcf
--rw-r--r--   0 rene      (1000) rene      (1000)      535 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/checkbox.on.hover.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      729 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/slider.bar.normal.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      224 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/console.png
--rw-r--r--   0 rene      (1000) rene      (1000)      549 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/dot.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)     1975 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/default/desktop.xcf
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/data/themes/gray/
--rw-r--r--   0 rene      (1000) rene      (1000)      145 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/slider.png
--rw-r--r--   0 rene      (1000) rene      (1000)      224 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/radio.off.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      217 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/dialog.close.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      634 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/filebrowser.folder.png
--rw-r--r--   0 rene      (1000) rene      (1000)      172 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/select.option.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      213 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/checkbox.on.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      178 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/checkbox.off.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      230 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/box.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      129 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/list.png
--rw-r--r--   0 rene      (1000) rene      (1000)      131 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/desktop.png
--rw-r--r--   0 rene      (1000) rene      (1000)      138 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/dialog.png
--rw-r--r--   0 rene      (1000) rene      (1000)      181 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/input.focus.png
--rw-r--r--   0 rene      (1000) rene      (1000)      147 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/menu.option.hover.png
--rw-r--r--   0 rene      (1000) rene      (1000)      181 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/select.options.png
--rw-r--r--   0 rene      (1000) rene      (1000)      172 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/list.item.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      168 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/tool.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      135 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/select.selected.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      168 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/tool.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      156 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/select.arrow.png
--rw-r--r--   0 rene      (1000) rene      (1000)      120 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/menu.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      270 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/dialog.close.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      165 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/checkbox.off.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      181 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/slider.bar.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      131 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/menu.option.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      224 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/console.input.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      224 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/console.input.focus.png
--rw-r--r--   0 rene      (1000) rene      (1000)      138 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/dialog.bar.png
--rw-r--r--   0 rene      (1000) rene      (1000)      238 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/radio.off.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      191 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/button.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)    65932 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/Vera.ttf
--rw-r--r--   0 rene      (1000) rene      (1000)      216 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/checkbox.on.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      250 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/radio.on.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      208 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/input.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)     6317 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/config.txt
--rw-r--r--   0 rene      (1000) rene      (1000)      248 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/radio.on.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      225 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/box.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      199 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/button.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      150 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/menu.hover.png
--rw-r--r--   0 rene      (1000) rene      (1000)      149 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/select.arrow.down.png
--rw-r--r--   0 rene      (1000) rene      (1000)      224 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/console.png
--rw-r--r--   0 rene      (1000) rene      (1000)      168 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/select.arrow.normal.png
--rw-r--r--   0 rene      (1000) rene      (1000)      149 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/themes/gray/menu.down.png
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/data/themes/tools/
--rw-r--r--   0 rene      (1000) rene      (1000)     1443 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/themes/tools/icons48.draw.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1595 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/themes/tools/icons48.bkgr.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1268 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/themes/tools/icons48.tile.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1360 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/themes/tools/icons48.code.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1141 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/themes/tools/icons48.line.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1221 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/themes/tools/icons48.fill.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1210 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/themes/tools/icons48.pixel.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1457 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/themes/tools/icons48.select.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      309 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/themes/tools/config.txt
--rw-r--r--   0 rene      (1000) rene      (1000)     1381 2011-03-03 11:01:11.000000 zanthor-1.2.3/zanthor/data/themes/tools/icons48.eraser.tga
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/data/levels/
--rw-r--r--   0 rene      (1000) rene      (1000)      235 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/test.tga
--rw-r--r--   0 rene      (1000) rene      (1000)    18577 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/codes.tga
--rw-r--r--   0 rene      (1000) rene      (1000)      585 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/tileedit.ini
--rw-r--r--   0 rene      (1000) rene      (1000)     1125 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/level1.tga
--rw-r--r--   0 rene      (1000) rene      (1000)    10843 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/tiles.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     6423 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/level5.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     7002 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/level7.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1613 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/level2.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1093 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/level4.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1458 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/level3.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1950 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/test2.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     2052 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/test4.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     4984 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/level6.tga
--rw-r--r--   0 rene      (1000) rene      (1000)     1675 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/leveledit.ini
--rw-r--r--   0 rene      (1000) rene      (1000)     9914 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/level8.tga
--rwxr-xr-x   0 rene      (1000) rene      (1000)    41404 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/leveledit.py
--rw-r--r--   0 rene      (1000) rene      (1000)     3653 2011-03-03 11:01:12.000000 zanthor-1.2.3/zanthor/data/levels/test3.tga
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/data/menu/
--rw-r--r--   0 rene      (1000) rene      (1000)     1599 2011-03-03 11:01:09.000000 zanthor-1.2.3/zanthor/data/menu/x.png
--rw-r--r--   0 rene      (1000) rene      (1000)     9848 2011-03-03 11:01:09.000000 zanthor-1.2.3/zanthor/data/menu/read_me.html
--rw-r--r--   0 rene      (1000) rene      (1000)    22022 2011-03-03 11:01:09.000000 zanthor-1.2.3/zanthor/data/menu/map.png
--rw-r--r--   0 rene      (1000) rene      (1000)    42872 2011-03-03 11:01:09.000000 zanthor-1.2.3/zanthor/data/menu/vinque.ttf
--rw-r--r--   0 rene      (1000) rene      (1000)    24623 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/castle.py
--rw-r--r--   0 rene      (1000) rene      (1000)    17918 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/interface.py
--rw-r--r--   0 rene      (1000) rene      (1000)     3060 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/truck.py
--rw-r--r--   0 rene      (1000) rene      (1000)      409 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/_effects.py
--rw-r--r--   0 rene      (1000) rene      (1000)     3051 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/fire.py
--rw-r--r--   0 rene      (1000) rene      (1000)     5922 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/main.py
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/pgu/
--rw-r--r--   0 rene      (1000) rene      (1000)      105 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/__init__.py
--rw-r--r--   0 rene      (1000) rene      (1000)     6413 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/tilevid.py
--rw-r--r--   0 rene      (1000) rene      (1000)       80 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/layout.py
--rw-r--r--   0 rene      (1000) rene      (1000)    16424 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/html.py
--rw-r--r--   0 rene      (1000) rene      (1000)     4029 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/high.py
--rw-r--r--   0 rene      (1000) rene      (1000)     1781 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/text.py
--rw-r--r--   0 rene      (1000) rene      (1000)     4116 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/fonts.py
--rw-r--r--   0 rene      (1000) rene      (1000)    17144 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/vid.py
--rw-r--r--   0 rene      (1000) rene      (1000)     3077 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/ani.py
--rw-r--r--   0 rene      (1000) rene      (1000)     4168 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/hexvid.py
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/zanthor/pgu/gui/
--rw-r--r--   0 rene      (1000) rene      (1000)     5139 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/surface.py
--rw-r--r--   0 rene      (1000) rene      (1000)      832 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/__init__.py
--rw-r--r--   0 rene      (1000) rene      (1000)     5873 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/app.py
--rw-r--r--   0 rene      (1000) rene      (1000)    12768 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/table.py
--rw-r--r--   0 rene      (1000) rene      (1000)     5027 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/layout.py
--rw-r--r--   0 rene      (1000) rene      (1000)     4993 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/dialog.py
--rw-r--r--   0 rene      (1000) rene      (1000)    14758 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/theme.py
--rw-r--r--   0 rene      (1000) rene      (1000)     1166 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/style.py
--rw-r--r--   0 rene      (1000) rene      (1000)     1143 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/group.py
--rw-r--r--   0 rene      (1000) rene      (1000)     8129 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/slider.py
--rw-r--r--   0 rene      (1000) rene      (1000)    13479 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/area.py
--rw-r--r--   0 rene      (1000) rene      (1000)     2343 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/deprecated.py
--rw-r--r--   0 rene      (1000) rene      (1000)    11343 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/container.py
--rw-r--r--   0 rene      (1000) rene      (1000)     1993 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/form.py
--rw-r--r--   0 rene      (1000) rene      (1000)     3726 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/menus.py
--rw-r--r--   0 rene      (1000) rene      (1000)     4566 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/input.py
--rw-r--r--   0 rene      (1000) rene      (1000)     3065 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/document.py
--rw-r--r--   0 rene      (1000) rene      (1000)     2087 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/keysym.py
--rw-r--r--   0 rene      (1000) rene      (1000)     2501 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/basic.py
--rw-r--r--   0 rene      (1000) rene      (1000)     5608 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/select.py
--rw-r--r--   0 rene      (1000) rene      (1000)     9249 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/button.py
--rw-r--r--   0 rene      (1000) rene      (1000)     9970 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/widget.py
--rw-r--r--   0 rene      (1000) rene      (1000)      757 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/const.py
--rw-r--r--   0 rene      (1000) rene      (1000)     1159 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/gui/misc.py
--rw-r--r--   0 rene      (1000) rene      (1000)     3603 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/algo.py
--rw-r--r--   0 rene      (1000) rene      (1000)     1554 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/timer.py
--rw-r--r--   0 rene      (1000) rene      (1000)     5582 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/isovid.py
--rw-r--r--   0 rene      (1000) rene      (1000)     4202 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/pgu/engine.py
--rw-r--r--   0 rene      (1000) rene      (1000)     1996 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/cannon.py
--rw-r--r--   0 rene      (1000) rene      (1000)    11477 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/menu.py
--rw-r--r--   0 rene      (1000) rene      (1000)     3959 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/steam.py
--rw-r--r--   0 rene      (1000) rene      (1000)      157 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/human.py
--rw-r--r--   0 rene      (1000) rene      (1000)     5982 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/title.py
--rw-r--r--   0 rene      (1000) rene      (1000)     3601 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/algo.py
--rw-r--r--   0 rene      (1000) rene      (1000)     2826 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/tiles.py
--rw-r--r--   0 rene      (1000) rene      (1000)    15287 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/isovid.py
--rw-r--r--   0 rene      (1000) rene      (1000)     5773 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/flock.py
--rw-r--r--   0 rene      (1000) rene      (1000)      344 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/effect.py
--rw-r--r--   0 rene      (1000) rene      (1000)     6467 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/robot.py
--rw-r--r--   0 rene      (1000) rene      (1000)     3864 2011-03-03 11:01:19.000000 zanthor-1.2.3/zanthor/const.py
--rw-r--r--   0 rene      (1000) rene      (1000)      988 2011-03-03 11:01:19.000000 zanthor-1.2.3/README.txt
--rw-r--r--   0 rene      (1000) rene      (1000)       50 2011-03-03 11:14:21.000000 zanthor-1.2.3/CHANGES.txt
--rw-r--r--   0 rene      (1000) rene      (1000)     1348 2009-10-13 01:02:58.000000 zanthor-1.2.3/TODO.txt
-drwxr-xr-x   0 rene      (1000) rene      (1000)        0 2011-03-03 12:29:22.000000 zanthor-1.2.3/scripts/
--rwxr-xr-x   0 rene      (1000) rene      (1000)       95 2011-03-03 11:01:19.000000 zanthor-1.2.3/scripts/zanthor
--rw-r--r--   0 rene      (1000) rene      (1000)    18032 2008-10-14 08:51:50.000000 zanthor-1.2.3/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.051908 zanthor-1.2.4a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-27 20:09:55.051908 zanthor-1.2.4a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 20:09:55.051908 zanthor-1.2.4a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1905 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.003908 zanthor-1.2.4a2/zanthor/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/algo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/cannon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25254 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/castle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/cyclic_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:54.995908 zanthor-1.2.4a2/zanthor/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.007908 zanthor-1.2.4a2/zanthor/data/gfx/
+-rw-r--r--   0 runner    (1001) docker     (127)    76032 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/background_bottom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30627 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/background_equipment.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32375 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/background_illustration.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27136 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/background_status_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)   487584 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/caastles.png
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/castle1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/castle1.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/coal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/hairs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/hairs.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/heart.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13069 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/heart.xcf.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/heart_pulse.png
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/hole.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/hole2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/hole3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/hole4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/tileedit.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38111 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/tileedit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42958 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/tiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)    87812 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/tiles.tga
+-rw-r--r--   0 runner    (1001) docker     (127)    42232 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/tiles2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81736 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/gfx/tiles2.tga
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.015908 zanthor-1.2.4a2/zanthor/data/intro/
+-rw-r--r--   0 runner    (1001) docker     (127)    31304 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/ETHNOCEN.TTF
+-rw-r--r--   0 runner    (1001) docker     (127)    36748 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/WALSHES.TTF
+-rw-r--r--   0 runner    (1001) docker     (127)    91644 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/dazzlesh.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   804138 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/grass.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)   101753 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/intro1.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    87309 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/introbg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54509 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/mybkgr.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/read_me.html
+-rw-r--r--   0 runner    (1001) docker     (127)   596043 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/soundtrack1.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)   656299 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/soundtrack2.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)   633397 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/soundtrack3.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    32033 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/title.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   457195 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/intro/zanthor.ogg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.015908 zanthor-1.2.4a2/zanthor/data/levels/
+-rw-r--r--   0 runner    (1001) docker     (127)    18577 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/codes.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/level1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/level1.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/level2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/level2.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/level3.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/level4.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/level5.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/level6.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/level7.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/level8.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/leveledit.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42909 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/leveledit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/test.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/test2.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/test3.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/test4.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/tileedit.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    10843 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/levels/tiles.tga
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.019908 zanthor-1.2.4a2/zanthor/data/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)    22022 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/menu/map.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/menu/read_me.html
+-rw-r--r--   0 runner    (1001) docker     (127)    42872 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/menu/vinque.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/menu/x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.023908 zanthor-1.2.4a2/zanthor/data/sounds/
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/birds1.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    82275 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/birds2.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    17430 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/cannon.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    17739 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/cannon2.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/cannon3.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/coal.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/destroyenemy.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)   272104 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/engine-fast.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)   405886 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/engine-slow.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    12053 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/hitenemy.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/hitground.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    17332 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/hitwall.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    24014 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/hitwall2.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    24075 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/ouch1.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    23243 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/ouch2.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    48976 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/peasants1.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    31104 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/peasants2.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    46232 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/peasants3.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    33840 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/release.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/squish1.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/squish2.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    20374 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/upgrade.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)    30450 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/sounds/water.ogg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:54.995908 zanthor-1.2.4a2/zanthor/data/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.039908 zanthor-1.2.4a2/zanthor/data/themes/default/
+-rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/Vera.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/box.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/box.hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/box.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/box.xcf
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/button.down.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/button.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/button.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/check.png
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/checkbox.off.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/checkbox.off.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/checkbox.on.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/checkbox.on.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/config.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/console.input.focus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/console.input.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/console.png
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/desktop.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/desktop.xcf
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/dialog.bar.png
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/dialog.close.down.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/dialog.close.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/dialog.close.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/dot.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/dot.hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/dot.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/dot.xcf
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/filebrowser.folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/hslider.bar.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/hslider.bar.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/hslider.left.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/hslider.right.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/hslider.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/idot.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/input.focus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/input.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/left.png
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/list.item.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/list.item.hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/list.item.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/list.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/listitem.down.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/listitem.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/listitem.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/menu.down.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/menu.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/menu.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/notes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/out.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/progressbar.bar.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/progressbar.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/radio.off.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/radio.off.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/radio.on.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/radio.on.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/radio.png
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/rdot.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/rdot.hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/rdot.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/sbox.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/scroller.slide.bar.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/scroller.slide.bar.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/scroller.slide.h.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/scroller.slide.v.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/select.arrow.down.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/select.arrow.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/select.arrow.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/select.arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/select.option.hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/select.option.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/select.options.png
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/select.selected.down.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/select.selected.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/select.selected.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/slider.bar.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/slider.bar.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/slider.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/tool.down.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/tool.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/tool.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/up.png
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/vbox.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/vdot.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/vdot.hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/vdot.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/vsbox.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/vslider.bar.hover.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/vslider.bar.normal.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/vslider.down.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/vslider.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/vslider.up.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/default/x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.043908 zanthor-1.2.4a2/zanthor/data/themes/gray/
+-rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/Vera.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/box.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/box.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/button.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/button.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/checkbox.off.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/checkbox.off.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/checkbox.on.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/checkbox.on.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/config.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/console.input.focus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/console.input.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/console.png
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/desktop.png
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/dialog.bar.png
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/dialog.close.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/dialog.close.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/filebrowser.folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/input.focus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/input.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/list.item.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/list.png
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/menu.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/menu.hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/menu.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/menu.option.hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/menu.option.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/radio.off.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/radio.off.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/radio.on.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/radio.on.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/select.arrow.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/select.arrow.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/select.arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/select.option.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/select.options.png
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/select.selected.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/slider.bar.normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/slider.png
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/tool.down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/gray/tool.normal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.047908 zanthor-1.2.4a2/zanthor/data/themes/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/tools/config.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.bkgr.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.code.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.draw.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.eraser.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.fill.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.line.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.pixel.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.select.tga
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.tile.tga
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/explode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/fire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/flock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/human.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17835 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/intro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15776 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/isovid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.047908 zanthor-1.2.4a2/zanthor/pgu/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/algo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.051908 zanthor-1.2.4a2/zanthor/pgu/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/keysym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/menus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16011 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/gui/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/hexvid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/high.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/isovid.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/tilevid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17468 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/pgu/vid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/sound_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/sounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/tiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/truck.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-27 20:09:51.000000 zanthor-1.2.4a2/zanthor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:09:55.051908 zanthor-1.2.4a2/zanthor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-27 20:09:54.000000 zanthor-1.2.4a2/zanthor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-04-27 20:09:54.000000 zanthor-1.2.4a2/zanthor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 20:09:54.000000 zanthor-1.2.4a2/zanthor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-27 20:09:54.000000 zanthor-1.2.4a2/zanthor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 20:09:54.000000 zanthor-1.2.4a2/zanthor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 20:09:54.000000 zanthor-1.2.4a2/zanthor.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zanthor-1.2.3/zanthor/sounds.py` & `zanthor-1.2.4a2/zanthor/sounds.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,354 +6,317 @@
 
 NOTE: not using pygames channel queueing as it only allows one sound to be 
   queued.  Also the sound can only be queued on a certain channel.
 
 """
 
 
-
 import pygame
 import os
 import glob
 import time
 
 from pygame.locals import *
-from const import data_dir
+from .const import data_dir
 
 SOUND_PATH = data_dir("sounds")
 
 
 EXTENSIONS = [".wav", ".ogg"]
 
-def get_sound_list(path = SOUND_PATH, extensions = EXTENSIONS):
-    """ gets a list of sound names without thier path, or extension.
-    """
+
+def get_sound_list(path=SOUND_PATH, extensions=EXTENSIONS):
+    """gets a list of sound names without thier path, or extension."""
     # load a list of sounds without path at the beginning and .ogg at the end.
     sound_list = []
     for ext in extensions:
-        sound_list.extend( map(lambda x:x[len(path)+1:-4], 
-                               glob.glob(os.path.join(path,"*" + ext)) 
-                           ))
+        sound_list.extend(
+            [x[len(path) + 1 : -4] for x in glob.glob(os.path.join(path, "*" + ext))]
+        )
 
     return sound_list
-       
+
 
 SOUND_LIST = get_sound_list()
 
-def init(path = SOUND_PATH):
-    """
-    """
+
+def init(path=SOUND_PATH):
+    """ """
     global SOUND_LIST, SOUND_PATH
     SOUND_PATH = path
     SOUND_LIST = get_sound_list(path)
 
 
-
-        
-
-
-
 class SoundManager:
-    """ Controls loading, mixing, and playing the sounds.
-        Having seperate classes allows different groups of sounds to be 
-         loaded, and unloaded from memory easily.
-
-        Useage:
-            sm = SoundManager()
-            sm.Load()
+    """Controls loading, mixing, and playing the sounds.
+    Having seperate classes allows different groups of sounds to be
+     loaded, and unloaded from memory easily.
+
+    Useage:
+        sm = SoundManager()
+        sm.Load()
 
-            Then every loop.
-            sm.Update(elapsed_time_in_seconds)
+        Then every loop.
+        sm.Update(elapsed_time_in_seconds)
 
-            Then to play sounds.  eg to play data/sounds/asound.ogg
-            sm.Play("asound")
+        Then to play sounds.  eg to play data/sounds/asound.ogg
+        sm.Play("asound")
     """
 
+    def __init__(
+        self, sound_list=SOUND_LIST, sound_path=SOUND_PATH, extensions=EXTENSIONS
+    ):
+        """ """
+        self.mixer = None
+        self.music = None
+        self.sounds = {}
+        self.chans = {}
 
-    def __init__(self, sound_list = SOUND_LIST, sound_path = SOUND_PATH, extensions = EXTENSIONS):
-        """
-	"""
-	self.mixer = None
-	self.music = None
-	self.sounds = {}
-	self.chans = {}
-
-	self._debug_level = 0
+        self._debug_level = 0
 
         self.sound_list = sound_list
         self.sound_path = sound_path
         self.extensions = extensions
 
-
         # sounds which are queued to play.
         self.queued_sounds = []
 
-    def _debug(self, x, debug_level = 0):
-        """
-	"""
-        print x
-	if self._debug_level > debug_level:
-	    print x
-
-
+    def _debug(self, x, debug_level=0):
+        """ """
+        print(x)
+        if self._debug_level > debug_level:
+            print(x)
 
-    def Load(self, sound_list = []):
-	"""Loads sounds."""
+    def Load(self, sound_list=[]):
+        """Loads sounds."""
         sounds = self.sounds
 
-	if not pygame.mixer:
-	    for name in sound_list:
-		sounds[name] = None
-	    return
-	for name in sound_list:
-	    if not sounds.has_key(name):
+        if not pygame.mixer:
+            for name in sound_list:
+                sounds[name] = None
+            return
+        for name in sound_list:
+            if name not in sounds:
                 sound = None
                 for ext in self.extensions:
-                    fullname = os.path.join(self.sound_path, name+ext)
-                    if(os.path.exists(fullname)):
-                        try: 
+                    fullname = os.path.join(self.sound_path, name + ext)
+                    if os.path.exists(fullname):
+                        try:
                             sound = pygame.mixer.Sound(fullname)
-                        except: 
+                        except:
                             sound = None
                             self._debug("Error loading sound", fullname)
                         break
                 if not sound:
-                    self._debug("could not find sound:%s: at path :%s:" % (name, self.sound_path))
-		sounds[name] = sound
-
+                    self._debug(
+                        "could not find sound:%s: at path :%s:"
+                        % (name, self.sound_path)
+                    )
+            sounds[name] = sound
 
     def GetSound(self, name):
-        """ Returns a Sound object for the given name.
-	"""
-	if not self.sounds.has_key(name):
-	    self.Load([name])
-
-	return self.sounds[name]
-
+        """Returns a Sound object for the given name."""
+        if name not in self.sounds:
+            self.Load([name])
 
+        return self.sounds[name]
 
     def Stop(self, name):
-        if self.chans.has_key(name):
+        if name in self.chans:
             if self.chans[name]:
                 if self.chans[name].get_busy():
                     self.chans[name].stop()
 
     def StopAll(self):
-        """ stops all sounds.
-        """
+        """stops all sounds."""
 
-        for name in self.chans.keys():
+        for name in list(self.chans.keys()):
             self.Stop(name)
 
     def IsSoundPlaying(self, name):
-
-        if self.chans.has_key(name):
+        if name in self.chans:
             return self.chans[name].get_busy()
         else:
             return 0
 
-
-    def Play(self, name, 
-                   volume=[1.0, 1.0], 
-                   wait = 0,
-                   loop = 0):
-        """ Plays the sound with the given name.
-	    name - of the sound.
-	    volume - left and right.  Ranges 0.0 - 1.0
-	    wait - used to control what happens if sound is allready playing:
-                0 - will not wait if sound playing.  play anyway.
-                1 - if there is a sound of this type playing wait for it.
-                2 - if there is a sound of this type playing do not play again.
-                3 - will not wait.  No queing of the sounds.
-            loop - number of times to loop.  -1 means forever.
-	"""
+    def Play(self, name, volume=[1.0, 1.0], wait=0, loop=0):
+        """Plays the sound with the given name.
+        name - of the sound.
+        volume - left and right.  Ranges 0.0 - 1.0
+        wait - used to control what happens if sound is allready playing:
+            0 - will not wait if sound playing.  play anyway.
+            1 - if there is a sound of this type playing wait for it.
+            2 - if there is a sound of this type playing do not play again.
+            3 - will not wait.  No queing of the sounds.
+        loop - number of times to loop.  -1 means forever.
+        """
 
         vol_l, vol_r = volume
 
-	sound = self.GetSound(name)
-
-	if sound:
-            if wait in [1,2]:
+        sound = self.GetSound(name)
 
-                if self.chans.has_key(name) and self.chans[name].get_busy():
+        if sound:
+            if wait in [1, 2]:
+                if name in self.chans and self.chans[name].get_busy():
                     if wait == 1:
                         # sound is allready playing we wait for it to finish.
                         self.queued_sounds.append((name, volume, wait))
                         return
                     elif wait == 2:
                         # not going to play sound if playing.
                         return
-                        
-
-	    self.chans[name] = sound.play(loop)
 
+            self.chans[name] = sound.play(loop)
 
             if not self.chans[name]:
                 if loop == 1:
                     # forces a channel to return. we fade that out,
                     #  and enqueue our one.
                     if pygame.mixer:
                         self.chans[name] = pygame.mixer.find_channel(1)
 
-                    #TODO: does this fadeout block? YES.
+                    # TODO: does this fadeout block? YES.
                     self.chans[name].fadeout(100)
                     self.chans[name].queue(sound)
                 else:
                     # the pygame api doesn't allow you to queue a sound and
                     #  tell it to loop.  So we hope for the best, and queue
                     #  the sound.
                     if wait not in [3]:
                         self.queued_sounds.append((name, volume, wait))
                     # delete the None channel here.
                     del self.chans[name]
 
             elif self.chans[name]:
-                #self.chans[name].set_volume(vol_l, vol_r)
+                # self.chans[name].set_volume(vol_l, vol_r)
                 self.chans[name].set_volume(vol_l)
 
-
-
-
     def Update(self, elapsed_time):
-        """
-        """
+        """ """
 
-        for name in self.chans.keys():
+        for name in list(self.chans.keys()):
             if not self.chans[name]:
                 # it may be a NoneType I think.
                 del self.chans[name]
             elif not self.chans[name].get_busy():
                 del self.chans[name]
         old_queued = self.queued_sounds
         self.queued_sounds = []
 
         for snd_info in old_queued:
             # we do not queue up sounds with wait 0.
             if snd_info not in [3]:
                 self.Play(*snd_info)
 
-
-
     def PlayMusic(self, musicname):
-        """ Plays a music track.  Only one can be played at a time.
-	    So if there is one playing, it will be stopped and the new 
-             one started.
-	"""
-
+        """Plays a music track.  Only one can be played at a time.
+        So if there is one playing, it will be stopped and the new
+         one started.
+        """
 
         try:
             music = pygame.mixer.music
         except:
             music = None
 
-	if not music: return
-	if music.get_busy():
-	    #we really should fade out nicely and
-	    #wait for the end music event, for now, CUT 
-	    music.stop()
-	#fullname = os.path.join('sounds', musicname)
-	fullname = musicname
+        if not music:
+            return
+        if music.get_busy():
+            # we really should fade out nicely and
+            # wait for the end music event, for now, CUT
+            music.stop()
+        # fullname = os.path.join('sounds', musicname)
+        fullname = musicname
         try:
             music.load(fullname)
         except pygame.error:
             return
-        
-	music.play(-1)
-	music.set_volume(1.0)
+
+        music.play(-1)
+        music.set_volume(1.0)
 
     def PauseMusic(self):
         self._unp_PauseMusic(1)
 
     def UnPauseMusic(self):
         self._unp_PauseMusic(0)
 
-
     def _unp_PauseMusic(self, p):
         try:
             music = pygame.mixer.music
         except:
             music = None
 
         if music:
             if p:
                 music.pause()
             else:
                 music.unpause()
-        
-
-
-
-
 
 
 class ChannelFader:
-    """ For fading a channel in and out.
+    """For fading a channel in and out.
 
-        cf = ChannelFader(achannel)
+    cf = ChannelFader(achannel)
 
-        # fade out to 20% volume over 2.5 seconds.
-        cf.fade_out(2.5, 0.2)
+    # fade out to 20% volume over 2.5 seconds.
+    cf.fade_out(2.5, 0.2)
 
-        # fade in to full volume over 12.5 seconds.
-        cf.fade_out(12.5, 1.0)
+    # fade in to full volume over 12.5 seconds.
+    cf.fade_out(12.5, 1.0)
 
-        # called every tick with the elapsed seconds.
-        cf.Update(0.01)
+    # called every tick with the elapsed seconds.
+    cf.Update(0.01)
     """
 
     def __init__(self, channel):
         self.channel = channel
 
         self.seconds = 0
-        self.volume_to= 0
+        self.volume_to = 0
         self.fade_direction = -1
         self.last_volume = self.channel.get_volume()
         self.elapsed_time = 0
         self.passed_time = 0
 
-
     def _fade(self, seconds, volume_to, direction):
         self.seconds = seconds
-        self.volume_to= volume_to
+        self.volume_to = volume_to
         self.fade_direction = direction
         self.last_volume = self.channel.get_volume()
         self.change_per_time = (volume_to - self.last_volume) / seconds
 
     def fade_in(self, seconds, volume_to):
         self._fade(seconds, volume_to, 1)
 
-
     def fade_out(self, seconds, volume_to):
         self._fade(seconds, volume_to, -1)
 
     def stop_fade(self):
         self.fade_direction = 0
 
     def Update(self, elapsed_time):
-        """ - probably needs the real elapsed time.  not gameplay elapsed time.
-        """
-        
+        """- probably needs the real elapsed time.  not gameplay elapsed time."""
+
         if self.fade_direction == 0:
             return
 
-
         # we use the stored last volume incase something else is changing
         #  the volume.
         new_volume = self.last_volume + (self.change_per_time * elapsed_time)
-        #print "prev new volume:%s" % new_volume
+        # print "prev new volume:%s" % new_volume
 
-      
         if self.fade_direction == -1:
             if new_volume < self.volume_to:
                 new_volume = self.volume_to
                 self.stop_fade()
 
         if self.fade_direction == 1:
             if new_volume > self.volume_to:
                 new_volume = self.volume_to
                 self.stop_fade()
 
         # set volume.
         self.channel.set_volume(new_volume)
         self.last_volume = new_volume
 
-        #print "new volume:%s" % new_volume
+        # print "new volume:%s" % new_volume
```

### Comparing `zanthor-1.2.3/zanthor/factory.py` & `zanthor-1.2.4a2/zanthor/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,60 @@
-import isovid
-from units import Factory
+from . import isovid
+from .units import Factory
 
 
-def factory_new(g,t,value):
-    print 'factory',g.clayer[t.ty][t.tx],t.rect
-    
-    
-    
+def factory_new(g, t, value):
+    print(("factory", g.clayer[t.ty][t.tx], t.rect))
+
     g.clayer[t.ty][t.tx] = 0
     g.blayer[t.ty][t.tx] = 0x14
-    g.blayer[t.ty-1][t.tx] = 0x14
-    g.blayer[t.ty][t.tx-1] = 0x14
-    g.blayer[t.ty+1][t.tx] = 0x14
-    g.blayer[t.ty][t.tx+1] = 0x14
-
-    #s = isovid.Sprite(g.images['factory.3'],(0,0))
-    #s.rect.centerx,s.rect.centery = t.rect.centerx,t.rect.centery/2
-    s = isovid.Sprite(g.images['factory.3'],t.rect)
+    g.blayer[t.ty - 1][t.tx] = 0x14
+    g.blayer[t.ty][t.tx - 1] = 0x14
+    g.blayer[t.ty + 1][t.tx] = 0x14
+    g.blayer[t.ty][t.tx + 1] = 0x14
+
+    # s = isovid.Sprite(g.images['factory.3'],(0,0))
+    # s.rect.centerx,s.rect.centery = t.rect.centerx,t.rect.centery/2
+    s = isovid.Sprite(g.images["factory.3"], t.rect)
     g.sprites.append(s)
-    print s.rect
-    tx,ty = s.rect.centerx/g.iso_w,s.rect.centery/g.iso_h
-    print tx,ty
-    
-    #NOTE: this is just to show off!
-    #import steam
-    #s.effect = steam.Effect(32,1)
-    
-    import fire
-    s.effect = fire.Effect(16,1)
-    
-    #s.groups = g.string2groups('coal')
-    #s.agroups = g.string2groups('castle')
-    #s.hit = coal_hit
+    print((s.rect))
+    tx, ty = s.rect.centerx / g.iso_w, s.rect.centery / g.iso_h
+    print((tx, ty))
+
+    # NOTE: this is just to show off!
+    # import steam
+    # s.effect = steam.Effect(32,1)
+
+    from . import fire
+
+    s.effect = fire.Effect(16, 1)
+
+    # s.groups = g.string2groups('coal')
+    # s.agroups = g.string2groups('castle')
+    # s.hit = coal_hit
 
-    #s.groups = g.string2groups('factory')
-    #s.agroups =g.string2groups("castle")
+    # s.groups = g.string2groups('factory')
+    # s.agroups =g.string2groups("castle")
     s.hit = factory_hit
 
-    
     s.loop = factory_loop
     s.frame = 0
-    s.type = 'factory'
+    s.type = "factory"
 
     s.unit = Factory()
-    
-def factory_loop(g,s):
+
+
+def factory_loop(g, s):
     s.unit.loop()
 
-    tx,ty = s.rect.centerx/32,s.rect.centery/32#g.view_to_iso((s.rect.centerx,s.rect.centery))
-    #print s.rect
-    #print tx,ty
-    #print g.tlayer[ty][tx]
-    s.frame +=1
-    
-def factory_hit(g,a,b):
+    tx, ty = (
+        s.rect.centerx / 32,
+        s.rect.centery / 32,
+    )  # g.view_to_iso((s.rect.centerx,s.rect.centery))
+    # print s.rect
+    # print tx,ty
+    # print g.tlayer[ty][tx]
+    s.frame += 1
+
+
+def factory_hit(g, a, b):
     pass
```

### Comparing `zanthor-1.2.3/zanthor/sound_info.py` & `zanthor-1.2.4a2/zanthor/sound_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 here you can define which sounds are played.
 
 Each list defines a list of sounds which can be played when that event happens.
 
 They get played in random order, or in cyclic order.
 """
 
-import cyclic_list
+from . import cyclic_list
 
 cl = cyclic_list.cyclic_list
 
 cannon = cl(["cannon", "cannon2", "cannon3", "cannon", "cannon"])
 
 hitenemy = cl(["hitenemy"])
 
@@ -26,24 +26,23 @@
 coal = cl(["coal"])
 water = cl(["water"])
 
 
 def get_upgrade_sound(upgrade_what):
     return "upgrade"
 
-#TODO: need to put in the release sound, and engine noises.
+
+# TODO: need to put in the release sound, and engine noises.
 release = cl(["release"])
 
 engine_slow = cl(["engine-slow"])
 engine_fast = cl(["engine-fast"])
 
 
 birds = cl(["birds1", "birds2", "birds2"])
 
 peasants = cl(["peasants1", "peasants2", "peasants3"])
 
 squish = cl(["squish1", "squish2"])
 
 ouch2 = cl(["ouch2"])
 ouch1 = cl(["ouch1"])
-
-
```

### Comparing `zanthor-1.2.3/zanthor/html.py` & `zanthor-1.2.4a2/zanthor/html.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,537 +1,658 @@
 """a html renderer
 """
 import htmllib
 import re
 import pygame
 from pygame.locals import *
 
-from pgu import gui
+from .pgu import gui
+
+_amap = {
+    "left": -1,
+    "right": 1,
+    "center": 0,
+    None: None,
+    "": None,
+}
+_vamap = {
+    "top": -1,
+    "bottom": 1,
+    "center": 0,
+    "middle": 0,
+    None: None,
+    "": None,
+}
 
-_amap = {'left':-1,'right':1,'center':0,None:None,'':None,}
-_vamap = {'top':-1,'bottom':1,'center':0,'middle':0,None:None,'':None,}
 
 class _dummy:
     pass
 
+
 class _flush:
     def __init__(self):
         self.style = _dummy()
         self.style.font = None
         self.style.color = None
         self.cls = None
-    def add(self,w): pass
-    def space(self,v): pass
-    
+
+    def add(self, w):
+        pass
+
+    def space(self, v):
+        pass
+
+
 class _hr(gui.Color):
-    def __init__(self,**params):
-        gui.Color.__init__(self,(0,0,0),**params)
-    def resize(self,width=None,height=None):
-        w,h = self.style.width,self.style.height
-        #if width != None: self.rect.w = width
-        #else: self.rect.w = 1
-        
-        #xt,xr,xb,xl = self.getspacing()
-
-        if width != None: w = max(w,width)
-        if height != None: h = max(h,height)        
-        w = max(w,1)
-        h = max(h,1)
-        
-        return w,h #self.container.rect.w,h
-        
-        #self.rect.w = max(1,width,self.container.rect.w-(xl+xr))
-        
-        #print self.rect
-        #self.rect.w = 1
+    def __init__(self, **params):
+        gui.Color.__init__(self, (0, 0, 0), **params)
+
+    def resize(self, width=None, height=None):
+        w, h = self.style.width, self.style.height
+        # if width != None: self.rect.w = width
+        # else: self.rect.w = 1
+
+        # xt,xr,xb,xl = self.getspacing()
+
+        if width != None:
+            w = max(w, width)
+        if height != None:
+            h = max(h, height)
+        w = max(w, 1)
+        h = max(h, 1)
+
+        return w, h  # self.container.rect.w,h
+
+        # self.rect.w = max(1,width,self.container.rect.w-(xl+xr))
+
+        # print self.rect
+        # self.rect.w = 1
+
 
 class _html(htmllib.HTMLParser):
-    def init(self,doc,font,color,_globals,_locals):
+    def init(self, doc, font, color, _globals, _locals):
         self.mystack = []
         self.document = doc
         self.myfont = self.font = font
         self.mycolor = self.color = color
-        self.myopen('document',self.document)
-        
-        
+        self.myopen("document", self.document)
+
         self.form = None
-        
+
         self._globals = _globals
         self._locals = _locals
-        
-    def myopen(self,type_,w):
-    
-        self.mystack.append((type_,w))
-        self.type,self.item = type_,w
-        
-        #self.font = self.item.style.font
-        #self.color = self.item.style.color
-        
-        if not self.font: self.font = self.myfont
-        if not self.color: self.color = self.mycolor
-        
-    def myclose(self,type_):
+
+    def myopen(self, type_, w):
+        self.mystack.append((type_, w))
+        self.type, self.item = type_, w
+
+        # self.font = self.item.style.font
+        # self.color = self.item.style.color
+
+        if not self.font:
+            self.font = self.myfont
+        if not self.color:
+            self.color = self.mycolor
+
+    def myclose(self, type_):
         t = None
         self.mydone()
         while t != type_:
-            #if len(self.mystack)==0: return
-            t,w = self.mystack.pop()
-        t,w = self.mystack.pop()
-        self.myopen(t,w)
-        
-    def myback(self,type_):
-        if type(type_) == str: type_ = [type_,]
+            # if len(self.mystack)==0: return
+            t, w = self.mystack.pop()
+        t, w = self.mystack.pop()
+        self.myopen(t, w)
+
+    def myback(self, type_):
+        if type(type_) == str:
+            type_ = [
+                type_,
+            ]
         self.mydone()
-        #print 'myback',type_
+        # print 'myback',type_
         t = None
         while t not in type_:
-            #if len(self.mystack)==0: return
-            t,w = self.mystack.pop()
-        self.myopen(t,w)
-        
+            # if len(self.mystack)==0: return
+            t, w = self.mystack.pop()
+        self.myopen(t, w)
+
     def mydone(self):
-        #clearing out the last </p>
-        if not hasattr(self.item,'layout'): return 
-        if len(self.item.layout._widgets) == 0: return 
+        # clearing out the last </p>
+        if not hasattr(self.item, "layout"):
+            return
+        if len(self.item.layout._widgets) == 0:
+            return
         w = self.item.layout._widgets[-1]
         if type(w) == tuple:
             del self.item.layout._widgets[-1]
 
-        
-    def start_b(self,attrs): self.font.set_bold(1)
-    def end_b(self): self.font.set_bold(0)
-    def start_i(self,attrs): self.font.set_italic(1)
-    def end_i(self): self.font.set_italic(0)
-    def start_u(self,attrs): self.font.set_underline(1)
-    def end_u(self): self.font.set_underline(0)
-    def start_br(self,attrs): self.do_br(attrs)
-    def do_br(self,attrs): self.item.br(self.font.size(" ")[1])
-    def attrs_to_map(self,attrs):
+    def start_b(self, attrs):
+        self.font.set_bold(1)
+
+    def end_b(self):
+        self.font.set_bold(0)
+
+    def start_i(self, attrs):
+        self.font.set_italic(1)
+
+    def end_i(self):
+        self.font.set_italic(0)
+
+    def start_u(self, attrs):
+        self.font.set_underline(1)
+
+    def end_u(self):
+        self.font.set_underline(0)
+
+    def start_br(self, attrs):
+        self.do_br(attrs)
+
+    def do_br(self, attrs):
+        self.item.br(self.font.size(" ")[1])
+
+    def attrs_to_map(self, attrs):
         k = None
         r = {}
-        for k,v in attrs: r[k] = v
+        for k, v in attrs:
+            r[k] = v
         return r
-        
-    def map_to_params(self,r):
+
+    def map_to_params(self, r):
         anum = re.compile("\D")
-        
-        params = {'style':{}}
-        style = params['style']
-        
-        if 'bgcolor' in r: style['background'] = pygame.Color(r['bgcolor'])
-        if 'background' in r: style['background'] = pygame.image.load(r['background'])
-        if 'border' in r: style['border'] = int(r['border'])
-            
-        for k in ['width','height','colspan','rowspan','size','min','max']:
-            if k in r: params[k] = int(anum.sub("",r[k]))
-            
-        for k in ['name','value']:
-            if k in r: params[k] = r[k]
-        
-        if 'class' in r: params['cls'] = r['class']
-        
-        if 'align' in r: 
-            params['align'] = _amap[r['align']]
-        if 'valign' in r:
-            params['valign'] = _vamap[r['valign']]
-
-        if 'style' in r:
-            for st in r['style'].split(";"):
-                #print st
+
+        params = {"style": {}}
+        style = params["style"]
+
+        if "bgcolor" in r:
+            style["background"] = pygame.Color(r["bgcolor"])
+        if "background" in r:
+            style["background"] = pygame.image.load(r["background"])
+        if "border" in r:
+            style["border"] = int(r["border"])
+
+        for k in ["width", "height", "colspan", "rowspan", "size", "min", "max"]:
+            if k in r:
+                params[k] = int(anum.sub("", r[k]))
+
+        for k in ["name", "value"]:
+            if k in r:
+                params[k] = r[k]
+
+        if "class" in r:
+            params["cls"] = r["class"]
+
+        if "align" in r:
+            params["align"] = _amap[r["align"]]
+        if "valign" in r:
+            params["valign"] = _vamap[r["valign"]]
+
+        if "style" in r:
+            for st in r["style"].split(";"):
+                # print st
                 if ":" in st:
-                    #print st.split(":")
-                    k,v = st.split(":")
-                    k = k.replace("-","_")
-                    k = k.replace(" ","")
-                    v = v.replace(" ","")
-                    if k == 'color' or k == 'border_color' or k == 'background':
+                    # print st.split(":")
+                    k, v = st.split(":")
+                    k = k.replace("-", "_")
+                    k = k.replace(" ", "")
+                    v = v.replace(" ", "")
+                    if k == "color" or k == "border_color" or k == "background":
                         v = pygame.Color(v)
                     else:
-                        v = int(anum.sub("",v))
+                        v = int(anum.sub("", v))
                     style[k] = v
         return params
-        
-    def map_to_connects(self,e,r):
-        for k,evt in [('onclick',gui.CLICK),('onchange',gui.CHANGE)]: #blah blah blah
-            
+
+    def map_to_connects(self, e, r):
+        for k, evt in [
+            ("onclick", gui.CLICK),
+            ("onchange", gui.CHANGE),
+        ]:  # blah blah blah
             if k in r:
-                #print k,r[k]
-                e.connect(evt,self.myexec,(e,r[k]))
+                # print k,r[k]
+                e.connect(evt, self.myexec, (e, r[k]))
 
-    def start_p(self,attrs):
+    def start_p(self, attrs):
         r = self.attrs_to_map(attrs)
-        align = r.get("align","left")
-        
+        align = r.get("align", "left")
+
         self.check_p()
         self.item.block(_amap[align])
-        
+
     def check_p(self):
-        if len(self.item.layout._widgets) == 0: return
+        if len(self.item.layout._widgets) == 0:
+            return
         if type(self.item.layout._widgets[-1]) == tuple:
-            w,h = self.item.layout._widgets[-1]
-            if w == 0: return
+            w, h = self.item.layout._widgets[-1]
+            if w == 0:
+                return
         self.do_br(None)
-        
+
     def end_p(self):
-        #print 'end p'
+        # print 'end p'
         self.check_p()
-        
-        
-    def start_block(self,t,attrs,align=-1):
+
+    def start_block(self, t, attrs, align=-1):
         r = self.attrs_to_map(attrs)
         params = self.map_to_params(r)
-        if 'cls' in params: params['cls'] = t+"."+params['cls']
-        else: params['cls'] = t
+        if "cls" in params:
+            params["cls"] = t + "." + params["cls"]
+        else:
+            params["cls"] = t
         b = gui.Document(**params)
-        if 'align' in params:
-            align = params['align']
+        if "align" in params:
+            align = params["align"]
         self.item.block(align)
         self.item.add(b)
-        self.myopen(t,b)
+        self.myopen(t, b)
 
-        
-                
-    def end_block(self,t):
+    def end_block(self, t):
         self.myclose(t)
         self.item.block(-1)
-        
-    def start_div(self,attrs): self.start_block('div',attrs)
-    def end_div(self): self.end_block('div')
-    def start_center(self,attrs): self.start_block('div',attrs,0)
-    def end_center(self): self.end_block('div')
-    
-    def start_h1(self,attrs): self.start_block('h1',attrs)
-    def end_h1(self): self.end_block('h1')
-    def start_h2(self,attrs): self.start_block('h2',attrs)
-    def end_h2(self): self.end_block('h2')
-    def start_h3(self,attrs): self.start_block('h3',attrs)
-    def end_h3(self): self.end_block('h3')
-    def start_h4(self,attrs): self.start_block('h4',attrs)
-    def end_h4(self): self.end_block('h4')
-    def start_h5(self,attrs): self.start_block('h5',attrs)
-    def end_h5(self): self.end_block('h5')
-    def start_h6(self,attrs): self.start_block('h6',attrs)
-    def end_h6(self): self.end_block('h6')
-
-    def start_ul(self,attrs): self.start_block('ul',attrs)
-    def end_ul(self): self.end_block('ul')
-    def start_ol(self,attrs): 
-        self.start_block('ol',attrs)
+
+    def start_div(self, attrs):
+        self.start_block("div", attrs)
+
+    def end_div(self):
+        self.end_block("div")
+
+    def start_center(self, attrs):
+        self.start_block("div", attrs, 0)
+
+    def end_center(self):
+        self.end_block("div")
+
+    def start_h1(self, attrs):
+        self.start_block("h1", attrs)
+
+    def end_h1(self):
+        self.end_block("h1")
+
+    def start_h2(self, attrs):
+        self.start_block("h2", attrs)
+
+    def end_h2(self):
+        self.end_block("h2")
+
+    def start_h3(self, attrs):
+        self.start_block("h3", attrs)
+
+    def end_h3(self):
+        self.end_block("h3")
+
+    def start_h4(self, attrs):
+        self.start_block("h4", attrs)
+
+    def end_h4(self):
+        self.end_block("h4")
+
+    def start_h5(self, attrs):
+        self.start_block("h5", attrs)
+
+    def end_h5(self):
+        self.end_block("h5")
+
+    def start_h6(self, attrs):
+        self.start_block("h6", attrs)
+
+    def end_h6(self):
+        self.end_block("h6")
+
+    def start_ul(self, attrs):
+        self.start_block("ul", attrs)
+
+    def end_ul(self):
+        self.end_block("ul")
+
+    def start_ol(self, attrs):
+        self.start_block("ol", attrs)
         self.item.counter = 0
-    def end_ol(self): self.end_block('ol')
-    def start_li(self,attrs): 
-        self.myback(['ul','ol'])
+
+    def end_ol(self):
+        self.end_block("ol")
+
+    def start_li(self, attrs):
+        self.myback(["ul", "ol"])
         cur = self.item
-        self.start_block('li',attrs)
-        if hasattr(cur,'counter'):
+        self.start_block("li", attrs)
+        if hasattr(cur, "counter"):
             cur.counter += 1
-            self.handle_data("%d. "%cur.counter)
+            self.handle_data("%d. " % cur.counter)
         else:
             self.handle_data("- ")
-    #def end_li(self): self.end_block('li') #this isn't needed because of how the parser works
 
-    def start_pre(self,attrs): self.start_block('pre',attrs)
-    def end_pre(self): self.end_block('pre')
-    def start_code(self,attrs): self.start_block('code',attrs)
-    def end_code(self): self.end_block('code')
-            
-    def start_table(self,attrs):
+    # def end_li(self): self.end_block('li') #this isn't needed because of how the parser works
+
+    def start_pre(self, attrs):
+        self.start_block("pre", attrs)
+
+    def end_pre(self):
+        self.end_block("pre")
+
+    def start_code(self, attrs):
+        self.start_block("code", attrs)
+
+    def end_code(self):
+        self.end_block("code")
+
+    def start_table(self, attrs):
         r = self.attrs_to_map(attrs)
         params = self.map_to_params(r)
-        
-        align = r.get("align","left")
+
+        align = r.get("align", "left")
         self.item.block(_amap[align])
 
         t = gui.Table(**params)
         self.item.add(t)
-        
-        self.myopen('table',t)
-        
-    def start_tr(self,attrs):
-        self.myback('table')
+
+        self.myopen("table", t)
+
+    def start_tr(self, attrs):
+        self.myback("table")
         self.item.tr()
-        
-    def _start_td(self,t,attrs):
+
+    def _start_td(self, t, attrs):
         r = self.attrs_to_map(attrs)
         params = self.map_to_params(r)
-        if 'cls' in params: params['cls'] = t+"."+params['cls']
-        else: params['cls'] = t
+        if "cls" in params:
+            params["cls"] = t + "." + params["cls"]
+        else:
+            params["cls"] = t
         b = gui.Document(cls=t)
-        
-        self.myback('table')
-        self.item.td(b,**params)
-        self.myopen(t,b)
-    
-        #self.font = self.item.style.font
-        #self.color = self.item.style.color
-        
-    def start_td(self,attrs):
-        self._start_td('td',attrs)
-    
-    def start_th(self,attrs):
-        self._start_td('th',attrs)
-        
+
+        self.myback("table")
+        self.item.td(b, **params)
+        self.myopen(t, b)
+
+        # self.font = self.item.style.font
+        # self.color = self.item.style.color
+
+    def start_td(self, attrs):
+        self._start_td("td", attrs)
+
+    def start_th(self, attrs):
+        self._start_td("th", attrs)
+
     def end_table(self):
-        self.myclose('table')
+        self.myclose("table")
         self.item.block(-1)
-        
-    def start_form(self,attrs):
+
+    def start_form(self, attrs):
         r = self.attrs_to_map(attrs)
         e = self.form = gui.Form()
         e.groups = {}
-        
-        self._locals[r.get('id',None)] = e
-        
-    def start_input(self,attrs):
+
+        self._locals[r.get("id", None)] = e
+
+    def start_input(self, attrs):
         r = self.attrs_to_map(attrs)
-        params = self.map_to_params(r) #why bother
-        #params = {}
-        
-        type_,name,value = r.get('type','text'),r.get('name',None),r.get('value',None)
+        params = self.map_to_params(r)  # why bother
+        # params = {}
+
+        type_, name, value = (
+            r.get("type", "text"),
+            r.get("name", None),
+            r.get("value", None),
+        )
         f = self.form
-        if type_ == 'text':
+        if type_ == "text":
             e = gui.Input(**params)
-            self.map_to_connects(e,r)
+            self.map_to_connects(e, r)
             self.item.add(e)
-        elif type_ == 'radio':
+        elif type_ == "radio":
             if name not in f.groups:
                 f.groups[name] = gui.Group(name=name)
             g = f.groups[name]
-            del params['name']
-            e = gui.Radio(group=g,**params)
-            self.map_to_connects(e,r)
+            del params["name"]
+            e = gui.Radio(group=g, **params)
+            self.map_to_connects(e, r)
             self.item.add(e)
-            if 'checked' in r: g.value = value
-        elif type_ == 'checkbox':
+            if "checked" in r:
+                g.value = value
+        elif type_ == "checkbox":
             if name not in f.groups:
                 f.groups[name] = gui.Group(name=name)
             g = f.groups[name]
-            del params['name']
-            e = gui.Checkbox(group=g,**params)
-            self.map_to_connects(e,r)
+            del params["name"]
+            e = gui.Checkbox(group=g, **params)
+            self.map_to_connects(e, r)
             self.item.add(e)
-            if 'checked' in r: g.value = value
+            if "checked" in r:
+                g.value = value
 
-        elif type_ == 'button':
+        elif type_ == "button":
             e = gui.Button(**params)
-            self.map_to_connects(e,r)
+            self.map_to_connects(e, r)
             self.item.add(e)
-        elif type_ == 'submit':
+        elif type_ == "submit":
             e = gui.Button(**params)
-            self.map_to_connects(e,r)
+            self.map_to_connects(e, r)
             self.item.add(e)
-        elif type_ == 'file':
+        elif type_ == "file":
             e = gui.Input(**params)
-            self.map_to_connects(e,r)
+            self.map_to_connects(e, r)
             self.item.add(e)
-            b = gui.Button(value='Browse...')
+            b = gui.Button(value="Browse...")
             self.item.add(b)
+
             def _browse(value):
-                d = gui.FileDialog();
-                d.connect(gui.CHANGE,gui.action_setvalue,(d,e))
-                d.open();
-            b.connect(gui.CLICK,_browse,None)
+                d = gui.FileDialog()
+                d.connect(gui.CHANGE, gui.action_setvalue, (d, e))
+                d.open()
+
+            b.connect(gui.CLICK, _browse, None)
 
-        self._locals[r.get('id',None)] = e
+        self._locals[r.get("id", None)] = e
 
-    def start_object(self,attrs):
+    def start_object(self, attrs):
         r = self.attrs_to_map(attrs)
         params = self.map_to_params(r)
-        code = "e = %s(**params)"%r['type']
-        #print code
-        #print params
+        code = "e = %s(**params)" % r["type"]
+        # print code
+        # print params
         exec(code)
-        #print e
-        #print e.style.width,e.style.height
-        self.map_to_connects(e,r)
+        # print e
+        # print e.style.width,e.style.height
+        self.map_to_connects(e, r)
         self.item.add(e)
-        
-        self._locals[r.get('id',None)] = e
-    
-    def start_select(self,attrs):
+
+        self._locals[r.get("id", None)] = e
+
+    def start_select(self, attrs):
         r = self.attrs_to_map(attrs)
         params = {}
-        
-        name,value = r.get('name',None),r.get('value',None)
-        e = gui.Select(name=name,value=value,**params)
-        self.map_to_connects(e,r)
+
+        name, value = r.get("name", None), r.get("value", None)
+        e = gui.Select(name=name, value=value, **params)
+        self.map_to_connects(e, r)
         self.item.add(e)
-        self.myopen('select',e)
-        
-    def start_option(self,attrs):
+        self.myopen("select", e)
+
+    def start_option(self, attrs):
         r = self.attrs_to_map(attrs)
-        params = {} #style = self.map_to_style(r)
-        
-        self.myback('select')
+        params = {}  # style = self.map_to_style(r)
+
+        self.myback("select")
         e = gui.Document(**params)
-        self.item.add(e,value=r.get('value',None))
-        self.myopen('option',e)
-        
-        
+        self.item.add(e, value=r.get("value", None))
+        self.myopen("option", e)
+
     def end_select(self):
-        self.myclose('select')
-        
-    def start_hr(self,attrs):
+        self.myclose("select")
+
+    def start_hr(self, attrs):
         self.do_hr(attrs)
-    def do_hr(self,attrs):
-        h = self.font.size(" ")[1]/2
-        
+
+    def do_hr(self, attrs):
+        h = self.font.size(" ")[1] / 2
+
         r = self.attrs_to_map(attrs)
         params = self.map_to_params(r)
-        params['style']['padding'] = h
-        print params
+        params["style"]["padding"] = h
+        print(params)
 
         self.item.block(0)
         self.item.add(_hr(**params))
         self.item.block(-1)
-        
-    def anchor_begin(self,href,name,type_):
+
+    def anchor_begin(self, href, name, type_):
         pass
 
     def anchor_end(self):
         pass
-        
-    def start_title(self,attrs): self.myopen('title',_flush())
-    def end_title(self): self.myclose('title')
-            
-    def myexec(self,value):
-        w,code = value
+
+    def start_title(self, attrs):
+        self.myopen("title", _flush())
+
+    def end_title(self):
+        self.myclose("title")
+
+    def myexec(self, value):
+        w, code = value
         g = self._globals
         l = self._locals
-        l['self'] = w
-        exec(code,g,l)
-        
-    def handle_image(self,src,alt,ismap,align,width,height):
+        l["self"] = w
+        exec(code, g, l)
+
+    def handle_image(self, src, alt, ismap, align, width, height):
         try:
             w = gui.Image(pygame.image.load(src))
-            if align != '':
-                self.item.add(w,_amap[align])
+            if align != "":
+                self.item.add(w, _amap[align])
             else:
                 self.item.add(w)
         except:
-            print 'handle_image: missing %s'%src
-                
-    def handle_data(self,txt):
-        if self.type == 'table': return 
-        elif self.type in ('pre','code'): 
-            txt = txt.replace("\t","        ")
+            print(("handle_image: missing %s" % src))
+
+    def handle_data(self, txt):
+        if self.type == "table":
+            return
+        elif self.type in ("pre", "code"):
+            txt = txt.replace("\t", "        ")
             ss = txt.split("\n")
-            if ss[-1] == "": del ss[-1]
+            if ss[-1] == "":
+                del ss[-1]
             for sentence in ss:
-                img = self.myfont.render(sentence,1,self.mycolor)
+                img = self.myfont.render(sentence, 1, self.mycolor)
                 w = gui.Image(img)
                 self.item.add(w)
                 self.item.block(-1)
             return
 
-        txt = re.compile("^[\t\r\n]+").sub("",txt)
-        txt = re.compile("[\t\r\n]+$").sub("",txt)
-        
-        tst = re.compile("[\t\r\n]+").sub("",txt)
-        if tst == "": return
-        
-        txt = re.compile("\s+").sub(" ",txt)
-        if txt == "": return
-        
+        txt = re.compile("^[\t\r\n]+").sub("", txt)
+        txt = re.compile("[\t\r\n]+$").sub("", txt)
+
+        tst = re.compile("[\t\r\n]+").sub("", txt)
+        if tst == "":
+            return
+
+        txt = re.compile("\s+").sub(" ", txt)
+        if txt == "":
+            return
+
         if txt == " ":
             self.item.space(self.myfont.size(" "))
             return
-        
+
         for word in txt.split(" "):
-            word = word.replace(chr(160)," ") #&nbsp;
-            #print self.item.cls
-            w = gui.Image(self.myfont.render(word,1,self.mycolor))
+            word = word.replace(chr(160), " ")  # &nbsp;
+            # print self.item.cls
+            w = gui.Image(self.myfont.render(word, 1, self.mycolor))
             self.item.add(w)
             self.item.space(self.myfont.size(" "))
-            
+
 
 class HTML(gui.Document):
     """a gui HTML object
-    
+
     <pre>HTML(data,globals=None,locals=None)</pre>
-        
-    <dl>    
+
+    <dl>
     <dt>data <dd>html data
     <dt>globals <dd>global variables (for scripting)
     <dt>locals <dd>local variables (for scripting)
     </dl>
-    
+
     <p>you may access html elements that have an id via widget[id]</p>
     """
-    def __init__(self,data,globals=None,locals=None,**params):
-        gui.Document.__init__(self,**params)
-        
-        _globals,_locals = globals,locals
-        
-        if _globals == None: _globals = {}
-        if _locals == None: _locals = {}
+
+    def __init__(self, data, globals=None, locals=None, **params):
+        gui.Document.__init__(self, **params)
+
+        _globals, _locals = globals, locals
+
+        if _globals == None:
+            _globals = {}
+        if _locals == None:
+            _locals = {}
         self._globals = _globals
         self._locals = _locals
-        
-        #font = gui.theme.get("label","","font")
-        p = _html(htmllib.AS_IS,0)
-        print self.style.color
-        p.init(self,self.style.font,self.style.color,_globals,_locals)
-        p.feed(data) 
-        p.close() 
+
+        # font = gui.theme.get("label","","font")
+        p = _html(htmllib.AS_IS, 0)
+        print((self.style.color))
+        p.init(self, self.style.font, self.style.color, _globals, _locals)
+        p.feed(data)
+        p.close()
         p.mydone()
-        
-        
-    def __getitem__(self,k):
+
+    def __getitem__(self, k):
         return self._locals[k]
 
-def render(font,rect,text,aa,color,bgcolor=(0,0,0,0)):
+
+def render(font, rect, text, aa, color, bgcolor=(0, 0, 0, 0)):
     """render some html
-    
+
     <pre>render(font,rect,text,aa,color,bgcolor=(0,0,0,0))</pre>
     """
-    fnt,r,txt,a,fg,bg = font,rect,text,aa,color,bgcolor
-    
-    e = HTML(txt,font=fnt,color=fg)
+    fnt, r, txt, a, fg, bg = font, rect, text, aa, color, bgcolor
+
+    e = HTML(txt, font=fnt, color=fg)
     e.resize(width=rect.w)
-    s = pygame.Surface((e.rect.w,e.rect.h),SWSURFACE|SRCALPHA,32)
+    s = pygame.Surface((e.rect.w, e.rect.h), SWSURFACE | SRCALPHA, 32)
     s.fill(bg)
     e.paint(s)
-    
+
     return s
 
-def rendertrim(font,rect,text,aa,color,bgcolor=(0,0,0,0)):
+
+def rendertrim(font, rect, text, aa, color, bgcolor=(0, 0, 0, 0)):
     """render html, and make sure to trim the size
-    
+
     <pre>rendertrim(font,rect,text,aa,color,bgcolor=(0,0,0,0))</pre>
     """
-    fnt,r,txt,a,fg,bg = font,rect,text,aa,color,bgcolor
-    #print r
-    w = HTML(txt,font=fnt,color=fg)
+    fnt, r, txt, a, fg, bg = font, rect, text, aa, color, bgcolor
+    # print r
+    w = HTML(txt, font=fnt, color=fg)
     w.resize(width=rect.w)
-    s = pygame.Surface((w.rect.w,w.rect.h),SWSURFACE|SRCALPHA,32)
+    s = pygame.Surface((w.rect.w, w.rect.h), SWSURFACE | SRCALPHA, 32)
     s.fill(bg)
     w.paint(s)
-    
-    minx,miny,maxx,maxy = 1024,1024,-1024,-1024
+
+    minx, miny, maxx, maxy = 1024, 1024, -1024, -1024
     for e in w.layout.widgets:
-        x,y,w,h = e.rect.x,e.rect.y,e.rect.w,e.rect.h
-        minx = min(minx,x)
-        miny = min(miny,y)
-        x,y = x+w,y+h
-        maxx = max(maxx,x)
-        maxy = max(maxy,y)
-        
-    r = pygame.Rect(minx,miny,maxx-minx,maxy-miny)
-        
+        x, y, w, h = e.rect.x, e.rect.y, e.rect.w, e.rect.h
+        minx = min(minx, x)
+        miny = min(miny, y)
+        x, y = x + w, y + h
+        maxx = max(maxx, x)
+        maxy = max(maxy, y)
+
+    r = pygame.Rect(minx, miny, maxx - minx, maxy - miny)
+
     return s.subsurface((r))
 
-    
-def write(s,font,rect,text,aa=0,color=(0,0,0)):
+
+def write(s, font, rect, text, aa=0, color=(0, 0, 0)):
     """write html to a surface
-    
+
     <pre>write(s,font,rect,text,aa=0,color=(0,0,0))</pre>
     """
-    fnt,r,txt,a,fg = font,rect,text,aa,color
+    fnt, r, txt, a, fg = font, rect, text, aa, color
+
+    e = HTML(txt, font=fnt, color=fg)
 
-    e = HTML(txt,font=fnt,color=fg)
-    
     e.resize(width=rect.w)
     s = s.subsurface(rect)
     e.paint(s)
-    
+
+
 # vim: set filetype=python sts=4 sw=4 noet si :
```

### Comparing `zanthor-1.2.3/zanthor/level.py` & `zanthor-1.2.4a2/zanthor/level.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,582 +1,581 @@
 import os, random, time
 
 import pygame
-#from pgu import isovid
-import isovid
-from pgu import gui
 
-from pygame.locals import *
-from const import *
-import const
-import human, castle, items
-import interface
-import states
-
-import truck,cannon,robot
-import factory
+# from pgu import isovid
+from . import isovid
+from .pgu import gui
 
+from pygame.locals import *
+from .const import *
+from . import const
+from . import human, castle, items
+from . import interface
+# from . import states
+
+from . import truck, cannon, robot
+from . import factory
 
-import tiles
-import menu
-import flock
 
+from . import tiles
+from . import menu
+from . import flock
 
 
 class Level:
-    def __init__(self,game,_round,perc,music):
+    def __init__(self, game, _round, perc, music):
         self.game = game
         self.round = _round
         self.percent = perc
-        
+
         self.tv = tv = isovid.Isovid()
         self.tv.level = self
-        
 
         self.last_mouse_event_time = time.time()
         self.last_mouse_moves = 0
 
-
         if music:
             if pygame.mixer:
-                pygame.mixer.music.load(data_dir("intro",music))
+                pygame.mixer.music.load(data_dir("intro", music))
                 pygame.mixer.music.play(-1)
 
         tdata = {
-            
-            0x01:('castle',tiles.tile_coal,None),
-            0x02:('castle',tiles.tile_water,None),
-            #0x03:('castle',tiles.tile_block,{'top':1,'bottom':1,'left':1,'right':1}),
-            #0x04:('castle',tiles.tile_block,{'top':1,'bottom':1,'left':1,'right':1}),
-            #0x05:('castle',tiles.tile_block,{'top':1,'bottom':1,'left':1,'right':1}),
-            #0x06:('castle',tiles.tile_block,{'top':1,'bottom':1,'left':1,'right':1}),
-            #0x03:('cball',tiles.tile_wall,None),
-            0x04:('cball',tiles.tile_wall,None),
-            0x05:('cball',tiles.tile_wall,None),
-            0x06:('cball',tiles.tile_wall,None),
-            0x07:('castle',tiles.tile_rubble,None),
-
-            8:('castle',tiles.tile_part,None),
-            9:('castle',tiles.tile_part,None),
-            10:('castle',tiles.tile_part,None),
-            11:('castle',tiles.tile_part,None),
-            12:('castle',tiles.tile_part,None),
-            13:('castle',tiles.tile_part,None),
-            14:('castle',tiles.tile_part,None),
-            15:('castle',tiles.tile_part,None),
-
-            
-
-            0x1c:('castle,cball,robot',tiles.tile_limit,None), #remove item from level if it goes here.
-            }
-            #TODO: FIXME:
-            
-
-        tv.tga_load_tiles(data_dir("gfx","tiles2.tga"),(32,64),tdata)
-        
-        tv.tiles[1].item = items.Coal(3.0) #HERE!!
+            0x01: ("castle", tiles.tile_coal, None),
+            0x02: ("castle", tiles.tile_water, None),
+            # 0x03:('castle',tiles.tile_block,{'top':1,'bottom':1,'left':1,'right':1}),
+            # 0x04:('castle',tiles.tile_block,{'top':1,'bottom':1,'left':1,'right':1}),
+            # 0x05:('castle',tiles.tile_block,{'top':1,'bottom':1,'left':1,'right':1}),
+            # 0x06:('castle',tiles.tile_block,{'top':1,'bottom':1,'left':1,'right':1}),
+            # 0x03:('cball',tiles.tile_wall,None),
+            0x04: ("cball", tiles.tile_wall, None),
+            0x05: ("cball", tiles.tile_wall, None),
+            0x06: ("cball", tiles.tile_wall, None),
+            0x07: ("castle", tiles.tile_rubble, None),
+            8: ("castle", tiles.tile_part, None),
+            9: ("castle", tiles.tile_part, None),
+            10: ("castle", tiles.tile_part, None),
+            11: ("castle", tiles.tile_part, None),
+            12: ("castle", tiles.tile_part, None),
+            13: ("castle", tiles.tile_part, None),
+            14: ("castle", tiles.tile_part, None),
+            15: ("castle", tiles.tile_part, None),
+            0x1C: (
+                "castle,cball,robot",
+                tiles.tile_limit,
+                None,
+            ),  # remove item from level if it goes here.
+        }
+        # TODO: FIXME:
+
+        tv.tga_load_tiles(data_dir("gfx", "tiles2.tga"), (32, 64), tdata)
+
+        tv.tiles[1].item = items.Coal(3.0)  # HERE!!
         tv.tiles[2].item = items.Water(3.0)
 
         tv.tiles[8].item = items.Part("UpEngine Efficiency", "")
         tv.tiles[9].item = items.Part("UpEngine Speed", "")
         tv.tiles[10].item = items.Part("UpCannon Balls", "")
         tv.tiles[11].item = items.Part("UpArmour", "")
         tv.tiles[12].item = items.Part("UpSteam Tank", "")
         tv.tiles[13].item = items.Part("UpWater Tank", "")
         tv.tiles[14].item = items.Part("UpCoal Tank", "")
         tv.tiles[15].item = items.Part("UpCannon Power", "")
 
-
         tv.tiles[7].item = items.Rubble()
 
+        # TODO: add in the rubble item.
 
-
-        #TODO: add in the rubble item.
-        
         fname = self.round
-        if fname == 0: fname = 'test2.tga'
-        tv.tga_load_level(data_dir("levels",fname),1)
-        
-        #NOTE: blur the background
-        for n in xrange(0,1):
+        if fname == 0:
+            fname = "test2.tga"
+        tv.tga_load_level(data_dir("levels", fname), 1)
+
+        # NOTE: blur the background
+        for n in range(0, 1):
             layer = tv.blayer
-            nlayer= [[0 for x in xrange(0,tv.size[0])] for y in xrange(0,tv.size[1])]
-            w,h = tv.size
-            for y in xrange(0,h):
-                for x in xrange(0,w):
+            nlayer = [[0 for x in range(0, tv.size[0])] for y in range(0, tv.size[1])]
+            w, h = tv.size
+            for y in range(0, h):
+                for x in range(0, w):
                     v = 0
-                    for dx,dy in [(-1,-1),(0,-1),(1,-1),(-1,0),(1,0),(-1,1),(0,1),(1,1)]:
-                        xx = min(max(x+dx,0),w-1)
-                        yy = min(max(y+dy,0),h-1)
+                    for dx, dy in [
+                        (-1, -1),
+                        (0, -1),
+                        (1, -1),
+                        (-1, 0),
+                        (1, 0),
+                        (-1, 1),
+                        (0, 1),
+                        (1, 1),
+                    ]:
+                        xx = min(max(x + dx, 0), w - 1)
+                        yy = min(max(y + dy, 0), h - 1)
                         v += layer[yy][xx]
                     v /= 8
                     nlayer[y][x] = v
-            for y in xrange(0,h):
-                for x in xrange(0,w):
+            for y in range(0, h):
+                for x in range(0, w):
                     layer[y][x] = nlayer[y][x]
-                    
-                    
-                        
-        
-        #NOTE: this layer is for enemies "astar" stuff
-        tv.truck_layer= [[0 for x in xrange(0,tv.size[0])] for y in xrange(0,tv.size[1])]
-        tv.robot_layer= [[0 for x in xrange(0,tv.size[0])] for y in xrange(0,tv.size[1])]
-        tv.castle_layer= [[0 for x in xrange(0,tv.size[0])] for y in xrange(0,tv.size[1])]
-        #this is for robots to see who is near by
-        tv.robot_list_layer= [[[] for x in xrange(0,tv.size[0])] for y in xrange(0,tv.size[1])]
-
-        
-        #this is to init all the astar layers, forcefully...
-        #since load_level shortcuts all the .set() stuff
-        for y in xrange(0,tv.size[1]):
-            for x in xrange(0,tv.size[0]):
-                tv.set((x,y),tv.get((x,y)))
-        
-        
-        
+
+        # NOTE: this layer is for enemies "astar" stuff
+        tv.truck_layer = [
+            [0 for x in range(0, tv.size[0])] for y in range(0, tv.size[1])
+        ]
+        tv.robot_layer = [
+            [0 for x in range(0, tv.size[0])] for y in range(0, tv.size[1])
+        ]
+        tv.castle_layer = [
+            [0 for x in range(0, tv.size[0])] for y in range(0, tv.size[1])
+        ]
+        # this is for robots to see who is near by
+        tv.robot_list_layer = [
+            [[] for x in range(0, tv.size[0])] for y in range(0, tv.size[1])
+        ]
+
+        # this is to init all the astar layers, forcefully...
+        # since load_level shortcuts all the .set() stuff
+        for y in range(0, tv.size[1]):
+            for x in range(0, tv.size[0]):
+                tv.set((x, y), tv.get((x, y)))
+
         tv.view.x = -220
         tv.view.y = -64
-        tv.view.w,tv.view.h = S_VIEW.w,S_VIEW.h
-        #tv.view.w,tv.view.h = SW,SH
-        #print "view"
-        #print tv.view
-        
-        
-        tv.tile_w,tv.tile_h = 32,64
-        tv.iso_w,tv.iso_h = 32,32
-        tv.base_w,tv.base_h = 32,16
+        tv.view.w, tv.view.h = S_VIEW.w, S_VIEW.h
+        # tv.view.w,tv.view.h = SW,SH
+        # print "view"
+        # print tv.view
+
+        tv.tile_w, tv.tile_h = 32, 64
+        tv.iso_w, tv.iso_h = 32, 32
+        tv.base_w, tv.base_h = 32, 16
         tv.iso_z = 1
 
+        # best#shape = (8,64-24,16,16)
+        shape = (0, 48, 32, 16)
 
-        #best#shape = (8,64-24,16,16)
-        shape = (0,48,32,16)
-        
-        
-        #shape = (2,64-30,28,28)
-        #shape = (16,64-16,1,1)
+        # shape = (2,64-30,28,28)
+        # shape = (16,64-16,1,1)
 
         idata = [
-            #('castle',data_dir('gfx', 'castle1.png'),(8,64-16,16,8)),
-            #('coal',data_dir('gfx', 'coal.png'),(8,64-16,16,8)),
-            #('castle',tv.tiles[8].image,shape),
-            ('coal',tv.tiles[1].image,shape),
-            ('water',tv.tiles[2].image,shape),
-
-            ('UpEngine Efficiency',tv.tiles[8].image,shape),
-            ('UpEngine Speed',     tv.tiles[9].image,shape),
-            ('UpCannon Balls',     tv.tiles[10].image,shape),
-            ('UpArmour',           tv.tiles[11].image,shape),
-            ('UpSteam Tank',       tv.tiles[12].image,shape),
-            ('UpWater Tank',       tv.tiles[13].image,shape),
-            ('UpCoal Tank',        tv.tiles[14].image,shape),
-            ('UpCannon Power',     tv.tiles[15].image,shape),
-
-            ('factory.1',tv.tiles[3].image,shape),
-            ('factory.2',tv.tiles[4].image,shape),
-            ('factory.3',tv.tiles[5].image,shape),
-            ('cannon_tower',tv.tiles[11].image,shape),
-            ('wall',tv.tiles[23].image,shape),
-            ('human',tv.tiles[9].image,shape),
-            ('baddie_robot',tv.tiles[10].image,shape),
-            
-            ('truck',tv.tiles[15].image,shape),
-            ('cannon',tv.tiles[11].image,shape),
-            #('cball',tv.tiles[14].image,shape),
-            ('cball',tv.tiles[32].image,shape),
-            ('cball2',tv.tiles[33].image,shape),
-            ('cball3',tv.tiles[34].image,shape),
-            ('cball4',tv.tiles[35].image,shape),
-            ('robot',tv.tiles[12].image.subsurface(0,24,32,32+8),(8,24,16,16)),
-            ]
-        timg = pygame.image.load(data_dir("gfx","tiles2.tga")).convert_alpha()
-        img = timg.subsurface((0,64*2+32,64,64+32))
-        shape = (16,32+32,32,32)
-        idata.append(('castle',img,shape))
-        idata.append(('castle.left',img,shape))
-        idata.append(('castle.right',pygame.transform.flip(img,-1,0),shape))
+            # ('castle',data_dir('gfx', 'castle1.png'),(8,64-16,16,8)),
+            # ('coal',data_dir('gfx', 'coal.png'),(8,64-16,16,8)),
+            # ('castle',tv.tiles[8].image,shape),
+            ("coal", tv.tiles[1].image, shape),
+            ("water", tv.tiles[2].image, shape),
+            ("UpEngine Efficiency", tv.tiles[8].image, shape),
+            ("UpEngine Speed", tv.tiles[9].image, shape),
+            ("UpCannon Balls", tv.tiles[10].image, shape),
+            ("UpArmour", tv.tiles[11].image, shape),
+            ("UpSteam Tank", tv.tiles[12].image, shape),
+            ("UpWater Tank", tv.tiles[13].image, shape),
+            ("UpCoal Tank", tv.tiles[14].image, shape),
+            ("UpCannon Power", tv.tiles[15].image, shape),
+            ("factory.1", tv.tiles[3].image, shape),
+            ("factory.2", tv.tiles[4].image, shape),
+            ("factory.3", tv.tiles[5].image, shape),
+            ("cannon_tower", tv.tiles[11].image, shape),
+            ("wall", tv.tiles[23].image, shape),
+            ("human", tv.tiles[9].image, shape),
+            ("baddie_robot", tv.tiles[10].image, shape),
+            ("truck", tv.tiles[15].image, shape),
+            ("cannon", tv.tiles[11].image, shape),
+            # ('cball',tv.tiles[14].image,shape),
+            ("cball", tv.tiles[32].image, shape),
+            ("cball2", tv.tiles[33].image, shape),
+            ("cball3", tv.tiles[34].image, shape),
+            ("cball4", tv.tiles[35].image, shape),
+            (
+                "robot",
+                tv.tiles[12].image.subsurface(0, 24, 32, 32 + 8),
+                (8, 24, 16, 16),
+            ),
+        ]
+        try:
+            timg = pygame.image.load(data_dir("gfx", "tiles2.tga")).convert_alpha()
+        except:
+            timg = pygame.image.load(data_dir("gfx", "tiles2.png")).convert_alpha()
+        img = timg.subsurface((0, 64 * 2 + 32, 64, 64 + 32))
+        shape = (16, 32 + 32, 32, 32)
+        idata.append(("castle", img, shape))
+        idata.append(("castle.left", img, shape))
+        idata.append(("castle.right", pygame.transform.flip(img, -1, 0), shape))
 
         cdata = {
-            1:(castle.castle_new,None),
-            #2:(coal_new,None),
-            #3:(water_new,None),
-            4:(factory.factory_new,None),
-            
-            #16:(cannon_tower_new,None),
-            #17:(baddie_robot_new,None),
-            #18:(wall_new,None),
-            #19:(human_new,None),
-            
-            5:(truck.truck_new,None),
-            6:(cannon.cannon_new,None),
-            7:(robot.robot_new,None),
-            
+            1: (castle.castle_new, None),
+            # 2:(coal_new,None),
+            # 3:(water_new,None),
+            4: (factory.factory_new, None),
+            # 16:(cannon_tower_new,None),
+            # 17:(baddie_robot_new,None),
+            # 18:(wall_new,None),
+            # 19:(human_new,None),
+            5: (truck.truck_new, None),
+            6: (cannon.cannon_new, None),
+            7: (robot.robot_new, None),
         }
 
-        #tv.load_images(idata) #should do this later, but i'm
-        #using a quick hack for now
-        for name,img,shape in idata:
-            tv.images[name]=img,shape
-        
-        tw,th = tv.iso_w,tv.iso_h
-        w,h = tv.size
-        border = tw*2
-        rect = pygame.Rect(-border,-border,tw*w+border*2,th*h+border*2)
-        #tv.robots = flock.Flock(rect,tw*3/2)
-        tv.robots = flock.Flock(rect,tw*2)
-        tv.run_codes(cdata,(0,0,tv.size[0],tv.size[1]))
-        
-        tv.robots_total = len(tv.robots)
-
-
+        # tv.load_images(idata) #should do this later, but i'm
+        # using a quick hack for now
+        for name, img, shape in idata:
+            tv.images[name] = img, shape
+
+        tw, th = tv.iso_w, tv.iso_h
+        w, h = tv.size
+        border = tw * 2
+        rect = pygame.Rect(-border, -border, tw * w + border * 2, th * h + border * 2)
+        # tv.robots = flock.Flock(rect,tw*3/2)
+        tv.robots = flock.Flock(rect, tw * 2)
+        tv.run_codes(cdata, (0, 0, tv.size[0], tv.size[1]))
 
+        tv.robots_total = len(tv.robots)
 
-        # 
+        #
         self.interface = interface.Interface()
         self.interface.load()
 
         self.interface.tv = tv
         self.interface.max_robots = len(tv.robots)
 
-
         # ??? what does this code do???
 
-
-
-        for k,v in tv.images.items():
+        for k, v in list(tv.images.items()):
             shape = None
-            print v
+            print(v)
             if len(v) > 1:
-                img,shape = v
-            else: img = v
-            
-            img2 = pygame.Surface((img.get_width(),img.get_height())).convert()
-            ck = (255,0,255)
+                img, shape = v
+            else:
+                img = v
+
+            img2 = pygame.Surface((img.get_width(), img.get_height())).convert()
+            ck = (255, 0, 255)
             img2.fill(ck)
-            img2.blit(img,(0,0))
+            img2.blit(img, (0, 0))
             img2.set_colorkey(ck)
-            
+
             if shape != None:
-                tv.images[k] = img2,shape
+                tv.images[k] = img2, shape
             else:
                 tv.images[k] = img2
-        
+
         n = 0
         for t in tv.tiles:
             if t != None and t.image != None:
-                ck = (255,0,255,255)
+                ck = (255, 0, 255, 255)
                 img = t.image
                 minh = 64
                 maxh = 0
                 x = 16
-                for y in xrange(0,64):
-                    c = img.get_at((x,y))
+                for y in range(0, 64):
+                    c = img.get_at((x, y))
                     if c[3] == 255:
-                        minh = min(minh,y)
-                        maxh = max(maxh,y)
-                        
+                        minh = min(minh, y)
+                        maxh = max(maxh, y)
+
                 if minh > maxh:
                     img2 = None
-                    print 'ahh',n
+                    print(("ahh", n))
                 elif minh != 0 or maxh != 63:
-                    t.h = maxh-minh
-                    img = img.subsurface(0,minh,32,maxh-minh)
-                    img2 = pygame.Surface((img.get_width(),img.get_height())).convert()
-                    ck = (255,0,255)
+                    t.h = maxh - minh
+                    img = img.subsurface(0, minh, 32, maxh - minh)
+                    img2 = pygame.Surface((img.get_width(), img.get_height())).convert()
+                    ck = (255, 0, 255)
                     img2.fill(ck)
-                    img2.blit(img,(0,0))
+                    img2.blit(img, (0, 0))
                     img2.set_colorkey(ck)
-                else: 
-                    img2 = pygame.Surface((img.get_width(),img.get_height())).convert()
-                    ck = (255,0,255)
+                else:
+                    img2 = pygame.Surface((img.get_width(), img.get_height())).convert()
+                    ck = (255, 0, 255)
                     img2.fill(ck)
-                    img2.blit(img,(0,0))
+                    img2.blit(img, (0, 0))
                     img2.set_colorkey(ck)
 
-                
                 t.image = img2
             n += 1
 
-        #load a few more images...
-        tv.images['hole'] = pygame.image.load(data_dir('gfx','hole.png')).convert_alpha()
-        tv.images['hole2'] = pygame.image.load(data_dir('gfx','hole2.png')).convert_alpha()
-        tv.images['hole3'] = pygame.image.load(data_dir('gfx','hole3.png')).convert_alpha()
-        tv.images['hole4'] = pygame.image.load(data_dir('gfx','hole4.png')).convert_alpha()
-        
-        img = pygame.Surface((1,1)).convert()
-        img.fill((255,0,255))
-        img.set_colorkey((255,0,255))
-        tv.images['blank'] = img
-        
+        # load a few more images...
+        tv.images["hole"] = pygame.image.load(
+            data_dir("gfx", "hole.png")
+        ).convert_alpha()
+        tv.images["hole2"] = pygame.image.load(
+            data_dir("gfx", "hole2.png")
+        ).convert_alpha()
+        tv.images["hole3"] = pygame.image.load(
+            data_dir("gfx", "hole3.png")
+        ).convert_alpha()
+        tv.images["hole4"] = pygame.image.load(
+            data_dir("gfx", "hole4.png")
+        ).convert_alpha()
+
+        img = pygame.Surface((1, 1)).convert()
+        img.fill((255, 0, 255))
+        img.set_colorkey((255, 0, 255))
+        tv.images["blank"] = img
+
         tv.auto_scroll = True
-        
-        self.hairs = pygame.image.load(data_dir("gfx","hairs.tga")).convert_alpha()
+
+        try:
+            self.hairs = pygame.image.load(data_dir("gfx", "hairs.tga")).convert_alpha()
+        except:
+            self.hairs = pygame.image.load(data_dir("gfx", "hairs.png")).convert_alpha()
 
         self.frames = 0
         self.hair_update = None
-        
+
         self.game.magic_castle = tv.castle
         self.interface.stats_draw.robots_total = 0
         self.interface.stats_draw.robots_update = 0
 
         self.last_show_hairs = False
 
     def init(self):
-        #blah blah
+        # blah blah
         pass
-    
-    def paint(self,screen):
-        
+
+    def paint(self, screen):
         tv = self.tv
-        
+
         # we set these variables because the can change.
         SCROLL_MOUSE, SCROLL_AUTO, SCROLL_BORDER = const.get_mouse_info()
 
-
         show_hairs = True
-        
-        if self.frames > FPS: #don't scroll for at least a second...
+
+        if self.frames > FPS:  # don't scroll for at least a second...
             sv = pygame.Rect(S_VIEW)
             border = 8
             sv.x += border
             sv.y += border
-            sv.w -= border*2
-            sv.h -= border *2
+            sv.w -= border * 2
+            sv.h -= border * 2
             v = tv.view
-            x,y = pygame.mouse.get_pos()
+            x, y = pygame.mouse.get_pos()
             inc = SCROLL_MOUSE
-            if not sv.collidepoint((x,y)): tv.auto_scroll = False
-            if x <= sv.left: 
+            if not sv.collidepoint((x, y)):
+                tv.auto_scroll = False
+            if x <= sv.left:
                 v.x -= inc
                 show_hairs = False
-            if x >= sv.right: 
+            if x >= sv.right:
                 v.x += inc
                 show_hairs = False
-            if y <= sv.top: 
+            if y <= sv.top:
                 v.y -= inc
                 show_hairs = False
-            if y >= sv.bottom: 
+            if y >= sv.bottom:
                 v.y += inc
                 show_hairs = False
             c = tv.castle.irect
             if not v.contains(c):
-                if v.left > c.left: v.left = c.left
-                if v.right < c.right: v.right = c.right
-                if v.top > c.top: v.top = c.top
-                if v.bottom < c.bottom: v.bottom = c.bottom
-        
+                if v.left > c.left:
+                    v.left = c.left
+                if v.right < c.right:
+                    v.right = c.right
+                if v.top > c.top:
+                    v.top = c.top
+                if v.bottom < c.bottom:
+                    v.bottom = c.bottom
+
         v = tv.view
         p = tv.castle.irect
         border = SCROLL_BORDER
-        
+
         inc = SCROLL_AUTO
-        if self.frames < 5: #HACK, i don't know what it'll be...
+        if self.frames < 5:  # HACK, i don't know what it'll be...
             inc = 16384
 
-
         # if it isn't moved for a while we turn off mouse look.
         when_last_moved = time.time() - self.last_mouse_event_time
 
-        if when_last_moved > 3.:
+        if when_last_moved > 3.0:
             const.DISABLE_MOUSE_LOOK = 1
 
         # if we move the mouse enough mouse look will go back on.
         if self.last_mouse_moves > 20:
             self.last_mouse_moves = 0
             const.DISABLE_MOUSE_LOOK = 0
 
-
-
         if const.DISABLE_MOUSE_LOOK:
             tv.auto_scroll = True
 
-        #print "autoscrol is :%s:" % tv.auto_scroll
+        # print "autoscrol is :%s:" % tv.auto_scroll
         if tv.auto_scroll:
-            if p.left-border < v.left: 
-                v.left = max(v.left-inc,p.left-border)
-            if p.right+border > v.right: 
-                v.right = min(v.right+inc,p.right+border)
-            if p.top-border < v.top: 
-                v.top = max(v.top-inc,p.top-border)
-            if p.bottom+border > v.bottom: 
-                v.bottom =min(v.bottom+inc, p.bottom+border)
-        
+            if p.left - border < v.left:
+                v.left = max(v.left - inc, p.left - border)
+            if p.right + border > v.right:
+                v.right = min(v.right + inc, p.right + border)
+            if p.top - border < v.top:
+                v.top = max(v.top - inc, p.top - border)
+            if p.bottom + border > v.bottom:
+                v.bottom = min(v.bottom + inc, p.bottom + border)
+
         b = tv.bounds
-        #print "*"*30
-        #print "b is:"
-        #print b
-        #print "v is:"
-        #print v
+        # print "*"*30
+        # print "b is:"
+        # print b
+        # print "v is:"
+        # print v
         if b != None:
-            v.left = max(v.left,b.left)
-            v.right = min(v.right,b.right)
-            v.top = max(v.top,b.top)
-            v.bottom = min(v.bottom,b.bottom)
-        
+            v.left = max(v.left, b.left)
+            v.right = min(v.right, b.right)
+            v.top = max(v.top, b.top)
+            v.bottom = min(v.bottom, b.bottom)
+
         updates = []
-        
+
         s = screen.subsurface(S_VIEW)
-        #s.fill((0,0,0))
+        # s.fill((0,0,0))
         self.tv.paint(s)
-        
+
         updates.append(S_VIEW)
-        
-        vv = len(self.tv.robots)- (self.tv.robots_total*(100-self.percent)/100)
+
+        vv = len(self.tv.robots) - (self.tv.robots_total * (100 - self.percent) / 100)
         if vv != self.interface.stats_draw.robots_total:
-            self.interface.stats_draw.robots_image = self.tv.images['robot'][0]
+            self.interface.stats_draw.robots_image = self.tv.images["robot"][0]
             self.interface.stats_draw.robots_total = vv
-            #self.interface.dirty['background_illustration'] = 1
+            # self.interface.dirty['background_illustration'] = 1
             self.interface.stats_draw.robots_update = 1
 
-
-
         #
         interface_rects = self.interface.update(tv, screen)
         self.interface.stats_draw.robots_update = 0
         updates.extend(interface_rects)
-        
 
         if self.hair_update != None:
             updates.append(self.hair_update)
             self.hair_update = None
-        
-
 
         if show_hairs == True:
-            bmx,bmy = pygame.mouse.get_pos()
+            bmx, bmy = pygame.mouse.get_pos()
 
             if self.last_show_hairs != show_hairs:
                 pass
-                #pygame.mouse.set_visible(False)
-                #pygame.mouse.set_pos((bmx,bmy))
+                # pygame.mouse.set_visible(False)
+                # pygame.mouse.set_pos((bmx,bmy))
 
-            mx,my = pygame.mouse.get_pos()
+            mx, my = pygame.mouse.get_pos()
             hairs = self.hairs
-            hw,hh = hairs.get_width(),hairs.get_height()
-            hr = pygame.Rect((mx-hw/2,my-hh/2,hw,hh))
-            tmp = pygame.Surface((hw,hh),0,32)
-            tmp.blit(screen,(0,0),hr)
-            screen.blit(hairs,hr)
+            hw, hh = hairs.get_width(), hairs.get_height()
+            hr = pygame.Rect((mx - hw / 2, my - hh / 2, hw, hh))
+            tmp = pygame.Surface((hw, hh), 0, 32)
+            tmp.blit(screen, (0, 0), hr)
+            screen.blit(hairs, hr)
             updates.append(hr)
         else:
-            #bmx,bmy = pygame.mouse.get_pos()
+            # bmx,bmy = pygame.mouse.get_pos()
 
             if self.last_show_hairs != show_hairs:
                 pass
-                #pygame.mouse.set_visible(True)
-                #pygame.mouse.set_pos((bmx,bmy))
-       
+                # pygame.mouse.set_visible(True)
+                # pygame.mouse.set_pos((bmx,bmy))
+
         pygame.display.update(updates)
-        
+
         if show_hairs == True:
-            screen.blit(tmp,hr)
+            screen.blit(tmp, hr)
             self.hair_update = hr
         self.last_show_hairs = show_hairs
-        
-    def update(self,screen):
+
+    def update(self, screen):
         self.paint(screen)
-        #[pygame.Rect(0,0,screen.get_width(),screen.get_height())]
-        
+        # [pygame.Rect(0,0,screen.get_width(),screen.get_height())]
 
-    
     def loop(self):
-        
         tv = self.tv
-        
-        #HACK for optimization of gfx
-        tv.tiles[0].image = pygame.Surface((32,32))
-        
+
+        # HACK for optimization of gfx
+        tv.tiles[0].image = pygame.Surface((32, 32))
+
         self.tv.loop()
-        
-        tv.tiles[0].image= None
+
+        tv.tiles[0].image = None
         pass
-        
 
-        if self.frames%(FPS*12) == 0:
+        if self.frames % (FPS * 12) == 0:
             self.interface.new_random_message()
-        
-        
-        #if not self.frames % 5:
+
+        # if not self.frames % 5:
         #    flock.flock(tv.robots, 1, 1)
-        #else:
+        # else:
         #    flock.flock(tv.robots, 0, 0)
         #    pass
-        
-        tv.robots.loop() #flock 'em
-        
-#         for r in tv.robots:
-#             r._frect = r.frect
-#             r.frect = pygame.Rect(r.rect)
 
+        tv.robots.loop()  # flock 'em
 
-        self.frames +=1
+        #         for r in tv.robots:
+        #             r._frect = r.frect
+        #             r.frect = pygame.Rect(r.rect)
 
-        #check to see if the beat the level...
-        if (tv.robots_total-len(tv.robots))*100/tv.robots_total >= self.percent:
+        self.frames += 1
 
-            tv.castle.unit.stats['Health'] = 10.
+        # check to see if the beat the level...
+        if (tv.robots_total - len(tv.robots)) * 100 / tv.robots_total >= self.percent:
+            tv.castle.unit.stats["Health"] = 10.0
             tv.castle.backup_castle()
             self.game.robots_left = len(tv.robots)
             self.game.max_robots = self.interface.max_robots
 
-            #self.interface.max_robots = len(tv.robots)
+            # self.interface.max_robots = len(tv.robots)
+
+            from . import states
 
-            import states
-            self.game.data['levels'].append(self.round)
-            if len(self.game.data['levels']) == 8:
+            self.game.data["levels"].append(self.round)
+            if len(self.game.data["levels"]) == 8:
                 return states.GameWon(self.game)
-            
-            return states.NextLevel(self.game)
 
+            return states.NextLevel(self.game)
 
-    def event(self,e):
-#         if e.type is MOUSEMOTION and 1 in e.buttons:
-#             self.tv.view.x -= e.rel[0]
-#             self.tv.view.y -= e.rel[1]
+    def event(self, e):
+        #         if e.type == MOUSEMOTION and 1 in e.buttons:
+        #             self.tv.view.x -= e.rel[0]
+        #             self.tv.view.y -= e.rel[1]
 
         # if the castle is in a pickup state, then see if enter or right click.
 
         # note the time when the mouse is moved.
         if e.type in [MOUSEMOTION, MOUSEBUTTONDOWN, MOUSEBUTTONUP]:
             self.last_mouse_event_time = time.time()
             self.last_mouse_moves += 1
 
-        self.interface.event(self.tv,e)
+        self.interface.event(self.tv, e)
+
+        self.tv.castle.event(self.tv, e)
+
+        if e.type == KEYDOWN and e.key in (K_RETURN, K_p, K_h):
+            from . import states
+
+            return states.Pause(self.game, "pause", self)
+
+        if e.type == KEYDOWN and e.key == K_ESCAPE:
+            from . import states
+            from . import menu
+
+            return states.Prompt(self.game, "give up? y/n", menu.Menu(self.game), self)
+
+        # CHEAT keys
+        if e.type == KEYDOWN and e.key == K_F10:
+            from . import menu
+            from . import states
 
-        self.tv.castle.event(self.tv,e)
-        
-        if e.type is KEYDOWN and e.key in (K_RETURN,K_p, K_h):
-            import states
-            return states.Pause(self.game,"pause",self)
-        
-        if e.type is KEYDOWN and e.key == K_ESCAPE:
-            import states
-            import menu
-            return states.Prompt(self.game,"give up? y/n",menu.Menu(self.game),self)
-        
-        #CHEAT keys
-        if e.type is KEYDOWN and e.key == K_F10:
-            import menu
-            import states
             return states.GameOver(self.game)
-        if e.type is KEYDOWN and e.key in [K_F11, K_n]:
-            import menu
-            import states
-            self.game.data['levels'].append(self.round)
+        if e.type == KEYDOWN and e.key in [K_F11, K_n]:
+            from . import menu
+            from . import states
+
+            self.game.data["levels"].append(self.round)
             return states.NextLevel(self.game)
-        if e.type is KEYDOWN and e.key in [K_F12, K_v]:
-            import menu
-            import states
-            self.game.data['levels'].append(self.round)
+        if e.type == KEYDOWN and e.key in [K_F12, K_v]:
+            from . import menu
+            from . import states
+
+            self.game.data["levels"].append(self.round)
             return states.GameWon(self.game)
 
-        if e.type is KEYDOWN and e.key in [K_m]:
+        if e.type == KEYDOWN and e.key in [K_m]:
             const.DISABLE_MOUSE_LOOK = not const.DISABLE_MOUSE_LOOK
-    
 
-        #bound the mouse position
+        # bound the mouse position
+
+
 #         x,y = pygame.mouse.get_pos()
 #         r = pygame.Rect(x,y,1,1)
 #         r.clamp_ip(S_VIEW)
 #         pygame.mouse.set_pos((r.x,r.y))
-
-        
-
```

### Comparing `zanthor-1.2.3/zanthor/explode.py` & `zanthor-1.2.4a2/zanthor/explode.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,175 +1,194 @@
 import pygame
 from pygame.locals import *
 import random
 
-from pgu import timer
+from .pgu import timer
 
 rr = random.randrange
 
+
 class Part:
-    def __init__(self,pos):
-        self.pos = pygame.Rect(pos[0],pos[1],1,1)
+    def __init__(self, pos):
+        self.pos = pygame.Rect(pos[0], pos[1], 1, 1)
         self._pos = pygame.Rect(self.pos)
         self.frame = 0
 
-SIZE = 16 #32 is original
+
+SIZE = 16  # 32 is original
+
 
 class Effect:
-    def __init__(self,total,add):
-        
-        if not hasattr(Effect,'init'):
+    def __init__(self, total, add):
+        if not hasattr(Effect, "init"):
             Effect._init(self)
-        
+
         self.total = total
         self._total = 0
         self.add = add
-        
+
         self.parts = []
-        
+
         self.frame = 0
-        
+
     def _init(self):
         Effect.init = True
         Effect.colors = colors = []
-        for r in xrange(0,32):
-            if r < 8: 
-                rr = r-0
-                c = (255,255,255-rr*8)
+        for r in range(0, 32):
+            if r < 8:
+                rr = r - 0
+                c = (255, 255, 255 - rr * 8)
             elif r < 16:
-                rr = r-8
-                c = (255,255-rr*16,255-(rr+8)*8)
+                rr = r - 8
+                c = (255, 255 - rr * 16, 255 - (rr + 8) * 8)
             else:
-                rr = r-16
-                c = (255-rr*8,128-rr*8,128-rr*8)
-                
+                rr = r - 16
+                c = (255 - rr * 8, 128 - rr * 8, 128 - rr * 8)
+
             colors.append(c)
-            
+
         Effect.images = images = []
-        for v in xrange(0,32):
-            r = max(1,v*SIZE/32)
-            img = pygame.Surface((r*2,r*2)).convert()
-            img.fill((255,0,255))
-            img.set_colorkey((255,0,255))
-            img.set_alpha(255-v*8)
-            
-            if v < 8: 
-                rr = v-0
-                c = (255,255,255-rr*8)
+        for v in range(0, 32):
+            r = max(1, v * SIZE // 32)
+            img = pygame.Surface((r * 2, r * 2)).convert()
+            img.fill((255, 0, 255))
+            img.set_colorkey((255, 0, 255))
+            img.set_alpha(255 - v * 8)
+
+            if v < 8:
+                rr = v - 0
+                c = (255, 255, 255 - rr * 8)
             elif v < 16:
-                rr = v-8
-                c = (255,255-rr*16,255-(rr+8)*8)
+                rr = v - 8
+                c = (255, 255 - rr * 16, 255 - (rr + 8) * 8)
             else:
-                rr = v-16
-                c = (255-rr*8,128-rr*8,128-rr*8)
-            #print c
-            pygame.draw.circle(img,c,(r,r),max(1,r/2))
-            #pygame.draw.circle(img,(255-r*8,255-r*8,255-r*8),(r,r),r)
+                rr = v - 16
+                c = (255 - rr * 8, 128 - rr * 8, 128 - rr * 8)
+            # print c
+            pygame.draw.circle(img, c, (r, r), max(1, r // 2))
+            # pygame.draw.circle(img,(255-r*8,255-r*8,255-r*8),(r,r),r)
             images.append(img)
 
-        
-    def paint(self,screen,origin):
-        if self.frame > 16: return
-        
+    def paint(self, screen, origin):
+        if self.frame > 16:
+            return
+
         _screen = screen
-        
+
         center = self.center
-        sz = 240*SIZE/32
-        screen = pygame.Surface((sz,sz)).convert() 
-        screen.fill((80,0,0))
-        screen.set_colorkey((80,0,0))
-        f = max(0,self.frame-8)
-        screen.set_alpha(255-f*32)
-        adj = (sz/2-center[0],sz/2-center[1])
-        
+        sz = 240 * SIZE // 32
+        screen = pygame.Surface((sz, sz)).convert()
+        screen.fill((80, 0, 0))
+        screen.set_colorkey((80, 0, 0))
+        f = max(0, self.frame - 8)
+        screen.set_alpha(255 - f * 32)
+        adj = (sz // 2 - center[0], sz // 2 - center[1])
+
         center = self.center
 
-        todo = [[] for n in xrange(0,32)]
-        
+        todo = [[] for n in range(0, 32)]
+
         for part in self.parts:
-            p,_p = part.pos,part._pos
-            xx,yy = abs(center[0]-p.x),abs(center[1]-p.y)
-            #f = self.frame*2
-            #r = ( abs((xx*xx+yy*yy) - (f*f)))/256
-            r =  (xx*xx+yy*yy) / (256*SIZE/32)
-            #dx,dy = p.x-_p.x,p.y-_p.y
-            #r = ((xx*xx+yy*yy)*(dx*dx+dy*dy))/16384
-            if r >= 0 and r < 32: todo[r].append((_p,p))
-            
-        ox,oy = adj
-        for v in xrange(31,-1,-1):
+            p, _p = part.pos, part._pos
+            xx, yy = abs(center[0] - p.x), abs(center[1] - p.y)
+            # f = self.frame*2
+            # r = ( abs((xx*xx+yy*yy) - (f*f)))/256
+            r = (xx * xx + yy * yy) // (256 * SIZE // 32)
+            # dx,dy = p.x-_p.x,p.y-_p.y
+            # r = ((xx*xx+yy*yy)*(dx*dx+dy*dy))/16384
+            if r >= 0 and r < 32:
+                todo[r].append((_p, p))
+
+        ox, oy = adj
+        for v in range(31, -1, -1):
             img = Effect.images[v]
             c = Effect.colors[v]
-            #v = 255-r*8
-            #c = (v,v,v)
-            #c = (255,255,255,v)
-            r = img.get_width()/2 #max(1,v*SIZE/32)
-            sz = max(1,((32-v)/3+1)*SIZE/32)
-            for _p,p in todo[v]:
-                #pygame.draw.circle(screen,c,(p.x+pos[0],p.y+pos[1]),r+3)
-                #screen.blit(img,(p.x-r+pos[0],p.y-r+pos[1]))
-                
-                dx,dy = p.x-_p.x,p.y-_p.y
-                
-                #sz = self.frame
-                pygame.draw.line(screen,c,(ox+_p.x-dx*1,oy+_p.y-dy*1),(ox+p.x,oy+p.y),sz)
-                screen.blit(img,(p.x-r+adj[0],p.y-r+adj[1]))
-
-        _screen.blit(screen,(-origin[0]+center[0]-screen.get_width()/2,-origin[1]+center[1]-screen.get_height()/2))
-            
-    def loop(self,pos):
-        if self.frame > 20: return
+            # v = 255-r*8
+            # c = (v,v,v)
+            # c = (255,255,255,v)
+            r = img.get_width() // 2  # max(1,v*SIZE/32)
+            sz = max(1, ((32 - v) // 3 + 1) * SIZE // 32)
+            for _p, p in todo[v]:
+                # pygame.draw.circle(screen,c,(p.x+pos[0],p.y+pos[1]),r+3)
+                # screen.blit(img,(p.x-r+pos[0],p.y-r+pos[1]))
+
+                dx, dy = p.x - _p.x, p.y - _p.y
+
+                # sz = self.frame
+                pygame.draw.line(
+                    screen,
+                    c,
+                    (ox + _p.x - dx * 1, oy + _p.y - dy * 1),
+                    (ox + p.x, oy + p.y),
+                    sz,
+                )
+                screen.blit(img, (p.x - r + adj[0], p.y - r + adj[1]))
+
+        _screen.blit(
+            screen,
+            (
+                -origin[0] + center[0] - screen.get_width() // 2,
+                -origin[1] + center[1] - screen.get_height() // 2,
+            ),
+        )
+
+    def loop(self, pos):
+        if self.frame > 20:
+            return
         self.frame += 1
-        
+
         self.center = pos
-            
-            
+
         parts = self.parts
         if self._total < self.total:
-            for n in xrange(0,self.add):
-                part = Part((pos[0]+rr(-12*SIZE/32,13*SIZE/32),pos[1]+rr(-12*SIZE/32,13*SIZE/32)))
-                part._pos.x,part._pos.y = pos[0],pos[1]
+            for n in range(0, self.add):
+                part = Part(
+                    (
+                        pos[0] + rr(-12 * SIZE // 32, 13 * SIZE // 32),
+                        pos[1] + rr(-12 * SIZE // 32, 13 * SIZE // 32),
+                    )
+                )
+                part._pos.x, part._pos.y = pos[0], pos[1]
                 parts.append(part)
                 self._total += 1
         l = len(parts)
         rm = []
         for part in self.parts:
-            p,_p = part.pos,part._pos
+            p, _p = part.pos, part._pos
+
+            dx, dy = p.x - _p.x, p.y - _p.y
+            _p.x, _p.y = p.x, p.y
+
+            p.x += dx
+            p.y += dy
+
+
+if __name__ == "__main__":
+    screen = pygame.display.set_mode((640, 480))
+
+    # ss = [((rr(160,640),rr(160,480)),Effect(256,64)) for n in xrange(0,1)]
 
-            dx,dy = p.x-_p.x,p.y-_p.y
-            _p.x,_p.y = p.x,p.y
-            
-            p.x += dx 
-            p.y += dy 
-            
-            
-            
-if __name__ == '__main__':
-    screen = pygame.display.set_mode((640,480))
-    
-    
-    #ss = [((rr(160,640),rr(160,480)),Effect(256,64)) for n in xrange(0,1)]
-    
     ss = []
-    
+
     t = timer.Timer(40)
-    
+
     f = 0
-    
+
     _quit = False
     while not _quit:
         for e in pygame.event.get():
-            if e.type is QUIT: _quit = True
-            if e.type is KEYDOWN and e.key == K_ESCAPE: _quit = True
-        
-        screen.fill((0,0,0))
-        for pos,s in ss:
+            if e.type == QUIT:
+                _quit = True
+            if e.type == KEYDOWN and e.key == K_ESCAPE:
+                _quit = True
+
+        screen.fill((0, 0, 0))
+        for pos, s in ss:
             s.loop(pos)
-            s.paint(screen,(0,0))
+            s.paint(screen, (0, 0))
         pygame.display.flip()
-        
-        if f%20 == 0:
-            ss = [((rr(160,480),rr(160,320)),Effect(512,128))]
+
+        if f % 20 == 0:
+            ss = [((rr(160, 480), rr(160, 320)), Effect(512, 128))]
         f += 1
-        
+
         t.tick()
-
```

### Comparing `zanthor-1.2.3/zanthor/intro.py` & `zanthor-1.2.4a2/zanthor/intro.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,145 +1,140 @@
-
 import time
 import pygame
 from pygame.locals import *
-from const import *
+from .const import *
 
 import os
-from pgu import engine
+from .pgu import engine
 
-#tempo = 125
-#speed = 6
+# tempo = 125
+# speed = 6
 
 data = [
-    (0,'you',0,64),
-    (8,'are',90,64),
-    (16,'Zanthor',128,144),
-    (28,'and',160,64),
-    (32,'you',190,64),
-    (48,'are',210,64),
-    (64+0,'MAD',255,320),
-    ]
+    (0, "you", 0, 64),
+    (8, "are", 90, 64),
+    (16, "Zanthor", 128, 144),
+    (28, "and", 160, 64),
+    (32, "you", 190, 64),
+    (48, "are", 210, 64),
+    (64 + 0, "MAD", 255, 320),
+]
 
 #     (0,'you',0,32),
 #     (8,'are',90,32),
 #     (16,'Zanthor',128,72),
 #     (28,'and',160,32),
 #     (32,'you',190,32),
 #     (48,'are',210,32),
 #     (64+0,'MAD',255,160),
 
 # uncomment this to test it without a mixer.
-#pygame.mixer = None
+# pygame.mixer = None
+
 
 class Intro(engine.State):
-    
     def init(self):
-        
-        #rev up music...
+        # rev up music...
         if pygame.mixer:
-            pygame.mixer.music.load(data_dir("intro","intro1.ogg"))
-            #pygame.time.wait(2500) #let fullscreen kick in,
+            pygame.mixer.music.load(data_dir("intro", "intro1.ogg"))
+            # pygame.time.wait(2500) #let fullscreen kick in,
             pygame.mixer.music.play()
         else:
             self.cur_time = time.time()
-            self.elapsed_time = 0.
+            self.elapsed_time = 0.0
 
-        im_path = data_dir("intro","introbg.png")
+        im_path = data_dir("intro", "introbg.png")
         self.bkgr = pygame.image.load(im_path).convert()
         screen_size = pygame.display.get_surface().get_size()
-        self.bkgr = pygame.transform.scale( self.bkgr, screen_size )
+        self.bkgr = pygame.transform.scale(self.bkgr, screen_size)
 
         self.fonts = {}
-        
-        for frame,text,alpha,size in data:
-            self.fonts[size] = pygame.font.Font(data_dir("intro","WALSHES.TTF"),size)
- 
 
+        for frame, text, alpha, size in data:
+            self.fonts[size] = pygame.font.Font(data_dir("intro", "WALSHES.TTF"), size)
 
         self.cur = None
         self.frame = 0
-        
+
         pygame.mouse.set_visible(False)
-        
 
-    def paint(self,screen):
+    def paint(self, screen):
         return
-        #screen.fill((0,0,0))
-        #pygame.display.flip()
-        
-        
+        # screen.fill((0,0,0))
+        # pygame.display.flip()
+
     def loop(self):
         if pygame.mixer:
             if not pygame.mixer.music.get_busy():
-                import title
+                from . import title
+
                 return title.Title(self.game)
         else:
             if self.elapsed_time > 15.3462460041:
-                import title
+                from . import title
+
                 return title.Title(self.game)
-                
-    
-    def update(self,screen):
+
+    def update(self, screen):
         if pygame.mixer:
             t = pygame.mixer.music.get_pos()
         else:
             last_time = self.cur_time
             self.cur_time = time.time()
-            self.elapsed_time += (self.cur_time - last_time)
+            self.elapsed_time += self.cur_time - last_time
             t = int(self.elapsed_time * 1000)
-            
 
+        f = t * 125 * 4 / (60 * 1000)
 
-        f = t*125*4/(60*1000)
-        
         for d in data:
             if f >= d[0]:
                 cur = d
-            
-        #print f,'render',cur
-        if cur != self.cur: 
-            self.cur,self.frame = cur,0
-        
-        frame,text,alpha,size = cur
-        
-        if self.frame > 1 and text != 'MAD': return
-        
+
+        # print f,'render',cur
+        if cur != self.cur:
+            self.cur, self.frame = cur, 0
+
+        frame, text, alpha, size = cur
+
+        if self.frame > 1 and text != "MAD":
+            return
+
         fnt = self.fonts[size]
-        
+
         if self.frame == 0:
-            screen.fill((255,255,255))
-            img = fnt.render(text,1,(0,0,0))
-            screen.blit(img,((SW-img.get_width())/2,(SH-img.get_height())/2))
-            
+            screen.fill((255, 255, 255))
+            img = fnt.render(text, 1, (0, 0, 0))
+            screen.blit(img, ((SW - img.get_width()) / 2, (SH - img.get_height()) / 2))
+
         if self.frame > 0:
             v = 0
-            if alpha == 255: v = 255
-            screen.fill((v,0,0))
+            if alpha == 255:
+                v = 255
+            screen.fill((v, 0, 0))
             bg = self.bkgr
-            if text == 'MAD':
-                alpha = max(0,alpha-self.frame*4)
+            if text == "MAD":
+                alpha = max(0, alpha - self.frame * 4)
             bg.set_alpha(alpha)
-            screen.blit(bg,(0,0))
-            img = fnt.render(text,1,(0,0,0))
-            for dx,dy in [(-2,0),(2,0),(0,2),(0,-2)]:
-                screen.blit(img,(dx+(SW-img.get_width())/2,dy+(SH-img.get_height())/2))
-            
-            img = fnt.render(text,1,(255,255,255))
-            screen.blit(img,((SW-img.get_width())/2,(SH-img.get_height())/2))
-            
+            screen.blit(bg, (0, 0))
+            img = fnt.render(text, 1, (0, 0, 0))
+            for dx, dy in [(-2, 0), (2, 0), (0, 2), (0, -2)]:
+                screen.blit(
+                    img,
+                    (dx + (SW - img.get_width()) / 2, dy + (SH - img.get_height()) / 2),
+                )
+
+            img = fnt.render(text, 1, (255, 255, 255))
+            screen.blit(img, ((SW - img.get_width()) / 2, (SH - img.get_height()) / 2))
+
         pygame.display.flip()
-        
+
         self.frame += 1
-        
-        
-    
-    def event(self,e):
-        #if e.type in [KEYDOWN, MOUSEBUTTONDOWN, JOYBUTTONDOWN]:
+
+    def event(self, e):
+        # if e.type in [KEYDOWN, MOUSEBUTTONDOWN, JOYBUTTONDOWN]:
         if e.type in [KEYDOWN, JOYBUTTONDOWN]:
             if pygame.mixer:
                 pygame.mixer.music.stop()
-            import title
+            from . import title
+
             return title.Title(self.game)
-            #return level.Level(self.game,0)
-            
-        
+            # return level.Level(self.game,0)
```

### Comparing `zanthor-1.2.3/zanthor/units.py` & `zanthor-1.2.4a2/zanthor/units.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,422 +1,406 @@
 """ For storing the units information.  All in one file for ease of tweaking.
 """
 
-from const import *
-import items
+from .const import *
+from . import items
 
 
-import cyclic_list
-
+from . import cyclic_list
 
 
 upgrade_amounts = {}
-u= upgrade_amounts
+u = upgrade_amounts
 cl = cyclic_list.cyclic_list
 
-u['UpEngine Efficiency'] = cl([1.0, 2.0, 2.0, 2.0, 2.0,  3.0, 3.0, 3.0, 3.0, 3.0,   4.0, 4.0, 4.0, 4.0, 4.0 ])
-u['UpEngine Speed']      = cl([1.0, 2.0, 2.0, 2.0, 2.0,  3.0, 3.0, 3.0, 3.0, 3.0,   4.0, 4.0, 4.0, 4.0, 4.0 ])
-u['UpCannon Balls']      = cl([1.0, 2.0, 2.0, 2.0, 2.0,  3.0, 3.0, 3.0, 3.0, 3.0,   4.0, 4.0, 4.0, 4.0, 4.0 ])
-u['UpArmour']            = cl([1.0, 2.0, 2.0, 2.0, 2.0,  3.0, 3.0, 3.0, 3.0, 3.0,   4.0, 4.0, 4.0, 4.0, 4.0 ])
-u['UpSteam Tank']        = cl([1.0, 2.0, 2.0, 2.0, 2.0,  3.0, 3.0, 3.0, 3.0, 3.0,   4.0, 4.0, 4.0, 4.0, 4.0 ])
-u['UpWater Tank']        = cl([1.0, 2.0, 2.0, 2.0, 2.0,  3.0, 3.0, 3.0, 3.0, 3.0,   4.0, 4.0, 4.0, 4.0, 4.0 ])
-u['UpCoal Tank']         = cl([1.0, 2.0, 2.0, 2.0, 2.0,  3.0, 3.0, 3.0, 3.0, 3.0,   4.0, 4.0, 4.0, 4.0, 4.0 ])
-u['UpCannon Power']      = cl([1.0, 2.0, 2.0, 2.0, 2.0,  3.0, 3.0, 3.0, 3.0, 3.0,   4.0, 4.0, 4.0, 4.0, 4.0 ])
-
-
-upgrade_words = ["UpEngine Efficiency", "UpEngine Speed", "UpCannon Balls", "UpCannon Power", "UpArmour", "UpSteam Tank", "UpWater Tank", "UpCoal Tank"]
-
-
-
-
+u["UpEngine Efficiency"] = cl(
+    [1.0, 2.0, 2.0, 2.0, 2.0, 3.0, 3.0, 3.0, 3.0, 3.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+)
+u["UpEngine Speed"] = cl(
+    [1.0, 2.0, 2.0, 2.0, 2.0, 3.0, 3.0, 3.0, 3.0, 3.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+)
+u["UpCannon Balls"] = cl(
+    [1.0, 2.0, 2.0, 2.0, 2.0, 3.0, 3.0, 3.0, 3.0, 3.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+)
+u["UpArmour"] = cl(
+    [1.0, 2.0, 2.0, 2.0, 2.0, 3.0, 3.0, 3.0, 3.0, 3.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+)
+u["UpSteam Tank"] = cl(
+    [1.0, 2.0, 2.0, 2.0, 2.0, 3.0, 3.0, 3.0, 3.0, 3.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+)
+u["UpWater Tank"] = cl(
+    [1.0, 2.0, 2.0, 2.0, 2.0, 3.0, 3.0, 3.0, 3.0, 3.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+)
+u["UpCoal Tank"] = cl(
+    [1.0, 2.0, 2.0, 2.0, 2.0, 3.0, 3.0, 3.0, 3.0, 3.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+)
+u["UpCannon Power"] = cl(
+    [1.0, 2.0, 2.0, 2.0, 2.0, 3.0, 3.0, 3.0, 3.0, 3.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+)
+
+
+upgrade_words = [
+    "UpEngine Efficiency",
+    "UpEngine Speed",
+    "UpCannon Balls",
+    "UpCannon Power",
+    "UpArmour",
+    "UpSteam Tank",
+    "UpWater Tank",
+    "UpCoal Tank",
+]
 
 
 class BaseUnit:
-
     def __init__(self, *args, **kwargs):
-
-        self.stats = {"Armour":0., 
-                      "Speed":20., 
-                      "Weight":1., 
-                      "Health":5., 
-                      "Water":10., 
-                      "Coal":10.,
-                      "Steam": 0., 
-                      "CannonPressure": 0., 
-                      "MaxCannonPressure": 16., 
-                      "EngineEfficiency": 1,
-                      "MaxHealth":10., 
-                      "MaxWater":70., 
-                      "MaxCoal":70.,
-                      "MaxSteam": 100., 
-                      "Temperature": 0., 
-                      "Damage": 1., 
-                      "WeaponSteam": 1., 
-                      "MoveSteam": 0.05,
-                      "GenerateSteamCoal": 0.05,
-                      "GenerateSteamWater": 0.05,
-                      }
+        self.stats = {
+            "Armour": 0.0,
+            "Speed": 20.0,
+            "Weight": 1.0,
+            "Health": 5.0,
+            "Water": 10.0,
+            "Coal": 10.0,
+            "Steam": 0.0,
+            "CannonPressure": 0.0,
+            "MaxCannonPressure": 16.0,
+            "EngineEfficiency": 1,
+            "MaxHealth": 10.0,
+            "MaxWater": 70.0,
+            "MaxCoal": 70.0,
+            "MaxSteam": 100.0,
+            "Temperature": 0.0,
+            "Damage": 1.0,
+            "WeaponSteam": 1.0,
+            "MoveSteam": 0.05,
+            "GenerateSteamCoal": 0.05,
+            "GenerateSteamWater": 0.05,
+        }
         self.parts = {}
-        
-
 
     def pickup_item(self, item):
-        """ this picks up the item passed in, and adds it to the robot.
-        """
-
+        """this picks up the item passed in, and adds it to the robot."""
 
         if item.type == items.ITEM_COAL:
-
-            if self.stats['Coal'] >= self.stats['MaxCoal']:
+            if self.stats["Coal"] >= self.stats["MaxCoal"]:
                 return 0
             else:
-                self.stats['Coal'] += item.amount
-                if self.stats['Coal'] >= self.stats['MaxCoal']:
-                    self.stats['Coal'] = self.stats['MaxCoal']
+                self.stats["Coal"] += item.amount
+                if self.stats["Coal"] >= self.stats["MaxCoal"]:
+                    self.stats["Coal"] = self.stats["MaxCoal"]
                 return 1
 
         if item.type == items.ITEM_WATER:
-
-            if self.stats['Water'] >= self.stats['MaxWater']:
+            if self.stats["Water"] >= self.stats["MaxWater"]:
                 return 0
             else:
-                self.stats['Water'] += item.amount
-                if self.stats['Water'] >= self.stats['MaxWater']:
-                    self.stats['Water'] = self.stats['MaxWater']
+                self.stats["Water"] += item.amount
+                if self.stats["Water"] >= self.stats["MaxWater"]:
+                    self.stats["Water"] = self.stats["MaxWater"]
 
                 return 1
-            
+
         if item.type & items.ITEM_PART:
             self.parts[item.name] = item
             return 1
 
         return 0
 
-
     def hit(self, damage_amount):
-        """
-        """
+        """ """
         # we can't do negative damage.
-        x = damage_amount / (self.stats['Armour']+ 1.0)
+        x = damage_amount / (self.stats["Armour"] + 1.0)
         if x > 0:
-            self.stats['Health'] -= x
+            self.stats["Health"] -= x
 
-        if self.stats['Health'] <= 0:
+        if self.stats["Health"] <= 0:
             return 1
         else:
             return 0
 
     def try_move(self):
-        return self.try_use_steam(self.stats['MoveSteam'])
+        return self.try_use_steam(self.stats["MoveSteam"])
 
     def try_fire(self):
-        #print "depricated"
-        return self.try_use_steam(self.stats['WeaponSteam'])
-    
+        # print "depricated"
+        return self.try_use_steam(self.stats["WeaponSteam"])
+
     def prep_fire(self):
-        self.stats['CannonPressure'] = 4
+        self.stats["CannonPressure"] = 4
 
     def try_do_fire(self):
+        if self.stats["CannonPressure"] > self.stats["MaxCannonPressure"]:
+            self.stats["CannonPressure"] = self.stats["MaxCannonPressure"]
 
-        if self.stats['CannonPressure'] > self.stats['MaxCannonPressure']:
-            self.stats['CannonPressure'] = self.stats['MaxCannonPressure']
-
-        if self.stats['CannonPressure'] > self.stats['Steam']:
-            self.stats['CannonPressure'] = self.stats['Steam']
+        if self.stats["CannonPressure"] > self.stats["Steam"]:
+            self.stats["CannonPressure"] = self.stats["Steam"]
 
-        if self.stats['CannonPressure'] < MIN_CANNON_PRESSURE:
-            self.stats['CannonPressure'] = MIN_CANNON_PRESSURE
+        if self.stats["CannonPressure"] < MIN_CANNON_PRESSURE:
+            self.stats["CannonPressure"] = MIN_CANNON_PRESSURE
 
-        if self.try_use_steam(self.stats['CannonPressure']):
-            pressure = self.stats['CannonPressure']
-            self.stats['CannonPressure'] = 0
+        if self.try_use_steam(self.stats["CannonPressure"]):
+            pressure = self.stats["CannonPressure"]
+            self.stats["CannonPressure"] = 0
             return pressure
         else:
-            self.stats['CannonPressure'] = 0
+            self.stats["CannonPressure"] = 0
             return MIN_CANNON_PRESSURE
 
-
     def try_use_steam(self, amount):
-        """ returns 1 if you can, else 0.  It uses up the steam regardless.
-        """
+        """returns 1 if you can, else 0.  It uses up the steam regardless."""
 
         amount /= 2
-        #print "try use steam."
+        # print "try use steam."
 
-        # 
-        if amount > self.stats['Steam']:
-            self.stats['Steam'] = 0.
+        #
+        if amount > self.stats["Steam"]:
+            self.stats["Steam"] = 0.0
             return 0
         else:
-            self.stats['Steam'] -= amount
+            self.stats["Steam"] -= amount
             return 1
 
-
     def loop(self):
         self.generate_steam()
-        
-        if self.stats['CannonPressure']:
-            self.stats['CannonPressure'] += 1.2
-            if self.stats['CannonPressure'] > self.stats['MaxCannonPressure']:
-                self.stats['CannonPressure'] = self.stats['MaxCannonPressure']
-            if self.stats['CannonPressure'] > self.stats['Steam']:
-                self.stats['CannonPressure'] = self.stats['Steam']
-                
-
 
+        if self.stats["CannonPressure"]:
+            self.stats["CannonPressure"] += 1.2
+            if self.stats["CannonPressure"] > self.stats["MaxCannonPressure"]:
+                self.stats["CannonPressure"] = self.stats["MaxCannonPressure"]
+            if self.stats["CannonPressure"] > self.stats["Steam"]:
+                self.stats["CannonPressure"] = self.stats["Steam"]
 
     def generate_steam(self):
-        """ Returns amount of steam it generates from coal & water given.
-        """
+        """Returns amount of steam it generates from coal & water given."""
 
         coal = self.stats["GenerateSteamCoal"]
         water = self.stats["GenerateSteamWater"]
 
-
         # not allowed negatives...
-        assert(coal >= 0)
-        assert(water >= 0)
+        assert coal >= 0
+        assert water >= 0
 
         # if no coal, or no water, then you can't have steam.
         if not coal or not water:
-            print "no coal, or no water passed in for generation"
+            print("no coal, or no water passed in for generation")
             steam = 0
             return 0
         else:
-
             # can only use what we have.
-            if water > self.stats['Water']:
-                water = self.stats['Water']
-
-            if coal > self.stats['Coal']:
-                coal = self.stats['Coal']
+            if water > self.stats["Water"]:
+                water = self.stats["Water"]
 
-            self.stats['Water'] -= water
-            self.stats['Coal'] -= coal
+            if coal > self.stats["Coal"]:
+                coal = self.stats["Coal"]
 
+            self.stats["Water"] -= water
+            self.stats["Coal"] -= coal
 
             if coal == 0 or water == 0:
                 steam = 0
             else:
-                #calculate how much steam we use.
+                # calculate how much steam we use.
                 # ... this is just the average of the coal and water.
                 steam = coal + water
                 if steam > 0:
                     steam = steam / 2
                 else:
                     pass
-                    #print "no coal, or no water left"
+                    # print "no coal, or no water left"
 
         steam = steam * self.stats["EngineEfficiency"]
 
-        total_steam = self.stats['Steam'] + steam
-        if total_steam > self.stats['MaxSteam']:
-            #print "too much steam"
-            self.stats['Steam'] = self.stats['MaxSteam']
+        total_steam = self.stats["Steam"] + steam
+        if total_steam > self.stats["MaxSteam"]:
+            # print "too much steam"
+            self.stats["Steam"] = self.stats["MaxSteam"]
         else:
-            self.stats['Steam'] += steam
+            self.stats["Steam"] += steam
 
         return steam
 
-
     def upgrade_part(self, part_up, amount):
-        """ call this to upgrade one part.
-            part_up - 
-                      UpEngine Efficiency
-                      UpEngine Speed
-                      UpCannon Balls
-                      UpArmour
-                      UpSteam Tank
-                      UpWater Tank
-                      UpCoal Tank
-                      UpCannon Power
+        """call this to upgrade one part.
+        part_up -
+                  UpEngine Efficiency
+                  UpEngine Speed
+                  UpCannon Balls
+                  UpArmour
+                  UpSteam Tank
+                  UpWater Tank
+                  UpCoal Tank
+                  UpCannon Power
         """
 
-        print "upgrading :%s" % part_up
-
+        print(("upgrading :%s" % part_up))
 
         if part_up == "UpEngine Efficiency":
-            self.stats['EngineEfficiency'] += amount
+            self.stats["EngineEfficiency"] += amount
         if part_up == "UpEngine Speed":
-            self.stats['Speed'] += amount
+            self.stats["Speed"] += amount
         if part_up == "UpCannon Balls":
-            self.stats['Damage'] += amount
+            self.stats["Damage"] += amount
         if part_up == "UpArmour":
-            self.stats['Armour'] += amount
+            self.stats["Armour"] += amount
         if part_up == "UpSteam Tank":
-            self.stats['MaxSteam'] += amount
+            self.stats["MaxSteam"] += amount
         if part_up == "UpWater Tank":
-            self.stats['MaxWater'] += amount
+            self.stats["MaxWater"] += amount
         if part_up == "UpCoal Tank":
-            self.stats['MaxCoal'] += amount
+            self.stats["MaxCoal"] += amount
         if part_up == "UpCannon Power":
-            self.stats['MaxCannonPressure'] += amount
+            self.stats["MaxCannonPressure"] += amount
 
 
 class Castle(BaseUnit):
-    
     def __init__(self, *args, **kwargs):
         BaseUnit.__init__(self, *args, **kwargs)
 
         self.name = "castle"
 
-        self.stats = {"Armour":0., 
-                      "Speed":10., 
-                      "Weight":1., 
-                      "Health":10., 
-                      "Water":65., 
-                      "Coal":65.,
-                      "Steam": 100., 
-                      "EngineEfficiency": 3.,
-
-                      "CannonPressure": 0., 
-                      "MaxCannonPressure": 16., 
-                      "MaxHealth":10., 
-                      "MaxWater":70., 
-                      "MaxCoal":70.,
-                      "MaxSteam": 100., 
-                      "Temperature": 0., 
-                      "Damage": 1., 
-                      "WeaponSteam": 1., 
-                      "MoveSteam": 0.05,
-                      "GenerateSteamCoal": 0.05,
-                      "GenerateSteamWater": 0.05,
-
-                      "UpEngine Speed":0,
-                      "UpEngine Efficiency":0,
-                      "UpCannon Balls":0,
-                      "UpCannon Power":0,
-                      "UpArmour":0,
-                      "UpSteam Tank":0,
-                      "UpWater Tank":0,
-                      "UpCoal Tank":0,
-                      "upgrade_amounts": upgrade_amounts,
-                      }
+        self.stats = {
+            "Armour": 0.0,
+            "Speed": 10.0,
+            "Weight": 1.0,
+            "Health": 10.0,
+            "Water": 65.0,
+            "Coal": 65.0,
+            "Steam": 100.0,
+            "EngineEfficiency": 3.0,
+            "CannonPressure": 0.0,
+            "MaxCannonPressure": 16.0,
+            "MaxHealth": 10.0,
+            "MaxWater": 70.0,
+            "MaxCoal": 70.0,
+            "MaxSteam": 100.0,
+            "Temperature": 0.0,
+            "Damage": 1.0,
+            "WeaponSteam": 1.0,
+            "MoveSteam": 0.05,
+            "GenerateSteamCoal": 0.05,
+            "GenerateSteamWater": 0.05,
+            "UpEngine Speed": 0,
+            "UpEngine Efficiency": 0,
+            "UpCannon Balls": 0,
+            "UpCannon Power": 0,
+            "UpArmour": 0,
+            "UpSteam Tank": 0,
+            "UpWater Tank": 0,
+            "UpCoal Tank": 0,
+            "upgrade_amounts": upgrade_amounts,
+        }
 
 
 class Robot(BaseUnit):
-    
-
     def __init__(self, *args, **kwargs):
         BaseUnit.__init__(self, *args, **kwargs)
         self.name = "baddie_robot"
 
-        self.stats = {"Armour":0., 
-                      "Speed":20., 
-                      "Weight":1., 
-                      "Health":5., 
-                      "Water":10., 
-                      "Coal":10.,
-                      "EngineEfficiency": 1,
-                      "Steam": 100., 
-                      "CannonPressure": 0., 
-                      "MaxCannonPressure": 16., 
-                      "MaxHealth":70., 
-                      "MaxWater":70., 
-                      "MaxCoal":70.,
-                      "MaxSteam": 70., 
-                      "Temperature": 0., 
-                      "Damage": 1., 
-                      "WeaponSteam": 1., 
-                      "MoveSteam": 0.05,
-                      "GenerateSteamCoal": 0.05,
-                      "GenerateSteamWater": 0.05,
-                      }
+        self.stats = {
+            "Armour": 0.0,
+            "Speed": 20.0,
+            "Weight": 1.0,
+            "Health": 5.0,
+            "Water": 10.0,
+            "Coal": 10.0,
+            "EngineEfficiency": 1,
+            "Steam": 100.0,
+            "CannonPressure": 0.0,
+            "MaxCannonPressure": 16.0,
+            "MaxHealth": 70.0,
+            "MaxWater": 70.0,
+            "MaxCoal": 70.0,
+            "MaxSteam": 70.0,
+            "Temperature": 0.0,
+            "Damage": 1.0,
+            "WeaponSteam": 1.0,
+            "MoveSteam": 0.05,
+            "GenerateSteamCoal": 0.05,
+            "GenerateSteamWater": 0.05,
+        }
 
 
 class CannonTower(BaseUnit):
-    
-
     def __init__(self, *args, **kwargs):
         BaseUnit.__init__(self, *args, **kwargs)
 
         self.name = "cannon_tower"
 
-        self.stats = {"Armour":0., 
-                      "Speed":0., 
-                      "Weight":1., 
-                      "Health":3., 
-                      "Water":10., 
-                      "Coal":10.,
-                      "Steam": 100.,
-                      "MaxHealth":70., 
-                      "EngineEfficiency": 1,
-                      "MaxWater":70., 
-                      "MaxCoal":70.,
-                      "MaxSteam": 70., 
-                      "CannonPressure": 0., 
-                      "MaxCannonPressure": 16., 
-
-                      "Temperature": 0.,
-                      "Damage": 1.,
-                      "WeaponSteam": 1.,
-                      "MoveSteam": 0.05,
-                      "GenerateSteamCoal": 0.05,
-                      "GenerateSteamWater": 0.05,
-                      }
+        self.stats = {
+            "Armour": 0.0,
+            "Speed": 0.0,
+            "Weight": 1.0,
+            "Health": 3.0,
+            "Water": 10.0,
+            "Coal": 10.0,
+            "Steam": 100.0,
+            "MaxHealth": 70.0,
+            "EngineEfficiency": 1,
+            "MaxWater": 70.0,
+            "MaxCoal": 70.0,
+            "MaxSteam": 70.0,
+            "CannonPressure": 0.0,
+            "MaxCannonPressure": 16.0,
+            "Temperature": 0.0,
+            "Damage": 1.0,
+            "WeaponSteam": 1.0,
+            "MoveSteam": 0.05,
+            "GenerateSteamCoal": 0.05,
+            "GenerateSteamWater": 0.05,
+        }
 
 
 class CoalTruck(BaseUnit):
-    
-
     def __init__(self, *args, **kwargs):
         BaseUnit.__init__(self, *args, **kwargs)
         self.name = "coal_truck"
 
-        self.stats = {"Armour":0., 
-                      "Speed":20., 
-                      "Weight":1., 
-                      "Health":5., 
-                      "Water":10., 
-                      "Coal":10.,
-                      "Steam": 100., 
-                      "EngineEfficiency": 1,
-                      "MaxHealth":70., 
-                      "MaxWater":70., 
-                      "MaxCoal":70.,
-                      "MaxSteam": 70., 
-                      "CannonPressure": 0., 
-                      "MaxCannonPressure": 16., 
-
-                      "Temperature": 0., 
-                      "Damage": 1., 
-                      "WeaponSteam": 1., 
-                      "MoveSteam": 0.05,
-                      "GenerateSteamCoal": 0.05,
-                      "GenerateSteamWater": 0.05,
-                      }
+        self.stats = {
+            "Armour": 0.0,
+            "Speed": 20.0,
+            "Weight": 1.0,
+            "Health": 5.0,
+            "Water": 10.0,
+            "Coal": 10.0,
+            "Steam": 100.0,
+            "EngineEfficiency": 1,
+            "MaxHealth": 70.0,
+            "MaxWater": 70.0,
+            "MaxCoal": 70.0,
+            "MaxSteam": 70.0,
+            "CannonPressure": 0.0,
+            "MaxCannonPressure": 16.0,
+            "Temperature": 0.0,
+            "Damage": 1.0,
+            "WeaponSteam": 1.0,
+            "MoveSteam": 0.05,
+            "GenerateSteamCoal": 0.05,
+            "GenerateSteamWater": 0.05,
+        }
 
 
 class Factory(BaseUnit):
-
     def __init__(self, *args, **kwargs):
         BaseUnit.__init__(self, *args, **kwargs)
         self.name = "factory"
 
-        self.stats = {"Armour":0., 
-                      "Speed":20., 
-                      "Weight":1., 
-                      "Health":5., 
-                      "Water":10., 
-                      "EngineEfficiency": 1,
-                      "Coal":10.,
-                      "Steam": 100., 
-                      "MaxHealth":70., 
-                      "MaxWater":70., 
-                      "MaxCoal":70.,
-                      "MaxSteam": 70., 
-                      "CannonPressure": 0., 
-                      "MaxCannonPressure": 16., 
-
-                      "Temperature": 0., 
-                      "Damage": 1., 
-                      "WeaponSteam": 1., 
-                      "MoveSteam": 0.05,
-                      "GenerateSteamCoal": 0.05,
-                      "GenerateSteamWater": 0.05,
-                      }
-
-
-
-
-
-
+        self.stats = {
+            "Armour": 0.0,
+            "Speed": 20.0,
+            "Weight": 1.0,
+            "Health": 5.0,
+            "Water": 10.0,
+            "EngineEfficiency": 1,
+            "Coal": 10.0,
+            "Steam": 100.0,
+            "MaxHealth": 70.0,
+            "MaxWater": 70.0,
+            "MaxCoal": 70.0,
+            "MaxSteam": 70.0,
+            "CannonPressure": 0.0,
+            "MaxCannonPressure": 16.0,
+            "Temperature": 0.0,
+            "Damage": 1.0,
+            "WeaponSteam": 1.0,
+            "MoveSteam": 0.05,
+            "GenerateSteamCoal": 0.05,
+            "GenerateSteamWater": 0.05,
+        }
```

### Comparing `zanthor-1.2.3/zanthor/items.py` & `zanthor-1.2.4a2/zanthor/items.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,59 @@
-
-ITEM_COAL            = 0x0001
-ITEM_WATER           = 0x0002
-ITEM_PART            = 0x0010
-ITEM_CANNON          = 0x0020
-ITEM_ENGINE          = 0x0030
-ITEM_WATERTANK       = 0x0040
+ITEM_COAL = 0x0001
+ITEM_WATER = 0x0002
+ITEM_PART = 0x0010
+ITEM_CANNON = 0x0020
+ITEM_ENGINE = 0x0030
+ITEM_WATERTANK = 0x0040
 ITEM_COALSTORAGEROOM = 0x0050
-ITEM_ARMOUR          = 0x0060
-ITEM_RUBBLE          = 0x0100
+ITEM_ARMOUR = 0x0060
+ITEM_RUBBLE = 0x0100
 ITEM_ = 10
 ITEM_ = 11
 ITEM_ = 12
 ITEM_ = 13
 ITEM_ = 14
 ITEM_ = 15
 ITEM_ = 16
 
+
 class Coal:
     type = ITEM_COAL
 
-    def __init__(self, amount = 1.0):
+    def __init__(self, amount=1.0):
         self.amount = amount
         self.name = "Coal"
         self.pickup_string = "Pick up some Coal?"
 
+
 class Water:
     type = ITEM_WATER
 
-    def __init__(self, amount = 1.0):
+    def __init__(self, amount=1.0):
         self.amount = amount
         self.name = "Water"
         self.pickup_string = "Suck up some water?"
 
+
 class Rubble:
     type = ITEM_RUBBLE
 
     def __init__(self):
         self.name = "Rubble"
         self.pickup_string = "Pick up some rubble?"
 
 
-
-
-
 class Cannon:
     type = ITEM_CANNON
 
     def __init__(self):
         self.name = "cannon"
         self.pickup_string = "Pick up a Cannon?"
 
 
-
 class Part:
     type = ITEM_PART
 
     def __init__(self, name, pickup_string):
         self.name = name
         self.pickup_string = pickup_string
 
@@ -63,173 +61,156 @@
 class Engine:
     type = ITEM_ENGINE
 
     def __init__(self):
         self.name = "engine"
         self.pickup_string = "Pick up an engine?"
 
+
 class WaterTank:
     type = ITEM_WATERTANK
 
     def __init__(self):
         self.name = "water tank"
         self.pickup_string = "Pick up a water tank?"
 
+
 class CoalStorageRoom:
     type = ITEM_COALSTORAGEROOM
 
     def __init__(self):
         self.name = "coal storage room"
         self.pickup_string = "Pick up a coal storage room?"
 
+
 class Armour:
     type = ITEM_ARMOUR
 
     def __init__(self):
         self.name = "armour"
         self.pickup_string = "Pick up some armour?"
 
 
-
-
-
-def coal_new(g,t,value):
+def coal_new(g, t, value):
     g.clayer[t.ty][t.tx] = 0
-    s = isovid.Sprite(g.images['coal'],t.rect)
+    s = isovid.Sprite(g.images["coal"], t.rect)
     s.frame = 0
 
-    s.item = items.Coal(1.)
+    s.item = items.Coal(1.0)
 
     g.sprites.append(s)
     s.loop = coal_loop
 
-    s.groups = g.string2groups('coal')
-    s.agroups = g.string2groups('castle')
+    s.groups = g.string2groups("coal")
+    s.agroups = g.string2groups("castle")
     s.hit = coal_hit
-    
-    import fire
-    #s.effect = fire.Effect(64,1)
 
+    from . import fire
 
-def coal_hit(g,s,a):
-    #print "coal hit"
-    pass
+    # s.effect = fire.Effect(64,1)
 
 
-
-def coal_loop(g,s):
+def coal_hit(g, s, a):
+    # print "coal hit"
     pass
-    #s.rect.clamp_ip(g.view)
-    s.frame +=1
-    
 
 
+def coal_loop(g, s):
+    pass
+    # s.rect.clamp_ip(g.view)
+    s.frame += 1
 
 
-def cannon_tower_new(g,t,value):
+def cannon_tower_new(g, t, value):
     g.clayer[t.ty][t.tx] = 0
-    s = isovid.Sprite(g.images['cannon_tower'],t.rect)
+    s = isovid.Sprite(g.images["cannon_tower"], t.rect)
 
-    s.item = items.Coal(1.)
+    s.item = items.Coal(1.0)
 
     g.sprites.append(s)
     s.loop = cannon_tower_loop
 
-    #s.groups = g.string2groups('cannon_tower')
-    #s.agroups = g.string2groups('castle')
-    #s.hit = cannon_tower_hit
-
+    # s.groups = g.string2groups('cannon_tower')
+    # s.agroups = g.string2groups('castle')
+    # s.hit = cannon_tower_hit
 
-def cannon_tower_hit(g,s,a):
-    pass
 
-def cannon_tower_loop(g,s):
+def cannon_tower_hit(g, s, a):
     pass
 
 
+def cannon_tower_loop(g, s):
+    pass
 
 
-
-    
-def water_new(g,t,value):
+def water_new(g, t, value):
     g.clayer[t.ty][t.tx] = 0
 
-    s = isovid.Sprite(g.images['water'],t.rect)
+    s = isovid.Sprite(g.images["water"], t.rect)
     g.sprites.append(s)
-    #s.groups = g.string2groups('coal')
-    #s.agroups = g.string2groups('castle')
-    #s.hit = coal_hit
+    # s.groups = g.string2groups('coal')
+    # s.agroups = g.string2groups('castle')
+    # s.hit = coal_hit
 
-    s.frame = random.randrange(0,32)
+    s.frame = random.randrange(0, 32)
     s.loop = water_loop
-    
-def water_loop(g,s):
 
-    #if s.frame%20 == 0:
+
+def water_loop(g, s):
+    # if s.frame%20 == 0:
     #    import explode
     #    s.effect = explode.Effect(512,128)
     #    pass
-        
-    s.frame += 1
-
-
 
+    s.frame += 1
 
 
-def human_new(g,t,value):
+def human_new(g, t, value):
     g.clayer[t.ty][t.tx] = 0
 
-    s = isovid.Sprite(g.images['human'],t.rect)
+    s = isovid.Sprite(g.images["human"], t.rect)
     g.sprites.append(s)
 
-    s.frame = random.randrange(0,32)
+    s.frame = random.randrange(0, 32)
     s.loop = human_loop
-    
 
-def human_loop(g,s):
-    s.frame += 1
 
+def human_loop(g, s):
+    s.frame += 1
 
 
-def wall_new(g,t,value):
+def wall_new(g, t, value):
     g.clayer[t.ty][t.tx] = 0
 
-    s = isovid.Sprite(g.images['wall'],t.rect)
+    s = isovid.Sprite(g.images["wall"], t.rect)
     g.sprites.append(s)
 
-    s.frame = random.randrange(0,32)
+    s.frame = random.randrange(0, 32)
     s.loop = wall_loop
-    
-
-def wall_loop(g,s):
-    s.frame += 1
 
 
+def wall_loop(g, s):
+    s.frame += 1
 
 
-def baddie_robot_new(g,t,value):
+def baddie_robot_new(g, t, value):
     g.clayer[t.ty][t.tx] = 0
 
-    s = isovid.Sprite(g.images['baddie_robot'],t.rect)
+    s = isovid.Sprite(g.images["baddie_robot"], t.rect)
     g.sprites.append(s)
 
-    s.frame = random.randrange(0,32)
+    s.frame = random.randrange(0, 32)
     s.loop = baddie_robot_loop
-    
 
-def baddie_robot_loop(g,s):
-    s.frame += 1
 
+def baddie_robot_loop(g, s):
+    s.frame += 1
 
 
 # castle
 # human
 # factory
 # coal
 # water
 # cannon towers
 # walls
 # baddie robots. not castles, but smaller sleaker ones.
-
-
-
-
```

### Comparing `zanthor-1.2.3/zanthor/data/gfx/caastles.png` & `zanthor-1.2.4a2/zanthor/data/gfx/caastles.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/background_illustration.png` & `zanthor-1.2.4a2/zanthor/data/gfx/background_illustration.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/heart.xcf.bz2` & `zanthor-1.2.4a2/zanthor/data/gfx/heart.xcf.bz2`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/tiles.tga` & `zanthor-1.2.4a2/zanthor/data/gfx/tiles.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/background_equipment.png` & `zanthor-1.2.4a2/zanthor/data/gfx/background_equipment.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/hairs.tga` & `zanthor-1.2.4a2/zanthor/data/gfx/hairs.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/coal.png` & `zanthor-1.2.4a2/zanthor/data/gfx/coal.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/background_bottom.png` & `zanthor-1.2.4a2/zanthor/data/gfx/background_bottom.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/hole2.png` & `zanthor-1.2.4a2/zanthor/data/gfx/hole2.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/tiles2.tga` & `zanthor-1.2.4a2/zanthor/data/gfx/tiles2.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/hole.png` & `zanthor-1.2.4a2/zanthor/data/gfx/hole.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/background_status_left.png` & `zanthor-1.2.4a2/zanthor/data/gfx/background_status_left.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/heart_pulse.png` & `zanthor-1.2.4a2/zanthor/data/gfx/heart_pulse.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/castle1.tga` & `zanthor-1.2.4a2/zanthor/data/gfx/castle1.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/tileedit.py` & `zanthor-1.2.4a2/zanthor/data/gfx/tileedit.py`

 * *Files 19% similar despite different names*

```diff
@@ -56,938 +56,1188 @@
 . - flip vertical
 
 arrows - change tile
 F10 - toggle fullscreen
 </pre>
 """
 
-import os,sys    
+import os, sys
 from optparse import OptionParser
-from ConfigParser import ConfigParser
+from configparser import ConfigParser
 import pygame
 from pygame.locals import *
 
 try:
     import Image
-    have_pil=True
+
+    have_pil = True
 except:
-    print "import Image failure; PIL not found."
-    have_pil=False
+    print("import Image failure; PIL not found.")
+    have_pil = False
 
 have_pil = False
 
 
 # the following line is not needed if pgl is installed
-import sys; sys.path.insert(0, "..")
+import sys
+
+sys.path.insert(0, "..")
 import shutil
 
 from pgu import gui, html
 
 
-#whatever...
+# whatever...
 ini_fname = "tileedit.ini"
 ini = ConfigParser()
 
 cfg = {}
 
+
 class _app(gui.Container):
     def __init__(self):
         gui.Container.__init__(self)
-        #self.cls = "desktop"
-        #self.background = gui.Box(self.style.background)
-        
-        self.screen_w = cfg['screen_w']
-        self.screen_h = cfg['screen_h']
-        self.screen = pygame.display.set_mode((self.screen_w,self.screen_h),SWSURFACE)
-        
-        self.fname = cfg['fname']
+        # self.cls = "desktop"
+        # self.background = gui.Box(self.style.background)
 
-        if self.fname != None:
-            if have_pil==True:
+        self.screen_w = cfg["screen_w"]
+        self.screen_h = cfg["screen_h"]
+        self.screen = pygame.display.set_mode((self.screen_w, self.screen_h), SWSURFACE)
 
+        self.fname = cfg["fname"]
+
+        if self.fname != None:
+            if have_pil == True:
                 im = Image.open(self.fname)
                 mode = im.mode
                 size = im.size
                 data = im.tostring()
-		print mode
+                print(mode)
 
                 assert mode in ["RGB", "RGBA"]
 
                 self.tiles = pygame.image.fromstring(data, size, mode)
 
             else:
-                self.tiles = pygame.image.load(self.fname) # old tga-only method
+                self.tiles = pygame.image.load(self.fname)  # old tga-only method
         else:
-            w,h = cfg['width'],cfg['height']
-            s = pygame.Surface((w,h),SWSURFACE|SRCALPHA,32)
-            s.fill((0,0,0,0))
+            w, h = cfg["width"], cfg["height"]
+            s = pygame.Surface((w, h), SWSURFACE | SRCALPHA, 32)
+            s.fill((0, 0, 0, 0))
             self.tiles = s
 
-        self.tiles_w, self.tiles_h = self.tiles.get_width(),self.tiles.get_height()
-            
-        
-        self.tile_w, self.tile_h = cfg['tile_w'],cfg['tile_h'] 
-        self.tile = self.tiles.subsurface((0,0,self.tile_w,self.tile_h))
-        
-        self.color = (255,255,255,255)
-        self.mode = 'draw'
+        self.tiles_w, self.tiles_h = self.tiles.get_width(), self.tiles.get_height()
+
+        self.tile_w, self.tile_h = cfg["tile_w"], cfg["tile_h"]
+        self.tile = self.tiles.subsurface((0, 0, self.tile_w, self.tile_h))
+
+        self.color = (255, 255, 255, 255)
+        self.mode = "draw"
         self.clipboard = None
-        self.select = Rect(0,0,self.tile_w,self.tile_h)
+        self.select = Rect(0, 0, self.tile_w, self.tile_h)
         self.history = []
         self.dirty = 0
-        
+
     def archive(self):
         h = self.history
         if len(h) >= 32:
             del h[0]
-        c = pygame.Surface((self.tile_w,self.tile_h),SWSURFACE,self.tile)
-        c.fill((0,0,0,0))
-        c.blit(self.tile,(0,0))
-        h.append((c,self.tile.get_offset()))
+        c = pygame.Surface((self.tile_w, self.tile_h), SWSURFACE, self.tile)
+        c.fill((0, 0, 0, 0))
+        c.blit(self.tile, (0, 0))
+        h.append((c, self.tile.get_offset()))
         self.dirty = 1
-        
+
     def undo(self):
-        if len(self.history) == 0: return
-        c,off = self.history.pop()
-        self.tiles.fill((0,0,0,0),(off[0],off[1],self.tile_w,self.tile_h))
-        self.tiles.blit(c,off)
+        if len(self.history) == 0:
+            return
+        c, off = self.history.pop()
+        self.tiles.fill((0, 0, 0, 0), (off[0], off[1], self.tile_w, self.tile_h))
+        self.tiles.blit(c, off)
         self.tdraw.repaint()
         self.tpicker.repaint()
         self.dirty = 1
-        
-    def __setattr__(self,k,v):
+
+    def __setattr__(self, k, v):
         self.__dict__[k] = v
-        
-        if k == 'color':
-            if hasattr(self,'cpreview'): self.cpreview.repaint()
-        if k == 'tile':
-            if hasattr(self,'tdraw'): self.tdraw.repaint()
-            if hasattr(self,'tpicker'): self.tpicker.repaint()
-            if hasattr(self,'tpreview'): self.tpreview.repaint()
-    def event(self,e):
-        if e.type is KEYDOWN:
-            for key,cmd,value in keys:
+
+        if k == "color":
+            if hasattr(self, "cpreview"):
+                self.cpreview.repaint()
+        if k == "tile":
+            if hasattr(self, "tdraw"):
+                self.tdraw.repaint()
+            if hasattr(self, "tpicker"):
+                self.tpicker.repaint()
+            if hasattr(self, "tpreview"):
+                self.tpreview.repaint()
+
+    def event(self, e):
+        if e.type == KEYDOWN:
+            for key, cmd, value in keys:
                 if e.key == key:
                     cmd(value)
                     return
-        return gui.Container.event(self,e)
-    
+        return gui.Container.event(self, e)
+
+
 class cpreview(gui.Widget):
-    def __init__(self,w,h):
+    def __init__(self, w, h):
         gui.Widget.__init__(self)
-        self.style.width = w 
+        self.style.width = w
         self.style.height = h
-        
-    def paint(self,s):
-        s.fill((128,128,128))
+
+    def paint(self, s):
+        s.fill((128, 128, 128))
         s.fill(app.color)
 
-        
+
 class cpicker(gui.Widget):
-    def __init__(self,w,h,pal):
+    def __init__(self, w, h, pal):
         gui.Widget.__init__(self)
         self.style.width = w
         self.style.height = h
         self.palette = pal
         self.palette_w = pal.get_width()
         self.palette_h = pal.get_height()
-    
-    def paint(self,s):
-        s.blit(pygame.transform.scale(self.palette,(self.rect.w,self.rect.h)),(0,0))
-            
-    def event(self,e):
-        if (e.type is MOUSEBUTTONDOWN) or (e.type is MOUSEMOTION and e.buttons[0] == 1 and self.container.myfocus == self):
-            x,y = e.pos[0]*self.palette_w/self.rect.w,e.pos[1]*self.palette_h/self.rect.h
-            x,y = max(0,x),max(0,y)
-            x,y = min(self.palette_w-1,x),min(self.palette_h-1,y)
-        
-            app.color = self.palette.get_at((x,y))
+
+    def paint(self, s):
+        s.blit(pygame.transform.scale(self.palette, (self.rect.w, self.rect.h)), (0, 0))
+
+    def event(self, e):
+        if (e.type == MOUSEBUTTONDOWN) or (
+            e.type == MOUSEMOTION
+            and e.buttons[0] == 1
+            and self.container.myfocus == self
+        ):
+            x, y = (
+                e.pos[0] * self.palette_w / self.rect.w,
+                e.pos[1] * self.palette_h / self.rect.h,
+            )
+            x, y = max(0, x), max(0, y)
+            x, y = min(self.palette_w - 1, x), min(self.palette_h - 1, y)
+
+            app.color = self.palette.get_at((x, y))
+
 
 class tpicker(gui.Widget):
     def __init__(self):
         gui.Widget.__init__(self)
         self.style.width = app.tiles_w
         self.style.height = app.tiles_h
-        
-    def paint(self,s):
-        s.fill((128,128,128))
-        s.blit(app.tiles,(0,0))
+
+    def paint(self, s):
+        s.fill((128, 128, 128))
+        s.blit(app.tiles, (0, 0))
         off = app.tile.get_offset()
-        pygame.draw.rect(s,(255,255,255),(off[0],off[1],app.tile_w,app.tile_h),2)
-        
-    def pick(self,pos):
-        x,y = pos
-        while x < 0: x += self.rect.w
-        while y < 0: y += self.rect.h
-        while x >= self.rect.w: x -= self.rect.w
-        while y >= self.rect.h: y -= self.rect.h
-        app.tile = app.tiles.subsurface((x,y,app.tile_w,app.tile_h))
-
-    def event(self,e):
-        if (e.type is MOUSEBUTTONDOWN and e.button == 1) or (e.type is MOUSEMOTION and e.buttons[0] == 1 and self.container.myfocus == self):
-            x,y = e.pos[0]/app.tile_w*app.tile_w,e.pos[1]/app.tile_h*app.tile_h
-            self.pick((x,y))
-            
-        if (e.type is MOUSEBUTTONDOWN and e.button == 3) or (e.type is MOUSEMOTION and e.buttons[2] == 1 and self.container.myfocus == self):
-            x,y = e.pos[0]-app.tile_w/2,e.pos[1]-app.tile_h/2
-            x = min(self.rect.w-app.tile_w-1,max(0,x))
-            y = min(self.rect.h-app.tile_h-1,max(0,y))
-            self.pick((x,y))
+        pygame.draw.rect(
+            s, (255, 255, 255), (off[0], off[1], app.tile_w, app.tile_h), 2
+        )
+
+    def pick(self, pos):
+        x, y = pos
+        while x < 0:
+            x += self.rect.w
+        while y < 0:
+            y += self.rect.h
+        while x >= self.rect.w:
+            x -= self.rect.w
+        while y >= self.rect.h:
+            y -= self.rect.h
+        app.tile = app.tiles.subsurface((x, y, app.tile_w, app.tile_h))
+
+    def event(self, e):
+        if (e.type == MOUSEBUTTONDOWN and e.button == 1) or (
+            e.type == MOUSEMOTION
+            and e.buttons[0] == 1
+            and self.container.myfocus == self
+        ):
+            x, y = (
+                e.pos[0] / app.tile_w * app.tile_w,
+                e.pos[1] / app.tile_h * app.tile_h,
+            )
+            self.pick((x, y))
+
+        if (e.type == MOUSEBUTTONDOWN and e.button == 3) or (
+            e.type == MOUSEMOTION
+            and e.buttons[2] == 1
+            and self.container.myfocus == self
+        ):
+            x, y = e.pos[0] - app.tile_w / 2, e.pos[1] - app.tile_h / 2
+            x = min(self.rect.w - app.tile_w - 1, max(0, x))
+            y = min(self.rect.h - app.tile_h - 1, max(0, y))
+            self.pick((x, y))
+
 
 class tpreview(gui.Widget):
     def __init__(self):
         gui.Widget.__init__(self)
-        self.style.width = app.tile_w*3
-        self.style.height = app.tile_h*3
+        self.style.width = app.tile_w * 3
+        self.style.height = app.tile_h * 3
+
     def paint(self, s):
         atw = app.tile_w
         ath = app.tile_h
-        s.fill((100,100,100))
-        s.blit(app.tile,(0,0))
-        s.blit(app.tile,(1*atw,0))
-        s.blit(app.tile,(2*atw,0))
-        s.blit(app.tile,(0,1*ath))
-        s.blit(app.tile,(1*atw,1*ath))
-        s.blit(app.tile,(2*atw,1*ath))
-        s.blit(app.tile,(0,2*ath))
-        s.blit(app.tile,(1*atw,2*ath))
-        s.blit(app.tile,(2*atw,2*ath))        
+        s.fill((100, 100, 100))
+        s.blit(app.tile, (0, 0))
+        s.blit(app.tile, (1 * atw, 0))
+        s.blit(app.tile, (2 * atw, 0))
+        s.blit(app.tile, (0, 1 * ath))
+        s.blit(app.tile, (1 * atw, 1 * ath))
+        s.blit(app.tile, (2 * atw, 1 * ath))
+        s.blit(app.tile, (0, 2 * ath))
+        s.blit(app.tile, (1 * atw, 2 * ath))
+        s.blit(app.tile, (2 * atw, 2 * ath))
+
 
 class tdraw(gui.Widget):
-    def __init__(self,w,h):
+    def __init__(self, w, h):
         gui.Widget.__init__(self)
         self.rect.w = self.style.width = w
         self.rect.h = self.style.height = h
-        self.overlay = pygame.Surface((app.tile_w,app.tile_h)).convert_alpha()
-        self.overlay.fill((0,0,0,0))
-        s = pygame.Surface((self.rect.w,self.rect.h))
-        clrs = [(148,148,148),(108,108,108)]
-        for y in range(0,app.tile_h*2):
-            for x in range(0,app.tile_w*2):
-                s.fill(clrs[(x+y)%2],(
-                    self.rect.w*x/(app.tile_w*2),
-                    self.rect.h*y/(app.tile_h*2),
-                    self.rect.w/(app.tile_w*2)+1,
-                    self.rect.h/(app.tile_h*2)+2))
+        self.overlay = pygame.Surface((app.tile_w, app.tile_h)).convert_alpha()
+        self.overlay.fill((0, 0, 0, 0))
+        s = pygame.Surface((self.rect.w, self.rect.h))
+        clrs = [(148, 148, 148), (108, 108, 108)]
+        for y in range(0, app.tile_h * 2):
+            for x in range(0, app.tile_w * 2):
+                s.fill(
+                    clrs[(x + y) % 2],
+                    (
+                        self.rect.w * x / (app.tile_w * 2),
+                        self.rect.h * y / (app.tile_h * 2),
+                        self.rect.w / (app.tile_w * 2) + 1,
+                        self.rect.h / (app.tile_h * 2) + 2,
+                    ),
+                )
         self.bg = s
 
-        s = pygame.Surface((self.rect.w,self.rect.h)).convert_alpha()
-        s.fill((0,0,0,0))
-        for x in range(0,app.tile_w):
-            pygame.draw.line(s,(0,0,0),(self.rect.w*x/app.tile_w,0),(self.rect.w*x/app.tile_w,self.rect.h))
-        for y in range(0,app.tile_h):
-            pygame.draw.line(s,(0,0,0),(0,self.rect.h*y/app.tile_h),(self.rect.w,self.rect.h*y/app.tile_h))
+        s = pygame.Surface((self.rect.w, self.rect.h)).convert_alpha()
+        s.fill((0, 0, 0, 0))
+        for x in range(0, app.tile_w):
+            pygame.draw.line(
+                s,
+                (0, 0, 0),
+                (self.rect.w * x / app.tile_w, 0),
+                (self.rect.w * x / app.tile_w, self.rect.h),
+            )
+        for y in range(0, app.tile_h):
+            pygame.draw.line(
+                s,
+                (0, 0, 0),
+                (0, self.rect.h * y / app.tile_h),
+                (self.rect.w, self.rect.h * y / app.tile_h),
+            )
         self.grid = s
 
-        
-    def paint(self,s):
-        s.blit(self.bg,(0,0))
-        s.blit(pygame.transform.scale(app.tile,(self.rect.w,self.rect.h)),(0,0))
-        s.blit(pygame.transform.scale(self.overlay,(self.rect.w,self.rect.h)),(0,0))
-        #if app.mode == 'select':
-        s.blit(self.grid,(0,0))
+    def paint(self, s):
+        s.blit(self.bg, (0, 0))
+        s.blit(pygame.transform.scale(app.tile, (self.rect.w, self.rect.h)), (0, 0))
+        s.blit(pygame.transform.scale(self.overlay, (self.rect.w, self.rect.h)), (0, 0))
+        # if app.mode == 'select':
+        s.blit(self.grid, (0, 0))
         r = app.select
-        pygame.draw.rect(s,(255,255,255,128),Rect(r.x*self.rect.w/app.tile_w,r.y*self.rect.h/app.tile_h,r.w*self.rect.w/app.tile_w,r.h*self.rect.h/app.tile_h),4)
-        
-    def event(self,e):
-        if (e.type is MOUSEBUTTONDOWN and e.button == 3) or (e.type is MOUSEMOTION and e.buttons[2]==1 and self.container.myfocus == self):
+        pygame.draw.rect(
+            s,
+            (255, 255, 255, 128),
+            Rect(
+                r.x * self.rect.w / app.tile_w,
+                r.y * self.rect.h / app.tile_h,
+                r.w * self.rect.w / app.tile_w,
+                r.h * self.rect.h / app.tile_h,
+            ),
+            4,
+        )
+
+    def event(self, e):
+        if (e.type == MOUSEBUTTONDOWN and e.button == 3) or (
+            e.type == MOUSEMOTION
+            and e.buttons[2] == 1
+            and self.container.myfocus == self
+        ):
             self.picker_down(e)
-        if e.type is MOUSEBUTTONDOWN and e.button == 1:
-            a = '%s_down'%app.mode
-            if hasattr(self,a): getattr(self,a)(e)
-        if e.type is MOUSEMOTION and e.buttons[0] and self.container.myfocus == self:
-            a = '%s_drag'%app.mode
-            if hasattr(self,a): getattr(self,a)(e)
-        if e.type is MOUSEBUTTONUP and e.button == 1:
-            a = '%s_up'%app.mode
-            if hasattr(self,a): getattr(self,a)(e)
-            
-    #picker
-    def picker_down(self,e):
+        if e.type == MOUSEBUTTONDOWN and e.button == 1:
+            a = "%s_down" % app.mode
+            if hasattr(self, a):
+                getattr(self, a)(e)
+        if e.type == MOUSEMOTION and e.buttons[0] and self.container.myfocus == self:
+            a = "%s_drag" % app.mode
+            if hasattr(self, a):
+                getattr(self, a)(e)
+        if e.type == MOUSEBUTTONUP and e.button == 1:
+            a = "%s_up" % app.mode
+            if hasattr(self, a):
+                getattr(self, a)(e)
+
+    # picker
+    def picker_down(self, e):
         pos = self.getpos(e)
         c = app.tile.get_at(pos)
         app.color = c
-    
-    #fill
-    def fill_down(self,e):
+
+    # fill
+    def fill_down(self, e):
         app.archive()
         pos = self.getpos(e)
         bg = app.tile.get_at(pos)
-        if bg == app.color: return
-        self.fill_pixel(pos,bg)
+        if bg == app.color:
+            return
+        self.fill_pixel(pos, bg)
         self.repaint()
-        
-        
-    def fill_pixel(self,pos,bg): #worst algorithm
+
+    def fill_pixel(self, pos, bg):  # worst algorithm
         c = app.tile.get_at(pos)
-        if c != bg: return
-        app.tile.set_at(pos,app.color)
-        x,y = pos
-        if x > 0: self.fill_pixel((x-1,y),bg)
-        if x < app.tile_w-1: self.fill_pixel((x+1,y),bg)
-        if y > 0: self.fill_pixel((x,y-1),bg)
-        if y < app.tile_h-1: self.fill_pixel((x,y+1),bg)
-        
-    #pixel        
-    def pixel_down(self,e):
+        if c != bg:
+            return
+        app.tile.set_at(pos, app.color)
+        x, y = pos
+        if x > 0:
+            self.fill_pixel((x - 1, y), bg)
+        if x < app.tile_w - 1:
+            self.fill_pixel((x + 1, y), bg)
+        if y > 0:
+            self.fill_pixel((x, y - 1), bg)
+        if y < app.tile_h - 1:
+            self.fill_pixel((x, y + 1), bg)
+
+    # pixel
+    def pixel_down(self, e):
         app.archive()
         pos = self.getpos(e)
-        app.tile.set_at(pos,app.color)
+        app.tile.set_at(pos, app.color)
         self.repaint()
-        
-    #line
-    def line_down(self,e):
+
+    # line
+    def line_down(self, e):
         pos = self.getpos(e)
         self.pos = pos
-        
-    def line_drag(self,e):
-        self.overlay.fill((0,0,0,0))
+
+    def line_drag(self, e):
+        self.overlay.fill((0, 0, 0, 0))
         pos = self.getpos(e)
-        pygame.draw.line(self.overlay,app.color,self.pos,pos)
+        pygame.draw.line(self.overlay, app.color, self.pos, pos)
         self.repaint()
-    
-    def line_up(self,e):
+
+    def line_up(self, e):
         app.archive()
-        self.overlay.fill((0,0,0,0))
+        self.overlay.fill((0, 0, 0, 0))
         pos = self.getpos(e)
-        pygame.draw.line(app.tile,app.color,self.pos,pos)
+        pygame.draw.line(app.tile, app.color, self.pos, pos)
         self.repaint()
-        
-    #ellipse
-    def ellipse_down(self,e):
+
+    # ellipse
+    def ellipse_down(self, e):
         pos = self.getpos(e)
         self.pos = pos
-        
-    def ellipse_drag(self,e):
-        self.overlay.fill((0,0,0,0))
+
+    def ellipse_drag(self, e):
+        self.overlay.fill((0, 0, 0, 0))
         pos = self.getpos(e)
-        r = pygame.Rect(self.pos[0],self.pos[1],pos[0]-self.pos[0],pos[1]-self.pos[1])
+        r = pygame.Rect(
+            self.pos[0], self.pos[1], pos[0] - self.pos[0], pos[1] - self.pos[1]
+        )
         r.normalize()
         r.width += 1
         r.height += 1
-        r.width,r.height = max(2,r.width),max(2,r.height)
-        pygame.draw.ellipse(self.overlay,app.color,r,1)
+        r.width, r.height = max(2, r.width), max(2, r.height)
+        pygame.draw.ellipse(self.overlay, app.color, r, 1)
         self.repaint()
-    
-    def ellipse_up(self,e):
+
+    def ellipse_up(self, e):
         app.archive()
-        self.overlay.fill((0,0,0,0))
+        self.overlay.fill((0, 0, 0, 0))
         pos = self.getpos(e)
-        r = pygame.Rect(self.pos[0],self.pos[1],pos[0]-self.pos[0],pos[1]-self.pos[1])
+        r = pygame.Rect(
+            self.pos[0], self.pos[1], pos[0] - self.pos[0], pos[1] - self.pos[1]
+        )
         r.normalize()
         r.width += 1
         r.height += 1
-        r.width,r.height = max(2,r.width),max(2,r.height)
-        pygame.draw.ellipse(app.tile,app.color,r,1)
+        r.width, r.height = max(2, r.width), max(2, r.height)
+        pygame.draw.ellipse(app.tile, app.color, r, 1)
         self.repaint()
-        
-    #draw
-    def draw_down(self,e):
+
+    # draw
+    def draw_down(self, e):
         app.archive()
         pos = self.getpos(e)
-        app.tile.set_at(pos,app.color)
+        app.tile.set_at(pos, app.color)
         self.pos = pos
         self.repaint()
-        
-    def draw_drag(self,e):
+
+    def draw_drag(self, e):
         pos = self.getpos(e)
-        pygame.draw.line(app.tile,app.color,self.pos,pos)
+        pygame.draw.line(app.tile, app.color, self.pos, pos)
         self.pos = pos
         self.repaint()
-        
-    def getpos(self,e):
-        x,y = (e.pos[0])*app.tile_w/self.rect.w,(e.pos[1])*app.tile_h/self.rect.h
-        x = min(max(0,x),app.tile_w-1)
-        y = min(max(0,y),app.tile_h-1)
-        return x,y
-    
-    def getpos2(self,e):
-        w = self.rect.w/app.tile_w
-        h = self.rect.h/app.tile_h
-        x,y = (e.pos[0]+w/2)*app.tile_w/self.rect.w,(e.pos[1]+h/2)*app.tile_h/self.rect.h
-        x = min(max(0,x),app.tile_w)
-        y = min(max(0,y),app.tile_h)
-        return x,y
-    
-            
-    
-    #select
-    def select_down(self,e):
+
+    def getpos(self, e):
+        x, y = (e.pos[0]) * app.tile_w / self.rect.w, (
+            e.pos[1]
+        ) * app.tile_h / self.rect.h
+        x = min(max(0, x), app.tile_w - 1)
+        y = min(max(0, y), app.tile_h - 1)
+        return x, y
+
+    def getpos2(self, e):
+        w = self.rect.w / app.tile_w
+        h = self.rect.h / app.tile_h
+        x, y = (e.pos[0] + w / 2) * app.tile_w / self.rect.w, (
+            e.pos[1] + h / 2
+        ) * app.tile_h / self.rect.h
+        x = min(max(0, x), app.tile_w)
+        y = min(max(0, y), app.tile_h)
+        return x, y
+
+    # select
+    def select_down(self, e):
         pos = self.getpos2(e)
-        app.select = Rect(pos[0],pos[1],0,0)
+        app.select = Rect(pos[0], pos[1], 0, 0)
         self.repaint()
-        
-    def select_drag(self,e):
+
+    def select_drag(self, e):
         pos = self.getpos2(e)
-        #pos = (e.pos[0]+app.tile_w/2)/app.tile_w,(e.pos[1]+app.tile_h/2)/app.tile_h
-        
-        app.select = Rect(app.select.x,app.select.y,pos[0]-app.select.x,pos[1]-app.select.y)
-        app.select.w = max(0,app.select.w)
-        app.select.h = max(0,app.select.h)
-        
-        #print app.select
-        
+        # pos = (e.pos[0]+app.tile_w/2)/app.tile_w,(e.pos[1]+app.tile_h/2)/app.tile_h
+
+        app.select = Rect(
+            app.select.x, app.select.y, pos[0] - app.select.x, pos[1] - app.select.y
+        )
+        app.select.w = max(0, app.select.w)
+        app.select.h = max(0, app.select.h)
+
+        # print app.select
+
         self.repaint()
-        
 
-        
-    #eraser
-    def eraser_down(self,e):
+    # eraser
+    def eraser_down(self, e):
         app.archive()
         pos = self.getpos(e)
-        app.tile.set_at(pos,(0,0,0,0))
+        app.tile.set_at(pos, (0, 0, 0, 0))
         self.pos = pos
         self.repaint()
-        
-    def eraser_drag(self,e):
+
+    def eraser_drag(self, e):
         pos = self.getpos(e)
-        pygame.draw.line(app.tile,(0,0,0,0),self.pos,pos)
+        pygame.draw.line(app.tile, (0, 0, 0, 0), self.pos, pos)
         self.pos = pos
         self.repaint()
-        
+
 
 def cmd_quit(value):
-    if app.dirty: _dirty(_cmd_quit,value)
-    else: _cmd_quit(value)
+    if app.dirty:
+        _dirty(_cmd_quit, value)
+    else:
+        _cmd_quit(value)
+
 
 def _cmd_quit(value):
     app.top.quit()
 
+
 def cmd_all(value):
-    app.select = Rect(0,0,app.tile_w,app.tile_h)
+    app.select = Rect(0, 0, app.tile_w, app.tile_h)
     app.tdraw.repaint()
 
+
 def cmd_undo(value):
     app.undo()
-    
+
+
 def cmd_redo(value):
     pass
-    
+
+
 def cmd_copy(value):
-    #next version of pygame?
-    #app.clipboard = app.tile.subsurface(app.select).copy()
+    # next version of pygame?
+    # app.clipboard = app.tile.subsurface(app.select).copy()
     s = app.tile.subsurface(app.select)
-    app.clipboard = pygame.Surface((app.select.w,app.select.h),SWSURFACE,s)
-    app.clipboard.fill((0,0,0,0))
-    app.clipboard.blit(s,(0,0))
-    
+    app.clipboard = pygame.Surface((app.select.w, app.select.h), SWSURFACE, s)
+    app.clipboard.fill((0, 0, 0, 0))
+    app.clipboard.blit(s, (0, 0))
+
+
 def cmd_paste(value):
     if app.clipboard != None:
         app.archive()
-        app.tile.fill((0,0,0,0),(app.select.x,app.select.y,app.clipboard.get_width(),app.clipboard.get_height()))
-        app.tile.blit(app.clipboard,app.select)
+        app.tile.fill(
+            (0, 0, 0, 0),
+            (
+                app.select.x,
+                app.select.y,
+                app.clipboard.get_width(),
+                app.clipboard.get_height(),
+            ),
+        )
+        app.tile.blit(app.clipboard, app.select)
         app.tdraw.repaint()
 
+
 def cmd_cut(value):
     cmd_copy(value)
     cmd_delete(value)
-    
+
+
 def cmd_fullscreen(value):
     pygame.display.toggle_fullscreen()
-    
+
+
 def cmd_delete(value):
     app.archive()
-    app.tile.fill((0,0,0,0),app.select)
+    app.tile.fill((0, 0, 0, 0), app.select)
     app.tdraw.repaint()
 
-def cmd_fill(value):        
+
+def cmd_fill(value):
     app.archive()
-    app.tile.fill(app.color,app.select)
+    app.tile.fill(app.color, app.select)
     app.tdraw.repaint()
 
-#NOTE: this feature is a temporary HACK, to be replaced by
-#an ellipse tool in the future
+
+# NOTE: this feature is a temporary HACK, to be replaced by
+# an ellipse tool in the future
 def cmd_ellipse(value):
     app.archive()
-    pygame.draw.ellipse(app.tile,app.color,app.select,1)
+    pygame.draw.ellipse(app.tile, app.color, app.select, 1)
     app.tdraw.repaint()
-        
+
+
 def cmd_rotate(value):
     a = value
     app.archive()
-    s = pygame.transform.rotate(app.tile,a)
-    app.tile.fill((0,0,0,0))
-    app.tile.blit(s,(0,0))
+    s = pygame.transform.rotate(app.tile, a)
+    app.tile.fill((0, 0, 0, 0))
+    app.tile.blit(s, (0, 0))
     app.tdraw.repaint()
-    
+
+
 def cmd_flip(value):
-    fh,fv = value
+    fh, fv = value
     app.archive()
-    s = pygame.transform.flip(app.tile,fh,fv)
-    app.tile.fill((0,0,0,0))
-    app.tile.blit(s,(0,0))
+    s = pygame.transform.flip(app.tile, fh, fv)
+    app.tile.fill((0, 0, 0, 0))
+    app.tile.blit(s, (0, 0))
     app.tdraw.repaint()
 
+
 def cmd_tpick(value):
-    dx,dy = value
+    dx, dy = value
     off = app.tile.get_offset()
-    app.tpicker.pick((off[0]+dx*app.tile_w,off[1]+dy*app.tile_h))
-    
+    app.tpicker.pick((off[0] + dx * app.tile_w, off[1] + dy * app.tile_h))
+
+
 def cmd_mode(value):
     mode = value
     app.mode = mode
 
+
 def cmd_load(value):
-    if app.dirty: _dirty(_cmd_load,value)
-    else: _cmd_load(value)
+    if app.dirty:
+        _dirty(_cmd_load, value)
+    else:
+        _cmd_load(value)
 
 
 def _cmd_load(value):
     if app.fname == None:
-        ErrorDialog("Load failed","Image is untitled.").open()
+        ErrorDialog("Load failed", "Image is untitled.").open()
         return
     raise Restart()
-    
+
 
 def cmd_active_save(value):
-    """ we check if we want to save on screen focus...
-    """
+    """we check if we want to save on screen focus..."""
 
     if app.save_activeevent_switch.value:
         if app.dirty:
-            #"is dirty... saving"
+            # "is dirty... saving"
             return cmd_save(value)
     else:
         pass
-        #"is not dirty, not saving"
-
-
+        # "is not dirty, not saving"
 
 
 def cmd_save(value):
     if app.fname == None:
         return cmd_saveas(value)
     try:
         # make a temp file... save it there, and then move it in.
         # so as to avoid race with anything reading it.
 
         temp_file_name = "tmp_" + app.fname
-        print temp_file_name
-        if have_pil==True:
+        print(temp_file_name)
+        if have_pil == True:
             stim = pygame.image.tostring(app.tiles, "RGB")
-            im=Image.fromstring("RGB", (app.tiles.get_width(),app.tiles.get_height()), stim)
+            im = Image.fromstring(
+                "RGB", (app.tiles.get_width(), app.tiles.get_height()), stim
+            )
             im.save(temp_file_name)
         else:
-            pygame.image.save(app.tiles,temp_file_name)
-        #move temp file into place.
+            pygame.image.save(app.tiles, temp_file_name)
+        # move temp file into place.
         shutil.move(temp_file_name, app.fname)
-        cfg_to_ini(['tile_w','tile_h','palette'],app.fname)
+        cfg_to_ini(["tile_w", "tile_h", "palette"], app.fname)
         ini_save()
         app.dirty = 0
-    except Exception, v:
-        ErrorDialog("Save failed.",v).open()
+    except Exception as v:
+        ErrorDialog("Save failed.", v).open()
         return
-    
+
+
 def cmd_saveas(value):
     dialog = SaveAsDialog()
-    
+
     def onchange(value):
         value.close()
         vv = value.value
-        fname = vv['fname'].value
+        fname = vv["fname"].value
         if len(fname) == 0:
-            ErrorDialog("Save As failed.","File Name too short!").open()
+            ErrorDialog("Save As failed.", "File Name too short!").open()
             return
         global cfg
-        app.fname = cfg['fname'] = fname
+        app.fname = cfg["fname"] = fname
         return cmd_save(None)
-        
-    dialog.connect(gui.CHANGE,onchange,dialog)
+
+    dialog.connect(gui.CHANGE, onchange, dialog)
     dialog.open()
 
+
 def cmd_open(value):
-    if app.dirty: _dirty(_cmd_open,value)
-    else: _cmd_open(value)
+    if app.dirty:
+        _dirty(_cmd_open, value)
+    else:
+        _cmd_open(value)
+
 
-    
 def _cmd_open(value):
     dialog = OpenDialog()
-    
+
     def onchange(value):
         value.close()
         vv = value.value
         ok = 0
-        
-        try:        
-            fname,tile_w,tile_h = vv['fname'].value,int(vv['tile_w'].value),int(vv['tile_h'].value)
+
+        try:
+            fname, tile_w, tile_h = (
+                vv["fname"].value,
+                int(vv["tile_w"].value),
+                int(vv["tile_h"].value),
+            )
             global cfg
-            cfg['fname'] = fname
-            cfg['tile_w'] = tile_w
-            cfg['tile_h'] = tile_h
+            cfg["fname"] = fname
+            cfg["tile_w"] = tile_w
+            cfg["tile_h"] = tile_h
             ok = 1
-        except Exception,v:
-            ErrorDialog("Open failed.",v).open()
-            
-        if ok: raise Restart()
+        except Exception as v:
+            ErrorDialog("Open failed.", v).open()
 
-    
-    dialog.connect(gui.CHANGE,onchange,dialog)
+        if ok:
+            raise Restart()
+
+    dialog.connect(gui.CHANGE, onchange, dialog)
     dialog.open()
 
 
 class Restart(Exception):
     pass
-def _dirty(fnc,v):
+
+
+def _dirty(fnc, v):
     dialog = DirtyDialog()
+
     def onchange(value):
         value.close()
         return fnc(v)
-    dialog.connect(gui.CHANGE,onchange,dialog)
+
+    dialog.connect(gui.CHANGE, onchange, dialog)
     dialog.open()
-    
+
+
 def cmd_new(value):
-    if app.dirty: _dirty(_cmd_new,value)
-    else: _cmd_new(value)
-    
-        
+    if app.dirty:
+        _dirty(_cmd_new, value)
+    else:
+        _cmd_new(value)
+
+
 def _cmd_new(value):
     dialog = NewDialog()
-    
+
     def onchange(value):
         value.close()
         vv = value.value
         ok = 0
-        try:        
-            width,height,tile_w,tile_h = int(vv['width'].value),int(vv['height'].value),int(vv['tile_w'].value),int(vv['tile_h'].value)
+        try:
+            width, height, tile_w, tile_h = (
+                int(vv["width"].value),
+                int(vv["height"].value),
+                int(vv["tile_w"].value),
+                int(vv["tile_h"].value),
+            )
             global cfg
-            cfg['fname'] = None
-            cfg['width'] = width
-            cfg['height'] = height
-            cfg['tile_w'] = tile_w
-            cfg['tile_h'] = tile_h
+            cfg["fname"] = None
+            cfg["width"] = width
+            cfg["height"] = height
+            cfg["tile_w"] = tile_w
+            cfg["tile_h"] = tile_h
             ok = 1
-        except Exception, v:
-            ErrorDialog("New failed.",v).open()
+        except Exception as v:
+            ErrorDialog("New failed.", v).open()
         if ok:
             raise Restart()
-    
-    dialog.connect(gui.CHANGE,onchange,dialog)
+
+    dialog.connect(gui.CHANGE, onchange, dialog)
     dialog.open()
 
 
 menus = [
-    ('File/New',cmd_new,None),
-    ('File/Open',cmd_open,None),
-    ('File/Save',cmd_save,None),
-    ('File/Save As',cmd_saveas,None),
-    ('File/Reload',cmd_load,None),
-    ('File/Quit',cmd_quit,None),
-
-    ('Edit/Undo',cmd_undo,None),
-    #('Edit/Redo',None,None,None),
-    ('Edit/Cut',cmd_cut,None),
-    ('Edit/Copy',cmd_copy,None),
-    ('Edit/Paste',cmd_paste,None),
-    ('Edit/Delete',cmd_delete,None),
-    ('Edit/Fill',cmd_fill,None),
-        ('Edit/Ellipse',cmd_ellipse,None),
-    ('Edit/Select All',cmd_all,None),
-    
-    ('Transform/Rotate 90 CCW',cmd_rotate,90),
-    ('Transform/Rotate 90 CW',cmd_rotate,-90),
-    ('Transform/Flip Horizontal',cmd_flip,(1,0)),
-    ('Transform/Flip Vertical',cmd_flip,(0,1)),
-    ]
+    ("File/New", cmd_new, None),
+    ("File/Open", cmd_open, None),
+    ("File/Save", cmd_save, None),
+    ("File/Save As", cmd_saveas, None),
+    ("File/Reload", cmd_load, None),
+    ("File/Quit", cmd_quit, None),
+    ("Edit/Undo", cmd_undo, None),
+    # ('Edit/Redo',None,None,None),
+    ("Edit/Cut", cmd_cut, None),
+    ("Edit/Copy", cmd_copy, None),
+    ("Edit/Paste", cmd_paste, None),
+    ("Edit/Delete", cmd_delete, None),
+    ("Edit/Fill", cmd_fill, None),
+    ("Edit/Ellipse", cmd_ellipse, None),
+    ("Edit/Select All", cmd_all, None),
+    ("Transform/Rotate 90 CCW", cmd_rotate, 90),
+    ("Transform/Rotate 90 CW", cmd_rotate, -90),
+    ("Transform/Flip Horizontal", cmd_flip, (1, 0)),
+    ("Transform/Flip Vertical", cmd_flip, (0, 1)),
+]
 
 keys = [
-    (K_s,cmd_save,None),
-    (K_d,cmd_load,None),
+    (K_s, cmd_save, None),
+    (K_d, cmd_load, None),
+    (K_a, cmd_all, None),
+    (K_z, cmd_undo, None),
+    # ('Edit/Redo',None,None,None),
+    (K_c, cmd_copy, None),
+    (K_v, cmd_paste, None),
+    (K_x, cmd_cut, None),
+    (K_DELETE, cmd_delete, None),
+    (K_f, cmd_fill, None),
+    (K_e, cmd_ellipse, None),
+    (K_LEFTBRACKET, cmd_rotate, 90),
+    (K_RIGHTBRACKET, cmd_rotate, -90),
+    (K_COMMA, cmd_flip, (1, 0)),
+    (K_PERIOD, cmd_flip, (0, 1)),
+    (K_UP, cmd_tpick, (0, -1)),
+    (K_DOWN, cmd_tpick, (0, 1)),
+    (K_LEFT, cmd_tpick, (-1, 0)),
+    (K_RIGHT, cmd_tpick, (1, 0)),
+    (K_F10, cmd_fullscreen, None),
+]
 
-    (K_a,cmd_all,None),
-    (K_z,cmd_undo,None),
-    #('Edit/Redo',None,None,None),
-    (K_c,cmd_copy,None),
-    (K_v,cmd_paste,None),
-    (K_x,cmd_cut,None),
-    (K_DELETE,cmd_delete,None),
-    (K_f,cmd_fill,None),
-        (K_e,cmd_ellipse,None),
-    
-    (K_LEFTBRACKET,cmd_rotate,90),
-    (K_RIGHTBRACKET,cmd_rotate,-90),
-    (K_COMMA,cmd_flip,(1,0)),
-    (K_PERIOD,cmd_flip,(0,1)),
-    
-    (K_UP,cmd_tpick,(0,-1)),
-    (K_DOWN,cmd_tpick,(0,1)),
-    (K_LEFT,cmd_tpick,(-1,0)),
-    (K_RIGHT,cmd_tpick,(1,0)),
-    
-    (K_F10,cmd_fullscreen,None),
-    ]
-    
 
 tools = [
-    ('draw','draw'),
-    ('pixel','pixel'),
-    ('line','line'),
-    #('ellipse','ellipse'),
-    ('fill','fill'),
-    ('select','select'),
-    ('eraser','eraser'),
-    ]
+    ("draw", "draw"),
+    ("pixel", "pixel"),
+    ("line", "line"),
+    # ('ellipse','ellipse'),
+    ("fill", "fill"),
+    ("select", "select"),
+    ("eraser", "eraser"),
+]
 
 
 def init_ini():
     ini.read([ini_fname])
 
+
 def ini_save():
-    f = open(ini_fname,"wb")
+    f = open(ini_fname, "wb")
     ini.write(f)
     f.close()
-    
+
 
 def init_opts():
     usage = "%prog [tiles.tga] [tile_w] [tile_h]"
 
     parser = OptionParser(usage)
-    parser.add_option("--sw",dest="screen_w",help="screen width (app)",type='int')
-    parser.add_option("--sh",dest="screen_h",help="screen height (app)",type='int')
-    parser.add_option("--tw",dest="tile_w",help="tile width (image)",type='int')
-    parser.add_option("--th",dest="tile_h",help="tile height (image)",type='int')
-    parser.add_option("--width",dest="width",help="new width (image)",type='int')
-    parser.add_option("--height",dest="height",help="new height (image)",type='int')
-    parser.add_option("-p","--pal",dest="palette",help="filename of palette (image)")
-    parser.add_option("-d","--defaults",dest="defaults",help="set default settings (image)",action="store_true")
-    #parser.add_option("-a","--app",dest="app",help="set application level defaults",action="store_true")
-    
-    (opts,args) = parser.parse_args()
-    
-    if len(args) > 3: parser.error("incorrect number of arguments")
-    
-    #parse arguments
+    parser.add_option("--sw", dest="screen_w", help="screen width (app)", type="int")
+    parser.add_option("--sh", dest="screen_h", help="screen height (app)", type="int")
+    parser.add_option("--tw", dest="tile_w", help="tile width (image)", type="int")
+    parser.add_option("--th", dest="tile_h", help="tile height (image)", type="int")
+    parser.add_option("--width", dest="width", help="new width (image)", type="int")
+    parser.add_option("--height", dest="height", help="new height (image)", type="int")
+    parser.add_option("-p", "--pal", dest="palette", help="filename of palette (image)")
+    parser.add_option(
+        "-d",
+        "--defaults",
+        dest="defaults",
+        help="set default settings (image)",
+        action="store_true",
+    )
+    # parser.add_option("-a","--app",dest="app",help="set application level defaults",action="store_true")
+
+    (opts, args) = parser.parse_args()
+
+    if len(args) > 3:
+        parser.error("incorrect number of arguments")
+
+    # parse arguments
     if len(args) == 0:
         opts.fname = "None"
     elif len(args) == 1:
         opts.fname = args[0]
     elif len(args) == 2:
         opts.fname = "None"
-        try: opts.tile_w,opts.tile_h = int(args[0]),int(args[1])
-        except: parser.error("tile width and height must be integers")
-        if opts.tile_w < 1 or opts.tile_h < 1: parser.error("width and height must be greater than 0")
+        try:
+            opts.tile_w, opts.tile_h = int(args[0]), int(args[1])
+        except:
+            parser.error("tile width and height must be integers")
+        if opts.tile_w < 1 or opts.tile_h < 1:
+            parser.error("width and height must be greater than 0")
     else:
-        try: opts.fname,opts.tile_w,opts.tile_h = args[0],int(args[1]),int(args[2])
-        except: parser.error("tile width and height must be integers")
-        if opts.tile_w < 1 or opts.tile_h < 1: parser.error("width and height must be greater than 0")
-        
+        try:
+            opts.fname, opts.tile_w, opts.tile_h = args[0], int(args[1]), int(args[2])
+        except:
+            parser.error("tile width and height must be integers")
+        if opts.tile_w < 1 or opts.tile_h < 1:
+            parser.error("width and height must be greater than 0")
+
     fname = opts.fname
-    
-    #create all sections
-    for k in [fname,"None","app"]:
+
+    # create all sections
+    for k in [fname, "None", "app"]:
         if not ini.has_section(k):
             ini.add_section(k)
-    
-    #set app level defaults
-    for k,v in [('screen_w',800),('screen_h',600)]:
-        if not ini.has_option('app',k):
-            ini.set('app',k,str(v))
-            
-    #set app level values
-    for k in ['screen_w','screen_h']:
-        if hasattr(opts,k):
-            v = getattr(opts,k)
-            if v != None: ini.set('app',k,str(v))
-            
-    #set default defaults
-    for k,v in [('width',256),('height',256),('tile_w',32),('tile_h',32),('palette','palette.tga')]:
-        if not ini.has_option('None',k):
-            ini.set('None',k,str(v))
-    
-    #name of keys for normal stuff
-    file_ks = ['width','height','tile_w','tile_h','palette']
-        
-    #set default values
+
+    # set app level defaults
+    for k, v in [("screen_w", 800), ("screen_h", 600)]:
+        if not ini.has_option("app", k):
+            ini.set("app", k, str(v))
+
+    # set app level values
+    for k in ["screen_w", "screen_h"]:
+        if hasattr(opts, k):
+            v = getattr(opts, k)
+            if v != None:
+                ini.set("app", k, str(v))
+
+    # set default defaults
+    for k, v in [
+        ("width", 256),
+        ("height", 256),
+        ("tile_w", 32),
+        ("tile_h", 32),
+        ("palette", "palette.tga"),
+    ]:
+        if not ini.has_option("None", k):
+            ini.set("None", k, str(v))
+
+    # name of keys for normal stuff
+    file_ks = ["width", "height", "tile_w", "tile_h", "palette"]
+
+    # set default values
     if opts.defaults:
         for k in file_ks:
-            if hasattr(opts,k):
-                v = getattr(opts,k)
-                if v != None: ini.set('None',k,str(v))
-    
-    #set fname values
+            if hasattr(opts, k):
+                v = getattr(opts, k)
+                if v != None:
+                    ini.set("None", k, str(v))
+
+    # set fname values
     for k in file_ks:
-        if hasattr(opts,k):
-            v = getattr(opts,k)
-            if v != None: ini.set(fname,k,str(v))
-    
-    #save the ini
+        if hasattr(opts, k):
+            v = getattr(opts, k)
+            if v != None:
+                ini.set(fname, k, str(v))
+
+    # save the ini
     ini_save()
-            
-    #convert ini to cfg stuff...
-    ini_to_cfg(['app','None',fname])
-    if fname == 'None': fname = None
-    cfg['fname'] = fname
-    
-            
+
+    # convert ini to cfg stuff...
+    ini_to_cfg(["app", "None", fname])
+    if fname == "None":
+        fname = None
+    cfg["fname"] = fname
+
+
 def ini_to_cfg(sections):
     global cfg
-    ik = ['screen_w','screen_h','tile_w','tile_h','width','height']
+    ik = ["screen_w", "screen_h", "tile_w", "tile_h", "width", "height"]
     for s in sections:
-        for k,v in ini.items(s):
-            if k in ik: v = int(v)
+        for k, v in ini.items(s):
+            if k in ik:
+                v = int(v)
             cfg[k] = v
+
+
 def ini_to_dict(section):
     cfg = {}
-    ik = ['screen_w','screen_h','tile_w','tile_h','width','height']
+    ik = ["screen_w", "screen_h", "tile_w", "tile_h", "width", "height"]
     for s in [section]:
-        for k,v in ini.items(s):
-            if k in ik: v = int(v)
+        for k, v in ini.items(s):
+            if k in ik:
+                v = int(v)
             cfg[k] = v
     return cfg
 
-def cfg_to_ini(ks,section):
-    if not ini.has_section(section): ini.add_section(section)
+
+def cfg_to_ini(ks, section):
+    if not ini.has_section(section):
+        ini.add_section(section)
     for k in ks:
         v = cfg[k]
-        ini.set(section,k,str(v))
-        
-        
+        ini.set(section, k, str(v))
+
+
 def init_gui():
-    #themes = cfg['theme'].split(",")
-    #gui.theme.load(themes)
-    #gui.theme.load(['default','tools'])
+    # themes = cfg['theme'].split(",")
+    # gui.theme.load(themes)
+    # gui.theme.load(['default','tools'])
     global top
-    top = gui.Desktop(theme=gui.Theme(['default','tools']))
+    top = gui.Desktop(theme=gui.Theme(["default", "tools"]))
 
-    #top = gui.Desktop()
-    #top.theme.load(['default','tools'])
+    # top = gui.Desktop()
+    # top.theme.load(['default','tools'])
+
+    # pass
 
 
-    #pass
-    
 def init_app():
     global app
     app = _app()
 
     #
     colors_height = 64
     ss = 8
-        
-    #--- top
-    x,y,h = 0,0,0
-        
-    #menus
+
+    # --- top
+    x, y, h = 0, 0, 0
+
+    # menus
     e = gui.Menus(menus)
-    e.rect.w,e.rect.h = e.resize()
-    app.add(e,x,y)
-    x,h = x+e.rect.w,max(h,e.rect.h)
+    e.rect.w, e.rect.h = e.resize()
+    app.add(e, x, y)
+    x, h = x + e.rect.w, max(h, e.rect.h)
     menus_height = e.rect.h
-    
-    #--- row
-    x,y,h = 0,y+h,0
-    
-    #--- vspace
+
+    # --- row
+    x, y, h = 0, y + h, 0
+
+    # --- vspace
     y += ss
-    
-    #--- hspace
+
+    # --- hspace
     x += ss
-    
-    #tools
-    e = gui.Toolbox(tools,1,0,value='draw') #,"icons48")
-    e.rect.w,e.rect.h = e.resize()
+
+    # tools
+    e = gui.Toolbox(tools, 1, 0, value="draw")  # ,"icons48")
+    e.rect.w, e.rect.h = e.resize()
+
     def _set_mode(value):
         cmd_mode(value.value)
-    e.connect(gui.CHANGE,_set_mode,e)
-    app.add(e,x,y)
 
-    
-    #--- vspace
-    y += ss
+    e.connect(gui.CHANGE, _set_mode, e)
+    app.add(e, x, y)
 
+    # --- vspace
+    y += ss
 
-    #--- switchbox for saving.
-    sx, sy = x,y+(max(h,e.rect.h))
+    # --- switchbox for saving.
+    sx, sy = x, y + (max(h, e.rect.h))
 
     savelabel = gui.Label("Save on")
-    app.add(savelabel, sx,sy)
+    app.add(savelabel, sx, sy)
     savelabel2 = gui.Label("focus:")
-    app.add(savelabel2, sx,sy+(ss*2))
+    app.add(savelabel2, sx, sy + (ss * 2))
 
-    #--- vspace
-    y += (ss *5)
-    sy += (ss *5)
+    # --- vspace
+    y += ss * 5
+    sy += ss * 5
 
     save_activeevent_switch = gui.Switch(False)
-    app.add(save_activeevent_switch, sx,sy)
+    app.add(save_activeevent_switch, sx, sy)
     app.save_activeevent_switch = save_activeevent_switch
 
-    x,h = x+e.rect.w,max(h,e.rect.h)
+    x, h = x + e.rect.w, max(h, e.rect.h)
     toolbox_width = e.rect.w
 
-    #--- hspace
+    # --- hspace
     x += ss
-    y -= ss*6 #undo what was done above to the y val
-        
-    #tdraw
-    #tdraw-calcs
-    dw = app.screen_w - (toolbox_width+app.tiles.get_width()+ss*4)
-    dh = app.screen_h - (menus_height+colors_height+ss*2)
-    if dw/float(app.tile_w) > dh/float(app.tile_h): dw = dh/float(app.tile_h)*app.tile_w
-    else: dh = dw/float(app.tile_w)*app.tile_h
-    e = app.tdraw = tdraw(dw,dh)
-    app.add(e,x,y)
-    x,h = x+e.rect.w,max(h,e.rect.h)
-    
-    #--- hspace
+    y -= ss * 6  # undo what was done above to the y val
+
+    # tdraw
+    # tdraw-calcs
+    dw = app.screen_w - (toolbox_width + app.tiles.get_width() + ss * 4)
+    dh = app.screen_h - (menus_height + colors_height + ss * 2)
+    if dw / float(app.tile_w) > dh / float(app.tile_h):
+        dw = dh / float(app.tile_h) * app.tile_w
+    else:
+        dh = dw / float(app.tile_w) * app.tile_h
+    e = app.tdraw = tdraw(dw, dh)
+    app.add(e, x, y)
+    x, h = x + e.rect.w, max(h, e.rect.h)
+
+    # --- hspace
     x += ss
-    
-    #tpicker
+
+    # tpicker
     e = app.tpicker = tpicker()
-    e.rect.w,e.rect.h = e.resize()
-    #--- right
-    x = app.screen_w-e.rect.w-ss
-    app.add(e,x,y)
-    h = max(h,e.rect.h)
+    e.rect.w, e.rect.h = e.resize()
+    # --- right
+    x = app.screen_w - e.rect.w - ss
+    app.add(e, x, y)
+    h = max(h, e.rect.h)
 
-    #tpreview
-    y = y+e.rect.h
+    # tpreview
+    y = y + e.rect.h
     e = app.tpreview = tpreview()
-    e.rect.w,e.rect.h = e.resize()
-    app.add(e,x,y)
-    
-    #--- bottom
-    x,y,h = 0,app.screen_h - colors_height,0
-    
-    #cpreview
+    e.rect.w, e.rect.h = e.resize()
+    app.add(e, x, y)
+
+    # --- bottom
+    x, y, h = 0, app.screen_h - colors_height, 0
+
+    # cpreview
     colors_width = toolbox_width + ss * 2
-    e = app.cpreview = cpreview(colors_width,colors_height)
-    e.rect.w,e.rect.h = e.resize()
-    app.add(e,x,y)
-    x,h = x+e.rect.w,max(h,e.rect.h)
-    
-    #cpicker
-    if os.path.isfile(cfg['palette']):
-        pal = pygame.image.load(cfg['palette'])
+    e = app.cpreview = cpreview(colors_width, colors_height)
+    e.rect.w, e.rect.h = e.resize()
+    app.add(e, x, y)
+    x, h = x + e.rect.w, max(h, e.rect.h)
+
+    # cpicker
+    if os.path.isfile(cfg["palette"]):
+        pal = pygame.image.load(cfg["palette"])
     else:
-        #default to EGA / NES palette
-        
-        pw,ph = 16,6
-        pdata = [(0, 0, 0, 255), (0, 0, 170, 255), (0, 170, 0, 255), (0, 170, 170, 255), (170, 0, 0, 255), (170, 0, 170, 255), (170, 85, 0, 255), (170, 170, 170, 255), (85, 85, 85, 255), (85, 85, 255, 255), (85, 255, 85, 255), (85, 255, 255, 255), (255, 85, 85, 255), (255, 85, 255, 255), (255, 255, 85, 255), (255, 255, 255, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255), (255, 255, 255, 255), (173, 243, 255, 255), (223, 214, 255, 255), (255, 190, 255, 255), (255, 176, 255, 255), (255, 177, 237, 255), (255, 191, 185, 255), (255, 217, 145, 255), (237, 246, 128, 255), (185, 255, 138, 255), (145, 255, 173, 255), (128, 255, 223, 255), (138, 255, 255, 255), (197, 197, 197, 255), (0, 0, 0, 255), (0, 0, 0, 255), (255, 255, 255, 255), (129, 200, 255, 255), (179, 171, 255, 255), (231, 146, 255, 255), (255, 132, 244, 255), (255, 133, 194, 255), (255, 148, 141, 255), (244, 173, 101, 255), (194, 202, 84, 255), (141, 227, 94, 255), (101, 240, 129, 255), (84, 240, 179, 255), (94, 225, 231, 255), (120, 120, 120, 255), (0, 0, 0, 255), (0, 0, 0, 255), (192, 192, 192, 255), (57, 128, 200, 255), (108, 99, 217, 255), (160, 74, 207, 255), (200, 61, 172, 255), (217, 61, 122, 255), (207, 76, 70, 255), (172, 102, 30, 255), (122, 130, 13, 255), (70, 155, 23, 255), (30, 169, 57, 255), (13, 168, 108, 255), (23, 153, 160, 255), (61, 61, 61, 255), (0, 0, 0, 255), (0, 0, 0, 255), (128, 128, 128, 255), (16, 87, 159, 255), (67, 58, 176, 255), (119, 34, 166, 255), (159, 20, 131, 255), (176, 20, 81, 255), (166, 35, 29, 255), (131, 61, 0, 255), (81, 89, 0, 255), (29, 114, 0, 255), (0, 128, 16, 255), (0, 127, 67, 255), (0, 112, 119, 255), (0, 0, 0, 255), (0, 0, 0, 255), (0, 0, 0, 255)]
+        # default to EGA / NES palette
+
+        pw, ph = 16, 6
+        pdata = [
+            (0, 0, 0, 255),
+            (0, 0, 170, 255),
+            (0, 170, 0, 255),
+            (0, 170, 170, 255),
+            (170, 0, 0, 255),
+            (170, 0, 170, 255),
+            (170, 85, 0, 255),
+            (170, 170, 170, 255),
+            (85, 85, 85, 255),
+            (85, 85, 255, 255),
+            (85, 255, 85, 255),
+            (85, 255, 255, 255),
+            (255, 85, 85, 255),
+            (255, 85, 255, 255),
+            (255, 255, 85, 255),
+            (255, 255, 255, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (255, 255, 255, 255),
+            (173, 243, 255, 255),
+            (223, 214, 255, 255),
+            (255, 190, 255, 255),
+            (255, 176, 255, 255),
+            (255, 177, 237, 255),
+            (255, 191, 185, 255),
+            (255, 217, 145, 255),
+            (237, 246, 128, 255),
+            (185, 255, 138, 255),
+            (145, 255, 173, 255),
+            (128, 255, 223, 255),
+            (138, 255, 255, 255),
+            (197, 197, 197, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (255, 255, 255, 255),
+            (129, 200, 255, 255),
+            (179, 171, 255, 255),
+            (231, 146, 255, 255),
+            (255, 132, 244, 255),
+            (255, 133, 194, 255),
+            (255, 148, 141, 255),
+            (244, 173, 101, 255),
+            (194, 202, 84, 255),
+            (141, 227, 94, 255),
+            (101, 240, 129, 255),
+            (84, 240, 179, 255),
+            (94, 225, 231, 255),
+            (120, 120, 120, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (192, 192, 192, 255),
+            (57, 128, 200, 255),
+            (108, 99, 217, 255),
+            (160, 74, 207, 255),
+            (200, 61, 172, 255),
+            (217, 61, 122, 255),
+            (207, 76, 70, 255),
+            (172, 102, 30, 255),
+            (122, 130, 13, 255),
+            (70, 155, 23, 255),
+            (30, 169, 57, 255),
+            (13, 168, 108, 255),
+            (23, 153, 160, 255),
+            (61, 61, 61, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (128, 128, 128, 255),
+            (16, 87, 159, 255),
+            (67, 58, 176, 255),
+            (119, 34, 166, 255),
+            (159, 20, 131, 255),
+            (176, 20, 81, 255),
+            (166, 35, 29, 255),
+            (131, 61, 0, 255),
+            (81, 89, 0, 255),
+            (29, 114, 0, 255),
+            (0, 128, 16, 255),
+            (0, 127, 67, 255),
+            (0, 112, 119, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+            (0, 0, 0, 255),
+        ]
+
+        pal = pygame.Surface((pw, ph), SWSURFACE, 32)
+        n = 0
+        for py in range(0, ph):
+            for px in range(0, pw):
+                pal.set_at((px, py), pdata[n])
+                n += 1
+
+    e = app.cpicker = cpicker(app.screen_w - colors_width, colors_height, pal)
+    e.rect.w, e.rect.h = e.resize()
+    app.add(e, x, y)
+    x, h = x + e.rect.w, max(h, e.rect.h)
+
+    pygame.key.set_repeat(500, 30)
+
+    app.screen.fill((255, 255, 255, 255))
+
 
-        pal = pygame.Surface((pw,ph),SWSURFACE,32)
-        n=0
-        for py in range(0,ph):
-            for px in range(0,pw):
-                pal.set_at((px,py),pdata[n])
-                n+=1
-        
-        
-    e = app.cpicker = cpicker(app.screen_w-colors_width,colors_height,pal)
-    e.rect.w,e.rect.h = e.resize()
-    app.add(e,x,y)
-    x,h = x+e.rect.w,max(h,e.rect.h)
-    
-    pygame.key.set_repeat(500,30)
-    
-    app.screen.fill((255,255,255,255))
-    
 class NewDialog(gui.Dialog):
-    def __init__(self,**params):
+    def __init__(self, **params):
         title = gui.Label("New...")
-        
-        doc = html.HTML(globals={'gui':gui,'dialog':self},data="""<form id='form'><table>
+
+        doc = html.HTML(
+            globals={"gui": gui, "dialog": self},
+            data="""<form id='form'><table>
         <tr>
         <td align=center>Image Size
         <td align=center>Tile Size
 
         <tr><td colspan='1' align='center' style='padding-right:8px;'><table>
         <tr><td align=right>Width: <td><input type='text' size='4' value='%(width)s' name='width'>
         <tr><td align=right>Height: <td><input type='text' size='4' value='%(height)s' name='height'>
@@ -1000,124 +1250,147 @@
         
         <tr><td colspan=2>Palette: <input type='text' size=20 name='palette' value='%(palette)s'>
         
         <tr><td>&nbsp;
         
         <tr><td colspan=2><input type='button' value='Okay' onclick='dialog.send(gui.CHANGE)'> <input type='button' value='Cancel' onclick='dialog.close()'>
         
-        </table>"""%ini_to_dict('None'))
-        gui.Dialog.__init__(self,title,doc)
-        
-        self.value = doc['form']
+        </table>"""
+            % ini_to_dict("None"),
+        )
+        gui.Dialog.__init__(self, title, doc)
+
+        self.value = doc["form"]
+
 
 class SaveAsDialog(gui.Dialog):
-    def __init__(self,**params):
+    def __init__(self, **params):
         title = gui.Label("Save As...")
-        
-        doc = html.HTML(globals={'gui':gui,'dialog':self},data="""
+
+        doc = html.HTML(
+            globals={"gui": gui, "dialog": self},
+            data="""
         <form id='form'>
         
         <table>
         
         <tr><td colspan=2>File Name: <input type='file' size=20 name='fname' value=''>
         
         <tr><td>&nbsp;
         
         <tr><td colspan=2><input type='button' value='Okay' onclick='dialog.send(gui.CHANGE)'> <input type='button' value='Cancel' onclick='dialog.close()'>
         
-        </table>""")
-        gui.Dialog.__init__(self,title,doc)
-        
-        self.value = doc['form']
+        </table>""",
+        )
+        gui.Dialog.__init__(self, title, doc)
+
+        self.value = doc["form"]
+
 
 class OpenDialog(gui.Dialog):
-    def __init__(self,**params):
+    def __init__(self, **params):
         title = gui.Label("Open...")
-        
-        def load_vals(fname,form):
-            if not ini.has_section(fname): return
-            
-            for k,v in ini.items(fname):
+
+        def load_vals(fname, form):
+            if not ini.has_section(fname):
+                return
+
+            for k, v in ini.items(fname):
                 if k in form:
                     form[k].value = v
-        doc = html.HTML(globals={'load_vals':load_vals,'ini':ini,'gui':gui,'dialog':self},data="""<form id='form'><table>
+
+        doc = html.HTML(
+            globals={"load_vals": load_vals, "ini": ini, "gui": gui, "dialog": self},
+            data="""<form id='form'><table>
         
         <tr><td align=right>File Name:&nbsp;<td  align=left><input type='file' size=20 name='fname' value='' onchange='load_vals(self.value,form)'>
         <tr><td align=right>Tile Width:&nbsp;<td align=left><input type='text' size='4' value='%(tile_w)s' name='tile_w'>
         <tr><td align=right>Tile Height:&nbsp;<td align=left><input type='text' size='4' value='%(tile_h)s' name='tile_h'>
         
         <tr><td align=right>Palette:&nbsp;<td align=left><input type='text' size=20 name='palette' value='%(palette)s'>
         
         <tr><td>&nbsp;
         
         <tr><td colspan=2><input type='button' value='Okay' onclick='dialog.send(gui.CHANGE)'> <input type='button' value='Cancel' onclick='dialog.close()'>
         
-        </table>"""%ini_to_dict('None'))
-        gui.Dialog.__init__(self,title,doc)
-        
-        self.value = doc['form']
+        </table>"""
+            % ini_to_dict("None"),
+        )
+        gui.Dialog.__init__(self, title, doc)
+
+        self.value = doc["form"]
+
 
 class ErrorDialog(gui.Dialog):
-    def __init__(self,tt,data,**params):
-        title = gui.Label("Error: "+tt)
+    def __init__(self, tt, data, **params):
+        title = gui.Label("Error: " + tt)
         data = str(data)
-        
-        doc = html.HTML(globals={'gui':gui,'dialog':self},data="""
+
+        doc = html.HTML(
+            globals={"gui": gui, "dialog": self},
+            data="""
         <form id='form'>
         
         <table>
         <tr><td><h1>&lt;!&gt;&nbsp;</h1>
-        <td>"""+data+"""
+        <td>"""
+            + data
+            + """
         <tr><td>&nbsp;
         <tr><td colspan=2><input type='button' value='Okay' onclick='dialog.send(gui.CHANGE);dialog.close()'>
-        </table>""")
-        gui.Dialog.__init__(self,title,doc)
-        
-        self.value = doc['form']
+        </table>""",
+        )
+        gui.Dialog.__init__(self, title, doc)
+
+        self.value = doc["form"]
+
 
 class DirtyDialog(gui.Dialog):
-    def __init__(self,**params):
+    def __init__(self, **params):
         title = gui.Label("File not yet saved...")
         data = "Your file is not yet saved.<br>Are you sure you want to continue?"
-        
-        doc = html.HTML(globals={'gui':gui,'dialog':self},data="""
+
+        doc = html.HTML(
+            globals={"gui": gui, "dialog": self},
+            data="""
         <form id='form'>
         
         <table>
         <tr><td><h1>&lt;!&gt;&nbsp;</h1>
-        <td>"""+data+"""
+        <td>"""
+            + data
+            + """
         <tr><td>&nbsp;
         <tr><td colspan=2><input type='button' value='Okay' onclick='dialog.send(gui.CHANGE)'> <input type='button' value='Cancel' onclick='dialog.close()'>
-        </table>""")
-        gui.Dialog.__init__(self,title,doc)
-        
-        self.value = doc['form']
+        </table>""",
+        )
+        gui.Dialog.__init__(self, title, doc)
 
+        self.value = doc["form"]
 
 
 def run():
-    #top.connect(gui.QUIT,top.quit,None)
-    top.connect(gui.QUIT,cmd_quit,None)
-    top.connect(pygame.ACTIVEEVENT, cmd_active_save,None)
-    top.init(app,app.screen)
+    # top.connect(gui.QUIT,top.quit,None)
+    top.connect(gui.QUIT, cmd_quit, None)
+    top.connect(pygame.ACTIVEEVENT, cmd_active_save, None)
+    top.init(app, app.screen)
     app.top = top
     top.run()
-    
+
 
 def main():
     init_ini()
     init_opts()
     init_gui()
-    
+
     restart = 1
     while restart:
         restart = 0
         try:
             init_app()
             run()
-        except Restart: restart = 1
-        
+        except Restart:
+            restart = 1
+
 
-        
-    
 main()
 # vim: set filetype=python sts=4 sw=4 noet si :
```

### Comparing `zanthor-1.2.3/zanthor/data/gfx/hole4.png` & `zanthor-1.2.4a2/zanthor/data/gfx/hole4.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/heart.png` & `zanthor-1.2.4a2/zanthor/data/gfx/heart.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/gfx/hole3.png` & `zanthor-1.2.4a2/zanthor/data/gfx/hole3.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/ETHNOCEN.TTF` & `zanthor-1.2.4a2/zanthor/data/intro/ETHNOCEN.TTF`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/soundtrack2.ogg` & `zanthor-1.2.4a2/zanthor/data/intro/soundtrack2.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/grass.ogg` & `zanthor-1.2.4a2/zanthor/data/intro/grass.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/dazzlesh.ttf` & `zanthor-1.2.4a2/zanthor/data/intro/dazzlesh.ttf`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/read_me.html` & `zanthor-1.2.4a2/zanthor/data/intro/read_me.html`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/intro1.ogg` & `zanthor-1.2.4a2/zanthor/data/intro/intro1.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/mybkgr.png` & `zanthor-1.2.4a2/zanthor/data/intro/mybkgr.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/title.jpg` & `zanthor-1.2.4a2/zanthor/data/intro/title.jpg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/soundtrack1.ogg` & `zanthor-1.2.4a2/zanthor/data/intro/soundtrack1.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/zanthor.ogg` & `zanthor-1.2.4a2/zanthor/data/intro/zanthor.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/WALSHES.TTF` & `zanthor-1.2.4a2/zanthor/data/intro/WALSHES.TTF`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/introbg.png` & `zanthor-1.2.4a2/zanthor/data/intro/introbg.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/intro/soundtrack3.ogg` & `zanthor-1.2.4a2/zanthor/data/intro/soundtrack3.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/peasants1.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/peasants1.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/cannon2.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/cannon2.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/hitground.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/hitground.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/squish2.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/squish2.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/water.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/water.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/peasants2.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/peasants2.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/peasants3.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/peasants3.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/birds1.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/birds1.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/ouch2.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/ouch2.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/upgrade.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/upgrade.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/hitenemy.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/hitenemy.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/birds2.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/birds2.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/hitwall2.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/hitwall2.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/cannon3.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/cannon3.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/engine-fast.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/engine-fast.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/cannon.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/cannon.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/coal.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/coal.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/ouch1.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/ouch1.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/squish1.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/squish1.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/engine-slow.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/engine-slow.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/destroyenemy.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/destroyenemy.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/hitwall.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/hitwall.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/sounds/release.ogg` & `zanthor-1.2.4a2/zanthor/data/sounds/release.ogg`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/vslider.up.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/vslider.up.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/scroller.slide.v.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/scroller.slide.v.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/scroller.slide.h.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/scroller.slide.h.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/filebrowser.folder.png` & `zanthor-1.2.4a2/zanthor/data/themes/default/filebrowser.folder.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/vslider.bar.hover.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/vslider.bar.hover.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/vslider.bar.normal.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/vslider.bar.normal.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/rdot.hover.png` & `zanthor-1.2.4a2/zanthor/data/themes/default/rdot.hover.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/dialog.close.normal.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/dialog.close.normal.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/slider.bar.hover.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/button.hover.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/progressbar.bar.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/progressbar.bar.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/tool.down.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/menu.down.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/menu.down.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/tool.down.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/hslider.bar.hover.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/hslider.bar.hover.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/button.hover.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/slider.bar.hover.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/hslider.bar.normal.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/button.normal.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/dialog.close.hover.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/dialog.close.hover.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/box.xcf` & `zanthor-1.2.4a2/zanthor/data/themes/default/box.xcf`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/button.down.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/button.down.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/hslider.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/hslider.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/radio.off.hover.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/radio.off.hover.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/vslider.down.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/vslider.down.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/tool.hover.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/tool.hover.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/vdot.down.png` & `zanthor-1.2.4a2/zanthor/data/themes/default/vdot.down.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/slider.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/slider.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/vdot.hover.png` & `zanthor-1.2.4a2/zanthor/data/themes/default/vdot.hover.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/dialog.close.down.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/dialog.close.down.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/radio.off.normal.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/radio.off.normal.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/rdot.down.png` & `zanthor-1.2.4a2/zanthor/data/themes/default/rdot.down.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/out.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/out.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/button.normal.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/hslider.bar.normal.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/listitem.hover.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/listitem.hover.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/radio.on.hover.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/radio.on.hover.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/listitem.down.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/listitem.down.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/listitem.normal.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/listitem.normal.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/Vera.ttf` & `zanthor-1.2.4a2/zanthor/data/themes/default/Vera.ttf`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/vslider.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/vslider.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/config.txt` & `zanthor-1.2.4a2/zanthor/data/themes/default/config.txt`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/radio.on.normal.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/radio.on.normal.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/dot.hover.png` & `zanthor-1.2.4a2/zanthor/data/themes/default/dot.hover.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/dot.xcf` & `zanthor-1.2.4a2/zanthor/data/themes/default/dot.xcf`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/checkbox.on.hover.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/checkbox.on.hover.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/slider.bar.normal.tga` & `zanthor-1.2.4a2/zanthor/data/themes/default/slider.bar.normal.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/dot.down.png` & `zanthor-1.2.4a2/zanthor/data/themes/default/dot.down.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/default/desktop.xcf` & `zanthor-1.2.4a2/zanthor/data/themes/default/desktop.xcf`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/gray/filebrowser.folder.png` & `zanthor-1.2.4a2/zanthor/data/themes/gray/filebrowser.folder.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/gray/Vera.ttf` & `zanthor-1.2.4a2/zanthor/data/themes/gray/Vera.ttf`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/gray/config.txt` & `zanthor-1.2.4a2/zanthor/data/themes/gray/config.txt`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/tools/icons48.draw.tga` & `zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.draw.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/tools/icons48.bkgr.tga` & `zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.bkgr.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/tools/icons48.tile.tga` & `zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.tile.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/tools/icons48.code.tga` & `zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.code.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/tools/icons48.line.tga` & `zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.line.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/tools/icons48.fill.tga` & `zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.fill.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/tools/icons48.pixel.tga` & `zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.pixel.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/tools/icons48.select.tga` & `zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.select.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/themes/tools/icons48.eraser.tga` & `zanthor-1.2.4a2/zanthor/data/themes/tools/icons48.eraser.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/codes.tga` & `zanthor-1.2.4a2/zanthor/data/levels/codes.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/tileedit.ini` & `zanthor-1.2.4a2/zanthor/data/levels/tileedit.ini`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/level1.tga` & `zanthor-1.2.4a2/zanthor/data/levels/level1.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/tiles.tga` & `zanthor-1.2.4a2/zanthor/data/levels/tiles.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/level5.tga` & `zanthor-1.2.4a2/zanthor/data/levels/level5.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/level7.tga` & `zanthor-1.2.4a2/zanthor/data/levels/level7.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/level2.tga` & `zanthor-1.2.4a2/zanthor/data/levels/level2.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/level4.tga` & `zanthor-1.2.4a2/zanthor/data/levels/level4.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/level3.tga` & `zanthor-1.2.4a2/zanthor/data/levels/level3.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/test2.tga` & `zanthor-1.2.4a2/zanthor/data/levels/test2.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/test4.tga` & `zanthor-1.2.4a2/zanthor/data/levels/test4.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/level6.tga` & `zanthor-1.2.4a2/zanthor/data/levels/level6.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/leveledit.ini` & `zanthor-1.2.4a2/zanthor/data/levels/leveledit.ini`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/level8.tga` & `zanthor-1.2.4a2/zanthor/data/levels/level8.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/levels/leveledit.py` & `zanthor-1.2.4a2/zanthor/data/levels/leveledit.py`

 * *Files 20% similar despite different names*

```diff
@@ -61,950 +61,1024 @@
 arrows - change tile
 shift+arrows - scroll screen by 1/8 screen size jumps
 ctrl+arrows - scroll screen by full screen size jumps
 return - toggle fullscreen
 </pre>
 """
 
-import os,sys    
+import os, sys
 from optparse import OptionParser
-from ConfigParser import ConfigParser
+from configparser import ConfigParser
 import pygame
 from pygame.locals import *
 
 # the following line is not needed if pgu is installed
-import sys; sys.path.insert(0, "..")
+import sys
 
-from pgu import gui, html, tilevid, isovid, hexvid
+sys.path.insert(0, "..")
 
+from pgu import gui, html, tilevid, isovid, hexvid
 
 
-#whatever...
+# whatever...
 ini_fname = "leveledit.ini"
 ini = ConfigParser()
 cfg = {}
 
+
 class _app(gui.Container):
     def __init__(self):
         gui.Container.__init__(self)
-        #self.cls = "desktop"
-        #self.background = gui.Box(self.style.background)
+        # self.cls = "desktop"
+        # self.background = gui.Box(self.style.background)
 
-        self.screen_w = cfg['screen_w']
-        self.screen_h = cfg['screen_h']
-        self.screen = pygame.display.set_mode((self.screen_w,
-            self.screen_h), SWSURFACE)
+        self.screen_w = cfg["screen_w"]
+        self.screen_h = cfg["screen_h"]
+        self.screen = pygame.display.set_mode((self.screen_w, self.screen_h), SWSURFACE)
 
-        self.fname = cfg['fname']
-        
-        k = cfg['class']
+        self.fname = cfg["fname"]
+
+        k = cfg["class"]
         parts = k.split(".")
         n = ".".join(parts[:-1])
-        m = __import__(n,globals(),locals(),parts[-1])
-        c = getattr(m,parts[-1])
+        m = __import__(n, globals(), locals(), parts[-1])
+        c = getattr(m, parts[-1])
         self.level = c()
 
-        #self.level = pygame.image.load(self.level_fname)
-        #self.level = tilevid.Tilevid()
-        #g = self.level = isovid.Isovid()
-        
-    
+        # self.level = pygame.image.load(self.level_fname)
+        # self.level = tilevid.Tilevid()
+        # g = self.level = isovid.Isovid()
+
         if self.fname != None:
-            self.level.tga_load_level(self.fname,1)
+            self.level.tga_load_level(self.fname, 1)
         else:
-            self.level.resize((cfg['width'],cfg['height']),1)
-        #self.level_w, self.level_h = (self.level.get_width(), self.level.get_height())
-        self.level_w, self.level_h = len(self.level.tlayer[0]),len(self.level.tlayer)
+            self.level.resize((cfg["width"], cfg["height"]), 1)
+        # self.level_w, self.level_h = (self.level.get_width(), self.level.get_height())
+        self.level_w, self.level_h = len(self.level.tlayer[0]), len(self.level.tlayer)
 
         self.tiles_last_ctime = None
         self.codes_last_ctime = None
 
         self.load_tiles_and_codes()
-        
-
-
 
-        
-        
         self.tile = 0
         self.code = 0
-        
-        self.mode = 'tile'
+
+        self.mode = "tile"
         self.clipboard = None
         self.history = []
-        #self.modrect = pygame.Rect(0xffff,0xffff,-0xffff,-0xffff)
-        
+        # self.modrect = pygame.Rect(0xffff,0xffff,-0xffff,-0xffff)
+
         self.changes = []
         self.dirty = 0
-        
 
     def load_tiles_and_codes(self):
         #
         #
 
-        self.tile_w, self.tile_h = cfg['tile_w'], cfg['tile_h']
+        self.tile_w, self.tile_h = cfg["tile_w"], cfg["tile_h"]
 
-        self.tiles_fname = cfg['tiles']
+        self.tiles_fname = cfg["tiles"]
         if os.path.isfile(self.tiles_fname):
             # we check to see if the ctime is the same.
 
             newctime = os.stat(self.tiles_fname)[9]
             if newctime <= self.tiles_last_ctime:
-                #nothing to do, so we return.
+                # nothing to do, so we return.
                 return
 
             self.tiles_last_ctime = newctime
 
             self.tiles = pygame.image.load(self.tiles_fname)
         else:
             self.tiles = hex_image(self)
-        self.tiles_w, self.tiles_h = (self.tiles.get_width(),
-            self.tiles.get_height())
-        self.level.tga_load_tiles(self.tiles,(self.tile_w,self.tile_h))
+        self.tiles_w, self.tiles_h = (self.tiles.get_width(), self.tiles.get_height())
+        self.level.tga_load_tiles(self.tiles, (self.tile_w, self.tile_h))
 
-        self.codes_fname = cfg['codes']
+        self.codes_fname = cfg["codes"]
         if os.path.isfile(self.codes_fname):
             newctime = os.stat(self.codes_fname)[9]
             if newctime <= self.codes_last_ctime:
-                #nothing to do, so we return.
+                # nothing to do, so we return.
                 return
             self.codes_last_ctime = newctime
 
             self.codes = pygame.image.load(self.codes_fname)
         else:
             self.codes = hex_image(self)
-                        
-        self.codes_w, self.codes_h = (self.codes.get_width(),
-            self.codes.get_height())
 
-        
+        self.codes_w, self.codes_h = (self.codes.get_width(), self.codes.get_height())
+
         tmp = self.level.tiles
-        self.level.tiles = [None for i in xrange(0,256)]
-        self.level.tga_load_tiles(self.codes,(self.tile_w,self.tile_h))
+        self.level.tiles = [None for i in range(0, 256)]
+        self.level.tga_load_tiles(self.codes, (self.tile_w, self.tile_h))
         self.level.codes = self.level.tiles
         self.level.tiles = tmp
 
+    def mod(self, rect):
+        self.dirty = 1
+        self.changes.append((pygame.Rect(rect), self.copy(rect)))
 
+    def view_init(self, dw, dh):
+        self.view_w = dw  # / self.tile_w
+        self.view_h = dh  # / self.tile_h
 
+        if "view_w" in cfg and cfg["view_w"] != 0:
+            self.view_w = min(self.view_w, cfg["view_w"])
+        if "view_h" in cfg and cfg["view_h"] != 0:
+            self.view_h = min(self.view_h, cfg["view_h"])
 
+        # self.view_w = min(self.level.size[0],self.view_w)
+        # self.view_h = min(self.level.size[1],self.view_h)
 
+        # print self.view_w,self.view_h
 
-    def mod(self,rect):
-        self.dirty = 1
-        self.changes.append((pygame.Rect(rect),self.copy(rect)))
-    
+        # self.view = self.level.subsurface((0,0,self.view_w,self.view_h))
+        self.select = Rect(
+            0, 0, self.level.size[0], self.level.size[1]
+        )  # self.view_w,self.view_h)
 
-    def view_init(self,dw,dh):        
-        
-        self.view_w = dw #/ self.tile_w
-        self.view_h = dh #/ self.tile_h
-        
-        if 'view_w' in cfg and cfg['view_w'] != 0:
-            self.view_w = min(self.view_w, cfg['view_w'])
-        if 'view_h' in cfg and cfg['view_h'] != 0:
-            self.view_h = min(self.view_h, cfg['view_h'])
-        
-        #self.view_w = min(self.level.size[0],self.view_w)
-        #self.view_h = min(self.level.size[1],self.view_h)
-        
-        #print self.view_w,self.view_h
-        
-        #self.view = self.level.subsurface((0,0,self.view_w,self.view_h))
-        self.select = Rect(0,0,self.level.size[0],self.level.size[1]) #self.view_w,self.view_h)
-        
-    def fill(self,rect,v):
+    def fill(self, rect, v):
         lvl = self.level
-        w,h = lvl.size
-        
-        for layer,n in [ (lvl.tlayer,0), (lvl.blayer,1), (lvl.clayer,2) ]:
-            for y in range(0,rect.h):
-                for x in range(0,rect.w):
-                    tx,ty = x+rect.x,y+rect.y
-                    if tx >= 0 and tx < w and ty >= 0 and ty < h: layer[ty][tx] = v[n]
-        
-    def copy(self,rect):
-        data = [[[None for x in range(0,rect.w)] for y in range(0,rect.h)] for l in range(0,4)] 
+        w, h = lvl.size
+
+        for layer, n in [(lvl.tlayer, 0), (lvl.blayer, 1), (lvl.clayer, 2)]:
+            for y in range(0, rect.h):
+                for x in range(0, rect.w):
+                    tx, ty = x + rect.x, y + rect.y
+                    if tx >= 0 and tx < w and ty >= 0 and ty < h:
+                        layer[ty][tx] = v[n]
+
+    def copy(self, rect):
+        data = [
+            [[None for x in range(0, rect.w)] for y in range(0, rect.h)]
+            for l in range(0, 4)
+        ]
 
         lvl = self.level
-        w,h = lvl.size
-        
-        for layer,n in [ (lvl.tlayer,0), (lvl.blayer,1), (lvl.clayer,2) ]:
-            for y in range(0,rect.h):
-                for x in range(0,rect.w):
-                    tx,ty = x+rect.x,y+rect.y
-                    if tx >= 0 and tx < w and ty >= 0 and ty < h: data[n][y][x] = layer[ty][tx]
+        w, h = lvl.size
+
+        for layer, n in [(lvl.tlayer, 0), (lvl.blayer, 1), (lvl.clayer, 2)]:
+            for y in range(0, rect.h):
+                for x in range(0, rect.w):
+                    tx, ty = x + rect.x, y + rect.y
+                    if tx >= 0 and tx < w and ty >= 0 and ty < h:
+                        data[n][y][x] = layer[ty][tx]
         return data
-                
-    def paste(self,rect,data):
+
+    def paste(self, rect, data):
         lvl = self.level
-        w,h = lvl.size
-        
-        for layer,n in [ (lvl.tlayer,0), (lvl.blayer,1), (lvl.clayer,2) ]:
-            for y in range(0,rect.h):
-                for x in range(0,rect.w):
-                    tx,ty = x+rect.x,y+rect.y
+        w, h = lvl.size
+
+        for layer, n in [(lvl.tlayer, 0), (lvl.blayer, 1), (lvl.clayer, 2)]:
+            for y in range(0, rect.h):
+                for x in range(0, rect.w):
+                    tx, ty = x + rect.x, y + rect.y
                     v = data[n][y][x]
-                    if v != None and tx >= 0 and tx < w and ty >= 0 and ty < h: layer[ty][tx] = v
-        
-        
+                    if v != None and tx >= 0 and tx < w and ty >= 0 and ty < h:
+                        layer[ty][tx] = v
+
     def archive(self):
-        if not len(self.changes): return
-        
+        if not len(self.changes):
+            return
+
         self.dirty = 1
         h = self.history
         if len(h) >= 32:
             del h[0]
-        #c = pygame.Surface((self.view_w,self.view_h),SWSURFACE,self.view)
-        #c.fill((0,0,0,0))
-        #c.blit(self.view,(0,0))
-        
+        # c = pygame.Surface((self.view_w,self.view_h),SWSURFACE,self.view)
+        # c.fill((0,0,0,0))
+        # c.blit(self.view,(0,0))
+
         lvl = self.level
-        #ox,oy = lvl.screen_to_tile((0,0))
-        #bx,by = lvl.screen_to_tile((self.vdraw.rect.w,self.vdraw.rect.h))
-        
-        #rect = pygame.Rect(ox,oy,bx-ox,by-oy)
-        #print self.modrect
-        
+        # ox,oy = lvl.screen_to_tile((0,0))
+        # bx,by = lvl.screen_to_tile((self.vdraw.rect.w,self.vdraw.rect.h))
+
+        # rect = pygame.Rect(ox,oy,bx-ox,by-oy)
+        # print self.modrect
+
         h.append(self.changes)
         self.changes = []
-        
+
     def undo(self):
-        if len(self.changes): self.archive()
-            
-        if len(self.history) == 0: return
-        
+        if len(self.changes):
+            self.archive()
+
+        if len(self.history) == 0:
+            return
+
         self.dirty = 1
         changes = self.history.pop()
-        
+
         changes.reverse()
-        for rect,data in changes:
-            self.paste(rect,data)
-            
+        for rect, data in changes:
+            self.paste(rect, data)
+
         self.vdraw.repaint()
-        self.tpicker.repaint() #huh?
-        
+        self.tpicker.repaint()  # huh?
+
         self.changes = []
         return
-        
-        self.level.fill((0,0,0,0),(off[0],off[1],self.view_w,self.view_h))
-        self.level.blit(c,off)
+
+        self.level.fill((0, 0, 0, 0), (off[0], off[1], self.view_w, self.view_h))
+        self.level.blit(c, off)
         self.vdraw.repaint()
         self.tpicker.repaint()
-        
-    def __setattr__(self,k,v):
+
+    def __setattr__(self, k, v):
         self.__dict__[k] = v
-        
-        if k == 'view':
-            if hasattr(self,'vdraw'): self.vdraw.repaint()
-        
-        if k == 'tile':
-            if hasattr(self,'tpicker'): self.tpicker.repaint()
-                
-        if k == 'code':
-            if hasattr(self,'cpicker'): self.cpicker.repaint()
-        
-            
-    def event(self,e):
-        if e.type is KEYDOWN:
-            for key,cmd,value in keys:
+
+        if k == "view":
+            if hasattr(self, "vdraw"):
+                self.vdraw.repaint()
+
+        if k == "tile":
+            if hasattr(self, "tpicker"):
+                self.tpicker.repaint()
+
+        if k == "code":
+            if hasattr(self, "cpicker"):
+                self.cpicker.repaint()
+
+    def event(self, e):
+        if e.type == KEYDOWN:
+            for key, cmd, value in keys:
                 if e.key == key:
                     cmd(value)
                     return
-        return gui.Container.event(self,e)
-    
+        return gui.Container.event(self, e)
+
 
 def hex_image(self):
-    if not hasattr(self,'tiles_w'): self.tiles_w = 256
-    if not hasattr(self,'tiles_h'): self.tiles_h = 256
-    rimg = pygame.Surface((self.tiles_w,self.tiles_h)).convert_alpha()
-    rimg.fill((0,0,0,0))
-    w,h = self.tiles_w / self.tile_w, self.tiles_h / self.tile_h
+    if not hasattr(self, "tiles_w"):
+        self.tiles_w = 256
+    if not hasattr(self, "tiles_h"):
+        self.tiles_h = 256
+    rimg = pygame.Surface((self.tiles_w, self.tiles_h)).convert_alpha()
+    rimg.fill((0, 0, 0, 0))
+    w, h = self.tiles_w / self.tile_w, self.tiles_h / self.tile_h
     n = 0
-    fnt = pygame.font.SysFont("helvetica",self.tile_h-1)
-    for y in range(0,h):
-        for x in range(0,w):
-            n = x+y*w
+    fnt = pygame.font.SysFont("helvetica", self.tile_h - 1)
+    for y in range(0, h):
+        for x in range(0, w):
+            n = x + y * w
             if n != 0:
-                xx,yy = x*self.tile_w,y*self.tile_h
-                img = fnt.render("%02X"%n,0,(0,0,0))
-                img = pygame.transform.scale(img,(self.tile_w-1,self.tile_h-1))
-                rimg.blit(img,(xx+1,yy+1))
-                img = fnt.render("%02X"%n,0,(255,255,255))
-                img = pygame.transform.scale(img,(self.tile_w-1,self.tile_h-1))
-                rimg.blit(img,(xx,yy))
+                xx, yy = x * self.tile_w, y * self.tile_h
+                img = fnt.render("%02X" % n, 0, (0, 0, 0))
+                img = pygame.transform.scale(img, (self.tile_w - 1, self.tile_h - 1))
+                rimg.blit(img, (xx + 1, yy + 1))
+                img = fnt.render("%02X" % n, 0, (255, 255, 255))
+                img = pygame.transform.scale(img, (self.tile_w - 1, self.tile_h - 1))
+                rimg.blit(img, (xx, yy))
     return rimg
 
 
 class tpicker(gui.Widget):
     def __init__(self):
         gui.Widget.__init__(self)
         self.style.width = app.tiles_w
         self.style.height = app.tiles_h
-        
-    def paint(self,s):
-        s.fill((128,128,128))
-        s.blit(app.tiles,(0,0))
-        w = app.tiles_w/app.tile_w
-        x,y = app.tile%w,app.tile/w
-        off = x*app.tile_w,y*app.tile_h
-        pygame.draw.rect(s,(255,255,255),(off[0],off[1],app.tile_w,app.tile_h),2)
-        
-    def event(self,e):
-        if (e.type is MOUSEBUTTONDOWN and e.button == 1) or (e.type is MOUSEMOTION and e.buttons[0] == 1 and self.container.myfocus == self):
-            w = app.tiles_w/app.tile_w
-            x,y = e.pos[0]/app.tile_w,e.pos[1]/app.tile_h
-            n = x+y*w
+
+    def paint(self, s):
+        s.fill((128, 128, 128))
+        s.blit(app.tiles, (0, 0))
+        w = app.tiles_w / app.tile_w
+        x, y = app.tile % w, app.tile / w
+        off = x * app.tile_w, y * app.tile_h
+        pygame.draw.rect(
+            s, (255, 255, 255), (off[0], off[1], app.tile_w, app.tile_h), 2
+        )
+
+    def event(self, e):
+        if (e.type == MOUSEBUTTONDOWN and e.button == 1) or (
+            e.type == MOUSEMOTION
+            and e.buttons[0] == 1
+            and self.container.myfocus == self
+        ):
+            w = app.tiles_w / app.tile_w
+            x, y = e.pos[0] / app.tile_w, e.pos[1] / app.tile_h
+            n = x + y * w
             self.set(n)
-            if app.mode not in ('tile','bkgr'):
-                app.tools['tile'].click()
-    
-    def set(self,n):
-        if n < 0 or n >= len(app.level.tiles) or app.level.tiles[n] == None: return
+            if app.mode not in ("tile", "bkgr"):
+                app.tools["tile"].click()
+
+    def set(self, n):
+        if n < 0 or n >= len(app.level.tiles) or app.level.tiles[n] == None:
+            return
         app.tile = n
 
 
 class cpicker(gui.Widget):
     def __init__(self):
         gui.Widget.__init__(self)
         self.style.width = app.codes_w
         self.style.height = app.codes_h
-        
-    def paint(self,s):
-        s.fill((128,128,128))
-        s.blit(app.codes,(0,0))
-        w = app.codes_w/app.tile_w
-        x,y = app.code%w,app.code/w
-        off = x*app.tile_w,y*app.tile_h
-        pygame.draw.rect(s,(255,255,255),(off[0],off[1],app.tile_w,app.tile_h),2)
-        
-    def event(self,e):
-        if (e.type is MOUSEBUTTONDOWN and e.button == 1) or (e.type is MOUSEMOTION and e.buttons[0] == 1 and self.container.myfocus == self):
-            w = app.codes_w/app.tile_w
-            x,y = e.pos[0]/app.tile_w,e.pos[1]/app.tile_h
-            n = x+y*w
+
+    def paint(self, s):
+        s.fill((128, 128, 128))
+        s.blit(app.codes, (0, 0))
+        w = app.codes_w / app.tile_w
+        x, y = app.code % w, app.code / w
+        off = x * app.tile_w, y * app.tile_h
+        pygame.draw.rect(
+            s, (255, 255, 255), (off[0], off[1], app.tile_w, app.tile_h), 2
+        )
+
+    def event(self, e):
+        if (e.type == MOUSEBUTTONDOWN and e.button == 1) or (
+            e.type == MOUSEMOTION
+            and e.buttons[0] == 1
+            and self.container.myfocus == self
+        ):
+            w = app.codes_w / app.tile_w
+            x, y = e.pos[0] / app.tile_w, e.pos[1] / app.tile_h
+            n = x + y * w
             self.set(n)
-            app.tools['code'].click()
-    
-    def set(self,n):
-        if n < 0 or n >= len(app.level.codes) or app.level.codes[n] == None: return
-        app.code = n
+            app.tools["code"].click()
 
+    def set(self, n):
+        if n < 0 or n >= len(app.level.codes) or app.level.codes[n] == None:
+            return
+        app.code = n
 
 
 class vwrap(gui.Table):
-    def __init__(self,**params):
-        gui.Table.__init__(self,**params)
-        self.style.width = app.view_w #* app.tile_w
-        self.style.height = app.view_h #* app.tile_h
-        w,h = self.rect.w,self.rect.h = self.style.width,self.style.height
-        
+    def __init__(self, **params):
+        gui.Table.__init__(self, **params)
+        self.style.width = app.view_w  # * app.tile_w
+        self.style.height = app.view_h  # * app.tile_h
+        w, h = self.rect.w, self.rect.h = self.style.width, self.style.height
+
         sw = 16
-        
-        self.vdraw = e = vdraw(width=w-sw,height=h-sw)
-        self.add(e,0,0)
-        
-        rect = pygame.Rect(0,0,app.level.size[0],app.level.size[1])
-        tcorners = [rect.topleft,rect.topright,rect.bottomright,rect.bottomleft] 
-        corners = [app.level.tile_to_view(tcorners[n]) for n in range(0,4)]
-        
-        minx,miny,maxx,maxy = 0xffff,0xffff,-0xffff,-0xffff
-        for x,y in corners:
-            minx,miny,maxx,maxy = min(minx,x),min(miny,y),max(maxx,x),max(maxy,y)
-
-        minx -= w/2
-        maxx -= w/2
-        miny -= h/2
-        maxy -= h/2
-        
-        self.vs = e = gui.VSlider(0,miny,maxy,sw*4,width=sw,height=h-sw)
-        self.add(e,1,0)
-        e.connect(gui.CHANGE,self.move_y,e)
-        
-        self.hs = e = gui.HSlider(0,minx,maxx,sw*4,width=w-sw,height=sw)
-        self.add(e,0,1)
-        e.connect(gui.CHANGE,self.move_x,e)
-        
-    def move_x(self,value):
+
+        self.vdraw = e = vdraw(width=w - sw, height=h - sw)
+        self.add(e, 0, 0)
+
+        rect = pygame.Rect(0, 0, app.level.size[0], app.level.size[1])
+        tcorners = [rect.topleft, rect.topright, rect.bottomright, rect.bottomleft]
+        corners = [app.level.tile_to_view(tcorners[n]) for n in range(0, 4)]
+
+        minx, miny, maxx, maxy = 0xFFFF, 0xFFFF, -0xFFFF, -0xFFFF
+        for x, y in corners:
+            minx, miny, maxx, maxy = (
+                min(minx, x),
+                min(miny, y),
+                max(maxx, x),
+                max(maxy, y),
+            )
+
+        minx -= w / 2
+        maxx -= w / 2
+        miny -= h / 2
+        maxy -= h / 2
+
+        self.vs = e = gui.VSlider(0, miny, maxy, sw * 4, width=sw, height=h - sw)
+        self.add(e, 1, 0)
+        e.connect(gui.CHANGE, self.move_y, e)
+
+        self.hs = e = gui.HSlider(0, minx, maxx, sw * 4, width=w - sw, height=sw)
+        self.add(e, 0, 1)
+        e.connect(gui.CHANGE, self.move_x, e)
+
+    def move_x(self, value):
         v = value.value
         if app.level.view.x != v:
             app.level.view.x = v
             app.vdraw.repaint()
-    
-    def move_y(self,value):
+
+    def move_y(self, value):
         v = value.value
         if app.level.view.y != v:
             app.level.view.y = v
             app.vdraw.repaint()
-        
+
     def adjust(self):
         self.vs.value = app.level.view.y
         self.hs.value = app.level.view.x
-        
+
 
 class vdraw(gui.Widget):
     def repaint(self):
         self.container.adjust()
         gui.Widget.repaint(self)
-        
-    def __init__(self,**params):
-        gui.Widget.__init__(self,**params)
-        #self.style.width = app.view_w #* app.tile_w
-        #self.style.height = app.view_h #* app.tile_h
-        self.rect.w,self.rect.h = self.style.width,self.style.height
-        
-        s = pygame.Surface((self.rect.w,self.rect.h))
-        clrs = [(148,148,148),(108,108,108)]
+
+    def __init__(self, **params):
+        gui.Widget.__init__(self, **params)
+        # self.style.width = app.view_w #* app.tile_w
+        # self.style.height = app.view_h #* app.tile_h
+        self.rect.w, self.rect.h = self.style.width, self.style.height
+
+        s = pygame.Surface((self.rect.w, self.rect.h))
+        clrs = [(148, 148, 148), (108, 108, 108)]
         inc = 7
-        for y in range(0,self.rect.w/inc):
-            for x in range(0,self.rect.h/inc):
-                s.fill(clrs[(x+y)%2],(x*inc,y*inc,inc,inc))
+        for y in range(0, self.rect.w / inc):
+            for x in range(0, self.rect.h / inc):
+                s.fill(clrs[(x + y) % 2], (x * inc, y * inc, inc, inc))
         self.bg = s
 
-        s = pygame.Surface((self.rect.w,self.rect.h)).convert_alpha()
-        s.fill((0,0,0,0))
-        for x in range(0,app.view_w):
-            pygame.draw.line(s,(0,0,0),(self.rect.w*x/app.view_w,0),(self.rect.w*x/app.view_w,self.rect.h))
-        for y in range(0,app.view_h):
-            pygame.draw.line(s,(0,0,0),(0,self.rect.h*y/app.view_h),(self.rect.w,self.rect.h*y/app.view_h))
+        s = pygame.Surface((self.rect.w, self.rect.h)).convert_alpha()
+        s.fill((0, 0, 0, 0))
+        for x in range(0, app.view_w):
+            pygame.draw.line(
+                s,
+                (0, 0, 0),
+                (self.rect.w * x / app.view_w, 0),
+                (self.rect.w * x / app.view_w, self.rect.h),
+            )
+        for y in range(0, app.view_h):
+            pygame.draw.line(
+                s,
+                (0, 0, 0),
+                (0, self.rect.h * y / app.view_h),
+                (self.rect.w, self.rect.h * y / app.view_h),
+            )
         self.grid = s
-        
-        self.pos = 0,0
 
-        
-    def paint(self,s):
-        #print s
-        #print s.get_width(),s.get_height(),s.get_clip()
-        #s.blit(self.bg,(0,0))
-        s.fill((128,128,128))
+        self.pos = 0, 0
+
+    def paint(self, s):
+        # print s
+        # print s.get_width(),s.get_height(),s.get_clip()
+        # s.blit(self.bg,(0,0))
+        s.fill((128, 128, 128))
 
-        #make sure to clamp the bounds
+        # make sure to clamp the bounds
         if app.level.bounds != None:
             app.level.view.clamp_ip(app.level.bounds)
-        
-        #draw border        
-        rect = pygame.Rect(0,0,app.level.size[0],app.level.size[1])
-        tcorners = [rect.topleft,rect.topright,rect.bottomright,rect.bottomleft]
-        corners = [app.level.tile_to_screen(tcorners[n]) for n in range(0,4)]
-        pygame.draw.lines(s,(255,255,0),1,corners,2)
 
-        
-        #s.fill((0,0,0))
-        #0/0
+        # draw border
+        rect = pygame.Rect(0, 0, app.level.size[0], app.level.size[1])
+        tcorners = [rect.topleft, rect.topright, rect.bottomright, rect.bottomleft]
+        corners = [app.level.tile_to_screen(tcorners[n]) for n in range(0, 4)]
+        pygame.draw.lines(s, (255, 255, 0), 1, corners, 2)
+
+        # s.fill((0,0,0))
+        # 0/0
         app.level.paint(s)
-        
+
         tmp_tiles = app.level.tiles
         tmp_tlayer = app.level.tlayer
         tmp_blayer = app.level.blayer
-        
+
         app.level.tiles = app.level.codes
         app.level.tlayer = app.level.clayer
         app.level.blayer = None
-        
+
         app.level.paint(s)
-        
+
         app.level.tiles = tmp_tiles
         app.level.tlayer = tmp_tlayer
         app.level.blayer = tmp_blayer
-        
-        rect = pygame.Rect(self.pos[0],self.pos[1],1,1)
-        tcorners = [rect.topleft,rect.topright,rect.bottomright,rect.bottomleft]
-        corners = [app.level.tile_to_screen(tcorners[n]) for n in range(0,4)]
-        pygame.draw.lines(s,(196,196,196),1,corners,2)
-
-        rect = pygame.Rect(app.select.x,app.select.y,app.select.w,app.select.h) 
-        tcorners = [rect.topleft,rect.topright,rect.bottomright,rect.bottomleft]
-        corners = [app.level.tile_to_screen(tcorners[n]) for n in range(0,4)]
-        pygame.draw.lines(s,(255,255,255),1,corners,2)
 
+        rect = pygame.Rect(self.pos[0], self.pos[1], 1, 1)
+        tcorners = [rect.topleft, rect.topright, rect.bottomright, rect.bottomleft]
+        corners = [app.level.tile_to_screen(tcorners[n]) for n in range(0, 4)]
+        pygame.draw.lines(s, (196, 196, 196), 1, corners, 2)
+
+        rect = pygame.Rect(app.select.x, app.select.y, app.select.w, app.select.h)
+        tcorners = [rect.topleft, rect.topright, rect.bottomright, rect.bottomleft]
+        corners = [app.level.tile_to_screen(tcorners[n]) for n in range(0, 4)]
+        pygame.draw.lines(s, (255, 255, 255), 1, corners, 2)
+
+        # s.blit(self.grid,(0,0))
+        # r = app.select
+        # pygame.draw.rect(s,(255,255,255,128),Rect(r.x*self.rect.w/app.view_w,r.y*self.rect.h/app.view_h,r.w*self.rect.w/app.view_w,r.h*self.rect.h/app.view_h),4)
 
-                
-        
-        #s.blit(self.grid,(0,0))
-        #r = app.select
-        #pygame.draw.rect(s,(255,255,255,128),Rect(r.x*self.rect.w/app.view_w,r.y*self.rect.h/app.view_h,r.w*self.rect.w/app.view_w,r.h*self.rect.h/app.view_h),4)
-        
-    def event(self,e):
-        if e.type is MOUSEMOTION:
+    def event(self, e):
+        if e.type == MOUSEMOTION:
             self.getpos(e)
-        if (e.type is MOUSEBUTTONDOWN and e.button == 3) or (e.type is MOUSEMOTION and e.buttons[2]==1 and self.container.myfocus == self):
+        if (e.type == MOUSEBUTTONDOWN and e.button == 3) or (
+            e.type == MOUSEMOTION
+            and e.buttons[2] == 1
+            and self.container.myfocus == self
+        ):
             self.picker_down(e)
-        if e.type is MOUSEBUTTONDOWN and e.button == 1:
+        if e.type == MOUSEBUTTONDOWN and e.button == 1:
             self.getpos(e)
-            a = '%s_down'%app.mode
-            if hasattr(self,a): getattr(self,a)(e)
-        if e.type is MOUSEMOTION and e.buttons[0] and self.container.myfocus == self:
-            a = '%s_drag'%app.mode
-            if hasattr(self,a): getattr(self,a)(e)
-        if e.type is MOUSEBUTTONUP and e.button == 1:
-            a = '%s_up'%app.mode
-            if hasattr(self,a): getattr(self,a)(e)
-        if e.type is MOUSEBUTTONDOWN and e.button == 2:
+            a = "%s_down" % app.mode
+            if hasattr(self, a):
+                getattr(self, a)(e)
+        if e.type == MOUSEMOTION and e.buttons[0] and self.container.myfocus == self:
+            a = "%s_drag" % app.mode
+            if hasattr(self, a):
+                getattr(self, a)(e)
+        if e.type == MOUSEBUTTONUP and e.button == 1:
+            a = "%s_up" % app.mode
+            if hasattr(self, a):
+                getattr(self, a)(e)
+        if e.type == MOUSEBUTTONDOWN and e.button == 2:
             self.move_down(e)
-        if e.type is MOUSEMOTION and e.buttons[1] and self.container.myfocus == self:
+        if e.type == MOUSEMOTION and e.buttons[1] and self.container.myfocus == self:
             self.move_drag(e)
-    
-    #move
-    def move_down(self,e):
-        self.moff = app.level.view.x,app.level.view.y
+
+    # move
+    def move_down(self, e):
+        self.moff = app.level.view.x, app.level.view.y
         self.m1 = e.pos
-        
-    def move_drag(self,e):
+
+    def move_drag(self, e):
         m1 = self.m1
         m2 = e.pos
-        #app.view = app.level.subsurface((x,y,app.view_w,app.view_h))
-        app.level.view.x,app.level.view.y = self.moff[0] + m1[0]-m2[0], self.moff[1]+m1[1]-m2[1]
+        # app.view = app.level.subsurface((x,y,app.view_w,app.view_h))
+        app.level.view.x, app.level.view.y = (
+            self.moff[0] + m1[0] - m2[0],
+            self.moff[1] + m1[1] - m2[1],
+        )
         self.repaint()
-            
-    #picker
-    def picker_down(self,e):
+
+    # picker
+    def picker_down(self, e):
         pos = self.getpos(e)
-        #tx,ty = app.level.screen_to_tile(e.pos)
-        #r,g,b,a = app.view.get_at(pos)
-        if pos == None: return 
-        tx,ty = pos
-        
-        if app.mode == 'tile':
+        # tx,ty = app.level.screen_to_tile(e.pos)
+        # r,g,b,a = app.view.get_at(pos)
+        if pos == None:
+            return
+        tx, ty = pos
+
+        if app.mode == "tile":
             app.tile = app.level.tlayer[ty][tx]
-        if app.mode == 'bkgr':
+        if app.mode == "bkgr":
             app.tile = app.level.blayer[ty][tx]
         app.code = app.level.clayer[ty][tx]
-        
-    
-    
-    #tile
-    def tile_down(self,e):
+
+    # tile
+    def tile_down(self, e):
         app.archive()
         self.tile_drag(e)
-    
-    def tile_drag(self,e):
+
+    def tile_drag(self, e):
         pos = self.getpos(e)
-        #r,g,b,a = app.view.get_at(pos)
-        #r = app.tile
-        #app.view.set_at(pos,(r,g,b))
-        
-        if pos == None: return
-        tx,ty = pos
-        app.mod(pygame.Rect(tx,ty,1,1))
+        # r,g,b,a = app.view.get_at(pos)
+        # r = app.tile
+        # app.view.set_at(pos,(r,g,b))
+
+        if pos == None:
+            return
+        tx, ty = pos
+        app.mod(pygame.Rect(tx, ty, 1, 1))
         app.level.tlayer[ty][tx] = app.tile
         self.repaint()
-        
-    #bkgr
-    def bkgr_down(self,e):
+
+    # bkgr
+    def bkgr_down(self, e):
         app.archive()
         self.bkgr_drag(e)
-    
-    def bkgr_drag(self,e):
+
+    def bkgr_drag(self, e):
         pos = self.getpos(e)
-        #r,g,b,a = app.view.get_at(pos)
-        #g = app.tile
-        #app.view.set_at(pos,(r,g,b))
-        if pos == None: return
-        tx,ty = pos
-        app.mod(pygame.Rect(tx,ty,1,1))
+        # r,g,b,a = app.view.get_at(pos)
+        # g = app.tile
+        # app.view.set_at(pos,(r,g,b))
+        if pos == None:
+            return
+        tx, ty = pos
+        app.mod(pygame.Rect(tx, ty, 1, 1))
         app.level.blayer[ty][tx] = app.tile
         self.repaint()
-        
-        
-    #code
-    def code_down(self,e):
+
+    # code
+    def code_down(self, e):
         app.archive()
         self.code_drag(e)
-    
-    def code_drag(self,e):
+
+    def code_drag(self, e):
         pos = self.getpos(e)
-        #r,g,b,a = app.view.get_at(pos)
-        #b = app.code
-        #app.view.set_at(pos,(r,g,b))
-        if pos == None: return
-        tx,ty =  pos
-        app.mod(pygame.Rect(tx,ty,1,1))
+        # r,g,b,a = app.view.get_at(pos)
+        # b = app.code
+        # app.view.set_at(pos,(r,g,b))
+        if pos == None:
+            return
+        tx, ty = pos
+        app.mod(pygame.Rect(tx, ty, 1, 1))
         app.level.clayer[ty][tx] = app.code
         self.repaint()
-        
-    #eraser
-    def eraser_down(self,e):
+
+    # eraser
+    def eraser_down(self, e):
         app.archive()
         self.eraser_drag(e)
-    
-    def eraser_drag(self,e):
+
+    def eraser_drag(self, e):
         pos = self.getpos(e)
-        if pos == None: return
-        tx,ty = pos
-        app.mod(pygame.Rect(tx,ty,1,1))
+        if pos == None:
+            return
+        tx, ty = pos
+        app.mod(pygame.Rect(tx, ty, 1, 1))
         app.level.tlayer[ty][tx] = 0
         app.level.blayer[ty][tx] = 0
         app.level.clayer[ty][tx] = 0
-        #app.view.set_at(pos,(0,0,0))
+        # app.view.set_at(pos,(0,0,0))
         self.repaint()
-        
-    def getpos(self,e):
-        tx,ty = app.level.screen_to_tile(e.pos)
-        
-        if tx < 0 or ty < 0 or tx >= app.level.size[0] or ty >= app.level.size[1]: return None
-        
-        if (tx,ty) != self.pos:
-            self.pos = tx,ty
+
+    def getpos(self, e):
+        tx, ty = app.level.screen_to_tile(e.pos)
+
+        if tx < 0 or ty < 0 or tx >= app.level.size[0] or ty >= app.level.size[1]:
+            return None
+
+        if (tx, ty) != self.pos:
+            self.pos = tx, ty
             self.repaint()
-        return tx,ty
-        
-        x,y = e.pos[0]/app.tile_w,e.pos[1]/app.tile_h
-        x = min(max(0,x),app.view_w-1)
-        y = min(max(0,y),app.view_h-1)
-        return x,y
-    
-    def getpos2(self,e):
-        tx,ty = app.level.screen_to_tile(e.pos)
-        
-        return tx+1,ty+1
-        
+        return tx, ty
+
+        x, y = e.pos[0] / app.tile_w, e.pos[1] / app.tile_h
+        x = min(max(0, x), app.view_w - 1)
+        y = min(max(0, y), app.view_h - 1)
+        return x, y
+
+    def getpos2(self, e):
+        tx, ty = app.level.screen_to_tile(e.pos)
+
+        return tx + 1, ty + 1
+
         w = app.tile_w
         h = app.tile_h
-        x,y = (e.pos[0]+w/2)/app.tile_w,(e.pos[1]+h/2)/app.tile_h
-        x = min(max(0,x),app.view_w)
-        y = min(max(0,y),app.view_h)
-        return x,y
-    
-    #select
-    def select_down(self,e):
+        x, y = (e.pos[0] + w / 2) / app.tile_w, (e.pos[1] + h / 2) / app.tile_h
+        x = min(max(0, x), app.view_w)
+        y = min(max(0, y), app.view_h)
+        return x, y
+
+    # select
+    def select_down(self, e):
         pos = self.getpos2(e)
-        pos = pos[0]-1,pos[1]-1
-        app.select = Rect(pos[0],pos[1],1,1)
+        pos = pos[0] - 1, pos[1] - 1
+        app.select = Rect(pos[0], pos[1], 1, 1)
         self.repaint()
-        
-    def select_drag(self,e):
+
+    def select_drag(self, e):
         pos = self.getpos2(e)
-        app.select = Rect(app.select.x,app.select.y,pos[0]-app.select.x,pos[1]-app.select.y)
-        app.select.w = max(1,app.select.w)
-        app.select.h = max(1,app.select.h)
+        app.select = Rect(
+            app.select.x, app.select.y, pos[0] - app.select.x, pos[1] - app.select.y
+        )
+        app.select.w = max(1, app.select.w)
+        app.select.h = max(1, app.select.h)
 
         self.repaint()
-        
+
 
 def cmd_all(value):
-    app.select = Rect(0,0,app.level.size[0],app.level.size[1])
+    app.select = Rect(0, 0, app.level.size[0], app.level.size[1])
     app.vdraw.repaint()
-    
-    #print 'deprecated in v0.5'
-    
-def cmd_shrink(value):    
-    if app.select.w <= 2 or app.select.h <= 2: return
+
+    # print 'deprecated in v0.5'
+
+
+def cmd_shrink(value):
+    if app.select.w <= 2 or app.select.h <= 2:
+        return
     app.select.x += 1
     app.select.y += 1
     app.select.w -= 2
     app.select.h -= 2
 
+
 def cmd_undo(value):
     app.undo()
-    
+
+
 def cmd_redo(value):
     pass
-    
+
+
 def cmd_copy(value):
-    #next version of pygame?
-    #app.clipboard = app.tile.subsurface(app.select).copy()
-    
+    # next version of pygame?
+    # app.clipboard = app.tile.subsurface(app.select).copy()
+
     data = app.copy(app.select)
-    app.clipboard = pygame.Rect(app.select),data
+    app.clipboard = pygame.Rect(app.select), data
     return
-    
-    #s = app.view.subsurface(app.select)
-    #app.clipboard = pygame.Surface((app.select.w,app.select.h),SWSURFACE,s)
-    #app.clipboard.fill((0,0,0,0))
-    #app.clipboard.blit(s,(0,0))
-    
-    print app.clipboard.get_at((0,0))
-    
+
+    # s = app.view.subsurface(app.select)
+    # app.clipboard = pygame.Surface((app.select.w,app.select.h),SWSURFACE,s)
+    # app.clipboard.fill((0,0,0,0))
+    # app.clipboard.blit(s,(0,0))
+
+    print(app.clipboard.get_at((0, 0)))
+
+
 def cmd_paste(value):
     if app.clipboard != None:
         app.archive()
-        #app.view.fill((0,0,0,0),(app.select[0],app.select[1],app.clipboard.get_width(),app.clipboard.get_height()))
-        #app.view.blit(app.clipboard,app.select)
-        #app.vdraw.repaint()
-        
-        rect,data = app.clipboard
-        rect = pygame.Rect(app.select.x,app.select.y,rect.w,rect.h)
-        
+        # app.view.fill((0,0,0,0),(app.select[0],app.select[1],app.clipboard.get_width(),app.clipboard.get_height()))
+        # app.view.blit(app.clipboard,app.select)
+        # app.vdraw.repaint()
+
+        rect, data = app.clipboard
+        rect = pygame.Rect(app.select.x, app.select.y, rect.w, rect.h)
+
         app.mod(rect)
-        app.paste(rect,data)
+        app.paste(rect, data)
         app.vdraw.repaint()
 
+
 class Restart(Exception):
     pass
-    
-def _dirty(fnc,v):
+
+
+def _dirty(fnc, v):
     dialog = DirtyDialog()
+
     def onchange(value):
         value.close()
         return fnc(v)
-    dialog.connect(gui.CHANGE,onchange,dialog)
+
+    dialog.connect(gui.CHANGE, onchange, dialog)
     dialog.open()
 
+
 def cmd_new(value):
-    if app.dirty: _dirty(_cmd_new,value)
-    else: _cmd_new(value)
-    
+    if app.dirty:
+        _dirty(_cmd_new, value)
+    else:
+        _cmd_new(value)
+
+
 def _cmd_new(value):
     dialog = NewDialog()
-    
+
     def onchange(value):
         value.close()
         vv = value.value
         ok = 0
-        try:        
-            width,height,tile_w,tile_h,codes,tiles,klass = int(vv['width'].value),int(vv['height'].value),int(vv['tile_w'].value),int(vv['tile_h'].value),vv['codes'].value,vv['tiles'].value,vv['class'].value
+        try:
+            width, height, tile_w, tile_h, codes, tiles, klass = (
+                int(vv["width"].value),
+                int(vv["height"].value),
+                int(vv["tile_w"].value),
+                int(vv["tile_h"].value),
+                vv["codes"].value,
+                vv["tiles"].value,
+                vv["class"].value,
+            )
             global cfg
-            cfg['fname'] = None
-            cfg['width'] = width
-            cfg['height'] = height
-            cfg['tile_w'] = tile_w
-            cfg['tile_h'] = tile_h
-            cfg['codes'] = codes
-            cfg['tiles'] = tiles
-            cfg['class'] = klass
+            cfg["fname"] = None
+            cfg["width"] = width
+            cfg["height"] = height
+            cfg["tile_w"] = tile_w
+            cfg["tile_h"] = tile_h
+            cfg["codes"] = codes
+            cfg["tiles"] = tiles
+            cfg["class"] = klass
             ok = 1
-        except Exception, v:
-            ErrorDialog("New failed.",v).open()
+        except Exception as v:
+            ErrorDialog("New failed.", v).open()
         if ok:
             raise Restart()
-    
-    dialog.connect(gui.CHANGE,onchange,dialog)
+
+    dialog.connect(gui.CHANGE, onchange, dialog)
     dialog.open()
 
-    
+
 def cmd_open(value):
-    if app.dirty: _dirty(_cmd_open,value)
-    else: _cmd_open(value)
+    if app.dirty:
+        _dirty(_cmd_open, value)
+    else:
+        _cmd_open(value)
+
 
 def _cmd_open(value):
     dialog = OpenDialog()
-    
+
     def onchange(value):
         value.close()
         vv = value.value
         ok = 0
-        
-        try:        
-            
-            fname,tile_w,tile_h,codes,tiles,klass = vv['fname'].value,int(vv['tile_w'].value),int(vv['tile_h'].value),vv['codes'].value,vv['tiles'].value,vv['class'].value
+
+        try:
+            fname, tile_w, tile_h, codes, tiles, klass = (
+                vv["fname"].value,
+                int(vv["tile_w"].value),
+                int(vv["tile_h"].value),
+                vv["codes"].value,
+                vv["tiles"].value,
+                vv["class"].value,
+            )
             global cfg
-            cfg['fname'] = fname
-            cfg['tile_w'] = tile_w
-            cfg['tile_h'] = tile_h
-            cfg['codes'] = codes
-            cfg['tiles'] = tiles
-            cfg['class'] = klass
+            cfg["fname"] = fname
+            cfg["tile_w"] = tile_w
+            cfg["tile_h"] = tile_h
+            cfg["codes"] = codes
+            cfg["tiles"] = tiles
+            cfg["class"] = klass
 
-            
             ok = 1
-        except Exception,v:
-            ErrorDialog("Open failed.",v).open()
-            
-        if ok: raise Restart()
+        except Exception as v:
+            ErrorDialog("Open failed.", v).open()
 
-    
-    dialog.connect(gui.CHANGE,onchange,dialog)
+        if ok:
+            raise Restart()
+
+    dialog.connect(gui.CHANGE, onchange, dialog)
     dialog.open()
 
+
 def cmd_saveas(value):
     dialog = SaveAsDialog()
-    
+
     def onchange(value):
         value.close()
         vv = value.value
-        fname = vv['fname'].value
+        fname = vv["fname"].value
         if len(fname) == 0:
-            ErrorDialog("Save As failed.","File Name too short!").open()
+            ErrorDialog("Save As failed.", "File Name too short!").open()
             return
         global cfg
-        app.fname = cfg['fname'] = fname
+        app.fname = cfg["fname"] = fname
         return cmd_save(None)
-        
-    dialog.connect(gui.CHANGE,onchange,dialog)
+
+    dialog.connect(gui.CHANGE, onchange, dialog)
     dialog.open()
-        
+
+
 def cmd_cut(value):
     cmd_copy(value)
     cmd_delete(value)
 
+
 def cmd_fullscreen(value):
     pygame.display.toggle_fullscreen()
-    
+
+
 def cmd_delete(value):
     app.archive()
-    #app.view.fill((0,0,0,0),app.select)
+    # app.view.fill((0,0,0,0),app.select)
     app.mod(app.select)
-    app.fill(app.select,(0,0,0,0))
+    app.fill(app.select, (0, 0, 0, 0))
     app.vdraw.repaint()
-        
-#NOTE: this function is a temporary HACK, to be replaced
-#with layer editing in the future, maybe.
+
+
+# NOTE: this function is a temporary HACK, to be replaced
+# with layer editing in the future, maybe.
 def cmd_tswitch(value):
     blayer = app.level.blayer
     tlayer = app.level.tlayer
-    for ty in xrange(0,app.level.size[1]):
-        for tx in xrange(0,app.level.size[0]):
+    for ty in range(0, app.level.size[1]):
+        for tx in range(0, app.level.size[0]):
             tmp = blayer[ty][tx]
             blayer[ty][tx] = tlayer[ty][tx]
             tlayer[ty][tx] = tmp
     app.vdraw.repaint()
-    
+
 
 def cmd_fill(value):
     pass
 
+
 def cmd_pick(value):
-    dx,dy = value
-    
+    dx, dy = value
+
     mods = pygame.key.get_mods()
-    
-    
-    if (mods&KMOD_SHIFT) != 0:
-        app.level.view.x += dx*app.vdraw.rect.w/8
-        app.level.view.y += dy*app.vdraw.rect.h/8
+
+    if (mods & KMOD_SHIFT) != 0:
+        app.level.view.x += dx * app.vdraw.rect.w / 8
+        app.level.view.y += dy * app.vdraw.rect.h / 8
         app.vdraw.repaint()
-        #x,y = app.view.get_offset()
-        #x = x + 1*dx
-        #y = y + 1*dy
-        #x = min(max(x,0),app.level_w-app.view_w)
-        #y = min(max(y,0),app.level_h-app.view_h)
-        #app.view = app.level.subsurface((x,y,app.view_w,app.view_h))
-        
-    elif (mods&KMOD_CTRL) != 0:
-        app.level.view.x += dx*app.vdraw.rect.w
-        app.level.view.y += dy*app.vdraw.rect.h
+        # x,y = app.view.get_offset()
+        # x = x + 1*dx
+        # y = y + 1*dy
+        # x = min(max(x,0),app.level_w-app.view_w)
+        # y = min(max(y,0),app.level_h-app.view_h)
+        # app.view = app.level.subsurface((x,y,app.view_w,app.view_h))
+
+    elif (mods & KMOD_CTRL) != 0:
+        app.level.view.x += dx * app.vdraw.rect.w
+        app.level.view.y += dy * app.vdraw.rect.h
         app.vdraw.repaint()
-        #x,y = app.view.get_offset()
-        #x = x + app.view_w*dx
-        #y = y + app.view_h*dy
-        #x = min(max(x,0),app.level_w-app.view_w)
-        #y = min(max(y,0),app.level_h-app.view_h)
-        #app.view = app.level.subsurface((x,y,app.view_w,app.view_h))
-        
-    
+        # x,y = app.view.get_offset()
+        # x = x + app.view_w*dx
+        # y = y + app.view_h*dy
+        # x = min(max(x,0),app.level_w-app.view_w)
+        # y = min(max(y,0),app.level_h-app.view_h)
+        # app.view = app.level.subsurface((x,y,app.view_w,app.view_h))
+
     else:
-        w = app.tiles_w/app.tile_w
-        if app.mode == 'code':
-            n = app.code + dx + dy*w
+        w = app.tiles_w / app.tile_w
+        if app.mode == "code":
+            n = app.code + dx + dy * w
             app.cpicker.set(n)
         else:
-            n = app.tile + dx + dy*w
+            n = app.tile + dx + dy * w
             app.tpicker.set(n)
-        
+
+
 def cmd_mode(value):
     mode = value
     app.mode = mode
 
+
 def cmd_load(value):
-    if app.dirty: _dirty(_cmd_load,value)
-    else: _cmd_load(value)
+    if app.dirty:
+        _dirty(_cmd_load, value)
+    else:
+        _cmd_load(value)
+
 
 def _cmd_load(value):
     if app.fname == None:
-        ErrorDialog("Load failed","Image is untitled.").open()
+        ErrorDialog("Load failed", "Image is untitled.").open()
         return
     raise Restart()
 
-    
+
 def cmd_save(value):
     if app.fname == None:
         return cmd_saveas(value)
     try:
         app.level.tga_save_level(app.fname)
-        cfg_to_ini(['class','codes','tiles','tile_w','tile_h'],app.fname)
+        cfg_to_ini(["class", "codes", "tiles", "tile_w", "tile_h"], app.fname)
         ini_save()
         app.dirty = 0
-    except Exception, v:
-        ErrorDialog("Save failed.",v).open()
+    except Exception as v:
+        ErrorDialog("Save failed.", v).open()
         return
 
-    
+
 import os
+
+
 def cmd_preview(value):
     app.level.tga_save_level("_preview.tga")
     cmd = "python preview.py _preview.tga"
-    print cmd
+    print(cmd)
     os.system(cmd)
-    
+
+
 def cmd_quit(value):
-    if app.dirty: _dirty(_cmd_quit,value)
-    else: _cmd_quit(value)
+    if app.dirty:
+        _dirty(_cmd_quit, value)
+    else:
+        _cmd_quit(value)
+
 
 def _cmd_quit(value):
-    app.top.quit()    
-    
-def cmd_refreshtiles(value):
-    app.load_tiles_and_codes()
+    app.top.quit()
 
 
+def cmd_refreshtiles(value):
+    app.load_tiles_and_codes()
 
 
 menus = [
-    ('File/New',cmd_new,None),
-    ('File/Open',cmd_open,None),
-    ('File/Save',cmd_save,None),
-    ('File/Save As',cmd_saveas,None),
-    ('File/Reload',cmd_load,None),
-    ('File/Preview',cmd_preview,None),
-    ('File/Quit',cmd_quit,None),
-
-    ('Edit/Undo',cmd_undo,None),
-    ('Edit/Cut',cmd_cut,None),
-    ('Edit/Copy',cmd_copy,None),
-    ('Edit/Paste',cmd_paste,None),
-    ('Edit/Delete',cmd_delete,None),
-    ('Edit/Select All',cmd_all,None),
-    ('Edit/Shrink',cmd_shrink,None),
-    #('Edit/Redo',None,None,None),
-    #('Edit/Cut',None,None,None),
-    #('Edit/Fill',cmd_fill,None),
-    
-    ]
+    ("File/New", cmd_new, None),
+    ("File/Open", cmd_open, None),
+    ("File/Save", cmd_save, None),
+    ("File/Save As", cmd_saveas, None),
+    ("File/Reload", cmd_load, None),
+    ("File/Preview", cmd_preview, None),
+    ("File/Quit", cmd_quit, None),
+    ("Edit/Undo", cmd_undo, None),
+    ("Edit/Cut", cmd_cut, None),
+    ("Edit/Copy", cmd_copy, None),
+    ("Edit/Paste", cmd_paste, None),
+    ("Edit/Delete", cmd_delete, None),
+    ("Edit/Select All", cmd_all, None),
+    ("Edit/Shrink", cmd_shrink, None),
+    # ('Edit/Redo',None,None,None),
+    # ('Edit/Cut',None,None,None),
+    # ('Edit/Fill',cmd_fill,None),
+]
 
 keys = [
-    (K_s,cmd_save,None),
-    (K_d,cmd_load,None),
-    (K_p,cmd_preview,None),
-
-    (K_a,cmd_all,None),
-    (K_z,cmd_undo,None),
-    #('Edit/Redo',None,None,None),
-    (K_x,cmd_cut,None),
-    (K_c,cmd_copy,None),
-    (K_v,cmd_paste,None),
-    #('Edit/Cut',None,None,None),
-    (K_DELETE,cmd_delete,None),
-    #(K_f,cmd_fill,None),
-        
-        (K_t,cmd_tswitch,None),
-    
-    (K_F10,cmd_fullscreen,None),
-    
-    (K_UP,cmd_pick,(0,-1)),
-    (K_DOWN,cmd_pick,(0,1)),
-    (K_LEFT,cmd_pick,(-1,0)),
-    (K_RIGHT,cmd_pick,(1,0)),
-    ]
-    
+    (K_s, cmd_save, None),
+    (K_d, cmd_load, None),
+    (K_p, cmd_preview, None),
+    (K_a, cmd_all, None),
+    (K_z, cmd_undo, None),
+    # ('Edit/Redo',None,None,None),
+    (K_x, cmd_cut, None),
+    (K_c, cmd_copy, None),
+    (K_v, cmd_paste, None),
+    # ('Edit/Cut',None,None,None),
+    (K_DELETE, cmd_delete, None),
+    # (K_f,cmd_fill,None),
+    (K_t, cmd_tswitch, None),
+    (K_F10, cmd_fullscreen, None),
+    (K_UP, cmd_pick, (0, -1)),
+    (K_DOWN, cmd_pick, (0, 1)),
+    (K_LEFT, cmd_pick, (-1, 0)),
+    (K_RIGHT, cmd_pick, (1, 0)),
+]
+
 
 tools = [
-    ('tile','tile'),
-    ('bkgr','bkgr'),
-    ('code','code'),
-    ('select','select'),
-    ('eraser','eraser'),
-    ]
+    ("tile", "tile"),
+    ("bkgr", "bkgr"),
+    ("code", "code"),
+    ("select", "select"),
+    ("eraser", "eraser"),
+]
 
-    
-    
 
 class NewDialog(gui.Dialog):
-    def __init__(self,**params):
+    def __init__(self, **params):
         title = gui.Label("New...")
-        
-        doc = html.HTML(globals={'gui':gui,'dialog':self},data="""
+
+        doc = html.HTML(
+            globals={"gui": gui, "dialog": self},
+            data="""
 <form id='form'>
 
 <table>
 
 <tr><td colspan=2>
 
 <table>
@@ -1034,51 +1108,61 @@
 <tr><td align=right>Height: <td><input type='text' size='4' value='%(tile_h)s' name='tile_h'>
 </table>
 
 <tr><td>&nbsp;
 
 <tr><td colspan=2><input type='button' value='Okay' onclick='dialog.send(gui.CHANGE)'> <input type='button' value='Cancel' onclick='dialog.close()'>
 
-</table>"""%ini_to_dict('None'))
-        gui.Dialog.__init__(self,title,doc)
-        
-        self.value = doc['form']
+</table>"""
+            % ini_to_dict("None"),
+        )
+        gui.Dialog.__init__(self, title, doc)
+
+        self.value = doc["form"]
+
 
 class SaveAsDialog(gui.Dialog):
-    def __init__(self,**params):
+    def __init__(self, **params):
         title = gui.Label("Save As...")
-        
-        doc = html.HTML(globals={'gui':gui,'dialog':self},data="""
+
+        doc = html.HTML(
+            globals={"gui": gui, "dialog": self},
+            data="""
 <form id='form'>
 
 <table>
 
 <tr><td colspan=2>File Name: <input type='file' size=20 name='fname' value=''>
 
 <tr><td>&nbsp;
 
 <tr><td colspan=2><input type='button' value='Okay' onclick='dialog.send(gui.CHANGE)'> <input type='button' value='Cancel' onclick='dialog.close()'>
 
-</table>""")
-        gui.Dialog.__init__(self,title,doc)
-        
-        self.value = doc['form']
+</table>""",
+        )
+        gui.Dialog.__init__(self, title, doc)
+
+        self.value = doc["form"]
+
 
 class OpenDialog(gui.Dialog):
-    def __init__(self,**params):
+    def __init__(self, **params):
         title = gui.Label("Open...")
-        
-        def load_vals(fname,form):
-            if not ini.has_section(fname): return
-            
-            for k,v in ini.items(fname):
+
+        def load_vals(fname, form):
+            if not ini.has_section(fname):
+                return
+
+            for k, v in ini.items(fname):
                 if k in form:
                     form[k].value = v
 
-        doc = html.HTML(globals={'load_vals':load_vals,'ini':ini,'gui':gui,'dialog':self},data="""<form id='form'><table>
+        doc = html.HTML(
+            globals={"load_vals": load_vals, "ini": ini, "gui": gui, "dialog": self},
+            data="""<form id='form'><table>
         
         <tr><td align=right>File Name:&nbsp;<td  align=left><input type='file' size=20 name='fname' value='' onchange='load_vals(self.value,form)'>
 
         <tr><td align=right>Level&nbsp;<br>Type:&nbsp;
         <td align=left><input type=radio name='class' value='pgu.tilevid.Tilevid' checked> Tile<br><input type=radio name='class' value='pgu.isovid.Isovid'> Isometric<br><input type=radio name='class' value='pgu.hexvid.Hexvid'> Hexoganol
         
         <tr><td align=right>Tiles:&nbsp;<td align=left><input type='text' size=20 name='tiles' value='%(tiles)s'>
@@ -1088,301 +1172,365 @@
         <tr><td align=right>Tile Height:&nbsp;<td align=left><input type='text' size='4' value='%(tile_h)s' name='tile_h'>
 
 
 <tr><td>&nbsp;
 
 <tr><td colspan=2><input type='button' value='Okay' onclick='dialog.send(gui.CHANGE)'> <input type='button' value='Cancel' onclick='dialog.close()'>
 
-</table>"""%ini_to_dict('None'))
-        gui.Dialog.__init__(self,title,doc)
-        
-        self.value = doc['form']
+</table>"""
+            % ini_to_dict("None"),
+        )
+        gui.Dialog.__init__(self, title, doc)
+
+        self.value = doc["form"]
+
 
 class ErrorDialog(gui.Dialog):
-    def __init__(self,tt,data,**params):
-        title = gui.Label("Error: "+tt)
+    def __init__(self, tt, data, **params):
+        title = gui.Label("Error: " + tt)
         data = str(data)
-        
-        doc = html.HTML(globals={'gui':gui,'dialog':self},data="""
+
+        doc = html.HTML(
+            globals={"gui": gui, "dialog": self},
+            data="""
 <form id='form'>
 
 <table>
 <tr><td><h1>&lt;!&gt;&nbsp;</h1>
-<td>"""+data+"""
+<td>"""
+            + data
+            + """
 <tr><td>&nbsp;
 <tr><td colspan=2><input type='button' value='Okay' onclick='dialog.send(gui.CHANGE);dialog.close()'>
-</table>""")
-        gui.Dialog.__init__(self,title,doc)
-        
-        self.value = doc['form']
+</table>""",
+        )
+        gui.Dialog.__init__(self, title, doc)
+
+        self.value = doc["form"]
+
 
 class DirtyDialog(gui.Dialog):
-    def __init__(self,**params):
+    def __init__(self, **params):
         title = gui.Label("File not yet saved...")
         data = "Your file is not yet saved.<br>Are you sure you want to continue?"
-        
-        doc = html.HTML(globals={'gui':gui,'dialog':self},data="""
+
+        doc = html.HTML(
+            globals={"gui": gui, "dialog": self},
+            data="""
 <form id='form'>
 
 <table>
 <tr><td><h1>&lt;!&gt;&nbsp;</h1>
-<td>"""+data+"""
+<td>"""
+            + data
+            + """
 <tr><td>&nbsp;
 <tr><td colspan=2><input type='button' value='Okay' onclick='dialog.send(gui.CHANGE)'> <input type='button' value='Cancel' onclick='dialog.close()'>
-</table>""")
-        gui.Dialog.__init__(self,title,doc)
-        
-        self.value = doc['form']
+</table>""",
+        )
+        gui.Dialog.__init__(self, title, doc)
+
+        self.value = doc["form"]
 
 
-    
-        
 def init_ini():
     ini.read([ini_fname])
 
+
 def ini_save():
-    f = open(ini_fname,"wb")
+    f = open(ini_fname, "wb")
     ini.write(f)
     f.close()
 
 
 def init_opts():
     ini.read([ini_fname])
-    
-    usage = "usage: %prog level.tga [tiles.tga] [codes.tga] [tile_w] [tile_h]"
-    
-    parser = OptionParser(usage)
-    
-    parser.add_option("-t", "--tiles", dest="tiles",
-        help="filename of the tiles image (level)")
-    parser.add_option("-c", "--codes", dest="codes",
-        help="file name of the codes image (level)")
 
-    parser.add_option("--tw", dest="tile_w", help="tile width (level)", type='int')
-    parser.add_option("--th", dest="tile_h", help="tile height (level)", type='int')
+    usage = "usage: %prog level.tga [tiles.tga] [codes.tga] [tile_w] [tile_h]"
 
-    parser.add_option("--vw", dest="view_w", help="view width (level)", type='int')
-    parser.add_option("--vh", dest="view_h", help="view height (level)", type='int')
-        
-    parser.add_option("--sw", dest="screen_w", help="screen width (app)", type='int')
-    parser.add_option("--sh", dest="screen_h", help="screen height (app)", type='int')
-    parser.add_option("--class",dest="class",help="class (e.g. pgu.tilevid.Tilevid) (level)")
-    parser.add_option("--tile",action="store_const",const="pgu.tilevid.Tilevid",dest="class",help="use pgu.tilevid.Tilevid")
-    parser.add_option("--iso",action="store_const",const="pgu.isovid.Isovid",dest="class",help="use pgu.isovid.Isovid")
-    parser.add_option("--hex",action="store_const",const="pgu.hexvid.Hexvid",dest="class",help="use pgu.hexvid.Hexvid")
-    
-    parser.add_option("--width",dest="width",help="new width (level)",type='int')
-    parser.add_option("--height",dest="height",help="new height (level)",type='int')
+    parser = OptionParser(usage)
 
-    parser.add_option("-d","--defaults",dest="defaults",help="set default settings (image)",action="store_true")
+    parser.add_option(
+        "-t", "--tiles", dest="tiles", help="filename of the tiles image (level)"
+    )
+    parser.add_option(
+        "-c", "--codes", dest="codes", help="file name of the codes image (level)"
+    )
+
+    parser.add_option("--tw", dest="tile_w", help="tile width (level)", type="int")
+    parser.add_option("--th", dest="tile_h", help="tile height (level)", type="int")
+
+    parser.add_option("--vw", dest="view_w", help="view width (level)", type="int")
+    parser.add_option("--vh", dest="view_h", help="view height (level)", type="int")
+
+    parser.add_option("--sw", dest="screen_w", help="screen width (app)", type="int")
+    parser.add_option("--sh", dest="screen_h", help="screen height (app)", type="int")
+    parser.add_option(
+        "--class", dest="class", help="class (e.g. pgu.tilevid.Tilevid) (level)"
+    )
+    parser.add_option(
+        "--tile",
+        action="store_const",
+        const="pgu.tilevid.Tilevid",
+        dest="class",
+        help="use pgu.tilevid.Tilevid",
+    )
+    parser.add_option(
+        "--iso",
+        action="store_const",
+        const="pgu.isovid.Isovid",
+        dest="class",
+        help="use pgu.isovid.Isovid",
+    )
+    parser.add_option(
+        "--hex",
+        action="store_const",
+        const="pgu.hexvid.Hexvid",
+        dest="class",
+        help="use pgu.hexvid.Hexvid",
+    )
+
+    parser.add_option("--width", dest="width", help="new width (level)", type="int")
+    parser.add_option("--height", dest="height", help="new height (level)", type="int")
+
+    parser.add_option(
+        "-d",
+        "--defaults",
+        dest="defaults",
+        help="set default settings (image)",
+        action="store_true",
+    )
 
-    #parser.add_option("-a", "--app", dest="app",
+    # parser.add_option("-a", "--app", dest="app",
     #    help="set application level defaults", action="store_true")
-    
+
     (opts, args) = parser.parse_args()
-    
-    if len(args) not in (0,1,2,3,4,5):
+
+    if len(args) not in (0, 1, 2, 3, 4, 5):
         parser.error("incorrect number of arguments")
-    
-    #parse arguments
+
+    # parse arguments
     if len(args) == 0:
         opts.fname = "None"
     if len(args) > 0:
         opts.fname = args[0]
     if len(args) > 1:
         opts.tiles = args[1]
-    if len(args) in (3,5):
+    if len(args) in (3, 5):
         opts.codes = args[2]
-    if len(args) in (4,5):
-        n = len(args)-2
-        try: opts.tile_w,opts.tile_h = int(args[n]),int(args[n+1])
-        except: parser.error("width and height must be integers")
-        if opts.tile_w < 1 or opts.tile_h < 1: parser.error("width and height must be greater than 0")
-        
+    if len(args) in (4, 5):
+        n = len(args) - 2
+        try:
+            opts.tile_w, opts.tile_h = int(args[n]), int(args[n + 1])
+        except:
+            parser.error("width and height must be integers")
+        if opts.tile_w < 1 or opts.tile_h < 1:
+            parser.error("width and height must be greater than 0")
+
     fname = opts.fname
-    
-    #create all sections
-    for k in [fname,"None","app"]:
+
+    # create all sections
+    for k in [fname, "None", "app"]:
         if not ini.has_section(k):
             ini.add_section(k)
-    
-    #set app level defaults
-    for k,v in [('screen_w',800),('screen_h',600)]:
-        if not ini.has_option('app',k):
-            ini.set('app',k,str(v))
-    
-    #set app level values
-    for k in ['screen_w','screen_h']:
-        if hasattr(opts,k):
-            v = getattr(opts,k)
-            if v != None: ini.set('app',k,str(v))
-
-    #set default defaults
-    for k,v in [('width',40),('height',30),('tile_w',32),('tile_h',32),('tiles','tiles.tga'),('codes','codes.tga'),('class','pgu.tilevid.Tilevid')]:
-        if not ini.has_option('None',k):
-            ini.set('None',k,str(v))
-    
-    #name of keys for normal stuff
-    file_ks = ['class','tiles','codes','width','height','tile_w','tile_h']
-            
-    #set default values
+
+    # set app level defaults
+    for k, v in [("screen_w", 800), ("screen_h", 600)]:
+        if not ini.has_option("app", k):
+            ini.set("app", k, str(v))
+
+    # set app level values
+    for k in ["screen_w", "screen_h"]:
+        if hasattr(opts, k):
+            v = getattr(opts, k)
+            if v != None:
+                ini.set("app", k, str(v))
+
+    # set default defaults
+    for k, v in [
+        ("width", 40),
+        ("height", 30),
+        ("tile_w", 32),
+        ("tile_h", 32),
+        ("tiles", "tiles.tga"),
+        ("codes", "codes.tga"),
+        ("class", "pgu.tilevid.Tilevid"),
+    ]:
+        if not ini.has_option("None", k):
+            ini.set("None", k, str(v))
+
+    # name of keys for normal stuff
+    file_ks = ["class", "tiles", "codes", "width", "height", "tile_w", "tile_h"]
+
+    # set default values
     if opts.defaults:
         for k in file_ks:
-            if hasattr(opts,k):
-                v = getattr(opts,k)
-                if v != None: ini.set('None',k,str(v))
-    
-    #set fname values
+            if hasattr(opts, k):
+                v = getattr(opts, k)
+                if v != None:
+                    ini.set("None", k, str(v))
+
+    # set fname values
     for k in file_ks:
-        if hasattr(opts,k):
-            v = getattr(opts,k)
-            if v != None: ini.set(fname,k,str(v))
-    
-    #save the ini
+        if hasattr(opts, k):
+            v = getattr(opts, k)
+            if v != None:
+                ini.set(fname, k, str(v))
+
+    # save the ini
     ini_save()
-            
-    #convert ini to cfg stuff...
-    ini_to_cfg(['app','None',fname])
-    if fname == 'None': fname = None
-    cfg['fname'] = fname
+
+    # convert ini to cfg stuff...
+    ini_to_cfg(["app", "None", fname])
+    if fname == "None":
+        fname = None
+    cfg["fname"] = fname
+
 
 def ini_to_cfg(sections):
     global cfg
-    ik = ['screen_w','screen_h','tile_w','tile_h','width','height']
+    ik = ["screen_w", "screen_h", "tile_w", "tile_h", "width", "height"]
     for s in sections:
-        for k,v in ini.items(s):
-            if k in ik: v = int(v)
+        for k, v in ini.items(s):
+            if k in ik:
+                v = int(v)
             cfg[k] = v
 
+
 def ini_to_dict(section):
     cfg = {}
-    ik = ['screen_w','screen_h','tile_w','tile_h','width','height']
+    ik = ["screen_w", "screen_h", "tile_w", "tile_h", "width", "height"]
     for s in [section]:
-        for k,v in ini.items(s):
-            if k in ik: v = int(v)
+        for k, v in ini.items(s):
+            if k in ik:
+                v = int(v)
             cfg[k] = v
     return cfg
 
-def cfg_to_ini(ks,section):
-    if not ini.has_section(section): ini.add_section(section)
+
+def cfg_to_ini(ks, section):
+    if not ini.has_section(section):
+        ini.add_section(section)
     for k in ks:
         v = cfg[k]
-        ini.set(section,k,str(v))
+        ini.set(section, k, str(v))
+
 
-        
 def init_gui():
-    #themes = cfg['theme'].split(",")
-#    themes2 = []
-#    for t in themes:
-#        if t[0] == "/" or t[0] == ".": themes2.append(t)
-#        else: themes2.append(dname+"/"+t)
-    #gui.theme.load(themes)
-    #gui.theme.load(['default','tools'])
+    # themes = cfg['theme'].split(",")
+    #    themes2 = []
+    #    for t in themes:
+    #        if t[0] == "/" or t[0] == ".": themes2.append(t)
+    #        else: themes2.append(dname+"/"+t)
+    # gui.theme.load(themes)
+    # gui.theme.load(['default','tools'])
     global top
-    top = gui.Desktop(theme=gui.Theme(['default','tools']))
-    #top.theme.load(['default','tools'])
-
+    top = gui.Desktop(theme=gui.Theme(["default", "tools"]))
+    # top.theme.load(['default','tools'])
 
     pass
 
+
 def init_app():
     global app
     app = _app()
-    
+
     #
     ss = 8
-        
-    #--- top
-    x,y,h = 0,0,0
-        
-    #menus
+
+    # --- top
+    x, y, h = 0, 0, 0
+
+    # menus
     e = gui.Menus(menus)
-    e.rect.w,e.rect.h = e.resize()
-    app.add(e,x,y)
-    x,h = x+e.rect.w,max(h,e.rect.h)
+    e.rect.w, e.rect.h = e.resize()
+    app.add(e, x, y)
+    x, h = x + e.rect.w, max(h, e.rect.h)
     menus_height = e.rect.h
-        
-    #--- row
-    x,y,h = 0,y+h,0
-    
-    #--- vspace
+
+    # --- row
+    x, y, h = 0, y + h, 0
+
+    # --- vspace
     y += ss
-    
-    #--- hspace
+
+    # --- hspace
     x += ss
-    
-    #tools
-    e = gui.Toolbox(tools,1,0,value='tile')#,"icons48")
-    e.rect.w,e.rect.h = e.resize()
-    def _set_mode(value): cmd_mode(value.value)
-    e.connect(gui.CHANGE,_set_mode,e)
-    app.add(e,x,y)
+
+    # tools
+    e = gui.Toolbox(tools, 1, 0, value="tile")  # ,"icons48")
+    e.rect.w, e.rect.h = e.resize()
+
+    def _set_mode(value):
+        cmd_mode(value.value)
+
+    e.connect(gui.CHANGE, _set_mode, e)
+    app.add(e, x, y)
     app.tools = e.tools
-    x,h = x+e.rect.w,max(h,e.rect.h)
+    x, h = x + e.rect.w, max(h, e.rect.h)
     toolbox_width = e.rect.w
-    
-    #--- hspace
+
+    # --- hspace
     x += ss
-    
-    #vdraw
-    dw = app.screen_w - (toolbox_width+app.tiles.get_width()+ss*4)
-    dh = app.screen_h - (menus_height+ss*2)
-    app.view_init(dw,dh)
-    
-    
+
+    # vdraw
+    dw = app.screen_w - (toolbox_width + app.tiles.get_width() + ss * 4)
+    dh = app.screen_h - (menus_height + ss * 2)
+    app.view_init(dw, dh)
+
     e = app.vwrap = vwrap()
     app.vdraw = e.vdraw
-    e.rect.w,e.rect.h = e.resize()
-    app.add(e,x,y)
-    x,h = x+e.rect.w,max(h,e.rect.h)
-    
-    #--- hspace
+    e.rect.w, e.rect.h = e.resize()
+    app.add(e, x, y)
+    x, h = x + e.rect.w, max(h, e.rect.h)
+
+    # --- hspace
     x += ss
-    
-    #tpicker
+
+    # tpicker
     e = app.tpicker = tpicker()
-    e.rect.w,e.rect.h = e.resize()
-    #--- right
-    x = app.screen_w-e.rect.w-ss
-    app.add(e,x,y)
-    x,h = x+e.rect.w,max(h,e.rect.h)
+    e.rect.w, e.rect.h = e.resize()
+    # --- right
+    x = app.screen_w - e.rect.w - ss
+    app.add(e, x, y)
+    x, h = x + e.rect.w, max(h, e.rect.h)
     tpicker_height = e.rect.h
-    
-    #cpicker
-    e = app.cpicker = cpicker()
-    e.rect.w,e.rect.h = e.resize()
-    #--- right
-    x = app.screen_w-e.rect.w-ss
-    app.add(e,x,y+tpicker_height+ss)
-    x,h = x+e.rect.w,max(h,e.rect.h)
-    
 
+    # cpicker
+    e = app.cpicker = cpicker()
+    e.rect.w, e.rect.h = e.resize()
+    # --- right
+    x = app.screen_w - e.rect.w - ss
+    app.add(e, x, y + tpicker_height + ss)
+    x, h = x + e.rect.w, max(h, e.rect.h)
 
+    pygame.key.set_repeat(500, 30)
 
-    pygame.key.set_repeat(500,30)
-    
-    app.screen.fill((255,255,255,255))
+    app.screen.fill((255, 255, 255, 255))
 
 
 def run():
-    top.connect(gui.QUIT,cmd_quit,None)
-    top.connect(pygame.ACTIVEEVENT, cmd_refreshtiles,None)
+    top.connect(gui.QUIT, cmd_quit, None)
+    top.connect(pygame.ACTIVEEVENT, cmd_refreshtiles, None)
 
-    top.init(app,app.screen)
-    app.top=top
+    top.init(app, app.screen)
+    app.top = top
     top.run()
 
+
 def main():
     init_ini()
     init_opts()
     init_gui()
-    
+
     restart = 1
     while restart:
         restart = 0
         try:
             init_app()
             run()
-        except Restart: restart = 1
+        except Restart:
+            restart = 1
+
 
 main()
 # vim: set filetype=python sts=4 sw=4 noet si :
```

### Comparing `zanthor-1.2.3/zanthor/data/levels/test3.tga` & `zanthor-1.2.4a2/zanthor/data/levels/test3.tga`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/menu/x.png` & `zanthor-1.2.4a2/zanthor/data/menu/x.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/menu/read_me.html` & `zanthor-1.2.4a2/zanthor/data/menu/read_me.html`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/menu/map.png` & `zanthor-1.2.4a2/zanthor/data/menu/map.png`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/data/menu/vinque.ttf` & `zanthor-1.2.4a2/zanthor/data/menu/vinque.ttf`

 * *Files identical despite different names*

### Comparing `zanthor-1.2.3/zanthor/castle.py` & `zanthor-1.2.4a2/zanthor/castle.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
 
 to keep the state of the castle.
 
 """
-import random,pprint,copy
+import random, pprint, copy
 
-import effect,steam,explode
+from . import effect, steam, explode
 
 
 import pygame
 from pygame.locals import *
 
-import states
-import isovid
+from . import isovid
+from . import robot
 
-import robot
 
-from pgu import gui
-def dist(a,b):
-    return abs(a[0]-b[0])+abs(a[1]-b[1])
+def dist(a, b):
+    return abs(a[0] - b[0]) + abs(a[1] - b[1])
+
 
 def sign(v):
-    if v == 0: return v
-    return v/abs(v)
+    if v == 0:
+        return v
+    return v // abs(v)
 
-import algo
-from const import *
 
-#from units import *
-import units
-import items
+from . import algo
+from .const import *
 
-import sound_info
+# from units import *
+from . import units
+from . import items
 
+from . import sound_info
 
 
 def iso_facing_to_screen_facing(kx, ky):
     if kx == 0 and ky == -1:
         kx = -1
         ky = -1
 
@@ -64,318 +64,294 @@
 
     elif kx == -1 and ky == 0:
         kx = -1
         ky = 1
     return (kx, ky)
 
 
-
 class CastleSprite(isovid.Sprite):
     def __init__(self, *args, **kwargs):
         isovid.Sprite.__init__(self, *args, **kwargs)
 
         self.unit = units.Castle()
 
-
         self.can_move = True
         self.loop = castle_loop
         self.hit = castle_hit
 
         self.doing = ""
 
         self.frame = 0
 
         # counters for when hitting coal.
         self.last_hit_coal = 0
         self.last_loop = 0
 
         # how long ago we updated steam.
         self.last_update_steam = 0
-        
+
         self.path = []
         self.target = None
 
         self.fire_state = ""
 
         self.direction_dx = 0
         self.direction_dy = 0
         self.last_direction_dy = 0
         self.last_direction_dx = 0
-        
 
     def no_move(self):
         self.can_move = False
 
     def yes_move(self):
         self.can_move = True
 
     def yes_pickup(self, e):
-        print "yes pickup"
+        print("yes pickup")
 
         self.doing = ""
         self.yes_move()
 
         if not hasattr(self.item_tile, "item"):
-            print "WEIRD: tile does not have an item attached?"
-            print self.item_tile
-            print dir(self.item_tile)
+            print("WEIRD: tile does not have an item attached?")
+            print((self.item_tile))
+            print((dir(self.item_tile)))
             return
 
-
-        print self.item_tile.item
+        print((self.item_tile.item))
 
         # if not pickup item, then it's not picked up.
         #  this can happen if coal/water tanks are too small.
         if self.unit.pickup_item(self.item_tile.item):
             item = self.item_tile.item
 
             if item.type & items.ITEM_PART:
                 self.upgrade_something(item.name)
 
-
-
             if not AUTO_PICKUP:
                 # remove the buttons.
-                self.g.app.main_container.remove( self.g.app.question_table )
-
+                self.g.app.main_container.remove(self.g.app.question_table)
 
-            #tw,th = self.g.iso_w,self.g.iso_h
+            # tw,th = self.g.iso_w,self.g.iso_h
             tx, ty = self.item_tile.tx, self.item_tile.ty
-            self.g.set((tx,ty),0)
-
-
+            self.g.set((tx, ty), 0)
 
     def no_pickup(self, e):
-
         if not AUTO_PICKUP:
-            print "no pickup"
-            #self.unit.pickup_item(self.item_sprite)
+            print("no pickup")
+            # self.unit.pickup_item(self.item_sprite)
             self.doing = ""
             self.yes_move()
             # remove the buttons... if they are there.
             try:
-                self.g.app.main_container.remove( self.g.app.question_table )
+                self.g.app.main_container.remove(self.g.app.question_table)
             except ValueError:
                 pass
 
     def check_for_pickup(self, g, t):
-
         self.last_hit_coal += 1
 
         if AUTO_PICKUP:
             self.doing = "deciding on picking up"
             self.item_tile = t
 
             self.yes_pickup("")
         else:
-
             if not self.doing:
-                print "adding button"
-                #s.no_move()
+                print("adding button")
+                # s.no_move()
 
                 self.doing = "deciding on picking up"
                 self.item_tile = t
 
-                #TODO: show the question.
-
+                # TODO: show the question.
 
     def upgrade_something(self, upgrade_what):
-        """ this upgrades something.
-        """
+        """this upgrades something."""
 
-        amount = self.unit.stats['upgrade_amounts'][upgrade_what].cur()
-        self.unit.stats['upgrade_amounts'][upgrade_what].next()
+        amount = self.unit.stats["upgrade_amounts"][upgrade_what].cur()
+        next(self.unit.stats["upgrade_amounts"][upgrade_what])
         self.unit.upgrade_part(upgrade_what, amount)
 
-        #play upgrade sound here.
+        # play upgrade sound here.
         self.g.level.game.sm.Play(sound_info.get_upgrade_sound(upgrade_what))
 
         # update the equipment section
         self.g.level.interface.new_equipment(self.unit.stats)
 
         # say a message about the upgrade.
         self.g.level.interface.new_upgrade_message(upgrade_what)
 
-
-    def event(self, g , e):
-        tw,th = g.iso_w,g.iso_h
+    def event(self, g, e):
+        tw, th = g.iso_w, g.iso_h
         s = self
-        sx,sy = s.rect.centerx/tw,s.rect.centery/th
+        sx, sy = s.rect.centerx // tw, s.rect.centery // th
 
-
-
-        if hasattr(e,'pos'):
-            epos = e.pos[0]-S_VIEW.x,e.pos[1]-S_VIEW.y
-            #print epos
-            #print "sx:%s  sy:%s" % (sx, sy)
-        
-        if e.type is MOUSEBUTTONDOWN and e.button == 3:
-            tx,ty = g.screen_to_tile(epos)
-            #print 'left',tx,ty
-            w,h = g.size
-            if (tx,ty) != (sx,sy) and (tx >= 0 and ty >=0 and tx < w and ty <h):
-                self.target = tx,ty
-                self.path = algo.astar((sx,sy),(tx,ty),g.castle_layer,dist)
-                #print self.path
-            #elif self.doing:
+        if hasattr(e, "pos"):
+            epos = e.pos[0] - S_VIEW.x, e.pos[1] - S_VIEW.y
+            # print epos
+            # print "sx:%s  sy:%s" % (sx, sy)
+
+        if e.type == MOUSEBUTTONDOWN and e.button == 3:
+            tx, ty = g.screen_to_tile(epos)
+            # print 'left',tx,ty
+            w, h = g.size
+            if (tx, ty) != (sx, sy) and (tx >= 0 and ty >= 0 and tx < w and ty < h):
+                self.target = tx, ty
+                self.path = algo.astar((sx, sy), (tx, ty), g.castle_layer, dist)
+                # print self.path
+            # elif self.doing:
             #    self.yes_pickup(e)
-                
-        #print e   
-#        if (e.type is MOUSEBUTTONDOWN and e.button == 3 or 
-#            e.type == JOYBUTTONDOWN and e.button ==JOY_FIRE_BUTTON):
-        if (e.type is MOUSEBUTTONDOWN and e.button == 1):
 
+        # print e
+        #        if (e.type == MOUSEBUTTONDOWN and e.button == 3 or
+        #            e.type == JOYBUTTONDOWN and e.button ==JOY_FIRE_BUTTON):
+        if e.type == MOUSEBUTTONDOWN and e.button == 1:
             # use up some steam in order to fire.
             self.unit.prep_fire()
-                
-        if (e.type is MOUSEBUTTONUP and e.button == 1):
-            tx,ty = g.screen_to_tile(epos)
-            #print 'right',tx,ty
-            
-            x,y = g.screen_to_tile(epos)
-            cannon_pressure = self.unit.try_do_fire()
-
-            tw,th = g.iso_w,g.iso_h
-            cball_new(g,self.rect,(x*tw+tw/2,y*th+th/2), self.unit.stats['Damage'],cannon_pressure*1.5)
-
-
-
 
+        if e.type == MOUSEBUTTONUP and e.button == 1:
+            tx, ty = g.screen_to_tile(epos)
+            # print 'right',tx,ty
 
+            x, y = g.screen_to_tile(epos)
+            cannon_pressure = self.unit.try_do_fire()
 
+            tw, th = g.iso_w, g.iso_h
+            cball_new(
+                g,
+                self.rect,
+                (x * tw + tw // 2, y * th + th // 2),
+                self.unit.stats["Damage"],
+                cannon_pressure * 1.5,
+            )
 
         if e.type == JOYBUTTONDOWN:
             pass
 
-        #if self.direction_dy != 0:
+        # if self.direction_dy != 0:
         #    self.last_direction_dy = self.direction_dy
-        #if self.direction_dx != 0:
+        # if self.direction_dx != 0:
         #    self.last_direction_dx = self.direction_dx
 
         if e.type == JOYAXISMOTION:
             if e.axis == 0:
                 if round(e.value) < 0:
                     self.direction_dx = -1
                     self.last_direction_dx = self.direction_dx
                     self.last_direction_dy = self.direction_dy
-                    #print "less than"
+                    # print "less than"
                 elif round(e.value) > 0:
                     self.direction_dx = 1
                     self.last_direction_dx = self.direction_dx
                     self.last_direction_dy = self.direction_dy
-                    #print "greater than"
+                    # print "greater than"
                 else:
-                    #print "nothing!"
+                    # print "nothing!"
                     self.last_direction_dx = self.direction_dx
                     self.direction_dx = 0
 
-
-
             if e.axis == 1:
                 if round(e.value) < 0:
                     self.direction_dy = -1
                     self.last_direction_dy = self.direction_dy
                     self.last_direction_dx = self.direction_dx
                 elif round(e.value) > 0:
                     self.direction_dy = 1
                     self.last_direction_dy = self.direction_dy
                     self.last_direction_dx = self.direction_dx
                 else:
                     self.last_direction_dy = self.direction_dy
                     self.direction_dy = 0
-                
 
-        if (e.type == JOYBUTTONUP and e.button ==JOY_FIRE_BUTTON):
+        if e.type == JOYBUTTONUP and e.button == JOY_FIRE_BUTTON:
             pass
 
             if 0:
-
                 self.direction_dx = 0
                 self.direction_dy = 0
-                tx,ty = g.screen_to_tile(epos)
-                x,y = g.screen_to_tile(epos)
-
+                tx, ty = g.screen_to_tile(epos)
+                x, y = g.screen_to_tile(epos)
 
                 if self.unit.try_fire():
-                    #print (x*tw+tw/2,y*th+th/2)
-                    cball_new(g,s.rect,(x*tw+tw/2,y*th+th/2), self.unit.stats['Damage'])
-
-
-
-        if (e.type == JOYBUTTONDOWN and e.button ==JOY_FIRE_BUTTON):
+                    # print (x*tw+tw/2,y*th+th/2)
+                    cball_new(
+                        g,
+                        s.rect,
+                        (x * tw + tw // 2, y * th + th // 2),
+                        self.unit.stats["Damage"],
+                    )
 
+        if e.type == JOYBUTTONDOWN and e.button == JOY_FIRE_BUTTON:
             # TODO: find out which way we are facing.
             # TODO: fire in facing direction.
             self.fire_state = "firing"
 
+        if (e.type == JOYBUTTONDOWN and e.button == JOY_FIRE_BUTTON) or (
+            e.type == KEYDOWN and e.key in [K_f, K_LCTRL, K_RCTRL, K_SPACE]
+        ):
+            sx, sy = self.rect.centerx // tw, self.rect.centery // th
 
-        if ((e.type == JOYBUTTONDOWN and e.button ==JOY_FIRE_BUTTON) or
-            (e.type == KEYDOWN and e.key in [K_f, K_LCTRL, K_RCTRL, K_SPACE])):
-
-            sx,sy = self.rect.centerx/tw, self.rect.centery/th
-
-            #print "last dx:%s:   last dy:%s:" % (self.last_direction_dx, self.last_direction_dy)
-            #print "sx:%s:   sy:%s:" % (sx, sy)
+            # print "last dx:%s:   last dy:%s:" % (self.last_direction_dx, self.last_direction_dy)
+            # print "sx:%s:   sy:%s:" % (sx, sy)
 
-            
-            
             self.unit.prep_fire()
-            
-        if ((e.type == JOYBUTTONUP and e.button ==JOY_FIRE_BUTTON) or
-            (e.type == KEYUP and e.key in [K_f, K_LCTRL, K_RCTRL, K_SPACE])):
+
+        if (e.type == JOYBUTTONUP and e.button == JOY_FIRE_BUTTON) or (
+            e.type == KEYUP and e.key in [K_f, K_LCTRL, K_RCTRL, K_SPACE]
+        ):
             facing_x, facing_y = (self.last_direction_dx, self.last_direction_dy)
-            facing_x, facing_y = iso_facing_to_screen_facing(self.last_direction_dx, self.last_direction_dy)
+            facing_x, facing_y = iso_facing_to_screen_facing(
+                self.last_direction_dx, self.last_direction_dy
+            )
 
             x = (5 * facing_x) + sx
             y = (5 * facing_y) + sy
 
-            #x,y = g.screen_to_tile(epos)
+            # x,y = g.screen_to_tile(epos)
             cannon_pressure = self.unit.try_do_fire()
 
-            tw,th = g.iso_w,g.iso_h
-            cball_new(g,self.rect,(x*tw+tw/2,y*th+th/2), self.unit.stats['Damage'],cannon_pressure)
-
-
+            tw, th = g.iso_w, g.iso_h
+            cball_new(
+                g,
+                self.rect,
+                (x * tw + tw // 2, y * th + th // 2),
+                self.unit.stats["Damage"],
+                cannon_pressure,
+            )
 
             # use up some steam in order to fire.
-            #if self.unit.try_fire():
+            # if self.unit.try_fire():
             #    cball_new(g,s.rect,(x*tw+tw/2,y*th+th/2), self.unit.stats['Damage'])
 
-
-
-
-        
         if self.doing:
             if (
-                (e.type == KEYDOWN and self.doing and e.key == K_RETURN) or
-                (e.type == KEYDOWN and self.doing and e.key == K_SPACE) or
-                (e.type == MOUSEBUTTONDOWN and e.button == 3) or 
-                (e.type == JOYBUTTONDOWN and e.button == JOY_PICKUP_BUTTON)):
+                (e.type == KEYDOWN and self.doing and e.key == K_RETURN)
+                or (e.type == KEYDOWN and self.doing and e.key == K_SPACE)
+                or (e.type == MOUSEBUTTONDOWN and e.button == 3)
+                or (e.type == JOYBUTTONDOWN and e.button == JOY_PICKUP_BUTTON)
+            ):
                 self.yes_pickup(e)
 
-
         if e.type == KEYUP:
-
             if e.key in [K_UP, K_w]:
                 self.last_direction_dy = self.direction_dy
                 self.direction_dy = 0
             elif e.key in [K_DOWN, K_s]:
                 self.last_direction_dy = self.direction_dy
                 self.direction_dy = 0
             elif e.key in [K_LEFT, K_a]:
                 self.last_direction_dx = self.direction_dx
                 self.direction_dx = 0
             elif e.key in [K_RIGHT, K_d]:
                 self.last_direction_dx = self.direction_dx
                 self.direction_dx = 0
 
-
         # some testing keys.
         if e.type == KEYDOWN:
-
             if e.key in [K_UP, K_w]:
                 self.direction_dy = -1
                 self.last_direction_dy = self.direction_dy
                 self.last_direction_dx = self.direction_dx
             elif e.key in [K_DOWN, K_s]:
                 self.direction_dy = 1
                 self.last_direction_dy = self.direction_dy
@@ -385,34 +361,31 @@
                 self.last_direction_dx = self.direction_dx
                 self.last_direction_dy = self.direction_dy
             elif e.key in [K_RIGHT, K_d]:
                 self.direction_dx = 1
                 self.last_direction_dx = self.direction_dx
                 self.last_direction_dy = self.direction_dy
 
-
-
             if e.key == K_KP_PLUS:
-                self.unit.stats['Speed'] += 1
+                self.unit.stats["Speed"] += 1
 
             elif e.key == K_KP_MINUS:
-                self.unit.stats['Speed'] -= 1
+                self.unit.stats["Speed"] -= 1
 
             elif e.key == K_h:
                 self.unit.hit(2)
 
             elif e.key == K_r:
-                #tx, ty = self.item_tile.tx, self.item_tile.ty
+                # tx, ty = self.item_tile.tx, self.item_tile.ty
                 # drop rubble test.
-                tx,ty = self.rect.centerx/tw, self.rect.centery/th
+                tx, ty = self.rect.centerx // tw, self.rect.centery // th
 
-                self.g.set((tx,ty),7)
+                self.g.set((tx, ty), 7)
 
             if UPGRADE_FUN:
-
                 if e.key == K_1:
                     self.upgrade_something("UpEngine Efficiency")
                 elif e.key == K_2:
                     self.upgrade_something("UpEngine Speed")
                 elif e.key == K_3:
                     self.upgrade_something("UpCannon Balls")
                 elif e.key == K_4:
@@ -423,157 +396,131 @@
                     self.upgrade_something("UpSteam Tank")
                 elif e.key == K_7:
                     self.upgrade_something("UpWater Tank")
                 elif e.key == K_8:
                     self.upgrade_something("UpCoal Tank")
 
                 elif e.key in [K_9, K_0]:
-                    pprint.pprint( self.unit.stats )
+                    pprint.pprint(self.unit.stats)
 
-                    
             if e.key == K_y:
-                #get_savable_upgrade_amounts()
-                print self.backup_castle()
+                # get_savable_upgrade_amounts()
+                print((self.backup_castle()))
             if e.key == K_u:
-                #get_savable_upgrade_amounts()
-                print self.reset_castle()
+                # get_savable_upgrade_amounts()
+                print((self.reset_castle()))
             if e.key == K_z:
-                #get_savable_upgrade_amounts()
-                print self.unit.stats
+                # get_savable_upgrade_amounts()
+                print((self.unit.stats))
 
-
-            #elif e.key == K_s:
+            # elif e.key == K_s:
             #    r = self.unit.try_use_steam(1)
             #    print "tried to use steam :%s:" % r
 
-
     def reset_castle(self):
-        """ resets the castle stats to the backup.
-        """
+        """resets the castle stats to the backup."""
 
         if self.g.level.game.backup_castle_stats:
-            print "before"
-            print self.unit.stats
+            print("before")
+            print((self.unit.stats))
             self.unit.stats = copy.deepcopy(self.g.level.game.backup_castle_stats)
-            print "after"
-            print self.unit.stats
+            print("after")
+            print((self.unit.stats))
             if hasattr(self.g, "level"):
                 if hasattr(self.g.level, "interface"):
                     self.g.level.interface.new_equipment(self.unit.stats)
 
-
     def backup_castle(self):
-        """ backs the castle stats up.
-        """
+        """backs the castle stats up."""
         self.g.level.game.backup_castle_stats = copy.deepcopy(self.unit.stats)
 
 
-
-
-
-def castle_new(g,t,value):
+def castle_new(g, t, value):
     g.clayer[t.ty][t.tx] = 0
-    s = CastleSprite(g.images['castle'],t.rect)
+    s = CastleSprite(g.images["castle"], t.rect)
     s.g = g
-    #print "castle"
-    #print t.rect
-    s.groups = g.string2groups('castle')
-    s.agroups = g.string2groups('robot')
-    
-    s.effect = steam.Effect(32,1)
+    # print "castle"
+    # print t.rect
+    s.groups = g.string2groups("castle")
+    s.agroups = g.string2groups("robot")
+
+    s.effect = steam.Effect(32, 1)
 
     g.castle = s
 
     g.sprites.append(s)
     if g.level.game.should_restore_stats:
         pass
-        #TODO:
+        # TODO:
         s.reset_castle()
-        s.unit.stats['Health'] = 10.
+        s.unit.stats["Health"] = 10.0
 
-        
-        
-    
 
+def castle_hit(g, s, a):
+    # screams of smushing go here.
+    a.state = "dead"
 
-def castle_hit(g,s,a):
-    
-    #screams of smushing go here.
-    a.state = 'dead'
-        
     g.level.game.sm.Play(random.choice(sound_info.squish))
 
-    
-    #print g
-    #print dir(s)
-    #print a
-
-    #print "castle hit"
+    # print g
+    # print dir(s)
+    # print a
 
+    # print "castle hit"
 
     # test for collision between castle sprite and other types...
-    # if the sprite has an item then pop up a dialog asking the 
+    # if the sprite has an item then pop up a dialog asking the
     #  player if they want to pick it up.
 
     # the player shouldn't be able to move when being asked about coal.
 
-    #NOTE: this is only a todo if we stop the castle from moving 
+    # NOTE: this is only a todo if we stop the castle from moving
     #  whilst picking things up.
-    #TODO: after picking not picking up the item, how long before asking again?
+    # TODO: after picking not picking up the item, how long before asking again?
     #  maybe put a timer in there for 3. seconds before asking again.
 
-
     # store the item sprite to pick up on click.
-    #s.item_sprite = a
-    #s.last_hit_coal += 1
-    
-
-
+    # s.item_sprite = a
+    # s.last_hit_coal += 1
 
 
-
-
-def castle_loop(g,s):
-    #print "castle loop"
+def castle_loop(g, s):
+    # print "castle loop"
 
     s.unit.loop()
 
     # update the steam every second.
-    #print g.level.game.ticks_passed
-
-    #tw,th = g.iso_w,g.iso_h
+    # print g.level.game.ticks_passed
 
-    tw,th = g.iso_w,g.iso_h
-    sx,sy = s.rect.centerx/tw,s.rect.centery/th
+    # tw,th = g.iso_w,g.iso_h
 
+    tw, th = g.iso_w, g.iso_h
+    sx, sy = s.rect.centerx // tw, s.rect.centery // th
 
     s.last_update_steam += g.level.game.elapsed_time
 
     if s.can_move:
-        #s.rect.x += 1
+        # s.rect.x += 1
 
-        speed = int(s.unit.stats['Speed'])
+        speed = int(s.unit.stats["Speed"])
 
-        kx,ky = 0,0
+        kx, ky = 0, 0
 
         # put in the joystick movement.
         if kx == 0:
             kx += s.direction_dx
-            #s.dx = 0
+            # s.dx = 0
         if ky == 0:
             ky += s.direction_dy
-            #s.dy = 0
-
+            # s.dy = 0
 
         # HACK: we do a little invert here.  because hex movement is weird.
         # we try to make up joy go up on screen.
 
         if 1:
-
-
             if kx == 0 and ky == -1:
                 kx = -1
                 ky = -1
 
             elif kx == 0 and ky == 1:
                 kx = 1
                 ky = 1
@@ -596,301 +543,297 @@
                 kx = 1
                 ky = -1
 
             elif kx == -1 and ky == 0:
                 kx = -1
                 ky = 1
 
-        #if ky == 1 and kx == 0:
+        # if ky == 1 and kx == 0:
         #    kx = 1
         #    ky = 1
 
-        #print kx,ky
+        # print kx,ky
 
         keyboard_or_joy_speed_slow = 1
-        #if ky == 0 or kx == 0:
-#        if (kx,ky) != (0,0):
-#
-#            if (kx,ky) == (1,1) or (kx,ky) == (-1,-1) or kx == 0 or ky == 0:
-#                keyboard_or_joy_speed_slow = 0
+        # if ky == 0 or kx == 0:
+        #        if (kx,ky) != (0,0):
+        #
+        #            if (kx,ky) == (1,1) or (kx,ky) == (-1,-1) or kx == 0 or ky == 0:
+        #                keyboard_or_joy_speed_slow = 0
 
-
-
-        if (kx,ky) != (0,0):
+        if (kx, ky) != (0, 0):
             keyboard_or_joy = 1
 
-            tx,ty = sx+kx,sy+ky
+            tx, ty = sx + kx, sy + ky
             if g.castle_layer[ty][tx] == 0:
-                s.path = [(tx,ty)]
+                s.path = [(tx, ty)]
 
-            
-        dx,dy = 0,0
+        dx, dy = 0, 0
         path = s.path
         while len(path) > 0:
             g.auto_scroll = True
-            bx,by = path[0]
-            if (bx,by) == (sx,sy): 
+            bx, by = path[0]
+            if (bx, by) == (sx, sy):
                 path.pop(0)
                 continue
-            dx,dy = bx-sx,by-sy
-            #v = 4
-            #s.rect.x += sign(dx)*v
-            #s.rect.y += sign(dy)*v
-            dx,dy = sign(dx),sign(dy)
+            dx, dy = bx - sx, by - sy
+            # v = 4
+            # s.rect.x += sign(dx)*v
+            # s.rect.y += sign(dy)*v
+            dx, dy = sign(dx), sign(dy)
             break
 
         if keyboard_or_joy_speed_slow:
-            speed = int(round(speed / 2.))
+            speed = int(round(speed // 2.0))
 
         if dx != 0 or dy != 0:
-            #HACK: so i can move this guy ! :)
+            # HACK: so i can move this guy ! :)
             if 1 or s.unit.try_move():
-                s.rect.x += dx*speed
-                s.rect.y += dy*speed
-                
+                s.rect.x += dx * speed
+                s.rect.y += dy * speed
+
             if dx < 0:
-                s.setimage(g.images['castle.left'])
+                s.setimage(g.images["castle.left"])
             if dx > 0:
-                s.setimage(g.images['castle.right'])
+                s.setimage(g.images["castle.right"])
 
-        #s.rect.clamp_ip(g.view)
+        # s.rect.clamp_ip(g.view)
     if s.last_hit_coal:
-        #print "last_hit_coal, last"
+        # print "last_hit_coal, last"
         if s.last_hit_coal == s.last_loop:
             s.last_loop = 0
             s.last_hit_coal = 0
             s.no_pickup("")
         else:
             s.last_loop = s.last_hit_coal
 
-    #okay, so the robots are scared to death of you...
+    # okay, so the robots are scared to death of you...
     a = s
     for r in g.robots:
-        rx,ry = r.x,r.y
-        ax,ay = a.rect.x,a.rect.y
-        dx,dy = rx-ax,ry-ay
-        dist = (dx*dx+dy*dy)**0.5
-        if dist and dist < 32*3:
-            r.min = min(r._min,r.min+12.0)
+        rx, ry = r.x, r.y
+        ax, ay = a.rect.x, a.rect.y
+        dx, dy = rx - ax, ry - ay
+        dist = (dx * dx + dy * dy) ** 0.5
+        if dist and dist < 32 * 3:
+            r.min = min(r._min, r.min + 12.0)
             inc = 16.0
-            x,y = rx + dx*inc/dist, ry + dy*inc/dist
-            robot.robot_shove(g,r,(x,y))
-
-
-    s.frame +=1
+            x, y = rx + dx * inc // dist, ry + dy * inc // dist
+            robot.robot_shove(g, r, (x, y))
 
+    s.frame += 1
 
 
-def cball_new(g,pos,dest, damage = 1.0,pressure=16):
-    #g.level.game.sm.Play(random.choice(sound_info.cannon))
-    #g.level.game.sm.Play(sound_info.cannon.nextone())
+def cball_new(g, pos, dest, damage=1.0, pressure=16):
+    # g.level.game.sm.Play(random.choice(sound_info.cannon))
+    # g.level.game.sm.Play(sound_info.cannon.nextone())
 
     if pressure < 9:
         g.level.game.sm.Play(sound_info.cannon[0], wait=3)
-        print "cannon 1 sound"
+        print("cannon 1 sound")
     elif pressure >= 9 and pressure < 15:
         g.level.game.sm.Play(sound_info.cannon[1], wait=3)
-        print "cannon 2 sound"
+        print("cannon 2 sound")
     elif pressure >= 15 and pressure < 25:
         g.level.game.sm.Play(sound_info.cannon[2], wait=3)
-        print "cannon 3 sound"
+        print("cannon 3 sound")
     elif pressure >= 25:
-        print "cannon 4 sound,  two cannon 3 sounds played at once."
+        print("cannon 4 sound,  two cannon 3 sounds played at once.")
         g.level.game.sm.Play(sound_info.cannon[2], wait=3)
         g.level.game.sm.Play(sound_info.cannon[2], wait=3)
 
-
-
     # Here we use a different graphic for the cannon balls depending on Damage.
-    
 
-    if damage <= 1.:
-        img_name = 'cball'
+    if damage <= 1.0:
+        img_name = "cball"
         num_steam, num_steam_add = 20, 5
-    elif damage > 1. and damage < 4.:
-        img_name = 'cball2'
+    elif damage > 1.0 and damage < 4.0:
+        img_name = "cball2"
         num_steam, num_steam_add = 30, 10
-    elif damage >= 4. and damage < 6.:
-        img_name = 'cball3'
+    elif damage >= 4.0 and damage < 6.0:
+        img_name = "cball3"
         num_steam, num_steam_add = 25, 15
-    elif damage >= 6. and damage < 8.:
-        img_name = 'cball4'
+    elif damage >= 6.0 and damage < 8.0:
+        img_name = "cball4"
         num_steam, num_steam_add = 35, 20
-    elif damage >= 8. and damage < 10.:
-        img_name = 'cball4'
+    elif damage >= 8.0 and damage < 10.0:
+        img_name = "cball4"
         num_steam, num_steam_add = 42, 23
-    elif damage >= 10.:
-        img_name = 'cball4'
+    elif damage >= 10.0:
+        img_name = "cball4"
         num_steam, num_steam_add = 50, 25
 
-    
-    s = isovid.Sprite(g.images[img_name],pos)
+    s = isovid.Sprite(g.images[img_name], pos)
 
     # we assign the damage that is done by this cannon ball.
     s.damage = damage
     s.num_steam, s.num_steam_add = num_steam, num_steam_add
-    
 
     s.frame = 0
 
     g.sprites.append(s)
     s.loop = cball_loop
     s.hit = cball_hit
     s.groups = g.string2groups("cball")
-    s.agroups = g.string2groups("robot,cannon") #,factory,truck,cannon")
-    
-    #s.rect, s._rect
-    
-    dx,dy = dest[0]-s.rect.x,dest[1]-s.rect.y
-    dist = (dx*dx+dy*dy)**0.5
-    if dist <= 0: return 
+    s.agroups = g.string2groups("robot,cannon")  # ,factory,truck,cannon")
+
+    # s.rect, s._rect
+
+    dx, dy = dest[0] - s.rect.x, dest[1] - s.rect.y
+    dist = (dx * dx + dy * dy) ** 0.5
+    if dist <= 0:
+        return
     v = float(pressure)
-    s.vx, s.vy = dx*v/dist,dy*v/dist
+    s.vx, s.vy = dx * v // dist, dy * v // dist
     s.vz = -5
     s.z = 0
 
     # we add a steam effect for when firing the cannon ball.
     #   It's steamyness is different depending on the damage of the cannon.
     rect = pygame.Rect(s.rect)
-    rect.x += s.vx*2
-    rect.y += s.vy *2
-    effect.effect_new(g,rect,steam.Effect(num_steam,num_steam_add,12,0,(255,255,255)),20)
-    
-    
-def cball_loop(g,s):
+    rect.x += s.vx * 2
+    rect.y += s.vy * 2
+    effect.effect_new(
+        g, rect, steam.Effect(num_steam, num_steam_add, 12, 0, (255, 255, 255)), 20
+    )
+
+
+def cball_loop(g, s):
     try:
         s.rect.x += s.vx
-    except AttributeError: 
+    except AttributeError:
         return
 
     s.rect.y += s.vy
     s.z += s.vz
     s.vz += 1
     if s.vz == 8:
         if s in g.sprites:
             g.sprites.remove(s)
 
         img_name = get_hole_for_damage(s.damage)
-        g.bkgr_blit(g.images[img_name],(s.rect.centerx,s.rect.centery))
-
+        g.bkgr_blit(g.images[img_name], (s.rect.centerx, s.rect.centery))
 
         g.level.game.sm.Play(sound_info.hitground.nextone(), wait=3)
-        
+
         if HOLES_ARE_TILES:
-            tw,th = g.iso_w,g.iso_h
-            tx,ty = s.rect.centerx/tw,s.rect.centery/th
-            
-            dirs = [(0,0)]
+            tw, th = g.iso_w, g.iso_h
+            tx, ty = s.rect.centerx // tw, s.rect.centery // th
+
+            dirs = [(0, 0)]
             if HOLES_ARE_TILES > 1:
-                dirs.extend([(-1,0),(1,0),(0,1),(0,-1)])
-            for dx,dy in dirs:
-                xx,yy = tx+dx,ty+dy
-                v = g.get((xx,yy))
-                if v in (0,7):
-                    g.set((xx,yy),30)
-        
+                dirs.extend([(-1, 0), (1, 0), (0, 1), (0, -1)])
+            for dx, dy in dirs:
+                xx, yy = tx + dx, ty + dy
+                v = g.get((xx, yy))
+                if v in (0, 7):
+                    g.set((xx, yy), 30)
 
-        #ss = effect.effect_new(g,s.rect,steam.Effect(20,20,8,0,(117,110,94)),20)
+        # ss = effect.effect_new(g,s.rect,steam.Effect(20,20,8,0,(117,110,94)),20)
         num_steam, num_steam_add = s.num_steam, s.num_steam_add
-        ss = effect.effect_new(g,s.rect,steam.Effect(int(num_steam*2), int(num_steam_add*2),num_steam_add,0,(0,0,0)),20)
+        ss = effect.effect_new(
+            g,
+            s.rect,
+            steam.Effect(
+                int(num_steam * 2), int(num_steam_add * 2), num_steam_add, 0, (0, 0, 0)
+            ),
+            20,
+        )
         ss.z = 8
-        
-        print 'gahhh'
+
+        print("gahhh")
         a = s
         for r in g.robots:
-            rx,ry = r.x,r.y
-            ax,ay = a.rect.x,a.rect.y
-            dx,dy = rx-ax,ry-ay
-            dist = (dx*dx+dy*dy)**0.5
-            if dist and dist < 32*4:
-                r.min = min(r._min,r.min+12.0)
+            rx, ry = r.x, r.y
+            ax, ay = a.rect.x, a.rect.y
+            dx, dy = rx - ax, ry - ay
+            dist = (dx * dx + dy * dy) ** 0.5
+            if dist and dist < 32 * 4:
+                r.min = min(r._min, r.min + 12.0)
                 inc = 31.0
-                x,y = rx + dx*inc/dist, ry + dy*inc/dist
-                robot.robot_shove(g,r,(x,y))
+                x, y = rx + dx * inc // dist, ry + dy * inc // dist
+                robot.robot_shove(g, r, (x, y))
 
-            if dist < 32*3: #1.5:
-                r.state = 'dead'
+            if dist < 32 * 3:  # 1.5:
+                r.state = "dead"
 
-    #print s.rect
+    # print s.rect
     s.frame += 1
-    
+
+
 class SpriteBlast:
     def __init__(self):
-        self.e1 = explode.Effect(64,16)
-        #self.e2 = steam.Effect(128,32,24,0)
-        self.e2 = steam.Effect(120,40,16,0)
-        
-    def loop(self,pos):
+        self.e1 = explode.Effect(64, 16)
+        # self.e2 = steam.Effect(128,32,24,0)
+        self.e2 = steam.Effect(120, 40, 16, 0)
+
+    def loop(self, pos):
         self.e1.loop(pos)
         self.e2.loop(pos)
-        
-    def paint(self,screen,origin):
-        self.e1.paint(screen,origin)
-        self.e2.paint(screen,origin)
 
-def cball_hit(g,a,b):
+    def paint(self, screen, origin):
+        self.e1.paint(screen, origin)
+        self.e2.paint(screen, origin)
+
 
+def cball_hit(g, a, b):
     # we just destroy 'robots'... aka peasants.  cball keeps going.
-    if hasattr(b,'type') and b.type == 'robot':
+    if hasattr(b, "type") and b.type == "robot":
         if b in g.sprites:
-            #g.sprites.remove(b)
-            b.state = 'dead'
+            # g.sprites.remove(b)
+            b.state = "dead"
     else:
-        return cball_hit_old(g,a,b)
+        return cball_hit_old(g, a, b)
+
 
 def get_hole_for_damage(damage):
-    if damage <= 1.:
-        img_name = 'hole'
-    elif damage > 1. and damage < 4.:
-        img_name = 'hole2'
-    elif damage >= 4. and damage < 6.:
-        img_name = 'hole3'
-    elif damage >= 6. and damage < 8.:
-        img_name = 'hole4'
-    elif damage >= 8. and damage < 10.:
-        img_name = 'hole4'
-    elif damage >= 10.:
-        img_name = 'hole4'
+    if damage <= 1.0:
+        img_name = "hole"
+    elif damage > 1.0 and damage < 4.0:
+        img_name = "hole2"
+    elif damage >= 4.0 and damage < 6.0:
+        img_name = "hole3"
+    elif damage >= 6.0 and damage < 8.0:
+        img_name = "hole4"
+    elif damage >= 8.0 and damage < 10.0:
+        img_name = "hole4"
+    elif damage >= 10.0:
+        img_name = "hole4"
     return img_name
 
 
-def cball_hit_old(g,a_cannon_ball,b):
-
-    ss = effect.effect_new(g,b.rect,steam.Effect(60,20,4,0),20)
-
+def cball_hit_old(g, a_cannon_ball, b):
+    ss = effect.effect_new(g, b.rect, steam.Effect(60, 20, 4, 0), 20)
 
     # lets hit the unit, and see if it dies.
     if b.unit.hit(a_cannon_ball.damage):
-
         g.level.game.sm.Play(sound_info.destroyenemy.nextone())
 
-#         if b.unit.name == "factory":
-#             g.level.game.state = states.NextLevel(g.level.game, g.level.game.state)
-#             print "you won!"
-#             return
+        #         if b.unit.name == "factory":
+        #             g.level.game.state = states.NextLevel(g.level.game, g.level.game.state)
+        #             print "you won!"
+        #             return
 
         if b in g.sprites:
             g.sprites.remove(b)
 
         img_name = get_hole_for_damage(a_cannon_ball.damage)
 
-        g.bkgr_blit(g.images[img_name],(a_cannon_ball.rect.centerx,a_cannon_ball.rect.centery))
-        
-        #do an explosion here...
-        #that looks like...
-        ss = effect.effect_new(g,b.rect,SpriteBlast(),20)
+        g.bkgr_blit(
+            g.images[img_name], (a_cannon_ball.rect.centerx, a_cannon_ball.rect.centery)
+        )
+
+        # do an explosion here...
+        # that looks like...
+        ss = effect.effect_new(g, b.rect, SpriteBlast(), 20)
     else:
         # we only play the hit sound if the thing doesn't die?
         g.level.game.sm.Play(sound_info.hitenemy.nextone())
-        
 
     try:
         g.sprites.remove(a_cannon_ball)
     except ValueError:
         # already removed??? yeah that happens :)
         # if the ball hits more than one tile
         pass
 
-
-    print "hit!", b.unit.name
+    print(("hit!", b.unit.name))
     pass
-
```

### Comparing `zanthor-1.2.3/zanthor/interface.py` & `zanthor-1.2.4a2/zanthor/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,654 +3,577 @@
 import os
 import random
 
 
 import pygame.draw
 
 
-import util
-from pgu import gui
+from . import util
+from .pgu import gui
 
-#import pgu.html
-import html
+try:
+    # import pgu.html
+    from . import html
+except ImportError:
+    # a fake html write function.
+    class __html(object):
+        def write(self, *args):
+            pass
 
+    html = __html()
 
-from const import *
-import units
+from .const import *
+from . import units
 
-import messages
+from . import messages
 
-import cyclic_list
+from . import cyclic_list
 import pygame.sprite
 
-#class 
-
+# class
 
 
 class StatsDraw:
-    """ draws the stats health, coal, water, steam on the left side of interface.
-    """
+    """draws the stats health, coal, water, steam on the left side of interface."""
+
     def __init__(self):
         self.frames = 0
         self.update_frame = {}
-        self.update_which = cyclic_list.cyclic_list(['Health', 'Coal', 'Water', 'Steam'])
+        self.update_which = cyclic_list.cyclic_list(
+            ["Health", "Coal", "Water", "Steam"]
+        )
         self.frames_health = 0
 
     def draw_img(self, screen, min, max, current, color, where_rect, astat):
-        """ eg. min - 0, max - 100, current - 45
-        """
+        """eg. min - 0, max - 100, current - 45"""
 
         # this draws an image cutting off the top bit
 
-        height = (((max - min) / (max * 1.0)) * current)
+        height = ((max - min) // (max * 1.0)) * current
         graph_height = where_rect.h
-        height = (graph_height / (max * 1.0)) * current
+        height = (graph_height // (max * 1.0)) * current
 
         clip_rect = pygame.Rect(where_rect)
         clip_rect.x = 0
         clip_rect.y = 0
         clip_rect.h = int(height)
 
         diff = where_rect.h - int(height)
         clip_rect.y += diff
 
         im_border = None
 
         if astat == "Health":
             # show the heart every pulse every half a second or so.
-            if self.frames_health > (FPS / 2):
-                k = 'heart.png'
+            if self.frames_health > (FPS // 2):
+                k = "heart.png"
                 if self.frames_health > FPS:
                     self.frames_health = 0
             else:
-                k = 'heart_pulse.png' 
+                k = "heart_pulse.png"
 
             im = self.images[k]
 
-            if not self.images.has_key(k + "laplacian"):
+            if k + "laplacian" not in self.images:
                 self.images[k + "laplacian"] = pygame.transform.laplacian(im)
 
             im_border = self.images[k + "laplacian"]
 
             c = clip_rect.clip(im.get_rect())
             if not c.width and not c.height:
                 s = None
             else:
-                print im,c
+                print((im, c))
                 s = im.subsurface(c)
 
         else:
-            raise "not implemented for this stat"
-        
+            raise ValueError("not implemented for this stat")
+
         draw_rect = pygame.Rect(where_rect)
         draw_rect.y += diff
         if s:
             screen.blit(s, draw_rect)
-            
+
         if im_border:
             screen.blit(im_border, where_rect)
-            
-        return where_rect
-
-
-
 
+        return where_rect
 
     def draw_rect(self, screen, min, max, current, color, where_rect):
-        """ eg. min - 0, max - 100, current - 45
-        """
+        """eg. min - 0, max - 100, current - 45"""
         draw_rect = pygame.Rect(where_rect)
 
-        height = (((max - min) / (max * 1.0)) * current)
-        
+        height = ((max - min) // (max * 1.0)) * current
+
         graph_height = draw_rect.h
 
-        height = (graph_height / (max * 1.0)) * current
+        height = (graph_height // (max * 1.0)) * current
 
         draw_rect.h = int(height)
         draw_rect.y += where_rect.h - draw_rect.h
 
-        #draw_rect = multr( dxdy, draw_rect)
+        # draw_rect = multr( dxdy, draw_rect)
 
         s = screen.subsurface(draw_rect)
         s.fill(color)
         return where_rect
 
-
     def update_stats(self, screen, stats, robots, max_robots):
-    #def update_stats(self, screen, stats):
-        #print stats
-        #print max_robots
+        # def update_stats(self, screen, stats):
+        # print stats
+        # print max_robots
 
-        #return []
+        # return []
 
-        self.interface.dirty['left_background'] = 1
+        self.interface.dirty["left_background"] = 1
         self.interface.update_left_background(screen)
 
-        stat_rect={}
-        stat_rect['Health'] = S_HEALTH
-        stat_rect['Coal'] = S_COAL
-        stat_rect['Water'] = S_WATER
-        stat_rect['Steam'] = S_STEAM
-        stat_rect['CannonPressure'] = S_CANNON_PRESSURE
-
-        stat_color={}
-        stat_color['Health'] = (255,0,0)
-        stat_color['Coal'] = (0,0,0)
-        stat_color['Water'] = (0,0,255)
-        stat_color['Steam'] = (200,200,200)
-        stat_color['CannonPressure'] = (100,100,200)
-
-
+        stat_rect = {}
+        stat_rect["Health"] = S_HEALTH
+        stat_rect["Coal"] = S_COAL
+        stat_rect["Water"] = S_WATER
+        stat_rect["Steam"] = S_STEAM
+        stat_rect["CannonPressure"] = S_CANNON_PRESSURE
+
+        stat_color = {}
+        stat_color["Health"] = (255, 0, 0)
+        stat_color["Coal"] = (0, 0, 0)
+        stat_color["Water"] = (0, 0, 255)
+        stat_color["Steam"] = (200, 200, 200)
+        stat_color["CannonPressure"] = (100, 100, 200)
 
         updates = []
         update_thisone = self.update_which.nextone()
 
-        for astat in ['Health', 'Coal', 'Water', 'Steam', 'CannonPressure']:
+        for astat in ["Health", "Coal", "Water", "Steam", "CannonPressure"]:
             # update cannon pressure every frame.  Spread the others out.
-            if not (astat in [update_thisone, 'CannonPressure']):
+            if not (astat in [update_thisone, "CannonPressure"]):
                 continue
 
-
             where_rect = stat_rect[astat]
             color = stat_color[astat]
-            min =0
+            min = 0
             max = int(stats["Max" + astat])
             current = int(stats[astat])
-            #print where_rect
+            # print where_rect
 
-            #only draw the screen where the rectangle will be drawn.
+            # only draw the screen where the rectangle will be drawn.
             if 0:
                 c = screen.get_clip()
                 screen.set_clip(where_rect)
-                screen.blit( self.images["background_status_left.png"], S_STATUS)
+                screen.blit(self.images["background_status_left.png"], S_STATUS)
                 screen.set_clip(c)
 
-            if astat in ['Health']:
+            if astat in ["Health"]:
                 r = self.draw_img(screen, min, max, current, color, where_rect, astat)
             else:
                 r = self.draw_rect(screen, min, max, current, color, where_rect)
             updates.append(r)
 
-
-
         # robots.
         if 1:
             where_rect = S_PEASANTS_REMAINING
-#             color = (200,200,40)
-#             min =0
-#             max = max_robots
-#             current = int(len(robots))
-# 
-#             updates = []
-#             r = self.draw_rect(screen, min, max, current, color, where_rect)
-            
-            
+            #             color = (200,200,40)
+            #             min =0
+            #             max = max_robots
+            #             current = int(len(robots))
+            #
+            #             updates = []
+            #             r = self.draw_rect(screen, min, max, current, color, where_rect)
+
             # top right corner remaining 'robots' are shown.
-            
+
             if self.robots_update:
                 r = where_rect
                 sc = screen.subsurface(where_rect)
-                sc.fill((0,0,0))
+                sc.fill((0, 0, 0))
                 img = self.robots_image
-                w = sc.get_width()-img.get_width()
-                h = sc.get_height()-img.get_height()
-                
-                for n in xrange(0,self.robots_total):
-                    sc.blit(img,(random.randrange(0,w),random.randrange(0,h)))
+                w = sc.get_width() - img.get_width()
+                h = sc.get_height() - img.get_height()
 
+                for n in range(0, int(self.robots_total)):
+                    sc.blit(img, (random.randrange(0, w), random.randrange(0, h)))
 
-            
                 updates.append(r)
 
-
         self.frames_health += 1
         self.frames += 1
         return updates
 
 
-
-    
 class Interface:
-    
     def __init__(self):
-        """
-        """
+        """ """
 
         self.frames = 0
         self.message = messages.generate()
         self.last_message = ""
-        
-        self.message_font = pygame.font.Font(data_dir("menu","vinque.ttf"),20)
-        self.equipment_message_font = pygame.font.Font(data_dir("menu","vinque.ttf"),14)
+
+        self.message_font = pygame.font.Font(data_dir("menu", "vinque.ttf"), 20)
+        self.equipment_message_font = pygame.font.Font(
+            data_dir("menu", "vinque.ttf"), 14
+        )
 
         self.stats = {}
         self.stats_draw = StatsDraw()
         self.stats_draw.interface = self
 
         self.equipment_last_message = ""
         self.equipment_message = ""
 
-
     def loop(self):
-        
         self.frames += 0
 
-
     def load(self):
-        """ loads the graphics/sounds/resources needed.
-        """
-
-        images_needed = ["health_overlay.png", 
-                         "coal_overlay.png",
-                         "water_overlay.png",
-                         "steam_overlay.png",
-                         "background_status_left.png",
-                         "background_bottom.png",
-                         "background_illustration.png",
-                         "background_equipment.png",
-                         "background_buttons.png",
-                         "background_messages.png",
-
-                         "button_save.png",
-                         "button_load.png",
-                         "button_quit.png",
-                         "button_news.png",
-
-                         "button_save_rollover.png",
-                         "button_load_rollover.png",
-                         "button_quit_rollover.png",
-                         "button_news_rollover.png",
-
-                         "button_save_down.png",
-                         "button_load_down.png",
-                         "button_quit_down.png",
-                         "button_news_down.png",
-                         "heart.png",
-                         "heart_pulse.png",
+        """loads the graphics/sounds/resources needed."""
 
-                        ]
+        images_needed = [
+            "health_overlay.png",
+            "coal_overlay.png",
+            "water_overlay.png",
+            "steam_overlay.png",
+            "background_status_left.png",
+            "background_bottom.png",
+            "background_illustration.png",
+            "background_equipment.png",
+            "background_buttons.png",
+            "background_messages.png",
+            "button_save.png",
+            "button_load.png",
+            "button_quit.png",
+            "button_news.png",
+            "button_save_rollover.png",
+            "button_load_rollover.png",
+            "button_quit_rollover.png",
+            "button_news_rollover.png",
+            "button_save_down.png",
+            "button_load_down.png",
+            "button_quit_down.png",
+            "button_news_down.png",
+            "heart.png",
+            "heart_pulse.png",
+        ]
         self.images = {}
         self.stats_draw.images = self.images
 
         for i in images_needed:
             image_path = data_dir("gfx", i)
-            print image_path
+            print(image_path)
             if os.path.exists(image_path):
                 self.images[i] = pygame.image.load(image_path)
                 if i in ["heart.png", "heart_pulse.png"]:
                     self.images[i] = self.images[i].convert_alpha()
                 else:
                     self.images[i] = self.images[i].convert()
             else:
                 self.images[i] = None
 
-
         def scale_images(images):
             screen_size = pygame.display.get_surface().get_size()
-            #scaler = pygame.transform.smoothscale
+            # scaler = pygame.transform.smoothscale
             scaler = pygame.transform.scale
             new_images = {}
 
-            orig_size = 640,480
-            for i,surf in images.items():
+            orig_size = 640, 480
+            for i, surf in list(images.items()):
                 if images[i]:
                     r = surf.get_rect()
                     size_scale = util.scale_rect(r, orig_size, screen_size)[2:]
 
-                    new_images[i] = scaler( surf, size_scale)
+                    new_images[i] = scaler(surf, size_scale)
                 else:
                     new_images[i] = surf
             return new_images
 
         self.images = scale_images(self.images)
 
-
-        self.bkgrb = pygame.Surface((S_BOTTOM_MESSAGES.w, S_BOTTOM_MESSAGES.h) )
+        self.bkgrb = pygame.Surface((S_BOTTOM_MESSAGES.w, S_BOTTOM_MESSAGES.h))
         self.bkgrb = self.bkgrb.convert_alpha()
-        self.bkgrb.fill((0,0,0, 70))
-
+        self.bkgrb.fill((0, 0, 0, 70))
 
         self.dirty = {}
         d = self.dirty
 
-        d['messages'] = 1
-        d['bottom_background'] = 1
-        d['left_background'] = 1
-        d['background_equipment'] = 1
-        d['background_illustration'] = 1
-        d['background_buttons'] = 1
-        d['background_messages'] = 1
-        d['equipment_words'] = 1
-        d[''] = 1
-
-
-
-
+        d["messages"] = 1
+        d["bottom_background"] = 1
+        d["left_background"] = 1
+        d["background_equipment"] = 1
+        d["background_illustration"] = 1
+        d["background_buttons"] = 1
+        d["background_messages"] = 1
+        d["equipment_words"] = 1
+        d[""] = 1
 
     def event(self, g, e):
         pass
 
-        #TODO: handle button clicks.
+        # TODO: handle button clicks.
         if e.type == MOUSEBUTTONDOWN:
-            x,y = e.pos
-            print x,y
+            x, y = e.pos
+            print((x, y))
 
             if S_BUTTONS_SAVE.collidepoint(x, y):
-                print "save"
+                print("save")
 
             if S_BUTTONS_LOAD.collidepoint(x, y):
-                print "load"
+                print("load")
 
             if S_BUTTONS_QUIT.collidepoint(x, y):
-                print "quit"
+                print("quit")
 
             if S_BUTTONS_NEWS.collidepoint(x, y):
-                print "news"
+                print("news")
         if e.type == KEYDOWN:
             if e.key == K_m:
-                print "ASDFSADF"
+                print("ASDFSADF")
                 self.new_random_message()
 
-
-
     def new_stats(self, stats):
-        """ draws the stats with new values.
-        """
-
-
+        """draws the stats with new values."""
 
     def new_random_message(self):
         self.last_message = self.message
         self.message = messages.generate()
         self.message = self.message.replace("ZANTHOR", "<b>ZANTHOR</b>")
         self.message = self.message.replace("Zanthor", "<b>ZANTHOR</b>")
         self.message = self.message.replace("zanthor", "<b>ZANTHOR</b>")
-        self.dirty['messages'] = 1
-        self.dirty['background_messages'] = 1
-
+        self.dirty["messages"] = 1
+        self.dirty["background_messages"] = 1
 
     def new_upgrade_message(self, upgrade_what):
         if upgrade_what:
             self.last_message = self.message
             self.message = messages.generate_upgrade_message(upgrade_what)
-        self.dirty['messages'] = 1
-        self.dirty['background_messages'] = 1
-
-
-
-
-
+        self.dirty["messages"] = 1
+        self.dirty["background_messages"] = 1
 
     def update_messages(self, screen):
-        """
-        """
+        """ """
 
         # the messages are the same... no need to update.
-        if not self.dirty['messages']:
+        if not self.dirty["messages"]:
             if self.message == self.last_message:
-                self.dirty['messages'] = 0
+                self.dirty["messages"] = 0
                 return []
 
-        if self.dirty['messages']:
-            self.dirty['messages'] = 0
+        if self.dirty["messages"]:
+            self.dirty["messages"] = 0
 
-            font = self.message_font #pygame.font.Font(None, 18)
+            font = self.message_font  # pygame.font.Font(None, 18)
             rect = S_MESSAGES
             rect2 = pygame.Rect(S_MESSAGES)
             rect2.x -= 1
             rect2.y += 1
 
             aa = 0
-            #color = (0x55,0xff,0x55) #(80,80,80)
-            color = (0xff,0x55,0x55) #(80,80,80)
-            color2 = (0,0,0) #(80,80,80)
+            # color = (0x55,0xff,0x55) #(80,80,80)
+            color = (0xFF, 0x55, 0x55)  # (80,80,80)
+            color2 = (0, 0, 0)  # (80,80,80)
 
-            bgcolor = (0,0,0,0)
+            bgcolor = (0, 0, 0, 0)
             s = screen
-            #screen.blit(self.bkgrb, S_MESSAGES)
+            # screen.blit(self.bkgrb, S_MESSAGES)
 
-            #pgu.html.render(font,rect,text,aa,color,bgcolor)
-            html.write(s,font,rect2,self.message,aa,color2)
-            html.write(s,font,rect,self.message,aa,color)
+            # pgu.html.render(font,rect,text,aa,color,bgcolor)
+            html.write(s, font, rect2, self.message, aa, color2)
+            html.write(s, font, rect, self.message, aa, color)
 
             return [rect]
         else:
             return []
 
-
-
-
-
-
     def update_bottom_background(self, screen):
-        if self.dirty['bottom_background']:
-            self.dirty['bottom_background'] = 0
-            screen.blit( self.images["background_bottom.png"], S_BOTTOM )
-
+        if self.dirty["bottom_background"]:
+            self.dirty["bottom_background"] = 0
+            screen.blit(self.images["background_bottom.png"], S_BOTTOM)
 
             return [S_BOTTOM]
         else:
             return []
 
     def update_left_background(self, screen):
-        if self.dirty['left_background']:
-            #FIXME: HACK: TODO: this should be 0 when stats update properly.
-            self.dirty['left_background'] = 0
-            screen.blit( self.images["background_status_left.png"], S_STATUS)
+        if self.dirty["left_background"]:
+            # FIXME: HACK: TODO: this should be 0 when stats update properly.
+            self.dirty["left_background"] = 0
+            screen.blit(self.images["background_status_left.png"], S_STATUS)
             return [S_STATUS]
         else:
             return []
 
-
-
     def new_equipment(self, stats):
         self.equipment_last_message = self.equipment_message
         self.equipment_message = "<br><br>"
 
         for upword in units.upgrade_words:
-            self.equipment_message += "%s/%s " % (stats['upgrade_amounts'][upword].idx, 5)
-            self.equipment_message += "" + upword.replace("Up","") + "<br>"
-            #TODO: HACK: fix up 5 to be the maximum for that level.
-
-        self.dirty['equipment_words'] = 1
-        self.dirty['background_equipment'] = 1
-
+            self.equipment_message += "%s/%s " % (
+                stats["upgrade_amounts"][upword].idx,
+                5,
+            )
+            self.equipment_message += "" + upword.replace("Up", "") + "<br>"
+            # TODO: HACK: fix up 5 to be the maximum for that level.
 
+        self.dirty["equipment_words"] = 1
+        self.dirty["background_equipment"] = 1
 
     def update_background_equipment(self, screen):
-        if self.dirty['background_equipment']:
-            self.dirty['background_equipment'] = 0
-            screen.blit( self.images["background_equipment.png"], S_ITEMS)
+        if self.dirty["background_equipment"]:
+            self.dirty["background_equipment"] = 0
+            screen.blit(self.images["background_equipment.png"], S_ITEMS)
             return [S_ITEMS]
         else:
             return []
 
-
     def update_equipment_words(self, screen):
-        """
-        """
+        """ """
 
         # the messages are the same... no need to update.
-        if not self.dirty['equipment_words']:
+        if not self.dirty["equipment_words"]:
             if self.equipment_message == self.equipment_last_message:
-                self.dirty['equipment_words'] = 0
+                self.dirty["equipment_words"] = 0
                 return []
 
-        if self.dirty['equipment_words']:
-            self.dirty['equipment_words'] = 0
+        if self.dirty["equipment_words"]:
+            self.dirty["equipment_words"] = 0
 
-            font = self.equipment_message_font#pygame.font.Font(None, 18)
+            font = self.equipment_message_font  # pygame.font.Font(None, 18)
             rect = S_ITEMS
             rect2 = pygame.Rect(S_ITEMS)
             rect2.x -= 1
             rect2.y += 1
 
             aa = 0
-            color = (0x55,0xff,0x55) #(80,80,80)
-            color2 = (0,0,0)
-            bgcolor = (0,0,0,0)
+            color = (0x55, 0xFF, 0x55)  # (80,80,80)
+            color2 = (0, 0, 0)
+            bgcolor = (0, 0, 0, 0)
             s = screen
 
-            #pgu.html.render(font,rect,text,aa,color,bgcolor)
-            html.write(s,font,rect2,self.equipment_message,aa,color2)
-            html.write(s,font,rect,self.equipment_message,aa,color)
+            # pgu.html.render(font,rect,text,aa,color,bgcolor)
+            html.write(s, font, rect2, self.equipment_message, aa, color2)
+            html.write(s, font, rect, self.equipment_message, aa, color)
 
             return [rect]
         else:
             return []
 
-
     def update_background_illustration(self, screen):
-        if self.dirty['background_illustration']:
-            self.dirty['background_illustration'] = 0
-            screen.blit( self.images["background_illustration.png"], S_ROBOT)
-            
+        if self.dirty["background_illustration"]:
+            self.dirty["background_illustration"] = 0
+            screen.blit(self.images["background_illustration.png"], S_ROBOT)
+
             return [S_ROBOT]
         else:
             return []
 
-
-
     def update_background_buttons(self, screen):
-        if self.dirty['background_buttons']:
-            self.dirty['background_buttons'] = 0
+        if self.dirty["background_buttons"]:
+            self.dirty["background_buttons"] = 0
             s = screen.subsurface(S_BUTTONS)
             surf = self.images["background_bottom.png"]
 
-            screen.blit( surf, S_BUTTONS, S_BOTTOM_BUTTONS)
+            screen.blit(surf, S_BUTTONS, S_BOTTOM_BUTTONS)
             return [S_BUTTONS]
         else:
             return []
 
-
     def update_background_buttons(self, screen):
-        if self.dirty['background_messages']:
-            self.dirty['background_messages'] = 0
+        if self.dirty["background_messages"]:
+            self.dirty["background_messages"] = 0
             surf = self.images["background_bottom.png"]
 
-            screen.blit( surf, S_MESSAGES, S_BOTTOM_MESSAGES)
+            screen.blit(surf, S_MESSAGES, S_BOTTOM_MESSAGES)
             return [S_MESSAGES]
         else:
             return []
 
-
-
     def update(self, tv, screen):
-        """ returns a list of rects.
-        """
-
+        """returns a list of rects."""
 
         if self.equipment_message == "":
             self.new_equipment(tv.castle.unit.stats)
 
-
         updates = []
 
-
         # temporary interface boxes.
         if 0:
             s = screen.subsurface(S_HEALTH)
-            s.fill((255,0,0))
+            s.fill((255, 0, 0))
             updates.append(S_HEALTH)
 
             s = screen.subsurface(S_COAL)
-            s.fill((0,0,0))
+            s.fill((0, 0, 0))
             updates.append(S_COAL)
 
             s = screen.subsurface(S_WATER)
-            s.fill((0,0,255))
+            s.fill((0, 0, 255))
             updates.append(S_WATER)
 
             s = screen.subsurface(S_STEAM)
-            s.fill((200,200,200))
+            s.fill((200, 200, 200))
             updates.append(S_STEAM)
 
+        updates.extend(self.update_bottom_background(screen))
+        updates.extend(self.update_left_background(screen))
 
-        updates.extend( self.update_bottom_background(screen) )
-        updates.extend( self.update_left_background(screen) )
-
-        updates.extend( self.update_background_buttons(screen) )
-        updates.extend( self.update_background_illustration(screen) )
-        updates.extend( self.update_background_equipment(screen) )
-
-
-        updates.extend( self.update_background_buttons(screen) )
-
+        updates.extend(self.update_background_buttons(screen))
+        updates.extend(self.update_background_illustration(screen))
+        updates.extend(self.update_background_equipment(screen))
+
+        updates.extend(self.update_background_buttons(screen))
+
+        # updates.extend( self.update_status_left(screen) )
+        # updates.extend( self.update_background_equipment(screen) )
+        # updates.extend( self.update_(screen) )
 
-
-        #updates.extend( self.update_status_left(screen) )
-        #updates.extend( self.update_background_equipment(screen) )
-        #updates.extend( self.update_(screen) )
-        
         if 0:
-            screen.blit( self.images["background_status_left.png"], S_STATUS)
+            screen.blit(self.images["background_status_left.png"], S_STATUS)
             updates.append(S_STATUS)
 
-
-            screen.blit( self.images["background_equipment.png"], S_ITEMS)
+            screen.blit(self.images["background_equipment.png"], S_ITEMS)
             updates.append(S_ITEMS)
 
-
-            screen.blit( self.images["background_illustration.png"], S_ROBOT)
+            screen.blit(self.images["background_illustration.png"], S_ROBOT)
             updates.append(S_ROBOT)
 
-
-        #s = screen.subsurface(S_MESSAGES)
-        #s.fill((0,200,0))
+        # s = screen.subsurface(S_MESSAGES)
+        # s.fill((0,200,0))
 
         m = self.update_messages(screen)
         updates.extend(m)
 
-
-
-
         ew = self.update_equipment_words(screen)
         updates.extend(ew)
 
-
-        stats_rects = self.stats_draw.update_stats(screen, self.tv.castle.unit.stats, self.tv.robots, self.max_robots)
+        stats_rects = self.stats_draw.update_stats(
+            screen, self.tv.castle.unit.stats, self.tv.robots, self.max_robots
+        )
         updates.extend(stats_rects)
 
+        # s = screen.subsurface(S_ROBOT)
+        # s.fill((200,200,200))
+        # updates.append(S_ROBOT)
+
+        # s = screen.subsurface(S_ITEMS)
+        # s.fill((250,250,250))
+        # updates.append(S_ITEMS)
 
-        #s = screen.subsurface(S_ROBOT)
-        #s.fill((200,200,200))
-        #updates.append(S_ROBOT)
-
-        #s = screen.subsurface(S_ITEMS)
-        #s.fill((250,250,250))
-        #updates.append(S_ITEMS)
-
-        #s = screen.subsurface(S_BUTTONS)
-        #s.fill((150,150,200))
+        # s = screen.subsurface(S_BUTTONS)
+        # s.fill((150,150,200))
 
         if 0:
             s = screen.subsurface(S_BUTTONS_SAVE)
-            s.fill((50,50,20))
+            s.fill((50, 50, 20))
             s = screen.subsurface(S_BUTTONS_LOAD)
-            s.fill((50,50,20))
+            s.fill((50, 50, 20))
             s = screen.subsurface(S_BUTTONS_QUIT)
-            s.fill((50,50,200))
+            s.fill((50, 50, 200))
             s = screen.subsurface(S_BUTTONS_NEWS)
-            s.fill((50,150,200))
-
+            s.fill((50, 150, 200))
 
             updates.append(S_BUTTONS)
 
-
-        #print updates
+        # print updates
 
         return updates
 
 
-
-
-
-
-
-
-
-if __name__=="__main__":
+if __name__ == "__main__":
     pass
-
-
-
```

### Comparing `zanthor-1.2.3/zanthor/truck.py` & `zanthor-1.2.4a2/zanthor/truck.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,121 @@
-import isovid
-import algo
+from . import isovid
+from . import algo
 
-from const import *
-from units import CoalTruck
+from .const import *
+from .units import CoalTruck
 
 
-
-def truck_new(g,t,v):
-    print 'trucks disabled'
+def truck_new(g, t, v):
+    print("trucks disabled")
     return
     g.clayer[t.ty][t.tx] = 0
-    s = isovid.Sprite(g.images['truck'],t.rect)
-    
+    s = isovid.Sprite(g.images["truck"], t.rect)
+
     s.frame = 0
 
     g.sprites.append(s)
     s.loop = truck_loop
     s.hit = truck_hit
     s.groups = g.string2groups("truck")
-    s.agroups= g.string2groups("castle")
-    
-    s.origin = t.tx,t.ty
-    s.state = 'init'
+    s.agroups = g.string2groups("castle")
+
+    s.origin = t.tx, t.ty
+    s.state = "init"
     s.unit = CoalTruck()
 
 
-def dist(a,b):
-    return abs(a[0]-b[0])+abs(a[1]-b[1])
+def dist(a, b):
+    return abs(a[0] - b[0]) + abs(a[1] - b[1])
+
 
 def sign(v):
-    if v == 0: return v
-    return v/abs(v)
-    
-def truck_loop(g,s):
+    if v == 0:
+        return v
+    return v / abs(v)
+
+
+def truck_loop(g, s):
     s.unit.loop()
 
     s.frame += 1
-    
-    tw,th = g.iso_w,g.iso_h
-    ww,hh = g.size
-    sx,sy = s.rect.centerx/tw,s.rect.centery/th
-    if s.state == 'init':
-        best_s,best_d = None,65535
+
+    tw, th = g.iso_w, g.iso_h
+    ww, hh = g.size
+    sx, sy = s.rect.centerx / tw, s.rect.centery / th
+    if s.state == "init":
+        best_s, best_d = None, 65535
         for ss in g.sprites:
-            if hasattr(ss,'type') and ss.type == 'factory':
-                fx,fy = ss.rect.centerx/tw,ss.rect.centery/th
-                dst = dist((sx,sy),(fx,fy))
+            if hasattr(ss, "type") and ss.type == "factory":
+                fx, fy = ss.rect.centerx / tw, ss.rect.centery / th
+                dst = dist((sx, sy), (fx, fy))
                 if dst < best_d:
-                    best_s,best_d = ss,dst
+                    best_s, best_d = ss, dst
         s.factory = best_s
-        s.state = 'search'
+        s.state = "search"
         return
-                
-    
-                
-    if s.state == 'search':
+
+    if s.state == "search":
         coals = []
-        for y in xrange(0,ww):
-            for x in xrange(0,hh):
-                if g.tlayer[y][x] == 1: #HACK: if is coal
-                    coals.append((x,y))
+        for y in range(0, ww):
+            for x in range(0, hh):
+                if g.tlayer[y][x] == 1:  # HACK: if is coal
+                    coals.append((x, y))
         if len(coals) == 0:
-            s.state = 'wait'
+            s.state = "wait"
             return
-        
-        best,best_d = None,65535
-        fx,fy = s.factory.rect.centerx/tw,s.factory.rect.centery/th
-        for cx,cy in coals:
-            dst = dist((cx,cy),(fx,fy))
+
+        best, best_d = None, 65535
+        fx, fy = s.factory.rect.centerx / tw, s.factory.rect.centery / th
+        for cx, cy in coals:
+            dst = dist((cx, cy), (fx, fy))
             if dst < best_d:
-                best,best_d = (cx,cy),dst
-            
-        cx,cy = best
-        s.target = cx,cy
-        s.path = algo.astar((sx,sy),(cx,cy),g.truck_layer,dist)
-        s.state = 'coal'
-                    
-    #once a second check if some coal has appeared...
-    if s.state == 'wait':
-        if s.frame%FPS == 0:
-            s.state = 'search'
+                best, best_d = (cx, cy), dst
+
+        cx, cy = best
+        s.target = cx, cy
+        s.path = algo.astar((sx, sy), (cx, cy), g.truck_layer, dist)
+        s.state = "coal"
+
+    # once a second check if some coal has appeared...
+    if s.state == "wait":
+        if s.frame % FPS == 0:
+            s.state = "search"
         return
-        
-        
-    if s.state == 'coal':
-        fx,fy = s.target
-        n = g.tlayer[fy][fx] 
-        if n != 1: #HACK: coal?
-            s.state = 'search'
+
+    if s.state == "coal":
+        fx, fy = s.target
+        n = g.tlayer[fy][fx]
+        if n != 1:  # HACK: coal?
+            s.state = "search"
             return
-        if (sx,sy) == s.target:
+        if (sx, sy) == s.target:
             s.coal = 1
-            g.set((sx,sy),0)
-            
-            fx,fy = s.factory.rect.centerx/tw,s.factory.rect.centery/th
-            s.target = fx,fy
-            s.path = algo.astar((sx,sy),(fx,fy),g.truck_layer,dist)
-            s.state = 'factory'
-        
-    if s.state == 'factory':
-        if (sx,sy) == s.target:
+            g.set((sx, sy), 0)
+
+            fx, fy = s.factory.rect.centerx / tw, s.factory.rect.centery / th
+            s.target = fx, fy
+            s.path = algo.astar((sx, sy), (fx, fy), g.truck_layer, dist)
+            s.state = "factory"
+
+    if s.state == "factory":
+        if (sx, sy) == s.target:
             s.coal = 0
-            #NOTE: give the coal to the factory here....
-            s.state = 'search'
+            # NOTE: give the coal to the factory here....
+            s.state = "search"
             return
-    
+
     path = s.path
     while len(path) > 1:
-        bx,by = path[1]
-        if (bx,by) == (sx,sy): 
+        bx, by = path[1]
+        if (bx, by) == (sx, sy):
             path.pop(0)
             continue
-        dx,dy = bx-sx,by-sy
+        dx, dy = bx - sx, by - sy
         v = 4
-        s.rect.x += sign(dx)*v
-        s.rect.y += sign(dy)*v
+        s.rect.x += sign(dx) * v
+        s.rect.y += sign(dy) * v
         break
-        
 
-        
-            
-    
- 
 
-def truck_hit(g,a,b):
+def truck_hit(g, a, b):
     pass
```

### Comparing `zanthor-1.2.3/zanthor/fire.py` & `zanthor-1.2.4a2/zanthor/fire.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,111 +1,110 @@
 import pygame
 from pygame.locals import *
 import random
 
-from pgu import timer
+from .pgu import timer
 
 rr = random.randrange
 
+
 class Part:
-    def __init__(self,pos):
-        self.pos = pygame.Rect(pos[0],pos[1],1,1)
+    def __init__(self, pos):
+        self.pos = pygame.Rect(pos[0], pos[1], 1, 1)
         self._pos = pygame.Rect(self.pos)
         self.frame = 0
 
+
 class Effect:
-    def __init__(self,total,add):
-        
-        if not hasattr(Effect,'images'):
+    def __init__(self, total, add):
+        if not hasattr(Effect, "images"):
             Effect._init(self)
-        
+
         self.total = total
         self.add = add
-        
+
         self.parts = []
-        
+
         self.frame = 0
-        
+
     def _init(self):
         Effect.images = images = []
-        for r in xrange(0,32):
-            img = pygame.Surface((r*2,r*2)).convert()
-            img.fill((255,0,255))
-            img.set_colorkey((255,0,255))
-            img.set_alpha(255-r*8)
-            
-            if r < 8: 
-                rr = r-0
-                c = (255,255,255-rr*8)
+        for r in range(0, 32):
+            img = pygame.Surface((r * 2, r * 2)).convert()
+            img.fill((255, 0, 255))
+            img.set_colorkey((255, 0, 255))
+            img.set_alpha(255 - r * 8)
+
+            if r < 8:
+                rr = r - 0
+                c = (255, 255, 255 - rr * 8)
             elif r < 16:
-                rr = r-8
-                c = (255,255-rr*16,255-(rr+8)*8)
+                rr = r - 8
+                c = (255, 255 - rr * 16, 255 - (rr + 8) * 8)
             else:
-                rr = r-16
-                c = (255-rr*8,128-rr*8,128-rr*8)
-            #print c
-            pygame.draw.circle(img,c,(r,r),r/2)
-            #pygame.draw.circle(img,(255-r*8,255-r*8,255-r*8),(r,r),r)
+                rr = r - 16
+                c = (255 - rr * 8, 128 - rr * 8, 128 - rr * 8)
+            # print c
+            pygame.draw.circle(img, c, (r, r), r / 2)
+            # pygame.draw.circle(img,(255-r*8,255-r*8,255-r*8),(r,r),r)
             images.append(img)
-        
-    def paint(self,screen,origin):
-        todo = [[] for n in xrange(0,32)]
+
+    def paint(self, screen, origin):
+        todo = [[] for n in range(0, 32)]
         for part in self.parts:
             p = part.pos
-            r = part.frame 
-            if r >= 0 and r < 32: todo[r].append(p)
-        for r in xrange(31,-1,-1):
+            r = part.frame
+            if r >= 0 and r < 32:
+                todo[r].append(p)
+        for r in range(31, -1, -1):
             img = Effect.images[r]
-            v = 255-r*8
-            #c = (v,v,v)
-            #c = (255,255,255,v)
+            v = 255 - r * 8
+            # c = (v,v,v)
+            # c = (255,255,255,v)
             for p in todo[r]:
-                #pygame.draw.circle(screen,c,(p.x+pos[0],p.y+pos[1]),r+3)
-                screen.blit(img,(-origin[0]+p.x-r,-origin[1]+p.y-r))
+                # pygame.draw.circle(screen,c,(p.x+pos[0],p.y+pos[1]),r+3)
+                screen.blit(img, (-origin[0] + p.x - r, -origin[1] + p.y - r))
 
-            
-    def loop(self,pos):
+    def loop(self, pos):
         parts = self.parts
         if len(parts) < self.total:
-            for n in xrange(0,self.add):
-                part = Part((pos[0]+0,pos[1]+rr(-2,0)))
+            for n in range(0, self.add):
+                part = Part((pos[0] + 0, pos[1] + rr(-2, 0)))
                 parts.append(part)
         for part in parts:
-            p,_p = part.pos,part._pos
+            p, _p = part.pos, part._pos
+
+            dx, dy = p.x - _p.x, p.y - _p.y
+            _p.x, _p.y = p.x, p.y
+
+            p.x += dx / 3 + rr(-1, 2)
+            p.y += dy / 4 + rr(-2, 1)
 
-            dx,dy = p.x-_p.x,p.y-_p.y
-            _p.x,_p.y = p.x,p.y
-            
-            p.x += dx/3 + rr(-1,2)
-            p.y += dy/4 + rr(-2,1)
-            
-            
             part.frame += 1
             if part.frame >= 32:
-                p.x,p.y = pos[0]+0,pos[1]+rr(-2,0)
-                _p.x,_p.y = p.x,p.y
+                p.x, p.y = pos[0] + 0, pos[1] + rr(-2, 0)
+                _p.x, _p.y = p.x, p.y
                 part.frame = 0
-                
-            
-            
-if __name__ == '__main__':
-    screen = pygame.display.set_mode((640,480))
-    
-    
-    ss = [((rr(160,640),rr(160,480)),Effect(64,1)) for n in xrange(0,8)]
-    
+
+
+if __name__ == "__main__":
+    screen = pygame.display.set_mode((640, 480))
+
+    ss = [((rr(160, 640), rr(160, 480)), Effect(64, 1)) for n in range(0, 8)]
+
     t = timer.Timer(40)
-    
+
     _quit = False
     while not _quit:
         for e in pygame.event.get():
-            if e.type is QUIT: _quit = True
-            if e.type is KEYDOWN and e.key == K_ESCAPE: _quit = True
-        
-        screen.fill((0,0,0))
-        for pos,s in ss:
+            if e.type == QUIT:
+                _quit = True
+            if e.type == KEYDOWN and e.key == K_ESCAPE:
+                _quit = True
+
+        screen.fill((0, 0, 0))
+        for pos, s in ss:
             s.loop(pos)
-            s.paint(screen,(0,0))
+            s.paint(screen, (0, 0))
         pygame.display.flip()
-        
+
         t.tick()
-
```

### Comparing `zanthor-1.2.3/zanthor/main.py` & `zanthor-1.2.4a2/zanthor/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,247 +1,258 @@
 if 0:
     try:
-        #0/0 #HACK: so i can CTRL-c out
+        # 0/0 #HACK: so i can CTRL-c out
         import psyco
+
         psyco.profile()
-        print 'psyco installed'
+        print("psyco installed")
     except:
-        print 'psyco not installed'
+        print("psyco not installed")
 
-import os,sys,time,copy
+import os, sys, time, copy
 
 
 import pygame
-from pygame.locals import *
+
+# Import the android module. If we can't import it, set it to None - this
+# lets us test it, and check to see if we want android-specific behavior.
+try:
+    import android
+except ImportError:
+    android = None
 
 
+try:
+    import pygame.mixer as mixer
+except ImportError:
+    import android_mixer
 
+    pygame.mixer = android_mixer
 
 
-from pgu import engine
-from pgu import timer
+from pygame.locals import *
+
 
-from const import *
+from .pgu import engine
+from .pgu import timer
+
+from .const import *
 
 if 0:
     # this can be used to figure out how big the desktop is...
     pygame.display.init()
-    screen = pygame.display.set_mode((0,0))
+    screen = pygame.display.set_mode((0, 0))
     SW, SH = screen.get_size()
-    import const
-    const.SW, const.SH = screen.get_size()
+    from . import const
 
+    const.SW, const.SH = screen.get_size()
 
 
-import states
-import level
-import units
-import sounds
+from . import states
+from . import level
+from . import units
+from . import sounds
 
 import traceback
 
-import intro
-import menu
-
+from . import intro
+from . import menu
 
 
 class Game(engine.Game):
     def init(self):
-        #self.timer = timer.Timer(FPS)
-        self.timer = timer.Speedometer() 
+        # self.timer = timer.Timer(FPS)
+        self.timer = timer.Speedometer()
         self.clock = pygame.time.Clock()
         self.elapsed_time = 0
         self.last_time = time.time()
         self.cur_time = self.last_time
 
         self.clock.tick(FPS)
 
         # start a song playing here as things load.
         self.sm = sounds.SoundManager()
-        #self.sm.PlayMusic( data_dir('music', "intro.ogg") )
-        self.sm.PlayMusic( data_dir('intro', "intro1.ogg") )
+        # self.sm.PlayMusic( data_dir('music', "intro.ogg") )
+        self.sm.PlayMusic(data_dir("intro", "intro1.ogg"))
         self.sm.Load()
 
-
         # for saving the states between levels.
-        
 
         self.data_reset()
         self.should_restore_stats = True
-        
-
 
     def tick(self):
-        r =  self.timer.tick()
-	if r != None: 
-            #print r
-            print "fps :%s:" % self.clock.get_fps()
-        self.cur_ticks = self.clock.tick(FPS) #to not limit it
+        r = self.timer.tick()
+        if r != None:
+            # print r
+            print(("fps :%s:" % self.clock.get_fps()))
+        self.cur_ticks = self.clock.tick(FPS)  # to not limit it
         self.cur_time = time.time()
 
         self.elapsed_time = self.cur_time - self.last_time
 
         self.sm.Update(self.elapsed_time)
-        #print "&"*20
-        #print self.elapsed_time
-        #print self.clock.get_fps()
-        #for name in dir(self):
+        # print "&"*20
+        # print self.elapsed_time
+        # print self.clock.get_fps()
+        # for name in dir(self):
         #    print name,getattr(self,name)
 
-
     def save_castle_data(self):
-        """
-        """
-        
+        """ """
+
     def data_reset(self):
         self.data = {}
-        self.data['levels'] = []
+        self.data["levels"] = []
         self.upgradable_amounts = None
         self.castle_stats = None
 
         self.backup_upgradable_amounts = None
         self.backup_castle_stats = None
 
-        
-    def event(self,e):
-        #capture special events on a top level,
-        #should only be used for screen shots, forced quits, 
-        #magic cheat buttons, etc... debug keys and the like ...
-        if e.type is QUIT:
+    def event(self, e):
+        # Android-specific:
+        if android:
+            if android.check_pause():
+                android.wait_for_resume()
+
+        # capture special events on a top level,
+        # should only be used for screen shots, forced quits,
+        # magic cheat buttons, etc... debug keys and the like ...
+        if e.type == QUIT:
             self.state = engine.Quit(self)
             return 1
-        
-#         if e.type is KEYDOWN and e.key == K_F10:
+
+
+#         if e.type == KEYDOWN and e.key == K_F10:
 #             self.state = states.SPause(self,self.state)
 #             return 1
 
 #         if e.type == KEYDOWN and e.key == K_ESCAPE:
 #             self.state = engine.Quit(self)
 #             return 1
 
 
-
-
-
-
-def do_main(no_intro = 0, the_level = 0):
+def do_main(no_intro=0, the_level=0):
     global flags
 
+    print("hello from zanthor do_main")
+
     pygame.mixer.pre_init(22050, -16, 2, 1024)
 
     pygame.init()
+    if pygame.mixer and not pygame.mixer.get_init():
+        pygame.mixer = None
     pygame.font.init()
-    #pygame.display.set_caption("The Wrath of ZANTHOR") #It's powered by steam!")
-    pygame.display.set_caption("The Wrath of ZANTHOR!  It's powered by steam!  h key for help")
-
-    #flags = FULLSCREEN
-    print flags
-    print (SW,SH)
-    screen = pygame.display.set_mode((SW,SH), flags)
-
+    # pygame.display.set_caption("The Wrath of ZANTHOR") #It's powered by steam!")
+    pygame.display.set_caption(
+        "The Wrath of ZANTHOR!  It's powered by steam!  h key for help"
+    )
+
+    # flags = FULLSCREEN
+    print(flags)
+    print((SW, SH))
+    screen = pygame.display.set_mode((SW, SH), flags)
+
+    # Map the back button to the escape key.
+    if android:
+        android.map_key(android.KEYCODE_BACK, pygame.K_ESCAPE)
 
+    print("initialising joystick module")
 
     pygame.joystick.init()
-
-    joystics =[]
-
+    joystics = []
     num_joys = pygame.joystick.get_count()
 
-
-    print "initialising joys", num_joys
+    print(("initialising joys", num_joys))
     for x in range(num_joys):
-        print "x joy is:", x
-        j=pygame.joystick.Joystick(x)
+        print(("x joy is:", x))
+        j = pygame.joystick.Joystick(x)
         j.init()
         joystics.append(j)
 
-    print "initialising joys: done."
-
-
-
-
+    print("initialising joys: done.")
 
     game = Game()
     game.should_restore_stats = True
     game.backup_upgradable_amounts = None
     game.backup_castle_stats = None
 
-
     # the intro is not done first.
-    #game.run(states.Title(game),screen)
+    # game.run(states.Title(game),screen)
     if no_intro == 0:
-        game.run(intro.Intro(game),screen)
-        
+        game.run(intro.Intro(game), screen)
+
     elif no_intro == 1:
-        #game.run(level.Level(game, 0,100),screen)
-        game.run(menu.Menu(game),screen)
+        # game.run(level.Level(game, 0,100),screen)
+        game.run(menu.Menu(game), screen)
     elif no_intro == 3:
         # we load the level number from the levels defined in menu.
         n = menu.data[no_intro][4]
         perc = menu.data[no_intro][5]
         music = menu.data[no_intro][7]
-        game.run(level.Level(game,n,perc,music),screen)
+        game.run(level.Level(game, n, perc, music), screen)
     else:
-        game.run(level.Level(game,no_intro,100,None),screen)
-    
+        game.run(level.Level(game, no_intro, 100, None), screen)
 
 
 def main():
     global flags
 
-    if 'speed' in sys.argv:
+    print("hello from zanthor: top of main")
+
+    if "speed" in sys.argv:
         FPS = 65535
 
     the_level = None
-    #flags ^= FULLSCREEN
+    # flags ^= FULLSCREEN
     flags = 0
-    if 'fullscreen' in sys.argv or 'full' in sys.argv:
+    if "fullscreen" in sys.argv or "full" in sys.argv:
         flags ^= FULLSCREEN
 
-    if 'nointro' in sys.argv or "no" in sys.argv:
-        no_intro =1
-    elif 'next' in sys.argv or "nextlevel" in sys.argv:
-        no_intro =2 #uhh, i removed this because i'm dumb
-    elif 'l' in sys.argv:
+    if "nointro" in sys.argv or "no" in sys.argv:
+        no_intro = 1
+    elif "next" in sys.argv or "nextlevel" in sys.argv:
+        no_intro = 2  # uhh, i removed this because i'm dumb
+    elif "l" in sys.argv:
         # main.py l 5
         # we play the level given as an index into menu.data
         the_level = int(sys.argv[-1])
-        no_intro =3
+        no_intro = 3
     else:
-        no_intro =0
-        
-    #jump to any level by specifying, e.g. "level8.tga"
+        no_intro = 0
+
+    # jump to any level by specifying, e.g. "level8.tga"
     for fname in sys.argv:
-        if '.tga' in fname:
+        if ".tga" in fname:
             no_intro = fname
 
-
     if "profile" in sys.argv:
         import hotshot
         import hotshot.stats
         import tempfile
         import os
- 
+
         profile_data_fname = tempfile.mktemp("prf")
         try:
             prof = hotshot.Profile(profile_data_fname)
-            prof.run('do_main(no_intro, the_level = the_level)')
+            prof.run("do_main(no_intro, the_level = the_level)")
             del prof
             s = hotshot.stats.load(profile_data_fname)
             s.strip_dirs()
-            print "cumulative\n\n"
-            s.sort_stats('cumulative').print_stats()
-            print "By time.\n\n"
-            s.sort_stats('time').print_stats()
+            print("cumulative\n\n")
+            s.sort_stats("cumulative").print_stats()
+            print("By time.\n\n")
+            s.sort_stats("time").print_stats()
             del s
         finally:
             # clean up the temporary file name.
             try:
                 os.remove(profile_data_fname)
             except:
                 # may have trouble deleting ;)
                 pass
     else:
         try:
-            do_main(no_intro, the_level = the_level)
+            do_main(no_intro, the_level=the_level)
         except:
             traceback.print_exc(sys.stderr)
```

### Comparing `zanthor-1.2.3/zanthor/pgu/tilevid.py` & `zanthor-1.2.4a2/zanthor/pgu/tilevid.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,195 +1,202 @@
 """Square tile based engine."""
 
 from pgu.vid import *
 import pygame
 
+
 class Tilevid(Vid):
     """Based on [[vid]] -- see for reference."""
-    def paint(self,s):
-        sw,sh = s.get_width(),s.get_height()
-        self.view.w,self.view.h = sw,sh
-        
+
+    def paint(self, s):
+        sw, sh = s.get_width(), s.get_height()
+        self.view.w, self.view.h = sw, sh
+
         tiles = self.tiles
-        tw,th = tiles[0].image.get_width(),tiles[0].image.get_height()
-        w,h = self.size
-        
-        if self.bounds != None: self.view.clamp_ip(self.bounds)
-        
-        ox,oy = self.view.x,self.view.y
+        tw, th = tiles[0].image.get_width(), tiles[0].image.get_height()
+        w, h = self.size
+
+        if self.bounds != None:
+            self.view.clamp_ip(self.bounds)
+
+        ox, oy = self.view.x, self.view.y
         tlayer = self.tlayer
         blayer = self.blayer
         alayer = self.alayer
         sprites = self.sprites
-        
+
         blit = s.blit
-        yy = - (self.view.y%th) 
-        my = (oy+sh)/th
-        if (oy+sh)%th: my += 1
-        
+        yy = -(self.view.y % th)
+        my = (oy + sh) / th
+        if (oy + sh) % th:
+            my += 1
+
         if blayer != None:
-            for y in xrange(oy/th,my):
-                if y >=0 and y < h:
+            for y in range(oy / th, my):
+                if y >= 0 and y < h:
                     trow = tlayer[y]
                     brow = blayer[y]
                     arow = alayer[y]
-                    xx= - (self.view.x%tw)
-                    mx = (ox+sw)/tw
-                    #if (ox+sh)%tw: mx += 1
-                    for x in xrange(ox/tw,mx+1):
-                        if x >=0and x<w:
-                            blit(tiles[brow[x]].image,(xx,yy))
-                            blit(tiles[trow[x]].image,(xx,yy))
-                            arow[x]=0
+                    xx = -(self.view.x % tw)
+                    mx = (ox + sw) / tw
+                    # if (ox+sh)%tw: mx += 1
+                    for x in range(ox / tw, mx + 1):
+                        if x >= 0 and x < w:
+                            blit(tiles[brow[x]].image, (xx, yy))
+                            blit(tiles[trow[x]].image, (xx, yy))
+                            arow[x] = 0
                         xx += tw
-                yy+=th
+                yy += th
         else:
-            for y in xrange(oy/th,my):
-                if y >=0 and y<h:
+            for y in range(oy / th, my):
+                if y >= 0 and y < h:
                     trow = tlayer[y]
                     arow = alayer[y]
-                    xx= - (self.view.x%tw)
-                    mx = (ox+sw)/tw
-                    #if (ox+sh)%tw: mx += 1
-                    for x in xrange(ox/tw,mx+1):
-                        if x >=0 and x<w:
-                            blit(tiles[trow[x]].image,(xx,yy))
-                            arow[x]=0
+                    xx = -(self.view.x % tw)
+                    mx = (ox + sw) / tw
+                    # if (ox+sh)%tw: mx += 1
+                    for x in range(ox / tw, mx + 1):
+                        if x >= 0 and x < w:
+                            blit(tiles[trow[x]].image, (xx, yy))
+                            arow[x] = 0
                         xx += tw
-                yy+=th
+                yy += th
 
         for s in sprites:
-            s.irect.x = s.rect.x-s.shape.x
-            s.irect.y = s.rect.y-s.shape.y
-            blit(s.image,(s.irect.x-ox,s.irect.y-oy))
-            s.updated=0
+            s.irect.x = s.rect.x - s.shape.x
+            s.irect.y = s.rect.y - s.shape.y
+            blit(s.image, (s.irect.x - ox, s.irect.y - oy))
+            s.updated = 0
             s._irect = Rect(s.irect)
-            #s._rect = Rect(s.rect)
+            # s._rect = Rect(s.rect)
 
         self.updates = []
         self._view = pygame.Rect(self.view)
-        return [Rect(0,0,sw,sh)]
-        
-    def update(self,s):
-        sw,sh = s.get_width(),s.get_height()
-        self.view.w,self.view.h = sw,sh
-        
-        if self.bounds != None: self.view.clamp_ip(self.bounds)
-        if self.view.x != self._view.x or self.view.y != self._view.y: 
+        return [Rect(0, 0, sw, sh)]
+
+    def update(self, s):
+        sw, sh = s.get_width(), s.get_height()
+        self.view.w, self.view.h = sw, sh
+
+        if self.bounds != None:
+            self.view.clamp_ip(self.bounds)
+        if self.view.x != self._view.x or self.view.y != self._view.y:
             return self.paint(s)
-        
-        ox,oy = self.view.x,self.view.y
-        sw,sh = s.get_width(),s.get_height()
-        w,h = self.size
+
+        ox, oy = self.view.x, self.view.y
+        sw, sh = s.get_width(), s.get_height()
+        w, h = self.size
         tlayer = self.tlayer
         blayer = self.blayer
         alayer = self.alayer
         tiles = self.tiles
-        tw,th = tiles[0].image.get_width(),tiles[0].image.get_height()
+        tw, th = tiles[0].image.get_width(), tiles[0].image.get_height()
         sprites = self.sprites
         blit = s.blit
-        
+
         us = []
-        
-        #mark places where sprites have moved, or been removed
-        
+
+        # mark places where sprites have moved, or been removed
+
         ss = self.sprites.removed
         self.sprites.removed = []
         ss.extend(sprites)
-        for s in ss: 
-            #figure out what has been updated.
-            s.irect.x = s.rect.x-s.shape.x
-            s.irect.y = s.rect.y-s.shape.y
-            if (s.irect.x != s._irect.x or s.irect.y != s._irect.y
-                     or s.image != s._image):
-                 #w,h can be skipped, image covers that...
-                 s.updated = 1
+        for s in ss:
+            # figure out what has been updated.
+            s.irect.x = s.rect.x - s.shape.x
+            s.irect.y = s.rect.y - s.shape.y
+            if (
+                s.irect.x != s._irect.x
+                or s.irect.y != s._irect.y
+                or s.image != s._image
+            ):
+                # w,h can be skipped, image covers that...
+                s.updated = 1
             if s.updated:
                 r = s._irect
-                y = max(0,r.y/th)
-                yy = min(h,r.bottom/th+1)
+                y = max(0, r.y / th)
+                yy = min(h, r.bottom / th + 1)
                 while y < yy:
-                    x = max(0,r.x/tw)
-                    xx = min(w,r.right/tw+1)
+                    x = max(0, r.x / tw)
+                    xx = min(w, r.right / tw + 1)
                     while x < xx:
                         if alayer[y][x] == 0:
-                            self.updates.append((x,y))
-                        alayer[y][x]=1
+                            self.updates.append((x, y))
+                        alayer[y][x] = 1
                         x += 1
                     y += 1
 
                 r = s.irect
-                y = max(0,r.y/th)
-                yy = min(h,r.bottom/th+1)
+                y = max(0, r.y / th)
+                yy = min(h, r.bottom / th + 1)
                 while y < yy:
-                    x = r.x/tw
-                    xx = min(w,r.right/tw+1)
+                    x = r.x / tw
+                    xx = min(w, r.right / tw + 1)
                     while x < xx:
-                        if alayer[y][x]==0:
-                            alayer[y][x]=2
-                            self.updates.append((x,y))
+                        if alayer[y][x] == 0:
+                            alayer[y][x] = 2
+                            self.updates.append((x, y))
                         x += 1
                     y += 1
-                    
 
-        #mark sprites that are not being updated that need to be updated because
-        #they are being overwritte by sprites / tiles
+        # mark sprites that are not being updated that need to be updated because
+        # they are being overwritte by sprites / tiles
         for s in sprites:
-            if s.updated==0:
+            if s.updated == 0:
                 r = s.irect
-                y = max(0,r.y/th)
-                yy = min(h,r.bottom/th+1)
+                y = max(0, r.y / th)
+                yy = min(h, r.bottom / th + 1)
                 while y < yy:
-                    x = max(0,r.x/tw)
-                    xx = min(w,r.right/tw+1)
+                    x = max(0, r.x / tw)
+                    xx = min(w, r.right / tw + 1)
                     while x < xx:
-                        if alayer[y][x]==1:
-                            s.updated=1
+                        if alayer[y][x] == 1:
+                            s.updated = 1
                         x += 1
                     y += 1
 
-        
         for u in self.updates:
-            x,y=u
-            xx,yy=x*tw-ox,y*th-oy
+            x, y = u
+            xx, yy = x * tw - ox, y * th - oy
             if alayer[y][x] == 1:
-                if blayer != None: blit(tiles[blayer[y][x]].image,(xx,yy))
-                blit(tiles[tlayer[y][x]].image,(xx,yy))
-            alayer[y][x]=0
-            us.append(Rect(xx,yy,tw,th))
-        
+                if blayer != None:
+                    blit(tiles[blayer[y][x]].image, (xx, yy))
+                blit(tiles[tlayer[y][x]].image, (xx, yy))
+            alayer[y][x] = 0
+            us.append(Rect(xx, yy, tw, th))
+
         for s in sprites:
             if s.updated:
-                blit(s.image,(s.irect.x-ox, s.irect.y-oy))
-                s.updated=0
+                blit(s.image, (s.irect.x - ox, s.irect.y - oy))
+                s.updated = 0
                 s._irect = Rect(s.irect)
                 s._image = s.image
-                
+
         self.updates = []
         return us
 
-    def view_to_tile(self,pos):
-        x,y = pos
+    def view_to_tile(self, pos):
+        x, y = pos
         tiles = self.tiles
-        tw,th = tiles[0].image.get_width(),tiles[0].image.get_height()
-        return x/tw,y/th
-        
-    def tile_to_view(self,pos):
-        x,y = pos
+        tw, th = tiles[0].image.get_width(), tiles[0].image.get_height()
+        return x / tw, y / th
+
+    def tile_to_view(self, pos):
+        x, y = pos
         tiles = self.tiles
-        tw,th = tiles[0].image.get_width(),tiles[0].image.get_height()
-        x,y = x*tw, y*th 
-        return x,y
-        
-                    
-    def screen_to_tile(self,pos):
-        x,y = pos
-        x,y = x+self.view.x,y+self.view.y
-        return self.view_to_tile((x,y))
-        
-    def tile_to_screen(self,pos):
-        x,y = pos
-        x,y = self.tile_to_view(pos)
-        x,y = x - self.view.x, y - self.view.y
-        return x,y
-                    
+        tw, th = tiles[0].image.get_width(), tiles[0].image.get_height()
+        x, y = x * tw, y * th
+        return x, y
+
+    def screen_to_tile(self, pos):
+        x, y = pos
+        x, y = x + self.view.x, y + self.view.y
+        return self.view_to_tile((x, y))
+
+    def tile_to_screen(self, pos):
+        x, y = pos
+        x, y = self.tile_to_view(pos)
+        x, y = x - self.view.x, y - self.view.y
+        return x, y
+
+
 # vim: set filetype=python sts=4 sw=4 noet si :
```

### Comparing `zanthor-1.2.3/zanthor/pgu/html.py` & `zanthor-1.2.4a2/zanthor/pgu/html.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,534 +3,656 @@
 import htmllib
 import re
 import pygame
 from pygame.locals import *
 
 from pgu import gui
 
-_amap = {'left':-1,'right':1,'center':0,None:None,'':None,}
-_vamap = {'top':-1,'bottom':1,'center':0,'middle':0,None:None,'':None,}
+_amap = {
+    "left": -1,
+    "right": 1,
+    "center": 0,
+    None: None,
+    "": None,
+}
+_vamap = {
+    "top": -1,
+    "bottom": 1,
+    "center": 0,
+    "middle": 0,
+    None: None,
+    "": None,
+}
+
 
 class _dummy:
     pass
 
+
 class _flush:
     def __init__(self):
         self.style = _dummy()
         self.style.font = None
         self.style.color = None
         self.cls = None
-    def add(self,w): pass
-    def space(self,v): pass
-    
+
+    def add(self, w):
+        pass
+
+    def space(self, v):
+        pass
+
+
 class _hr(gui.Color):
-    def __init__(self,**params):
-        gui.Color.__init__(self,(0,0,0),**params)
-    def resize(self,width=None,height=None):
-        w,h = self.style.width,self.style.height
-        #if width != None: self.rect.w = width
-        #else: self.rect.w = 1
-        
-        #xt,xr,xb,xl = self.getspacing()
-
-        if width != None: w = max(w,width)
-        if height != None: h = max(h,height)        
-        w = max(w,1)
-        h = max(h,1)
-        
-        return w,h #self.container.rect.w,h
-        
-        #self.rect.w = max(1,width,self.container.rect.w-(xl+xr))
-        
-        #print self.rect
-        #self.rect.w = 1
+    def __init__(self, **params):
+        gui.Color.__init__(self, (0, 0, 0), **params)
+
+    def resize(self, width=None, height=None):
+        w, h = self.style.width, self.style.height
+        # if width != None: self.rect.w = width
+        # else: self.rect.w = 1
+
+        # xt,xr,xb,xl = self.getspacing()
+
+        if width != None:
+            w = max(w, width)
+        if height != None:
+            h = max(h, height)
+        w = max(w, 1)
+        h = max(h, 1)
+
+        return w, h  # self.container.rect.w,h
+
+        # self.rect.w = max(1,width,self.container.rect.w-(xl+xr))
+
+        # print self.rect
+        # self.rect.w = 1
+
 
 class _html(htmllib.HTMLParser):
-    def init(self,doc,font,color,_globals,_locals):
+    def init(self, doc, font, color, _globals, _locals):
         self.mystack = []
         self.document = doc
-        self.myopen('document',self.document)
-        
+        self.myopen("document", self.document)
+
         self.myfont = self.font = font
         self.mycolor = self.color = color
-        
+
         self.form = None
-        
+
         self._globals = _globals
         self._locals = _locals
-        
-    def myopen(self,type_,w):
-    
-        self.mystack.append((type_,w))
-        self.type,self.item = type_,w
-        
+
+    def myopen(self, type_, w):
+        self.mystack.append((type_, w))
+        self.type, self.item = type_, w
+
         self.font = self.item.style.font
         self.color = self.item.style.color
-        
-        if not self.font: self.font = self.myfont
-        if not self.color: self.color = self.mycolor
-        
-    def myclose(self,type_):
+
+        if not self.font:
+            self.font = self.myfont
+        if not self.color:
+            self.color = self.mycolor
+
+    def myclose(self, type_):
         t = None
         self.mydone()
         while t != type_:
-            #if len(self.mystack)==0: return
-            t,w = self.mystack.pop()
-        t,w = self.mystack.pop()
-        self.myopen(t,w)
-        
-    def myback(self,type_):
-        if type(type_) == str: type_ = [type_,]
+            # if len(self.mystack)==0: return
+            t, w = self.mystack.pop()
+        t, w = self.mystack.pop()
+        self.myopen(t, w)
+
+    def myback(self, type_):
+        if type(type_) == str:
+            type_ = [
+                type_,
+            ]
         self.mydone()
-        #print 'myback',type_
+        # print 'myback',type_
         t = None
         while t not in type_:
-            #if len(self.mystack)==0: return
-            t,w = self.mystack.pop()
-        self.myopen(t,w)
-        
+            # if len(self.mystack)==0: return
+            t, w = self.mystack.pop()
+        self.myopen(t, w)
+
     def mydone(self):
-        #clearing out the last </p>
-        if not hasattr(self.item,'layout'): return 
-        if len(self.item.layout._widgets) == 0: return 
+        # clearing out the last </p>
+        if not hasattr(self.item, "layout"):
+            return
+        if len(self.item.layout._widgets) == 0:
+            return
         w = self.item.layout._widgets[-1]
         if type(w) == tuple:
             del self.item.layout._widgets[-1]
 
-        
-    def start_b(self,attrs): self.font.set_bold(1)
-    def end_b(self): self.font.set_bold(0)
-    def start_i(self,attrs): self.font.set_italic(1)
-    def end_i(self): self.font.set_italic(0)
-    def start_u(self,attrs): self.font.set_underline(1)
-    def end_u(self): self.font.set_underline(0)
-    def start_br(self,attrs): self.do_br(attrs)
-    def do_br(self,attrs): self.item.br(self.font.size(" ")[1])
-    def attrs_to_map(self,attrs):
+    def start_b(self, attrs):
+        self.font.set_bold(1)
+
+    def end_b(self):
+        self.font.set_bold(0)
+
+    def start_i(self, attrs):
+        self.font.set_italic(1)
+
+    def end_i(self):
+        self.font.set_italic(0)
+
+    def start_u(self, attrs):
+        self.font.set_underline(1)
+
+    def end_u(self):
+        self.font.set_underline(0)
+
+    def start_br(self, attrs):
+        self.do_br(attrs)
+
+    def do_br(self, attrs):
+        self.item.br(self.font.size(" ")[1])
+
+    def attrs_to_map(self, attrs):
         k = None
         r = {}
-        for k,v in attrs: r[k] = v
+        for k, v in attrs:
+            r[k] = v
         return r
-        
-    def map_to_params(self,r):
+
+    def map_to_params(self, r):
         anum = re.compile("\D")
-        
-        params = {'style':{}}
-        style = params['style']
-        
-        if 'bgcolor' in r: style['background'] = pygame.Color(r['bgcolor'])
-        if 'background' in r: style['background'] = pygame.image.load(r['background'])
-        if 'border' in r: style['border'] = int(r['border'])
-            
-        for k in ['width','height','colspan','rowspan','size','min','max']:
-            if k in r: params[k] = int(anum.sub("",r[k]))
-            
-        for k in ['name','value']:
-            if k in r: params[k] = r[k]
-        
-        if 'class' in r: params['cls'] = r['class']
-        
-        if 'align' in r: 
-            params['align'] = _amap[r['align']]
-        if 'valign' in r:
-            params['valign'] = _vamap[r['valign']]
-
-        if 'style' in r:
-            for st in r['style'].split(";"):
-                #print st
+
+        params = {"style": {}}
+        style = params["style"]
+
+        if "bgcolor" in r:
+            style["background"] = pygame.Color(r["bgcolor"])
+        if "background" in r:
+            style["background"] = pygame.image.load(r["background"])
+        if "border" in r:
+            style["border"] = int(r["border"])
+
+        for k in ["width", "height", "colspan", "rowspan", "size", "min", "max"]:
+            if k in r:
+                params[k] = int(anum.sub("", r[k]))
+
+        for k in ["name", "value"]:
+            if k in r:
+                params[k] = r[k]
+
+        if "class" in r:
+            params["cls"] = r["class"]
+
+        if "align" in r:
+            params["align"] = _amap[r["align"]]
+        if "valign" in r:
+            params["valign"] = _vamap[r["valign"]]
+
+        if "style" in r:
+            for st in r["style"].split(";"):
+                # print st
                 if ":" in st:
-                    #print st.split(":")
-                    k,v = st.split(":")
-                    k = k.replace("-","_")
-                    k = k.replace(" ","")
-                    v = v.replace(" ","")
-                    if k == 'color' or k == 'border_color' or k == 'background':
+                    # print st.split(":")
+                    k, v = st.split(":")
+                    k = k.replace("-", "_")
+                    k = k.replace(" ", "")
+                    v = v.replace(" ", "")
+                    if k == "color" or k == "border_color" or k == "background":
                         v = pygame.Color(v)
                     else:
-                        v = int(anum.sub("",v))
+                        v = int(anum.sub("", v))
                     style[k] = v
         return params
-        
-    def map_to_connects(self,e,r):
-        for k,evt in [('onclick',gui.CLICK),('onchange',gui.CHANGE)]: #blah blah blah
-            
+
+    def map_to_connects(self, e, r):
+        for k, evt in [
+            ("onclick", gui.CLICK),
+            ("onchange", gui.CHANGE),
+        ]:  # blah blah blah
             if k in r:
-                #print k,r[k]
-                e.connect(evt,self.myexec,(e,r[k]))
+                # print k,r[k]
+                e.connect(evt, self.myexec, (e, r[k]))
 
-    def start_p(self,attrs):
+    def start_p(self, attrs):
         r = self.attrs_to_map(attrs)
-        align = r.get("align","left")
-        
+        align = r.get("align", "left")
+
         self.check_p()
         self.item.block(_amap[align])
-        
+
     def check_p(self):
-        if len(self.item.layout._widgets) == 0: return
+        if len(self.item.layout._widgets) == 0:
+            return
         if type(self.item.layout._widgets[-1]) == tuple:
-            w,h = self.item.layout._widgets[-1]
-            if w == 0: return
+            w, h = self.item.layout._widgets[-1]
+            if w == 0:
+                return
         self.do_br(None)
-        
+
     def end_p(self):
-        #print 'end p'
+        # print 'end p'
         self.check_p()
-        
-        
-    def start_block(self,t,attrs,align=-1):
+
+    def start_block(self, t, attrs, align=-1):
         r = self.attrs_to_map(attrs)
         params = self.map_to_params(r)
-        if 'cls' in params: params['cls'] = t+"."+params['cls']
-        else: params['cls'] = t
+        if "cls" in params:
+            params["cls"] = t + "." + params["cls"]
+        else:
+            params["cls"] = t
         b = gui.Document(**params)
-        if 'align' in params:
-            align = params['align']
+        if "align" in params:
+            align = params["align"]
         self.item.block(align)
         self.item.add(b)
-        self.myopen(t,b)
+        self.myopen(t, b)
 
-        
-                
-    def end_block(self,t):
+    def end_block(self, t):
         self.myclose(t)
         self.item.block(-1)
-        
-    def start_div(self,attrs): self.start_block('div',attrs)
-    def end_div(self): self.end_block('div')
-    def start_center(self,attrs): self.start_block('div',attrs,0)
-    def end_center(self): self.end_block('div')
-    
-    def start_h1(self,attrs): self.start_block('h1',attrs)
-    def end_h1(self): self.end_block('h1')
-    def start_h2(self,attrs): self.start_block('h2',attrs)
-    def end_h2(self): self.end_block('h2')
-    def start_h3(self,attrs): self.start_block('h3',attrs)
-    def end_h3(self): self.end_block('h3')
-    def start_h4(self,attrs): self.start_block('h4',attrs)
-    def end_h4(self): self.end_block('h4')
-    def start_h5(self,attrs): self.start_block('h5',attrs)
-    def end_h5(self): self.end_block('h5')
-    def start_h6(self,attrs): self.start_block('h6',attrs)
-    def end_h6(self): self.end_block('h6')
-
-    def start_ul(self,attrs): self.start_block('ul',attrs)
-    def end_ul(self): self.end_block('ul')
-    def start_ol(self,attrs): 
-        self.start_block('ol',attrs)
+
+    def start_div(self, attrs):
+        self.start_block("div", attrs)
+
+    def end_div(self):
+        self.end_block("div")
+
+    def start_center(self, attrs):
+        self.start_block("div", attrs, 0)
+
+    def end_center(self):
+        self.end_block("div")
+
+    def start_h1(self, attrs):
+        self.start_block("h1", attrs)
+
+    def end_h1(self):
+        self.end_block("h1")
+
+    def start_h2(self, attrs):
+        self.start_block("h2", attrs)
+
+    def end_h2(self):
+        self.end_block("h2")
+
+    def start_h3(self, attrs):
+        self.start_block("h3", attrs)
+
+    def end_h3(self):
+        self.end_block("h3")
+
+    def start_h4(self, attrs):
+        self.start_block("h4", attrs)
+
+    def end_h4(self):
+        self.end_block("h4")
+
+    def start_h5(self, attrs):
+        self.start_block("h5", attrs)
+
+    def end_h5(self):
+        self.end_block("h5")
+
+    def start_h6(self, attrs):
+        self.start_block("h6", attrs)
+
+    def end_h6(self):
+        self.end_block("h6")
+
+    def start_ul(self, attrs):
+        self.start_block("ul", attrs)
+
+    def end_ul(self):
+        self.end_block("ul")
+
+    def start_ol(self, attrs):
+        self.start_block("ol", attrs)
         self.item.counter = 0
-    def end_ol(self): self.end_block('ol')
-    def start_li(self,attrs): 
-        self.myback(['ul','ol'])
+
+    def end_ol(self):
+        self.end_block("ol")
+
+    def start_li(self, attrs):
+        self.myback(["ul", "ol"])
         cur = self.item
-        self.start_block('li',attrs)
-        if hasattr(cur,'counter'):
+        self.start_block("li", attrs)
+        if hasattr(cur, "counter"):
             cur.counter += 1
-            self.handle_data("%d. "%cur.counter)
+            self.handle_data("%d. " % cur.counter)
         else:
             self.handle_data("- ")
-    #def end_li(self): self.end_block('li') #this isn't needed because of how the parser works
 
-    def start_pre(self,attrs): self.start_block('pre',attrs)
-    def end_pre(self): self.end_block('pre')
-    def start_code(self,attrs): self.start_block('code',attrs)
-    def end_code(self): self.end_block('code')
-            
-    def start_table(self,attrs):
+    # def end_li(self): self.end_block('li') #this isn't needed because of how the parser works
+
+    def start_pre(self, attrs):
+        self.start_block("pre", attrs)
+
+    def end_pre(self):
+        self.end_block("pre")
+
+    def start_code(self, attrs):
+        self.start_block("code", attrs)
+
+    def end_code(self):
+        self.end_block("code")
+
+    def start_table(self, attrs):
         r = self.attrs_to_map(attrs)
         params = self.map_to_params(r)
-        
-        align = r.get("align","left")
+
+        align = r.get("align", "left")
         self.item.block(_amap[align])
 
         t = gui.Table(**params)
         self.item.add(t)
-        
-        self.myopen('table',t)
-        
-    def start_tr(self,attrs):
-        self.myback('table')
+
+        self.myopen("table", t)
+
+    def start_tr(self, attrs):
+        self.myback("table")
         self.item.tr()
-        
-    def _start_td(self,t,attrs):
+
+    def _start_td(self, t, attrs):
         r = self.attrs_to_map(attrs)
         params = self.map_to_params(r)
-        if 'cls' in params: params['cls'] = t+"."+params['cls']
-        else: params['cls'] = t
+        if "cls" in params:
+            params["cls"] = t + "." + params["cls"]
+        else:
+            params["cls"] = t
         b = gui.Document(cls=t)
-        
-        self.myback('table')
-        self.item.td(b,**params)
-        self.myopen(t,b)
-    
+
+        self.myback("table")
+        self.item.td(b, **params)
+        self.myopen(t, b)
+
         self.font = self.item.style.font
         self.color = self.item.style.color
-        
-    def start_td(self,attrs):
-        self._start_td('td',attrs)
-    
-    def start_th(self,attrs):
-        self._start_td('th',attrs)
-        
+
+    def start_td(self, attrs):
+        self._start_td("td", attrs)
+
+    def start_th(self, attrs):
+        self._start_td("th", attrs)
+
     def end_table(self):
-        self.myclose('table')
+        self.myclose("table")
         self.item.block(-1)
-        
-    def start_form(self,attrs):
+
+    def start_form(self, attrs):
         r = self.attrs_to_map(attrs)
         e = self.form = gui.Form()
         e.groups = {}
-        
-        self._locals[r.get('id',None)] = e
-        
-    def start_input(self,attrs):
+
+        self._locals[r.get("id", None)] = e
+
+    def start_input(self, attrs):
         r = self.attrs_to_map(attrs)
-        params = self.map_to_params(r) #why bother
-        #params = {}
-        
-        type_,name,value = r.get('type','text'),r.get('name',None),r.get('value',None)
+        params = self.map_to_params(r)  # why bother
+        # params = {}
+
+        type_, name, value = (
+            r.get("type", "text"),
+            r.get("name", None),
+            r.get("value", None),
+        )
         f = self.form
-        if type_ == 'text':
+        if type_ == "text":
             e = gui.Input(**params)
-            self.map_to_connects(e,r)
+            self.map_to_connects(e, r)
             self.item.add(e)
-        elif type_ == 'radio':
+        elif type_ == "radio":
             if name not in f.groups:
                 f.groups[name] = gui.Group(name=name)
             g = f.groups[name]
-            del params['name']
-            e = gui.Radio(group=g,**params)
-            self.map_to_connects(e,r)
+            del params["name"]
+            e = gui.Radio(group=g, **params)
+            self.map_to_connects(e, r)
             self.item.add(e)
-            if 'checked' in r: g.value = value
-        elif type_ == 'checkbox':
+            if "checked" in r:
+                g.value = value
+        elif type_ == "checkbox":
             if name not in f.groups:
                 f.groups[name] = gui.Group(name=name)
             g = f.groups[name]
-            del params['name']
-            e = gui.Checkbox(group=g,**params)
-            self.map_to_connects(e,r)
+            del params["name"]
+            e = gui.Checkbox(group=g, **params)
+            self.map_to_connects(e, r)
             self.item.add(e)
-            if 'checked' in r: g.value = value
+            if "checked" in r:
+                g.value = value
 
-        elif type_ == 'button':
+        elif type_ == "button":
             e = gui.Button(**params)
-            self.map_to_connects(e,r)
+            self.map_to_connects(e, r)
             self.item.add(e)
-        elif type_ == 'submit':
+        elif type_ == "submit":
             e = gui.Button(**params)
-            self.map_to_connects(e,r)
+            self.map_to_connects(e, r)
             self.item.add(e)
-        elif type_ == 'file':
+        elif type_ == "file":
             e = gui.Input(**params)
-            self.map_to_connects(e,r)
+            self.map_to_connects(e, r)
             self.item.add(e)
-            b = gui.Button(value='Browse...')
+            b = gui.Button(value="Browse...")
             self.item.add(b)
+
             def _browse(value):
-                d = gui.FileDialog();
-                d.connect(gui.CHANGE,gui.action_setvalue,(d,e))
-                d.open();
-            b.connect(gui.CLICK,_browse,None)
+                d = gui.FileDialog()
+                d.connect(gui.CHANGE, gui.action_setvalue, (d, e))
+                d.open()
 
-        self._locals[r.get('id',None)] = e
+            b.connect(gui.CLICK, _browse, None)
 
-    def start_object(self,attrs):
+        self._locals[r.get("id", None)] = e
+
+    def start_object(self, attrs):
         r = self.attrs_to_map(attrs)
         params = self.map_to_params(r)
-        code = "e = %s(**params)"%r['type']
-        #print code
-        #print params
+        code = "e = %s(**params)" % r["type"]
+        # print code
+        # print params
         exec(code)
-        #print e
-        #print e.style.width,e.style.height
-        self.map_to_connects(e,r)
+        # print e
+        # print e.style.width,e.style.height
+        self.map_to_connects(e, r)
         self.item.add(e)
-        
-        self._locals[r.get('id',None)] = e
-    
-    def start_select(self,attrs):
+
+        self._locals[r.get("id", None)] = e
+
+    def start_select(self, attrs):
         r = self.attrs_to_map(attrs)
         params = {}
-        
-        name,value = r.get('name',None),r.get('value',None)
-        e = gui.Select(name=name,value=value,**params)
-        self.map_to_connects(e,r)
+
+        name, value = r.get("name", None), r.get("value", None)
+        e = gui.Select(name=name, value=value, **params)
+        self.map_to_connects(e, r)
         self.item.add(e)
-        self.myopen('select',e)
-        
-    def start_option(self,attrs):
+        self.myopen("select", e)
+
+    def start_option(self, attrs):
         r = self.attrs_to_map(attrs)
-        params = {} #style = self.map_to_style(r)
-        
-        self.myback('select')
+        params = {}  # style = self.map_to_style(r)
+
+        self.myback("select")
         e = gui.Document(**params)
-        self.item.add(e,value=r.get('value',None))
-        self.myopen('option',e)
-        
-        
+        self.item.add(e, value=r.get("value", None))
+        self.myopen("option", e)
+
     def end_select(self):
-        self.myclose('select')
-        
-    def start_hr(self,attrs):
+        self.myclose("select")
+
+    def start_hr(self, attrs):
         self.do_hr(attrs)
-    def do_hr(self,attrs):
-        h = self.font.size(" ")[1]/2
-        
+
+    def do_hr(self, attrs):
+        h = self.font.size(" ")[1] / 2
+
         r = self.attrs_to_map(attrs)
         params = self.map_to_params(r)
-        params['style']['padding'] = h
-        print params
+        params["style"]["padding"] = h
+        print(params)
 
         self.item.block(0)
         self.item.add(_hr(**params))
         self.item.block(-1)
-        
-    def anchor_begin(self,href,name,type_):
+
+    def anchor_begin(self, href, name, type_):
         pass
 
     def anchor_end(self):
         pass
-        
-    def start_title(self,attrs): self.myopen('title',_flush())
-    def end_title(self): self.myclose('title')
-            
-    def myexec(self,value):
-        w,code = value
+
+    def start_title(self, attrs):
+        self.myopen("title", _flush())
+
+    def end_title(self):
+        self.myclose("title")
+
+    def myexec(self, value):
+        w, code = value
         g = self._globals
         l = self._locals
-        l['self'] = w
-        exec(code,g,l)
-        
-    def handle_image(self,src,alt,ismap,align,width,height):
+        l["self"] = w
+        exec(code, g, l)
+
+    def handle_image(self, src, alt, ismap, align, width, height):
         try:
             w = gui.Image(pygame.image.load(src))
-            if align != '':
-                self.item.add(w,_amap[align])
+            if align != "":
+                self.item.add(w, _amap[align])
             else:
                 self.item.add(w)
         except:
-            print 'handle_image: missing %s'%src
-                
-    def handle_data(self,txt):
-        if self.type == 'table': return 
-        elif self.type in ('pre','code'): 
-            txt = txt.replace("\t","        ")
+            print("handle_image: missing %s" % src)
+
+    def handle_data(self, txt):
+        if self.type == "table":
+            return
+        elif self.type in ("pre", "code"):
+            txt = txt.replace("\t", "        ")
             ss = txt.split("\n")
-            if ss[-1] == "": del ss[-1]
+            if ss[-1] == "":
+                del ss[-1]
             for sentence in ss:
-                img = self.font.render(sentence,1,self.color)
+                img = self.font.render(sentence, 1, self.color)
                 w = gui.Image(img)
                 self.item.add(w)
                 self.item.block(-1)
             return
 
-        txt = re.compile("^[\t\r\n]+").sub("",txt)
-        txt = re.compile("[\t\r\n]+$").sub("",txt)
-        
-        tst = re.compile("[\t\r\n]+").sub("",txt)
-        if tst == "": return
-        
-        txt = re.compile("\s+").sub(" ",txt)
-        if txt == "": return
-        
+        txt = re.compile("^[\t\r\n]+").sub("", txt)
+        txt = re.compile("[\t\r\n]+$").sub("", txt)
+
+        tst = re.compile("[\t\r\n]+").sub("", txt)
+        if tst == "":
+            return
+
+        txt = re.compile("\s+").sub(" ", txt)
+        if txt == "":
+            return
+
         if txt == " ":
             self.item.space(self.font.size(" "))
             return
-        
+
         for word in txt.split(" "):
-            word = word.replace(chr(160)," ") #&nbsp;
-            #print self.item.cls
-            w = gui.Image(self.font.render(word,1,self.color))
+            word = word.replace(chr(160), " ")  # &nbsp;
+            # print self.item.cls
+            w = gui.Image(self.font.render(word, 1, self.color))
             self.item.add(w)
             self.item.space(self.font.size(" "))
-            
+
 
 class HTML(gui.Document):
     """a gui HTML object
-    
+
     <pre>HTML(data,globals=None,locals=None)</pre>
-        
-    <dl>    
+
+    <dl>
     <dt>data <dd>html data
     <dt>globals <dd>global variables (for scripting)
     <dt>locals <dd>local variables (for scripting)
     </dl>
-    
+
     <p>you may access html elements that have an id via widget[id]</p>
     """
-    def __init__(self,data,globals=None,locals=None,**params):
-        gui.Document.__init__(self,**params)
-        
-        _globals,_locals = globals,locals
-        
-        if _globals == None: _globals = {}
-        if _locals == None: _locals = {}
+
+    def __init__(self, data, globals=None, locals=None, **params):
+        gui.Document.__init__(self, **params)
+
+        _globals, _locals = globals, locals
+
+        if _globals == None:
+            _globals = {}
+        if _locals == None:
+            _locals = {}
         self._globals = _globals
         self._locals = _locals
-        
-        #font = gui.theme.get("label","","font")
-        p = _html(htmllib.AS_IS,0)
-        p.init(self,self.style.font,self.style.color,_globals,_locals)
-        p.feed(data) 
-        p.close() 
+
+        # font = gui.theme.get("label","","font")
+        p = _html(htmllib.AS_IS, 0)
+        p.init(self, self.style.font, self.style.color, _globals, _locals)
+        p.feed(data)
+        p.close()
         p.mydone()
-        
-        
-    def __getitem__(self,k):
+
+    def __getitem__(self, k):
         return self._locals[k]
 
-def render(font,rect,text,aa,color,bgcolor=(0,0,0,0)):
+
+def render(font, rect, text, aa, color, bgcolor=(0, 0, 0, 0)):
     """render some html
-    
+
     <pre>render(font,rect,text,aa,color,bgcolor=(0,0,0,0))</pre>
     """
-    fnt,r,txt,a,fg,bg = font,rect,text,aa,color,bgcolor
-    
-    e = HTML(txt,font=fnt,color=fg)
+    fnt, r, txt, a, fg, bg = font, rect, text, aa, color, bgcolor
+
+    e = HTML(txt, font=fnt, color=fg)
     e.resize(width=rect.w)
-    s = pygame.Surface((e.rect.w,e.rect.h),SWSURFACE|SRCALPHA,32)
+    s = pygame.Surface((e.rect.w, e.rect.h), SWSURFACE | SRCALPHA, 32)
     s.fill(bg)
     e.paint(s)
-    
+
     return s
 
-def rendertrim(font,rect,text,aa,color,bgcolor=(0,0,0,0)):
+
+def rendertrim(font, rect, text, aa, color, bgcolor=(0, 0, 0, 0)):
     """render html, and make sure to trim the size
-    
+
     <pre>rendertrim(font,rect,text,aa,color,bgcolor=(0,0,0,0))</pre>
     """
-    fnt,r,txt,a,fg,bg = font,rect,text,aa,color,bgcolor
-    #print r
-    w = HTML(txt,font=fnt,color=fg)
+    fnt, r, txt, a, fg, bg = font, rect, text, aa, color, bgcolor
+    # print r
+    w = HTML(txt, font=fnt, color=fg)
     w.resize(width=rect.w)
-    s = pygame.Surface((w.rect.w,w.rect.h),SWSURFACE|SRCALPHA,32)
+    s = pygame.Surface((w.rect.w, w.rect.h), SWSURFACE | SRCALPHA, 32)
     s.fill(bg)
     w.paint(s)
-    
-    minx,miny,maxx,maxy = 1024,1024,-1024,-1024
+
+    minx, miny, maxx, maxy = 1024, 1024, -1024, -1024
     for e in w.layout.widgets:
-        x,y,w,h = e.rect.x,e.rect.y,e.rect.w,e.rect.h
-        minx = min(minx,x)
-        miny = min(miny,y)
-        x,y = x+w,y+h
-        maxx = max(maxx,x)
-        maxy = max(maxy,y)
-        
-    r = pygame.Rect(minx,miny,maxx-minx,maxy-miny)
-        
+        x, y, w, h = e.rect.x, e.rect.y, e.rect.w, e.rect.h
+        minx = min(minx, x)
+        miny = min(miny, y)
+        x, y = x + w, y + h
+        maxx = max(maxx, x)
+        maxy = max(maxy, y)
+
+    r = pygame.Rect(minx, miny, maxx - minx, maxy - miny)
+
     return s.subsurface((r))
 
-    
-def write(s,font,rect,text,aa=0,color=(0,0,0)):
+
+def write(s, font, rect, text, aa=0, color=(0, 0, 0)):
     """write html to a surface
-    
+
     <pre>write(s,font,rect,text,aa=0,color=(0,0,0))</pre>
     """
-    fnt,r,txt,a,fg = font,rect,text,aa,color
+    fnt, r, txt, a, fg = font, rect, text, aa, color
 
     e = HTML(txt)
-    
+
     e.resize(width=rect.w)
     s = s.subsurface(rect)
     e.paint(s)
-    
+
+
 # vim: set filetype=python sts=4 sw=4 noet si :
```

### Comparing `zanthor-1.2.3/zanthor/pgu/high.py` & `zanthor-1.2.4a2/zanthor/pgu/high.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,152 +1,155 @@
 """Classes for handling high score tables.
 """
 
 import os
 
-def High(fname,limit=10):
+
+def High(fname, limit=10):
     """Create a Highs object and returns the default high score table.
-    
+
     <pre>High(fname,limit=10)</pre>
-    
+
     <dl>
     <dt>fname <dd>filename to store high scores in
     <dt>limit <dd>limit of scores to be recorded, defaults to 10
     </dl>
     """
-    return Highs(fname,limit)['default']
-    
+    return Highs(fname, limit)["default"]
+
+
 class _Score:
-    def __init__(self,score,name,data=None):
-        self.score,self.name,self.data=score,name,data
-    
+    def __init__(self, score, name, data=None):
+        self.score, self.name, self.data = score, name, data
+
+
 class _High:
     """A high score table.  These objects are passed to the user, but should not be created directly.
-    
+
     <p>You can iterate them:</p>
     <code>
     for e in myhigh:
         print e.score,e.name,e.data
     </code>
-        
+
     <p>You can modify them:</p>
     <code>
     myhigh[0].name = 'Cuzco'
     </code>
-    
+
     <p>You can find out their length:</p>
     <code>
     print len(myhigh)
     </code>
     """
-    
-    def __init__(self,highs,limit=10):
+
+    def __init__(self, highs, limit=10):
         self.highs = highs
         self._list = []
         self.limit = limit
-        
+
     def save(self):
         """Save the high scores.
-        
+
         <pre>_High.save()</pre>
         """
         self.highs.save()
-        
-    def submit(self,score,name,data=None):
+
+    def submit(self, score, name, data=None):
         """Submit a high score to this table.
-        
+
         <pre>_High.submit(score,name,data=None)</pre>
-        
+
         <p>return -- the position in the table that the score attained.  None if the score did not attain a position in the table.</p>
         """
         n = 0
         for e in self._list:
             if score > e.score:
-                self._list.insert(n,_Score(score,name,data))
-                self._list = self._list[0:self.limit]
+                self._list.insert(n, _Score(score, name, data))
+                self._list = self._list[0 : self.limit]
                 return n
         if len(self._list) < self.limit:
-            self._list.append(_Score(score,name,data))
-            return len(self._list)-1
-    
-    def check(self,score):
+            self._list.append(_Score(score, name, data))
+            return len(self._list) - 1
+
+    def check(self, score):
         """Check if a score will attain a position in the table.
-        
+
         <pre>_High.check(score)</pre>
-        
+
         <p>return -- the position the score will attain, else None</p>
         """
         n = 0
         for e in self._list:
             if score > e.score:
                 return n
         if len(self._list) < self.limit:
             return len(self._list)
-        
-        
+
     def __iter__(self):
         return self._list.__iter__()
-        
-    def __getitem__(self,key):
+
+    def __getitem__(self, key):
         return self._list[key]
-        
+
     def __len__(self):
         return self._list.__len__()
-        
+
 
 class Highs:
     """The high score object.
-    
+
     <pre>Highs(fname,limit=10)</pre>
     <ul>
     <dt>fname <dd>filename to store high scores in
     <dt>limit <dd>limit of scores to be recorded, defaults to 10
     </ul>
-    
+
     <p>You may access _High objects through this object:</p>
-   
-    <code> 
+
+    <code>
     my_easy_hs = highs['easy']
     my_hard_hs = highs['hard']
     </code>
-    
+
     """
-    def __init__(self,fname,limit=10):
+
+    def __init__(self, fname, limit=10):
         self.fname = fname
         self.limit = limit
         self.load()
-        
+
     def load(self):
         """Re-load the high scores.
-        
+
         <pre>Highs.load()</pre>
         """
-        
+
         self._dict = {}
         try:
             f = open(self.fname)
             for line in f.readlines():
-                key,score,name,data = line.strip().split("\t")
+                key, score, name, data = line.strip().split("\t")
                 if key not in self._dict:
-                    self._dict[key] = _High(self,self.limit)
+                    self._dict[key] = _High(self, self.limit)
                 high = self._dict[key]
-                high.submit(int(score),name,data)
+                high.submit(int(score), name, data)
             f.close()
         except:
             pass
-    
+
     def save(self):
         """Save the high scores.
-        
+
         <pre>Highs.save()</pre>
         """
-        
-        f = open(self.fname,"w")
-        for key,high in self._dict.items():
+
+        f = open(self.fname, "w")
+        for key, high in list(self._dict.items()):
             for e in high:
-                f.write("%s\t%d\t%s\t%s\n"%(key,e.score,e.name,str(e.data)))
+                f.write("%s\t%d\t%s\t%s\n" % (key, e.score, e.name, str(e.data)))
         f.close()
-        
-    def __getitem__(self,key):
+
+    def __getitem__(self, key):
         if key not in self._dict:
-            self._dict[key] = _High(self,self.limit)
+            self._dict[key] = _High(self, self.limit)
         return self._dict[key]
```

### Comparing `zanthor-1.2.3/zanthor/pgu/fonts.py` & `zanthor-1.2.4a2/zanthor/pgu/fonts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,130 +1,135 @@
 """Some handy font-like objects.
 
 <p>please note that this file is alpha, and is subject to modification in
 future versions of pgu!</p>
 """
 
-print 'pgu.fonts','This module is alpha, and is subject to change.'
+print("pgu.fonts", "This module is alpha, and is subject to change.")
 
 import pygame
 from pygame.locals import *
 
+
 class TileFont:
     """Creates an instance of the TileFont class.  Interface compatible with pygame.Font
-    
+
     <p>TileFonts are fonts that are stored in a tiled image.  Where the image opaque, it assumed that the font is visible.  Font color is changed automatically, so it does not work with
     fonts with stylized coloring.</p>
-    
+
     <pre>TileFont(fname,size,hints,scale=None,sensitive=False)</pre>
-    
+
     <dl>
     <dt>size <dd>the dimensions of the characters
     <dt>hints <dd>a string of hints "abcdefg..."
     <dt>scale <dd>size to scale font to
     <dt>sensitive <dd>case sensitivity
     </dl>
     """
 
-    def __init__(self,fname,size,hints,scale=None,sensitive=False):
-        
+    def __init__(self, fname, size, hints, scale=None, sensitive=False):
         self.image = pygame.image.load(fname)
-        
-        w,h = self.image.get_width(),self.image.get_height()
-        tw,th = size
-        if not scale: scale = size
+
+        w, h = self.image.get_width(), self.image.get_height()
+        tw, th = size
+        if not scale:
+            scale = size
         self._size = size
         self.scale = scale
-        
+
         self.chars = {}
-        x,y = 0,0
+        x, y = 0, 0
         self.sensitive = sensitive
-        if not self.sensitive: hints = hints.lower()
+        if not self.sensitive:
+            hints = hints.lower()
         for c in hints:
-            if c not in ('\r','\n','\t'):
-                img = self.image.subsurface(x,y,tw,th)
+            if c not in ("\r", "\n", "\t"):
+                img = self.image.subsurface(x, y, tw, th)
                 self.chars[c] = img
                 x += tw
-                if x >= w: x,y = 0,y+th
-                
+                if x >= w:
+                    x, y = 0, y + th
+
         self.colors = {}
-                
-    def size(self,text):
-        tw,th = self.scale
-        return len(text)*tw,th
-        
-    def render(self,text,antialias=0,color=(255,255,255),background=None):
+
+    def size(self, text):
+        tw, th = self.scale
+        return len(text) * tw, th
+
+    def render(self, text, antialias=0, color=(255, 255, 255), background=None):
         size = self.size(text)
         scale = self.scale
-        tw,th = self._size
+        tw, th = self._size
         if background == None:
             s = pygame.Surface(size).convert_alpha()
-            s.fill((0,0,0,0))
+            s.fill((0, 0, 0, 0))
         else:
             s = pygame.Surface(size).convert()
             s.fill(background)
-            
-        if not self.sensitive: text = text.lower()
-        
-        if color not in self.colors: self.colors[color] = {}
+
+        if not self.sensitive:
+            text = text.lower()
+
+        if color not in self.colors:
+            self.colors[color] = {}
         colored = self.colors[color]
-        
-        x,y = 0,0
+
+        x, y = 0, 0
         for c in text:
             if c in self.chars:
                 if c not in colored:
                     img = self.chars[c].convert_alpha()
-                    for yy in xrange(0,th):
-                        for xx in xrange(0,tw):
-                            r,g,b,a = img.get_at((xx,yy))
+                    for yy in range(0, th):
+                        for xx in range(0, tw):
+                            r, g, b, a = img.get_at((xx, yy))
                             if a > 128:
-                                img.set_at((xx,yy),color)
+                                img.set_at((xx, yy), color)
                     colored[c] = img
                 img = colored[c]
-                if scale != (tw,th): img = pygame.transform.scale(img,scale)
-                s.blit(img,(x,y))
+                if scale != (tw, th):
+                    img = pygame.transform.scale(img, scale)
+                s.blit(img, (x, y))
             x += scale[0]
         return s
-        
-        
-class BorderFont: 
+
+
+class BorderFont:
     """a decorator for normal fonts, adds a border. Interface compatible with pygame.Font.
-    
+
     <pre>BorderFont(font,size=1,color=(0,0,0))</pre>
-    
+
     <dl>
     <dt>size <dd>width of border; defaults 0
     <dt>color <dd>color of border; default (0,0,0)
     </dl>
     """
-    def __init__(self,font,size=1,color=(0,0,0)):
-        
+
+    def __init__(self, font, size=1, color=(0, 0, 0)):
         self.font = font
         self._size = size
         self.color = color
-                
-    def size(self,text):
-        w,h = self.font.size(text)
+
+    def size(self, text):
+        w, h = self.font.size(text)
         s = self._size
-        return w+s*2,h+s*2
-        
-    def render(self,text,antialias=0,color=(255,255,255),background=None):
+        return w + s * 2, h + s * 2
+
+    def render(self, text, antialias=0, color=(255, 255, 255), background=None):
         size = self.size(text)
-        
+
         if background == None:
             s = pygame.Surface(size).convert_alpha()
-            s.fill((0,0,0,0))
+            s.fill((0, 0, 0, 0))
         else:
             s = pygame.Surface(size).convert()
             s.fill(background)
-            
-        bg = self.font.render(text,antialias,self.color)
-        fg = self.font.render(text,antialias,color)
-        
+
+        bg = self.font.render(text, antialias, self.color)
+        fg = self.font.render(text, antialias, color)
+
         si = self._size
-        dirs = [(-1,-1),(-1,0),(-1,1),(0,-1),(0,1),(1,-1),(1,0),(1,1)]
-        for dx,dy in dirs: s.blit(bg,(si+dx*si,si+dy*si))
-        s.blit(fg,(si,si))
+        dirs = [(-1, -1), (-1, 0), (-1, 1), (0, -1), (0, 1), (1, -1), (1, 0), (1, 1)]
+        for dx, dy in dirs:
+            s.blit(bg, (si + dx * si, si + dy * si))
+        s.blit(fg, (si, si))
 
         return s
-
-
```

### Comparing `zanthor-1.2.3/zanthor/pgu/vid.py` & `zanthor-1.2.4a2/zanthor/pgu/vid.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,426 +21,445 @@
 """
 
 import pygame
 from pygame.rect import Rect
 from pygame.locals import *
 import math
 
+
 class Sprite:
     """The object used for Sprites.
-    
+
     <pre>Sprite(ishape,pos)</pre>
-    
+
     <dl>
     <dt>ishape <dd>an image, or an image, rectstyle.  The rectstyle will
                 describe the shape of the image, used for collision
                 detection.
     <dt>pos <dd>initial (x,y) position of the Sprite.
     </dl>
-    
+
     <strong>Attributes</strong>
     <dl>
     <dt>rect <dd>the current position of the Sprite
     <dt>_rect <dd>the previous position of the Sprite
     <dt>groups <dd>the groups the Sprite is in
     <dt>agroups <dd>the groups the Sprite can hit in a collision
     <dt>hit <dd>the handler for hits -- hit(g,s,a)
     <dt>loop <dd>the loop handler, called once a frame
     </dl>
     """
-    def __init__(self,ishape,pos):
+
+    def __init__(self, ishape, pos):
         if not isinstance(ishape, tuple):
-            ishape = ishape,None
-        image,shape = ishape
+            ishape = ishape, None
+        image, shape = ishape
         if shape == None:
-            shape = pygame.Rect(0,0,image.get_width(),image.get_height())
-        if isinstance(shape, tuple): shape = pygame.Rect(shape)
+            shape = pygame.Rect(0, 0, image.get_width(), image.get_height())
+        if isinstance(shape, tuple):
+            shape = pygame.Rect(shape)
         self.image = image
         self._image = self.image
         self.shape = shape
-        self.rect = pygame.Rect(pos[0],pos[1],shape.w,shape.h)
+        self.rect = pygame.Rect(pos[0], pos[1], shape.w, shape.h)
         self._rect = pygame.Rect(self.rect)
-        self.irect = pygame.Rect(pos[0]-self.shape.x,pos[1]-self.shape.y,
-            image.get_width(),image.get_height())
+        self.irect = pygame.Rect(
+            pos[0] - self.shape.x,
+            pos[1] - self.shape.y,
+            image.get_width(),
+            image.get_height(),
+        )
         self._irect = pygame.Rect(self.irect)
         self.groups = 0
         self.agroups = 0
         self.updated = 1
-        
-    def setimage(self,ishape):
+
+    def setimage(self, ishape):
         """Set the image of the Sprite.
-        
+
         <pre>Sprite.setimage(ishape)</pre>
-        
+
         <dl>
         <dt>ishape <dd>an image, or an image, rectstyle.  The rectstyle will
                   describe the shape of the image, used for collision detection.
         </dl>
-        """        
+        """
         if not isinstance(ishape, tuple):
-            ishape = ishape,None
-        image,shape = ishape
+            ishape = ishape, None
+        image, shape = ishape
         if shape == None:
-            shape = pygame.Rect(0,0,image.get_width(),image.get_height())
+            shape = pygame.Rect(0, 0, image.get_width(), image.get_height())
         if isinstance(shape, tuple):
             shape = pygame.Rect(shape)
         self.image = image
         self.shape = shape
-        self.rect.w,self.rect.h = shape.w,shape.h
-        self.irect.w,self.irect.h = image.get_width(),image.get_height()
+        self.rect.w, self.rect.h = shape.w, shape.h
+        self.irect.w, self.irect.h = image.get_width(), image.get_height()
         self.updated = 1
 
-        
+
 class Tile:
     """Tile Object used by TileCollide.
-    
+
     <pre>Tile(image=None)</pre>
     <dl>
     <dt>image <dd>an image for the Tile.
     </dl>
-    
+
     <strong>Attributes</strong>
     <dl>
     <dt>agroups <dd>the groups the Tile can hit in a collision
     <dt>hit <dd>the handler for hits -- hit(g,t,a)
     </dl>
     """
-    def __init__(self,image=None):
+
+    def __init__(self, image=None):
         self.image = image
         self.agroups = 0
-        
-    def __setattr__(self,k,v):
-        if k == 'image' and v != None:
+
+    def __setattr__(self, k, v):
+        if k == "image" and v != None:
             self.image_h = v.get_height()
             self.image_w = v.get_width()
         self.__dict__[k] = v
 
+
 class _Sprites(list):
     def __init__(self):
         list.__init__(self)
         self.removed = []
-        
-    def append(self,v):
-        list.append(self,v)
+
+    def append(self, v):
+        list.append(self, v)
         v.updated = 1
-        
-    def remove(self,v):
-        list.remove(self,v)
+
+    def remove(self, v):
+        list.remove(self, v)
         v.updated = 1
         self.removed.append(v)
-        
+
+
 class Vid:
     """An engine for rendering Sprites and Tiles.
-    
+
     <pre>Vid()</pre>
-    
+
     <strong>Attributes</strong>
     <dl>
     <dt>sprites <dd>a list of the Sprites to be displayed.  You may append and
                remove Sprites from it.
-    <dt>images  <dd>a dict for images to be put in.  
+    <dt>images  <dd>a dict for images to be put in.
     <dt>size    <dd>the width, height in Tiles of the layers.  Do not modify.
     <dt>view    <dd>a pygame.Rect of the viewed area.  You may change .x, .y,
                 etc to move the viewed area around.
     <dt>bounds  <dd>a pygame.Rect (set to None by default) that sets the bounds
                 of the viewable area.  Useful for setting certain borders
                 as not viewable.
     <dt>tlayer  <dd>the foreground tiles layer
     <dt>clayer  <dd>the code layer (optional)
     <dt>blayer  <dd>the background tiles layer (optional)
-    <dt>groups  <dd>a hash of group names to group values (32 groups max, as a tile/sprites 
+    <dt>groups  <dd>a hash of group names to group values (32 groups max, as a tile/sprites
             membership in a group is determined by the bits in an integer)
     </dl>
     """
-    
+
     def __init__(self):
-        self.tiles = [None for x in xrange(0,256)]
+        self.tiles = [None for x in range(0, 256)]
         self.sprites = _Sprites()
-        self.images = {} #just a store for images.
+        self.images = {}  # just a store for images.
         self.layers = None
         self.size = None
-        self.view = pygame.Rect(0,0,0,0)
+        self.view = pygame.Rect(0, 0, 0, 0)
         self._view = pygame.Rect(self.view)
         self.bounds = None
         self.updates = []
         self.groups = {}
-    
-        
-    def resize(self,size,bg=0):
+
+    def resize(self, size, bg=0):
         """Resize the layers.
-        
+
         <pre>Vid.resize(size,bg=0)</pre>
-        
-        <dl>        
+
+        <dl>
         <dt>size <dd>w,h in Tiles of the layers
         <dt>bg   <dd>set to 1 if you wish to use both a foreground layer and a
                 background layer
         </dl>
         """
         self.size = size
-        w,h = size
-        self.layers = [[[0 for x in xrange(0,w)] for y in xrange(0,h)]
-            for z in xrange(0,4)]
+        w, h = size
+        self.layers = [
+            [[0 for x in range(0, w)] for y in range(0, h)] for z in range(0, 4)
+        ]
         self.tlayer = self.layers[0]
         self.blayer = self.layers[1]
-        if not bg: self.blayer = None
+        if not bg:
+            self.blayer = None
         self.clayer = self.layers[2]
         self.alayer = self.layers[3]
-        
-        self.view.x, self.view.y = 0,0
-        self._view.x, self.view.y = 0,0
+
+        self.view.x, self.view.y = 0, 0
+        self._view.x, self.view.y = 0, 0
         self.bounds = None
-        
+
         self.updates = []
-    
-    def set(self,pos,v):
+
+    def set(self, pos, v):
         """Set a tile in the foreground to a value.
-        
+
         <p>Use this method to set tiles in the foreground, as it will make
         sure the screen is updated with the change.  Directly changing
         the tlayer will not guarantee updates unless you are using .paint()
         </p>
-        
+
         <pre>Vid.set(pos,v)</pre>
-        
+
         <dl>
         <dt>pos <dd>(x,y) of tile
         <dt>v <dd>value
         </dl>
         """
-        if self.tlayer[pos[1]][pos[0]] == v: return
+        if self.tlayer[pos[1]][pos[0]] == v:
+            return
         self.tlayer[pos[1]][pos[0]] = v
         self.alayer[pos[1]][pos[0]] = 1
         self.updates.append(pos)
-        
-    def get(self,pos):
+
+    def get(self, pos):
         """Get the tlayer at pos.
-        
+
         <pre>Vid.get(pos): return value</pre>
-        
+
         <dl>
         <dt>pos <dd>(x,y) of tile
         </dl>
         """
         return self.tlayer[pos[1]][pos[0]]
-    
-    def paint(self,s):
+
+    def paint(self, s):
         """Paint the screen.
-        
+
         <pre>Vid.paint(screen): return [updates]</pre>
-        
+
         <dl>
         <dt>screen <dd>a pygame.Surface to paint to
         </dl>
-        
+
         <p>returns the updated portion of the screen (all of it)</p>
         """
         return []
-                
-    def update(self,s):
+
+    def update(self, s):
         """Update the screen.
-        
+
         <pre>Vid.update(screen): return [updates]</pre>
-        
+
         <dl>
         <dt>screen <dd>a pygame.Rect to update
         </dl>
-        
+
         <p>returns a list of updated rectangles.</p>
         """
         self.updates = []
         return []
 
-    def tga_load_level(self,fname,bg=0):
-        """Load a TGA level.  
-        
+    def tga_load_level(self, fname, bg=0):
+        """Load a TGA level.
+
         <pre>Vid.tga_load_level(fname,bg=0)</pre>
-        
+
         <dl>
         <dt>g        <dd>a Tilevid instance
         <dt>fname    <dd>tga image to load
         <dt>bg        <dd>set to 1 if you wish to load the background layer
         </dl>
         """
-        if type(fname) == str: img = pygame.image.load(fname)
-        else: img = fname
-        w,h = img.get_width(),img.get_height()
-        self.resize((w,h),bg)
-        for y in range(0,h):
-            for x in range(0,w):
-                t,b,c,_a = img.get_at((x,y))
+        if type(fname) == str:
+            img = pygame.image.load(fname)
+        else:
+            img = fname
+        w, h = img.get_width(), img.get_height()
+        self.resize((w, h), bg)
+        for y in range(0, h):
+            for x in range(0, w):
+                t, b, c, _a = img.get_at((x, y))
                 self.tlayer[y][x] = t
-                if bg: self.blayer[y][x] = b
+                if bg:
+                    self.blayer[y][x] = b
                 self.clayer[y][x] = c
-                
-    def tga_save_level(self,fname):
+
+    def tga_save_level(self, fname):
         """Save a TGA level.
-        
+
         <pre>Vid.tga_save_level(fname)</pre>
-        
+
         <dl>
         <dt>fname <dd>tga image to save to
         </dl>
         """
-        w,h = self.size
-        img = pygame.Surface((w,h),SWSURFACE,32)
-        img.fill((0,0,0,0))
-        for y in range(0,h):
-            for x in range(0,w):
+        w, h = self.size
+        img = pygame.Surface((w, h), SWSURFACE, 32)
+        img.fill((0, 0, 0, 0))
+        for y in range(0, h):
+            for x in range(0, w):
                 t = self.tlayer[y][x]
                 b = 0
                 if self.blayer:
                     b = self.blayer[y][x]
                 c = self.clayer[y][x]
                 _a = 0
-                img.set_at((x,y),(t,b,c,_a))
-        pygame.image.save(img,fname)
-                
-                
+                img.set_at((x, y), (t, b, c, _a))
+        pygame.image.save(img, fname)
 
-    def tga_load_tiles(self,fname,size,tdata={}):
+    def tga_load_tiles(self, fname, size, tdata={}):
         """Load a TGA tileset.
-        
+
         <pre>Vid.tga_load_tiles(fname,size,tdata={})</pre>
-        
+
         <dl>
         <dt>g       <dd>a Tilevid instance
         <dt>fname    <dd>tga image to load
         <dt>size    <dd>(w,h) size of tiles in pixels
         <dt>tdata    <dd>tile data, a dict of tile:(agroups, hit handler, config)
         </dl>
         """
-        TW,TH = size
-        if type(fname) == str: img = pygame.image.load(fname).convert_alpha()
-        else: img = fname
-        w,h = img.get_width(),img.get_height()
-        
+        TW, TH = size
+        if type(fname) == str:
+            try:
+                img = pygame.image.load(fname)
+            except:
+                img = pygame.image.load(fname.replace("tga", "png"))
+            img = img.convert_alpha()
+        else:
+            img = fname
+        w, h = img.get_width(), img.get_height()
+
         n = 0
-        for y in range(0,h,TH):
-            for x in range(0,w,TW):
-                i = img.subsurface((x,y,TW,TH))
+        for y in range(0, h, TH):
+            for x in range(0, w, TW):
+                i = img.subsurface((x, y, TW, TH))
                 tile = Tile(i)
                 self.tiles[n] = tile
                 if n in tdata:
-                    agroups,hit,config = tdata[n]
+                    agroups, hit, config = tdata[n]
                     tile.agroups = self.string2groups(agroups)
                     tile.hit = hit
                     tile.config = config
                 n += 1
 
-
-    def load_images(self,idata):
+    def load_images(self, idata):
         """Load images.
-        
+
         <pre>Vid.load_images(idata)</pre>
-        
+
         <dl>
         <dt>idata <dd>a list of (name, fname, shape)
         </dl>
         """
-        for name,fname,shape in idata:
-            self.images[name] = pygame.image.load(fname).convert_alpha(),shape
+        for name, fname, shape in idata:
+            self.images[name] = pygame.image.load(fname).convert_alpha(), shape
 
-    def run_codes(self,cdata,rect):
+    def run_codes(self, cdata, rect):
         """Run codes.
-        
+
         <pre>Vid.run_codes(cdata,rect)</pre>
-        
+
         <dl>
         <dt>cdata <dd>a dict of code:(handler function, value)
         <dt>rect <dd>a tile rect of the parts of the layer that should have
                  their codes run
         </dl>
         """
-        tw,th = self.tiles[0].image.get_width(),self.tiles[0].image.get_height()
+        tw, th = self.tiles[0].image.get_width(), self.tiles[0].image.get_height()
 
-        x1,y1,w,h = rect
+        x1, y1, w, h = rect
         clayer = self.clayer
         t = Tile()
-        for y in range(y1,y1+h):
-            for x in range(x1,x1+w):
+        for y in range(y1, y1 + h):
+            for x in range(x1, x1 + w):
                 n = clayer[y][x]
                 if n in cdata:
-                    fnc,value = cdata[n]
-                    t.tx,t.ty = x,y
-                    t.rect = pygame.Rect(x*tw,y*th,tw,th)
-                    fnc(self,t,value)
+                    fnc, value = cdata[n]
+                    t.tx, t.ty = x, y
+                    t.rect = pygame.Rect(x * tw, y * th, tw, th)
+                    fnc(self, t, value)
 
-        
-    def string2groups(self,str):
+    def string2groups(self, str):
         """Convert a string to groups.
-        
+
         <pre>Vid.string2groups(str): return groups</pre>
         """
-        if str == None: return 0
+        if str == None:
+            return 0
         return self.list2groups(str.split(","))
 
-    def list2groups(self,igroups):
+    def list2groups(self, igroups):
         """Convert a list to groups.
         <pre>Vid.list2groups(igroups): return groups</pre>
         """
         for s in igroups:
             if not s in self.groups:
-                self.groups[s] = 2**len(self.groups)
+                self.groups[s] = 2 ** len(self.groups)
         v = 0
-        for s,n in self.groups.items():
-            if s in igroups: v|=n
+        for s, n in list(self.groups.items()):
+            if s in igroups:
+                v |= n
         return v
 
-    def groups2list(self,groups):
+    def groups2list(self, groups):
         """Convert a groups to a list.
         <pre>Vid.groups2list(groups): return list</pre>
         """
         v = []
-        for s,n in self.groups.items():
-            if (n&groups)!=0: v.append(s)
+        for s, n in list(self.groups.items()):
+            if (n & groups) != 0:
+                v.append(s)
         return v
 
-    def hit(self,x,y,t,s):
+    def hit(self, x, y, t, s):
         tiles = self.tiles
-        tw,th = tiles[0].image.get_width(),tiles[0].image.get_height()
+        tw, th = tiles[0].image.get_width(), tiles[0].image.get_height()
         t.tx = x
         t.ty = y
-        t.rect = Rect(x*tw,y*th,tw,th)
+        t.rect = Rect(x * tw, y * th, tw, th)
         t._rect = t.rect
-        if hasattr(t,'hit'):
-            t.hit(self,t,s)
+        if hasattr(t, "hit"):
+            t.hit(self, t, s)
 
     def loop(self):
         """Update and hit testing loop.  Run this once per frame.
         <pre>Vid.loop()</pre>
         """
-        self.loop_sprites() #sprites may move
-        self.loop_tilehits() #sprites move
-        self.loop_spritehits() #no sprites should move
+        self.loop_sprites()  # sprites may move
+        self.loop_tilehits()  # sprites move
+        self.loop_spritehits()  # no sprites should move
         for s in self.sprites:
             s._rect = pygame.Rect(s.rect)
-        
+
     def loop_sprites(self):
         for s in self.sprites[:]:
-            if hasattr(s,'loop'):
-                s.loop(self,s)
+            if hasattr(s, "loop"):
+                s.loop(self, s)
 
     def loop_tilehits(self):
         tiles = self.tiles
-        tw,th = tiles[0].image.get_width(),tiles[0].image.get_height()
+        tw, th = tiles[0].image.get_width(), tiles[0].image.get_height()
 
         layer = self.layers[0]
 
         for s in self.sprites[:]:
             self._tilehits(s)
-    
-    def _tilehits(self,s):
+
+    def _tilehits(self, s):
         tiles = self.tiles
-        tw,th = tiles[0].image.get_width(),tiles[0].image.get_height()
+        tw, th = tiles[0].image.get_width(), tiles[0].image.get_height()
         layer = self.layers[0]
-        
-        for _z in (0,): 
-            if s.groups != 0:
 
+        for _z in (0,):
+            if s.groups != 0:
                 _rect = s._rect
                 rect = s.rect
 
                 _rectx = _rect.x
                 _recty = _rect.y
                 _rectw = _rect.w
                 _recth = _rect.h
@@ -450,108 +469,115 @@
                 rectw = rect.w
                 recth = rect.h
 
                 rect.y = _rect.y
                 rect.h = _rect.h
 
                 hits = []
-                ct,cb,cl,cr = rect.top,rect.bottom,rect.left,rect.right
-                #nasty ol loops
-                y = ct/th*th
+                ct, cb, cl, cr = rect.top, rect.bottom, rect.left, rect.right
+                # nasty ol loops
+                y = ct // th * th
                 while y < cb:
-                    x = cl/tw*tw
-                    yy = y/th
+                    x = cl // tw * tw
+                    yy = y // th
                     while x < cr:
-                        xx = x/tw
+                        xx = x // tw
                         t = tiles[layer[yy][xx]]
-                        if (s.groups & t.agroups)!=0:
-                            #self.hit(xx,yy,t,s)
-                            d = math.hypot(rect.centerx-(xx*tw+tw/2),
-                                rect.centery-(yy*th+th/2))
-                            hits.append((d,t,xx,yy))
+                        if (s.groups & t.agroups) != 0:
+                            # self.hit(xx,yy,t,s)
+                            d = math.hypot(
+                                rect.centerx - (xx * tw + tw // 2),
+                                rect.centery - (yy * th + th // 2),
+                            )
+                            hits.append((d, t, xx, yy))
 
                         x += tw
                     y += th
-                
+
                 hits.sort()
-                #if len(hits) > 0: print self.frame,hits
-                for d,t,xx,yy in hits:
-                    self.hit(xx,yy,t,s)
-                
-                #switching directions...
+                # if len(hits) > 0: print self.frame,hits
+                for d, t, xx, yy in hits:
+                    self.hit(xx, yy, t, s)
+
+                # switching directions...
                 _rect.x = rect.x
                 _rect.w = rect.w
                 rect.y = recty
                 rect.h = recth
 
                 hits = []
-                ct,cb,cl,cr = rect.top,rect.bottom,rect.left,rect.right
-                #nasty ol loops
-                y = ct/th*th
+                ct, cb, cl, cr = rect.top, rect.bottom, rect.left, rect.right
+                # nasty ol loops
+                y = ct // th * th
                 while y < cb:
-                    x = cl/tw*tw
-                    yy = y/th
+                    x = cl // tw * tw
+                    yy = y // th
                     while x < cr:
-                        xx = x/tw
+                        xx = x // tw
                         t = tiles[layer[yy][xx]]
-                        if (s.groups & t.agroups)!=0:
-                            d = math.hypot(rect.centerx-(xx*tw+tw/2),
-                                rect.centery-(yy*th+th/2))
-                            hits.append((d,t,xx,yy))
-                            #self.hit(xx,yy,t,s)
+                        if (s.groups & t.agroups) != 0:
+                            d = math.hypot(
+                                rect.centerx - (xx * tw + tw // 2),
+                                rect.centery - (yy * th + th // 2),
+                            )
+                            hits.append((d, t, xx, yy))
+                            # self.hit(xx,yy,t,s)
                         x += tw
                     y += th
-                
-                hits.sort()    
-                #if len(hits) > 0: print self.frame,hits
-                for d,t,xx,yy in hits:
-                    self.hit(xx,yy,t,s)
 
-                #done with loops
+                hits.sort()
+                # if len(hits) > 0: print self.frame,hits
+                for d, t, xx, yy in hits:
+                    self.hit(xx, yy, t, s)
+
+                # done with loops
                 _rect.x = _rectx
                 _rect.y = _recty
 
-
     def loop_spritehits(self):
         as_sprites = self.sprites[:]
         groups = {}
-        for n in range(0,31):
-            groups[1<<n] = []
+        for n in range(0, 31):
+            groups[1 << n] = []
         for s in as_sprites:
             g = s.groups
             n = 1
             while g:
-                if (g&1)!=0: groups[n].append(s)
+                if (g & 1) != 0:
+                    groups[n].append(s)
                 g >>= 1
                 n <<= 1
-                
+
         for s in as_sprites:
-            if s.agroups!=0:
-                rect1,rect2 = s.rect,Rect(s.rect)
-                #if rect1.centerx < 320: rect2.x += 640
-                #else: rect2.x -= 640
+            if s.agroups != 0:
+                rect1, rect2 = s.rect, Rect(s.rect)
+                # if rect1.centerx < 320: rect2.x += 640
+                # else: rect2.x -= 640
                 g = s.agroups
                 n = 1
                 while g:
-                    if (g&1)!=0:
-                        for b in groups[n]:    
-                            if (s != b and (s.agroups & b.groups)!=0
-                                    and s.rect.colliderect(b.rect)):
-                                s.hit(self,s,b)
+                    if (g & 1) != 0:
+                        for b in groups[n]:
+                            if (
+                                s != b
+                                and (s.agroups & b.groups) != 0
+                                and s.rect.colliderect(b.rect)
+                            ):
+                                s.hit(self, s, b)
 
                     g >>= 1
                     n <<= 1
 
-
-    def screen_to_tile(self,pos):
+    def screen_to_tile(self, pos):
         """Convert a screen position to a tile position.
         <pre>Vid.screen_to_tile(pos): return pos</pre>
         """
         return pos
-        
-    def tile_to_screen(self,pos):
+
+    def tile_to_screen(self, pos):
         """Convert a tile position to a screen position.
         <pre>Vid.tile_to_screen(pos): return pos</pre>
         """
         return pos
-                    
+
+
 # vim: set filetype=python sts=4 sw=4 noet si :
```

### Comparing `zanthor-1.2.3/zanthor/pgu/ani.py` & `zanthor-1.2.4a2/zanthor/pgu/ani.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 """animation loading and manipulating functions.
 
 <p>please note that this file is alpha, and is subject to modification in
 future versions of pgu!</p>
 """
 
-print 'pgu.ani','This module is alpha, and is subject to change.'
+print("pgu.ani", "This module is alpha, and is subject to change.")
 
 import math
 import pygame
 
-def _ani_load(tv,name,parts,frames,shape):
+
+def _ani_load(tv, name, parts, frames, shape):
     l = len(frames)
-    #print name,parts,l
+    # print name,parts,l
     n = parts.pop()
     if len(parts):
-        s = l/n
-        for i in xrange(0,n):
-            _ani_load(tv,name + ".%d"%i,parts[:],frames[s*i:s*(i+1)],shape)
+        s = l / n
+        for i in range(0, n):
+            _ani_load(
+                tv, name + ".%d" % i, parts[:], frames[s * i : s * (i + 1)], shape
+            )
         return
-    
-    for i in xrange(0,n):
-        tv.images[name+".%d"%i] = frames[i],shape
 
-def ani_load(tv,name,img,size,shape,parts):
+    for i in range(0, n):
+        tv.images[name + ".%d" % i] = frames[i], shape
+
+
+def ani_load(tv, name, img, size, shape, parts):
     """load an animation from an image
-    
+
     <pre>ani_load(tv,name,image,size,shape,parts)</pre>
-    
+
     <dl>
     <dt>tv<dd>vid to load into
     <dt>name <dd>prefix name to give the images
     <dt>image <dd>image to load anis from
     <dt>size <dd>w,h size of image
     <dt>shape <dd>shape of image (usually a subset of 0,0,w,h) used for collision detection
-    <dt>parts <dd>list of parts to divide the animation into 
+    <dt>parts <dd>list of parts to divide the animation into
         <br>for example parts = [4,5] would yield 4 animations 5 frames long, 20 total
         <br>for example parts = [a,b,c] would yield ... images['name.a.b.c'] ..., a*b*c total
     </dl>
-    
+
     """
     parts = parts[:]
     parts.reverse()
-    w,h = size
+    w, h = size
     frames = []
-    for y in xrange(0,img.get_height(),h):
-        for x in xrange(0,img.get_width(),w):
-            frames.append(img.subsurface(x,y,w,h))
-    _ani_load(tv,name,parts,frames,shape)
-    
-    
-def image_rotate(tv,name,img,shape,angles,diff=0):
+    for y in range(0, img.get_height(), h):
+        for x in range(0, img.get_width(), w):
+            frames.append(img.subsurface(x, y, w, h))
+    _ani_load(tv, name, parts, frames, shape)
+
+
+def image_rotate(tv, name, img, shape, angles, diff=0):
     """rotate an image and put it into tv.images
-    
+
     <pre>image_rotate(tv,name,image,shape,angles,diff=0)</pre>
-    
+
     <dl>
     <dt>tv <dd>vid to load into
     <dt>name <dd>prefix name to give the images
     <dt>image <dd>image to load anis from
     <dt>shape <dd>shape fimage (usually a subset of 0,0,w,h) used for collision detection
     <dt>angles <dd>a list of angles to render in degrees
     <dt>diff <dd>a number to add to the angles, to correct for source image not actually being at 0 degrees
     </dl>
     """
-    w1,h1 = img.get_width(),img.get_height()
+    w1, h1 = img.get_width(), img.get_height()
     shape = pygame.Rect(shape)
-    ps = shape.topleft,shape.topright,shape.bottomleft,shape.bottomright
+    ps = shape.topleft, shape.topright, shape.bottomleft, shape.bottomright
     for a in angles:
-        img2 = pygame.transform.rotate(img,a+diff)
-        w2,h2 = img2.get_width(),img2.get_height()
-        minx,miny,maxx,maxy = 1024,1024,0,0
-        for x,y in ps:
-            x,y = x-w1/2,y-h1/2
-            a2 = math.radians(a+diff)
-            #NOTE: the + and - are switched from the normal formula because of
-            #the weird way that pygame does the angle...
-            x2 = x*math.cos(a2) + y*math.sin(a2) 
-            y2 = y*math.cos(a2) - x*math.sin(a2)
-            x2,y2 = x2+w2/2,y2+h2/2
-            minx = min(minx,x2)
-            miny = min(miny,y2)
-            maxx = max(maxx,x2)
-            maxy = max(maxy,y2)
-        r = pygame.Rect(minx,miny,maxx-minx,maxy-miny)
-        #print r
-        #((ww-w)/2,(hh-h)/2,w,h)
-        tv.images["%s.%d"%(name,a)] = img2,r
-        
-
+        img2 = pygame.transform.rotate(img, a + diff)
+        w2, h2 = img2.get_width(), img2.get_height()
+        minx, miny, maxx, maxy = 1024, 1024, 0, 0
+        for x, y in ps:
+            x, y = x - w1 / 2, y - h1 / 2
+            a2 = math.radians(a + diff)
+            # NOTE: the + and - are switched from the normal formula because of
+            # the weird way that pygame does the angle...
+            x2 = x * math.cos(a2) + y * math.sin(a2)
+            y2 = y * math.cos(a2) - x * math.sin(a2)
+            x2, y2 = x2 + w2 / 2, y2 + h2 / 2
+            minx = min(minx, x2)
+            miny = min(miny, y2)
+            maxx = max(maxx, x2)
+            maxy = max(maxy, y2)
+        r = pygame.Rect(minx, miny, maxx - minx, maxy - miny)
+        # print r
+        # ((ww-w)/2,(hh-h)/2,w,h)
+        tv.images["%s.%d" % (name, a)] = img2, r
```

### Comparing `zanthor-1.2.3/zanthor/pgu/hexvid.py` & `zanthor-1.2.4a2/zanthor/pgu/hexvid.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,123 +5,127 @@
 terrains, however.  If you are able to update it and use it in a real game,
 help would be greatly appreciated!</p>
 
 <p>please note that this file is alpha, and is subject to modification in
 future versions of pgu!</p>
 
 """
-print 'pgu.hexvid','This module is alpha, and is subject to change.'
+print("pgu.hexvid", "This module is alpha, and is subject to change.")
 
 from pgu.vid import *
 import pygame
 
 
 class Hexvid(Vid):
     """Create an hex vid engine.  See [[vid]]"""
-    def update(self,screen):
+
+    def update(self, screen):
         return self.paint(screen)
-    
-    def paint(self,screen):
-        sw,sh = screen.get_width(),screen.get_height()
-        self.view.w,self.view.h = sw,sh
-        
+
+    def paint(self, screen):
+        sw, sh = screen.get_width(), screen.get_height()
+        self.view.w, self.view.h = sw, sh
+
         tlayer = self.tlayer
         blayer = self.blayer
-        #zlayer = self.zlayer
-        w,h = len(tlayer[0]),len(tlayer)
-        
-        #iso_w,iso_h,iso_z,tile_w,tile_h,base_w,base_h = self.iso_w,self.iso_h,self.iso_z,self.tile_w,self.tile_h,self.base_w,self.base_h
-        
-        tile_w,tile_h = self.tile_w,self.tile_h
-        tile_w2,tile_h2 = tile_w/2,tile_h/2
-        
+        # zlayer = self.zlayer
+        w, h = len(tlayer[0]), len(tlayer)
+
+        # iso_w,iso_h,iso_z,tile_w,tile_h,base_w,base_h = self.iso_w,self.iso_h,self.iso_z,self.tile_w,self.tile_h,self.base_w,self.base_h
+
+        tile_w, tile_h = self.tile_w, self.tile_h
+        tile_w2, tile_h2 = tile_w / 2, tile_h / 2
+
         view = self.view
-        adj = self.adj = pygame.Rect(-self.view.x,-self.view.y,0,0)
-        
-        w,h = len(tlayer[0]),len(tlayer)
+        adj = self.adj = pygame.Rect(-self.view.x, -self.view.y, 0, 0)
+
+        w, h = len(tlayer[0]), len(tlayer)
         tiles = self.tiles
-        
-        #""
+
+        # ""
         if self.bounds == None:
-            tmp,y1 = self.tile_to_view((0,0))
-            x1,tmp = self.tile_to_view((0,h+1))
-            tmp,y2 = self.tile_to_view((w+1,h+1))
-            x2,tmp = self.tile_to_view((w+1,0))
-            self.bounds = pygame.Rect(x1,y1,x2-x1,y2-y1)
-            print self.bounds
-        #""
-        
-        if self.bounds != None: self.view.clamp_ip(self.bounds)
-
-        ox,oy = self.screen_to_tile((0,0))
-        sx,sy = self.tile_to_view((ox,oy))
-        dx,dy = sx - self.view.x,sy - self.view.y
-        
+            tmp, y1 = self.tile_to_view((0, 0))
+            x1, tmp = self.tile_to_view((0, h + 1))
+            tmp, y2 = self.tile_to_view((w + 1, h + 1))
+            x2, tmp = self.tile_to_view((w + 1, 0))
+            self.bounds = pygame.Rect(x1, y1, x2 - x1, y2 - y1)
+            print(self.bounds)
+        # ""
+
+        if self.bounds != None:
+            self.view.clamp_ip(self.bounds)
+
+        ox, oy = self.screen_to_tile((0, 0))
+        sx, sy = self.tile_to_view((ox, oy))
+        dx, dy = sx - self.view.x, sy - self.view.y
+
         bot = 1
-        
-        tile_wi = tile_w + tile_w/2
-        tile_wi2 = tile_wi/2
-        
-        #dx += tile_w/2
-        
-        for i2 in xrange(-bot,self.view.h/tile_h2+bot*3): #NOTE: 3 seems a bit much, but it works.
-            tx,ty = ox + i2/2 + i2%2,oy + i2/2
-            x,y = (i2%2)*tile_wi2 + dx,i2*tile_h2 + dy
-            
-            #to adjust for the -1 in i1
-            x,tx,ty = x-tile_wi,tx-1,ty+1
-            
-            x -= tile_w/2
-            for i1 in xrange(-1,self.view.w/tile_wi+1):
+
+        tile_wi = tile_w + tile_w / 2
+        tile_wi2 = tile_wi / 2
+
+        # dx += tile_w/2
+
+        for i2 in range(
+            -bot, self.view.h / tile_h2 + bot * 3
+        ):  # NOTE: 3 seems a bit much, but it works.
+            tx, ty = ox + i2 / 2 + i2 % 2, oy + i2 / 2
+            x, y = (i2 % 2) * tile_wi2 + dx, i2 * tile_h2 + dy
+
+            # to adjust for the -1 in i1
+            x, tx, ty = x - tile_wi, tx - 1, ty + 1
+
+            x -= tile_w / 2
+            for i1 in range(-1, self.view.w / tile_wi + 1):
                 if ty >= 0 and ty < h and tx >= 0 and tx < w:
                     if blayer != None:
                         n = blayer[ty][tx]
                         if n != 0:
                             t = tiles[n]
                             if t != None and t.image != None:
-                                screen.blit(t.image,(x,y))
+                                screen.blit(t.image, (x, y))
                     n = tlayer[ty][tx]
                     if n != 0:
                         t = tiles[n]
                         if t != None and t.image != None:
-                            screen.blit(t.image,(x,y))
-                            
-            
+                            screen.blit(t.image, (x, y))
+
                 tx += 1
                 ty -= 1
-                x += tile_wi 
+                x += tile_wi
 
-        return [pygame.Rect(0,0,screen.get_width(),screen.get_height())]
-    
-    def view_to_tile(self,pos):
-        x,y = pos
-        #x = x + (self.tile_w*1/2)
-        
-        x,y = int(x*4/(self.tile_w*3)), y*2/self.tile_h
+        return [pygame.Rect(0, 0, screen.get_width(), screen.get_height())]
+
+    def view_to_tile(self, pos):
+        x, y = pos
+        # x = x + (self.tile_w*1/2)
+
+        x, y = int(x * 4 / (self.tile_w * 3)), y * 2 / self.tile_h
         nx = (x + y) / 2
         ny = (y - x) / 2
-        return nx,ny
-    
-    def tile_to_view(self,pos):
-        x,y = pos
+        return nx, ny
+
+    def tile_to_view(self, pos):
+        x, y = pos
         nx = x - y
         ny = x + y
-        nx,ny = int(nx*(self.tile_w*3)/4), ny*self.tile_h/2
-        
-        #nx = nx - (self.tile_w*1/2)
-        return nx,ny
-            
-    def screen_to_tile(self,pos): #NOTE HACK : not sure if the 3/8 is right or not, but it is pretty close...
-        pos = pos[0]+self.view.x + self.tile_w*3/8,pos[1]+self.view.y
+        nx, ny = int(nx * (self.tile_w * 3) / 4), ny * self.tile_h / 2
+
+        # nx = nx - (self.tile_w*1/2)
+        return nx, ny
+
+    def screen_to_tile(
+        self, pos
+    ):  # NOTE HACK : not sure if the 3/8 is right or not, but it is pretty close...
+        pos = pos[0] + self.view.x + self.tile_w * 3 / 8, pos[1] + self.view.y
         pos = self.view_to_tile(pos)
         return pos
-    
-    def tile_to_screen(self,pos):
+
+    def tile_to_screen(self, pos):
         pos = self.tile_to_view(pos)
-        pos = pos[0]-self.view.x,pos[1]-self.view.y
+        pos = pos[0] - self.view.x, pos[1] - self.view.y
         return pos
-    
-        
-    def tga_load_tiles(self,fname,size,tdata={}):
-        Vid.tga_load_tiles(self,fname,size,tdata)
-        
-        self.tile_w,self.tile_h = size
+
+    def tga_load_tiles(self, fname, size, tdata={}):
+        Vid.tga_load_tiles(self, fname, size, tdata)
+
+        self.tile_w, self.tile_h = size
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/app.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,218 +1,227 @@
 """
 """
 import pygame
 from pygame.locals import *
 
-import container
-from const import *
+from . import container
+from .const import *
+
 
 class App(container.Container):
     """The top-level widget for an application.
-    
+
     <pre>App(theme=None)</pre>
-    
+
     <dl>
     <dt>theme<dd>an instance of a Theme, optional as it will use the default Theme class.
     </dl>
-    
+
     <strong>Basic Example</strong>
     <code>
     app = gui.App()
     app.run(widget=widget,screen=screen)
     </code>
-    
+
     <strong>Integrated Example</strong>
     <code>
     app = gui.App()
     gui.init(widget=widget)
     while 1:
         for e in pygame.event.get():
             app.event(e)
         app.update(screen)
     </code>
-        
-    
-    
+
+
+
     """
-    def __init__(self,theme=None,**params):
+
+    def __init__(self, theme=None, **params):
         App.app = self
-        
-        if theme == None: 
-            from theme import Theme
+
+        if theme == None:
+            from .theme import Theme
+
             theme = Theme()
         self.theme = theme
-        
-        params['decorate'] = 'app'
-        container.Container.__init__(self,**params)
+
+        params["decorate"] = "app"
+        container.Container.__init__(self, **params)
         self._quit = False
         self.widget = None
         self._chsize = False
         self._repaint = False
-        
+
         self.screen = None
         self.container = None
         self.events = []
-        
+
     def resize(self):
-            
         screen = self.screen
         w = self.widget
         wsize = 0
-        
-        #5 cases
-        
-        #input screen is already set use its size
+
+        # 5 cases
+
+        # input screen is already set use its size
         if screen:
             self.screen = screen
-            width,height = screen.get_width(),screen.get_height()
-        
-        #display.screen
+            width, height = screen.get_width(), screen.get_height()
+
+        # display.screen
         elif pygame.display.get_surface():
             screen = pygame.display.get_surface()
             self.screen = screen
-            width,height = screen.get_width(),screen.get_height()
-        
-        #app has width,height
+            width, height = screen.get_width(), screen.get_height()
+
+        # app has width,height
         elif self.style.width != 0 and self.style.height != 0:
-            screen = pygame.display.set_mode((self.style.width,self.style.height),SWSURFACE)
+            screen = pygame.display.set_mode(
+                (self.style.width, self.style.height), SWSURFACE
+            )
             self.screen = screen
-            width,height = screen.get_width(),screen.get_height()
-        
-        #widget has width,height, or its own size..
+            width, height = screen.get_width(), screen.get_height()
+
+        # widget has width,height, or its own size..
         else:
             wsize = 1
-            width,height = w.rect.w,w.rect.h = w.resize()
-            #w._resize()
-            screen = pygame.display.set_mode((width,height),SWSURFACE)
+            width, height = w.rect.w, w.rect.h = w.resize()
+            # w._resize()
+            screen = pygame.display.set_mode((width, height), SWSURFACE)
             self.screen = screen
-        
-        #use screen to set up size of this widget
-        self.style.width,self.style.height = width,height
-        self.rect.w,self.rect.h = width,height
-        self.rect.x,self.rect.y = 0,0
-        
-        w.rect.x,w.rect.y = 0,0
-        w.rect.w,w.rect.h = w.resize(width,height)
-        
+
+        # use screen to set up size of this widget
+        self.style.width, self.style.height = width, height
+        self.rect.w, self.rect.h = width, height
+        self.rect.x, self.rect.y = 0, 0
+
+        w.rect.x, w.rect.y = 0, 0
+        w.rect.w, w.rect.h = w.resize(width, height)
+
         for w in self.windows:
-            w.rect.w,w.rect.h = w.resize()
+            w.rect.w, w.rect.h = w.resize()
 
-    
-    def init(self,widget=None,screen=None): #TODO widget= could conflict with module widget
+    def init(
+        self, widget=None, screen=None
+    ):  # TODO widget= could conflict with module widget
         """Initialize the application.
-        
+
         <pre>App.init(widget=None,screen=None)</pre>
-        
+
         <dl>
         <dt>widget<dd>main widget
         <dt>screen<dd>pygame.Surface to render to
         </dl>
         """
-        
+
         App.app = self
-        
-        if widget: self.widget = widget
-        if screen: self.screen = screen
-        
-        self.resize()   
-        
-        w = self.widget     
-        
+
+        if widget:
+            self.widget = widget
+        if screen:
+            self.screen = screen
+
+        self.resize()
+
+        w = self.widget
+
         self.widgets = []
         self.widgets.append(w)
         w.container = self
         self.focus(w)
-        
-        pygame.key.set_repeat(500,30)
-        
+
+        pygame.key.set_repeat(500, 30)
+
         self._repaint = True
         self._quit = False
-        
+
         self.send(INIT)
-    
-    def event(self,e):
+
+    def event(self, e):
         """Pass an event to the main widget.
-        
+
         <pre>App.event(e)</pre>
-        
+
         <dl>
         <dt>e<dd>event
         </dl>
         """
         App.app = self
-        #NOTE: might want to deal with ACTIVEEVENT in the future.
-        self.send(e.type,e)
-        container.Container.event(self,e)
+        # NOTE: might want to deal with ACTIVEEVENT in the future.
+        self.send(e.type, e)
+        container.Container.event(self, e)
         if e.type == MOUSEBUTTONUP:
-            sub = pygame.event.Event(CLICK,{
-                'button':e.button,
-                'pos':e.pos})
-            self.send(sub.type,sub)
-            container.Container.event(self,sub)
-            
-            
+            sub = pygame.event.Event(CLICK, {"button": e.button, "pos": e.pos})
+            self.send(sub.type, sub)
+            container.Container.event(self, sub)
 
-    
     def loop(self):
         App.app = self
         s = self.screen
         for e in pygame.event.get():
             if not (e.type == QUIT and self.mywindow):
                 self.event(e)
         us = self.update(s)
         pygame.display.update(us)
-        
-
 
-    def update(self,screen):
+    def update(self, screen):
         """Update the screen.
-        
+
         <dl>
         <dt>screen<dd>pygame surface
         </dl>
         """
         if self._chsize:
             self.resize()
             self._chsize = False
         if self._repaint:
-            if hasattr(self,'background'):
+            if hasattr(self, "background"):
                 self.background.paint(screen)
             self.paint(screen)
             self._repaint = False
-            return [pygame.Rect(0,0,screen.get_width(),screen.get_height())]
+            return [pygame.Rect(0, 0, screen.get_width(), screen.get_height())]
         else:
-            us = container.Container.update(self,screen)
+            us = container.Container.update(self, screen)
             return us
-    
-    def run(self,widget=None,screen=None): 
+
+    def run(self, widget=None, screen=None):
         """Run an application.
-        
+
         <p>Automatically calls <tt>App.init</tt> and then forever loops <tt>App.event</tt> and <tt>App.update</tt></p>
-        
+
         <dl>
         <dt>widget<dd>main widget
         <dt>screen<dd>pygame.Surface to render to
         </dl>
         """
-        self.init(widget,screen)
+        self.init(widget, screen)
         while not self._quit:
             self.loop()
             pygame.time.wait(10)
-    
-    def reupdate(self,w=None): pass
-    def repaint(self,w=None): self._repaint = True
-    def repaintall(self): self._repaint = True
+
+    def reupdate(self, w=None):
+        pass
+
+    def repaint(self, w=None):
+        self._repaint = True
+
+    def repaintall(self):
+        self._repaint = True
+
     def chsize(self):
         self._chsize = True
         self._repaint = True
-    
-    def quit(self,value=None): self._quit = True
+
+    def quit(self, value=None):
+        self._quit = True
+
 
 class Desktop(App):
     """Create an App using the <tt>desktop</tt> theme class.
-    
+
     <pre>Desktop()</pre>
     """
-    def __init__(self,**params):
-        params.setdefault('cls','desktop')
-        App.__init__(self,**params)
+
+    def __init__(self, **params):
+        params.setdefault("cls", "desktop")
+        App.__init__(self, **params)
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/table.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,332 +1,364 @@
 """
 """
-from const import *
-import container
+from .const import *
+from . import container
 
 
 class Table(container.Container):
     """A table style container.
-    
+
     <p>If you know HTML, this should all work roughly how you would expect.  If you are not
     familiar with HTML, please read <a href="http://www.w3.org/TR/REC-html40/struct/tables.html">Tables in HTML Documents</a>.  Pay attention to TABLE, TR, TD related parts of the document.</p>
-    
+
     <pre>Table()</pre>
-    
+
     <strong>Example</strong>
     <code>
     t = gui.Table()
-    
+
     t.tr()
     t.td(gui.Label("First Name"), align=-1)
     t.td(gui.Input())
 
     t.tr()
     t.td(gui.Label("Last Name"), align=-1)
     t.td(gui.Input())
     </code>
-        
+
     """
-    
-    
+
     def __init__(self, **params):
-        params.setdefault('cls','table')
+        params.setdefault("cls", "table")
         container.Container.__init__(self, **params)
         self._rows = []
         self._curRow = 0
         self._trok = False
-    
+
     def getRows(self):
         return len(self._rows)
-    
+
     def getColumns(self):
         if self._rows:
             return len(self._rows[0])
         else:
             return 0
-    
-    def remove_row(self, n): #NOTE: won't work in all cases.
+
+    def remove_row(self, n):  # NOTE: won't work in all cases.
         if n >= self.getRows():
-            print "Trying to remove a nonexistant row:", n, "there are only", self.getRows(), "rows"
+            print(
+                "Trying to remove a nonexistant row:",
+                n,
+                "there are only",
+                self.getRows(),
+                "rows",
+            )
             return
-        
+
         for cell in self._rows[n]:
             if isinstance(cell, dict) and cell["widget"] in self.widgets:
-                #print 'removing widget'
+                # print 'removing widget'
                 self.widgets.remove(cell["widget"])
         del self._rows[n]
-        #print "got here"
-        
+        # print "got here"
+
         for w in self.widgets:
-            if w.style.row > n: w.style.row -= 1
-        
+            if w.style.row > n:
+                w.style.row -= 1
+
         if self._curRow >= n:
             self._curRow -= 1
-        
-        #self.rect.w, self.rect.h = self.resize()
-        #self.repaint()
-        
+
+        # self.rect.w, self.rect.h = self.resize()
+        # self.repaint()
+
         self.chsize()
-    
+
     def clear(self):
         self._rows = []
         self._curRow = 0
         self._trok = False
 
         self.widgets = []
-        
+
         self.chsize()
-        
-        #print 'clear',self,self._rows
-    
+
+        # print 'clear',self,self._rows
+
     def _addRow(self):
-        self._rows.append([None for x in xrange(self.getColumns())])
-    
+        self._rows.append([None for x in range(self.getColumns())])
+
     def tr(self):
         """Start on the next row."""
         if not self._trok:
             self._trok = True
-            return 
+            return
         self._curRow += 1
         if self.getRows() <= self._curRow:
             self._addRow()
-    
+
     def _addColumn(self):
         if not self._rows:
             self._addRow()
         for row in self._rows:
             row.append(None)
-    
+
     def _setCell(self, w, col, row, colspan=1, rowspan=1):
-        #make room for the widget by adding columns and rows
+        # make room for the widget by adding columns and rows
         while self.getColumns() < col + colspan:
             self._addColumn()
         while self.getRows() < row + rowspan:
             self._addRow()
-            
-        #print w.__class__.__name__,col,row,colspan,rowspan
-        
-        #actual widget setting and modification stuff
+
+        # print w.__class__.__name__,col,row,colspan,rowspan
+
+        # actual widget setting and modification stuff
         w.container = self
-        w.style.row = row #HACK - to work with gal's list
-        w.style.col = col #HACK - to work with gal's list
-        self._rows[row][col] = {"widget":w, "colspan":colspan, "rowspan":rowspan}
+        w.style.row = row  # HACK - to work with gal's list
+        w.style.col = col  # HACK - to work with gal's list
+        self._rows[row][col] = {"widget": w, "colspan": colspan, "rowspan": rowspan}
         self.widgets.append(self._rows[row][col]["widget"])
-        
-        #set the spanned columns
-        #for acell in xrange(col + 1, col + colspan):
+
+        # set the spanned columns
+        # for acell in xrange(col + 1, col + colspan):
         #    self._rows[row][acell] = True
-        
-        #set the spanned rows and the columns on them
-        #for arow in xrange(row + 1, row + rowspan):
+
+        # set the spanned rows and the columns on them
+        # for arow in xrange(row + 1, row + rowspan):
         #    for acell in xrange(col, col + colspan): #incorrect?
         #        self._rows[arow][acell] = True
-        
-        for arow in xrange(row, row + rowspan):
-            for acell in xrange(col, col + colspan): #incorrect?
+
+        for arow in range(row, row + rowspan):
+            for acell in range(col, col + colspan):  # incorrect?
                 if row != arow or col != acell:
                     self._rows[arow][acell] = True
-    
-    
+
     def td(self, w, col=None, row=None, colspan=1, rowspan=1, **params):
         """Add a widget to a table after wrapping it in a TD container.
-        
+
         <pre>Table.td(w,col=None,row=None,colspan=1,rowspan=1,**params)</pre>
-        
+
         <dl>
         <dt>w<dd>widget
         <dt>col<dd>column
         <dt>row<dd>row
         <dt>colspan<dd>colspan
         <dt>rowspan<dd>rowspan
         <dt>align<dd>horizontal alignment (-1,0,1)
         <dt>valign<dd>vertical alignment (-1,0,1)
         <dt>params<dd>other params for the TD container, style information, etc
         </dl>
         """
-        
-        Table.add(self,_Table_td(w, **params), col=col, row=row, colspan=colspan, rowspan=rowspan)
-    
+
+        Table.add(
+            self,
+            _Table_td(w, **params),
+            col=col,
+            row=row,
+            colspan=colspan,
+            rowspan=rowspan,
+        )
+
     def add(self, w, col=None, row=None, colspan=1, rowspan=1):
         """Add a widget directly into the table, without wrapping it in a TD container.
-        
+
         <pre>Table.add(w,col=None,row=None,colspan=1,rowspan=1)</pre>
-        
+
         <p>See Table.td for an explanation of the parameters.</p>
         """
         self._trok = True
-        #if no row was specifically specified, set it to the current row
+        # if no row was specifically specified, set it to the current row
         if row is None:
             row = self._curRow
-            #print row
-        
-        #if its going to be a new row, have it be on the first column
+            # print row
+
+        # if its going to be a new row, have it be on the first column
         if row >= self.getRows():
             col = 0
-        
-        #try to find an open cell for the widget
+
+        # try to find an open cell for the widget
         if col is None:
-            for cell in xrange(self.getColumns()):
+            for cell in range(self.getColumns()):
                 if col is None and not self._rows[row][cell]:
                     col = cell
                     break
-        
-        #otherwise put the widget in a new column
+
+        # otherwise put the widget in a new column
         if col is None:
             col = self.getColumns()
-        
+
         self._setCell(w, col, row, colspan=colspan, rowspan=rowspan)
-        
+
         self.chsize()
         return
-        
-    def remove(self,w):
-        if hasattr(w,'_table_td'): w = w._table_td
-        row,col = w.style.row,w.style.col
+
+    def remove(self, w):
+        if hasattr(w, "_table_td"):
+            w = w._table_td
+        row, col = w.style.row, w.style.col
         cell = self._rows[row][col]
-        colspan,rowspan = cell['colspan'],cell['rowspan']
-        
-        for arow in xrange(row , row + rowspan):
-            for acell in xrange(col, col + colspan): #incorrect?
+        colspan, rowspan = cell["colspan"], cell["rowspan"]
+
+        for arow in range(row, row + rowspan):
+            for acell in range(col, col + colspan):  # incorrect?
                 self._rows[arow][acell] = False
         self.widgets.remove(w)
         self.chsize()
-        
-        
-    
+
     def resize(self, width=None, height=None):
-        #if 1 or self.getRows() == 82:
-            #print ''
-            #print 'resize',self.getRows(),self.getColumns(),width,height
-            #import inspect
-            #for obj,fname,line,fnc,code,n in inspect.stack()[9:20]:
-            #    print fname,line,':',fnc,code[0].strip()
+        # if 1 or self.getRows() == 82:
+        # print ''
+        # print 'resize',self.getRows(),self.getColumns(),width,height
+        # import inspect
+        # for obj,fname,line,fnc,code,n in inspect.stack()[9:20]:
+        #    print fname,line,':',fnc,code[0].strip()
 
-        
-        #resize the widgets to their smallest size
+        # resize the widgets to their smallest size
         for w in self.widgets:
             w.rect.w, w.rect.h = w.resize()
-        
-        #calculate row heights and column widths
-        rowsizes = [0 for y in xrange(self.getRows())]
-        columnsizes = [0 for x in xrange(self.getColumns())]
-        for row in xrange(self.getRows()):
-            for cell in xrange(self.getColumns()):
+
+        # calculate row heights and column widths
+        rowsizes = [0 for y in range(self.getRows())]
+        columnsizes = [0 for x in range(self.getColumns())]
+        for row in range(self.getRows()):
+            for cell in range(self.getColumns()):
                 if self._rows[row][cell] and self._rows[row][cell] is not True:
                     if not self._rows[row][cell]["colspan"] > 1:
-                        columnsizes[cell] = max(columnsizes[cell], self._rows[row][cell]["widget"].rect.w)
+                        columnsizes[cell] = max(
+                            columnsizes[cell], self._rows[row][cell]["widget"].rect.w
+                        )
                     if not self._rows[row][cell]["rowspan"] > 1:
-                        rowsizes[row] = max(rowsizes[row], self._rows[row][cell]["widget"].rect.h)
-        
-        #distribute extra space if necessary for wide colspanning/rowspanning
-        for row in xrange(self.getRows()):
-            for cell in xrange(self.getColumns()):
+                        rowsizes[row] = max(
+                            rowsizes[row], self._rows[row][cell]["widget"].rect.h
+                        )
+
+        # distribute extra space if necessary for wide colspanning/rowspanning
+        for row in range(self.getRows()):
+            for cell in range(self.getColumns()):
                 if self._rows[row][cell] and self._rows[row][cell] is not True:
                     if self._rows[row][cell]["colspan"] > 1:
-                        columns = xrange(cell, cell + self._rows[row][cell]["colspan"])
+                        columns = range(cell, cell + self._rows[row][cell]["colspan"])
                         totalwidth = 0
                         for acol in columns:
                             totalwidth += columnsizes[acol]
                         if totalwidth < self._rows[row][cell]["widget"].rect.w:
                             for acol in columns:
-                                columnsizes[acol] += _table_div(self._rows[row][cell]["widget"].rect.w - totalwidth, self._rows[row][cell]["colspan"],acol)
+                                columnsizes[acol] += _table_div(
+                                    self._rows[row][cell]["widget"].rect.w - totalwidth,
+                                    self._rows[row][cell]["colspan"],
+                                    acol,
+                                )
                     if self._rows[row][cell]["rowspan"] > 1:
-                        rows = xrange(row, row + self._rows[row][cell]["rowspan"])
+                        rows = range(row, row + self._rows[row][cell]["rowspan"])
                         totalheight = 0
                         for arow in rows:
                             totalheight += rowsizes[arow]
                         if totalheight < self._rows[row][cell]["widget"].rect.h:
                             for arow in rows:
-                                rowsizes[arow] += _table_div(self._rows[row][cell]["widget"].rect.h - totalheight, self._rows[row][cell]["rowspan"],arow)
-         
-        #make everything fill out to self.style.width, self.style.heigh, not exact, but pretty close...
+                                rowsizes[arow] += _table_div(
+                                    self._rows[row][cell]["widget"].rect.h
+                                    - totalheight,
+                                    self._rows[row][cell]["rowspan"],
+                                    arow,
+                                )
+
+        # make everything fill out to self.style.width, self.style.heigh, not exact, but pretty close...
         w, h = sum(columnsizes), sum(rowsizes)
         if w > 0 and w < self.style.width and len(columnsizes):
-            d = (self.style.width - w) 
-            for n in xrange(0, len(columnsizes)):
+            d = self.style.width - w
+            for n in range(0, len(columnsizes)):
                 v = columnsizes[n]
                 columnsizes[n] += v * d / w
         if h > 0 and h < self.style.height and len(rowsizes):
             d = (self.style.height - h) / len(rowsizes)
-            for n in xrange(0, len(rowsizes)):
+            for n in range(0, len(rowsizes)):
                 v = rowsizes[n]
                 rowsizes[n] += v * d / h
-        
-        #set the widget's position by calculating their row/column x/y offset
-        cellpositions = [[[sum(columnsizes[0:cell]), sum(rowsizes[0:row])] for cell in xrange(self.getColumns())] for row in xrange(self.getRows())]
-        for row in xrange(self.getRows()):
-            for cell in xrange(self.getColumns()):
+
+        # set the widget's position by calculating their row/column x/y offset
+        cellpositions = [
+            [
+                [sum(columnsizes[0:cell]), sum(rowsizes[0:row])]
+                for cell in range(self.getColumns())
+            ]
+            for row in range(self.getRows())
+        ]
+        for row in range(self.getRows()):
+            for cell in range(self.getColumns()):
                 if self._rows[row][cell] and self._rows[row][cell] is not True:
                     x, y = cellpositions[row][cell]
-                    w = sum(columnsizes[cell:cell+self._rows[row][cell]["colspan"]])
-                    h = sum(rowsizes[row:row+self._rows[row][cell]["rowspan"]])
-                    
+                    w = sum(columnsizes[cell : cell + self._rows[row][cell]["colspan"]])
+                    h = sum(rowsizes[row : row + self._rows[row][cell]["rowspan"]])
+
                     widget = self._rows[row][cell]["widget"]
                     widget.rect.x = x
                     widget.rect.y = y
-                    if 1 and (w,h) != (widget.rect.w,widget.rect.h):
-                        #if h > 50:
+                    if 1 and (w, h) != (widget.rect.w, widget.rect.h):
+                        # if h > 50:
                         #    print widget.widget.__class__.__name__, (widget.rect.w,widget.rect.h),'=>',(w,h)
                         widget.rect.w, widget.rect.h = widget.resize(w, h)
-                    
-                    #print self._rows[row][cell]["widget"].rect
-        
-        #print columnsizes
-        #print sum(columnsizes)
-        #size = sum(columnsizes), sum(rowsizes); print size
-        
-        #return the tables final size
-        return sum(columnsizes),sum(rowsizes)
-
-        
-def _table_div(a,b,c):
-    v,r = a/b, a%b
-    if r != 0 and (c%b)<r: v += 1
+
+                    # print self._rows[row][cell]["widget"].rect
+
+        # print columnsizes
+        # print sum(columnsizes)
+        # size = sum(columnsizes), sum(rowsizes); print size
+
+        # return the tables final size
+        return sum(columnsizes), sum(rowsizes)
+
+
+def _table_div(a, b, c):
+    v, r = a / b, a % b
+    if r != 0 and (c % b) < r:
+        v += 1
     return v
 
+
 class _Table_td(container.Container):
-    def __init__(self,widget,**params):#hexpand=0,vexpand=0,
-        container.Container.__init__(self,**params)
+    def __init__(self, widget, **params):  # hexpand=0,vexpand=0,
+        container.Container.__init__(self, **params)
         self.widget = widget
-        #self.hexpand=hexpand
-        #self.vexpand=vexpand
+        # self.hexpand=hexpand
+        # self.vexpand=vexpand
         widget._table_td = self
-        self.add(widget,0,0)
-    
-    def resize(self,width=None,height=None):
+        self.add(widget, 0, 0)
+
+    def resize(self, width=None, height=None):
         w = self.widget
-        
-        #expansion code, but i didn't like the idea that much..
-        #a bit obscure, fairly useless when a user can just
-        #add a widget to a table instead of td it in.
-        #ww,hh=None,None
-        #if self.hexpand: ww = self.style.width
-        #if self.vexpand: hh = self.style.height
-        #if self.hexpand and width != None: ww = max(ww,width)
-        #if self.vexpand and height != None: hh = max(hh,height)
-        #w.rect.w,w.rect.h = w.resize(ww,hh)
-        
-        #why bother, just do the lower mentioned item...
-        w.rect.w,w.rect.h = w.resize()
-        
-        #this should not be needed, widgets should obey their sizing on their own.
-        
-#         if (self.style.width!=0 and w.rect.w > self.style.width) or (self.style.height!=0 and w.rect.h > self.style.height):
-#             ww,hh = None,None
-#             if self.style.width: ww = self.style.width
-#             if self.style.height: hh = self.style.height
-#             w.rect.w,w.rect.h = w.resize(ww,hh)
-      
-  
-        #in the case that the widget is too big, we try to resize it
-        if (width != None and width < w.rect.w) or (height != None and height < w.rect.h):
-            w.rect.w,w.rect.h = w.resize(width,height)
-        
-        width = max(width,w.rect.w,self.style.width) #,self.style.cell_width)
-        height = max(height,w.rect.h,self.style.height) #,self.style.cell_height)
-        
-        dx = width-w.rect.w
-        dy = height-w.rect.h
-        w.rect.x = (self.style.align+1)*dx/2
-        w.rect.y = (self.style.valign+1)*dy/2
-        
-        return width,height
+
+        # expansion code, but i didn't like the idea that much..
+        # a bit obscure, fairly useless when a user can just
+        # add a widget to a table instead of td it in.
+        # ww,hh=None,None
+        # if self.hexpand: ww = self.style.width
+        # if self.vexpand: hh = self.style.height
+        # if self.hexpand and width != None: ww = max(ww,width)
+        # if self.vexpand and height != None: hh = max(hh,height)
+        # w.rect.w,w.rect.h = w.resize(ww,hh)
+
+        # why bother, just do the lower mentioned item...
+        w.rect.w, w.rect.h = w.resize()
+
+        # this should not be needed, widgets should obey their sizing on their own.
+
+        #         if (self.style.width!=0 and w.rect.w > self.style.width) or (self.style.height!=0 and w.rect.h > self.style.height):
+        #             ww,hh = None,None
+        #             if self.style.width: ww = self.style.width
+        #             if self.style.height: hh = self.style.height
+        #             w.rect.w,w.rect.h = w.resize(ww,hh)
+
+        # in the case that the widget is too big, we try to resize it
+        if (width != None and width < w.rect.w) or (
+            height != None and height < w.rect.h
+        ):
+            w.rect.w, w.rect.h = w.resize(width, height)
+
+        width = max(width, w.rect.w, self.style.width)  # ,self.style.cell_width)
+        height = max(height, w.rect.h, self.style.height)  # ,self.style.cell_height)
+
+        dx = width - w.rect.w
+        dy = height - w.rect.h
+        w.rect.x = (self.style.align + 1) * dx / 2
+        w.rect.y = (self.style.valign + 1) * dy / 2
+
+        return width, height
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/layout.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/layout.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """document layout engine."""
+
+
 class Layout:
     """the document layout engine
-    
-    .widgets -- elements are kept in this list.  read-only, use add to add items to it. 
+
+    .widgets -- elements are kept in this list.  read-only, use add to add items to it.
     """
-    
-    def __init__(self,rect=None):
+
+    def __init__(self, rect=None):
         """initialize the object with the size of the box."""
         self._widgets = []
         self.rect = rect
-        
-    def add(self,e): 
+
+    def add(self, e):
         """add a document element to the layout.
-        
+
         a document element may be
         - a tuple (w,h) if it is a whitespace element
         - a tuple (0,h) if it is a linebreak element
         - an integer -1,0,1 if it is a command to start a new block of elements that are aligned either left,center, or right.
         - an object with a .rect (for size) -- such as a word element
         - an object with a .rect (for size) and .align -- such as an image element
         """
-        
+
         self._widgets.append(e)
-        
-        
+
     def resize(self):
         """resize the layout
         this method recalculates the position of all document elements
         after they have been added to the document.  .rect.x,y will be updated for all
         objects.
         """
         self.init()
@@ -35,138 +36,142 @@
         for e in self._widgets:
             if type(e) is tuple and e[0] != 0:
                 self.do_space(e)
             elif type(e) is tuple and e[0] == 0:
                 self.do_br(e[1])
             elif type(e) is int:
                 self.do_block(align=e)
-            elif hasattr(e,'align'):
+            elif hasattr(e, "align"):
                 self.do_align(e)
             else:
                 self.do_item(e)
         self.line()
-        self.rect.h = max(self.y,self.left_bottom,self.right_bottom)
-            
+        self.rect.h = max(self.y, self.left_bottom, self.right_bottom)
+
     def init(self):
-        self.x,self.y = self.rect.x,self.rect.y
+        self.x, self.y = self.rect.x, self.rect.y
         self.left = self.rect.left
         self.right = self.rect.right
         self.left_bottom = 0
         self.right_bottom = 0
         self.y = self.rect.y
         self.x = self.rect.x
         self.h = 0
-        
+
         self.items = []
         self.align = -1
-        
+
     def getleft(self):
         if self.y > self.left_bottom:
             self.left = self.rect.left
         return self.left
-        
+
     def getright(self):
         if self.y > self.right_bottom:
             self.right = self.rect.right
         return self.right
-        
-    def do_br(self,h): 
+
+    def do_br(self, h):
         self.line()
         self.h = h
-    
-    def do_block(self,align=-1):
+
+    def do_block(self, align=-1):
         self.line()
         self.align = align
 
-    def do_align(self,e):
+    def do_align(self, e):
         align = e.align
-        ox,oy,oh = self.x,self.y,self.h
-        w,h = e.rect.w,e.rect.h
-        
-        if align == 0: 
+        ox, oy, oh = self.x, self.y, self.h
+        w, h = e.rect.w, e.rect.h
+
+        if align == 0:
             self.line()
-            self.x = self.rect.left + (self.rect.width-w)/2
+            self.x = self.rect.left + (self.rect.width - w) / 2
             self.fit = 0
-        elif align == -1: 
+        elif align == -1:
             self.line()
-            self.y = max(self.left_bottom,self.y + self.h)
+            self.y = max(self.left_bottom, self.y + self.h)
             self.h = 0
             self.x = self.rect.left
-        elif align == 1: 
+        elif align == 1:
             self.line()
-            self.y = max(self.right_bottom,self.y + self.h)
+            self.y = max(self.right_bottom, self.y + self.h)
             self.h = 0
-            self.x = self.rect.left + (self.rect.width-w)
+            self.x = self.rect.left + (self.rect.width - w)
+
+        e.rect.x, e.rect.y = self.x, self.y
 
-        e.rect.x,e.rect.y = self.x,self.y        
-            
         self.x = self.x + w
         self.y = self.y
-        
+
         if align == 0:
-            self.h = max(self.h,h)
+            self.h = max(self.h, h)
             self.y = self.y + self.h
             self.x = self.getleft()
             self.h = 0
         elif align == -1:
             self.left = self.x
             self.left_bottom = self.y + h
-            self.x,self.y,self.h = ox + w,oy,oh
-        elif align == 1: 
+            self.x, self.y, self.h = ox + w, oy, oh
+        elif align == 1:
             self.right = self.x - w
             self.right_bottom = self.y + h
-            self.x,self.y,self.h = ox,oy,oh
-        
+            self.x, self.y, self.h = ox, oy, oh
+
         self.widgets.append(e)
 
-    def do_space(self,e):
-        w,h = e
-        if self.x+w >= self.getright(): 
+    def do_space(self, e):
+        w, h = e
+        if self.x + w >= self.getright():
             self.line()
-        else: 
+        else:
             self.items.append(e)
-            self.h = max(self.h,h)
+            self.h = max(self.h, h)
             self.x += w
-    
-    def do_item(self,e):
-        w,h = e.rect.w,e.rect.h
-        if self.x+w >= self.getright(): 
+
+    def do_item(self, e):
+        w, h = e.rect.w, e.rect.h
+        if self.x + w >= self.getright():
             self.line()
         self.items.append(e)
-        self.h = max(self.h,h)
+        self.h = max(self.h, h)
         self.x += w
-    
+
     def line(self):
         x1 = self.getleft()
         x2 = self.getright()
         align = self.align
         y = self.y
-        
+
         if len(self.items) != 0 and type(self.items[-1]) == tuple:
             del self.items[-1]
-        
+
         w = 0
         for e in self.items:
-            if type(e) == tuple: w += e[0]
-            else: w += e.rect.w
-            
-        if align == -1: x = x1
-        elif align == 0: 
-            x = x1 + ((x2-x1)-w)/2
+            if type(e) == tuple:
+                w += e[0]
+            else:
+                w += e.rect.w
+
+        if align == -1:
+            x = x1
+        elif align == 0:
+            x = x1 + ((x2 - x1) - w) / 2
             self.fit = 0
-        elif align == 1: x = x2 - w
-            
+        elif align == 1:
+            x = x2 - w
+
         for e in self.items:
-            if type(e) == tuple: x += e[0]
+            if type(e) == tuple:
+                x += e[0]
             else:
-                e.rect.x,e.rect.y = x,y
+                e.rect.x, e.rect.y = x, y
                 self.widgets.append(e)
                 x += e.rect.w
-        
+
         self.items = []
         self.y = self.y + self.h
         self.x = self.getleft()
         self.h = 0
-        
 
 
 # vim: set filetype=python sts=4 sw=4 noet si :
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/dialog.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,153 +1,161 @@
 """
 """
 import os
 
-from const import *
-import table, area
-import basic, input, button
+from .const import *
+from . import table, area
+from . import basic, input, button
+
 
 class Dialog(table.Table):
     """A dialog window with a title bar and an "close" button on the bar.
-    
+
     <pre>Dialog(title,main)</pre>
-    
+
     <dl>
     <dt>title<dd>title widget, usually a label
     <dt>main<dd>main widget, usually a container
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     title = gui.Label("My Title")
     main = gui.Container()
     #add stuff to the container...
-    
+
     d = gui.Dialog(title,main)
     d.open()
     </code>
     """
-    def __init__(self,title,main,**params):
-        params.setdefault('cls','dialog')
-        table.Table.__init__(self,**params)
-        
-        
+
+    def __init__(self, title, main, **params):
+        params.setdefault("cls", "dialog")
+        table.Table.__init__(self, **params)
+
         self.tr()
-        self.td(title,align=-1,cls=self.cls+'.bar')
-        clos = button.Icon(self.cls+".bar.close")
-        clos.connect(CLICK,self.close,None) 
-        self.td(clos,align=1,cls=self.cls+'.bar')
-        
+        self.td(title, align=-1, cls=self.cls + ".bar")
+        clos = button.Icon(self.cls + ".bar.close")
+        clos.connect(CLICK, self.close, None)
+        self.td(clos, align=1, cls=self.cls + ".bar")
+
         self.tr()
-        self.td(main,colspan=2,cls=self.cls+".main")
-        
-        
+        self.td(main, colspan=2, cls=self.cls + ".main")
+
+
 #         self.tr()
-#         
-#         
+#
+#
 #         t = table.Table(cls=self.cls+".bar")
 #         t.tr()
 #         t.td(title)
 #         clos = button.Icon(self.cls+".bar.close")
 #         t.td(clos,align=1)
-#         clos.connect(CLICK,self.close,None) 
+#         clos.connect(CLICK,self.close,None)
 #         self.add(t,0,0)
-#         
+#
 #         main.rect.w,main.rect.h = main.resize()
 #         clos.rect.w,clos.rect.h = clos.resize()
 #         title.container.style.width = main.rect.w - clos.rect.w
-#         
+#
 #         self.tr()
 #         self.td(main,cls=self.cls+".main")
-# 
-        
+#
 
 
 class FileDialog(Dialog):
     """A file picker dialog window.
-    
+
     <pre>FileDialog()</pre>
     <p>Some optional parameters:</p>
     <dl>
     <dt>title_txt<dd>title text
     <dt>button_txt<dd>button text
     <dt>path<dd>initial path
     </dl>
     """
-    
-    def __init__(self, title_txt="File Browser", button_txt="Okay", cls="filedialog", path=None):
-        if not path: self.curdir = os.getcwd()
-        else: self.curdir = path
-        import app
-        self.dir_img = basic.Image(app.App.app.theme.get(cls+'.folder', '', 'image'))
-        td_style = {'padding_left': 4,
-                    'padding_right': 4,
-                    'padding_top': 2,
-                    'padding_bottom': 2}
-        self.title = basic.Label(title_txt, cls=cls+".title.label")
+
+    def __init__(
+        self, title_txt="File Browser", button_txt="Okay", cls="filedialog", path=None
+    ):
+        if not path:
+            self.curdir = os.getcwd()
+        else:
+            self.curdir = path
+        from . import app
+
+        self.dir_img = basic.Image(app.App.app.theme.get(cls + ".folder", "", "image"))
+        td_style = {
+            "padding_left": 4,
+            "padding_right": 4,
+            "padding_top": 2,
+            "padding_bottom": 2,
+        }
+        self.title = basic.Label(title_txt, cls=cls + ".title.label")
         self.body = table.Table()
         self.list = area.List(width=350, height=150)
-        self.input_dir = input.Input(cls=cls+".input")
-        self.input_file = input.Input(cls=cls+".input")
+        self.input_dir = input.Input(cls=cls + ".input")
+        self.input_file = input.Input(cls=cls + ".input")
         self._list_dir_()
         self.button_ok = button.Button(button_txt)
         self.body.tr()
-        self.body.td(basic.Label("Path", cls=cls+".label"), style=td_style, align=-1)
+        self.body.td(basic.Label("Path", cls=cls + ".label"), style=td_style, align=-1)
         self.body.td(self.input_dir, style=td_style)
         self.body.tr()
-        self.body.td(basic.Label("File", cls=cls+".label"), style=td_style, align=-1)
+        self.body.td(basic.Label("File", cls=cls + ".label"), style=td_style, align=-1)
         self.body.td(self.input_file, style=td_style)
         self.body.td(self.button_ok, style=td_style)
         self.body.tr()
         self.body.td(self.list, colspan=3, style=td_style)
         self.list.connect(CHANGE, self._item_select_changed_, None)
         self.button_ok.connect(CLICK, self._button_okay_clicked_, None)
         self.value = None
         Dialog.__init__(self, self.title, self.body)
-        
+
     def _list_dir_(self):
         self.input_dir.value = self.curdir
         self.input_dir.pos = len(self.curdir)
         self.input_dir.vpos = 0
         dirs = []
         files = []
         try:
             for i in os.listdir(self.curdir):
-                if os.path.isdir(os.path.join(self.curdir, i)): dirs.append(i)
-                else: files.append(i)
+                if os.path.isdir(os.path.join(self.curdir, i)):
+                    dirs.append(i)
+                else:
+                    files.append(i)
         except:
             self.input_file.value = "Opps! no access"
-        if '..' not in dirs: dirs.append('..')
+        if ".." not in dirs:
+            dirs.append("..")
         dirs.sort()
         files.sort()
         for i in dirs:
-            #item = ListItem(image=self.dir_img, text=i, value=i)
-            self.list.add(i,image=self.dir_img,value=i)
+            # item = ListItem(image=self.dir_img, text=i, value=i)
+            self.list.add(i, image=self.dir_img, value=i)
         for i in files:
-            #item = ListItem(image=None, text=i, value=i)
-            self.list.add(i,value=i)
-        #self.list.resize()
+            # item = ListItem(image=None, text=i, value=i)
+            self.list.add(i, value=i)
+        # self.list.resize()
         self.list.set_vertical_scroll(0)
-        #self.list.repaintall()
-        
-        
+        # self.list.repaintall()
+
     def _item_select_changed_(self, arg):
         self.input_file.value = self.list.value
         fname = os.path.abspath(os.path.join(self.curdir, self.input_file.value))
         if os.path.isdir(fname):
             self.input_file.value = ""
             self.curdir = fname
             self.list.clear()
             self._list_dir_()
 
-
     def _button_okay_clicked_(self, arg):
         if self.input_dir.value != self.curdir:
             if os.path.isdir(self.input_dir.value):
                 self.input_file.value = ""
                 self.curdir = os.path.abspath(self.input_dir.value)
                 self.list.clear()
                 self._list_dir_()
         else:
             self.value = os.path.join(self.curdir, self.input_file.value)
-	    self.send(CHANGE)
-            self.close()
+            self.send(CHANGE)
+            self.close()
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/theme.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/theme.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,442 +1,527 @@
 """
 """
 import os, re
 import pygame
 
-from const import *
-import surface
+from .const import *
+from . import surface
+
 
 def _list_themes(dir):
     d = {}
     for entry in os.listdir(dir):
-        if os.path.exists(os.path.join(dir, entry, 'config.txt')):
+        if os.path.exists(os.path.join(dir, entry, "config.txt")):
             d[entry] = os.path.join(dir, entry)
     return d
 
+
 class Theme:
     """Theme interface.
-    
-    <p>If you wish to create your own theme, create a class with this interface, and 
+
+    <p>If you wish to create your own theme, create a class with this interface, and
     pass it to gui.App via <tt>gui.App(theme=MyTheme())</tt>.</p>
-    
+
     <strong>Default Theme</strong>
-    
+
     <pre>Theme(dirs='default')</pre>
     <dl>
     <dt>dirs<dd>Name of the theme dir to load a theme from.  May be an absolute path to a theme, if pgu is not installed, or if you created your own theme.  May include several dirs in a list if data is spread across several themes.
     </dl>
-    
+
     <strong>Example</strong>
-    
-    <code>    
+
+    <code>
     theme = gui.Theme("default")
     theme = gui.Theme(["mytheme","mytheme2"])
     </code>
     """
-    def __init__(self,dirs='default'):
+
+    def __init__(self, dirs="default"):
         self.config = {}
         self.dict = {}
         self._loaded = []
         self.cache = {}
         self._preload(dirs)
         pygame.font.init()
-    
-    def _preload(self,ds):
+
+    def _preload(self, ds):
         if not isinstance(ds, list):
             ds = [ds]
         for d in ds:
             if d not in self._loaded:
                 self._load(d)
             self._loaded.append(d)
-    
+
     def _load(self, name):
-        #theme_dir = themes[name]
-        
-        #try to load the local dir, or absolute path
+        # theme_dir = themes[name]
+
+        # try to load the local dir, or absolute path
         dnames = [name]
-        
-        dnames.append(os.path.join("data","themes",name))
-        #if the package isn't installed and people are just
-        #trying out the scripts or examples
-        dnames.append(os.path.join(os.path.dirname(__file__),"..","..","data","themes",name))
-        
-        #if the package is installed, and the package is installed
-        #in /usr/lib/python2.3/site-packages/pgu/
-        #or c:\python23\lib\site-packages\pgu\
-        #the data is in ... lib/../share/ ...
-        dnames.append(os.path.join(os.path.dirname(__file__),"..","..","..","..","share","pgu","themes",name))
-        dnames.append(os.path.join(os.path.dirname(__file__),"..","..","..","..","..","share","pgu","themes",name))
-        
+
+        dnames.append(os.path.join("data", "themes", name))
+        # if the package isn't installed and people are just
+        # trying out the scripts or examples
+        dnames.append(
+            os.path.join(os.path.dirname(__file__), "..", "..", "data", "themes", name)
+        )
+
+        # if the package is installed, and the package is installed
+        # in /usr/lib/python2.3/site-packages/pgu/
+        # or c:\python23\lib\site-packages\pgu\
+        # the data is in ... lib/../share/ ...
+        dnames.append(
+            os.path.join(
+                os.path.dirname(__file__),
+                "..",
+                "..",
+                "..",
+                "..",
+                "share",
+                "pgu",
+                "themes",
+                name,
+            )
+        )
+        dnames.append(
+            os.path.join(
+                os.path.dirname(__file__),
+                "..",
+                "..",
+                "..",
+                "..",
+                "..",
+                "share",
+                "pgu",
+                "themes",
+                name,
+            )
+        )
+
         for dname in dnames:
-            if os.path.isdir(dname): break
-        if not os.path.isdir(dname): 
-            raise 'could not find theme '+name
-            
+            if os.path.isdir(dname):
+                break
+        if not os.path.isdir(dname):
+            raise "could not find theme " + name
+
         fname = os.path.join(dname, "config.txt")
         try:
             f = open(fname)
             for line in f.readlines():
                 vals = line.strip().split()
-                if len(vals) < 3: continue
+                if len(vals) < 3:
+                    continue
                 cls = vals[0]
                 del vals[0]
                 pcls = ""
-                if cls.find(":")>=0:
-                    cls,pcls = cls.split(":")
+                if cls.find(":") >= 0:
+                    cls, pcls = cls.split(":")
                 attr = vals[0]
                 del vals[0]
-                self.config[cls+":"+pcls+" "+attr] = (dname, vals)
+                self.config[cls + ":" + pcls + " " + attr] = (dname, vals)
         finally:
             f.close()
-    
-    is_image = re.compile('\.(gif|jpg|bmp|png|tga)$', re.I)
-    def _get(self,key):
-        if not key in self.config: return
-        if key in self.dict: return self.dict[key]
+
+    is_image = re.compile("\.(gif|jpg|bmp|png|tga)$", re.I)
+
+    def _get(self, key):
+        if not key in self.config:
+            return
+        if key in self.dict:
+            return self.dict[key]
         dvals = self.config[key]
         dname, vals = dvals
-        #theme_dir = themes[name]
+        # theme_dir = themes[name]
         v0 = vals[0]
-        if v0[0] == '#':
+        if v0[0] == "#":
             v = pygame.color.Color(v0)
         elif v0.endswith(".ttf") or v0.endswith(".TTF"):
-            v = pygame.font.Font(os.path.join(dname, v0),int(vals[1]))
+            v = pygame.font.Font(os.path.join(dname, v0), int(vals[1]))
         elif self.is_image.search(v0) is not None:
             v = pygame.image.load(os.path.join(dname, v0))
         else:
-            try: v = int(v0)
-            except: v = pygame.font.SysFont(v0, int(vals[1]))
+            try:
+                v = int(v0)
+            except:
+                v = pygame.font.SysFont(v0, int(vals[1]))
         self.dict[key] = v
-        return v    
-    
-    def get(self,cls,pcls,attr):
+        return v
+
+    def get(self, cls, pcls, attr):
         """Interface method -- get the value of a style attribute.
-        
+
         <pre>Theme.get(cls,pcls,attr): return value</pre>
-        
+
         <dl>
         <dt>cls<dd>class, for example "checkbox", "button", etc.
         <dt>pcls<dd>pseudo class, for example "hover", "down", etc.
         <dt>attr<dd>attribute, for example "image", "background", "font", "color", etc.
         </dl>
-        
+
         <p>returns the value of the attribute.</p>
-        
+
         <p>This method is called from [[gui-style]].</p>
         """
-        
-        if not self._loaded: self._preload("default")
-        
-        o = cls+":"+pcls+" "+attr
-        
-        #if not hasattr(self,'_count'):
+
+        if not self._loaded:
+            self._preload("default")
+
+        o = cls + ":" + pcls + " " + attr
+
+        # if not hasattr(self,'_count'):
         #    self._count = {}
-        #if o not in self._count: self._count[o] = 0
-        #self._count[o] += 1
-        
-        if o in self.cache: 
+        # if o not in self._count: self._count[o] = 0
+        # self._count[o] += 1
+
+        if o in self.cache:
             return self.cache[o]
-        
-        v = self._get(cls+":"+pcls+" "+attr)
-        if v: 
+
+        v = self._get(cls + ":" + pcls + " " + attr)
+        if v:
             self.cache[o] = v
             return v
-        
+
         pcls = ""
-        v = self._get(cls+":"+pcls+" "+attr)
-        if v: 
+        v = self._get(cls + ":" + pcls + " " + attr)
+        if v:
             self.cache[o] = v
             return v
-        
+
         cls = "default"
-        v = self._get(cls+":"+pcls+" "+attr)
-        if v: 
+        v = self._get(cls + ":" + pcls + " " + attr)
+        if v:
             self.cache[o] = v
             return v
-        
+
         v = 0
         self.cache[o] = v
         return v
-        
-    def box(self,w,s):
+
+    def box(self, w, s):
         style = w.style
         style.cache(1)
-        
-        c = (0,0,0)
-        if style.border_color != 0: c = style.border_color
-        w,h = s.get_width(),s.get_height()
-        
-        s.fill(c,(0,0,w,style.border_top))
-        s.fill(c,(0,h-style.border_bottom,w,style.border_bottom))
-        s.fill(c,(0,0,style.border_left,h))
-        s.fill(c,(w-style.border_right,0,style.border_right,h))
-        
+
+        c = (0, 0, 0)
+        if style.border_color != 0:
+            c = style.border_color
+        w, h = s.get_width(), s.get_height()
+
+        s.fill(c, (0, 0, w, style.border_top))
+        s.fill(c, (0, h - style.border_bottom, w, style.border_bottom))
+        s.fill(c, (0, 0, style.border_left, h))
+        s.fill(c, (w - style.border_right, 0, style.border_right, h))
+
         style.cache(0)
-        
-    def getspacing(self,w):
+
+    def getspacing(self, w):
         # return the top, right, bottom, left spacing around the widget
-        if not hasattr(w,'_spacing'): #HACK: assume spacing doesn't change re pcls
+        if not hasattr(w, "_spacing"):  # HACK: assume spacing doesn't change re pcls
             s = w.style
             s.cache(1)
-            xt = s.margin_top+s.border_top+s.padding_top
-            xr = s.padding_right+s.border_right+s.margin_right
-            xb = s.padding_bottom+s.border_bottom+s.margin_bottom
-            xl = s.margin_left+s.border_left+s.padding_left
+            xt = s.margin_top + s.border_top + s.padding_top
+            xr = s.padding_right + s.border_right + s.margin_right
+            xb = s.padding_bottom + s.border_bottom + s.margin_bottom
+            xl = s.margin_left + s.border_left + s.padding_left
             s.cache(0)
-            w._spacing = xt,xr,xb,xl
+            w._spacing = xt, xr, xb, xl
         return w._spacing
 
-        
-    def resize(self,w,m):
-        def func(width=None,height=None):
-            #ww,hh = m(width,height)
-            ow,oh = width,height
-            
-            
+    def resize(self, w, m):
+        def func(width=None, height=None):
+            # ww,hh = m(width,height)
+            ow, oh = width, height
+
             s = w.style
-            
+
             s.cache(1)
-            pt,pr,pb,pl = s.padding_top,s.padding_right,s.padding_bottom,s.padding_left
-            bt,br,bb,bl = s.border_top,s.border_right,s.border_bottom,s.border_left
-            mt,mr,mb,ml = s.margin_top,s.margin_right,s.margin_bottom,s.margin_left
+            pt, pr, pb, pl = (
+                s.padding_top,
+                s.padding_right,
+                s.padding_bottom,
+                s.padding_left,
+            )
+            bt, br, bb, bl = (
+                s.border_top,
+                s.border_right,
+                s.border_bottom,
+                s.border_left,
+            )
+            mt, mr, mb, ml = (
+                s.margin_top,
+                s.margin_right,
+                s.margin_bottom,
+                s.margin_left,
+            )
             s.cache(0)
-            
-            xt = pt+bt+mt
-            xr = pr+br+mr
-            xb = pb+bb+mb
-            xl = pl+bl+ml
-            ttw = xl+xr
-            tth = xt+xb
-            
-            ww,hh = None,None
-            if width != None: ww = width-ttw
-            if height != None: hh = height-tth
-            ww,hh = m(ww,hh)
-            
+
+            xt = pt + bt + mt
+            xr = pr + br + mr
+            xb = pb + bb + mb
+            xl = pl + bl + ml
+            ttw = xl + xr
+            tth = xt + xb
+
+            ww, hh = None, None
+            if width != None:
+                ww = width - ttw
+            if height != None:
+                hh = height - tth
+            ww, hh = m(ww, hh)
+
             rect = pygame.Rect(0 + xl, 0 + xt, ww, hh)
-            w._rect_content = rect #pygame.Rect(0 + xl, 0 + xt, width, height)
-            #r = rect
-        
-            if width == None: width = ww
-            if height == None: height = hh
-            #if the widget hasn't respected the style.width,
-            #style height, we'll add in the space for it...
-            width = max(width-ttw,ww,w.style.width)
-            height = max(height-tth,hh,w.style.height)
-            
-            #width = max(ww,w.style.width-tw)
-            #height = max(hh,w.style.height-th)
-
-            r = pygame.Rect(rect.x,rect.y,width,height)
-            
-            w._rect_padding = pygame.Rect(r.x-pl,r.y-pt,r.w+pl+pr,r.h+pt+pb)
+            w._rect_content = rect  # pygame.Rect(0 + xl, 0 + xt, width, height)
+            # r = rect
+
+            if width == None:
+                width = ww
+            if height == None:
+                height = hh
+            # if the widget hasn't respected the style.width,
+            # style height, we'll add in the space for it...
+            width = max(width - ttw, ww, w.style.width)
+            height = max(height - tth, hh, w.style.height)
+
+            # width = max(ww,w.style.width-tw)
+            # height = max(hh,w.style.height-th)
+
+            r = pygame.Rect(rect.x, rect.y, width, height)
+
+            w._rect_padding = pygame.Rect(
+                r.x - pl, r.y - pt, r.w + pl + pr, r.h + pt + pb
+            )
             r = w._rect_padding
-            w._rect_border = pygame.Rect(r.x-bl,r.y-bt,r.w+bl+br,r.h+bt+bb)
+            w._rect_border = pygame.Rect(
+                r.x - bl, r.y - bt, r.w + bl + br, r.h + bt + bb
+            )
             r = w._rect_border
-            w._rect_margin = pygame.Rect(r.x-ml,r.y-mt,r.w+ml+mr,r.h+mt+mb)
-            
-            #align it within it's zone of power.    
-            dx = width-rect.w
-            dy = height-rect.h
-            #rect.x += (1)*dx/2
-            #rect.y += (1)*dy/2
-            rect.x += (w.style.align+1)*dx/2
-            rect.y += (w.style.valign+1)*dy/2
-            
-            
-            #print w,ow, w._rect_margin.w,  ttw
-            return w._rect_margin.w,w._rect_margin.h
+            w._rect_margin = pygame.Rect(
+                r.x - ml, r.y - mt, r.w + ml + mr, r.h + mt + mb
+            )
+
+            # align it within it's zone of power.
+            dx = width - rect.w
+            dy = height - rect.h
+            # rect.x += (1)*dx/2
+            # rect.y += (1)*dy/2
+            rect.x += (w.style.align + 1) * dx / 2
+            rect.y += (w.style.valign + 1) * dy / 2
+
+            # print w,ow, w._rect_margin.w,  ttw
+            return w._rect_margin.w, w._rect_margin.h
+
         return func
-            
-        
-    def paint(self,w,m):
+
+    def paint(self, w, m):
         def func(s):
             if w.disabled:
                 orig = s
-                s = pygame.Surface((s.get_width(),s.get_height()),0,s)
-                s.blit(orig,(0,0))
-            
-            if hasattr(w,'background'):
-                w.background.paint(surface.subsurface(s,w._rect_border))
-            self.box(w,surface.subsurface(s,w._rect_border))
-            r = m(surface.subsurface(s,w._rect_content))
-            
+                s = pygame.Surface((s.get_width(), s.get_height()), 0, s)
+                s.blit(orig, (0, 0))
+
+            if hasattr(w, "background"):
+                w.background.paint(surface.subsurface(s, w._rect_border))
+            self.box(w, surface.subsurface(s, w._rect_border))
+            r = m(surface.subsurface(s, w._rect_content))
+
             if w.disabled:
                 s.set_alpha(128)
-                orig.blit(s,(0,0))
-                
-            
+                orig.blit(s, (0, 0))
+
             return r
+
         return func
-    
-    def event(self,w,m):
+
+    def event(self, w, m):
         def func(e):
             rect = w._rect_content
             if e.type == MOUSEBUTTONUP or e.type == MOUSEBUTTONDOWN:
-                sub = pygame.event.Event(e.type,{
-                    'button':e.button,
-                    'pos':(e.pos[0]-rect.x,e.pos[1]-rect.y)})
+                sub = pygame.event.Event(
+                    e.type,
+                    {"button": e.button, "pos": (e.pos[0] - rect.x, e.pos[1] - rect.y)},
+                )
             elif e.type == CLICK:
-                sub = pygame.event.Event(e.type,{
-                    'button':e.button,
-                    'pos':(e.pos[0]-rect.x,e.pos[1]-rect.y)})
+                sub = pygame.event.Event(
+                    e.type,
+                    {"button": e.button, "pos": (e.pos[0] - rect.x, e.pos[1] - rect.y)},
+                )
             elif e.type == MOUSEMOTION:
-                sub = pygame.event.Event(e.type,{
-                    'buttons':e.buttons,
-                    'pos':(e.pos[0]-rect.x,e.pos[1]-rect.y),
-                    'rel':e.rel})
+                sub = pygame.event.Event(
+                    e.type,
+                    {
+                        "buttons": e.buttons,
+                        "pos": (e.pos[0] - rect.x, e.pos[1] - rect.y),
+                        "rel": e.rel,
+                    },
+                )
             else:
                 sub = e
             r = m(sub)
             return r
+
         return func
-    
-    def update(self,w,m):
+
+    def update(self, w, m):
         def func(s):
-            if w.disabled: return []
-            r = m(surface.subsurface(s,w._rect_content))
+            if w.disabled:
+                return []
+            r = m(surface.subsurface(s, w._rect_content))
             if type(r) == list:
-                dx,dy = w._rect_content.topleft
+                dx, dy = w._rect_content.topleft
                 for rr in r:
-                    rr.x,rr.y = rr.x+dx,rr.y+dy
+                    rr.x, rr.y = rr.x + dx, rr.y + dy
             return r
+
         return func
-        
-    def open(self,w,m):
-        def func(widget=None,x=None,y=None):
-            if not hasattr(w,'_rect_content'): w.rect.w,w.rect.h = w.resize() #HACK: so that container.open won't resize again!
+
+    def open(self, w, m):
+        def func(widget=None, x=None, y=None):
+            if not hasattr(w, "_rect_content"):
+                (
+                    w.rect.w,
+                    w.rect.h,
+                ) = w.resize()  # HACK: so that container.open won't resize again!
             rect = w._rect_content
             ##print w.__class__.__name__, rect
-            if x != None: x += rect.x
-            if y != None: y += rect.y
-            return m(widget,x,y)
+            if x != None:
+                x += rect.x
+            if y != None:
+                y += rect.y
+            return m(widget, x, y)
+
         return func
-            
-    #def open(self,w,m):
+
+    # def open(self,w,m):
     #    def func(widget=None):
     #        return m(widget)
     #    return func
-        
-    def decorate(self,widget,level):
+
+    def decorate(self, widget, level):
         """Interface method -- decorate a widget.
-        
+
         <p>The theme system is given the opportunity to decorate a widget methods at the
         end of the Widget initializer.</p>
 
         <pre>Theme.decorate(widget,level)</pre>
-                
+
         <dl>
         <dt>widget<dd>the widget to be decorated
         <dt>level<dd>the amount of decoration to do, False for none, True for normal amount, 'app' for special treatment of App objects.
         </dl>
-        """        
-        
+        """
+
         w = widget
-        if level == False: return
-        
+        if level == False:
+            return
+
         if type(w.style.background) != int:
-            w.background = Background(w,self)    
-        
-        if level == 'app': return
-        
-        for k,v in w.style.__dict__.items():
-            if k in ('border','margin','padding'):
-                for kk in ('top','bottom','left','right'):
-                    setattr(w.style,'%s_%s'%(k,kk),v)
-
-        w.paint = self.paint(w,w.paint)
-        w.event = self.event(w,w.event)
-        w.update = self.update(w,w.update)
-        w.resize = self.resize(w,w.resize)
-        w.open = self.open(w,w.open)
+            w.background = Background(w, self)
+
+        if level == "app":
+            return
+
+        for k, v in list(w.style.__dict__.items()):
+            if k in ("border", "margin", "padding"):
+                for kk in ("top", "bottom", "left", "right"):
+                    setattr(w.style, "%s_%s" % (k, kk), v)
+
+        w.paint = self.paint(w, w.paint)
+        w.event = self.event(w, w.event)
+        w.update = self.update(w, w.update)
+        w.resize = self.resize(w, w.resize)
+        w.open = self.open(w, w.open)
 
-    def render(self,s,box,r):
+    def render(self, s, box, r):
         """Interface method - render a special widget feature.
-        
+
         <pre>Theme.render(s,box,r)</pre>
-        
+
         <dl>
         <dt>s<dt>pygame.Surface
         <dt>box<dt>box data, a value returned from Theme.get, typically a pygame.Surface
         <dt>r<dt>pygame.Rect with the size that the box data should be rendered
         </dl>
-        
+
         """
-        
-        if box == 0: return
-        
+
+        if box == 0:
+            return
+
         if type(box) == tuple:
-            s.fill(box,r)
+            s.fill(box, r)
             return
-        
-        x,y,w,h=r.x,r.y,r.w,r.h
-        ww,hh=box.get_width()/3,box.get_height()/3
-        xx,yy=x+w,y+h
-        src = pygame.rect.Rect(0,0,ww,hh)
-        dest = pygame.rect.Rect(0,0,ww,hh)
-        
-        s.set_clip(pygame.Rect(x+ww,y+hh,w-ww*2,h-hh*2))
-        src.x,src.y = ww,hh
-        for dest.y in xrange(y+hh,yy-hh,hh): 
-            for dest.x in xrange(x+ww,xx-ww,ww): s.blit(box,dest,src)
-        
-        s.set_clip(pygame.Rect(x+ww,y,w-ww*3,hh))
-        src.x,src.y,dest.y = ww,0,y
-        for dest.x in xrange(x+ww,xx-ww*2,ww): s.blit(box,dest,src)
-        dest.x = xx-ww*2
-        s.set_clip(pygame.Rect(x+ww,y,w-ww*2,hh))
-        s.blit(box,dest,src)
-        
-        s.set_clip(pygame.Rect(x+ww,yy-hh,w-ww*3,hh))
-        src.x,src.y,dest.y = ww,hh*2,y+h-hh
-        for dest.x in xrange(x+ww,xx-ww*2,ww): s.blit(box,dest,src)
-        dest.x = xx-ww*2
-        s.set_clip(pygame.Rect(x+ww,yy-hh,w-ww*2,hh))
-        s.blit(box,dest,src)
-    
-        s.set_clip(pygame.Rect(x,y+hh,xx,h-hh*3))
-        src.y,src.x,dest.x = hh,0,x
-        for dest.y in xrange(y+hh,yy-hh*2,hh): s.blit(box,dest,src)
-        dest.y = yy-hh*2
-        s.set_clip(pygame.Rect(x,y+hh,xx,h-hh*2))
-        s.blit(box,dest,src)
-    
-        s.set_clip(pygame.Rect(xx-ww,y+hh,xx,h-hh*3))
-        src.y,src.x,dest.x=hh,ww*2,x+w-ww
-        for dest.y in xrange(y+hh,yy-hh*2,hh): s.blit(box,dest,src)
-        dest.y = yy-hh*2
-        s.set_clip(pygame.Rect(xx-ww,y+hh,xx,h-hh*2))
-        s.blit(box,dest,src)
-        
+
+        x, y, w, h = r.x, r.y, r.w, r.h
+        ww, hh = box.get_width() / 3, box.get_height() / 3
+        xx, yy = x + w, y + h
+        src = pygame.rect.Rect(0, 0, ww, hh)
+        dest = pygame.rect.Rect(0, 0, ww, hh)
+
+        s.set_clip(pygame.Rect(x + ww, y + hh, w - ww * 2, h - hh * 2))
+        src.x, src.y = ww, hh
+        for dest.y in range(y + hh, yy - hh, hh):
+            for dest.x in range(x + ww, xx - ww, ww):
+                s.blit(box, dest, src)
+
+        s.set_clip(pygame.Rect(x + ww, y, w - ww * 3, hh))
+        src.x, src.y, dest.y = ww, 0, y
+        for dest.x in range(x + ww, xx - ww * 2, ww):
+            s.blit(box, dest, src)
+        dest.x = xx - ww * 2
+        s.set_clip(pygame.Rect(x + ww, y, w - ww * 2, hh))
+        s.blit(box, dest, src)
+
+        s.set_clip(pygame.Rect(x + ww, yy - hh, w - ww * 3, hh))
+        src.x, src.y, dest.y = ww, hh * 2, y + h - hh
+        for dest.x in range(x + ww, xx - ww * 2, ww):
+            s.blit(box, dest, src)
+        dest.x = xx - ww * 2
+        s.set_clip(pygame.Rect(x + ww, yy - hh, w - ww * 2, hh))
+        s.blit(box, dest, src)
+
+        s.set_clip(pygame.Rect(x, y + hh, xx, h - hh * 3))
+        src.y, src.x, dest.x = hh, 0, x
+        for dest.y in range(y + hh, yy - hh * 2, hh):
+            s.blit(box, dest, src)
+        dest.y = yy - hh * 2
+        s.set_clip(pygame.Rect(x, y + hh, xx, h - hh * 2))
+        s.blit(box, dest, src)
+
+        s.set_clip(pygame.Rect(xx - ww, y + hh, xx, h - hh * 3))
+        src.y, src.x, dest.x = hh, ww * 2, x + w - ww
+        for dest.y in range(y + hh, yy - hh * 2, hh):
+            s.blit(box, dest, src)
+        dest.y = yy - hh * 2
+        s.set_clip(pygame.Rect(xx - ww, y + hh, xx, h - hh * 2))
+        s.blit(box, dest, src)
+
         s.set_clip()
-        src.x,src.y,dest.x,dest.y = 0,0,x,y
-        s.blit(box,dest,src)
-        
-        src.x,src.y,dest.x,dest.y = ww*2,0,x+w-ww,y
-        s.blit(box,dest,src)
-        
-        src.x,src.y,dest.x,dest.y = 0,hh*2,x,y+h-hh
-        s.blit(box,dest,src)
-        
-        src.x,src.y,dest.x,dest.y = ww*2,hh*2,x+w-ww,y+h-hh
-        s.blit(box,dest,src)
+        src.x, src.y, dest.x, dest.y = 0, 0, x, y
+        s.blit(box, dest, src)
+
+        src.x, src.y, dest.x, dest.y = ww * 2, 0, x + w - ww, y
+        s.blit(box, dest, src)
+
+        src.x, src.y, dest.x, dest.y = 0, hh * 2, x, y + h - hh
+        s.blit(box, dest, src)
+
+        src.x, src.y, dest.x, dest.y = ww * 2, hh * 2, x + w - ww, y + h - hh
+        s.blit(box, dest, src)
+
 
-        
-        
 import pygame
-import widget
+from . import widget
+
 
 class Background(widget.Widget):
-    def __init__(self,value,theme,**params):
-        params['decorate'] = False
-        widget.Widget.__init__(self,**params)
+    def __init__(self, value, theme, **params):
+        params["decorate"] = False
+        widget.Widget.__init__(self, **params)
         self.value = value
         self.theme = theme
-    
-    def paint(self,s):
-        r = pygame.Rect(0,0,s.get_width(),s.get_height())
+
+    def paint(self, s):
+        r = pygame.Rect(0, 0, s.get_width(), s.get_height())
         v = self.value.style.background
         if type(v) == tuple:
             s.fill(v)
-        else: 
-            self.theme.render(s,v,r)
+        else:
+            self.theme.render(s, v, r)
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/style.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/style.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 """
 """
+
+
 class Style:
     """The class used by widget for the widget.style
-    
+
     <p>This object is used mainly as a dictionary, accessed via <tt>widget.style.attr</tt>, as opposed to
     <tt>widget.style['attr']</tt>.  It automatically grabs information from the theme via <tt>value = theme.get(widget.cls,widget.pcls,attr)</tt>.</p>
-    
+
     """
-    def __init__(self,o,dict):
+
+    def __init__(self, o, dict):
         self.obj = o
         self._cache = 0
-        for k,v in dict.items(): self.__dict__[k]=v
-    
-    def __getattr__(self,k):
-        import app
+        for k, v in list(dict.items()):
+            self.__dict__[k] = v
+
+    def __getattr__(self, k):
+        from . import app
+
         v = app.App.app.theme.get(self.obj.cls, self.obj.pcls, k)
-        if self._cache: self.__dict__[k] = v
+        if self._cache:
+            self.__dict__[k] = v
         return v
-    
-    def cache(self,v):
+
+    def cache(self, v):
         """Enable the cache.
-        
+
         <p>This should be used when changes of the pcls are unlikely to impact the data, or when there is a lot of repetitive access to the same attributes expected.</p>
-        
+
         <pre>Style.cache(v)</pre>
-        
+
         <dl>
         <dt>v<dd>True if the cache should be enabled.
         </dl>
         """
-        if v: self._cache += 1
-        else: self._cache -= 1
-    
-    def __setattr__(self,k,v):
+        if v:
+            self._cache += 1
+        else:
+            self._cache -= 1
+
+    def __setattr__(self, k, v):
         self.__dict__[k] = v
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/group.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/group.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """
 """
-from const import *
-import widget
+from .const import *
+from . import widget
+
 
 class Group(widget.Widget):
     """An object for grouping together Form elements.
-    
+
     <pre>Group(name=None,value=None)</pre>
-    
+
     <dl>
     <dt>name<dd>name as used in the Form
     <dt>value<dd>values that are currently selected in the group
     </dl>
-    
+
     <p>See [[gui-button]] for several examples.</p>
-    
+
     <p>When the value changes, an <tt>gui.CHANGE</tt> event is sent.
     Although note, that when the value is a list, it may have to be sent by hand via
     <tt>g.send(gui.CHANGE)</tt></p>
     """
-    
-    def __init__(self,name=None,value=None):
-        widget.Widget.__init__(self,name=name,value=value)
+
+    def __init__(self, name=None, value=None):
+        widget.Widget.__init__(self, name=name, value=value)
         self.widgets = []
-    
-    def add(self,w):
+
+    def add(self, w):
         """Add a widget to this group.
-        
+
         <pre>Group.add(w)</pre>
         """
         self.widgets.append(w)
-    
-    def __setattr__(self,k,v):
-        _v = self.__dict__.get(k,NOATTR)
+
+    def __setattr__(self, k, v):
+        _v = self.__dict__.get(k, NOATTR)
         self.__dict__[k] = v
-        if k == 'value' and _v != NOATTR and _v != v:
+        if k == "value" and _v != NOATTR and _v != v:
             self._change()
-    
+
     def _change(self):
         self.send(CHANGE)
         for w in self.widgets:
             w.repaint()
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/area.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/area.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,379 +1,416 @@
 """
 """
 import os
 
-from const import *
-import surface
-import container, table
-import group
-import basic, button, slider
+from .const import *
+from . import surface
+from . import container, table
+from . import group
+from . import basic, button, slider
+
 
 class SlideBox(container.Container):
     """A scrollable area with no scrollbars.
-    
+
     <pre>SlideBox(widget,width,height)</pre>
-    
+
     <dl>
     <dt>widget<dd>widget to be able to scroll around
     <dt>width, height<dd>size of scrollable area
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     c = SlideBox(w,100,100)
     c.offset = (10,10)
     c.repaint()
     </code>
-    
+
     """
-    
+
     def __init__(self, widget, width, height, **params):
-        params.setdefault('width', width)
-        params.setdefault('height', height)
+        params.setdefault("width", width)
+        params.setdefault("height", height)
         container.Container.__init__(self, **params)
         self.offset = [0, 0]
         self.widget = widget
         self.add(widget, 0, 0)
-    
+
     def paint(self, s):
-        #if not hasattr(self,'surface'):
-        self.surface = pygame.Surface((self.max_rect.w,self.max_rect.h),0,s)
-        #self.surface.fill((0,0,0,0))
-        import app
-        app.App.app.theme.render(self.surface,self.style.background,pygame.Rect(0,0,self.max_rect.w,self.max_rect.h))
-        self.bkgr = pygame.Surface((s.get_width(),s.get_height()),0,s)
-        self.bkgr.blit(s,(0,0))
-        container.Container.paint(self,self.surface)
-        s.blit(self.surface,(-self.offset[0],-self.offset[1]))
+        # if not hasattr(self,'surface'):
+        self.surface = pygame.Surface((self.max_rect.w, self.max_rect.h), 0, s)
+        # self.surface.fill((0,0,0,0))
+        from . import app
+
+        app.App.app.theme.render(
+            self.surface,
+            self.style.background,
+            pygame.Rect(0, 0, self.max_rect.w, self.max_rect.h),
+        )
+        self.bkgr = pygame.Surface((s.get_width(), s.get_height()), 0, s)
+        self.bkgr.blit(s, (0, 0))
+        container.Container.paint(self, self.surface)
+        s.blit(self.surface, (-self.offset[0], -self.offset[1]))
         self._offset = self.offset[:]
         return
-        
-    def paint_for_when_pygame_supports_other_tricks(self,s): 
-        #this would be ideal if pygame had support for it!
-        #and if pgu also had a paint(self,s,rect) method to paint small parts
-        sr = (self.offset[0],self.offset[1],self.max_rect.w,self.max_rect.h)
-        cr = (-self.offset[0],-self.offset[1],s.get_width(),s.get_height())
+
+    def paint_for_when_pygame_supports_other_tricks(self, s):
+        # this would be ideal if pygame had support for it!
+        # and if pgu also had a paint(self,s,rect) method to paint small parts
+        sr = (self.offset[0], self.offset[1], self.max_rect.w, self.max_rect.h)
+        cr = (-self.offset[0], -self.offset[1], s.get_width(), s.get_height())
         s2 = s.subsurface(sr)
         s2.set_clip(cr)
-        container.Container.paint(self,s2)
-        
+        container.Container.paint(self, s2)
+
     def proxy_paint(self, s):
-        container.Container.paint(self, surface.ProxySurface(parent=None, 
-                                           rect=self.max_rect,
-                                           real_surface=s,
-                                           offset=self.offset))
+        container.Container.paint(
+            self,
+            surface.ProxySurface(
+                parent=None, rect=self.max_rect, real_surface=s, offset=self.offset
+            ),
+        )
+
     def update(self, s):
-        rects = container.Container.update(self,self.surface)
-        
+        rects = container.Container.update(self, self.surface)
+
         rets = []
-        s_rect = pygame.Rect(0,0,s.get_width(),s.get_height())
-        
+        s_rect = pygame.Rect(0, 0, s.get_width(), s.get_height())
+
         if self.offset == self._offset:
             for r in rects:
-                r2 = r.move((-self.offset[0],-self.offset[1]))
+                r2 = r.move((-self.offset[0], -self.offset[1]))
                 if r2.colliderect(s_rect):
-                    s.blit(self.surface.subsurface(r),r2)
+                    s.blit(self.surface.subsurface(r), r2)
                     rets.append(r2)
         else:
-            s.blit(self.bkgr,(0,0))
-            sub = pygame.Rect(self.offset[0],self.offset[1],min(s.get_width(),self.max_rect.w-self.offset[0]),min(s.get_height(),self.max_rect.h-self.offset[1]))
-            s.blit(self.surface.subsurface(sub),(0,0))
+            s.blit(self.bkgr, (0, 0))
+            sub = pygame.Rect(
+                self.offset[0],
+                self.offset[1],
+                min(s.get_width(), self.max_rect.w - self.offset[0]),
+                min(s.get_height(), self.max_rect.h - self.offset[1]),
+            )
+            s.blit(self.surface.subsurface(sub), (0, 0))
             rets.append(s_rect)
         self._offset = self.offset[:]
         return rets
-        
+
     def proxy_update(self, s):
-        rects = container.Container.update(self, surface.ProxySurface(parent=None, 
-                                                    rect=self.max_rect,
-                                                    real_surface=s,
-                                                    offset=self.offset))
+        rects = container.Container.update(
+            self,
+            surface.ProxySurface(
+                parent=None, rect=self.max_rect, real_surface=s, offset=self.offset
+            ),
+        )
         result = []
-        for r in rects: result.append(pygame.Rect(r).move(self.offset))
+        for r in rects:
+            result.append(pygame.Rect(r).move(self.offset))
         return result
-        
+
     def resize(self, width=None, height=None):
         container.Container.resize(self)
         self.max_rect = self.widget.rect
-        return self.style.width,self.style.height
-        #self.rect = pygame.Rect(self.rect[0], self.rect[1], self.style.width, self.style.height)
-    
+        return self.style.width, self.style.height
+        # self.rect = pygame.Rect(self.rect[0], self.rect[1], self.style.width, self.style.height)
+
     def event(self, e):
         if e.type in [MOUSEBUTTONDOWN, MOUSEBUTTONUP, MOUSEMOTION]:
             pos = (e.pos[0] + self.offset[0], e.pos[1] + self.offset[1])
             if self.max_rect.collidepoint(pos):
-                e_params = {'pos': pos }
-                if e.type == MOUSEMOTION: 
-                    e_params['buttons'] = e.buttons
-                    e_params['rel'] = e.rel
+                e_params = {"pos": pos}
+                if e.type == MOUSEMOTION:
+                    e_params["buttons"] = e.buttons
+                    e_params["rel"] = e.rel
                 else:
-                    e_params['button'] = e.button
+                    e_params["button"] = e.button
                 e = pygame.event.Event(e.type, e_params)
         container.Container.event(self, e)
 
-#class SlideBox(Area):
+
+# class SlideBox(Area):
 #    def __init__(self,*args,**params):
 #        print 'gui.SlideBox','Scheduled to be renamed to Area.'
 #        Area.__init__(self,*args,**params)
-    
+
+
 class ScrollArea(table.Table):
     """A scrollable area with scrollbars.
-    
+
     <pre>ScrollArea(widget,width,height,hscrollbar=True)</pre>
-    
+
     <dl>
     <dt>widget<dd>widget to be able to scroll around
     <dt>width, height<dd>size of scrollable area
     <dt>hscrollbar<dd>set to False if you do not wish to have a horizontal scrollbar
-    <dt>step<dd>set to how far clicks on the icons will step 
+    <dt>step<dd>set to how far clicks on the icons will step
     </dl>
     """
-    def __init__(self, widget, width, height, hscrollbar=True,step=24, **params):
-        w= widget
-        params.setdefault('cls', 'scrollarea')
-        table.Table.__init__(self, width=width,height=height,**params)
-        
+
+    def __init__(self, widget, width, height, hscrollbar=True, step=24, **params):
+        w = widget
+        params.setdefault("cls", "scrollarea")
+        table.Table.__init__(self, width=width, height=height, **params)
+
         self.widget = w
-        self.sbox = SlideBox(w, width=width, height=height, cls=self.cls+".content")
+        self.sbox = SlideBox(w, width=width, height=height, cls=self.cls + ".content")
         self.vscrollbar = None
         self.hscrollbar = None
-        
+
         self.step = step
 
-    def resize(self,width=None,height=None):
+    def resize(self, width=None, height=None):
         widget = self.widget
         box = self.sbox
-        
-        #self.clear()
+
+        # self.clear()
         table.Table.clear(self)
-        #print 'resize',self,self._rows
-        
+        # print 'resize',self,self._rows
+
         self.tr()
         self.td(box)
-        
-        box.style.width,box.style.height = self.style.width,self.style.height
-        
+
+        box.style.width, box.style.height = self.style.width, self.style.height
+
         widget.rect.w, widget.rect.h = widget.resize()
-        box.rect.w,box.rect.h = box.resize()
-        
-        #print widget.rect
-        #print box.rect
-        #r = table.Table.resize(self,width,height)
-        #print r
-        #return r
-        
-        #print box.offset
+        box.rect.w, box.rect.h = box.resize()
+
+        # print widget.rect
+        # print box.rect
+        # r = table.Table.resize(self,width,height)
+        # print r
+        # return r
+
+        # print box.offset
         self.vscrollbar = None
         if widget.rect.h > box.rect.h:
-            self.vscrollbar = slider.VScrollBar(box.offset[1],0, 65535, 0,step=self.step) 
+            self.vscrollbar = slider.VScrollBar(
+                box.offset[1], 0, 65535, 0, step=self.step
+            )
             self.td(self.vscrollbar)
             self.vscrollbar.connect(CHANGE, self._vscrollbar_changed, None)
-            
+
             vs = self.vscrollbar
-            vs.rect.w,vs.rect.h = vs.resize()
+            vs.rect.w, vs.rect.h = vs.resize()
             box.style.width = self.style.width - vs.rect.w
-            
-            
+
         self.hscrollbar = None
         if widget.rect.w > box.rect.w:
-            self.hscrollbar = slider.HScrollBar(box.offset[0], 0,65535, 0,step=self.step)
+            self.hscrollbar = slider.HScrollBar(
+                box.offset[0], 0, 65535, 0, step=self.step
+            )
             self.hscrollbar.connect(CHANGE, self._hscrollbar_changed, None)
             self.tr()
             self.td(self.hscrollbar)
-            
+
             hs = self.hscrollbar
-            hs.rect.w,hs.rect.h = hs.resize()
+            hs.rect.w, hs.rect.h = hs.resize()
             box.style.height = self.style.height - hs.rect.h
-            
+
         if self.hscrollbar:
             hs = self.hscrollbar
             hs.min = 0
             hs.max = widget.rect.w - box.style.width
             hs.style.width = box.style.width
             hs.size = hs.style.width * box.style.width / widget.rect.w
         else:
             box.offset[0] = 0
-            
+
         if self.vscrollbar:
             vs = self.vscrollbar
             vs.min = 0
             vs.max = widget.rect.h - box.style.height
             vs.style.height = box.style.height
             vs.size = vs.style.height * box.style.height / widget.rect.h
         else:
             box.offset[1] = 0
 
-        #print self.style.width,box.style.width, hs.style.width
-        
-            
-        r = table.Table.resize(self,width,height)
-        #print r
+        # print self.style.width,box.style.width, hs.style.width
+
+        r = table.Table.resize(self, width, height)
+        # print r
         return r
-    
+
     def x_resize(self, width=None, height=None):
-        w,h = table.Table.resize(self, width, height)
+        w, h = table.Table.resize(self, width, height)
         if self.hscrollbar:
             if self.widget.rect.w <= self.sbox.rect.w:
                 self.hscrollbar.size = self.hscrollbar.style.width
             else:
-                self.hscrollbar.size = max(20,self.hscrollbar.style.width * self.sbox.rect.w / self.widget.rect.w)
+                self.hscrollbar.size = max(
+                    20,
+                    self.hscrollbar.style.width * self.sbox.rect.w / self.widget.rect.w,
+                )
             self._hscrollbar_changed(None)
-        if self.widget.rect.h <= self.sbox.rect.h: 
+        if self.widget.rect.h <= self.sbox.rect.h:
             self.vscrollbar.size = self.vscrollbar.style.height
         else:
-            self.vscrollbar.size = max(20,self.vscrollbar.style.height * self.sbox.rect.h / self.widget.rect.h)
+            self.vscrollbar.size = max(
+                20, self.vscrollbar.style.height * self.sbox.rect.h / self.widget.rect.h
+            )
         self._vscrollbar_changed(None)
-        return w,h
+        return w, h
 
     def _vscrollbar_changed(self, xxx):
-        #y = (self.widget.rect.h - self.sbox.rect.h) * self.vscrollbar.value / 1000
-        #if y >= 0: self.sbox.offset[1] = -y
+        # y = (self.widget.rect.h - self.sbox.rect.h) * self.vscrollbar.value / 1000
+        # if y >= 0: self.sbox.offset[1] = -y
         self.sbox.offset[1] = self.vscrollbar.value
         self.sbox.reupdate()
 
     def _hscrollbar_changed(self, xxx):
-        #x = (self.widget.rect.w - self.sbox.rect.w) * self.hscrollbar.value / 1000
-        #if x >= 0: self.sbox.offset[0] = -x
+        # x = (self.widget.rect.w - self.sbox.rect.w) * self.hscrollbar.value / 1000
+        # if x >= 0: self.sbox.offset[0] = -x
         self.sbox.offset[0] = self.hscrollbar.value
         self.sbox.reupdate()
 
-
-    def set_vertical_scroll(self, percents): 
-        if not self.vscrollbar: return
-        self.vscrollbar.value = percents #min(max(percents*10, 0), 1000)
+    def set_vertical_scroll(self, percents):
+        if not self.vscrollbar:
+            return
+        self.vscrollbar.value = percents  # min(max(percents*10, 0), 1000)
         self._vscrollbar_changed(None)
 
-    def set_horizontal_scroll(self, percents): 
-        if not self.hscrollbar: return
-        self.hscrollbar.value = percents #min(max(percents*10, 0), 1000)
+    def set_horizontal_scroll(self, percents):
+        if not self.hscrollbar:
+            return
+        self.hscrollbar.value = percents  # min(max(percents*10, 0), 1000)
         self._hscrollbar_changed(None)
-        
-        
 
 
 class _List_Item(button._button):
-    def __init__(self,label=None,image=None,value=None,**params): #TODO label= could conflict with the module label
-        #param image: an imagez.Image object (optional)
-        #param text: a string object
-        params.setdefault('cls','list.item')
-        button._button.__init__(self,**params)
+    def __init__(
+        self, label=None, image=None, value=None, **params
+    ):  # TODO label= could conflict with the module label
+        # param image: an imagez.Image object (optional)
+        # param text: a string object
+        params.setdefault("cls", "list.item")
+        button._button.__init__(self, **params)
         self.group = None
-        self.value = value #(self, value)
+        self.value = value  # (self, value)
         self.widget = None
-        
-        if type(label) == str: 
-            label = basic.Label(label, cls=self.cls+".label")
+
+        if type(label) == str:
+            label = basic.Label(label, cls=self.cls + ".label")
 
         if image and label:
             self.widget = container.Container()
             self.widget.add(image, 0, 0)
-            #HACK: improper use of .resize()
-            image.rect.w,image.rect.h = image.resize()
+            # HACK: improper use of .resize()
+            image.rect.w, image.rect.h = image.resize()
             self.widget.add(label, image.rect.w, 0)
-        elif image: self.widget = image
-        elif label: self.widget = label
-        
+        elif image:
+            self.widget = image
+        elif label:
+            self.widget = label
+
         self.pcls = ""
-    
-    def resize(self,width=None,height=None):
-         self.widget.rect.w,self.widget.rect.h = self.widget.resize()
-         return self.widget.rect.w,self.widget.rect.h
-#         self.widget._resize()
-#         self.rect.w,self.rect.h = self.widget.rect_margin.w,self.widget.rect_margin.h
-    
-    def event(self,e):
-        button._button.event(self,e)
-        if self.group.value == self.value: self.pcls = "down"
-    
-    def paint(self,s):
-        if self.group.value == self.value: self.pcls = "down"
-        self.widget.paint(surface.subsurface(s,self.widget.rect))
-    
+
+    def resize(self, width=None, height=None):
+        self.widget.rect.w, self.widget.rect.h = self.widget.resize()
+        return self.widget.rect.w, self.widget.rect.h
+
+    #         self.widget._resize()
+    #         self.rect.w,self.rect.h = self.widget.rect_margin.w,self.widget.rect_margin.h
+
+    def event(self, e):
+        button._button.event(self, e)
+        if self.group.value == self.value:
+            self.pcls = "down"
+
+    def paint(self, s):
+        if self.group.value == self.value:
+            self.pcls = "down"
+        self.widget.paint(surface.subsurface(s, self.widget.rect))
+
     def click(self):
         self.group.value = self.value
         for w in self.group.widgets:
-            if w != self: w.pcls = ""
-
+            if w != self:
+                w.pcls = ""
 
 
 class List(ScrollArea):
     """A list of items in an area.
-    
+
     <p>This widget can be a form element, it has a value set to whatever item is selected.</p>
-    
+
     <pre>List(width,height)</pre>
     """
+
     def _change(self, value):
         self.value = self.group.value
         self.send(CHANGE)
 
     def __init__(self, width, height, **params):
-        params.setdefault('cls', 'list')
+        params.setdefault("cls", "list")
         self.table = table.Table(width=width)
         ScrollArea.__init__(self, self.table, width, height, no_hslider=True, **params)
-        
+
         self.items = []
-        
+
         g = group.Group()
         self.group = g
-        g.connect(CHANGE,self._change,None)
+        g.connect(CHANGE, self._change, None)
         self.value = self.group.value = None
-	
-	self.add = self._add
-	self.remove = self._remove
-        
+
+        self.add = self._add
+        self.remove = self._remove
+
     def clear(self):
         """Clear the list.
-        
+
         <pre>List.clear()</pre>
         """
         self.items = []
         self.group = group.Group()
-        self.group.connect(CHANGE,self._change,None)
+        self.group.connect(CHANGE, self._change, None)
         self.table.clear()
         self.set_vertical_scroll(0)
         self.blur(self.myfocus)
-        
-    def _docs(self): #HACK: nasty hack to get the docs in "my way"
+
+    def _docs(self):  # HACK: nasty hack to get the docs in "my way"
         def add(self, label, image=None, value=None):
             """Add an item to the list.
-            
+
             <pre>List.add(label,image=None,value=None)</pre>
-            
+
             <dl>
             <dt>label<dd>a label for the item
             <dt>image<dd>an image for the item
             <dt>value<dd>a value for the item
             </dl>
             """
-            
-        def remove(self,value):
+
+        def remove(self, value):
             """Remove an item from the list.
-            
+
             <pre>List.remove(value)</pre>
-            
+
             <dl>
             <dt>value<dd>a value of an item to remove from the list
             </dl>
             """
-        
-    def _add(self, label, image = None, value=None):
-    	item = _List_Item(label,image=image,value=value)
+
+    def _add(self, label, image=None, value=None):
+        item = _List_Item(label, image=image, value=value)
         self.table.tr()
         self.table.add(item)
         self.items.append(item)
         item.group = self.group
         item.group.add(item)
-        
+
     def _remove(self, item):
-    	for i in self.items:
-		if i.value == item: item = i
-        if item not in self.items: return
+        for i in self.items:
+            if i.value == item:
+                item = i
+            if item not in self.items:
+                return
         item.blur()
         self.items.remove(item)
         self.group.widgets.remove(item)
         self.table.remove_row(item.style.row)
-        
-#class List(ListArea):
+
+
+# class List(ListArea):
 #    def __init__(self,*args,**params):
 #        print 'gui.List','Scheduled to be renamed to ListArea.  API may also be changed in the future.'
 #        ListArea.__init__(self,*args,**params)
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/deprecated.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/deprecated.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,91 @@
 import pygame
 
-from const import *
-import table
-import group
-import button, basic
+from .const import *
+from . import table
+from . import group
+from . import button, basic
+
 
 def action_open(value):
-    print 'gui.action_open',"Scheduled to be deprecated."
-    value.setdefault('x',None)
-    value.setdefault('y',None)
-    value['container'].open(value['window'],value['x'],value['y'])
+    print("gui.action_open", "Scheduled to be deprecated.")
+    value.setdefault("x", None)
+    value.setdefault("y", None)
+    value["container"].open(value["window"], value["x"], value["y"])
+
 
 def action_setvalue(value):
-    print 'gui.action_setvalue',"Scheduled to be deprecated."
-    a,b = value
+    print("gui.action_setvalue", "Scheduled to be deprecated.")
+    a, b = value
     b.value = a.value
 
+
 def action_quit(value):
-    print 'gui.action_quit',"Scheduled to be deprecated."
+    print("gui.action_quit", "Scheduled to be deprecated.")
     value.quit()
 
+
 def action_exec(value):
-    print 'gui.action_exec',"Scheduled to be deprecated."
-    exec(value['script'],globals(),value['dict'])
+    print("gui.action_exec", "Scheduled to be deprecated.")
+    exec(value["script"], globals(), value["dict"])
+
 
 class Toolbox(table.Table):
-    def __setattr__(self,k,v):
-        _v = self.__dict__.get(k,NOATTR)
-        self.__dict__[k]=v
-        if k == 'value' and _v != NOATTR and _v != v: 
+    def __setattr__(self, k, v):
+        _v = self.__dict__.get(k, NOATTR)
+        self.__dict__[k] = v
+        if k == "value" and _v != NOATTR and _v != v:
             self.group.value = v
             for w in self.group.widgets:
-                if w.value != v: w.pcls = ""
-                else: w.pcls = "down"
+                if w.value != v:
+                    w.pcls = ""
+                else:
+                    w.pcls = "down"
             self.repaint()
-    
-    def _change(self,value):
+
+    def _change(self, value):
         self.value = self.group.value
         self.send(CHANGE)
-    
-    def __init__(self,data,cols=0,rows=0,tool_cls='tool',value=None,**params):
-        print 'gui.Toolbox','Scheduled to be deprecated.'
-        params.setdefault('cls','toolbox')
-        table.Table.__init__(self,**params)
-        
-        if cols == 0 and rows == 0: cols = len(data)
-        if cols != 0 and rows != 0: rows = 0
-        
+
+    def __init__(self, data, cols=0, rows=0, tool_cls="tool", value=None, **params):
+        print("gui.Toolbox", "Scheduled to be deprecated.")
+        params.setdefault("cls", "toolbox")
+        table.Table.__init__(self, **params)
+
+        if cols == 0 and rows == 0:
+            cols = len(data)
+        if cols != 0 and rows != 0:
+            rows = 0
+
         self.tools = {}
-        
+
         _value = value
-        
+
         g = group.Group()
         self.group = g
-        g.connect(CHANGE,self._change,None)
+        g.connect(CHANGE, self._change, None)
         self.group.value = _value
-        
-        x,y,p,s = 0,0,None,1
-        for ico,value in data:
-            #from __init__ import theme
-            import app
-            img = app.App.app.theme.get(tool_cls+"."+ico,"","image")
+
+        x, y, p, s = 0, 0, None, 1
+        for ico, value in data:
+            # from __init__ import theme
+            from . import app
+
+            img = app.App.app.theme.get(tool_cls + "." + ico, "", "image")
             if img:
                 i = basic.Image(img)
-            else: i = basic.Label(ico,cls=tool_cls+".label")
-            p = button.Tool(g,i,value,cls=tool_cls)
+            else:
+                i = basic.Label(ico, cls=tool_cls + ".label")
+            p = button.Tool(g, i, value, cls=tool_cls)
             self.tools[ico] = p
-            #p.style.hexpand = 1
-            #p.style.vexpand = 1
-            self.add(p,x,y)
+            # p.style.hexpand = 1
+            # p.style.vexpand = 1
+            self.add(p, x, y)
             s = 0
-            if cols != 0: x += 1
-            if cols != 0 and x == cols: x,y = 0,y+1
-            if rows != 0: y += 1
-            if rows != 0 and y == rows: x,y = x+1,0
+            if cols != 0:
+                x += 1
+            if cols != 0 and x == cols:
+                x, y = 0, y + 1
+            if rows != 0:
+                y += 1
+            if rows != 0 and y == rows:
+                x, y = x + 1, 0
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/container.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/container.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,351 +1,400 @@
 """
 """
 import pygame
 
-from const import *
-import widget, surface
+from .const import *
+from . import widget, surface
+
 
 class Container(widget.Widget):
     """The base container widget, can be used as a template as well as stand alone.
-    
+
     <pre>Container()</pre>
     """
-    def __init__(self,**params):
-        widget.Widget.__init__(self,**params)
+
+    def __init__(self, **params):
+        widget.Widget.__init__(self, **params)
         self.myfocus = None
         self.mywindow = None
         self.myhover = None
-        #self.background = 0
+        # self.background = 0
         self.widgets = []
         self.windows = []
         self.toupdate = {}
         self.topaint = {}
-    
-    def update(self,s):
+
+    def update(self, s):
         updates = []
-        
-        if self.myfocus: self.toupdate[self.myfocus] = self.myfocus
-        
+
+        if self.myfocus:
+            self.toupdate[self.myfocus] = self.myfocus
+
         for w in self.topaint:
             if w is self.mywindow:
                 continue
             else:
-                w.paint(surface.subsurface(s,w.rect))
+                w.paint(surface.subsurface(s, w.rect))
                 updates.append(pygame.rect.Rect(w.rect))
-        
+
         for w in self.toupdate:
             if w is self.mywindow:
                 continue
-            else:            
-                us = w.update(surface.subsurface(s,w.rect))
+            else:
+                us = w.update(surface.subsurface(s, w.rect))
             if us:
                 for u in us:
-                    updates.append(pygame.rect.Rect(u.x + w.rect.x,u.y+w.rect.y,u.w,u.h))
-        
+                    updates.append(
+                        pygame.rect.Rect(u.x + w.rect.x, u.y + w.rect.y, u.w, u.h)
+                    )
+
         for w in self.topaint:
             if w is self.mywindow:
-                w.paint(self.top_surface(s,w))
+                w.paint(self.top_surface(s, w))
                 updates.append(pygame.rect.Rect(w.rect))
             else:
-                continue 
-        
+                continue
+
         for w in self.toupdate:
             if w is self.mywindow:
-                us = w.update(self.top_surface(s,w))
-            else:            
-                continue 
+                us = w.update(self.top_surface(s, w))
+            else:
+                continue
             if us:
                 for u in us:
-                    updates.append(pygame.rect.Rect(u.x + w.rect.x,u.y+w.rect.y,u.w,u.h))
-        
+                    updates.append(
+                        pygame.rect.Rect(u.x + w.rect.x, u.y + w.rect.y, u.w, u.h)
+                    )
+
         self.topaint = {}
         self.toupdate = {}
-        
+
         return updates
-    
-    def repaint(self,w=None):
+
+    def repaint(self, w=None):
         if not w:
             return widget.Widget.repaint(self)
         self.topaint[w] = w
         self.reupdate()
-    
-    def reupdate(self,w=None):
+
+    def reupdate(self, w=None):
         if not w:
             return widget.Widget.reupdate(self)
         self.toupdate[w] = w
         self.reupdate()
-    
-    def paint(self,s):
+
+    def paint(self, s):
         self.toupdate = {}
         self.topaint = {}
-        
+
         for w in self.widgets:
             ok = False
             try:
-                sub = surface.subsurface(s,w.rect)
+                sub = surface.subsurface(s, w.rect)
                 ok = True
-            except: 
-                print 'container.paint(): %s not in %s'%(w.__class__.__name__,self.__class__.__name__)
-                print s.get_width(),s.get_height(),w.rect
+            except:
+                print(
+                    "container.paint(): %s not in %s"
+                    % (w.__class__.__name__, self.__class__.__name__)
+                )
+                print(s.get_width(), s.get_height(), w.rect)
                 ok = False
-            if ok: w.paint(sub)
-        
+            if ok:
+                w.paint(sub)
+
         for w in self.windows:
-            w.paint(self.top_surface(s,w))
-    
-    def top_surface(self,s,w):
-        x,y = s.get_abs_offset()
+            w.paint(self.top_surface(s, w))
+
+    def top_surface(self, s, w):
+        x, y = s.get_abs_offset()
         s = s.get_abs_parent()
-        return surface.subsurface(s,(x+w.rect.x,y+w.rect.y,w.rect.w,w.rect.h))
-    
-    def event(self,e):
+        return surface.subsurface(s, (x + w.rect.x, y + w.rect.y, w.rect.w, w.rect.h))
+
+    def event(self, e):
         if self.mywindow and e.type == MOUSEBUTTONDOWN:
             w = self.mywindow
             if self.myfocus is w:
-                if not w.rect.collidepoint(e.pos): self.blur(w)
+                if not w.rect.collidepoint(e.pos):
+                    self.blur(w)
             if not self.myfocus:
-                if w.rect.collidepoint(e.pos): self.focus(w)
-        
+                if w.rect.collidepoint(e.pos):
+                    self.focus(w)
+
         if not self.mywindow:
             #### by Gal Koren
             ##
             ## if e.type == FOCUS:
             if e.type == FOCUS and not self.myfocus:
-                #self.first()
+                # self.first()
                 pass
             elif e.type == EXIT:
-                if self.myhover: self.exit(self.myhover)
+                if self.myhover:
+                    self.exit(self.myhover)
             elif e.type == BLUR:
-                if self.myfocus: self.blur(self.myfocus)
+                if self.myfocus:
+                    self.blur(self.myfocus)
             elif e.type == MOUSEBUTTONDOWN:
                 h = None
                 for w in self.widgets:
                     if w.rect.collidepoint(e.pos):
                         h = w
-                        if self.myfocus is not w: self.focus(w)
+                        if self.myfocus is not w:
+                            self.focus(w)
                 if not h and self.myfocus:
                     self.blur(self.myfocus)
             elif e.type == MOUSEMOTION:
                 if 1 in e.buttons:
-                    if self.myfocus: ws = [self.myfocus]
-                    else: ws = []
-                else: ws = self.widgets
-                
+                    if self.myfocus:
+                        ws = [self.myfocus]
+                    else:
+                        ws = []
+                else:
+                    ws = self.widgets
+
                 h = None
                 for w in ws:
                     if w.rect.collidepoint(e.pos):
                         h = w
-                        if self.myhover is not w: self.enter(w)
+                        if self.myhover is not w:
+                            self.enter(w)
                 if not h and self.myhover:
                     self.exit(self.myhover)
                 w = self.myhover
-                
+
                 if w and w is not self.myfocus:
-                    sub = pygame.event.Event(e.type,{
-                        'buttons':e.buttons,
-                        'pos':(e.pos[0]-w.rect.x,e.pos[1]-w.rect.y),
-                        'rel':e.rel})
+                    sub = pygame.event.Event(
+                        e.type,
+                        {
+                            "buttons": e.buttons,
+                            "pos": (e.pos[0] - w.rect.x, e.pos[1] - w.rect.y),
+                            "rel": e.rel,
+                        },
+                    )
                     w._event(sub)
-        
+
         w = self.myfocus
         if w:
             sub = e
-            
+
             if e.type == MOUSEBUTTONUP or e.type == MOUSEBUTTONDOWN:
-                sub = pygame.event.Event(e.type,{
-                    'button':e.button,
-                    'pos':(e.pos[0]-w.rect.x,e.pos[1]-w.rect.y)})
+                sub = pygame.event.Event(
+                    e.type,
+                    {
+                        "button": e.button,
+                        "pos": (e.pos[0] - w.rect.x, e.pos[1] - w.rect.y),
+                    },
+                )
                 w._event(sub)
             elif e.type == CLICK and self.myhover is w:
-                sub = pygame.event.Event(e.type,{
-                    'button':e.button,
-                    'pos':(e.pos[0]-w.rect.x,e.pos[1]-w.rect.y)})
+                sub = pygame.event.Event(
+                    e.type,
+                    {
+                        "button": e.button,
+                        "pos": (e.pos[0] - w.rect.x, e.pos[1] - w.rect.y),
+                    },
+                )
                 w._event(sub)
-            elif e.type == CLICK: #a dead click
+            elif e.type == CLICK:  # a dead click
                 pass
             elif e.type == MOUSEMOTION:
-                sub = pygame.event.Event(e.type,{
-                    'buttons':e.buttons,
-                    'pos':(e.pos[0]-w.rect.x,e.pos[1]-w.rect.y),
-                    'rel':e.rel})
+                sub = pygame.event.Event(
+                    e.type,
+                    {
+                        "buttons": e.buttons,
+                        "pos": (e.pos[0] - w.rect.x, e.pos[1] - w.rect.y),
+                        "rel": e.rel,
+                    },
+                )
                 w._event(sub)
             else:
                 w._event(sub)
-    
-    def remove(self,w):
+
+    def remove(self, w):
         """Remove a widget from the container.
-        
+
         <pre>Container.remove(w)</pre>
         """
         self.blur(w)
         self.widgets.remove(w)
-        #self.repaint()
+        # self.repaint()
         self.chsize()
-    
-    def add(self,w,x,y):
+
+    def add(self, w, x, y):
         """Add a widget to the container.
-        
+
         <pre>Container.add(w,x,y)</pre>
-        
+
         <dl>
         <dt>x, y<dd>position of the widget
         </dl>
         """
         w.style.x = x
-        w.style.y = y 
+        w.style.y = y
         w.container = self
-        #NOTE: this might fix it, sort of...
-        #but the thing is, we don't really want to resize
-        #something if it is going to get resized again later
-        #for no reason...
-        #w.rect.x,w.rect.y = w.style.x,w.style.y
-        #w.rect.w, w.rect.h = w.resize()
+        # NOTE: this might fix it, sort of...
+        # but the thing is, we don't really want to resize
+        # something if it is going to get resized again later
+        # for no reason...
+        # w.rect.x,w.rect.y = w.style.x,w.style.y
+        # w.rect.w, w.rect.h = w.resize()
         self.widgets.append(w)
         self.chsize()
-    
-    def open(self,w=None,x=None,y=None):
-        from app import App #HACK: I import it here to prevent circular importing
+
+    def open(self, w=None, x=None, y=None):
+        from .app import App  # HACK: I import it here to prevent circular importing
+
         if not w:
-            if (not hasattr(self,'container') or not self.container) and self is not App.app:
+            if (
+                not hasattr(self, "container") or not self.container
+            ) and self is not App.app:
                 self.container = App.app
-            #print 'top level open'
+            # print 'top level open'
             return widget.Widget.open(self)
-        
+
         if self.container:
-            if x != None: return self.container.open(w,self.rect.x+x,self.rect.y+y)
+            if x != None:
+                return self.container.open(w, self.rect.x + x, self.rect.y + y)
             return self.container.open(w)
-        
+
         w.container = self
-        
-        if w.rect.w == 0 or w.rect.h == 0: #this might be okay, not sure if needed.
-            w.rect.w,w.rect.h = w.resize()
-        
-        if x == None or y == None: #auto center the window
-            #w.style.x,w.style.y = 0,0
-            w.rect.x = (self.rect.w-w.rect.w)/2
-            w.rect.y = (self.rect.h-w.rect.h)/2
-            #w.resize()
-            #w._resize(self.rect.w,self.rect.h)
-        else: #show it where we want it
+
+        if w.rect.w == 0 or w.rect.h == 0:  # this might be okay, not sure if needed.
+            w.rect.w, w.rect.h = w.resize()
+
+        if x == None or y == None:  # auto center the window
+            # w.style.x,w.style.y = 0,0
+            w.rect.x = (self.rect.w - w.rect.w) / 2
+            w.rect.y = (self.rect.h - w.rect.h) / 2
+            # w.resize()
+            # w._resize(self.rect.w,self.rect.h)
+        else:  # show it where we want it
             w.rect.x = x
             w.rect.y = y
-            #w._resize()
-        
-        
+            # w._resize()
+
         self.windows.append(w)
         self.mywindow = w
         self.focus(w)
         self.repaint(w)
         w.send(OPEN)
-    
-    def close(self,w=None):
+
+    def close(self, w=None):
         if not w:
             return widget.Widget.close(self)
-            
-        if self.container: #make sure we're in the App
+
+        if self.container:  # make sure we're in the App
             return self.container.close(w)
-        
-        if self.myfocus is w: self.blur(w)
-        
-        if w not in self.windows: return #no need to remove it twice! happens.
-        
+
+        if self.myfocus is w:
+            self.blur(w)
+
+        if w not in self.windows:
+            return  # no need to remove it twice! happens.
+
         self.windows.remove(w)
-        
+
         self.mywindow = None
         if self.windows:
             self.mywindow = self.windows[-1]
             self.focus(self.mywindow)
-        
+
         if not self.mywindow:
-            self.myfocus = self.widget #HACK: should be done fancier, i think..
+            self.myfocus = self.widget  # HACK: should be done fancier, i think..
             if not self.myhover:
                 self.enter(self.widget)
-            
+
         self.repaintall()
         w.send(CLOSE)
-    
-    def focus(self,w=None):
-        widget.Widget.focus(self) ### by Gal koren
-#        if not w:
-#            return widget.Widget.focus(self)
-        if not w: return
-        if self.myfocus: self.blur(self.myfocus)
-        if self.myhover is not w: self.enter(w)
+
+    def focus(self, w=None):
+        widget.Widget.focus(self)  ### by Gal koren
+        #        if not w:
+        #            return widget.Widget.focus(self)
+        if not w:
+            return
+        if self.myfocus:
+            self.blur(self.myfocus)
+        if self.myhover is not w:
+            self.enter(w)
         self.myfocus = w
         w._event(pygame.event.Event(FOCUS))
-    
-    def blur(self,w=None):
+
+    def blur(self, w=None):
         if not w:
             return widget.Widget.blur(self)
         if self.myfocus is w:
-            if self.myhover is w: self.exit(w)
+            if self.myhover is w:
+                self.exit(w)
             self.myfocus = None
             w._event(pygame.event.Event(BLUR))
-    
-    def enter(self,w):
-        if self.myhover: self.exit(self.myhover)
+
+    def enter(self, w):
+        if self.myhover:
+            self.exit(self.myhover)
         self.myhover = w
         w._event(pygame.event.Event(ENTER))
-    
-    def exit(self,w):
+
+    def exit(self, w):
         if self.myhover and self.myhover is w:
             self.myhover = None
-            w._event(pygame.event.Event(EXIT))    
-    
-    
-#     def first(self):
-#         for w in self.widgets:
-#             if w.focusable:
-#                 self.focus(w)
-#                 return
-#         if self.container: self.container.next(self)
-    
-#     def next(self,w):
-#         if w not in self.widgets: return #HACK: maybe.  this happens in windows for some reason...
-#         
-#         for w in self.widgets[self.widgets.index(w)+1:]:
-#             if w.focusable:
-#                 self.focus(w)
-#                 return
-#         if self.container: return self.container.next(self)
-    
-    
-    def _next(self,orig=None):
+            w._event(pygame.event.Event(EXIT))
+
+    #     def first(self):
+    #         for w in self.widgets:
+    #             if w.focusable:
+    #                 self.focus(w)
+    #                 return
+    #         if self.container: self.container.next(self)
+
+    #     def next(self,w):
+    #         if w not in self.widgets: return #HACK: maybe.  this happens in windows for some reason...
+    #
+    #         for w in self.widgets[self.widgets.index(w)+1:]:
+    #             if w.focusable:
+    #                 self.focus(w)
+    #                 return
+    #         if self.container: return self.container.next(self)
+
+    def _next(self, orig=None):
         start = 0
-        if orig in self.widgets: start = self.widgets.index(orig)+1
+        if orig in self.widgets:
+            start = self.widgets.index(orig) + 1
         for w in self.widgets[start:]:
             if not w.disabled and w.focusable:
-                if isinstance(w,Container):
+                if isinstance(w, Container):
                     if w._next():
                         return True
                 else:
                     self.focus(w)
                     return True
         return False
-                
-    def next(self,w):
-        if w not in self.widgets: return #HACK: maybe.  this happens in windows for some reason...
-        
-        if self._next(w): return True
-        if self.container: return self.container.next(self)
-    
-    
-    def previous(self,w):
-        print 'Container.previous: n/a'
-    
-    def resize(self,width=None,height=None):
-        #r = self.rect
-        #r.w,r.h = 0,0
-        ww,hh = 0,0
-        if self.style.width: ww = self.style.width
-        if self.style.height: hh = self.style.height
-        
+
+    def next(self, w):
+        if w not in self.widgets:
+            return  # HACK: maybe.  this happens in windows for some reason...
+
+        if self._next(w):
+            return True
+        if self.container:
+            return self.container.next(self)
+
+    def previous(self, w):
+        print("Container.previous: n/a")
+
+    def resize(self, width=None, height=None):
+        # r = self.rect
+        # r.w,r.h = 0,0
+        ww, hh = 0, 0
+        if self.style.width:
+            ww = self.style.width
+        if self.style.height:
+            hh = self.style.height
+
         for w in self.widgets:
-            #w.rect.w,w.rect.h = 0,0
-            w.rect.x,w.rect.y = w.style.x,w.style.y
+            # w.rect.w,w.rect.h = 0,0
+            w.rect.x, w.rect.y = w.style.x, w.style.y
             w.rect.w, w.rect.h = w.resize()
-            #w._resize()
-            
-            ww = max(ww,w.rect.right)
-            hh = max(hh,w.rect.bottom)
-        return ww,hh
+            # w._resize()
+
+            ww = max(ww, w.rect.right)
+            hh = max(hh, w.rect.bottom)
+        return ww, hh
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/form.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/form.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,86 @@
 """
 """
-import widget
+from . import widget
+
 
 class Form(widget.Widget):
     """A form that automatically will contain all named widgets.
-    
+
     <p>After a form is created, all named widget that are subsequently created are added
     to that form.  You may use dict style access to access named widgets.</p>
-    
+
     <pre>Form()</pre>
-    
+
     <strong>Example</strong>
     <code>
     f = gui.Form()
-    
+
     w = gui.Input("Phil",name="firstname")
     w = gui.Input("Hassey",name="lastname")
-    
+
     print f.results()
     print ''
     print f.items()
     print ''
     print f['firstname'].value
     print f['lastname'].value
     </code>
     """
-    
+
     def __init__(self):
-        widget.Widget.__init__(self,decorate=False)
+        widget.Widget.__init__(self, decorate=False)
         self._elist = []
         self._emap = {}
         self._dirty = 0
         Form.form = self
-    
-    def add(self,e,name=None,value=None):
-        if name != None: e.name = name
-        if value != None: e.value = value
+
+    def add(self, e, name=None, value=None):
+        if name != None:
+            e.name = name
+        if value != None:
+            e.value = value
         self._elist.append(e)
         self._dirty = 1
-    
+
     def _clean(self):
         for e in self._elist[:]:
-            if not hasattr(e,'name') or e.name == None:
+            if not hasattr(e, "name") or e.name == None:
                 self._elist.remove(e)
         self._emap = {}
         for e in self._elist:
             self._emap[e.name] = e
         self._dirty = 0
-    
-    def __getitem__(self,k):
-        if self._dirty: self._clean()
+
+    def __getitem__(self, k):
+        if self._dirty:
+            self._clean()
         return self._emap[k]
-    
-    def __contains__(self,k):
-        if self._dirty: self._clean()
-        if k in self._emap: return True
+
+    def __contains__(self, k):
+        if self._dirty:
+            self._clean()
+        if k in self._emap:
+            return True
         return False
-    
+
     def results(self):
         """Return a dict of name => values.
-        
+
         <pre>Form.results(): return dict</pre>
         """
-        if self._dirty: self._clean()
+        if self._dirty:
+            self._clean()
         r = {}
         for e in self._elist:
             r[e.name] = e.value
         return r
-    
+
     def items(self):
         """Return a list of name, value keys.
-        
+
         <pre>Form.items(): return list</pre>
         """
-        return self.results().items()
-    
-    #def start(self):
+        return list(self.results().items())
+
+    # def start(self):
     #    Object.start(self,-1)
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/menus.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/menus.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,120 +1,128 @@
 """
 """
-from const import *
-import table
-import basic, button
+from .const import *
+from . import table
+from . import basic, button
+
 
 class _Menu_Options(table.Table):
-    def __init__(self,menu,**params):
-        table.Table.__init__(self,**params)
-        
+    def __init__(self, menu, **params):
+        table.Table.__init__(self, **params)
+
         self.menu = menu
-    
-    def event(self,e):
+
+    def event(self, e):
         handled = False
         if e.type == MOUSEMOTION:
-            abspos = e.pos[0]+self.rect.x,e.pos[1]+self.rect.y
+            abspos = e.pos[0] + self.rect.x, e.pos[1] + self.rect.y
             for w in self.menu.container.widgets:
                 if not w is self.menu:
                     if w.rect.collidepoint(abspos):
                         self.menu._close(None)
                         w._open(None)
                         handled = True
         elif e.type == MOUSEBUTTONUP:
-            abspos = e.pos[0]+self.rect.x,e.pos[1]+self.rect.y
-            if not self.rect.collidepoint(abspos) and not self.menu.container.rect.collidepoint(abspos):
+            abspos = e.pos[0] + self.rect.x, e.pos[1] + self.rect.y
+            if not self.rect.collidepoint(
+                abspos
+            ) and not self.menu.container.rect.collidepoint(abspos):
                 self.close()
                 handled = True
-        
-        if not handled: table.Table.event(self,e)
+
+        if not handled:
+            table.Table.event(self, e)
+
 
 class _Menu(button.Button):
-    def __init__(self,widget=None,**params): #TODO widget= could conflict with module widget
-        params.setdefault('cls','menu')
-        button.Button.__init__(self,widget,**params)
-        
+    def __init__(
+        self, widget=None, **params
+    ):  # TODO widget= could conflict with module widget
+        params.setdefault("cls", "menu")
+        button.Button.__init__(self, widget, **params)
+
         self._cls = self.cls
-        self.options = _Menu_Options(self, cls=self.cls+".options")
-        
-        #self.options.connect(BLUR,self._close,None)
-        self.connect(CLICK,self._open,None)
-        
+        self.options = _Menu_Options(self, cls=self.cls + ".options")
+
+        # self.options.connect(BLUR,self._close,None)
+        self.connect(CLICK, self._open, None)
+
         self.pos = 0
-    
-    def _open(self,value):
+
+    def _open(self, value):
         self.cls = self._cls + "-open"
         self.repaint()
-        self.container.open(self.options,self.rect.x,self.rect.bottom)
-        #action_open({'container':self.container,'window':self.options,'x':self.rect.x,'y':self.rect.bottom})
+        self.container.open(self.options, self.rect.x, self.rect.bottom)
+        # action_open({'container':self.container,'window':self.options,'x':self.rect.x,'y':self.rect.bottom})
         self.options.blur(self.options.myfocus)
         self.options.focus()
         self.repaint()
-        
-    def _close(self,value):
+
+    def _close(self, value):
         self.cls = self._cls
         self.repaint()
         self.options.close()
-    
-    def _value(self,value):
-        #self.options.close()
+
+    def _value(self, value):
+        # self.options.close()
         self._close(None)
-        if value['fnc'] != None:
-            value['fnc'](value['value'])
-    
-#    def resize(self,width=None,height=None):
-#        w,h = button.Button.resize(self,width,height)
-#        
-#        return w,h
-#        #self.options._resize()
-    
-    def add(self,w,fnc=None,value=None):
-        #w.resize()
-        
+        if value["fnc"] != None:
+            value["fnc"](value["value"])
+
+    #    def resize(self,width=None,height=None):
+    #        w,h = button.Button.resize(self,width,height)
+    #
+    #        return w,h
+    #        #self.options._resize()
+
+    def add(self, w, fnc=None, value=None):
+        # w.resize()
+
         w.style.align = -1
-        b = button.Button(w,cls=self.cls+".option")
-        #b.style.hexpand = 1
-        b.connect(CLICK,self._value,{'fnc':fnc,'value':value})
-        
-        #self.options.add(b,0,self.pos,1,1,-1,0)
+        b = button.Button(w, cls=self.cls + ".option")
+        # b.style.hexpand = 1
+        b.connect(CLICK, self._value, {"fnc": fnc, "value": value})
+
+        # self.options.add(b,0,self.pos,1,1,-1,0)
         self.options.tr()
         self.options.add(b)
-        #self.pos += 1
-        
+        # self.pos += 1
+
         return b
 
+
 class Menus(table.Table):
     """A drop down menu bar.
-    
+
     <pre>Menus(data)</pre>
-    
+
     <dl>
     <dt>data<dd>Menu data, a list of (path,fnc,value), see example below
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     data = [
         ('File/Save',fnc_save,None),
         ('File/New',fnc_new,None),
         ('Edit/Copy',fnc_copy,None),
         ('Edit/Cut',fnc_cut,None),
         ('Help/About',fnc_help,help_about_content),
         ('Help/Reference',fnc_help,help_reference_content),
         ]
     w = Menus(data)
     """
-    
-    def __init__(self,data,menu_cls='menu',**params):
-        params.setdefault('cls','menus')
-        table.Table.__init__(self,**params)
-        
-        n,m,mt = 0,None,None
-        for path,cmd,value in data:
+
+    def __init__(self, data, menu_cls="menu", **params):
+        params.setdefault("cls", "menus")
+        table.Table.__init__(self, **params)
+
+        n, m, mt = 0, None, None
+        for path, cmd, value in data:
             parts = path.split("/")
             if parts[0] != mt:
                 mt = parts[0]
-                m = _Menu(basic.Label(mt,cls=menu_cls+".label"),cls=menu_cls)
-                self.add(m,n,0)
+                m = _Menu(basic.Label(mt, cls=menu_cls + ".label"), cls=menu_cls)
+                self.add(m, n, 0)
                 n += 1
-            m.add(basic.Label(parts[1],cls=m.cls+".option.label"),cmd,value)
-            #m.resize()
+            m.add(basic.Label(parts[1], cls=m.cls + ".option.label"), cmd, value)
+            # m.resize()
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/input.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/input.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,155 +1,165 @@
 """
 """
 import pygame
 from pygame.locals import *
 
-from const import *
-import widget
+from .const import *
+from . import widget
+
 
 class Input(widget.Widget):
     """A single line text input.
-    
+
     <pre>Input(value="",size=20)</pre>
-    
+
     <dl>
     <dt>value<dd>initial text
     <dt>size<dd>size for the text box, in characters
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     w = Input(value="Cuzco the Goat",size=20)
-    
+
     w = Input("Marbles")
     </code>
-    
+
     """
-    def __init__(self,value="",size=20,**params):
-        params.setdefault('cls','input')
-        widget.Widget.__init__(self,**params)
+
+    def __init__(self, value="", size=20, **params):
+        params.setdefault("cls", "input")
+        widget.Widget.__init__(self, **params)
         self.value = value
         self.pos = len(str(value))
         self.vpos = 0
         self.font = self.style.font
-        w,h = self.font.size("e"*size)
-        self.style.width,self.style.height = w,h
-        #self.rect.w=w+self.style.padding_left+self.style.padding_right;
-        #self.rect.h=h+self.style.padding_top+self.style.padding_bottom;
-    
-    def paint(self,s):
-        
-        r = pygame.Rect(0,0,self.rect.w,self.rect.h)
-        
-        cs = 2 #NOTE: should be in a style
-        
-        w,h = self.font.size(self.value[0:self.pos])
-        x = w-self.vpos
-        if x < 0: self.vpos -= -x
-        if x+cs > s.get_width(): self.vpos += x+cs-s.get_width()
-        
-        s.blit(self.font.render(self.value, 1, self.style.color),(-self.vpos,0))
-        
+        w, h = self.font.size("e" * size)
+        self.style.width, self.style.height = w, h
+        # self.rect.w=w+self.style.padding_left+self.style.padding_right;
+        # self.rect.h=h+self.style.padding_top+self.style.padding_bottom;
+
+    def paint(self, s):
+        r = pygame.Rect(0, 0, self.rect.w, self.rect.h)
+
+        cs = 2  # NOTE: should be in a style
+
+        w, h = self.font.size(self.value[0 : self.pos])
+        x = w - self.vpos
+        if x < 0:
+            self.vpos -= -x
+        if x + cs > s.get_width():
+            self.vpos += x + cs - s.get_width()
+
+        s.blit(self.font.render(self.value, 1, self.style.color), (-self.vpos, 0))
+
         if self.container.myfocus is self:
-            w,h = self.font.size(self.value[0:self.pos])
-            r.x = w-self.vpos
+            w, h = self.font.size(self.value[0 : self.pos])
+            r.x = w - self.vpos
             r.w = cs
             r.h = h
-            s.fill(self.style.color,r)
-    
-    def _setvalue(self,v):
-        self.__dict__['value'] = v
+            s.fill(self.style.color, r)
+
+    def _setvalue(self, v):
+        self.__dict__["value"] = v
         self.send(CHANGE)
-    
-    def event(self,e):
-        if e.type == KEYDOWN:    
+
+    def event(self, e):
+        if e.type == KEYDOWN:
             if e.key == K_BACKSPACE:
                 if self.pos:
-                    self._setvalue(self.value[:self.pos-1] + self.value[self.pos:])
+                    self._setvalue(self.value[: self.pos - 1] + self.value[self.pos :])
                     self.pos -= 1
             elif e.key == K_DELETE:
                 if len(self.value) > self.pos:
-                    self._setvalue(self.value[:self.pos] + self.value[self.pos+1:])
-            elif e.key == K_HOME: 
+                    self._setvalue(self.value[: self.pos] + self.value[self.pos + 1 :])
+            elif e.key == K_HOME:
                 self.pos = 0
             elif e.key == K_END:
                 self.pos = len(self.value)
             elif e.key == K_LEFT:
-                if self.pos > 0: self.pos -= 1
+                if self.pos > 0:
+                    self.pos -= 1
             elif e.key == K_RIGHT:
-                if self.pos < len(self.value): self.pos += 1
+                if self.pos < len(self.value):
+                    self.pos += 1
             elif e.key == K_RETURN:
-                self.next()
+                next(self)
             elif e.key == K_TAB:
-                self.next()    
+                next(self)
             else:
-                #c = str(e.unicode)
-                c = (e.unicode).encode('latin-1')
+                # c = str(e.unicode)
+                c = (e.str).encode("latin-1")
                 if c:
-                    self._setvalue(self.value[:self.pos] + c + self.value[self.pos:])
+                    self._setvalue(self.value[: self.pos] + c + self.value[self.pos :])
                     self.pos += 1
             self.repaint()
         elif e.type == FOCUS:
             self.repaint()
         elif e.type == BLUR:
             self.repaint()
-        
+
         self.pcls = ""
-        if self.container.myfocus is self: self.pcls = "focus"
-    
-    def __setattr__(self,k,v):
-        if k == 'value':
-            if v == None: v = ''
+        if self.container.myfocus is self:
+            self.pcls = "focus"
+
+    def __setattr__(self, k, v):
+        if k == "value":
+            if v == None:
+                v = ""
             v = str(v)
             self.pos = len(v)
-        _v = self.__dict__.get(k,NOATTR)
-        self.__dict__[k]=v
-        if k == 'value' and _v != NOATTR and _v != v: 
+        _v = self.__dict__.get(k, NOATTR)
+        self.__dict__[k] = v
+        if k == "value" and _v != NOATTR and _v != v:
             self.send(CHANGE)
             self.repaint()
-            
+
+
 class Password(Input):
     """A password input, text is *-ed out.
-    
+
     <pre>Password(value="",size=20)</pre>
-    
+
     <dl>
     <dt>value<dd>initial text
     <dt>size<dd>size for the text box, in characters
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     w = Password(value="password",size=20)
-    
+
     w = Password("53[r3+")
     </code>
-    
+
     """
 
-    def paint(self,s):
-        hidden="*"
-        show=len(self.value)*hidden
-        
-        #print "self.value:",self.value
-
-        if self.pos == None: self.pos = len(self.value)
-        
-        r = pygame.Rect(0,0,self.rect.w,self.rect.h)
-        
-        cs = 2 #NOTE: should be in a style
-        
-        w,h = self.font.size(show)
-        x = w-self.vpos
-        if x < 0: self.vpos -= -x
-        if x+cs > s.get_width(): self.vpos += x+cs-s.get_width()
-        
-        s.blit(self.font.render(show, 1, self.style.color),(-self.vpos,0))
-        
+    def paint(self, s):
+        hidden = "*"
+        show = len(self.value) * hidden
+
+        # print "self.value:",self.value
+
+        if self.pos == None:
+            self.pos = len(self.value)
+
+        r = pygame.Rect(0, 0, self.rect.w, self.rect.h)
+
+        cs = 2  # NOTE: should be in a style
+
+        w, h = self.font.size(show)
+        x = w - self.vpos
+        if x < 0:
+            self.vpos -= -x
+        if x + cs > s.get_width():
+            self.vpos += x + cs - s.get_width()
+
+        s.blit(self.font.render(show, 1, self.style.color), (-self.vpos, 0))
+
         if self.container.myfocus is self:
-            #w,h = self.font.size(self.value[0:self.pos])            
-            w,h = self.font.size(show[0:self.pos])
-            r.x = w-self.vpos
+            # w,h = self.font.size(self.value[0:self.pos])
+            w, h = self.font.size(show[0 : self.pos])
+            r.x = w - self.vpos
             r.w = cs
             r.h = h
-            s.fill(self.style.color,r)
-                       
+            s.fill(self.style.color, r)
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/document.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/document.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,125 @@
 """
 """
 import pygame
 
-import container
-import layout
+from . import container
+from . import layout
+
 
 class _document_widget:
-    def __init__(self,w,align=None):
-        #w.rect.w,w.rect.h = w.resize()
-        #self.rect = w.rect
+    def __init__(self, w, align=None):
+        # w.rect.w,w.rect.h = w.resize()
+        # self.rect = w.rect
         self.widget = w
-        if align != None: self.align = align
+        if align != None:
+            self.align = align
+
 
 class Document(container.Container):
     """A document container contains many widgets strung together in a document format.  (How informative!)
-    
+
     <pre>Document()</pre>
-    
+
     """
-    def __init__(self,**params):
-        params.setdefault('cls','document')
-        container.Container.__init__(self,**params)
-        self.layout =  layout.Layout(pygame.Rect(0,0,self.rect.w,self.rect.h))
-    
-    def add(self,e,align=None):
+
+    def __init__(self, **params):
+        params.setdefault("cls", "document")
+        container.Container.__init__(self, **params)
+        self.layout = layout.Layout(pygame.Rect(0, 0, self.rect.w, self.rect.h))
+
+    def add(self, e, align=None):
         """Add a widget.
-        
+
         <pre>Document.add(e,align=None)</pre>
-        
+
         <dl>
         <dt>e<dd>widget
         <dt>align<dd>alignment (None,-1,0,1)
         </dl>
         """
-        dw = _document_widget(e,align)
+        dw = _document_widget(e, align)
         self.layout.add(dw)
         e.container = self
         e._c_dw = dw
         self.widgets.append(e)
         self.chsize()
-        
-    def remove(self,e):
+
+    def remove(self, e):
         self.layout._widgets.remove(e._c_dw)
         self.widgets.remove(e)
         self.chsize()
-        
-    
-    def block(self,align):
+
+    def block(self, align):
         """Start a new block.
-        
+
         <pre>Document.block(align)</pre>
-        
+
         <dl>
         <dt>align<dd>alignment of block (-1,0,1)
         </dl>
         """
         self.layout.add(align)
-    
-    def space(self,e):
+
+    def space(self, e):
         """Add a spacer.
-        
+
         <pre>Document.space(e)</pre>
-        
+
         <dl>
         <dt>e<dd>a (w,h) size for the spacer
         </dl>
         """
         self.layout.add(e)
-    
-    def br(self,height):
+
+    def br(self, height):
         """Add a line break.
-        
+
         <pre>Document.br(height)</pre>
-        
+
         <dl>
         <dt>height<dd>height of line break
         </dl>
         """
-        self.layout.add((0,height))
-    
-    def resize(self,width=None,height=None):
-        if self.style.width: width = self.style.width
-        if self.style.height: height = self.style.height
-        
+        self.layout.add((0, height))
+
+    def resize(self, width=None, height=None):
+        if self.style.width:
+            width = self.style.width
+        if self.style.height:
+            height = self.style.height
+
         for w in self.widgets:
-            w.rect.w,w.rect.h = w.resize()
-            
-            if (width != None and w.rect.w > width) or (height != None and w.rect.h > height):
-                w.rect.w,w.rect.h = w.resize(width,height)
-            
+            w.rect.w, w.rect.h = w.resize()
+
+            if (width != None and w.rect.w > width) or (
+                height != None and w.rect.h > height
+            ):
+                w.rect.w, w.rect.h = w.resize(width, height)
+
             dw = w._c_dw
-            dw.rect = pygame.Rect(0,0,w.rect.w,w.rect.h)
-        
-        if width == None: width = 65535
-        self.layout.rect = pygame.Rect(0,0,width,0)
+            dw.rect = pygame.Rect(0, 0, w.rect.w, w.rect.h)
+
+        if width == None:
+            width = 65535
+        self.layout.rect = pygame.Rect(0, 0, width, 0)
         self.layout.resize()
-        
+
         _max_w = 0
-        
+
         for w in self.widgets:
-            #xt,xl,xb,xr = w.getspacing()
+            # xt,xl,xb,xr = w.getspacing()
             dw = w._c_dw
-            w.style.x,w.style.y,w.rect.w,w.rect.h = dw.rect.x,dw.rect.y,dw.rect.w,dw.rect.h
-            #w.resize()
-            w.rect.x,w.rect.y = w.style.x,w.style.y
-            _max_w = max(_max_w,w.rect.right)
-        
-        #self.rect.w = _max_w #self.layout.rect.w
-        #self.rect.h = self.layout.rect.h
-        #print 'document',_max_w,self.layout.rect.h
-        return _max_w,self.layout.rect.h
+            w.style.x, w.style.y, w.rect.w, w.rect.h = (
+                dw.rect.x,
+                dw.rect.y,
+                dw.rect.w,
+                dw.rect.h,
+            )
+            # w.resize()
+            w.rect.x, w.rect.y = w.style.x, w.style.y
+            _max_w = max(_max_w, w.rect.right)
+
+        # self.rect.w = _max_w #self.layout.rect.w
+        # self.rect.h = self.layout.rect.h
+        # print 'document',_max_w,self.layout.rect.h
+        return _max_w, self.layout.rect.h
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/basic.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/basic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,107 @@
 """These widgets are all grouped together because they are non-interactive widgets.
 """
 
 import pygame
 
-from const import *
-import widget
+from .const import *
+from . import widget
+
 
 class Spacer(widget.Widget):
     """A invisible space.
-    
+
     <pre>Spacer(width,height)</pre>
-    
+
     """
-    def __init__(self,width,height,**params):
-        params.setdefault('focusable',False)
-        widget.Widget.__init__(self,width=width,height=height,**params)
-        
+
+    def __init__(self, width, height, **params):
+        params.setdefault("focusable", False)
+        widget.Widget.__init__(self, width=width, height=height, **params)
+
 
 class Color(widget.Widget):
     """A block of color.
-    
+
     <p>The color can be changed at run-time.</p>
-    
+
     <pre>Color(value=None)</pre>
-    
+
     <strong>Example</strong>
     <code>
     c = Color()
     c.value = (255,0,0)
     c.value = (0,255,0)
     </code>
     """
-    
-    
-    def __init__(self,value=None,**params):
-        params.setdefault('focusable',False)
-        if value != None: params['value']=value
-        widget.Widget.__init__(self,**params)
-    
-    def paint(self,s):
-        if hasattr(self,'value'): s.fill(self.value)
-    
-    def __setattr__(self,k,v):
-        if k == 'value' and type(v) == str: v = pygame.Color(v)
-        _v = self.__dict__.get(k,NOATTR)
-        self.__dict__[k]=v
-        if k == 'value' and _v != NOATTR and _v != v: 
+
+    def __init__(self, value=None, **params):
+        params.setdefault("focusable", False)
+        if value != None:
+            params["value"] = value
+        widget.Widget.__init__(self, **params)
+
+    def paint(self, s):
+        if hasattr(self, "value"):
+            s.fill(self.value)
+
+    def __setattr__(self, k, v):
+        if k == "value" and type(v) == str:
+            v = pygame.Color(v)
+        _v = self.__dict__.get(k, NOATTR)
+        self.__dict__[k] = v
+        if k == "value" and _v != NOATTR and _v != v:
             self.send(CHANGE)
             self.repaint()
 
+
 class Label(widget.Widget):
     """A text label.
-    
+
     <pre>Label(value)</pre>
-    
+
     <dl>
     <dt>value<dd>text to be displayed
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     w = Label(value="I own a rubber chicken!")
-    
+
     w = Label("3 rubber chickens")
     </code>
     """
-    def __init__(self,value,**params):
-        params.setdefault('focusable',False)
-        params.setdefault('cls','label')
-        widget.Widget.__init__(self,**params)
+
+    def __init__(self, value, **params):
+        params.setdefault("focusable", False)
+        params.setdefault("cls", "label")
+        widget.Widget.__init__(self, **params)
         self.value = value
         self.font = self.style.font
         self.style.width, self.style.height = self.font.size(self.value)
-    
-    def paint(self,s):
-        s.blit(self.font.render(self.value, 1, self.style.color),(0,0))
+
+    def paint(self, s):
+        s.blit(self.font.render(self.value, 1, self.style.color), (0, 0))
+
 
 class Image(widget.Widget):
     """An image.
-    
+
     <pre>Image(value)</pre>
-    
+
     <dl>
     <dt>value<dd>a file name or a pygame.Surface
     </dl>
-    
+
     """
-    def __init__(self,value,**params):
-        params.setdefault('focusable',False)
-        widget.Widget.__init__(self,**params)
-        if type(value) == str: value = pygame.image.load(value)
+
+    def __init__(self, value, **params):
+        params.setdefault("focusable", False)
+        widget.Widget.__init__(self, **params)
+        if type(value) == str:
+            value = pygame.image.load(value)
         self.value = value
         self.style.width = self.value.get_width()
         self.style.height = self.value.get_height()
-    
-    def paint(self,s):
-        s.blit(self.value,(0,0))
+
+    def paint(self, s):
+        s.blit(self.value, (0, 0))
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/select.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/select.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,176 +1,182 @@
 """
 """
-from const import *
-import table
-import basic, button
+from .const import *
+from . import table
+from . import basic, button
+
 
 class Select(table.Table):
     """A select input.
-    
+
     <pre>Select(value=None)</pre>
-    
+
     <dl>
     <dt>value<dd>initial value
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     w = Select(value="goats")
     w.add("Cats","cats")
     w.add("Goats","goats")
     w.add("Dogs","Dogs")
-    
+
     w.value = 'dogs' #changes the value from goats to dogs
     </code>
-    
+
     """
 
-    def __init__(self,value=None,**params):
-        params.setdefault('cls','select')
-        table.Table.__init__(self,**params)
-        
-        self.top_selected = button.Button(cls=self.cls+".selected")
-        table.Table.add(self,self.top_selected) #,hexpand=1,vexpand=1)#,0,0)
-        self.top_selected.value = basic.Label(" ",cls=self.cls+".option.label")
-        
-        self.top_arrow = button.Button(basic.Image(self.style.arrow),cls=self.cls+".arrow")
-        table.Table.add(self,self.top_arrow) #,hexpand=1,vexpand=1) #,1,0)
-        
-        self.options = table.Table() #style={'border':3})
-        
+    def __init__(self, value=None, **params):
+        params.setdefault("cls", "select")
+        table.Table.__init__(self, **params)
+
+        self.top_selected = button.Button(cls=self.cls + ".selected")
+        table.Table.add(self, self.top_selected)  # ,hexpand=1,vexpand=1)#,0,0)
+        self.top_selected.value = basic.Label(" ", cls=self.cls + ".option.label")
+
+        self.top_arrow = button.Button(
+            basic.Image(self.style.arrow), cls=self.cls + ".arrow"
+        )
+        table.Table.add(self, self.top_arrow)  # ,hexpand=1,vexpand=1) #,1,0)
+
+        self.options = table.Table()  # style={'border':3})
+
         self.options.tr()
-        self.spacer_top = basic.Spacer(0,0)
+        self.spacer_top = basic.Spacer(0, 0)
         self.options.add(self.spacer_top)
-        
+
         self.options.tr()
-        self._options = table.Table(cls=self.cls+".options")
+        self._options = table.Table(cls=self.cls + ".options")
         self.options.add(self._options)
-        
+
         self.options.tr()
-        self.spacer_bottom = basic.Spacer(0,0)
+        self.spacer_bottom = basic.Spacer(0, 0)
         self.options.add(self.spacer_bottom)
 
-        
-        self.options.connect(BLUR,self.options.close,None)
-        self.spacer_top.connect(CLICK,self.options.close,None)
-        self.spacer_bottom.connect(CLICK,self.options.close,None)
-        
+        self.options.connect(BLUR, self.options.close, None)
+        self.spacer_top.connect(CLICK, self.options.close, None)
+        self.spacer_bottom.connect(CLICK, self.options.close, None)
+
         self.values = []
         self.value = value
-    
-    def resize(self,width=None,height=None):
-        max_w,max_h = 0,0
+
+    def resize(self, width=None, height=None):
+        max_w, max_h = 0, 0
         for w in self._options.widgets:
-            w.rect.w,w.rect.h = w.resize()
-            max_w,max_h = max(max_w,w.rect.w),max(max_h,w.rect.h)
-        
-        #xt,xr,xb,xl = self.top_selected.getspacing()
-        self.top_selected.style.width = max_w #+ xl + xr
-        self.top_selected.style.height = max_h #+ xt + xb
-        
-        self.top_arrow.connect(CLICK,self._open,None)
-        self.top_selected.connect(CLICK,self._open,None)
-        
-        w,h = table.Table.resize(self,width,height)
-        
-        self.spacer_top.style.width, self.spacer_top.style.height = w,h
-        self.spacer_bottom.style.width, self.spacer_bottom.style.height = w,h
-        self._options.style.width = w - 2 #HACK, this depends on the theme, really...
-        #HACK: sort of, but not a big one..
+            w.rect.w, w.rect.h = w.resize()
+            max_w, max_h = max(max_w, w.rect.w), max(max_h, w.rect.h)
+
+        # xt,xr,xb,xl = self.top_selected.getspacing()
+        self.top_selected.style.width = max_w  # + xl + xr
+        self.top_selected.style.height = max_h  # + xt + xb
+
+        self.top_arrow.connect(CLICK, self._open, None)
+        self.top_selected.connect(CLICK, self._open, None)
+
+        w, h = table.Table.resize(self, width, height)
+
+        self.spacer_top.style.width, self.spacer_top.style.height = w, h
+        self.spacer_bottom.style.width, self.spacer_bottom.style.height = w, h
+        self._options.style.width = w - 2  # HACK, this depends on the theme, really...
+        # HACK: sort of, but not a big one..
         self._options.resize()
-        
-        return w,h
-        
-    def _open(self,value):
-        sh = self.rect.h #spacer height
+
+        return w, h
+
+    def _open(self, value):
+        sh = self.rect.h  # spacer height
         opts = self.options
-        
+
         self.spacer_top.style.height = 0
         self.spacer_bottom.style.height = 0
         opts.rect.w, opts.rect.h = opts.resize()
         h = opts.rect.h
-        
+
         y = self.rect.y
         c = self.container
-        while hasattr(c,'container'):
+        while hasattr(c, "container"):
             y += c.rect.y
-            if c.container == None: break
+            if c.container == None:
+                break
             c = c.container
-            
-        if y + sh + h <= c.rect.h: #down
+
+        if y + sh + h <= c.rect.h:  # down
             self.spacer_top.style.height = sh
             dy = self.rect.y
-        else: #up
+        else:  # up
             self.spacer_bottom.style.height = sh
             dy = self.rect.y - h
-            
+
         opts.rect.w, opts.rect.h = opts.resize()
-            
-        self.container.open(opts,self.rect.x,dy)
-    
-    def _setvalue(self,value):
+
+        self.container.open(opts, self.rect.x, dy)
+
+    def _setvalue(self, value):
         self.value = value._value
-        if hasattr(self,'container'):
-            #self.chsize()
-            #HACK: improper use of resize()
-            #self.resize() #to recenter the new value, etc.
+        if hasattr(self, "container"):
+            # self.chsize()
+            # HACK: improper use of resize()
+            # self.resize() #to recenter the new value, etc.
             pass
         #    #self._resize()
-        
+
         self.options.close()
-        self.repaint() #this will happen anyways
-    
-    def __setattr__(self,k,v):
+        self.repaint()  # this will happen anyways
+
+    def __setattr__(self, k, v):
         mywidget = None
-        if k == 'value':
+        if k == "value":
             for w in self.values:
                 if w._value == v:
                     mywidget = w
-        _v = self.__dict__.get(k,NOATTR)
-        self.__dict__[k]=v
-        if k == 'value' and _v != NOATTR and _v != v: 
+        _v = self.__dict__.get(k, NOATTR)
+        self.__dict__[k] = v
+        if k == "value" and _v != NOATTR and _v != v:
             self.send(CHANGE)
             self.repaint()
-        if k == 'value':
+        if k == "value":
             if not mywidget:
-                mywidget = basic.Label(" ",cls=self.cls+".option.label")
+                mywidget = basic.Label(" ", cls=self.cls + ".option.label")
             self.top_selected.value = mywidget
-    
-    def add(self,w,value=None):
+
+    def add(self, w, value=None):
         """Add a widget, value item to the Select.
-        
+
         <pre>Select.add(widget,value=None)</pre>
-        
+
         <dl>
         <dt>widget<dd>Widget or string to represent the item
         <dt>value<dd>value for this item
         </dl>
-        
+
         <strong>Example</strong>
         <code>
         w = Select()
         w.add("Goat") #adds a Label
         w.add("Goat","goat") #adds a Label with the value goat
         w.add(gui.Label("Cuzco"),"goat") #adds a Label with value goat
         </code>
         """
-        
-        if type(w) == str: w = basic.Label(w,cls=self.cls+".option.label")
-        
+
+        if type(w) == str:
+            w = basic.Label(w, cls=self.cls + ".option.label")
+
         w.style.align = -1
-        b = button.Button(w,cls=self.cls+".option")
-        b.connect(CLICK,self._setvalue,w)
-        #b = w
-        #w.cls = self.cls+".option"
-        #w.cls = self.cls+".option"
-        
+        b = button.Button(w, cls=self.cls + ".option")
+        b.connect(CLICK, self._setvalue, w)
+        # b = w
+        # w.cls = self.cls+".option"
+        # w.cls = self.cls+".option"
+
         self._options.tr()
-        self._options.add(b) #,align=-1)
-        #self._options.td(b, align=-1, cls=self.cls+".option")
-        #self._options.td(_List_Item(w,value=value),align=-1)
-        
-        if value != None: w._value = value
-        else: w._value = w
+        self._options.add(b)  # ,align=-1)
+        # self._options.td(b, align=-1, cls=self.cls+".option")
+        # self._options.td(_List_Item(w,value=value),align=-1)
+
+        if value != None:
+            w._value = value
+        else:
+            w._value = w
         if self.value == w._value:
             self.top_selected.value = w
         self.values.append(w)
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/button.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/button.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,323 +1,347 @@
 """
 """
 
 from pygame.locals import *
 
-from const import *
-import widget, surface
-import basic
+from .const import *
+from . import widget, surface
+from . import basic
+
 
 class _button(widget.Widget):
-    def __init__(self,**params):
-        widget.Widget.__init__(self,**params)
+    def __init__(self, **params):
+        widget.Widget.__init__(self, **params)
         self.state = 0
-    
-    def event(self,e):
-        if e.type == ENTER: self.repaint()
-        elif e.type == EXIT: self.repaint()
-        elif e.type == FOCUS: self.repaint()
-        elif e.type == BLUR: self.repaint()
+
+    def event(self, e):
+        if e.type == ENTER:
+            self.repaint()
+        elif e.type == EXIT:
+            self.repaint()
+        elif e.type == FOCUS:
+            self.repaint()
+        elif e.type == BLUR:
+            self.repaint()
         elif e.type == KEYDOWN:
             if e.key == K_SPACE:
                 self.state = 1
                 self.repaint()
             elif e.key == K_TAB:
-                self.next()
-        elif e.type == MOUSEBUTTONDOWN: 
+                next(self)
+        elif e.type == MOUSEBUTTONDOWN:
             self.state = 1
             self.repaint()
         elif e.type == KEYUP:
-            if self.state == 1: 
-                sub = pygame.event.Event(CLICK,{})
-                self.send(sub.type,sub)
-            
+            if self.state == 1:
+                sub = pygame.event.Event(CLICK, {})
+                self.send(sub.type, sub)
+
             self.state = 0
             self.repaint()
         elif e.type == MOUSEBUTTONUP:
             self.state = 0
             self.repaint()
         elif e.type == CLICK:
             self.click()
-        
+
         self.pcls = ""
         if self.state == 0 and self.container.myhover is self:
             self.pcls = "hover"
         if self.state == 1 and self.container.myhover is self:
             self.pcls = "down"
-    
-    def click(self): 
+
+    def click(self):
         pass
 
 
 class Button(_button):
     """A button, buttons can be clicked, they are usually used to set up callbacks.
-    
+
     <pre>Button(value=None)</pre>
-    
+
     <dl>
     <dt>value<dd>either a widget or a string
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     w = gui.Button("Click Me")
     w.connect(gui.CLICK,fnc,value)
     </code>
     """
-    def __init__(self,value=None,**params):
-        params.setdefault('cls','button')
-        _button.__init__(self,**params)
+
+    def __init__(self, value=None, **params):
+        params.setdefault("cls", "button")
+        _button.__init__(self, **params)
         self.value = value
-    
-    def __setattr__(self,k,v):
-        if k == 'value' and type(v) == str: v = basic.Label(v,cls=self.cls+".label")
-        _v = self.__dict__.get(k,NOATTR)
-        self.__dict__[k]=v
-        if k == 'value' and v != None:
+
+    def __setattr__(self, k, v):
+        if k == "value" and type(v) == str:
+            v = basic.Label(v, cls=self.cls + ".label")
+        _v = self.__dict__.get(k, NOATTR)
+        self.__dict__[k] = v
+        if k == "value" and v != None:
             pass
-        
-        if k == 'value' and _v != NOATTR and _v != None and _v != v:
+
+        if k == "value" and _v != NOATTR and _v != None and _v != v:
             self.send(CHANGE)
             self.chsize()
-    
-    def resize(self,width=None,height=None):
-        self.value.rect.x,self.value.rect.y = 0,0
-        self.value.rect.w,self.value.rect.h = self.value.resize(width,height)
-        return self.value.rect.w,self.value.rect.h
-#         
-#         self.value._resize()
-#         self.rect.w,self.rect.h = self.value.rect_margin.w,self.value.rect_margin.h
-#         
-#         if self.style.width: self.rect.w = max(self.rect.w,self.style.width)
-#         if self.style.height: self.rect.w = max(self.rect.w,self.style.height)
-#         
-#         xt,xr,xb,xl = self.value.getspacing()
-#         
-#         self.value._resize(self.rect.w-(xl+xr),self.rect.h-(xt+xb))
-#     
-    def paint(self,s):
-        self.value.paint(surface.subsurface(s,self.value.rect))
+
+    def resize(self, width=None, height=None):
+        self.value.rect.x, self.value.rect.y = 0, 0
+        self.value.rect.w, self.value.rect.h = self.value.resize(width, height)
+        return self.value.rect.w, self.value.rect.h
+
+    #
+    #         self.value._resize()
+    #         self.rect.w,self.rect.h = self.value.rect_margin.w,self.value.rect_margin.h
+    #
+    #         if self.style.width: self.rect.w = max(self.rect.w,self.style.width)
+    #         if self.style.height: self.rect.w = max(self.rect.w,self.style.height)
+    #
+    #         xt,xr,xb,xl = self.value.getspacing()
+    #
+    #         self.value._resize(self.rect.w-(xl+xr),self.rect.h-(xt+xb))
+    #
+    def paint(self, s):
+        self.value.paint(surface.subsurface(s, self.value.rect))
+
 
 class Switch(_button):
     """A switch can have two states, True or False.
-    
+
     <pre>Switch(value=False)</pre>
-    
+
     <dl>
     <dt>value<dd>initial value, (True, False)
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     w = gui.Switch(True)
     w.connect(gui.CHANGE,fnc,value)
     </code>
     """
-    def __init__(self,value=False,**params):
-        params.setdefault('cls','switch')
-        _button.__init__(self,**params)
+
+    def __init__(self, value=False, **params):
+        params.setdefault("cls", "switch")
+        _button.__init__(self, **params)
         self.value = value
-        
+
         img = self.style.off
         self.style.width = img.get_width()
         self.style.height = img.get_height()
-    
-    def paint(self,s):
-        #self.pcls = ""
-        #if self.container.myhover is self: self.pcls = "hover"
-        if self.value: img = self.style.on
-        else: img = self.style.off
-        s.blit(img,(0,0))
-    
-    def __setattr__(self,k,v):
-        _v = self.__dict__.get(k,NOATTR)
-        self.__dict__[k]=v
-        if k == 'value' and _v != NOATTR and _v != v: 
+
+    def paint(self, s):
+        # self.pcls = ""
+        # if self.container.myhover is self: self.pcls = "hover"
+        if self.value:
+            img = self.style.on
+        else:
+            img = self.style.off
+        s.blit(img, (0, 0))
+
+    def __setattr__(self, k, v):
+        _v = self.__dict__.get(k, NOATTR)
+        self.__dict__[k] = v
+        if k == "value" and _v != NOATTR and _v != v:
             self.send(CHANGE)
             self.repaint()
-    
+
     def click(self):
         self.value = not self.value
 
-class Checkbox(_button):    
+
+class Checkbox(_button):
     """Within a Group of Checkbox widgets several may be selected at a time.
-    
+
     <pre>Checkbox(group,value=None)</pre>
-    
+
     <dl>
     <dt>group<dd>a gui.Group for the Checkbox to belong to
     <dt>value<dd>the value
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     g = gui.Group(name='colors',value=['r','b'])
-    
+
     t = gui.Table()
     t.tr()
     t.td(gui.Label('Red'))
     t.td(gui.Checkbox(g,'r'))
     t.tr()
     t.td(gui.Label('Green'))
     t.td(gui.Checkbox(g,'g'))
     t.tr()
     t.td(gui.Label('Blue'))
     t.td(gui.Checkbox(g,'b'))
     </code>
     """
-    
-    def __init__(self,group,value=None,**params):
-        params.setdefault('cls','checkbox')
-        _button.__init__(self,**params)
+
+    def __init__(self, group, value=None, **params):
+        params.setdefault("cls", "checkbox")
+        _button.__init__(self, **params)
         self.group = group
         self.group.add(self)
         if self.group.value == None:
             self.group.value = []
         self.value = value
-        
+
         img = self.style.off
         self.style.width = img.get_width()
         self.style.height = img.get_height()
-    
-    def paint(self,s):
-        #self.pcls = ""
-        #if self.container.myhover is self: self.pcls = "hover"
-        if self.value in self.group.value: img = self.style.on
-        else: img = self.style.off
-        
-        s.blit(img,(0,0))
-    
+
+    def paint(self, s):
+        # self.pcls = ""
+        # if self.container.myhover is self: self.pcls = "hover"
+        if self.value in self.group.value:
+            img = self.style.on
+        else:
+            img = self.style.off
+
+        s.blit(img, (0, 0))
+
     def click(self):
         if self.value in self.group.value:
             self.group.value.remove(self.value)
         else:
             self.group.value.append(self.value)
         self.group._change()
 
+
 class Radio(_button):
     """Within a Group of Radio widgets only one may be selected at a time.
-    
+
     <pre>Radio(group,value=None)</pre>
-    
+
     <dl>
     <dt>group<dd>a gui.Group for the Radio to belong to
     <dt>value<dd>the value
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     g = gui.Group(name='colors',value='g')
-    
+
     t = gui.Table()
     t.tr()
     t.td(gui.Label('Red'))
     t.td(gui.Radio(g,'r'))
     t.tr()
     t.td(gui.Label('Green'))
     t.td(gui.Radio(g,'g'))
     t.tr()
     t.td(gui.Label('Blue'))
     t.td(gui.Radio(g,'b'))
     </code>
     """
-    
-    
-    def __init__(self,group=None,value=None,**params):
-        params.setdefault('cls','radio')
-        _button.__init__(self,**params)
+
+    def __init__(self, group=None, value=None, **params):
+        params.setdefault("cls", "radio")
+        _button.__init__(self, **params)
         self.group = group
         self.group.add(self)
         self.value = value
-        
+
         img = self.style.off
         self.style.width = img.get_width()
         self.style.height = img.get_height()
-    
-    def paint(self,s):
-        #self.pcls = ""
-        #if self.container.myhover is self: self.pcls = "hover"
-        if self.group.value == self.value: img = self.style.on
-        else: img = self.style.off
-        s.blit(img,(0,0))
-    
+
+    def paint(self, s):
+        # self.pcls = ""
+        # if self.container.myhover is self: self.pcls = "hover"
+        if self.group.value == self.value:
+            img = self.style.on
+        else:
+            img = self.style.off
+        s.blit(img, (0, 0))
+
     def click(self):
         self.group.value = self.value
 
+
 class Tool(_button):
     """Within a Group of Tool widgets only one may be selected at a time.
-    
+
     <pre>Tool(group,widget=None,value=None)</pre>
-    
+
     <dl>
     <dt>group<dd>a gui.Group for the Tool to belong to
     <dt>widget<dd>a widget to appear on the Tool (similar to a Button)
     <dt>value<dd>the value
     </dl>
-    
+
     <strong>Example</strong>
     <code>
     g = gui.Group(name='colors',value='g')
-    
+
     t = gui.Table()
     t.tr()
     t.td(gui.Tool(g,'Red','r'))
     t.tr()
     t.td(gui.Tool(g,'Green','g'))
     t.tr()
     t.td(gui.Tool(g,'Blue','b'))
     </code>
     """
 
-    def __init__(self,group,widget=None,value=None,**params): #TODO widget= could conflict with module widget
-        params.setdefault('cls','tool')
-        _button.__init__(self,**params)
+    def __init__(
+        self, group, widget=None, value=None, **params
+    ):  # TODO widget= could conflict with module widget
+        params.setdefault("cls", "tool")
+        _button.__init__(self, **params)
         self.group = group
         self.group.add(self)
         self.value = value
-        
+
         if widget:
             self.setwidget(widget)
-        
-        if self.group.value == self.value: self.pcls = "down"
-    
-    def setwidget(self,w):
+
+        if self.group.value == self.value:
+            self.pcls = "down"
+
+    def setwidget(self, w):
         self.widget = w
-    
-    def resize(self,width=None,height=None):
-        self.widget.rect.w,self.widget.rect.h = self.widget.resize()
-        #self.widget._resize()
-        #self.rect.w,self.rect.h = self.widget.rect_margin.w,self.widget.rect_margin.h
-        
-        return self.widget.rect.w,self.widget.rect.h
-    
-    def event(self,e):
-        _button.event(self,e)
-        if self.group.value == self.value: self.pcls = "down"
-    
-    def paint(self,s):
-        if self.group.value == self.value: self.pcls = "down"
-        self.widget.paint(surface.subsurface(s,self.widget.rect))
-    
+
+    def resize(self, width=None, height=None):
+        self.widget.rect.w, self.widget.rect.h = self.widget.resize()
+        # self.widget._resize()
+        # self.rect.w,self.rect.h = self.widget.rect_margin.w,self.widget.rect_margin.h
+
+        return self.widget.rect.w, self.widget.rect.h
+
+    def event(self, e):
+        _button.event(self, e)
+        if self.group.value == self.value:
+            self.pcls = "down"
+
+    def paint(self, s):
+        if self.group.value == self.value:
+            self.pcls = "down"
+        self.widget.paint(surface.subsurface(s, self.widget.rect))
+
     def click(self):
         self.group.value = self.value
         for w in self.group.widgets:
-            if w != self: w.pcls = ""
+            if w != self:
+                w.pcls = ""
+
 
-            
 class Icon(_button):
-    """TODO - might be deprecated
-    """
-    def __init__(self,cls,**params):
-        _button.__init__(self,**params)
+    """TODO - might be deprecated"""
+
+    def __init__(self, cls, **params):
+        _button.__init__(self, **params)
         self.cls = cls
-        self.pcls = ""        
+        self.pcls = ""
         s = self.style.image
         self.style.width = s.get_width()
         self.style.height = s.get_height()
         self.state = 0
-    
-    def paint(self,s):
-        #self.pcls = ""
-        #if self.state == 0 and hasattr(self.container,'myhover') and self.container.myhover is self: self.pcls = "hover"
-        #if self.state == 1 and hasattr(self.container,'myhover') and self.container.myhover is self: self.pcls = "down"
-        s.blit(self.style.image,(0,0))
+
+    def paint(self, s):
+        # self.pcls = ""
+        # if self.state == 0 and hasattr(self.container,'myhover') and self.container.myhover is self: self.pcls = "hover"
+        # if self.state == 1 and hasattr(self.container,'myhover') and self.container.myhover is self: self.pcls = "down"
+        s.blit(self.style.image, (0, 0))
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/widget.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,305 +1,348 @@
 """
 """
 import pygame
 
-import style
+from . import style
+
 
 class Widget:
     """Template object - base for all widgets.
-    
+
     <pre>Widget(**params)</pre>
-    
+
     <p>A number of optional params may be passed to the Widget initializer.</p>
-    
+
     <dl>
     <dt>decorate<dd>defaults to True.  If true, will call <tt>theme.decorate(self)</tt> to allow the theme a chance to decorate the widget.
     <dt>style<dd>a dict of style parameters.
     <dt>x, y, width, height<dd>position and size parameters, passed along to style
     <dt>align, valign<dd>alignment parameters, passed along to style
     <dt>font, color, background<dd>other common parameters that are passed along to style
     <dt>cls<dd>class name as used by Theme
     <dt>name<dd>name of widget as used by Form.  If set, will call <tt>form.add(self,name)</tt> to add the widget to the most recently created Form.
     <dt>focusable<dd>True if this widget can receive focus.  Defaults to True.
     <dt>disabled<dd>True of this widget is disabled.  Defaults to False.
     <dt>value<dd>initial value
     </dl>
-    
+
     <strong>Example - Creating your own Widget</strong>
     <p>This example shows which methods are template methods.</p>
     <code>
     class Draw(gui.Widget):
         def paint(self,s):
             #paint the pygame.Surface
             return
-        
+
         def update(self,s):
             #update the pygame.Surface and return the update rects
             return [pygame.Rect(0,0,self.rect.w,self.rect.h)]
-            
+
         def event(self,e):
             #handle the pygame.Event
             return
-            
+
         def resize(self,width=None,height=None):
             #return the width and height of this widget
             return 256,256
     </code>
     """
-    
-    def __init__(self,**params): 
-        #object.Object.__init__(self) 
+
+    def __init__(self, **params):
+        # object.Object.__init__(self)
         self.connects = {}
-        params.setdefault('decorate',True)
-        params.setdefault('style',{})
-        params.setdefault('focusable',True)
-        params.setdefault('disabled',False)
-        
-        self.focusable = params['focusable']
-        self.disabled = params['disabled']
-        
-        self.rect = pygame.Rect(params.get('x',0),params.get('y',0),params.get('width',0),params.get('height',0))
-        
-        s = params['style']
-        #some of this is a bit "theme-ish" but it is very handy, so these
-        #things don't have to be put directly into the style.
-        for att in ('align','valign','x','y','width','height','color','font','background'):
-            if att in params: s[att] = params[att]
-        self.style = style.Style(self,s)
-        
-        self.cls = 'default'
-        if 'cls' in params: self.cls = params['cls']
-        if 'name' in params:    
-            import form
-            self.name = params['name']
-            if hasattr(form.Form,'form') and form.Form.form != None: 
+        params.setdefault("decorate", True)
+        params.setdefault("style", {})
+        params.setdefault("focusable", True)
+        params.setdefault("disabled", False)
+
+        self.focusable = params["focusable"]
+        self.disabled = params["disabled"]
+
+        self.rect = pygame.Rect(
+            params.get("x", 0),
+            params.get("y", 0),
+            params.get("width", 0),
+            params.get("height", 0),
+        )
+
+        s = params["style"]
+        # some of this is a bit "theme-ish" but it is very handy, so these
+        # things don't have to be put directly into the style.
+        for att in (
+            "align",
+            "valign",
+            "x",
+            "y",
+            "width",
+            "height",
+            "color",
+            "font",
+            "background",
+        ):
+            if att in params:
+                s[att] = params[att]
+        self.style = style.Style(self, s)
+
+        self.cls = "default"
+        if "cls" in params:
+            self.cls = params["cls"]
+        if "name" in params:
+            from . import form
+
+            self.name = params["name"]
+            if hasattr(form.Form, "form") and form.Form.form != None:
                 form.Form.form.add(self)
                 self.form = form.Form.form
-        if 'value' in params: self.value = params['value']
+        if "value" in params:
+            self.value = params["value"]
         self.pcls = ""
-        
-        if params['decorate'] != False:
-            import app
-            if not hasattr(app.App,'app'):
-                print 'gui.widget: creating an App'
+
+        if params["decorate"] != False:
+            from . import app
+
+            if not hasattr(app.App, "app"):
+                print("gui.widget: creating an App")
                 app.App.app = app.App()
-            app.App.app.theme.decorate(self,params['decorate'])
-    
+            app.App.app.theme.decorate(self, params["decorate"])
+
     def focus(self):
         """Focus this Widget.
-        
+
         <pre>Widget.focus()</pre>
         """
-        if getattr(self,'container',None) != None: 
+        if getattr(self, "container", None) != None:
             if self.container.myfocus != self:  ## by Gal Koren
                 self.container.focus(self)
-    def blur(self): 
+
+    def blur(self):
         """Blur this Widget.
-        
+
         <pre>Widget.blur()</pre>
         """
-        if getattr(self,'container',None) != None: self.container.blur(self)
+        if getattr(self, "container", None) != None:
+            self.container.blur(self)
+
     def open(self):
         """Open this Widget as a modal dialog.
-        
+
         <pre>Widget.open()</pre>
         """
-        if getattr(self,'container',None) != None: self.container.open(self)
-    def close(self): 
+        if getattr(self, "container", None) != None:
+            self.container.open(self)
+
+    def close(self):
         """Close this Widget (if it is a modal dialog.)
-        
+
         <pre>Widget.close()</pre>
         """
-        if getattr(self,'container',None) != None: self.container.close(self)
-    def resize(self,width=None,height=None):
+        if getattr(self, "container", None) != None:
+            self.container.close(self)
+
+    def resize(self, width=None, height=None):
         """Template method - return the size and width of this widget.
 
         <p>Responsible for also resizing all sub-widgets.</p>
-                
+
         <pre>Widget.resize(width,height): return width,height</pre>
-        
+
         <dl>
         <dt>width<dd>suggested width
         <dt>height<dd>suggested height
         </dl>
-        
+
         <p>If not overridden, will return self.style.width, self.style.height</p>
         """
         return self.style.width, self.style.height
+
     def chsize(self):
         """Change the size of this widget.
-        
+
         <p>Calling this method will cause a resize on all the widgets,
         including this one.</p>
-        
+
         <pre>Widget.chsize()</pre>
         """
-        if not hasattr(self,'container'): return
-        import app
-        if hasattr(app.App,'app'):
-            if app.App.app._chsize: return
+        if not hasattr(self, "container"):
+            return
+        from . import app
+
+        if hasattr(app.App, "app"):
+            if app.App.app._chsize:
+                return
             app.App.app.chsize()
             return
-            
-        #if hasattr(app.App,'app'):
+
+        # if hasattr(app.App,'app'):
         #    w,h = self.rect.w,self.rect.h
         #    w2,h2 = self.resize()
         #    if w2 != w or h2 != h:
         #        app.App.app.chsize()
-        #    else: 
+        #    else:
         #        self.repaint()
-        
 
-    def update(self,s):
+    def update(self, s):
         """Template method - update the surface
-        
+
         <pre>Widget.update(s): return list of pygame.Rect(s)</pre>
-        
+
         <dl>
         <dt>s<dd>pygame.Surface to update
         </dl>
-        
+
         <p>return - a list of the updated areas as pygame.Rect(s).</p>
         """
         return
-        
-    def paint(self,s):
+
+    def paint(self, s):
         """Template method - paint the surface
-        
+
         <pre>Widget.paint(s)</pre>
-        
+
         <dl>
         <dt>s<dd>pygame.Surface to paint
         </dl>
         """
         return
 
-    def repaint(self): 
+    def repaint(self):
         """Request a repaint of this Widget.
-        
+
         <pre>Widget.repaint()</pre>
         """
-        if getattr(self,'container',None) != None: self.container.repaint(self)
+        if getattr(self, "container", None) != None:
+            self.container.repaint(self)
+
     def repaintall(self):
         """Request a repaint of all Widgets.
-        
+
         <pre>Widget.repaintall()</pre>
         """
-        if getattr(self,'container',None) != None: self.container.repaintall()
-    def reupdate(self): 
+        if getattr(self, "container", None) != None:
+            self.container.repaintall()
+
+    def reupdate(self):
         """Request a reupdate of this Widget
-        
+
         <pre>Widget.reupdate()</pre>
         """
-        if getattr(self,'container',None) != None: self.container.reupdate(self)
-    def next(self): 
+        if getattr(self, "container", None) != None:
+            self.container.reupdate(self)
+
+    def __next__(self):
         """Pass focus to next Widget.
-        
+
         <p>Widget order determined by the order they were added to their container.</p>
-        
+
         <pre>Widget.next()</pre>
         """
-        if getattr(self,'container',None) != None: self.container.next(self)
-    def previous(self): 
+        if getattr(self, "container", None) != None:
+            self.container.next(self)
+
+    def previous(self):
         """Pass focus to previous Widget.
-        
+
         <p>Widget order determined by the order they were added to their container.</p>
-        
+
         <pre>Widget.previous()</pre>
         """
-        
-        if getattr(self,'container',None) != None: self.container.previous(self)
-    
+
+        if getattr(self, "container", None) != None:
+            self.container.previous(self)
+
     def get_abs_rect(self):
         """Get the absolute rect of this widget on the App screen
-        
+
         <pre>Widget.get_abs_rect(): return pygame.Rect</pre>
         """
         x, y = self.rect[:2]
-        c = getattr(self,'container',None)
+        c = getattr(self, "container", None)
         while c:
             x += c.rect[0]
             y += c.rect[1]
-            c = getattr(c,'container',None)
+            c = getattr(c, "container", None)
         return pygame.Rect(x, y, self.rect.w, self.rect.h)
 
-    def connect(self,code,fnc,*values):
+    def connect(self, code, fnc, *values):
         """Connect a event code to a callback function.
-        
+
         <p>There may only be one callback per event code.</p>
-        
+
         <pre>Object.connect(code,fnc,value)</pre>
-        
+
         <dl>
         <dt>code<dd>event type [[gui-const]]
         <dt>fnc<dd>callback function
         <dt>*values<dd>values to pass to callback.  Please note that callbacks may also have "magicaly" parameters.  Such as:
             <dl>
             <dt>_event<dd>receive the event
             <dt>_code<dd>receive the event code
             <dt>_widget<dd>receive the sending widget
             </dl>
         </dl>
-        
+
         <strong>Example</strong>
         <code>
         def onclick(value):
             print 'click',value
-        
+
         w = Button("PGU!")
         w.connect(gui.CLICK,onclick,'PGU Button Clicked')
         </code>
         """
-        
-        self.connects[code] = {'fnc':fnc,'values':values}
-    
-    def send(self,code,event=None):
+
+        self.connects[code] = {"fnc": fnc, "values": values}
+
+    def send(self, code, event=None):
         """Send a code, event callback trigger.
-        
+
         <pre>Object.send(code,event=None)</pre>
-        
+
         <dl>
         <dt>code<dd>event code
         <dt>event<dd>event
         </dl>
         """
         if code in self.connects:
             con = self.connects[code]
-            #con['fnc'](*con['values'])
-        
-            fnc = con['fnc']
-            values = list(con['values'])
-            
-            nargs = fnc.func_code.co_argcount
-            names = list(fnc.func_code.co_varnames)[:nargs]
-            if hasattr(fnc,'im_class'): names.pop(0)
-            
+            # con['fnc'](*con['values'])
+
+            fnc = con["fnc"]
+            values = list(con["values"])
+
+            nargs = fnc.__code__.co_argcount
+            names = list(fnc.__code__.co_varnames)[:nargs]
+            if hasattr(fnc, "im_class"):
+                names.pop(0)
+
             args = []
-            magic = {'_event':event,'_code':code,'_widget':self}
+            magic = {"_event": event, "_code": code, "_widget": self}
             for name in names:
-                if name in magic.keys():
+                if name in list(magic.keys()):
                     args.append(magic[name])
                 elif len(values):
                     args.append(values.pop(0))
                 else:
                     break
             args.extend(values)
             fnc(*args)
-    
-    def _event(self,e):
-        if self.disabled: return
-        self.send(e.type,e)
+
+    def _event(self, e):
+        if self.disabled:
+            return
+        self.send(e.type, e)
         self.event(e)
         return
-        import app
-        if hasattr(app.App,'app'):
-            app.App.app.events.append((self,e))
-        
-    def event(self,e):
+        from . import app
+
+        if hasattr(app.App, "app"):
+            app.App.app.events.append((self, e))
+
+    def event(self, e):
         """Template method - called when an event is passed to this object.
-        
+
         <dl>
         <dt>e<dd>event
         </dl>
         """
-        
+
         return
```

### Comparing `zanthor-1.2.3/zanthor/pgu/gui/const.py` & `zanthor-1.2.4a2/zanthor/pgu/gui/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,29 @@
 <strong>Other</strong>
 <dl>
 <dt>NOATTR
 </dl>
 """
 import pygame
 
-from pygame.locals import QUIT, MOUSEBUTTONDOWN, MOUSEBUTTONUP, MOUSEMOTION, KEYDOWN, USEREVENT
+from pygame.locals import (
+    QUIT,
+    MOUSEBUTTONDOWN,
+    MOUSEBUTTONUP,
+    MOUSEMOTION,
+    KEYDOWN,
+    USEREVENT,
+)
+
 ENTER = pygame.locals.USEREVENT + 0
 EXIT = pygame.locals.USEREVENT + 1
 BLUR = pygame.locals.USEREVENT + 2
 FOCUS = pygame.locals.USEREVENT + 3
 CLICK = pygame.locals.USEREVENT + 4
 CHANGE = pygame.locals.USEREVENT + 5
 OPEN = pygame.locals.USEREVENT + 6
 CLOSE = pygame.locals.USEREVENT + 7
-INIT = 'init'
+INIT = "init"
+
 
-class NOATTR: pass
+class NOATTR:
+    pass
```

### Comparing `zanthor-1.2.3/zanthor/pgu/algo.py` & `zanthor-1.2.4a2/zanthor/pgu/algo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,135 +1,162 @@
 """Some handy algorithms for use in games, etc.
 
 <p>please note that this file is alpha, and is subject to modification in
 future versions of pgu!</p>
 """
-print 'pgu.algo','This module is alpha, and is subject to change.'
+print("pgu.algo", "This module is alpha, and is subject to change.")
 
-#def dist(a,b):
+# def dist(a,b):
 #    return abs(a[0]-b[0]) + abs(a[1]-b[1])
-    
+
+
 class node:
-    def __init__(self,prev,pos,dest):
-        self.prev,self.pos,self.dest = prev,pos,dest
-        if self.prev == None: self.g = 0
-        else: self.g = self.prev.g + 1
-        self.h = dist(pos,dest)
-        self.f = self.g+self.h
+    def __init__(self, prev, pos, dest):
+        self.prev, self.pos, self.dest = prev, pos, dest
+        if self.prev == None:
+            self.g = 0
+        else:
+            self.g = self.prev.g + 1
+        self.h = dist(pos, dest)
+        self.f = self.g + self.h
 
 
-def astar(start,end,layer,_dist):
+def astar(start, end, layer, _dist):
     """uses the a* algorithm to find a path
-    
+
     <pre>astar(start,end,layer,dist): return [list of positions]</pre>
-    
+
     <dl>
     <dt>start<dd>start position
     <dt>end<dd>end position
     <dt>layer<dd>a grid where zero cells are open and non-zero cells are walls
     <dt>dist<dd>a distance function dist(a,b)
     </dl>
-    
+
     <p>returns a list of positions from start to end</p>
     """
     global dist
     dist = _dist
-    if layer[start[1]][start[0]]: return [] #start is blocked
-    if layer[end[1]][end[0]]: return [] #end is blocked
-    w,h = len(layer[0]),len(layer)
-    if start[0] < 0 or start[1] < 0 or start[0] >= w or start[1] >= h: return [] #start outside of layer
-    if end[0] < 0 or end[1] < 0 or end[0] >= w or end[1] >= h: return [] #end outside of layer
+    if layer[start[1]][start[0]]:
+        return []  # start is blocked
+    if layer[end[1]][end[0]]:
+        return []  # end is blocked
+    w, h = len(layer[0]), len(layer)
+    if start[0] < 0 or start[1] < 0 or start[0] >= w or start[1] >= h:
+        return []  # start outside of layer
+    if end[0] < 0 or end[1] < 0 or end[0] >= w or end[1] >= h:
+        return []  # end outside of layer
 
     opens = []
     open = {}
     closed = {}
-    cur = node(None,start,end)
+    cur = node(None, start, end)
     open[cur.pos] = cur
     opens.append(cur)
     while len(open):
         cur = opens.pop(0)
-        if cur.pos not in open: continue
+        if cur.pos not in open:
+            continue
         del open[cur.pos]
         closed[cur.pos] = cur
-        if cur.pos == end: break
-        for dx,dy in [(0,-1),(1,0),(0,1),(-1,0)]:#(-1,-1),(1,-1),(-1,1),(1,1)]:
-            x,y = pos = cur.pos[0]+dx,cur.pos[1]+dy
-            if layer[y][x]: continue
-            #check for blocks of diagonals
-            if layer[cur.pos[1]+dy][cur.pos[0]]: continue
-            if layer[cur.pos[1]][cur.pos[0]+dx]: continue
-            new = node(cur,pos,end)
-            if pos in open and new.f >= open[pos].f: continue
-            if pos in closed and new.f >= closed[pos].f: continue
-            if pos in open: del open[pos]
-            if pos in closed: del closed[pos]
+        if cur.pos == end:
+            break
+        for dx, dy in [
+            (0, -1),
+            (1, 0),
+            (0, 1),
+            (-1, 0),
+        ]:  # (-1,-1),(1,-1),(-1,1),(1,1)]:
+            x, y = pos = cur.pos[0] + dx, cur.pos[1] + dy
+            if layer[y][x]:
+                continue
+            # check for blocks of diagonals
+            if layer[cur.pos[1] + dy][cur.pos[0]]:
+                continue
+            if layer[cur.pos[1]][cur.pos[0] + dx]:
+                continue
+            new = node(cur, pos, end)
+            if pos in open and new.f >= open[pos].f:
+                continue
+            if pos in closed and new.f >= closed[pos].f:
+                continue
+            if pos in open:
+                del open[pos]
+            if pos in closed:
+                del closed[pos]
             open[pos] = new
             lo = 0
             hi = len(opens)
             while lo < hi:
-                mid = (lo+hi)/2
-                if new.f < opens[mid].f: hi = mid
-                else: lo = mid + 1
-            opens.insert(lo,new)
-    
-    if cur.pos != end: 
+                mid = (lo + hi) / 2
+                if new.f < opens[mid].f:
+                    hi = mid
+                else:
+                    lo = mid + 1
+            opens.insert(lo, new)
+
+    if cur.pos != end:
         return []
-                    
+
     path = []
     while cur.prev != None:
         path.append(cur.pos)
         cur = cur.prev
     path.reverse()
     return path
-    
 
-def getline(a,b):
+
+def getline(a, b):
     """returns a path of points from a to b
-    
+
     <pre>getline(a,b): return [list of points]</pre>
-    
+
     <dl>
     <dt>a<dd>starting point
     <dt>b<dd>ending point
     </dl>
-    
+
     <p>returns a list of points from a to b</p>
     """
-           
+
     path = []
-    
-    x1,y1 = a
-    x2,y2 = b
-    dx,dy = abs(x2-x1),abs(y2-y1)
-
-    if x2 >= x1: xi1,xi2 = 1,1
-    else: xi1,xi2 = -1,-1
-    
-    if y2 >= y1: yi1,yi2 = 1,1
-    else: yi1,yi2 = -1,-1
-    
+
+    x1, y1 = a
+    x2, y2 = b
+    dx, dy = abs(x2 - x1), abs(y2 - y1)
+
+    if x2 >= x1:
+        xi1, xi2 = 1, 1
+    else:
+        xi1, xi2 = -1, -1
+
+    if y2 >= y1:
+        yi1, yi2 = 1, 1
+    else:
+        yi1, yi2 = -1, -1
+
     if dx >= dy:
-        xi1,yi2 = 0,0
+        xi1, yi2 = 0, 0
         d = dx
-        n = dx/2
+        n = dx / 2
         a = dy
         p = dx
     else:
-        xi2,yi1 = 0,0
+        xi2, yi1 = 0, 0
         d = dy
-        n = dy/2
+        n = dy / 2
         a = dx
         p = dy
-        
-    x,y = x1,y1
+
+    x, y = x1, y1
     c = 0
     while c <= p:
-        path.append((x,y))
+        path.append((x, y))
         n += a
-        if n > d: 
+        if n > d:
             n -= d
             x += xi1
             y += yi1
         x += xi2
         y += yi2
         c += 1
     return path
```

### Comparing `zanthor-1.2.3/zanthor/pgu/timer.py` & `zanthor-1.2.4a2/zanthor/pgu/timer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 """A timer for games with set-rate FPS.
 """
 
 import pygame
 
+
 class Timer:
     """A timer for games with set-rate FPS.
-    
+
     <pre>Timer(fps)</pre>
     """
-    
-    def __init__(self,fps):
-        self.wait = 1000/fps
+
+    def __init__(self, fps):
+        self.wait = 1000 / fps
         self.nt = pygame.time.get_ticks()
-        
+
     def tick(self):
         """Wait correct amount of time each frame.  Call this once per frame.
-        
+
         <pre>Timer.tick()</pre>
         """
         self.ct = pygame.time.get_ticks()
         if self.ct < self.nt:
-            pygame.time.wait(self.nt-self.ct)
-            self.nt+=self.wait
-        else: 
-            self.nt = pygame.time.get_ticks()+self.wait
+            pygame.time.wait(self.nt - self.ct)
+            self.nt += self.wait
+        else:
+            self.nt = pygame.time.get_ticks() + self.wait
 
 
 class Speedometer:
     """A timer replacement that returns out FPS once a second.
     <pre>Speedometer()</pre>
-    
+
     <strong>Attributes</strong>
     <dl>
     <dt>fps <dd>always set to the current FPS
     </dl>
     """
+
     def __init__(self):
         self.frames = 0
         self.st = pygame.time.get_ticks()
         self.fps = 0
-        
+
     def tick(self):
-        """ Call this once per frame.
-        
+        """Call this once per frame.
+
         <pre>Speedometer.tick()</pre>
         """
         r = None
         self.frames += 1
         self.ct = pygame.time.get_ticks()
-        if (self.ct - self.st) >= 1000: 
+        if (self.ct - self.st) >= 1000:
             r = self.fps = self.frames
-            #print "%s: %d fps"%(self.__class__.__name__,self.fps)
+            # print "%s: %d fps"%(self.__class__.__name__,self.fps)
             self.frames = 0
             self.st += 1000
-        pygame.time.wait(0) #NOTE: not sure why, but you gotta call this now and again
+        pygame.time.wait(0)  # NOTE: not sure why, but you gotta call this now and again
         return r
 
-            
 
 # vim: set filetype=python sts=4 sw=4 noet si :
```

### Comparing `zanthor-1.2.3/zanthor/pgu/isovid.py` & `zanthor-1.2.4a2/zanthor/pgu/isovid.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,168 +4,176 @@
 particular needs.  If you are able to update it, help would be 
 greatly appreciated!</p>
 
 <p>please note that this file is alpha, and is subject to modification in
 future versions of pgu!</p>
 
 """
-print 'pgu.isovid','This module is alpha, and is subject to change.'
+print("pgu.isovid", "This module is alpha, and is subject to change.")
 
 from pgu.vid import *
 import pygame
 
+
 class Isovid(Vid):
     """Create an iso vid engine.  See [[vid]]"""
-    def update(self,screen):
+
+    def update(self, screen):
         return self.paint(screen)
-    
-    def paint(self,screen):
-        sw,sh = screen.get_width(),screen.get_height()
-        
+
+    def paint(self, screen):
+        sw, sh = screen.get_width(), screen.get_height()
+
         tlayer = self.tlayer
         blayer = self.blayer
         zlayer = self.zlayer
-        w,h = len(tlayer[0]),len(tlayer)
-        
-        iso_w,iso_h,iso_z,tile_w,tile_h,base_w,base_h = self.iso_w,self.iso_h,self.iso_z,self.tile_w,self.tile_h,self.base_w,self.base_h
-        
-        base_h2 = base_h/2
-        base_w2 = base_w/2
-        
-        bot = tile_h/base_h2
-        todo_max = sh/base_h2+bot
-        todo = [[] for y in xrange(0,todo_max)]
-        
-        self.view.w,self.view.h = sw,sh
+        w, h = len(tlayer[0]), len(tlayer)
+
+        iso_w, iso_h, iso_z, tile_w, tile_h, base_w, base_h = (
+            self.iso_w,
+            self.iso_h,
+            self.iso_z,
+            self.tile_w,
+            self.tile_h,
+            self.base_w,
+            self.base_h,
+        )
+
+        base_h2 = base_h / 2
+        base_w2 = base_w / 2
+
+        bot = tile_h / base_h2
+        todo_max = sh / base_h2 + bot
+        todo = [[] for y in range(0, todo_max)]
+
+        self.view.w, self.view.h = sw, sh
         view = self.view
-        adj = self.adj = pygame.Rect(-self.view.x,-self.view.y,0,0)
-        
+        adj = self.adj = pygame.Rect(-self.view.x, -self.view.y, 0, 0)
+
         for s in self.sprites:
             self.sprite_calc_irect(s)
-            x,y = self.iso_to_view((s.rect.centerx,s.rect.centery))
-            v = (y+adj.y)/base_h2 - 1
+            x, y = self.iso_to_view((s.rect.centerx, s.rect.centery))
+            v = (y + adj.y) / base_h2 - 1
             if v >= 0 and v < todo_max:
-                todo[v].append((s.image,s.irect))
-            #else: print 'doesnt fit',v
-                
-        w,h = len(tlayer[0]),len(tlayer)
+                todo[v].append((s.image, s.irect))
+            # else: print 'doesnt fit',v
+
+        w, h = len(tlayer[0]), len(tlayer)
         tiles = self.tiles
-        
-        #""
+
+        # ""
         if self.bounds == None:
-            tmp,y1 = self.tile_to_view((0,0))
-            x1,tmp = self.tile_to_view((0,h+1))
-            tmp,y2 = self.tile_to_view((w+1,h+1))
-            x2,tmp = self.tile_to_view((w+1,0))
-            self.bounds = pygame.Rect(x1,y1,x2-x1,y2-y1)
-        #""
-        
-        if self.bounds != None: self.view.clamp_ip(self.bounds)
-
-        ox,oy = self.screen_to_tile((0,0))
-        sx,sy = self.iso_to_view((ox*iso_w,oy*iso_h))
-        dx,dy = sx - self.view.x,sy - self.view.y
-        
-        for i2 in xrange(-bot,self.view.h/base_h2+bot):
-            tx,ty = ox + i2/2 + i2%2,oy + i2/2
-            x,y = (i2%2)*base_w2 + dx,i2*base_h2 + dy
-            
-            #to adjust for the -1 in i1
-            x,tx,ty = x-base_w,tx-1,ty+1
-            for i1 in xrange(-1,self.view.w/base_w+2): #NOTE: not sure why +2
+            tmp, y1 = self.tile_to_view((0, 0))
+            x1, tmp = self.tile_to_view((0, h + 1))
+            tmp, y2 = self.tile_to_view((w + 1, h + 1))
+            x2, tmp = self.tile_to_view((w + 1, 0))
+            self.bounds = pygame.Rect(x1, y1, x2 - x1, y2 - y1)
+        # ""
+
+        if self.bounds != None:
+            self.view.clamp_ip(self.bounds)
+
+        ox, oy = self.screen_to_tile((0, 0))
+        sx, sy = self.iso_to_view((ox * iso_w, oy * iso_h))
+        dx, dy = sx - self.view.x, sy - self.view.y
+
+        for i2 in range(-bot, self.view.h / base_h2 + bot):
+            tx, ty = ox + i2 / 2 + i2 % 2, oy + i2 / 2
+            x, y = (i2 % 2) * base_w2 + dx, i2 * base_h2 + dy
+
+            # to adjust for the -1 in i1
+            x, tx, ty = x - base_w, tx - 1, ty + 1
+            for i1 in range(-1, self.view.w / base_w + 2):  # NOTE: not sure why +2
                 if ty >= 0 and ty < h and tx >= 0 and tx < w:
-                    z = zlayer[ty][tx]*iso_z
+                    z = zlayer[ty][tx] * iso_z
                     if blayer != None:
                         n = blayer[ty][tx]
                         if n != 0:
                             t = tiles[n]
                             if t != None and t.image != None:
-                                screen.blit(t.image,(x-base_w2,y+z))
+                                screen.blit(t.image, (x - base_w2, y + z))
                     n = tlayer[ty][tx]
                     if n != 0:
                         t = tiles[n]
                         if t != None and t.image != None:
-                            screen.blit(t.image,(x-base_w2,y-(t.image_h-base_h)+z))
-            
+                            screen.blit(
+                                t.image, (x - base_w2, y - (t.image_h - base_h) + z)
+                            )
+
                 tx += 1
                 ty -= 1
                 x += base_w
-            for img,irect in todo[y/base_h2]:
-                screen.blit(img,(irect.x+adj.x,irect.y+adj.y))
+            for img, irect in todo[y / base_h2]:
+                screen.blit(img, (irect.x + adj.x, irect.y + adj.y))
+
+        return [pygame.Rect(0, 0, screen.get_width(), screen.get_height())]
 
-        return [pygame.Rect(0,0,screen.get_width(),screen.get_height())]
-        
-    def iso_to_view(self,pos):
+    def iso_to_view(self, pos):
         tlayer = self.tlayer
-        w,h = len(tlayer[0]),len(tlayer)
-        
-        x,y = pos
-        
-        #nx,ny = (h*self.iso_w + x - y)/2, (0 + x + y)/2
-        nx,ny = (x - y)/2, (0 + x + y)/2
-        
+        w, h = len(tlayer[0]), len(tlayer)
+
+        x, y = pos
+
+        # nx,ny = (h*self.iso_w + x - y)/2, (0 + x + y)/2
+        nx, ny = (x - y) / 2, (0 + x + y) / 2
+
         return (nx * self.base_w / self.iso_w), (ny * self.base_h / self.iso_h)
 
-    def view_to_iso(self,pos):
+    def view_to_iso(self, pos):
         tlayer = self.tlayer
-        w,h = len(tlayer[0]),len(tlayer)
-        
-        x,y = pos
-        
-        x,y = x*self.iso_w/self.base_w, y*self.iso_h/self.base_h
-        
-        #x -= (self.iso_w/2) * h
-        #x -= (self.iso_w/2) * h
-        
-        nx = (x+y) 
-        ny = y*2-nx
-    
-        return nx,ny
-    
-    def tile_to_view(self,pos):
-        return self.iso_to_view((pos[0]*self.iso_w,pos[1]*self.iso_h))
-    
-    def screen_to_tile(self,pos):
-        x,y = pos
+        w, h = len(tlayer[0]), len(tlayer)
+
+        x, y = pos
+
+        x, y = x * self.iso_w / self.base_w, y * self.iso_h / self.base_h
+
+        # x -= (self.iso_w/2) * h
+        # x -= (self.iso_w/2) * h
+
+        nx = x + y
+        ny = y * 2 - nx
+
+        return nx, ny
+
+    def tile_to_view(self, pos):
+        return self.iso_to_view((pos[0] * self.iso_w, pos[1] * self.iso_h))
+
+    def screen_to_tile(self, pos):
+        x, y = pos
         x += self.view.x
         y += self.view.y
-        x,y = self.view_to_iso((x,y))
-        return x/self.iso_w,y/self.iso_h
-        
-    def tile_to_screen(self,pos):
-        x,y = self.iso_to_view((pos[0]*self.iso_w,pos[1]*self.iso_h))
-        return x-self.view.x,y-self.view.y
-    
-    def tga_load_tiles(self,fname,size,tdata={}):
-        Vid.tga_load_tiles(self,fname,size,tdata)
-        
-        self.tile_w,self.tile_h = size
-        self.iso_w,self.iso_h,self.iso_z = self.tile_w,self.tile_w,1
-        self.base_w,self.base_h = self.tile_w,self.tile_w/2
-    
-
-        
-    def resize(self,size,bg=0):
-        Vid.resize(self,size,bg)
-        
-        tlayer = self.tlayer
-        w,h = len(tlayer[0]),len(tlayer)
-        
-        self.zlayer = [[0 for x in xrange(0,w)] for y in xrange(0,h)]
+        x, y = self.view_to_iso((x, y))
+        return x / self.iso_w, y / self.iso_h
+
+    def tile_to_screen(self, pos):
+        x, y = self.iso_to_view((pos[0] * self.iso_w, pos[1] * self.iso_h))
+        return x - self.view.x, y - self.view.y
+
+    def tga_load_tiles(self, fname, size, tdata={}):
+        Vid.tga_load_tiles(self, fname, size, tdata)
+
+        self.tile_w, self.tile_h = size
+        self.iso_w, self.iso_h, self.iso_z = self.tile_w, self.tile_w, 1
+        self.base_w, self.base_h = self.tile_w, self.tile_w / 2
 
-        
+    def resize(self, size, bg=0):
+        Vid.resize(self, size, bg)
+
+        tlayer = self.tlayer
+        w, h = len(tlayer[0]), len(tlayer)
 
+        self.zlayer = [[0 for x in range(0, w)] for y in range(0, h)]
 
-    def sprite_calc_irect(self,s):
+    def sprite_calc_irect(self, s):
         tlayer = self.tlayer
-        w,h = len(tlayer[0]),len(tlayer)
+        w, h = len(tlayer[0]), len(tlayer)
         zlayer = self.zlayer
-        
-        x,y = self.iso_to_view((s.rect.centerx,s.rect.centery))
-        tx,ty = s.rect.centerx/self.iso_w,s.rect.centery/self.iso_h
+
+        x, y = self.iso_to_view((s.rect.centerx, s.rect.centery))
+        tx, ty = s.rect.centerx / self.iso_w, s.rect.centery / self.iso_h
         z = 0
         if ty >= 0 and ty < h and tx >= 0 and tx < w:
-            z = zlayer[ty][tx]*self.iso_z
-        
-        nx,ny = x - s.shape.centerx, y - s.shape.centery + z
-        
-        s.irect.x,s.irect.y = nx,ny
+            z = zlayer[ty][tx] * self.iso_z
+
+        nx, ny = x - s.shape.centerx, y - s.shape.centery + z
+
+        s.irect.x, s.irect.y = nx, ny
```

### Comparing `zanthor-1.2.3/zanthor/pgu/engine.py` & `zanthor-1.2.4a2/zanthor/pgu/engine.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,154 +1,173 @@
 """a state engine. 
 """
 import pygame
 from pygame.locals import *
 
+
 class State:
     """Template Class -- for a state.
-    
+
     <pre>State(game,value...)</pre>
-    
+
     <dl>
     <dt>game<dd>The state engine.
     <dt>value<dd>I usually pass in a custom value to a state
     </dl>
-    
-    <p>For all of the template methods, they should return None unless they return 
+
+    <p>For all of the template methods, they should return None unless they return
     a new State to switch the engine to.</p>
     """
-    def __init__(self,game,value=None):
-        self.game,self.value = game,value
-    def init(self): 
+
+    def __init__(self, game, value=None):
+        self.game, self.value = game, value
+
+    def init(self):
         """Template Method - Initialize the state, called once the first time a state is selected.
-        
+
         <pre>State.init()</pre>
         """
         return
-    def paint(self,screen): 
-        """Template Method - Paint the screen.  Called once after the state is selected.  
-        
+
+    def paint(self, screen):
+        """Template Method - Paint the screen.  Called once after the state is selected.
+
         <p>State is responsible for calling <tt>pygame.display.flip()</tt> or whatever.</p>
-        
+
         <pre>State.paint(screen)</pre>
         """
         return
-        
-    def repaint(self): 
+
+    def repaint(self):
         """Template Method - Request a repaint of this state.
-        
+
         <pre>State.repaint()</pre>
         """
         self._paint = 1
-    def update(self,screen): 
+
+    def update(self, screen):
         """Template Method - Update the screen.
-        
+
         <p>State is responsible for calling <tt>pygame.display.update(updates)</tt> or whatever.</p>
-        
+
         <pre>State.update(screen)</pre>
         """
         return
+
     def loop(self):
         """Template Method - Run a logic loop, called once per frame.
-        
+
         <pre>State.loop()</pre>
         """
         return
-    def event(self,e):
+
+    def event(self, e):
         """Template Method - Recieve an event.
-        
+
         <pre>State.event(e)</pre>
         """
         return
 
+
 class Quit(State):
     """A state to quit the state engine.
-    
+
     <pre>Quit(game,value)</pre>
     """
-    
-    def init(self): 
+
+    def init(self):
         self.game.quit = 1
 
+
 class Game:
-    """Template Class - The state engine.
-    """
-    def fnc(self,f,v=None):
+    """Template Class - The state engine."""
+
+    def fnc(self, f, v=None):
         s = self.state
-        if not hasattr(s,f): return 0
-        f = getattr(s,f)
-        if v != None: r = f(v)
-        else: r = f()
+        if not hasattr(s, f):
+            return 0
+        f = getattr(s, f)
+        if v != None:
+            r = f(v)
+        else:
+            r = f()
         if r != None:
             self.state = r
             self.state._paint = 1
             return 1
         return 0
-        
-    def run(self,state,screen=None):
+
+    def run(self, state, screen=None):
         """Run the state engine, this is a infinite loop (until a quit occurs).
-        
+
         <pre>Game.run(state,screen=None)</pre>
-        
+
         <dl>
         <dt>game<dd>a state engine
         <dt>screen<dd>the screen
         </dl>
         """
         self.quit = 0
         self.state = state
-        if screen != None: self.screen = screen
-        
+        if screen != None:
+            self.screen = screen
+
         self.init()
-        
+
         while not self.quit:
             self.loop()
 
     def loop(self):
         s = self.state
-        if not hasattr(s,'_init') or s._init:
+        if not hasattr(s, "_init") or s._init:
             s._init = 0
-            if self.fnc('init'): return
-        else: 
-            if self.fnc('loop'): return
-        if not hasattr(s,'_paint') or s._paint:
+            if self.fnc("init"):
+                return
+        else:
+            if self.fnc("loop"):
+                return
+        if not hasattr(s, "_paint") or s._paint:
             s._paint = 0
-            if self.fnc('paint',self.screen): return
-        else: 
-            if self.fnc('update',self.screen): return
-        
+            if self.fnc("paint", self.screen):
+                return
+        else:
+            if self.fnc("update", self.screen):
+                return
+
         for e in pygame.event.get():
-            #NOTE: this might break API?
-	    #if self.event(e): return
-	    if not self.event(e):
-                if self.fnc('event',e): return
-            
+            # NOTE: this might break API?
+            # if self.event(e): return
+            if not self.event(e):
+                if self.fnc("event", e):
+                    return
+
         self.tick()
         return
-            
+
     def init(self):
         """Template Method - called at the beginning of State.run() to initialize things.
-        
+
         <pre>Game.init()</pre>
         """
         return
-        
+
     def tick(self):
         """Template Method - called once per frame, usually for timer purposes.
-        
+
         <pre>Game.tick()</pre>
         """
         pygame.time.wait(10)
-    
-    def event(self,e):
+
+    def event(self, e):
         """Template Method - called with each event, so the engine can capture special events.
-        
+
         <pre>Game.event(e): return captured</pre>
-        
+
         <p>return a True value if the event is captured and does not need to be passed onto the current
         state</p>
         """
-        if e.type is QUIT: 
+        if e.type == QUIT:
             self.state = Quit(self)
             return 1
 
+
 # vim: set filetype=python sts=4 sw=4 noet si :
```

### Comparing `zanthor-1.2.3/zanthor/cannon.py` & `zanthor-1.2.4a2/zanthor/cannon.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,92 @@
-import isovid
+from . import isovid
 import random
 
-from const import *
+from .const import *
 
-from units import CannonTower
+from .units import CannonTower
 
-import states
-import sound_info
+from . import sound_info
 
 
-def cannon_new(g,t,v):
+def cannon_new(g, t, v):
     g.clayer[t.ty][t.tx] = 0
-    s = isovid.Sprite(g.images['cannon'],t.rect)
-    
-    s.frame = random.randrange(0,FPS*3) 
+    s = isovid.Sprite(g.images["cannon"], t.rect)
+
+    s.frame = random.randrange(0, FPS * 3)
 
     g.sprites.append(s)
     s.loop = cannon_loop
     s.hit = cannon_hit
     s.groups = g.string2groups("cannon")
-    #s.agroups =g.string2groups("castle")
+    # s.agroups =g.string2groups("castle")
 
     s.unit = CannonTower()
 
 
-
-def cannon_loop(g,s):
+def cannon_loop(g, s):
     s.unit.loop()
 
-    tw,th = g.iso_w,g.iso_h
-    if s.frame%(FPS*3) == 0:
-        sx,sy = s.rect.centerx/tw,s.rect.centery/th
+    tw, th = g.iso_w, g.iso_h
+    if s.frame % (FPS * 3) == 0:
+        sx, sy = s.rect.centerx / tw, s.rect.centery / th
         p = g.castle
-        px,py = p.rect.centerx/tw,p.rect.centery/th
-        dx,dy = px-sx,py-sy
-        if (dx*dx+dy*dy)**0.5 < 12: #only shoot if they are reachable
-           # try and use some steam to fire.
+        px, py = p.rect.centerx / tw, p.rect.centery / th
+        dx, dy = px - sx, py - sy
+        if (dx * dx + dy * dy) ** 0.5 < 12:  # only shoot if they are reachable
+            # try and use some steam to fire.
             if s.unit.try_fire():
-                cball_new(g,(s.rect.centerx,s.rect.centery), s.unit.stats['Damage'])
-        
+                cball_new(g, (s.rect.centerx, s.rect.centery), s.unit.stats["Damage"])
 
     s.frame += 1
 
 
-def cannon_hit(g,a,b):
+def cannon_hit(g, a, b):
     pass
 
 
-def cball_new(g,pos, damage = 1.0):
+def cball_new(g, pos, damage=1.0):
     g.level.game.sm.Play("cannon")
 
-    s = isovid.Sprite(g.images['cball'],pos)
-    
+    s = isovid.Sprite(g.images["cball"], pos)
+
     s.frame = 0
 
     g.sprites.append(s)
     s.loop = cball_loop
     s.hit = cball_hit
-    #s.groups = g.string2groups("cball")
-    s.agroups =g.string2groups("castle")
-    
-    #s.rect, s._rect
-    
-    dx,dy = g.castle.rect.x-s.rect.x,g.castle.rect.y-s.rect.y
-    dist = (dx*dx+dy*dy)**0.5
+    # s.groups = g.string2groups("cball")
+    s.agroups = g.string2groups("castle")
+
+    # s.rect, s._rect
+
+    dx, dy = g.castle.rect.x - s.rect.x, g.castle.rect.y - s.rect.y
+    dist = (dx * dx + dy * dy) ** 0.5
     v = 16
-    s.vx, s.vy = dx*v/dist,dy*v/dist
+    s.vx, s.vy = dx * v / dist, dy * v / dist
     s.vz = -8
     s.z = 0
     s.damage = damage
-    
 
 
-def cball_loop(g,s):
-    
+def cball_loop(g, s):
     s.rect.x += s.vx
     s.rect.y += s.vy
     s.z += s.vz
     s.vz += 1
     if s.vz == 8:
         g.sprites.remove(s)
-    #print s.rect
+    # print s.rect
     s.frame += 1
-    
-    
-def cball_hit(g,a,b):
-    print "BANG!"
-    g.level.game.sm.Play(sound_info.ushit.nextone())
-
-    if b.unit.hit(a.damage):
-        #raise "game over, you got killed!"
-        #b.reset_castle()
-        g.level.game.state = states.GameOver(g.level.game) #, g.level.game.state)
 
 
+def cball_hit(g, a, b):
+    print("BANG!")
+    g.level.game.sm.Play(sound_info.ushit.nextone())
 
+    if b.unit.hit(a.damage):
+        # raise "game over, you got killed!"
+        # b.reset_castle()
+        from . import states
+        g.level.game.state = states.GameOver(g.level.game)  # , g.level.game.state)
 
     pass
-
```

### Comparing `zanthor-1.2.3/zanthor/menu.py` & `zanthor-1.2.4a2/zanthor/menu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,137 @@
 import pygame
 from pygame.locals import *
-from const import *
-#import pygame.draw
+from .const import *
 
-import util
+# import pygame.draw
+
+from . import util
 
 import os
-from pgu import engine
-import pgu.text
-import sound_info
+from .pgu import engine
+from .pgu import text
+from . import sound_info
+
+pgu_text_write = text.write
 
 """
 data = [
     (pygame.Rect(200,81,201,157),'Comfy Castle',4397,'level8.tga',100),
     (pygame.Rect(92,152,77,150),'Truthful Tower',1232,'level5.tga',100),
     (pygame.Rect(294,260,69,95),'Loyal Lookout',982,'level6.tga',100),
     (pygame.Rect(451,165,62,161),'Observatory of Honor',1444,'level7.tga',100),
     (pygame.Rect(17,335,99,58),'Simple City',214,'level1.tga',100),
     (pygame.Rect(144,390,117,52),'Valiant Village',319,'level2.tga',100),
     (pygame.Rect(325,378,118,54),'Humble Hamlet',182,'level3.tga',100),
     (pygame.Rect(509,328,96,66),'Congenial Burg',225,'level4.tga',100),
     ]
-""" 
+"""
 iy = img_shift_y = 44
-# 
-#lock,r,title,pop,n,perc,ztitle,music, selected
+#
+# lock,r,title,pop,n,perc,ztitle,music, selected
 data = [
-    (7,pygame.Rect(176, 7+iy, 213, 157),'Comfy Castle',4397,'level8.tga',70,        "Zanthor's Castle",'soundtrack3.ogg', (0,0)),
-
-    (4,pygame.Rect(100, 179+iy, 119, 94),'Truthful Tower',1232,'level5.tga',70,     "Zanthor's Obelisk",'soundtrack2.ogg', (1,0)),
-    (4,pygame.Rect(270, 179+iy, 119, 94),'Loyal Lookout',982,'level6.tga',70,       "Zanthor's Sausage Tree",'soundtrack2.ogg', (1,1)),
-    (4,pygame.Rect(389, 148+iy, 123, 125),'Observatory of Honor',1444,'level7.tga',70,"Zanthor's Toothpick",'soundtrack2.ogg', (1,2)),
-
-    (0,pygame.Rect(32, 237+iy, 144,  135),'Simple City',214,'level1.tga',80,        "Zanthor's Footstool",'soundtrack1.ogg', (2,0)),
-    (0,pygame.Rect(176, 273+iy, 125, 135),'Valiant Village',319,'level2.tga',80,    "Zanthor's Garden" ,'soundtrack1.ogg', (2,1)),
-    (0,pygame.Rect(301, 273+iy, 117, 83),'Humble Hamlet',182,'level3.tga',80,       "Zanthor's Coal Mine",'soundtrack1.ogg', (2,2)),
-    (0,pygame.Rect(487, 273+iy, 121, 135),'Congenial Burg',225,'level4.tga',80,     "Zanthor's Rec Room",'soundtrack1.ogg', (2,3)),
-    ]
+    (
+        7,
+        pygame.Rect(176, 7 + iy, 213, 157),
+        "Comfy Castle",
+        4397,
+        "level8.tga",
+        70,
+        "Zanthor's Castle",
+        "soundtrack3.ogg",
+        (0, 0),
+    ),
+    (
+        4,
+        pygame.Rect(100, 179 + iy, 119, 94),
+        "Truthful Tower",
+        1232,
+        "level5.tga",
+        70,
+        "Zanthor's Obelisk",
+        "soundtrack2.ogg",
+        (1, 0),
+    ),
+    (
+        4,
+        pygame.Rect(270, 179 + iy, 119, 94),
+        "Loyal Lookout",
+        982,
+        "level6.tga",
+        70,
+        "Zanthor's Sausage Tree",
+        "soundtrack2.ogg",
+        (1, 1),
+    ),
+    (
+        4,
+        pygame.Rect(389, 148 + iy, 123, 125),
+        "Observatory of Honor",
+        1444,
+        "level7.tga",
+        70,
+        "Zanthor's Toothpick",
+        "soundtrack2.ogg",
+        (1, 2),
+    ),
+    (
+        0,
+        pygame.Rect(32, 237 + iy, 144, 135),
+        "Simple City",
+        214,
+        "level1.tga",
+        80,
+        "Zanthor's Footstool",
+        "soundtrack1.ogg",
+        (2, 0),
+    ),
+    (
+        0,
+        pygame.Rect(176, 273 + iy, 125, 135),
+        "Valiant Village",
+        319,
+        "level2.tga",
+        80,
+        "Zanthor's Garden",
+        "soundtrack1.ogg",
+        (2, 1),
+    ),
+    (
+        0,
+        pygame.Rect(301, 273 + iy, 117, 83),
+        "Humble Hamlet",
+        182,
+        "level3.tga",
+        80,
+        "Zanthor's Coal Mine",
+        "soundtrack1.ogg",
+        (2, 2),
+    ),
+    (
+        0,
+        pygame.Rect(487, 273 + iy, 121, 135),
+        "Congenial Burg",
+        225,
+        "level4.tga",
+        80,
+        "Zanthor's Rec Room",
+        "soundtrack1.ogg",
+        (2, 3),
+    ),
+]
 
 
 def scale_data(data, size):
-
-    orig_size = 640,480
+    orig_size = 640, 480
     new_data = []
     for d in data:
         part = [d[0], util.scale_rect(d[1], orig_size, size)] + list(d[2:])
-        new_data.append( part )
-    
-    return new_data
-
+        new_data.append(part)
 
+    return new_data
 
 
 """
 32, 237, 144,  135
 176, 273, 125, 135
 231, 273, 117, 83
 487, 273, 121, 135
@@ -62,269 +140,284 @@
 119, 94, 270, 179
 123, 125, 289, 148
 213, 160, 176, 8
 """
 
 
 class Menu(engine.State):
-    
     def init(self):
-        self.bkgr = pygame.image.load(data_dir("gfx","caastles.png")).convert()
+        self.bkgr = pygame.image.load(data_dir("gfx", "caastles.png")).convert()
 
         screen_size = pygame.display.get_surface().get_size()
-        self.bkgr = pygame.transform.scale( self.bkgr, screen_size )
-        
+        self.bkgr = pygame.transform.scale(self.bkgr, screen_size)
+
         self.scaled_data = scale_data(data, screen_size)
 
+        # rev up music...
 
-        #rev up music...
-        
         self.fonts = {}
-        
-        for size in [48,24]:
-            self.fonts[size] = pygame.font.Font(data_dir("menu","vinque.ttf"),size)
+
+        for size in [48, 24]:
+            self.fonts[size] = pygame.font.Font(data_dir("menu", "vinque.ttf"), size)
 
         self.game.sm.Play(sound_info.birds[0])
         self.last_start = self.game.cur_time
         if hasattr(self.game.sm.sounds[sound_info.birds.cur()], "get_length"):
-            self.last_end = self.game.elapsed_time + self.game.sm.sounds[sound_info.birds.cur()].get_length()
+            self.last_end = (
+                self.game.elapsed_time
+                + self.game.sm.sounds[sound_info.birds.cur()].get_length()
+            )
         else:
             self.last_end = self.game.elapsed_time + 3.0
 
-
         self.frames = 0
         self.level = None
-        self.ximg = pygame.image.load(data_dir("menu","x.png")).convert_alpha()
+        self.ximg = pygame.image.load(data_dir("menu", "x.png")).convert_alpha()
         pygame.mouse.set_visible(True)
-        self.done = self.game.data['levels']
-        
+        self.done = self.game.data["levels"]
+
         if pygame.mixer:
             pygame.mixer.music.stop()
 
         self.selected_row = 2
         self.selected_collum = 0
 
         self.show_selected = 0
 
-        self.set_selected_parts((self.selected_row, self.selected_collum) )
-        
+        self.set_selected_parts((self.selected_row, self.selected_collum))
+
+    def paint(self, screen):
+        screen.blit(self.bkgr, (0, img_shift_y))
+        screen.blit(self.bkgr, (0, -SH + img_shift_y))
 
-    def paint(self,screen):
-        screen.blit(self.bkgr,(0,img_shift_y))
-        screen.blit(self.bkgr,(0,-SH+img_shift_y))
-        
-        fg = (0,0,0)
-        fg2 = (62,166,49)
+        fg = (0, 0, 0)
+        fg2 = (62, 166, 49)
         fnt = self.fonts[48]
-        
 
         text = "Sunflower Kingdom"
-        img = fnt.render(text,1,fg2)
-        x,y = (SW-img.get_width())/2,4
-        #screen.blit(img,(x-1,y+1))
-        pgu.text.write(screen,fnt,(x,y),(255,255,255),text,1)
+        img = fnt.render(text, 1, fg2)
+        x, y = (SW - img.get_width()) / 2, 4
+        # screen.blit(img,(x-1,y+1))
+        pgu_text_write(screen, fnt, (x, y), (255, 255, 255), text, 1)
+
+        #         img = fnt.render("Sunflower Kingdom",1,fg)
+        #         x,y = (SW-img.get_width())/2,4
+        #         screen.blit(img,(x,y))
 
-
-#         img = fnt.render("Sunflower Kingdom",1,fg)
-#         x,y = (SW-img.get_width())/2,4
-#         screen.blit(img,(x,y))
-        
         pos = pygame.mouse.get_pos()
-        
+
         fnt = self.fonts[24]
         self.level = None
-        
+
         done = self.done
         img = self.ximg
-        for lock,r,title,pop,n,perc,ztitle,music, selected in self.scaled_data:
+        for lock, r, title, pop, n, perc, ztitle, music, selected in self.scaled_data:
             if n in done:
-                screen.blit(img,(r.x+(r.w-img.get_width())/2,r.y+(r.h-img.get_height())/2))
+                screen.blit(
+                    img,
+                    (
+                        r.x + (r.w - img.get_width()) / 2,
+                        r.y + (r.h - img.get_height()) / 2,
+                    ),
+                )
 
         # selected is the row/collum of that city.
-        for lock,r,title,pop,n,perc,ztitle,music, selected in self.scaled_data:
-            #pygame.draw.rect(screen, (0,0,0), r, 1)
-            
-            
-            
+        for lock, r, title, pop, n, perc, ztitle, music, selected in self.scaled_data:
+            # pygame.draw.rect(screen, (0,0,0), r, 1)
+
             locked = False
-            if len(self.game.data['levels']) < lock: locked = True
+            if len(self.game.data["levels"]) < lock:
+                locked = True
 
-            if self.show_selected and selected == (self.selected_row, self.selected_collum):
-                text = 'selected'
-                img = fnt.render(text,1,fg)
-                #x,y = r.centerx-img.get_width()/2,r.bottom-24
-                x,y = r.centerx-img.get_width()/2,r.center[1]-10
-                pgu.text.write(screen,fnt,(x,y),(255,255,255),text,1)
+            if self.show_selected and selected == (
+                self.selected_row,
+                self.selected_collum,
+            ):
+                text = "selected"
+                img = fnt.render(text, 1, fg)
+                # x,y = r.centerx-img.get_width()/2,r.bottom-24
+                x, y = r.centerx - img.get_width() / 2, r.center[1] - 10
+                pgu_text_write(screen, fnt, (x, y), (255, 255, 255), text, 1)
 
                 if n not in done and not locked:
-                    self.level = n,perc,music
+                    self.level = n, perc, music
 
             if locked:
-                ltext = 'locked'
-                img = fnt.render(ltext,1,fg)
-                lx,ly = r.centerx-img.get_width()/2,r.bottom-24
-                pgu.text.write(screen,fnt,(lx,ly),(255,255,255),ltext,1)
-
-
-            if (self.show_selected and selected == (self.selected_row,self.selected_collum)):
+                ltext = "locked"
+                img = fnt.render(ltext, 1, fg)
+                lx, ly = r.centerx - img.get_width() / 2, r.bottom - 24
+                pgu_text_write(screen, fnt, (lx, ly), (255, 255, 255), ltext, 1)
+
+            if self.show_selected and selected == (
+                self.selected_row,
+                self.selected_collum,
+            ):
                 t = title
-                #if n in done: 
+                # if n in done:
                 #    t,pop = ztitle,0
-                
-                text = "%s - %s  -  %d citizens"%(n,t,pop)
-                text = "%s  -  %d citizens"%(t,pop)
-                
-                img = fnt.render(text,1,fg)
-                #img2 = fnt.render(text,1,fg2)
-                x,y = (SW-img.get_width())/2,SH-8-img.get_height()
-                pgu.text.write(screen,fnt,(x,y),(255,255,255),text,1)
 
+                text = "%s - %s  -  %d citizens" % (n, t, pop)
+                text = "%s  -  %d citizens" % (t, pop)
+
+                img = fnt.render(text, 1, fg)
+                # img2 = fnt.render(text,1,fg2)
+                x, y = (SW - img.get_width()) / 2, SH - 8 - img.get_height()
+                pgu_text_write(screen, fnt, (x, y), (255, 255, 255), text, 1)
 
                 # set this land as the selected place.
-                #self.selected_row, self.selected_collum = selected
+                # self.selected_row, self.selected_collum = selected
 
-                #screen.blit(img2,(x-1,y+1))
-                #screen.blit(img,(x,y))
+                # screen.blit(img2,(x-1,y+1))
+                # screen.blit(img,(x,y))
                 if n not in done and not locked:
-                    self.level = n,perc,music
-                #break
-            
-        
+                    self.level = n, perc, music
+                # break
+
         pygame.display.flip()
         return
-        
-        
-    def loop(self):
-        if not self.frames % int(FPS/ 4):
 
+    def loop(self):
+        if not self.frames % int(FPS / 4):
             # mix the sounds in with 1. second.
-            if (self.last_end - self.game.elapsed_time) < 1.:
+            if (self.last_end - self.game.elapsed_time) < 1.0:
                 self.game.sm.Play(sound_info.birds.nextone())
                 self.last_start = self.game.cur_time
                 if hasattr(self.game.sm.sounds[sound_info.birds.cur()], "get_length"):
-                    self.last_end = self.game.elapsed_time + self.game.sm.sounds[sound_info.birds.cur()].get_length()
+                    self.last_end = (
+                        self.game.elapsed_time
+                        + self.game.sm.sounds[sound_info.birds.cur()].get_length()
+                    )
                 else:
                     # we just play for 3 seconds.
                     self.last_end = self.game.elapsed_time + 3.0
 
         self.frames += 1
 
-
-    def update(self,screen):
+    def update(self, screen):
         return self.paint(screen)
-    
+
     def find_select_place(self, tobe):
-        """ Returns True if it finds the level.  else returns False.
-            goes through the level data to see if the tobe coords are the same as that level.
+        """Returns True if it finds the level.  else returns False.
+        goes through the level data to see if the tobe coords are the same as that level.
         """
-        #print tobe
+        # print tobe
 
         found = False
         for d in self.scaled_data:
             levellock = d[0]
             pos_of_place = d[8]
             n = d[4]
             # last collumn of data  eg (0,0) is the castle at top.
             if tobe == pos_of_place:
                 locked = False
-                
-                if len(self.game.data['levels']) < levellock:
+
+                if len(self.game.data["levels"]) < levellock:
                     locked = True
                 if not locked and n not in self.done:
                     found = True
                     break
 
         return found
 
-
     def set_selected_parts(self, tobe):
-        """ this makes sure the selected parts are within bounds.
-        """
+        """this makes sure the selected parts are within bounds."""
 
-        # check to see if we can select a level.  
-        #    Some levels are locked, or finished.  
+        # check to see if we can select a level.
+        #    Some levels are locked, or finished.
         #    Some are out of bounds. eg if pressing left on far left.
         # we try going in either direction... depending on what we find.
         if tobe[1] - self.selected_collum <= 0:
             # we see if the selected place exists... otherwise we don't set it.
             for x in range(5):
-                found = self.find_select_place((tobe[0], tobe[1] -x))
+                found = self.find_select_place((tobe[0], tobe[1] - x))
 
                 if found:
-                    self.selected_row, self.selected_collum = (tobe[0], tobe[1]-x )
+                    self.selected_row, self.selected_collum = (tobe[0], tobe[1] - x)
                     break
         else:
-        
             for x in range(5):
-                found = self.find_select_place((tobe[0], tobe[1] +x))
+                found = self.find_select_place((tobe[0], tobe[1] + x))
 
                 if found:
-                    self.selected_row, self.selected_collum = (tobe[0], tobe[1]+x )
+                    self.selected_row, self.selected_collum = (tobe[0], tobe[1] + x)
                     break
 
         # ok... we try and go up.
         if not found:
             for x in range(5):
-                found = self.find_select_place((tobe[0]-x, tobe[1]))
+                found = self.find_select_place((tobe[0] - x, tobe[1]))
 
                 if found:
-                    self.selected_row, self.selected_collum = (tobe[0]-x, tobe[1])
+                    self.selected_row, self.selected_collum = (tobe[0] - x, tobe[1])
                     break
 
-
-
-        
-
-    
-    def event(self,e):
-        if e.type is MOUSEMOTION:
-            for lock,r,title,pop,n,perc,ztitle,music, selected in self.scaled_data:
+    def event(self, e):
+        print("menu e, K_LEFT, K_a", e, K_LEFT, K_a)
+        if e.type == MOUSEMOTION:
+            for (
+                lock,
+                r,
+                title,
+                pop,
+                n,
+                perc,
+                ztitle,
+                music,
+                selected,
+            ) in self.scaled_data:
                 if r.collidepoint(e.pos):
                     self.show_selected = True
                     self.set_selected_parts(selected)
-                    
-        if (((e.type in [MOUSEBUTTONDOWN, JOYBUTTONDOWN]) or 
-             (e.type is KEYDOWN and e.key in [K_RETURN, K_SPACE])) and 
-             (self.level != None)):
-            import level
-            return level.Level(self.game,*self.level)
-        
-
-        if e.type is KEYDOWN and e.key == K_ESCAPE:
-            import states
-            import title
-            return states.Prompt(self.game,"quit? y/n",title.Title(self.game),self)
-        
+
+        if (
+            (e.type in [MOUSEBUTTONDOWN, JOYBUTTONDOWN])
+            or (e.type == KEYDOWN and e.key in [K_RETURN, K_SPACE])
+        ) and (self.level != None):
+            from . import level
+
+            return level.Level(self.game, *self.level)
+
+        if e.type == KEYDOWN and e.key == K_ESCAPE:
+            from . import states
+            from . import title
+
+            return states.Prompt(self.game, "quit? y/n", title.Title(self.game), self)
 
         if e.type in [KEYDOWN, JOYAXISMOTION]:
             self.show_selected = True
 
-        if e.type is KEYDOWN and e.key in [K_LEFT, K_a]:
-            self.set_selected_parts((self.selected_row, self.selected_collum-1))
+        if e.type == KEYDOWN and e.key in [K_LEFT, K_a]:
+            self.set_selected_parts((self.selected_row, self.selected_collum - 1))
 
-        if e.type is KEYDOWN and e.key in [K_RIGHT, K_d]:
-            self.set_selected_parts((self.selected_row, self.selected_collum+1))
+        if e.type == KEYDOWN and e.key in [K_RIGHT, K_d]:
+            self.set_selected_parts((self.selected_row, self.selected_collum + 1))
 
-        if e.type is KEYDOWN and e.key in [K_UP, K_w]:
-            self.set_selected_parts((self.selected_row-1, self.selected_collum))
-
-        if e.type is KEYDOWN and e.key in [K_DOWN, K_s]:
-            self.set_selected_parts((self.selected_row+1, self.selected_collum))
+        if e.type == KEYDOWN and e.key in [K_UP, K_w]:
+            self.set_selected_parts((self.selected_row - 1, self.selected_collum))
 
+        if e.type == KEYDOWN and e.key in [K_DOWN, K_s]:
+            self.set_selected_parts((self.selected_row + 1, self.selected_collum))
 
         if e.type == JOYAXISMOTION:
             if e.axis == 1:
                 if round(e.value) < 0:
                     # up
-                    self.set_selected_parts((self.selected_row-1, self.selected_collum))
+                    self.set_selected_parts(
+                        (self.selected_row - 1, self.selected_collum)
+                    )
                 elif round(e.value) > 0:
                     # down
-                    self.set_selected_parts((self.selected_row+1, self.selected_collum))
+                    self.set_selected_parts(
+                        (self.selected_row + 1, self.selected_collum)
+                    )
 
             if e.axis == 0:
                 if round(e.value) < 0:
                     # left
-                    self.set_selected_parts((self.selected_row, self.selected_collum-1))
+                    self.set_selected_parts(
+                        (self.selected_row, self.selected_collum - 1)
+                    )
                 elif round(e.value) > 0:
                     # right
-                    self.set_selected_parts((self.selected_row, self.selected_collum+1))
-
+                    self.set_selected_parts(
+                        (self.selected_row, self.selected_collum + 1)
+                    )
```

### Comparing `zanthor-1.2.3/zanthor/steam.py` & `zanthor-1.2.4a2/zanthor/steam.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,141 +1,141 @@
 import pygame
 from pygame.locals import *
 import random
 
-from pgu import timer
+from .pgu import timer
 
 rr = random.randrange
 
+
 class Part:
-    def __init__(self,pos,z):
-        self.pos = pygame.Rect(pos[0],pos[1],1,1)
+    def __init__(self, pos, z):
+        self.pos = pygame.Rect(pos[0], pos[1], 1, 1)
         self._pos = pygame.Rect(self.pos)
         self.frame = 0
         self.z = z
 
 
 NUM_BITS = 10
 
+
 class Effect:
-    def __init__(self,total,add,region=1,respawn=1,color=(255,255,255)):
-        
-        #if not hasattr(Effect,'images'):
+    def __init__(self, total, add, region=1, respawn=1, color=(255, 255, 255)):
+        # if not hasattr(Effect,'images'):
         #    Effect._init(self)
-        
+
         self._init(color)
-        
+
         self.total = total
         self.add = add
-        
+
         self.parts = []
         self.region = region
         self.respawn = respawn
-        
+
         self.frame = 0
         self.frames = 0
-        
-    def _init(self,color):
-        if not hasattr(Effect,'data'):
+
+    def _init(self, color):
+        if not hasattr(Effect, "data"):
             Effect.data = {}
         data = Effect.data
-        k = 'images.%s'%str(color)
+        k = "images.%s" % str(color)
         if k not in data:
             images = data[k] = []
-            for r in xrange(0,NUM_BITS):
-                img = pygame.Surface((r*2,r*2)).convert()
-                img.fill((255,0,255))
-                img.set_colorkey((255,0,255))
-                img.set_alpha(255-r*(8*32/NUM_BITS))
-                pygame.draw.circle(img,color,(r,r),r)
-                #pygame.draw.circle(img,(255-r*8,255-r*8,255-r*8),(r,r),r)
+            for r in range(0, NUM_BITS):
+                img = pygame.Surface((r * 2, r * 2)).convert()
+                img.fill((255, 0, 255))
+                img.set_colorkey((255, 0, 255))
+                img.set_alpha(255 - r * (8 * 32 / NUM_BITS))
+                pygame.draw.circle(img, color, (r, r), r)
+                # pygame.draw.circle(img,(255-r*8,255-r*8,255-r*8),(r,r),r)
                 images.append(img)
         self.images = data[k]
 
-        
-    def zpaint(self): #,origin):
-
+    def zpaint(self):  # ,origin):
         ret = []
 
         if 1 or not self.frames % 2:
-
-            todo = [[] for n in xrange(0,NUM_BITS)]
+            todo = [[] for n in range(0, NUM_BITS)]
             for part in self.parts:
                 p = part.pos
                 r = part.frame
-                if r >= 0 and r < NUM_BITS: todo[r].append(part)
-            for r in xrange(NUM_BITS-1,-1,-1):
+                if r >= 0 and r < NUM_BITS:
+                    todo[r].append(part)
+            for r in range(NUM_BITS - 1, -1, -1):
                 img = self.images[r]
-                v = 255-r*8
-                #c = (v,v,v)
-                #c = (255,255,255,v)
+                v = 255 - r * 8
+                # c = (v,v,v)
+                # c = (255,255,255,v)
                 for part in todo[r]:
                     p = part.pos
-                    #pygame.draw.circle(screen,c,(p.x+pos[0],p.y+pos[1]),r+3)
-                    #screen.blit(img,(-origin[0]+p.x-r,-origin[1]+p.y-r))
-                    ret.append((part.z,img,(p.x-r,p.y-r)))
+                    # pygame.draw.circle(screen,c,(p.x+pos[0],p.y+pos[1]),r+3)
+                    # screen.blit(img,(-origin[0]+p.x-r,-origin[1]+p.y-r))
+                    ret.append((part.z, img, (p.x - r, p.y - r)))
 
         self.frames += 1
-        
+
         return ret
-                
 
-            
-    def zloop(self,pos,z):
+    def zloop(self, pos, z):
         parts = self.parts
         if len(parts) < self.total:
             region = self.region
-            for n in xrange(0,self.add):
-                part = Part((pos[0]+rr(-region,region),pos[1]+rr(-region,region)),z)
+            for n in range(0, self.add):
+                part = Part(
+                    (pos[0] + rr(-region, region), pos[1] + rr(-region, region)), z
+                )
                 parts.append(part)
         for part in parts:
-            p,_p = part.pos,part._pos
+            p, _p = part.pos, part._pos
+
+            dx, dy = p.x - _p.x, p.y - _p.y
+            _p.x, _p.y = p.x, p.y
 
-            dx,dy = p.x-_p.x,p.y-_p.y
-            _p.x,_p.y = p.x,p.y
-            
-            p.x += dx/3 + rr(-4,2)
-            p.y += dy/4 + rr(-6,2)
-            
-            #r = (abs(p.x)+abs(p.y))/8
-            #if r > NUM_BITS:
+            p.x += dx / 3 + rr(-4, 2)
+            p.y += dy / 4 + rr(-6, 2)
+
+            # r = (abs(p.x)+abs(p.y))/8
+            # if r > NUM_BITS:
             part.frame += 1
-            
+
             if part.frame >= NUM_BITS and self.respawn:
-                p.x,p.y = pos[0]+rr(-2,2),pos[1]+rr(-2,0)
-                _p.x,_p.y = p.x,p.y
+                p.x, p.y = pos[0] + rr(-2, 2), pos[1] + rr(-2, 0)
+                _p.x, _p.y = p.x, p.y
                 part.z = z
                 part.frame = 0
-                
-                
-    def paint(self,screen,origin):
-        for z,img,pos in self.zpaint():
-            screen.blit(img,(-origin[0]+pos[0],-origin[1]+pos[1]))
-
-    def loop(self,pos):
-        return self.zloop(pos,0)
-            
-if __name__ == '__main__':
-    screen = pygame.display.set_mode((640,480))
-    
-    
-    ss = [((rr(160,640),rr(160,480)),Effect(NUM_BITS,1)) for n in xrange(0,8)]
-    
-    #t = timer.Timer(40)
+
+    def paint(self, screen, origin):
+        for z, img, pos in self.zpaint():
+            screen.blit(img, (-origin[0] + pos[0], -origin[1] + pos[1]))
+
+    def loop(self, pos):
+        return self.zloop(pos, 0)
+
+
+if __name__ == "__main__":
+    screen = pygame.display.set_mode((640, 480))
+
+    ss = [((rr(160, 640), rr(160, 480)), Effect(NUM_BITS, 1)) for n in range(0, 8)]
+
+    # t = timer.Timer(40)
     t = timer.Speedometer()
     pygame.time.get_ticks()
-    
+
     _quit = False
     while not _quit:
         for e in pygame.event.get():
-            if e.type is QUIT: _quit = True
-            if e.type is KEYDOWN and e.key == K_ESCAPE: _quit = True
-        
-        screen.fill((0,0,0))
-        for pos,s in ss:
+            if e.type == QUIT:
+                _quit = True
+            if e.type == KEYDOWN and e.key == K_ESCAPE:
+                _quit = True
+
+        screen.fill((0, 0, 0))
+        for pos, s in ss:
             s.loop(pos)
-            s.paint(screen,(0,0))
+            s.paint(screen, (0, 0))
         pygame.display.flip()
-        
+
         r = t.tick()
-        if r: print r
-        
+        if r:
+            print(r)
```

### Comparing `zanthor-1.2.3/zanthor/title.py` & `zanthor-1.2.4a2/zanthor/title.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,194 +1,222 @@
-
-#this file gets all the dinky little generic states
+# this file gets all the dinky little generic states
 
 import pygame
 from pygame.locals import *
 
 import os
 
-from pgu import engine
-import pgu.text
+from .pgu import engine
+from .pgu import text
 
-from const import *
-import util
+from .const import *
+from . import util
 import random
 
+pgu_text_write = text.write
+
 class Title(engine.State):
-    
     def init(self):
         self.menu = [
-            ('Start','start'),
-            #('Load','load'),
-            #('Save','save'),
-            ('Help',Help),
-            ('Credits',Credits),
-            ('Quit',engine.Quit),
-            ]
+            ("Start", "start"),
+            # ('Load','load'),
+            # ('Save','save'),
+            ("Help", Help),
+            ("Credits", Credits),
+            ("Quit", engine.Quit),
+        ]
         self.cur = 0
 
         if pygame.mixer:
-            pygame.mixer.music.load(data_dir("intro","zanthor.ogg"))
+            pygame.mixer.music.load(data_dir("intro", "zanthor.ogg"))
             pygame.mixer.music.play(-1)
-        
+
         self.font_title = []
-        for size in (160,165,170,175,180):
-            self.font_title.append(pygame.font.Font(data_dir("intro","WALSHES.TTF"),size))
-        self.font_main = pygame.font.Font(data_dir("menu","vinque.ttf"),32)
-        
+        for size in (160, 165, 170, 175, 180):
+            self.font_title.append(
+                pygame.font.Font(data_dir("intro", "WALSHES.TTF"), size)
+            )
+        self.font_main = pygame.font.Font(data_dir("menu", "vinque.ttf"), 32)
+
         self.rects = []
         pygame.mouse.set_visible(True)
-        self.bkgr = pygame.image.load(data_dir("intro","mybkgr.png"))
-        
+        self.bkgr = pygame.image.load(data_dir("intro", "mybkgr.png"))
+
         self.frame = 0
 
+    def paint(self, screen):
+        # print self.game.backup_castle_stats
+        screen.fill((255, 0, 0))
+
+        img = self.bkgr.subsurface((404, 121, 236, 359))
+        img = pygame.transform.rotozoom(
+            img, random.randrange(-15, 15), random.randrange(90, 115) / 100.0
+        )
+        x, y = 380 - img.get_width() / 2 + random.randrange(
+            -24, 24
+        ), 290 - img.get_height() / 2 + random.randrange(-12, 12)
+        screen.blit(img, (x, y))
 
-        
-    def paint(self,screen):
-        
-        #print self.game.backup_castle_stats
-        screen.fill((255,0,0))
-        
-        img = self.bkgr.subsurface((404,121,236,359))
-        img = pygame.transform.rotozoom(img, random.randrange(-15,15),random.randrange(90,115)/100.0)
-        x,y = 380-img.get_width()/2+random.randrange(-24,24),290-img.get_height()/2+random.randrange(-12,12)
-        screen.blit(img,(x,y))
-        
         fnt = random.choice(self.font_title)
         text = "Zanthor"
-        fg,bg,b = (255,255,255),(0,0,0),4
-        if self.frame%8 < 4: fg = (255,0x55,0x55)
-        
-        img = fnt.render(text,1,bg)
-        x,y = (SW-img.get_width())/2+random.randrange(-8,8),100-img.get_height()/2+random.randrange(-8,8)
-        for dx,dy in [(-1,0),(0,1),(1,0),(0,-1),(-1,-1),(-1,1),(1,-1),(1,1)]:
-            screen.blit(img,(x+dx*b,y+dy*b))
-        img = fnt.render(text,1,fg)
-        screen.blit(img,(x,y))
-        
-        
+        fg, bg, b = (255, 255, 255), (0, 0, 0), 4
+        if self.frame % 8 < 4:
+            fg = (255, 0x55, 0x55)
+
+        img = fnt.render(text, 1, bg)
+        x, y = (SW - img.get_width()) / 2 + random.randrange(
+            -8, 8
+        ), 100 - img.get_height() / 2 + random.randrange(-8, 8)
+        for dx, dy in [
+            (-1, 0),
+            (0, 1),
+            (1, 0),
+            (0, -1),
+            (-1, -1),
+            (-1, 1),
+            (1, -1),
+            (1, 1),
+        ]:
+            screen.blit(img, (x + dx * b, y + dy * b))
+        img = fnt.render(text, 1, fg)
+        screen.blit(img, (x, y))
+
         fnt = self.font_main
-        x,y,n = 48,220,0
-        self.rects= []
-        
-        for text,action in self.menu:
-            c = (0xaa,0xaa,0xaa)
-            if n == self.cur: c = (255,255,255)
-            bg = (0,0,0)
-            img = fnt.render(text,1,bg)
+        x, y, n = 48, 220, 0
+        self.rects = []
+
+        for text, action in self.menu:
+            c = (0xAA, 0xAA, 0xAA)
+            if n == self.cur:
+                c = (255, 255, 255)
+            bg = (0, 0, 0)
+            img = fnt.render(text, 1, bg)
             b = 2
-            for dx,dy in [(-1,0),(0,1),(1,0),(0,-1)]:
-                screen.blit(img,(x+dx*b,y+dy*b))
-            
-            img = fnt.render(text,1,c)
-            screen.blit(img,(x,y))
-            self.rects.append((n,pygame.Rect(x,y,img.get_width(),img.get_height())))
+            for dx, dy in [(-1, 0), (0, 1), (1, 0), (0, -1)]:
+                screen.blit(img, (x + dx * b, y + dy * b))
+
+            img = fnt.render(text, 1, c)
+            screen.blit(img, (x, y))
+            self.rects.append((n, pygame.Rect(x, y, img.get_width(), img.get_height())))
             y += 40
             n += 1
-        #print self.cur,n
-        
+        # print self.cur,n
+
         pygame.display.flip()
-        
+
     def loop(self):
-        if self.frame%3==0:
+        if self.frame % 3 == 0:
             self.repaint()
         self.frame += 1
-    
-    def event(self,e):
-        if e.type is MOUSEMOTION:
-            for n,r in self.rects:
+
+    def event(self, e):
+        print('title', e, e.type == KEYDOWN, e.type, KEYDOWN, K_UP, K_DOWN)
+        if e.type == MOUSEMOTION:
+            for n, r in self.rects:
                 if r.collidepoint(e.pos):
                     self.cur = n
-                    #self.repaint()
+                    # self.repaint()
 
         elif e.type == JOYAXISMOTION:
             if e.axis == 1:
                 if round(e.value) < 0:
-                    self.cur = (self.cur-1+len(self.menu))%len(self.menu)
+                    self.cur = (self.cur - 1 + len(self.menu)) % len(self.menu)
                 elif round(e.value) > 0:
-                    self.cur = (self.cur+1+len(self.menu))%len(self.menu)
-        
-        elif e.type is KEYDOWN:
+                    self.cur = (self.cur + 1 + len(self.menu)) % len(self.menu)
+
+        elif e.type == KEYDOWN:
+            print('keydown')
             if e.key == K_UP:
-                self.cur = (self.cur-1+len(self.menu))%len(self.menu)
-                #self.repaint()
+                print('UP', self.cur)
+                self.cur = (self.cur - 1 + len(self.menu)) % len(self.menu)
+                print('UP after', self.cur)
+                # self.repaint()
             if e.key == K_DOWN:
-                self.cur = (self.cur+1+len(self.menu))%len(self.menu)
-                #self.repaint()
-        if (e.type is KEYDOWN and e.key == K_RETURN) or e.type in [MOUSEBUTTONDOWN, JOYBUTTONDOWN]:
-            text,action = self.menu[self.cur]
-            if action == 'start':
+                print('DOWN', self.cur)
+                self.cur = (self.cur + 1 + len(self.menu)) % len(self.menu)
+                print('DOWN after', self.cur)
+                # self.repaint()
+
+            
+        if (e.type == KEYDOWN and e.key == K_RETURN) or e.type in [
+            MOUSEBUTTONDOWN,
+            JOYBUTTONDOWN,
+        ]:
+            text, action = self.menu[self.cur]
+            if action == "start":
                 if pygame.mixer:
                     pygame.mixer.music.stop()
                 g = self.game
                 g.data_reset()
-                import menu
+                from . import menu
+
                 return menu.Menu(self.game)
-            else: return action(self.game)
-        
-#etc...
+            else:
+                return action(self.game)
+
+
+# etc...
 
 
 class Help(engine.State):
-    def paint(self,screen):
-        screen.blit(pygame.image.load(data_dir("intro","mybkgr.png")),(0,0))
-        
+    def paint(self, screen):
+        screen.blit(pygame.image.load(data_dir("intro", "mybkgr.png")), (0, 0))
+
         text = [
-            'help',
-            '',
-            'press and hold right mouse',
-            'to build up pressure.',
-            'release to shoot.',
-            '',
+            "help",
+            "",
+            "press and hold right mouse",
+            "to build up pressure.",
+            "release to shoot.",
+            "",
             "collect coal and water",
             "to keep steam up.",
             "",
             "arrow keys, a/w/s/d also",
             "work.  f/space to fire.",
             "",
             "you are ZANTHOR!",
-            ]
-            
-        fnt = pygame.font.Font(data_dir("menu","vinque.ttf"),24)
-        x,y = 48,20
+        ]
+
+        fnt = pygame.font.Font(data_dir("menu", "vinque.ttf"), 24)
+        x, y = 48, 20
         for line in text:
-            img = fnt.render(line,0,(0,0,0))
-            #x = (SW-img.get_width())/2
-            #screen.blit(img,(x,y))
-            pgu.text.write(screen,fnt,(x,y),(255,255,255),line,1)
+            img = fnt.render(line, 0, (0, 0, 0))
+            # x = (SW-img.get_width())/2
+            # screen.blit(img,(x,y))
+            pgu_text_write(screen, fnt, (x, y), (255, 255, 255), line, 1)
             y += 32
         pygame.display.flip()
-        
-    def event(self,e):
-        if e.type is KEYDOWN or e.type is MOUSEBUTTONDOWN:
+
+    def event(self, e):
+        if e.type == KEYDOWN or e.type == MOUSEBUTTONDOWN:
             return Title(self.game)
-        
+
+
 class Credits(engine.State):
-    def paint(self,screen):
-        screen.fill((255,0,0))
+    def paint(self, screen):
+        screen.fill((255, 0, 0))
 
-        screen.blit(pygame.image.load(data_dir("intro","mybkgr.png")),(0,0))
+        screen.blit(pygame.image.load(data_dir("intro", "mybkgr.png")), (0, 0))
         text = [
-            'credits',
-            '',
-            'aka - graphics',
-            'illume - code, etc',
-            'philhassey - code, etc',
-            'TimInge - music, sfx',
-            '',
-            ]
-            
-        fnt = pygame.font.Font(data_dir("menu","vinque.ttf"),32)
-        x,y = 60,20
+            "credits",
+            "",
+            "aka - graphics",
+            "illume - code, etc",
+            "philhassey - code, etc",
+            "TimInge - music, sfx",
+            "",
+        ]
+
+        fnt = pygame.font.Font(data_dir("menu", "vinque.ttf"), 32)
+        x, y = 60, 20
         for line in text:
-            img = fnt.render(line,0,(0,0,0))
-            x = (460-img.get_width())/2
-            #screen.blit(img,(x,y))
-            pgu.text.write(screen,fnt,(x,y),(255,255,255),line,1)
+            img = fnt.render(line, 0, (0, 0, 0))
+            x = (460 - img.get_width()) / 2
+            # screen.blit(img,(x,y))
+            pgu_text_write(screen, fnt, (x, y), (255, 255, 255), line, 1)
             y += 48
         pygame.display.flip()
-            
-        
-    def event(self,e):
-        if e.type is KEYDOWN or e.type is MOUSEBUTTONDOWN:
-            return Title(self.game)
 
+    def event(self, e):
+        if e.type == KEYDOWN or e.type == MOUSEBUTTONDOWN:
+            return Title(self.game)
```

### Comparing `zanthor-1.2.3/zanthor/algo.py` & `zanthor-1.2.4a2/zanthor/algo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,135 +1,166 @@
 """Some handy algorithms for use in games, etc.
 
 <p>please note that this file is alpha, and is subject to modification in
 future versions of pgu!</p>
 """
-print 'pgu.algo','This module is alpha, and is subject to change.'
+print(("pgu.algo", "This module is alpha, and is subject to change."))
 
-#def dist(a,b):
+# def dist(a,b):
 #    return abs(a[0]-b[0]) + abs(a[1]-b[1])
-    
+
+
 class node:
-    def __init__(self,prev,pos,dest):
-        self.prev,self.pos,self.dest = prev,pos,dest
-        if self.prev == None: self.g = 0
-        else: self.g = self.prev.g + 1
-        self.h = dist(pos,dest)
-        self.f = self.g+self.h
+    def __init__(self, prev, pos, dest):
+        self.prev, self.pos, self.dest = prev, pos, dest
+        if self.prev == None:
+            self.g = 0
+        else:
+            self.g = self.prev.g + 1
+        self.h = dist(pos, dest)
+        self.f = self.g + self.h
 
 
-def astar(start,end,layer,_dist):
+def astar(start, end, layer, _dist):
     """uses the a* algorithm to find a path
-    
+
     <pre>astar(start,end,layer,dist): return [list of positions]</pre>
-    
+
     <dl>
     <dt>start<dd>start position
     <dt>end<dd>end position
     <dt>layer<dd>a grid where zero cells are open and non-zero cells are walls
     <dt>dist<dd>a distance function dist(a,b)
     </dl>
-    
+
     <p>returns a list of positions from start to end</p>
     """
     global dist
     dist = _dist
-    if layer[start[1]][start[0]]: return [] #start is blocked
-    if layer[end[1]][end[0]]: return [] #end is blocked
-    w,h = len(layer[0]),len(layer)
-    if start[0] < 0 or start[1] < 0 or start[0] >= w or start[1] >= h: return [] #start outside of layer
-    if end[0] < 0 or end[1] < 0 or end[0] >= w or end[1] >= h: return [] #end outside of layer
+    if layer[start[1]][start[0]]:
+        return []  # start is blocked
+    if layer[end[1]][end[0]]:
+        return []  # end is blocked
+    w, h = len(layer[0]), len(layer)
+    if start[0] < 0 or start[1] < 0 or start[0] >= w or start[1] >= h:
+        return []  # start outside of layer
+    if end[0] < 0 or end[1] < 0 or end[0] >= w or end[1] >= h:
+        return []  # end outside of layer
 
     opens = []
     open = {}
     closed = {}
-    cur = node(None,start,end)
+    cur = node(None, start, end)
     open[cur.pos] = cur
     opens.append(cur)
     while len(open):
         cur = opens.pop(0)
-        if cur.pos not in open: continue
+        if cur.pos not in open:
+            continue
         del open[cur.pos]
         closed[cur.pos] = cur
-        if cur.pos == end: break
-        for dx,dy in [(0,-1),(1,0),(0,1),(-1,0),(-1,-1),(1,-1),(-1,1),(1,1)]:
-            x,y = pos = cur.pos[0]+dx,cur.pos[1]+dy
-            if layer[y][x]: continue
-            #check for blocks of diagonals
-            if layer[cur.pos[1]+dy][cur.pos[0]]: continue
-            if layer[cur.pos[1]][cur.pos[0]+dx]: continue
-            new = node(cur,pos,end)
-            if pos in open and new.f >= open[pos].f: continue
-            if pos in closed and new.f >= closed[pos].f: continue
-            if pos in open: del open[pos]
-            if pos in closed: del closed[pos]
+        if cur.pos == end:
+            break
+        for dx, dy in [
+            (0, -1),
+            (1, 0),
+            (0, 1),
+            (-1, 0),
+            (-1, -1),
+            (1, -1),
+            (-1, 1),
+            (1, 1),
+        ]:
+            x, y = pos = cur.pos[0] + dx, cur.pos[1] + dy
+            if layer[y][x]:
+                continue
+            # check for blocks of diagonals
+            if layer[cur.pos[1] + dy][cur.pos[0]]:
+                continue
+            if layer[cur.pos[1]][cur.pos[0] + dx]:
+                continue
+            new = node(cur, pos, end)
+            if pos in open and new.f >= open[pos].f:
+                continue
+            if pos in closed and new.f >= closed[pos].f:
+                continue
+            if pos in open:
+                del open[pos]
+            if pos in closed:
+                del closed[pos]
             open[pos] = new
             lo = 0
             hi = len(opens)
             while lo < hi:
-                mid = (lo+hi)/2
-                if new.f < opens[mid].f: hi = mid
-                else: lo = mid + 1
-            opens.insert(lo,new)
-    
-    if cur.pos != end: 
+                mid = (lo + hi) / 2
+                if new.f < opens[mid].f:
+                    hi = mid
+                else:
+                    lo = mid + 1
+            opens.insert(lo, new)
+
+    if cur.pos != end:
         return []
-                    
+
     path = []
     while cur.prev != None:
         path.append(cur.pos)
         cur = cur.prev
     path.reverse()
     return path
-    
 
-def getline(a,b):
+
+def getline(a, b):
     """returns a path of points from a to b
-    
+
     <pre>getline(a,b): return [list of points]</pre>
-    
+
     <dl>
     <dt>a<dd>starting point
     <dt>b<dd>ending point
     </dl>
-    
+
     <p>returns a list of points from a to b</p>
     """
-           
+
     path = []
-    
-    x1,y1 = a
-    x2,y2 = b
-    dx,dy = abs(x2-x1),abs(y2-y1)
-
-    if x2 >= x1: xi1,xi2 = 1,1
-    else: xi1,xi2 = -1,-1
-    
-    if y2 >= y1: yi1,yi2 = 1,1
-    else: yi1,yi2 = -1,-1
-    
+
+    x1, y1 = a
+    x2, y2 = b
+    dx, dy = abs(x2 - x1), abs(y2 - y1)
+
+    if x2 >= x1:
+        xi1, xi2 = 1, 1
+    else:
+        xi1, xi2 = -1, -1
+
+    if y2 >= y1:
+        yi1, yi2 = 1, 1
+    else:
+        yi1, yi2 = -1, -1
+
     if dx >= dy:
-        xi1,yi2 = 0,0
+        xi1, yi2 = 0, 0
         d = dx
-        n = dx/2
+        n = dx / 2
         a = dy
         p = dx
     else:
-        xi2,yi1 = 0,0
+        xi2, yi1 = 0, 0
         d = dy
-        n = dy/2
+        n = dy / 2
         a = dx
         p = dy
-        
-    x,y = x1,y1
+
+    x, y = x1, y1
     c = 0
     while c <= p:
-        path.append((x,y))
+        path.append((x, y))
         n += a
-        if n > d: 
+        if n > d:
             n -= d
             x += xi1
             y += yi1
         x += xi2
         y += yi2
         c += 1
     return path
```

### Comparing `zanthor-1.2.3/zanthor/tiles.py` & `zanthor-1.2.4a2/zanthor/tiles.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,117 +1,137 @@
 import pygame
-import sound_info
+from . import sound_info
+
 PRINTDEBUG = 0
 
 
-def tile_block(g,t,s):
+def tile_block(g, t, s):
     a = s
-    
+
     c = t.config
-    if (c['top'] == 1 and a._rect.bottom <= t._rect.top and a.rect.bottom > t.rect.top):
+    if c["top"] == 1 and a._rect.bottom <= t._rect.top and a.rect.bottom > t.rect.top:
         a.rect.bottom = t.rect.top
-    if (c['left'] == 1 and a._rect.right <= t._rect.left and a.rect.right > t.rect.left):
+    if c["left"] == 1 and a._rect.right <= t._rect.left and a.rect.right > t.rect.left:
         a.rect.right = t.rect.left
-    if (c['right'] == 1 and a._rect.left >= t._rect.right and a.rect.left < t.rect.right):
+    if c["right"] == 1 and a._rect.left >= t._rect.right and a.rect.left < t.rect.right:
         a.rect.left = t.rect.right
-    if (c['bottom'] == 1 and a._rect.top >= t._rect.bottom and a.rect.top < t.rect.bottom):
+    if (
+        c["bottom"] == 1
+        and a._rect.top >= t._rect.bottom
+        and a.rect.top < t.rect.bottom
+    ):
         a.rect.top = t.rect.bottom
 
 
 class WallBlast:
     def __init__(self):
-        import explode,steam
-        #self.e1 = explode.Effect(64,16)
-        #self.e2 = steam.Effect(128,32,24,0)
-        self.e2 = steam.Effect(120,40,16,0,(143,136,129))
-        
-    def loop(self,pos):
-        #self.e1.loop(pos)
+        from . import explode, steam
+
+        # self.e1 = explode.Effect(64,16)
+        # self.e2 = steam.Effect(128,32,24,0)
+        self.e2 = steam.Effect(120, 40, 16, 0, (143, 136, 129))
+
+    def loop(self, pos):
+        # self.e1.loop(pos)
         self.e2.loop(pos)
-        
-    def paint(self,screen,origin):
-        #self.e1.paint(screen,origin)
-        self.e2.paint(screen,origin)
-
-def tile_wall(g,t,s):
-    #when hit, this cracks
-    
-    if s not in g.sprites: return
+
+    def paint(self, screen, origin):
+        # self.e1.paint(screen,origin)
+        self.e2.paint(screen, origin)
+
+
+def tile_wall(g, t, s):
+    # when hit, this cracks
+
+    if s not in g.sprites:
+        return
     g.sprites.remove(s)
 
     g.level.game.sm.Play(sound_info.hitwall.nextone())
-        
-    tx,ty = t.tx,t.ty
-    for a,dx,dy in [(2,0,0),(1,-1,0),(1,1,0),(1,0,1),(1,0,-1)]:
-        v = g.get((tx+dx,ty+dy))
-        if v in (4,5,6):
-            v = min(7,v + a)
-            g.set((tx+dx,ty+dy),v)
-            
-    import effect
-    tw,th = g.iso_w,g.iso_h
-    e = effect.effect_new(g,pygame.Rect(t.tx*tw+tw/2,t.ty*th+th/2,1,1),WallBlast(),20)
-    e.z = s.z+16
-    
 
-def tile_coal(g,t,s):
-    #print 'you hit coal'
+    tx, ty = t.tx, t.ty
+    for a, dx, dy in [(2, 0, 0), (1, -1, 0), (1, 1, 0), (1, 0, 1), (1, 0, -1)]:
+        v = g.get((tx + dx, ty + dy))
+        if v in (4, 5, 6):
+            v = min(7, v + a)
+            g.set((tx + dx, ty + dy), v)
+
+    from . import effect
+
+    tw, th = g.iso_w, g.iso_h
+    e = effect.effect_new(
+        g, pygame.Rect(t.tx * tw + tw / 2, t.ty * th + th / 2, 1, 1), WallBlast(), 20
+    )
+    e.z = s.z + 16
+
+
+def tile_coal(g, t, s):
+    # print 'you hit coal'
     pass
 
     g.level.game.sm.Play(sound_info.coal.nextone())
 
     s.check_for_pickup(g, t)
 
 
-def tile_water(g,t,s):
-    #print 'you hit water'
+def tile_water(g, t, s):
+    # print 'you hit water'
     pass
     g.level.game.sm.Play(sound_info.water.nextone())
 
     s.check_for_pickup(g, t)
 
-def tile_rubble(g,t,s):
-    print 'you hit rubble'
+
+def tile_rubble(g, t, s):
+    print("you hit rubble")
 
     s.check_for_pickup(g, t)
 
-def tile_part(g,t,s):
-    #print "*"*30
-    #print type(s)
-    #print s
-    #print g
-    if PRINTDEBUG: print "generic tile part"
+
+def tile_part(g, t, s):
+    # print "*"*30
+    # print type(s)
+    # print s
+    # print g
+    if PRINTDEBUG:
+        print("generic tile part")
     s.check_for_pickup(g, t)
 
-def tile_cannon(g,t,s):
-    if PRINTDEBUG: print "you hit cannon part"
+
+def tile_cannon(g, t, s):
+    if PRINTDEBUG:
+        print("you hit cannon part")
     s.check_for_pickup(g, t)
 
-def tile_engine(g,t,s):
-    if PRINTDEBUG: print "you hit engine part"
+
+def tile_engine(g, t, s):
+    if PRINTDEBUG:
+        print("you hit engine part")
     s.check_for_pickup(g, t)
 
-def tile_watertank(g,t,s):
-    if PRINTDEBUG: print "you hit watertank part"
+
+def tile_watertank(g, t, s):
+    if PRINTDEBUG:
+        print("you hit watertank part")
     s.check_for_pickup(g, t)
 
-def tile_coalstorageroom(g,t,s):
-    if PRINTDEBUG: print "you hit coalstorageroom part"
+
+def tile_coalstorageroom(g, t, s):
+    if PRINTDEBUG:
+        print("you hit coalstorageroom part")
     s.check_for_pickup(g, t)
 
-def tile_armour(g,t,s):
-    if PRINTDEBUG: print "you hit armour part"
+
+def tile_armour(g, t, s):
+    if PRINTDEBUG:
+        print("you hit armour part")
     s.check_for_pickup(g, t)
 
 
-def tile_limit(g,t,s):
-    print s,'out of bounds'
+def tile_limit(g, t, s):
+    print((s, "out of bounds"))
     if s in g.sprites:
         g.sprites.remove(s)
-    #HACK
+    # HACK
     if s in g.robots:
-        g.robots.remove(s) 
-    s.state = 'dead'
-
-
-
-
+        g.robots.remove(s)
+    s.state = "dead"
```

### Comparing `zanthor-1.2.3/zanthor/isovid.py` & `zanthor-1.2.4a2/zanthor/isovid.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,474 +4,465 @@
 particular needs.  If you are able to update it, help would be 
 greatly appreciated!</p>
 
 <p>please note that this file is alpha, and is subject to modification in
 future versions of pgu!</p>
 
 """
-print 'pgu.isovid','This module is alpha, and is subject to change.'
+print(("pgu.isovid", "This module is alpha, and is subject to change."))
 
-from pgu.vid import *
+from .pgu.vid import *
 import pygame
 import random
 
 import time, os
-from const import data_dir
+from .const import data_dir
 
 try:
-    import const
+    from . import const
+
     CACHE_USE_LEVEL_CACHE = const.CACHE_USE_LEVEL_CACHE
 except:
     CACHE_USE_LEVEL_CACHE = 0
 
 
 class Isovid(Vid):
     """Create an iso vid engine.  See [[vid]]"""
-    def update(self,screen):
+
+    def update(self, screen):
         return self.paint(screen)
-    
-    def bkgr_blit(self,img,pos):
-        #pos must be an iso coordinate, centered
-        
+
+    def bkgr_blit(self, img, pos):
+        # pos must be an iso coordinate, centered
+
         tlayer = self.tlayer
-        w,h = len(tlayer[0]),len(tlayer)
-        
-        tmp,y1 = self.tile_to_view((0,0))
-        x1,tmp = self.tile_to_view((0,h+1))
-        tmp,y2 = self.tile_to_view((w+1,h+1))
-        x2,tmp = self.tile_to_view((w+1,0))
-        
+        w, h = len(tlayer[0]), len(tlayer)
+
+        tmp, y1 = self.tile_to_view((0, 0))
+        x1, tmp = self.tile_to_view((0, h + 1))
+        tmp, y2 = self.tile_to_view((w + 1, h + 1))
+        x2, tmp = self.tile_to_view((w + 1, 0))
+
         pos = self.iso_to_view(pos)
-        
-        dest = (-x1+pos[0]-img.get_width()/2,-y1+pos[1]-img.get_height()/2)
-        print dest
-        self.bkgr.blit(img,dest)
-        
+
+        dest = (-x1 + pos[0] - img.get_width() // 2, -y1 + pos[1] - img.get_height() // 2)
+        print(dest)
+        self.bkgr.blit(img, dest)
 
     def load_bkgr_cache(self, level_fname, tiles_fname):
-        """ try and load the painted background from cache.
-            Returns True if it can load the background.  Otherwise False.
+        """try and load the painted background from cache.
+        Returns True if it can load the background.  Otherwise False.
         """
 
         if not CACHE_USE_LEVEL_CACHE:
             return False
 
-        #try:
+        # try:
         # check if the image is in cache.
         exts = [".jpg", ".tga"]
         found_image = False
 
         for ext in exts:
-            cached_fname = data_dir('cache', 'levels', os.path.basename(level_fname))
+            cached_fname = data_dir("cache", "levels", os.path.basename(level_fname))
             cached_fname = cached_fname[:-4] + ext
 
             if os.path.exists(cached_fname):
                 # check if the cached file is newer.
                 fname_stat = os.stat(level_fname)
-                cached_stat = os.stat( cached_fname )
+                cached_stat = os.stat(cached_fname)
                 if fname_stat.st_mtime > cached_stat.st_mtime:
                     return False
                 found_image = True
                 break
-                #TODO: check the tiles mtime too.
+                # TODO: check the tiles mtime too.
 
         if found_image:
-            print "loading :%s:" % cached_fname
+            print(("loading :%s:" % cached_fname))
             self.bkgr = pygame.image.load(cached_fname)
             self.bkgr = self.bkgr.convert()
             return True
         else:
             return False
 
-
-
         # check if the cached image is newer than the level tga, and the tile tga.
 
         # if it is valid in cache, load to the background.
 
+    def paint(self, screen):
+        sw, sh = screen.get_width(), screen.get_height()
 
-
-
-
-
-    def paint(self,screen):
-        
-        sw,sh = screen.get_width(),screen.get_height()
-        
         tlayer = self.tlayer
         blayer = self.blayer
         zlayer = self.zlayer
-        
-        w,h = len(tlayer[0]),len(tlayer)
-        if not hasattr(self,'bkgr') and not self.load_bkgr_cache(self.level_fname, self.tiles_fname):
+
+        w, h = len(tlayer[0]), len(tlayer)
+        if not hasattr(self, "bkgr") and not self.load_bkgr_cache(
+            self.level_fname, self.tiles_fname
+        ):
             t1 = time.time()
 
             self.bkgr = None
             v = self.view
-            tmp,y1 = self.tile_to_view((0,0))
-            x1,tmp = self.tile_to_view((0,h+1))
-            tmp,y2 = self.tile_to_view((w+1,h+1))
-            x2,tmp = self.tile_to_view((w+1,0))
-
-            ww,hh = x2-x1,y2-y1
-            self.view = pygame.Rect(x1,y1,ww,hh)
-            s = pygame.Surface((ww,hh)).convert()
-            s.fill((128,0,0))
+            tmp, y1 = self.tile_to_view((0, 0))
+            x1, tmp = self.tile_to_view((0, h + 1))
+            tmp, y2 = self.tile_to_view((w + 1, h + 1))
+            x2, tmp = self.tile_to_view((w + 1, 0))
+
+            ww, hh = x2 - x1, y2 - y1
+            self.view = pygame.Rect(x1, y1, ww, hh)
+            s = pygame.Surface((ww, hh)).convert()
+            s.fill((128, 0, 0))
             self.paint(s)
-            
-            s2 = pygame.Surface((ww,hh)).convert()
-                
-            for n in [1,2]: #,4]:
-                s2.blit(s,(0,0))
+
+            s2 = pygame.Surface((ww, hh)).convert()
+
+            for n in [1, 2]:  # ,4]:
+                s2.blit(s, (0, 0))
                 s.set_alpha(48)
-                for x,y in [(-16/n,0),(16/n,0),(0,-8/n),(0,8/n)]:
-                    s2.blit(s,(x+random.randrange(-2,3),y+random.randrange(-2,3)))
+                for x, y in [(-16 // n, 0), (16 // n, 0), (0, -8 // n), (0, 8 // n)]:
+                    s2.blit(
+                        s, (x + random.randrange(-2, 3), y + random.randrange(-2, 3))
+                    )
                 s.set_alpha(255)
-                s2,s = s,s2
-                
+                s2, s = s, s2
 
             self.bkgr = s
             t2 = time.time()
-            print "_" * 40
-            print "time to paint background: %s" % (t2 - t1)
-
+            print(("_" * 40))
+            print(("time to paint background: %s" % (t2 - t1)))
 
             # this is the caching stuff.
             if CACHE_USE_LEVEL_CACHE:
                 if t2 - t1 > 1.0:
                     # the machine didn't process this fast enough, so we cache it.
-                    if not os.path.exists(data_dir('cache')):
-                        os.mkdir(data_dir('cache'))
-                        if not os.path.exists(data_dir('cache', 'levels')):
-                            os.mkdir(data_dir('cache', 'levels'))
+                    if not os.path.exists(data_dir("cache")):
+                        os.mkdir(data_dir("cache"))
+                        if not os.path.exists(data_dir("cache", "levels")):
+                            os.mkdir(data_dir("cache", "levels"))
 
                     try:
-                        cached_fname = data_dir('cache', 'levels', os.path.basename(self.level_fname))
+                        cached_fname = data_dir(
+                            "cache", "levels", os.path.basename(self.level_fname)
+                        )
                         pygame.image.save(self.bkgr, cached_fname)
                     except:
                         pass
                         # no cache for this person.  Maybe no permission.
 
+        iso_w, iso_h, iso_z, tile_w, tile_h, base_w, base_h = (
+            self.iso_w,
+            self.iso_h,
+            self.iso_z,
+            self.tile_w,
+            self.tile_h,
+            self.base_w,
+            self.base_h,
+        )
+
+        base_h2 = base_h // 2
+        base_w2 = base_w // 2
+
+        bot = tile_h // base_h2
+        todo_max = sh // base_h2 + bot
+        # todo = [[] for y in xrange(0,todo_max)]
+        todo = {}
 
+        self.view.w, self.view.h = sw, sh
+        view = self.view
+        adj = self.adj = pygame.Rect(-self.view.x, -self.view.y, 0, 0)
 
+        shift = pygame.Rect(adj.x, adj.y // base_h2 * base_h2, 0, 0)
 
-        iso_w,iso_h,iso_z,tile_w,tile_h,base_w,base_h = self.iso_w,self.iso_h,self.iso_z,self.tile_w,self.tile_h,self.base_w,self.base_h
-        
-        base_h2 = base_h/2
-        base_w2 = base_w/2
-        
-        bot = tile_h/base_h2
-        todo_max = sh/base_h2+bot
-        #todo = [[] for y in xrange(0,todo_max)]
-        todo = {}
-        
-        self.view.w,self.view.h = sw,sh
-        view = self.view
-        adj = self.adj = pygame.Rect(-self.view.x,-self.view.y,0,0)
-        
-        shift = pygame.Rect(adj.x,adj.y/base_h2*base_h2,0,0)
-        
         for s in self.sprites:
             self.sprite_calc_irect(s)
-            
+
             if s.irect.colliderect(self.view):
-                x,y = self.iso_to_view((s.rect.centerx,s.rect.centery))
-                #v = (y+adj.y)/base_h2 - 1
-                #v = (y+shift.y)/base_h2 -1
-                #if v >= 0 and v < todo_max:
+                x, y = self.iso_to_view((s.rect.centerx, s.rect.centery))
+                # v = (y+adj.y)/base_h2 - 1
+                # v = (y+shift.y)/base_h2 -1
+                # if v >= 0 and v < todo_max:
                 #    todo[v].append((s,s.image,s.irect))
-                v = y/base_h2 -1
-                if v not in todo: todo[v] = []
-                todo[v].append((s,s.image,s.irect))
-                
-                if hasattr(s,'effect'):
+                v = y // base_h2 - 1
+                if v not in todo:
+                    todo[v] = []
+                todo[v].append((s, s.image, s.irect))
+
+                if hasattr(s, "effect"):
                     e = s.effect
-                    if hasattr(e,'zloop'):
+                    if hasattr(e, "zloop"):
                         z = 0
-                        if hasattr(s,'z'):
+                        if hasattr(s, "z"):
                             z = s.z
-                        
-                        irect= s.irect
-                        e.zloop((s.irect.x+irect.w/2,s.irect.y+irect.h/2+z),v)
-                        
-                        for z,img,pos in e.zpaint():
-                            if z not in todo: todo[z] = []
-                            todo[z].append((None,img,pygame.Rect(pos[0],pos[1],1,1)))
-                            
-                    
-            
-            #else: print 'doesnt fit',v
-                
-        w,h = len(tlayer[0]),len(tlayer)
+
+                        irect = s.irect
+                        e.zloop(
+                            (s.irect.x + irect.w // 2, s.irect.y + irect.h // 2 + z), v
+                        )
+
+                        for z, img, pos in e.zpaint():
+                            if z not in todo:
+                                todo[z] = []
+                            todo[z].append(
+                                (None, img, pygame.Rect(pos[0], pos[1], 1, 1))
+                            )
+
+            # else: print 'doesnt fit',v
+
+        w, h = len(tlayer[0]), len(tlayer)
         tiles = self.tiles
-        
+
         if self.bkgr != None:
-            #""
+            # ""
             if self.bounds == None:
-                tmp,y1 = self.tile_to_view((0,0))
-                x1,tmp = self.tile_to_view((0,h+1))
-                tmp,y2 = self.tile_to_view((w+1,h+1))
-                x2,tmp = self.tile_to_view((w+1,0))
-                self.bounds = pygame.Rect(x1,y1,x2-x1,y2-y1)
-            #""
-            
-            if self.bounds != None: self.view.clamp_ip(self.bounds)
-            #print self.bounds
-
-        ox,oy = self.screen_to_tile((0,0))
-        sx,sy = self.iso_to_view((ox*iso_w,oy*iso_h))
-        dx,dy = sx - self.view.x,sy - self.view.y
-        
-        
+                tmp, y1 = self.tile_to_view((0, 0))
+                x1, tmp = self.tile_to_view((0, h + 1))
+                tmp, y2 = self.tile_to_view((w + 1, h + 1))
+                x2, tmp = self.tile_to_view((w + 1, 0))
+                self.bounds = pygame.Rect(x1, y1, x2 - x1, y2 - y1)
+            # ""
+
+            if self.bounds != None:
+                self.view.clamp_ip(self.bounds)
+            # print self.bounds
+
+        ox, oy = self.screen_to_tile((0, 0))
+        sx, sy = self.iso_to_view((ox * iso_w, oy * iso_h))
+        dx, dy = sx - self.view.x, sy - self.view.y
+
         if self.bkgr == None:
-            print 'paint the background!!!'
+            print("paint the background!!!")
             t1 = time.time()
 
-            for i2 in xrange(-bot,self.view.h/base_h2+bot):
-                tx,ty = ox + i2/2 + i2%2,oy + i2/2
-                x,y = (i2%2)*base_w2 + dx,i2*base_h2 + dy
-                
-                #to adjust for the -1 in i1
-                x,tx,ty = x-base_w,tx-1,ty+1
-                for i1 in xrange(-1,self.view.w/base_w+2): #NOTE: not sure why +2
-                    #print tx,ty
+            for i2 in range(-bot, self.view.h // base_h2 + bot):
+                tx, ty = ox + i2 // 2 + i2 % 2, oy + i2 // 2
+                x, y = (i2 % 2) * base_w2 + dx, i2 * base_h2 + dy
+
+                # to adjust for the -1 in i1
+                x, tx, ty = x - base_w, tx - 1, ty + 1
+                for i1 in range(-1, self.view.w // base_w + 2):  # NOTE: not sure why +2
+                    # print tx,ty
                     if ty >= 0 and ty < h and tx >= 0 and tx < w:
-                        z = zlayer[ty][tx]*iso_z
+                        z = zlayer[ty][tx] * iso_z
                         if blayer != None:
                             n = blayer[ty][tx]
                             if n != 0:
-                                t = tiles[n]
+                                t = tiles[int(n)]
                                 if t != None and t.image != None:
-                                    screen.blit(t.image,(x-base_w2,y+z))
-                                    
-                                    
+                                    screen.blit(t.image, (x - base_w2, y + z))
+
                     tx += 1
                     ty -= 1
                     x += base_w
 
             t2 = time.time()
-            print "*" * 40
-            print "time to paint background: %s" % (t2 - t1)
+            print(("*" * 40))
+            print(("time to paint background: %s" % (t2 - t1)))
 
             return
-        
-        tmp,y1 = self.tile_to_view((0,0))
-        x1,tmp = self.tile_to_view((0,h+1))
-        tmp,y2 = self.tile_to_view((w+1,h+1))
-        x2,tmp = self.tile_to_view((w+1,0))
-        
-        #print x1,y1,adj
-        screen.blit(self.bkgr,(x1+adj.x,y1+adj.y))
-        
-        
-        for i2 in xrange(-bot,self.view.h/base_h2+bot):
-            tx,ty = ox + i2/2 + i2%2,oy + i2/2
-            x,y = (i2%2)*base_w2 + dx,i2*base_h2 + dy
-            
-            #to adjust for the -1 in i1
-            x,tx,ty = x-base_w,tx-1,ty+1
-            for i1 in xrange(-1,self.view.w/base_w+2): #NOTE: not sure why +2
+
+        tmp, y1 = self.tile_to_view((0, 0))
+        x1, tmp = self.tile_to_view((0, h + 1))
+        tmp, y2 = self.tile_to_view((w + 1, h + 1))
+        x2, tmp = self.tile_to_view((w + 1, 0))
+
+        # print x1,y1,adj
+        screen.blit(self.bkgr, (x1 + adj.x, y1 + adj.y))
+
+        for i2 in range(-bot, self.view.h // base_h2 + bot):
+            tx, ty = ox + i2 // 2 + i2 % 2, oy + i2 // 2
+            x, y = (i2 % 2) * base_w2 + dx, i2 * base_h2 + dy
+
+            # to adjust for the -1 in i1
+            x, tx, ty = x - base_w, tx - 1, ty + 1
+            for i1 in range(-1, self.view.w // base_w + 2):  # NOTE: not sure why +2
                 if ty >= 0 and ty < h and tx >= 0 and tx < w:
-                    z = zlayer[ty][tx]*iso_z
-#                     if blayer != None:
-#                         n = blayer[ty][tx]
-#                         if n != 0:
-#                             t = tiles[n]
-#                             if t != None and t.image != None:
-#                                 screen.blit(t.image,(x-base_w2,y+z))
+                    z = zlayer[ty][tx] * iso_z
+                    #                     if blayer != None:
+                    #                         n = blayer[ty][tx]
+                    #                         if n != 0:
+                    #                             t = tiles[n]
+                    #                             if t != None and t.image != None:
+                    #                                 screen.blit(t.image,(x-base_w2,y+z))
                     n = tlayer[ty][tx]
                     if n != 0:
                         t = tiles[n]
                         if t != None and t.image != None:
-                            screen.blit(t.image,(x-base_w2,y-(t.image_h-base_h)+z))
-            
+                            screen.blit(
+                                t.image, (x - base_w2, y - (t.image_h - base_h) + z)
+                            )
+
                 tx += 1
                 ty -= 1
                 x += base_w
-            #for s,img,irect in todo[y/base_h2]:
-            #if i2 in todo:
-            
-            zz = (y - adj.y) / base_h2
-            if zz not in todo: continue
-            for s,img,irect in todo[zz]:
+            # for s,img,irect in todo[y/base_h2]:
+            # if i2 in todo:
+
+            zz = (y - adj.y) // base_h2
+            if zz not in todo:
+                continue
+            for s, img, irect in todo[zz]:
                 z = 0
-                if hasattr(s,'z'):
+                if hasattr(s, "z"):
                     z = s.z
-                screen.blit(img,(irect.x+adj.x,irect.y+adj.y+z))
-                if hasattr(s,'effect'):
-                    if not hasattr(s.effect,'zloop'):
-                        s.effect.loop((s.irect.x+irect.w/2,s.irect.y+irect.h/2+z))
-                        s.effect.paint(screen,(-adj.x,-adj.y))#(irect.x+adj.x+irect.w/2,irect.y+adj.y+irect.h/2))
+                screen.blit(img, (irect.x + adj.x, irect.y + adj.y + z))
+                if hasattr(s, "effect"):
+                    if not hasattr(s.effect, "zloop"):
+                        s.effect.loop(
+                            (s.irect.x + irect.w // 2, s.irect.y + irect.h // 2 + z)
+                        )
+                        s.effect.paint(
+                            screen, (-adj.x, -adj.y)
+                        )  # (irect.x+adj.x+irect.w/2,irect.y+adj.y+irect.h/2))
 
         self.updates = []
-        return [pygame.Rect(0,0,screen.get_width(),screen.get_height())]
-        
-    def iso_to_view(self,pos):
+        return [pygame.Rect(0, 0, screen.get_width(), screen.get_height())]
+
+    def iso_to_view(self, pos):
         tlayer = self.tlayer
-        w,h = len(tlayer[0]),len(tlayer)
-        
-        x,y = pos
-        
-        #nx,ny = (h*self.iso_w + x - y)/2, (0 + x + y)/2
-        nx,ny = (x - y)/2, (0 + x + y)/2
-        
-        return (nx * self.base_w / self.iso_w), (ny * self.base_h / self.iso_h)
+        w, h = len(tlayer[0]), len(tlayer)
+
+        x, y = pos
+
+        # nx,ny = (h*self.iso_w + x - y)/2, (0 + x + y)/2
+        nx, ny = (x - y) // 2, (0 + x + y) // 2
+
+        return (nx * self.base_w // self.iso_w), (ny * self.base_h // self.iso_h)
 
-    def view_to_iso(self,pos):
+    def view_to_iso(self, pos):
         tlayer = self.tlayer
-        w,h = len(tlayer[0]),len(tlayer)
-        
-        x,y = pos
-        
-        x,y = x*self.iso_w/self.base_w, y*self.iso_h/self.base_h
-        
-        #x -= (self.iso_w/2) * h
-        #x -= (self.iso_w/2) * h
-        
-        nx = (x+y) 
-        ny = y*2-nx
-    
-        return nx,ny
-    
-    def tile_to_view(self,pos):
-        return self.iso_to_view((pos[0]*self.iso_w,pos[1]*self.iso_h))
-    
-    def screen_to_tile(self,pos):
-        x,y = pos
+        w, h = len(tlayer[0]), len(tlayer)
+
+        x, y = pos
+
+        x, y = x * self.iso_w // self.base_w, y * self.iso_h // self.base_h
+
+        # x -= (self.iso_w/2) * h
+        # x -= (self.iso_w/2) * h
+
+        nx = x + y
+        ny = y * 2 - nx
+
+        return nx, ny
+
+    def tile_to_view(self, pos):
+        return self.iso_to_view((pos[0] * self.iso_w, pos[1] * self.iso_h))
+
+    def screen_to_tile(self, pos):
+        x, y = pos
         x += self.view.x
         y += self.view.y
-        x,y = self.view_to_iso((x,y))
-        return x/self.iso_w,y/self.iso_h
-        
-    def tile_to_screen(self,pos):
-        x,y = self.iso_to_view((pos[0]*self.iso_w,pos[1]*self.iso_h))
-        return x-self.view.x,y-self.view.y
-    
-    def tga_load_tiles(self,fname,size,tdata={}):
-        Vid.tga_load_tiles(self,fname,size,tdata)
-        
-        self.tile_w,self.tile_h = size
-        self.iso_w,self.iso_h,self.iso_z = self.tile_w,self.tile_w,1
-        self.base_w,self.base_h = self.tile_w,self.tile_w/2
+        x, y = self.view_to_iso((x, y))
+        return x // self.iso_w, y // self.iso_h
+
+    def tile_to_screen(self, pos):
+        x, y = self.iso_to_view((pos[0] * self.iso_w, pos[1] * self.iso_h))
+        return x - self.view.x, y - self.view.y
+
+    def tga_load_tiles(self, fname, size, tdata={}):
+        Vid.tga_load_tiles(self, fname, size, tdata)
+
+        self.tile_w, self.tile_h = size
+        self.iso_w, self.iso_h, self.iso_z = self.tile_w, self.tile_w, 1
+        self.base_w, self.base_h = self.tile_w, self.tile_w // 2
 
         self.tiles_fname = fname
-    
 
-    def tga_load_level(self,fname,bg=0):
-        """Load a TGA level.  
-        
+    def tga_load_level(self, fname, bg=0):
+        """Load a TGA level.
+
         <pre>Vid.tga_load_level(fname,bg=0)</pre>
-        
+
         <dl>
         <dt>g        <dd>a Tilevid instance
         <dt>fname    <dd>tga image to load
         <dt>bg        <dd>set to 1 if you wish to load the background layer
         </dl>
         """
 
-        if type(fname) == str: 
-            img = pygame.image.load(fname)
+        if type(fname) == str:
+            try:
+                img = pygame.image.load(fname)
+            except:
+                print(fname)
+                img = pygame.image.load(fname.replace("tga", "png"))
+
             self.level_fname = fname
-        else: 
+        else:
             img = fname
             self.level_fname = repr(fname)
 
-        w,h = img.get_width(),img.get_height()
+        w, h = img.get_width(), img.get_height()
         pad = 12
-        self.resize((w+pad*2,h+pad*2),bg)
-        w,h = self.size
-        for y in range(0,h):
-            for x in range(0,w):
-                self.tlayer[y][x] = 0x1c
-        w,h = img.get_width(),img.get_height()
-        for y in range(0,h):
-            for x in range(0,w):
-                t,b,c,_a = img.get_at((x,y))
-                self.tlayer[y+pad][x+pad] = t
-                if bg: self.blayer[y+pad][x+pad] = b
-                self.clayer[y+pad][x+pad] = c
-                
-     
-    def resize(self,size,bg=0):
-        Vid.resize(self,size,bg)
-        
-        tlayer = self.tlayer
-        w,h = len(tlayer[0]),len(tlayer)
-        
-        self.zlayer = [[0 for x in xrange(0,w)] for y in xrange(0,h)]
+        self.resize((w + pad * 2, h + pad * 2), bg)
+        w, h = self.size
+        for y in range(0, h):
+            for x in range(0, w):
+                self.tlayer[y][x] = 0x1C
+        w, h = img.get_width(), img.get_height()
+        for y in range(0, h):
+            for x in range(0, w):
+                t, b, c, _a = img.get_at((x, y))
+                self.tlayer[y + pad][x + pad] = t
+                if bg:
+                    self.blayer[y + pad][x + pad] = b
+                self.clayer[y + pad][x + pad] = c
+
+    def resize(self, size, bg=0):
+        Vid.resize(self, size, bg)
 
-        
+        tlayer = self.tlayer
+        w, h = len(tlayer[0]), len(tlayer)
 
+        self.zlayer = [[0 for x in range(0, w)] for y in range(0, h)]
 
-    def sprite_calc_irect(self,s):
+    def sprite_calc_irect(self, s):
         tlayer = self.tlayer
-        w,h = len(tlayer[0]),len(tlayer)
+        w, h = len(tlayer[0]), len(tlayer)
         zlayer = self.zlayer
-        
-        x,y = self.iso_to_view((s.rect.centerx,s.rect.centery))
-        tx,ty = s.rect.centerx/self.iso_w,s.rect.centery/self.iso_h
+
+        x, y = self.iso_to_view((s.rect.centerx, s.rect.centery))
+        tx, ty = s.rect.centerx // self.iso_w, s.rect.centery // self.iso_h
         z = 0
         if ty >= 0 and ty < h and tx >= 0 and tx < w:
-            z = zlayer[ty][tx]*self.iso_z
-        
-        nx,ny = x - s.shape.centerx, y - s.shape.centery + z
-        
-        s.irect.x,s.irect.y = nx,ny
-        
-        
-        
-    def run_codes(self,cdata,rect):
-        #HACK to make run_codes work
-        w,h = self.iso_w,self.iso_h
-         
+            z = zlayer[ty][tx] * self.iso_z
+
+        nx, ny = x - s.shape.centerx, y - s.shape.centery + z
+
+        s.irect.x, s.irect.y = nx, ny
+
+    def run_codes(self, cdata, rect):
+        # HACK to make run_codes work
+        w, h = self.iso_w, self.iso_h
+
         img = self.tiles[0].image
-        
-        self.tiles[0].image = pygame.Surface((w,h))
-        r = Vid.run_codes(self,cdata,rect)
+
+        self.tiles[0].image = pygame.Surface((w, h))
+        r = Vid.run_codes(self, cdata, rect)
         self.tiles[0].image = img
         return r
-        
-        
-    def set(self,pos,v):
+
+    def set(self, pos, v):
         """Set a tile in the foreground to a value.
-        
+
         <p>Use this method to set tiles in the foreground, as it will make
         sure the screen is updated with the change.  Directly changing
         the tlayer will not guarantee updates unless you are using .paint()
         </p>
-        
+
         <pre>Vid.set(pos,v)</pre>
-        
+
         <dl>
         <dt>pos <dd>(x,y) of tile
         <dt>v <dd>value
         </dl>
         """
-        
-        #if self.tlayer[pos[1]][pos[0]] == v: return
+
+        # if self.tlayer[pos[1]][pos[0]] == v: return
         self.tlayer[pos[1]][pos[0]] = v
-        #self.alayer[pos[1]][pos[0]] = 1
-        
-        #self.robot_layer[pos[1]][pos[0]] = int(v!=0)
-        self.robot_layer[pos[1]][pos[0]] = int(v in (3,4,5,6,30))
-        self.truck_layer[pos[1]][pos[0]] = int(v>1)
-        self.castle_layer[pos[1]][pos[0]] = int(v in (3,4,5,6,30))
-        
-        #self.updates.append(pos)
-        
-        
-
-
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
+        # self.alayer[pos[1]][pos[0]] = 1
+
+        # self.robot_layer[pos[1]][pos[0]] = int(v!=0)
+        self.robot_layer[pos[1]][pos[0]] = int(v in (3, 4, 5, 6, 30))
+        self.truck_layer[pos[1]][pos[0]] = int(v > 1)
+        self.castle_layer[pos[1]][pos[0]] = int(v in (3, 4, 5, 6, 30))
+
+        # self.updates.append(pos)
```

### Comparing `zanthor-1.2.3/zanthor/flock.py` & `zanthor-1.2.4a2/zanthor/flock.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,197 +1,212 @@
 import pygame
 from pygame.locals import *
 import random
 
-from pgu import timer
+from .pgu import timer
 
 rr = random.randrange
 
+
 class Part:
-    def __init__(self,x,y):
-        x,y = float(x),float(y)
-        self.x,self.y = x,y
-        self._x,self._y = x,y
+    def __init__(self, x, y):
+        x, y = float(x), float(y)
+        self.x, self.y = x, y
+        self._x, self._y = x, y
         self.min = 4.0
         self.max = 16.0
         self.radius = 16.0
         self.center = 2.0
         self.search = 64.0
         self._flock_frame = 0
         self.near = []
-        
+
+
 class Flock:
-    def __init__(self,rect,spacing):
-        self.rect,self.spacing = rect,spacing
-        self.grid = [[[] for tx in xrange(rect.left,rect.right,spacing)] for ty in xrange(rect.top,rect.bottom,spacing)]
+    def __init__(self, rect, spacing):
+        self.rect, self.spacing = rect, spacing
+        self.grid = [
+            [[] for tx in range(rect.left, rect.right, spacing)]
+            for ty in range(rect.top, rect.bottom, spacing)
+        ]
         self.parts = []
-    
-    def append(self,p):
-        rect,spacing,grid,parts = self.rect,self.spacing,self.grid,self.parts
+
+    def append(self, p):
+        rect, spacing, grid, parts = self.rect, self.spacing, self.grid, self.parts
         self.parts.append(p)
-        tx,ty = p._tx,p._ty = int((p.x-rect.left)/spacing),int((p.y-rect.top)/spacing)
-        p.vx,p.vy = 0,0
+        tx, ty = p._tx, p._ty = int((p.x - rect.left) / spacing), int(
+            (p.y - rect.top) / spacing
+        )
+        p.vx, p.vy = 0, 0
         grid[ty][tx].append(p)
-        
-    def remove(self,p):
-        rect,spacing,grid,parts = self.rect,self.spacing,self.grid,self.parts
-        tx,ty = p._tx,p._ty
+
+    def remove(self, p):
+        rect, spacing, grid, parts = self.rect, self.spacing, self.grid, self.parts
+        tx, ty = p._tx, p._ty
         grid[ty][tx].remove(p)
         parts.remove(p)
-        
-        
+
     def __len__(self):
         return self.parts.__len__()
-    
+
     def __iter__(self):
         return self.parts.__iter__()
-        
+
     def loop(self):
-        rect,spacing,grid,parts = self.rect,self.spacing,self.grid,self.parts
-        gw,gh = len(grid[0]),len(grid)
-        
-        #update grid
+        rect, spacing, grid, parts = self.rect, self.spacing, self.grid, self.parts
+        gw, gh = len(grid[0]), len(grid)
+
+        # update grid
         for p in parts:
-            tx,ty = p._tx,p._ty
+            tx, ty = p._tx, p._ty
             grid[ty][tx].remove(p)
-            tx,ty = p._tx,p._ty = int((p.x-rect.left)/spacing),int((p.y-rect.top)/spacing)
+            tx, ty = p._tx, p._ty = int((p.x - rect.left) / spacing), int(
+                (p.y - rect.top) / spacing
+            )
             grid[ty][tx].append(p)
 
-        #calculate velocities
+        # calculate velocities
         for p in parts:
-            p.vx,p.vy = p.x-p._x,p.y-p._y
-            p._x,p._y = p.x,p.y
-            
-        #calculate neighbors
+            p.vx, p.vy = p.x - p._x, p.y - p._y
+            p._x, p._y = p.x, p.y
+
+        # calculate neighbors
         for p in parts:
-            tx,ty = p._tx,p._ty
-            
+            tx, ty = p._tx, p._ty
+
             p.near = []
-            for dy in (-1,0,1):
-                for dx in (-1,0,1):
-                    xx,yy = tx+dx,ty+dy
-                    if xx < 0 or yy < 0 or xx >= gw or yy >= gh: continue
+            for dy in (-1, 0, 1):
+                for dx in (-1, 0, 1):
+                    xx, yy = tx + dx, ty + dy
+                    if xx < 0 or yy < 0 or xx >= gw or yy >= gh:
+                        continue
                     p.near.extend(grid[yy][xx])
             p.near.remove(p)
-            
-            p.ax,p.ay = p.x,p.y
-            p.avx,p.avy = p.vx,p.vy
-    
+
+            p.ax, p.ay = p.x, p.y
+            p.avx, p.avy = p.vx, p.vy
+
             for _p in p.near:
                 p.ax += _p.x
                 p.ay += _p.y
                 p.avx += _p.vx
                 p.avy += _p.vy
-                
-            total = len(p.near)+1
+
+            total = len(p.near) + 1
             p.ax /= total
             p.ay /= total
             p.avx /= total
             p.avy /= total
-                    
-        #add average velocity to item
+
+        # add average velocity to item
         for p in parts:
-            p.x,p.y = p.x+p.avx,p.y+p.avy
-            
-        #move towards the center
+            p.x, p.y = p.x + p.avx, p.y + p.avy
+
+        # move towards the center
         for p in parts:
             step = p.center
-            ax,ay = p.ax,p.ay
-            dx,dy = ax-p.x,ay-p.y
-            dist = (dx*dx+dy*dy)**0.5
+            ax, ay = p.ax, p.ay
+            dx, dy = ax - p.x, ay - p.y
+            dist = (dx * dx + dy * dy) ** 0.5
             if dist > step:
-                p.x,p.y = p.x+step*dx/dist,p.y+step*dy/dist
+                p.x, p.y = p.x + step * dx / dist, p.y + step * dy / dist
 
-        #check min velocity
+        # check min velocity
         for p in parts:
             step = p.min
-            dx,dy = p.x-p._x,p.y-p._y
-            dist = (dx*dx+dy*dy)**0.5
+            dx, dy = p.x - p._x, p.y - p._y
+            dist = (dx * dx + dy * dy) ** 0.5
             while dist < 0.5:
-                dx,dy = random.randrange(-1,2),random.randrange(-1,2)
-                dist = (dx*dx+dy*dy)**0.5
+                dx, dy = random.randrange(-1, 2), random.randrange(-1, 2)
+                dist = (dx * dx + dy * dy) ** 0.5
             if dist < step:
-                p.x,p.y = p._x+dx*step/dist,p._y+dy*step/dist
-    
-        #keep away from neighbords
+                p.x, p.y = p._x + dx * step / dist, p._y + dy * step / dist
+
+        # keep away from neighbords
         for p in parts:
             for _p in p.near:
-                dx,dy = _p.x-p.x,_p.y-p.y
-                dist = (dx*dx+dy*dy)**0.5
-                r = p.radius+_p.radius
+                dx, dy = _p.x - p.x, _p.y - p.y
+                dist = (dx * dx + dy * dy) ** 0.5
+                r = p.radius + _p.radius
                 if dist < r:
-                    if dist == 0: dist,dx = 1,1
-                    inc = r/2.0
-                    mx,my = (p.x+_p.x)/2,(p.y+_p.y)/2
-                    p.x,p.y = mx - (inc*dx/dist), my - (inc*dy/dist)
-                    _p.x,_p.y = mx + (inc*dx/dist), my + (inc*dy/dist)
-                            
-        #check max velocity
+                    if dist == 0:
+                        dist, dx = 1, 1
+                    inc = r / 2.0
+                    mx, my = (p.x + _p.x) / 2, (p.y + _p.y) / 2
+                    p.x, p.y = mx - (inc * dx / dist), my - (inc * dy / dist)
+                    _p.x, _p.y = mx + (inc * dx / dist), my + (inc * dy / dist)
+
+        # check max velocity
         for p in parts:
             step = p.max
-            dx,dy = p.x-p._x,p.y-p._y
-            dist = (dx*dx+dy*dy)**0.5
+            dx, dy = p.x - p._x, p.y - p._y
+            dist = (dx * dx + dy * dy) ** 0.5
             if dist > step:
-                p.x,p.y = p._x+dx*step/dist,p._y+dy*step/dist
+                p.x, p.y = p._x + dx * step / dist, p._y + dy * step / dist
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     try:
-        #0/0 #HACK: so i can CTRL-c out
+        # 0/0 #HACK: so i can CTRL-c out
         import psyco
+
         psyco.profile()
-        print 'psyco installed'
+        print("psyco installed")
     except:
-        print 'psyco not installed'
+        print("psyco not installed")
 
+    SW, SH = 640, 480
+    screen = pygame.display.set_mode((SW, SH))
 
-    SW,SH = 640,480
-    screen = pygame.display.set_mode((SW,SH))
-    
     num = 256
     rad = 12
-    spacing = rad*3/2
-    border = spacing*2
-    myflock = Flock(pygame.Rect(-border,-border,SW+border*2,SH+border*2),spacing)
-    for n in xrange(0,num):
-        p = Part(rr(0,SW),rr(0,SH))
+    spacing = rad * 3 / 2
+    border = spacing * 2
+    myflock = Flock(
+        pygame.Rect(-border, -border, SW + border * 2, SH + border * 2), spacing
+    )
+    for n in range(0, num):
+        p = Part(rr(0, SW), rr(0, SH))
         p.radius = rad
         myflock.append(p)
-    
+
     t = timer.Speedometer()
     pygame.time.get_ticks()
-    
-    us = [(0,0,SW,SH)]
-    
+
+    us = [(0, 0, SW, SH)]
+
     _quit = False
     frames = 0
     while not _quit:
         for e in pygame.event.get():
-            if e.type is QUIT: _quit = True
-            if e.type is KEYDOWN and e.key == K_ESCAPE: _quit = True
-        
+            if e.type == QUIT:
+                _quit = True
+            if e.type == KEYDOWN and e.key == K_ESCAPE:
+                _quit = True
+
         for r in us:
-            screen.fill((0,0,0),r)
-        _us,us = us,[]
+            screen.fill((0, 0, 0), r)
+        _us, us = us, []
         us = []
 
-        p = myflock.parts[0] #HACK!!
-        p.x,p.y = pygame.mouse.get_pos()
+        p = myflock.parts[0]  # HACK!!
+        p.x, p.y = pygame.mouse.get_pos()
         p.radius = 64
-        x,y,r = int(p.x),int(p.y),int(p.radius)
-        pygame.draw.circle(screen,(0,0,128),(x,y),r)
-        us.append((x-r,y-r,r*2,r*2))
-        
+        x, y, r = int(p.x), int(p.y), int(p.radius)
+        pygame.draw.circle(screen, (0, 0, 128), (x, y), r)
+        us.append((x - r, y - r, r * 2, r * 2))
+
         myflock.loop()
-        
-        for p in myflock: #HACK!!
-            p.x = max(0,min(SW,p.x))
-            p.y = max(0,min(SH,p.y))
-            rect = int(p.x),int(p.y),4,4
-            screen.fill((255,255,255),rect)
+
+        for p in myflock:  # HACK!!
+            p.x = max(0, min(SW, p.x))
+            p.y = max(0, min(SH, p.y))
+            rect = int(p.x), int(p.y), 4, 4
+            screen.fill((255, 255, 255), rect)
             us.append(rect)
         pygame.display.update(_us)
         pygame.display.update(us)
-        
+
         r = t.tick()
-        if r: print r
+        if r:
+            print(r)
         frames += 1
-
```

### Comparing `zanthor-1.2.3/zanthor/const.py` & `zanthor-1.2.4a2/zanthor/const.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,164 +6,173 @@
 
 """
 
 
 import pygame
 
 import os
+
 _DATA_DIR = None
+
+
 def data_dir(*args):
     global _DATA_DIR
     if _DATA_DIR is None:
-        #_DATA_DIR = os.path.join(*(['zanthor', 'data'] + list(args)))
-        _DATA_DIR = os.path.join('zanthor', 'data')
+        # _DATA_DIR = os.path.join(*(['zanthor', 'data'] + list(args)))
+        _DATA_DIR = os.path.join("zanthor", "data")
         if not os.path.exists(_DATA_DIR):
-            _DATA_DIR = os.path.join(os.path.split(__file__)[0], 'data')
+            _DATA_DIR = os.path.join(os.path.split(__file__)[0], "data")
     return os.path.join(*([_DATA_DIR] + list(args)))
 
+
 # the base size.
-BSW,BSH = 640,480
-SW,SH = 640,480
-SW,SH = 320,200
-SW,SH = 800,600
-SW,SH = 1280,800
-SW,SH = 1024,768
+BSW, BSH = 640, 480
+SW, SH = 320, 200
+SW, SH = 800, 600
+SW, SH = 1280, 800
+SW, SH = 1024, 768
+SW, SH = 640, 480
 
 DX = float(SW) / BSW
 DY = float(SH) / BSH
 
 dxdy = (DX, DY)
 
 FPS = 30
 
 MIN_CANNON_PRESSURE = 6
 
-def multr(dx_dy, r):
-    a,b,c,d = tuple(r)
-    dx,dy = dxdy
-    return pygame.Rect(a*dx, b*dy, c*dx, d*dy)
-    
 
-#S_VIEW = pygame.Rect(0,0,480,480)
+def multr(dx_dy, r):
+    a, b, c, d = tuple(r)
+    dx, dy = dxdy
+    return pygame.Rect(a * dx, b * dy, c * dx, d * dy)
 
 
-S_STATUS = multr( dxdy, (480,320,400,160))
+# S_VIEW = pygame.Rect(0,0,480,480)
 
-S_ITEMS = multr( dxdy, (480,160,160,200))
-S_STATUS = multr( dxdy, (480,360,160,120))
 
+S_STATUS = multr(dxdy, (480, 320, 400, 160))
 
+S_ITEMS = multr(dxdy, (480, 160, 160, 200))
+S_STATUS = multr(dxdy, (480, 360, 160, 120))
 
 
 # game view area.
-S_VIEW = multr( dxdy, (76,0,380,340))
+S_VIEW = multr(dxdy, (76, 0, 380, 340))
 
 
 # left side, full status area.
-S_STATUS = multr( dxdy, (0,0,76,340) )
+S_STATUS = multr(dxdy, (0, 0, 76, 340))
 
 
 # left side status boxes.
-#S_HEALTH = pygame.Rect(10,30,60,70)
-S_HEALTH = multr( dxdy, (10,4,60,96) )
-S_COAL   = multr( dxdy, (10,100,60,70) )
-S_WATER  = multr( dxdy, (10,190,60,70) )
-S_STEAM  = multr( dxdy, (10,260,60,70) )
-
-S_PEASANTS_REMAINING = multr( dxdy, (487,24,122,114) )
-S_CANNON_PRESSURE = multr( dxdy, (76,0,5,340) )
-
-
+# S_HEALTH = pygame.Rect(10,30,60,70)
+S_HEALTH = multr(dxdy, (10, 4, 60, 96))
+S_COAL = multr(dxdy, (10, 100, 60, 70))
+S_WATER = multr(dxdy, (10, 190, 60, 70))
+S_STEAM = multr(dxdy, (10, 260, 60, 70))
 
+S_PEASANTS_REMAINING = multr(dxdy, (487, 24, 122, 114))
+S_CANNON_PRESSURE = multr(dxdy, (76, 0, 5, 340))
 
 
 # top right,  castle robot illustration area.
-S_ROBOT = multr( dxdy, (456,0,184,163) )
+S_ROBOT = multr(dxdy, (456, 0, 184, 163))
 
 
 # middle right, items area.
-S_ITEMS = multr( dxdy, (456,163,184,177) )
-
-
-S_ITEMS_ENGINE = multr( dxdy, (480,160,160,160) )
-S_ITEMS_COALSTORAGEROOM = multr( dxdy, (480,160,160,160) )
-S_ITEMS_WATERTANK = multr( dxdy, (480,160,160,160) )
-S_ITEMS_CANNON = multr( dxdy, (480,160,160,160) )
-S_ITEMS_ARMOUR = multr( dxdy, (480,160,160,160) )
+S_ITEMS = multr(dxdy, (456, 163, 184, 177))
 
 
+S_ITEMS_ENGINE = multr(dxdy, (480, 160, 160, 160))
+S_ITEMS_COALSTORAGEROOM = multr(dxdy, (480, 160, 160, 160))
+S_ITEMS_WATERTANK = multr(dxdy, (480, 160, 160, 160))
+S_ITEMS_CANNON = multr(dxdy, (480, 160, 160, 160))
+S_ITEMS_ARMOUR = multr(dxdy, (480, 160, 160, 160))
 
 
 # bottom right,  button area.
-S_BUTTONS = pygame.Rect(470,340,170,140)
+S_BUTTONS = pygame.Rect(470, 340, 170, 140)
 
-S_BUTTONS_SAVE = pygame.Rect(490,360,60,40)
-S_BUTTONS_LOAD = pygame.Rect(490,420,60,40)
-S_BUTTONS_QUIT = pygame.Rect(560,360,60,40)
-S_BUTTONS_NEWS = pygame.Rect(560,420,60,40)
+S_BUTTONS_SAVE = pygame.Rect(490, 360, 60, 40)
+S_BUTTONS_LOAD = pygame.Rect(490, 420, 60, 40)
+S_BUTTONS_QUIT = pygame.Rect(560, 360, 60, 40)
+S_BUTTONS_NEWS = pygame.Rect(560, 420, 60, 40)
+
+S_BOTTOM = pygame.Rect(0, 340, 640, 140)
+
+(
+    S_BUTTONS,
+    S_BUTTONS_SAVE,
+    S_BUTTONS_LOAD,
+    S_BUTTONS_QUIT,
+    S_BUTTONS_NEWS,
+    S_BOTTOM,
+) = [
+    multr(dxdy, x)
+    for x in [
+        S_BUTTONS,
+        S_BUTTONS_SAVE,
+        S_BUTTONS_LOAD,
+        S_BUTTONS_QUIT,
+        S_BUTTONS_NEWS,
+        S_BOTTOM,
+    ]
+]
 
-S_BOTTOM = pygame.Rect(0,340,640,140)
 
-S_BUTTONS, S_BUTTONS_SAVE, S_BUTTONS_LOAD, S_BUTTONS_QUIT, S_BUTTONS_NEWS, S_BOTTOM, = map(lambda x:multr(dxdy, x), [S_BUTTONS, S_BUTTONS_SAVE, S_BUTTONS_LOAD, S_BUTTONS_QUIT, S_BUTTONS_NEWS, S_BOTTOM])
-
-
-
-
-
-
-S_BOTTOM_BUTTONS = multr(dxdy, (470,0,170,140))
-S_BOTTOM_MESSAGES = multr(dxdy, (95,25,355,110))
+S_BOTTOM_BUTTONS = multr(dxdy, (470, 0, 170, 140))
+S_BOTTOM_MESSAGES = multr(dxdy, (95, 25, 355, 110))
 # bottom middle message area.
-S_MESSAGES = multr(dxdy, (95,365,355,110))
-
-#S_NEXT_LEVEL_MESSAGES = pygame.Rect(20,165,380,410)
-S_NEXT_LEVEL_MESSAGES = multr( dxdy, (20,20,500,410))
-
+S_MESSAGES = multr(dxdy, (95, 365, 355, 110))
 
+# S_NEXT_LEVEL_MESSAGES = pygame.Rect(20,165,380,410)
+S_NEXT_LEVEL_MESSAGES = multr(dxdy, (20, 20, 500, 410))
 
-S_= pygame.Rect(480,360,160,120)
 
+S_ = pygame.Rect(480, 360, 160, 120)
 
 
 UPGRADE_FUN = 1
 
 CACHE_USE_LEVEL_CACHE = 1
 
 # if you are modifying just the tiles or just the levels set one of these to 0.
-#  These only check the levels, 
+#  These only check the levels,
 #    or the tiles to see if its older than the cache.
 CACHE_CHECK_TILES = 1
 CACHE_CHECK_LEVEL = 1
 
 
 # joystick buttons
 JOY_FIRE_BUTTON = 1
 JOY_PICKUP_BUTTON = 2
 
 # should things be auto picked up or not?
 AUTO_PICKUP = 1
 
-#should holes that the castle hits the ground be
-#solid tiles
-#0 = no, 1 = yes, 2= big holes
+# should holes that the castle hits the ground be
+# solid tiles
+# 0 = no, 1 = yes, 2= big holes
 HOLES_ARE_TILES = 0
 
 
-#NOTE: mouselook seems to not work well on some systems...
+# NOTE: mouselook seems to not work well on some systems...
 #       can toggle it with the m key in game.
-DISABLE_MOUSE_LOOK =0
+DISABLE_MOUSE_LOOK = 0
 
 
 FLOCKING_FLUCT = 1
 
-def get_mouse_info():
 
+def get_mouse_info():
     if DISABLE_MOUSE_LOOK:
-        SCROLL_MOUSE = 0 #speed of mouse scroll
-        SCROLL_AUTO = 9 #speed of auto-return scroll
-        SCROLL_BORDER = 70 #size of scrolling border during auto-scroll
+        SCROLL_MOUSE = 0  # speed of mouse scroll
+        SCROLL_AUTO = 9  # speed of auto-return scroll
+        SCROLL_BORDER = 70  # size of scrolling border during auto-scroll
     else:
-        SCROLL_MOUSE = 12 #speed of mouse scroll
-        SCROLL_AUTO = 9 #speed of auto-return scroll
-        SCROLL_BORDER = 160 #size of scrolling border during auto-scroll
+        SCROLL_MOUSE = 12  # speed of mouse scroll
+        SCROLL_AUTO = 9  # speed of auto-return scroll
+        SCROLL_BORDER = 160  # size of scrolling border during auto-scroll
 
     return [SCROLL_MOUSE, SCROLL_AUTO, SCROLL_BORDER]
```

### Comparing `zanthor-1.2.3/LICENSE.txt` & `zanthor-1.2.4a2/LICENSE.txt`

 * *Files identical despite different names*

