# Comparing `tmp/tkeasygui-0.2.63.tar.gz` & `tmp/tkeasygui-0.2.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkeasygui-0.2.63.tar", last modified: Wed Apr 24 11:55:38 2024, max compression
+gzip compressed data, was "tkeasygui-0.2.67.tar", last modified: Sat Apr 27 13:47:06 2024, max compression
```

## Comparing `tkeasygui-0.2.63.tar` & `tkeasygui-0.2.67.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-24 11:55:38.458690 tkeasygui-0.2.63/
--rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.63/LICENSE
--rw-r--r--   0 kujirahand   (501) staff       (20)     6747 2024-04-24 11:55:38.458466 tkeasygui-0.2.63/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)     4343 2024-04-24 05:52:16.000000 tkeasygui-0.2.63/README.md
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-24 11:55:38.456990 tkeasygui-0.2.63/TkEasyGUI/
--rw-r--r--   0 kujirahand   (501) staff       (20)      376 2024-04-20 12:19:46.000000 tkeasygui-0.2.63/TkEasyGUI/__init__.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    27595 2024-04-21 12:07:15.000000 tkeasygui-0.2.63/TkEasyGUI/dialogs.py
--rw-r--r--   0 kujirahand   (501) staff       (20)     2545 2024-04-24 11:24:23.000000 tkeasygui-0.2.63/TkEasyGUI/locale_easy.py
--rw-r--r--   0 kujirahand   (501) staff       (20)     6538 2024-04-21 06:55:17.000000 tkeasygui-0.2.63/TkEasyGUI/utils.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-24 11:55:36.000000 tkeasygui-0.2.63/TkEasyGUI/version.py
--rw-r--r--   0 kujirahand   (501) staff       (20)   120490 2024-04-24 10:39:53.000000 tkeasygui-0.2.63/TkEasyGUI/widgets.py
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-24 11:55:38.458162 tkeasygui-0.2.63/TkEasyGUI.egg-info/
--rw-r--r--   0 kujirahand   (501) staff       (20)     6747 2024-04-24 11:55:38.000000 tkeasygui-0.2.63/TkEasyGUI.egg-info/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)      325 2024-04-24 11:55:38.000000 tkeasygui-0.2.63/TkEasyGUI.egg-info/SOURCES.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-24 11:55:38.000000 tkeasygui-0.2.63/TkEasyGUI.egg-info/dependency_links.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-24 11:55:38.000000 tkeasygui-0.2.63/TkEasyGUI.egg-info/requires.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-24 11:55:38.000000 tkeasygui-0.2.63/TkEasyGUI.egg-info/top_level.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-24 11:18:19.000000 tkeasygui-0.2.63/pyproject.toml
--rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-24 11:55:38.458737 tkeasygui-0.2.63/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-27 13:47:06.081625 tkeasygui-0.2.67/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.67/LICENSE
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6747 2024-04-27 13:47:06.081276 tkeasygui-0.2.67/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)     4343 2024-04-24 05:52:16.000000 tkeasygui-0.2.67/README.md
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-27 13:47:06.078857 tkeasygui-0.2.67/TkEasyGUI/
+-rw-r--r--   0 kujirahand   (501) staff       (20)      376 2024-04-20 12:19:46.000000 tkeasygui-0.2.67/TkEasyGUI/__init__.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)    28011 2024-04-27 13:34:47.000000 tkeasygui-0.2.67/TkEasyGUI/dialogs.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)     2545 2024-04-24 11:24:23.000000 tkeasygui-0.2.67/TkEasyGUI/locale_easy.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6538 2024-04-27 13:29:24.000000 tkeasygui-0.2.67/TkEasyGUI/utils.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-27 13:47:04.000000 tkeasygui-0.2.67/TkEasyGUI/version.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)   124136 2024-04-27 13:31:46.000000 tkeasygui-0.2.67/TkEasyGUI/widgets.py
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-27 13:47:06.080586 tkeasygui-0.2.67/TkEasyGUI.egg-info/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6747 2024-04-27 13:47:06.000000 tkeasygui-0.2.67/TkEasyGUI.egg-info/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)      325 2024-04-27 13:47:06.000000 tkeasygui-0.2.67/TkEasyGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-27 13:47:06.000000 tkeasygui-0.2.67/TkEasyGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-27 13:47:06.000000 tkeasygui-0.2.67/TkEasyGUI.egg-info/requires.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-27 13:47:06.000000 tkeasygui-0.2.67/TkEasyGUI.egg-info/top_level.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-27 13:34:59.000000 tkeasygui-0.2.67/pyproject.toml
+-rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-27 13:47:06.081719 tkeasygui-0.2.67/setup.cfg
```

### Comparing `tkeasygui-0.2.63/LICENSE` & `tkeasygui-0.2.67/LICENSE`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.63/PKG-INFO` & `tkeasygui-0.2.67/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.63
+Version: 0.2.67
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
```

