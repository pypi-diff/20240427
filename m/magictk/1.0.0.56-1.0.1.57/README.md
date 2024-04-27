# Comparing `tmp/magictk-1.0.0.56.tar.gz` & `tmp/magictk-1.0.1.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-1.0.0.56.tar", last modified: Fri Apr 26 03:20:51 2024, max compression
+gzip compressed data, was "magictk-1.0.1.57.tar", last modified: Sat Apr 27 09:37:54 2024, max compression
```

## Comparing `magictk-1.0.0.56.tar` & `magictk-1.0.1.57.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 03:20:51.533622 magictk-1.0.0.56/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-26 03:20:51.000000 magictk-1.0.0.56/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-26 03:20:51.533622 magictk-1.0.0.56/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1683 2024-04-26 03:20:51.000000 magictk-1.0.0.56/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 03:20:51.529622 magictk-1.0.0.56/magictk/
--rw-r--r--   0 root         (0) root         (0)      501 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3285 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    17051 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11247 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12242 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)     3725 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)     1890 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/icon.py
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/mtk.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5995 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     8106 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/scrollbar.py
--rw-r--r--   0 root         (0) root         (0)     6178 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)      372 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/style.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10245 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 03:20:51.533622 magictk-1.0.0.56/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      629 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-26 03:20:51.000000 magictk-1.0.0.56/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 03:20:51.533622 magictk-1.0.0.56/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-26 03:20:51.000000 magictk-1.0.0.56/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 09:37:54.020435 magictk-1.0.1.57/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-27 09:37:53.000000 magictk-1.0.1.57/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-27 09:37:54.020435 magictk-1.0.1.57/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1683 2024-04-27 09:37:53.000000 magictk-1.0.1.57/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 09:37:54.020435 magictk-1.0.1.57/magictk/
+-rw-r--r--   0 root         (0) root         (0)      514 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    17974 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11247 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12242 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/icon.py
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5995 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     8106 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/scrollbar.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)      372 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/style.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10245 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 09:37:54.020435 magictk-1.0.1.57/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      629 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-27 09:37:53.000000 magictk-1.0.1.57/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 09:37:54.020435 magictk-1.0.1.57/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-27 09:37:53.000000 magictk-1.0.1.57/setup.py
```

### Comparing `magictk-1.0.0.56/PKG-INFO` & `magictk-1.0.1.57/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 1.0.0.56
+Version: 1.0.1.57
 Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-1.0.0.56/README.md` & `magictk-1.0.1.57/README.md`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/_window_ctl.py` & `magictk-1.0.1.57/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/_window_size.py` & `magictk-1.0.1.57/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/basicwindow.py` & `magictk-1.0.1.57/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/button.py` & `magictk-1.0.1.57/magictk/button.py`

 * *Files 5% similar despite different names*

```diff
@@ -394,7 +394,25 @@
             self._color_fg1 = color_type+"_light3"
             self._color_fg = color_type+"_dark"
             self._color_fg3 = color_type+"_light3"
             self._color_fg2 = color_type+"_dark"
             self._color_text = "#FFFFFF"
         super().__init__(master=master, root_anim=root_anim, w=w, h=h,
                          text=text, color_list=color_list, func=func, _set_defaultcolor=True, iconname=iconname, iconsize=iconsize)
+
+
+class ButtonLight(ButtonFill):
+
+    def __init__(self, master=None, root_anim=None, color_type="plain", w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _dis_color=None, iconname="", iconsize=24):
+        if (color_list is not None):
+            self.color = color_list
+        if (_dis_color is None):
+            self._color_bd = "background"
+            self._color_bg = "background"
+            self._color_bg1 = "background"
+            self._color_fg1 = "placeholder_light"
+            self._color_fg = "border_light"
+            self._color_fg3 = "placeholder_light"
+            self._color_fg2 = "border_light"
+            self._color_text = self.color[color_type]
+        super().__init__(master=master, root_anim=root_anim, w=w, h=h,
+                         text=text, color_list=color_list, func=func, _dis_color=True, iconname=iconname, iconsize=iconsize)
```

### Comparing `magictk-1.0.0.56/magictk/checkbox.py` & `magictk-1.0.1.57/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/color_tmpl.py` & `magictk-1.0.1.57/magictk/color_tmpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "danger_light3": "#F89898",
     "danger_dark": "#C45656",
     "info": "#909399",
     "info_light": "#E9E9EB",
     "info_light2": "#F4F4F5",
     "info_light3": "#B1B3B8",
     "info_dark": "#73767A",
+    "plain": "#606266",
     "primary_text": "#303133",
     "regular_text": "#606266",
     "secondary_text": "#909399",
     "placeholder": "#C0C4CC",
     "placeholder_light": "#F5F7FA",
     "border_base": "#DCDFE6",
     "border_light": "#E4E7ED",
```

### Comparing `magictk-1.0.0.56/magictk/entry.py` & `magictk-1.0.1.57/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/fontconfig.py` & `magictk-1.0.1.57/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/frame.py` & `magictk-1.0.1.57/magictk/frame.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/icon.ico` & `magictk-1.0.1.57/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/icon.py` & `magictk-1.0.1.57/magictk/icon.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/photoload.py` & `magictk-1.0.1.57/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/progressbar.py` & `magictk-1.0.1.57/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/res.pickle` & `magictk-1.0.1.57/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/scrollbar.py` & `magictk-1.0.1.57/magictk/scrollbar.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/select.py` & `magictk-1.0.1.57/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/submenu.py` & `magictk-1.0.1.57/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/window.py` & `magictk-1.0.1.57/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk/workspace.py` & `magictk-1.0.1.57/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/magictk.egg-info/PKG-INFO` & `magictk-1.0.1.57/magictk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 1.0.0.56
+Version: 1.0.1.57
 Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-1.0.0.56/magictk.egg-info/SOURCES.txt` & `magictk-1.0.1.57/magictk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magictk-1.0.0.56/setup.py` & `magictk-1.0.1.57/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import os
 from setuptools import setup
 
 ####### config #######
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 ######################
 
 set_v = VERSION
 if (os.path.exists("runid.conf")):
     with open("runid.conf", "r") as file:
         runid = file.read()
     set_v = set_v+"."+runid
```