### Comparing `tkeasygui-0.2.63/README.md` & `tkeasygui-0.2.67/README.md`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.63/TkEasyGUI/dialogs.py` & `tkeasygui-0.2.67/TkEasyGUI/dialogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 TkEasyGUI dialogs
 """
 import subprocess
 import tkinter.filedialog as filedialog
 import tkinter.messagebox as messagebox
 from datetime import datetime, timedelta
-from pprint import pprint
 from tkinter import colorchooser
 from typing import Any, Union
 
 from . import locale_easy as le
 from . import widgets as eg
 from .utils import (
     FontType,
     get_root_window,
     is_mac,
     is_win,
 )
 
+# save original print
+_print = print
+
 #------------------------------------------------------------------------------
 # Dialogs
 #------------------------------------------------------------------------------
 # like PySimpleGUI
 
 def popup_buttons(
         message: str,
@@ -55,18 +57,19 @@
     
     # event loop
     timer_id = eg.time_checker_start()
     autoclose_sec: int = auto_close_duration * 1000
     if non_blocking:
         # TODO: popup non blocking window
         pass
-    while win.is_alive():
+    while True:
         event, _ = win.read(timeout=100, timeout_key=eg.WINDOW_TIMEOUT)
         if event == eg.WINDOW_CLOSED:
             result = eg.WINDOW_CLOSED
+            break
         if event in buttons:
             result = event
             break
         if event == eg.WINDOW_TIMEOUT:
             if auto_close_duration > 0 and eg.time_checker_end(timer_id) > autoclose_sec:
                 result = timeout_key # timeout_key only use result
                 break
@@ -588,43 +591,50 @@
     """Popup a color selection dialog. Return the color selected."""
     col = colorchooser.askcolor(title=title, color=default_color)
     if col[1] is None:
         return default_color
     return f"{col[1]}".upper()
 
 def popup_listbox(
-        items: list[str], # list of items
-        message: str = "",
-        title: str = "",
-        size: tuple[int,int] = (20, 7),
-        font: Union[FontType, None] = None,
-        multiple:bool = False # multiple selection
-        ) -> Union[str, None]:
+    values: list[str],  # list of items
+    message: str = "",
+    title: str = "",
+    size: tuple[int, int] = (20, 7),
+    font: Union[FontType, None] = None,
+    default_value: Union[str, None] = None,  # default value
+    multiple: bool = False,  # multiple selection
+) -> Union[str, None]:
     """Display Listbox in a popup window"""
     select_mode = eg.LISTBOX_SELECT_MODE_BROWSE if multiple is False else eg.LISTBOX_SELECT_MODE_MULTIPLE
-    win = eg.Window(title, layout=[
-        [eg.Text(message)],
-        [eg.Listbox(values=items, key="-list-", size=size, font=font, select_mode=select_mode)],
-        [eg.Button("OK", width=9), eg.Button("Cancel", width=5)]
-    ], modal=True)
-    result = None
-    while win.is_alive():
-        event, _ = win.read()
-        if event == "Cancel":
-            result = None
-            break
-        if event == "OK":
-            selected = win["-list-"].get()
-            if multiple:
-                result = selected
-            else:
-                if len(selected) == 1:
-                    result = selected[0]
-            break
-    win.close()
+    # create window
+    layout = []
+    if message != "":
+        layout.append([eg.Text(message)])
+    layout.append([
+        eg.Listbox(
+            values=values, key="-list-",
+            default_value=default_value, size=size,
+            font=font, select_mode=select_mode
+        )])
+    layout.append([eg.Button("OK", width=9), eg.Button("Cancel", width=5)])
+    with eg.Window(title, layout=layout, modal=True) as win:
+        # event loop
+        result = None
+        for event, values in win.event_iter():
+            if event == "Cancel":
+                result = None
+                break
+            if event == "OK":
+                selected = win["-list-"].get()
+                if multiple:
+                    result = selected
+                else:
+                    if len(selected) == 1:
+                        result = selected[0]
+                break
     return result
 
 def popup_image(
         message: str,
         title: Union[str,None] = None,
         image_path: Union[str,None] = None,
         image_data: Union[bytes,None] = None,
@@ -706,15 +716,18 @@
         title: Union[str,None] = None,
         default: str = ""
     ) -> str:
     """Display a message in a popup window with a text entry. Return the text entered."""
     return popup_input(message, title, default)
 
 def print(*args, **kw) -> None:
-    """Print message to popup window."""
+    """Print message to popup window.(call default print function if no_window is True)"""
+    if "no_window" in kw and kw["no_window"]:
+        _print(*args)
+        return
     lines = " ".join([str(a) for a in args])
     popup(lines)
 
 def confirm(
         question: str,
         title: Union[str,None] = None
     ) -> bool:
```

### Comparing `tkeasygui-0.2.63/TkEasyGUI/locale_easy.py` & `tkeasygui-0.2.67/TkEasyGUI/locale_easy.py`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.63/TkEasyGUI/utils.py` & `tkeasygui-0.2.67/TkEasyGUI/utils.py`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.63/TkEasyGUI/widgets.py` & `tkeasygui-0.2.67/TkEasyGUI/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,18 @@
         no_titlebar: bool = False,  # hide titlebar
         grab_anywhere: bool = False,  # can move window by dragging anywhere
         alpha_channel: float = 1.0,  # window alpha channel
         enable_key_events: bool = False,  # enable keyboard events
         return_keyboard_events: bool = False,  # enable keyboard events (for compatibility)
         location: Union[tuple[int, int], None] = None,  # window location
         center_window: bool = True,  # move window to center
-        row_padding: int = 2, # row padding
-        padding_x: int = 8, # x padding around the window
-        padding_y: int = 8, # y padding around the window 
+        row_padding: int = 2,  # row padding
+        padding_x: int = 8,  # x padding around the window
+        padding_y: int = 8,  # y padding around the window
+        show_scrollbar: bool = False,  # show scrollbar (Experimental)
         **kw,
     ) -> None:
         """Create a window with a layout of widgets."""
         self.modal: bool = modal
         # check active window
         active_win = utils._get_active_window()
         if active_win is None:
@@ -128,28 +129,50 @@
         self._mouse_y: Union[int, None] = None
         self.alpha_channel: float = alpha_channel
         self.enable_key_events: bool = enable_key_events
         self.return_keyboard_events: bool = return_keyboard_events
         self.font_size_average: tuple[int, int] = (12, 10)
         self.row_padding: int = row_padding
         self.center_window: bool = center_window
-        # Frame
-        self.frame: tk.Frame = tk.Frame(self.window)
+        self.padding_x: int = padding_x
+        self.padding_y: int = padding_y
+        self.show_scrollbar = show_scrollbar
+        # Canvas
+        self.canvas: Union[tk.Canvas, None] = None
+        if show_scrollbar:
+            self.canvas = tk.Canvas(self.window)
+            self.canvas.pack(
+                side=tk.LEFT, fill=tk.BOTH, expand=True,
+                padx=padding_x, pady=padding_y
+            )
+            # scrollbar
+            self.frame_bar = tk.Scrollbar(
+                self.window,
+                orient=tk.VERTICAL, 
+                command=self.canvas.yview
+            )
+            self.frame_bar.pack(side=tk.RIGHT, fill=tk.Y)
+            self.canvas.configure(yscrollcommand=self.frame_bar.set)
+            # Frame
+            self.frame: tk.Frame = tk.Frame(self.canvas)
+            self.canvas.create_window((0, 0), window=self.frame, anchor=tk.NW)
+        else:
+            self.frame: tk.Frame = tk.Frame(self.window)
+            self.frame.pack(expand=True, fill="both", padx=padding_x, pady=padding_y)
         # self.frame.configure(style="TFrame")
         # set window properties
         self.window.title(title)
         self.window.protocol("WM_DELETE_WINDOW", lambda : self._close_handler())
         self.size: Union[tuple[int, int], None] = size
         if size is not None:
             self.set_size(size)
         self.window.resizable(resizable, resizable)
         # create widgets
         self._create_widget(self.frame, layout)
         # pack frame
-        self.frame.pack(expand=True, fill="both", padx=padding_x, pady=padding_y)
         self.frame.rowconfigure(0, weight=1)
         if keep_on_top:
             self.window.attributes("-topmost", True)
         if no_titlebar:
             self.window.after_idle(self.hide_titlebar, True)
         if grab_anywhere:
             self.set_grab_anywhere(True)
@@ -173,29 +196,52 @@
             self.window.grab_set()
             self.window.focus_force()
         # push window
         self.parent_window: Union[Window, None] = _window_parent()
         _window_push(self)
         # set show event
         self.window.bind("<Map>", self._on_window_show)
+        # set window size
+        self.frame.bind("<Configure>", self._on_frame_configure)
         # position
         if location is not None:
             self.set_location(location)
         else:
             # could not get size with geometry() before window is shown
             # so, move window to center after window is shown `_on_window_show`
             pass
 
+    def _on_frame_configure(self, _event):
+        """Handle frame configure event."""
+        if self.canvas is None:
+            return
+        region = self.canvas.bbox("all")
+        self.canvas.configure(scrollregion=region)
+        # set size
+        pre_size = self.size
+        w, h = region[2], region[3]
+        sw, sh = self.get_screen_size()
+        pad_x = self.padding_x * 2
+        pad_y = self.padding_y * 2
+        if (pre_size is None):
+            if w > sw:
+                w = sw - pad_x
+            if h > sh:
+                h = sh - pad_y
+            self.set_size((w + pad_x, h + pad_y))
+            self.size = pre_size
+
     def _on_window_show(self, *event) -> None:
         """Handle window show event."""
         if self.center_window:
             if self.parent_window is None: # only this window
                 self.move_to_center()
             else:
                 self.move_to_center(center_pos=self.parent_window.get_center_location())
+        self.update_idle_tasks()
 
     def set_location(self, xy: tuple[int, int]) -> None:
         """Set window location."""
         self.window.geometry(f"+{xy[0]}+{xy[1]}")
     
     def get_location(self) -> tuple[int, int]:
         """Get window location."""
@@ -451,35 +497,32 @@
             # If an event hidden from the user occurs, continue to use the mainloop.
             if isinstance(key, str) and key.endswith("/hide"):
                 continue # hide system events
             # return a event
             break
         return (key, values)
 
-    def event_iter(self, timeout: Union[int, None] = None, timeout_key: str=TIMEOUT_KEY, auto_close: bool=True) -> Any:
+    def event_iter(self, timeout: Union[int, None] = None, timeout_key: str=TIMEOUT_KEY) -> Any:
         """
         Return generator with event and values
         **Example**
         ```py
         import TkEasyGUI as eg
         # create a window
-        window = eg.Window("test", layout=[[eg.Button("Hello")]])
-        # event loop
-        for event, values in window.event_iter():
-            if event == "Hello":
-                eg.popup("Hello, World!")
+        with eg.Window("test", layout=[[eg.Button("Hello")]]) as window:
+            # event loop
+            for event, values in window.event_iter():
+                if event == "Hello":
+                    eg.popup("Hello, World!")
         ```
        """
         # event loop
         while self.is_alive():
             event, values = self.read(timeout=timeout, timeout_key=timeout_key)
             yield (event, values)
-        # close window
-        if auto_close:
-            self.close()
     
     def _dispatch_event_hooks(self, key: str, values: dict[str, Any]) -> bool:
         """Dispatch event hooks."""
         # execute _event_hooks
         flag_stop = False
         if key in self._event_hooks:
             for handle in self._event_hooks[key]:
@@ -597,14 +640,17 @@
             self.window.overrideredirect(flag)
             self._no_titlebar = flag
         except Exception:
             pass
 
     def close(self) -> None:
         """Close the window."""
+        # The phenomenon where a closed window remains visible is occurring, so forcibly making it transparent.
+        self.set_alpha_channel(0.0) # force hide
+        self.hide()
         # already closed?
         if not self.flag_alive:
             return
         # close window
         try:
             self.flag_alive = False
             _window_pop(self)
@@ -2238,15 +2284,19 @@
             self.props["showvalue"] = 0 if disable_number_display else 1
         if value is not None:
             self.set(value)
         else:
             self._widget_update(**kw)
 
 class Canvas(Element):
-    """Canvas element."""
+    """
+    Canvas element.
+    This widget provides the same drawing methods as [tk.Canvas](https://tkdocs.com/tutorial/canvas.html).
+    methods: create_line/create_rectangle/create_oval/create_polygon/create_arc/create_image/delete etc...
+    """
     def __init__(
                 self,
                 key: Union[str, None] = None,
                 enable_events: bool = False,
                 background_color: Union[str, None] = None,
                 size: tuple[int, int] = (300, 300),
                 # other
@@ -2264,14 +2314,18 @@
                 "<Motion>": "mousemove"
             }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         self.widget = tk.Canvas(parent, **self.props)
         return self.widget
     
+    def clear(self) -> None:
+        """Clear the canvas."""
+        self.widget.delete("all")
+
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
     def update(self, *args, **kw) -> None:
         """Update the widget."""
         self._widget_update(**kw)
@@ -2508,26 +2562,33 @@
         self.widget = ttk.Separator(parent, orient="horizontal")
         return self.widget
 
 
 class Listbox(Element):
     """Listbox element."""
     def __init__(
-                self,
-                values: list[str] = [],
-                default_values: list[str] = [],
-                key: Union[str, None] = None,
-                enable_events: bool = False,
-                select_mode: ListboxSelectMode = LISTBOX_SELECT_MODE_BROWSE,
-                # other
-                metadata: Union[dict[str, Any], None] = None,
-                **kw) -> None:
+        self,
+        values: list[str] = [],
+        default_values: Union[list[str], None] = None,  # selected values
+        default_value: Union[str, None] = None,  # a default value
+        key: Union[str, None] = None,
+        enable_events: bool = False,
+        select_mode: ListboxSelectMode = LISTBOX_SELECT_MODE_BROWSE,
+        # other
+        metadata: Union[dict[str, Any], None] = None,
+        items: Union[list[str], None] = None,  # same as values (alias values)
+        **kw,
+    ) -> None:
         super().__init__("Listbox", "", key, True, metadata, **kw)
         self.values = values
+        if items is not None: # alias
+            self.values = items
         self.select_mode = select_mode
+        if default_value is not None:
+            default_values = [default_value]
         self.default_values = default_values
         # event
         if enable_events:
             self.bind_events({
                 "<<ListboxSelect>>": "select"
             }, "system")
 
@@ -2544,18 +2605,20 @@
         self.widget.pack(side="left", fill="both", expand=True)
         self.widget_scrollbar.pack(side="right", fill="y")
         # insert values
         self.set_values(self.values)
         self.select_values(self.default_values)
         return self.widget_frame
 
-    def select_values(self, values: list[str]) -> None:
+    def select_values(self, values: tuple[list[str], None]) -> None:
         """Select values"""
         if self.widget is None:
             return
+        if values is None:
+            return
         for v in values:
             try:
                 index = self.values.index(v)
                 self.widget.selection_set(index)
             except ValueError:
                 pass
 
@@ -2565,14 +2628,35 @@
         if self.widget is not None:
             # delete all
             self.widget.delete(0, "end")
             # insert data
             for i, v in enumerate(self.values):
                 self.widget.insert(i, v)
 
+    def get_cursor_index(self) -> int:
+        """Get cursor index (return -1 if not selected)"""
+        if self.widget is None:
+            return None
+        wg: tk.Listbox = self.widget
+        selections = wg.curselection()
+        if selections is None or len(selections) == 0:
+            return -1
+        return selections[0]
+    
+    def set_cursor_index(self, index: int) -> None:
+        """Set cursor index"""
+        if self.widget is None:
+            return
+        try:
+            self.widget.select_clear(0, "end")
+            self.widget.selection_set(index)
+            self.widget.see(index)
+        except Exception as _:
+            pass
+
     def get(self) -> Any:
         """Get the value of the widget."""
         if self.widget is None:
             return None
         wg: tk.Listbox = self.widget
         selected: list[str] = []
         selections: Any = wg.curselection()
@@ -3020,41 +3104,48 @@
         return result
 
 class ListBrowse(FileBrowse):
     """ListBrowse element."""
 
     def __init__(
         self,
-        items: list[str] = [],
+        values: list[str] = [],
         message: str = "",
         button_text: str = "...",
+        default_value: Union[str, None] = None,  # default value
         key: Union[str, None] = None,
         target_key: Union[str, None] = None,
         title: str = "",
         font: Union[FontType, None] = None,
         enable_events: bool = False,  # enable changing events
         # other
         metadata: Union[dict[str, Any], None] = None,
         **kw,
     ) -> None:
         super().__init__("ListBrowse", "", key, False, metadata, **kw)
         self.target_key = target_key
         self.title = title
         self.props["text"] = button_text
         self.enable_events = enable_events
-        self.items = items
+        self.values = values
         self.message = message
         self.font = font
+        self.default_value = default_value
 
     def show_dialog(self, *args) -> Union[str, None]:
         """Show Listbox dialog"""
         target: tk.Widget = self.get_prev_widget(self.target_key)
+        if target is not None:
+            val = target.get()
+            if (val != "") and (val in self.values):
+                self.default_value = val
         # popup
         result = dialogs.popup_listbox(
-            items=self.items,
+            values=self.values,
+            default_value=self.default_value,
             message=self.message,
             title=self.title,
             font=self.font,
         )
         if (target is not None) and (result is not None) and (result != ""):
             target.update(result)
             if self.enable_events:
@@ -3084,14 +3175,19 @@
         self.enable_events = enable_events
         self.message = message
         self.font = font
 
     def show_dialog(self, *args) -> Union[str, None]:
         """Show Listbox dialog"""
         target: tk.Widget = self.get_prev_widget(self.target_key)
+        if target is not None:
+            val = target.get()
+            if (val != ""):
+                val = val.replace("\\n", "\n")
+                self.message = val
         # popup
         result = dialogs.popup_scrolled(
             message=self.message,
             title=self.title,
             font=self.font,
         )
         if (target is not None) and (result is not None) and (result != ""):
```

### Comparing `tkeasygui-0.2.63/TkEasyGUI.egg-info/PKG-INFO` & `tkeasygui-0.2.67/TkEasyGUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.63
+Version: 0.2.67
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
```

### Comparing `tkeasygui-0.2.63/pyproject.toml` & `tkeasygui-0.2.67/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TkEasyGUI"
-version = "0.2.63"
+version = "0.2.67"
 dependencies = [
   "Pillow",
   "pyperclip",
 ]
 requires-python = ">=3.9"
 authors = [
   { name="kujirahand", email="web@kujirahand.com" },
```

