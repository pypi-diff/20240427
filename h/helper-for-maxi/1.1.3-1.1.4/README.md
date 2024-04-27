# Comparing `tmp/helper_for_maxi-1.1.3.tar.gz` & `tmp/helper_for_maxi-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helper_for_maxi-1.1.3.tar", last modified: Sat Apr 27 00:05:10 2024, max compression
+gzip compressed data, was "helper_for_maxi-1.1.4.tar", last modified: Sat Apr 27 16:18:48 2024, max compression
```

## Comparing `helper_for_maxi-1.1.3.tar` & `helper_for_maxi-1.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 00:05:10.523499 helper_for_maxi-1.1.3/
--rw-rw-rw-   0        0        0     1088 2024-03-21 21:19:01.000000 helper_for_maxi-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      962 2024-04-27 00:05:10.523499 helper_for_maxi-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-04-26 23:52:41.000000 helper_for_maxi-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 00:05:10.491158 helper_for_maxi-1.1.3/helper/
--rw-rw-rw-   0        0        0      774 2024-03-26 20:16:33.000000 helper_for_maxi-1.1.3/helper/__init__.py
--rw-rw-rw-   0        0        0      331 2023-11-06 19:03:02.000000 helper_for_maxi-1.1.3/helper/append_clipboard.py
--rw-rw-rw-   0        0        0     1055 2023-08-21 18:12:43.000000 helper_for_maxi-1.1.3/helper/better_color_input.py
--rw-rw-rw-   0        0        0      575 2023-08-21 18:19:43.000000 helper_for_maxi-1.1.3/helper/better_input.py
--rw-rw-rw-   0        0        0      659 2023-02-26 18:22:53.000000 helper_for_maxi-1.1.3/helper/better_print.py
--rw-rw-rw-   0        0        0      823 2023-08-21 18:27:01.000000 helper_for_maxi-1.1.3/helper/color_input.py
--rw-rw-rw-   0        0        0      621 2024-03-26 20:10:50.000000 helper_for_maxi-1.1.3/helper/key_dict.py
--rw-rw-rw-   0        0        0     1803 2023-12-25 14:34:47.000000 helper_for_maxi-1.1.3/helper/kwargs_handler.py
--rw-rw-rw-   0        0        0      335 2023-08-21 18:37:51.000000 helper_for_maxi-1.1.3/helper/output_stdout.py
--rw-rw-rw-   0        0        0     3149 2023-12-25 14:42:02.000000 helper_for_maxi-1.1.3/helper/terminal.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:05:10.522499 helper_for_maxi-1.1.3/helper_for_maxi.egg-info/
--rw-rw-rw-   0        0        0      962 2024-04-27 00:05:10.000000 helper_for_maxi-1.1.3/helper_for_maxi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      929 2024-04-27 00:05:10.000000 helper_for_maxi-1.1.3/helper_for_maxi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 00:05:10.000000 helper_for_maxi-1.1.3/helper_for_maxi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-27 00:05:10.000000 helper_for_maxi-1.1.3/helper_for_maxi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 00:05:10.000000 helper_for_maxi-1.1.3/helper_for_maxi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 00:05:10.515200 helper_for_maxi-1.1.3/maximyoga/
-drwxrwxrwx   0        0        0        0 2024-04-27 00:05:10.517499 helper_for_maxi-1.1.3/maximyoga/Terminal/
--rw-rw-rw-   0        0        0      172 2024-04-26 21:34:02.000000 helper_for_maxi-1.1.3/maximyoga/Terminal/__init__.py
--rw-rw-rw-   0        0        0     4322 2024-04-26 21:48:54.000000 helper_for_maxi-1.1.3/maximyoga/Terminal/_choices_interface.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:05:10.520499 helper_for_maxi-1.1.3/maximyoga/Terminal/color/
--rw-rw-rw-   0        0        0      230 2024-04-26 21:52:37.000000 helper_for_maxi-1.1.3/maximyoga/Terminal/color/__init__.py
--rw-rw-rw-   0        0        0      469 2024-04-26 21:52:59.000000 helper_for_maxi-1.1.3/maximyoga/Terminal/color/_background.py
--rw-rw-rw-   0        0        0      506 2024-04-26 21:53:06.000000 helper_for_maxi-1.1.3/maximyoga/Terminal/color/_foreground.py
--rw-rw-rw-   0        0        0      691 2024-03-26 21:46:16.000000 helper_for_maxi-1.1.3/maximyoga/__init__.py
--rw-rw-rw-   0        0        0      202 2024-04-26 21:49:41.000000 helper_for_maxi-1.1.3/maximyoga/_append_clipboard.py
--rw-rw-rw-   0        0        0      733 2024-04-26 22:02:44.000000 helper_for_maxi-1.1.3/maximyoga/_better_color_input.py
--rw-rw-rw-   0        0        0      442 2024-04-26 21:59:50.000000 helper_for_maxi-1.1.3/maximyoga/_better_input.py
--rw-rw-rw-   0        0        0      466 2024-04-26 22:00:43.000000 helper_for_maxi-1.1.3/maximyoga/_better_print.py
--rw-rw-rw-   0        0        0      478 2024-04-26 22:04:38.000000 helper_for_maxi-1.1.3/maximyoga/_color_input.py
--rw-rw-rw-   0        0        0      317 2024-04-26 22:17:15.000000 helper_for_maxi-1.1.3/maximyoga/_key_dict.py
--rw-rw-rw-   0        0        0     2127 2024-04-26 23:42:00.000000 helper_for_maxi-1.1.3/maximyoga/_kwargs_handler.py
--rw-rw-rw-   0        0        0      227 2024-04-26 23:42:26.000000 helper_for_maxi-1.1.3/maximyoga/_output_stdout.py
--rw-rw-rw-   0        0        0     3472 2024-04-26 23:45:37.000000 helper_for_maxi-1.1.3/maximyoga/_repr_iterable.py
--rw-rw-rw-   0        0        0      108 2022-12-23 14:16:08.000000 helper_for_maxi-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      713 2024-04-27 00:05:10.531577 helper_for_maxi-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 16:18:48.623314 helper_for_maxi-1.1.4/
+-rw-rw-rw-   0        0        0     1088 2024-03-21 21:19:01.000000 helper_for_maxi-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      962 2024-04-27 16:18:48.623314 helper_for_maxi-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-04-26 23:52:41.000000 helper_for_maxi-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 16:18:48.569271 helper_for_maxi-1.1.4/helper/
+-rw-rw-rw-   0        0        0      774 2024-03-26 20:16:33.000000 helper_for_maxi-1.1.4/helper/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-11-06 19:03:02.000000 helper_for_maxi-1.1.4/helper/append_clipboard.py
+-rw-rw-rw-   0        0        0     1055 2023-08-21 18:12:43.000000 helper_for_maxi-1.1.4/helper/better_color_input.py
+-rw-rw-rw-   0        0        0      575 2023-08-21 18:19:43.000000 helper_for_maxi-1.1.4/helper/better_input.py
+-rw-rw-rw-   0        0        0      659 2023-02-26 18:22:53.000000 helper_for_maxi-1.1.4/helper/better_print.py
+-rw-rw-rw-   0        0        0      823 2023-08-21 18:27:01.000000 helper_for_maxi-1.1.4/helper/color_input.py
+-rw-rw-rw-   0        0        0      621 2024-03-26 20:10:50.000000 helper_for_maxi-1.1.4/helper/key_dict.py
+-rw-rw-rw-   0        0        0     1803 2023-12-25 14:34:47.000000 helper_for_maxi-1.1.4/helper/kwargs_handler.py
+-rw-rw-rw-   0        0        0      335 2023-08-21 18:37:51.000000 helper_for_maxi-1.1.4/helper/output_stdout.py
+-rw-rw-rw-   0        0        0     3149 2023-12-25 14:42:02.000000 helper_for_maxi-1.1.4/helper/terminal.py
+drwxrwxrwx   0        0        0        0 2024-04-27 16:18:48.620797 helper_for_maxi-1.1.4/helper_for_maxi.egg-info/
+-rw-rw-rw-   0        0        0      962 2024-04-27 16:18:48.000000 helper_for_maxi-1.1.4/helper_for_maxi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      929 2024-04-27 16:18:48.000000 helper_for_maxi-1.1.4/helper_for_maxi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 16:18:48.000000 helper_for_maxi-1.1.4/helper_for_maxi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-27 16:18:48.000000 helper_for_maxi-1.1.4/helper_for_maxi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 16:18:48.000000 helper_for_maxi-1.1.4/helper_for_maxi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 16:18:48.610397 helper_for_maxi-1.1.4/maximyoga/
+drwxrwxrwx   0        0        0        0 2024-04-27 16:18:48.614636 helper_for_maxi-1.1.4/maximyoga/Terminal/
+-rw-rw-rw-   0        0        0      172 2024-04-26 21:34:02.000000 helper_for_maxi-1.1.4/maximyoga/Terminal/__init__.py
+-rw-rw-rw-   0        0        0     4436 2024-04-27 16:15:54.000000 helper_for_maxi-1.1.4/maximyoga/Terminal/_choices_interface.py
+drwxrwxrwx   0        0        0        0 2024-04-27 16:18:48.619796 helper_for_maxi-1.1.4/maximyoga/Terminal/color/
+-rw-rw-rw-   0        0        0      230 2024-04-26 21:52:37.000000 helper_for_maxi-1.1.4/maximyoga/Terminal/color/__init__.py
+-rw-rw-rw-   0        0        0      469 2024-04-26 21:52:59.000000 helper_for_maxi-1.1.4/maximyoga/Terminal/color/_background.py
+-rw-rw-rw-   0        0        0      506 2024-04-26 21:53:06.000000 helper_for_maxi-1.1.4/maximyoga/Terminal/color/_foreground.py
+-rw-rw-rw-   0        0        0      691 2024-03-26 21:46:16.000000 helper_for_maxi-1.1.4/maximyoga/__init__.py
+-rw-rw-rw-   0        0        0      202 2024-04-26 21:49:41.000000 helper_for_maxi-1.1.4/maximyoga/_append_clipboard.py
+-rw-rw-rw-   0        0        0      733 2024-04-26 22:02:44.000000 helper_for_maxi-1.1.4/maximyoga/_better_color_input.py
+-rw-rw-rw-   0        0        0      442 2024-04-26 21:59:50.000000 helper_for_maxi-1.1.4/maximyoga/_better_input.py
+-rw-rw-rw-   0        0        0      466 2024-04-26 22:00:43.000000 helper_for_maxi-1.1.4/maximyoga/_better_print.py
+-rw-rw-rw-   0        0        0      478 2024-04-26 22:04:38.000000 helper_for_maxi-1.1.4/maximyoga/_color_input.py
+-rw-rw-rw-   0        0        0      317 2024-04-26 22:17:15.000000 helper_for_maxi-1.1.4/maximyoga/_key_dict.py
+-rw-rw-rw-   0        0        0     2127 2024-04-26 23:42:00.000000 helper_for_maxi-1.1.4/maximyoga/_kwargs_handler.py
+-rw-rw-rw-   0        0        0      227 2024-04-26 23:42:26.000000 helper_for_maxi-1.1.4/maximyoga/_output_stdout.py
+-rw-rw-rw-   0        0        0     3472 2024-04-26 23:45:37.000000 helper_for_maxi-1.1.4/maximyoga/_repr_iterable.py
+-rw-rw-rw-   0        0        0      108 2022-12-23 14:16:08.000000 helper_for_maxi-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      713 2024-04-27 16:18:48.625321 helper_for_maxi-1.1.4/setup.cfg
```

### Comparing `helper_for_maxi-1.1.3/LICENSE` & `helper_for_maxi-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/PKG-INFO` & `helper_for_maxi-1.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: helper_for_maxi
-Version: 1.1.3
+Version: 1.1.4
 Summary: Contains all Functions
 Author: Maxi Myoga
-Project-URL: Github, https://github.com/CatMaxiMyoga/helper_for_maxi/tree/main/1.1.3/package
-Project-URL: Changelog, https://github.com/CatMaxiMyoga/helper_for_maxi/blob/main/1.1.3/CHANGELOG.md
+Project-URL: Github, https://github.com/CatMaxiMyoga/helper_for_maxi/tree/main/1.1.4/package
+Project-URL: Changelog, https://github.com/CatMaxiMyoga/helper_for_maxi/blob/main/1.1.4/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
```

### Comparing `helper_for_maxi-1.1.3/helper/__init__.py` & `helper_for_maxi-1.1.4/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/helper/better_color_input.py` & `helper_for_maxi-1.1.4/helper/better_color_input.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/helper/better_input.py` & `helper_for_maxi-1.1.4/helper/better_input.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/helper/better_print.py` & `helper_for_maxi-1.1.4/helper/better_print.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/helper/color_input.py` & `helper_for_maxi-1.1.4/helper/color_input.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/helper/key_dict.py` & `helper_for_maxi-1.1.4/helper/key_dict.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/helper/kwargs_handler.py` & `helper_for_maxi-1.1.4/helper/kwargs_handler.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/helper/terminal.py` & `helper_for_maxi-1.1.4/helper/terminal.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/helper_for_maxi.egg-info/PKG-INFO` & `helper_for_maxi-1.1.4/helper_for_maxi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: helper_for_maxi
-Version: 1.1.3
+Version: 1.1.4
 Summary: Contains all Functions
 Author: Maxi Myoga
-Project-URL: Github, https://github.com/CatMaxiMyoga/helper_for_maxi/tree/main/1.1.3/package
-Project-URL: Changelog, https://github.com/CatMaxiMyoga/helper_for_maxi/blob/main/1.1.3/CHANGELOG.md
+Project-URL: Github, https://github.com/CatMaxiMyoga/helper_for_maxi/tree/main/1.1.4/package
+Project-URL: Changelog, https://github.com/CatMaxiMyoga/helper_for_maxi/blob/main/1.1.4/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
```

### Comparing `helper_for_maxi-1.1.3/helper_for_maxi.egg-info/SOURCES.txt` & `helper_for_maxi-1.1.4/helper_for_maxi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/maximyoga/Terminal/_choices_interface.py` & `helper_for_maxi-1.1.4/maximyoga/Terminal/_choices_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from os import system
 from string import digits
 import random
 from pygetwindow import getActiveWindowTitle
 from pynput.keyboard import Listener, Key, KeyCode
-from .color import foreground, background, RESET
+from .color import foreground, background
 
 def clear() -> None:
 	system("cls")
 
 class ChoiceInterface:
 	type __key = Key | KeyCode
 
 	def __init__(
 		self, *,
 		textColor: foreground = foreground.WHITE,
 		highlightTextColor: foreground = foreground.BLACK,
 		highlightColor: background = background.WHITE,
-		confirmKey: list[__key] | tuple[__key] | __key = (Key.enter, Key.right),
-		cancelKey: list[__key] | tuple[__key] | __key = Key.esc,
+		confirmKey: list[__key] | tuple[__key, ...] | __key = (Key.enter, Key.right),
+		cancelKey: list[__key] | tuple[__key, ...] | __key = Key.esc,
 		choicesSurround: str = "",
 		addArrowToSelected: bool = False
 	) -> None:
 		r"""
 		Creates the callable ChoiceInterface instance
 		:param textColor:
 		:param highlightTextColor:
@@ -77,31 +77,31 @@
 		hlLen = minimumHighlightLength if (minimumHighlightLength >= 0 and
 		                                   not (any([self.choicesSurround, self.addArrowToSelected]))) \
 										else max([len(line) for line in choices]) + abs(minimumHighlightLength)
 
 		while True:
 			clear()
 			if prefix:
-				print(self.textColor.value + prefix+RESET)
+				print(self.textColor.value + prefix+foreground.RESET.value)
 
 			for i, line in enumerate(choices):
 				_out = ''
 				if i == selected:
 					if not any([self.choicesSurround, self.addArrowToSelected]):
-						_out = f"{self.hlColor.value+self.hlTextColor}{line:<{hlLen}}{RESET}"
+						_out = f"{self.hlColor.value+self.hlTextColor.value}{line:<{hlLen}}{foreground.RESET.value}"
 					elif self.addArrowToSelected:
-						_out = f"{self.hlColor.value+self.hlTextColor}{line+" >":<{hlLen+2}}{RESET}"
+						_out = f"{self.hlColor.value+self.hlTextColor.value}{line+" >":<{hlLen+2}}{foreground.RESET.value}"
 				else:
-					_out = self.textColor.value+line+RESET
+					_out = self.textColor.value+line+foreground.RESET.value
 				if self.choicesSurround:
 					_out = self.choicesSurround+_out+self.choicesSurround
 				print(_out)
 
 			if suffix:
-				print(self.textColor.value+prefix+RESET)
+				print(self.textColor.value+prefix+foreground.RESET.value)
 
 			key = self._waitForKey()
 
 			if key == Key.down and selected != len(choices)-1:
 				selected += 1
 			elif key == Key.up and selected != 0:
 				selected -= 1
@@ -114,19 +114,19 @@
 				system(f"TITLE {terminalTitleBefore}")
 				return -1
 			elif key in [Key.down, Key.up]:
 				pass
 			else:
 				raise Exception("Somehow, Somewhere, Something went wrong :/")
 
-	def _waitForKey(self) -> __key:
+	def _waitForKey(self) -> __key | None:
 		lst = Listener(on_press=lambda key: self._onKeyPress(key, lst))
 		lst.start()
 		lst.join()
 		return self.__lastKeyPressed
 
-	def _onKeyPress(self, key: __key, lst: Listener) -> None:
+	def _onKeyPress(self, key: __key | None, lst: Listener) -> None:
 		if getActiveWindowTitle() != self.terminalWindowTitle:
 			return
 		self.__lastKeyPressed = key
 		if self.__lastKeyPressed in self.confirmKeys+self.cancelKeys+[Key.up, Key.down]:
 			lst.stop()
```

### Comparing `helper_for_maxi-1.1.3/maximyoga/__init__.py` & `helper_for_maxi-1.1.4/maximyoga/__init__.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/maximyoga/_better_color_input.py` & `helper_for_maxi-1.1.4/maximyoga/_better_color_input.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/maximyoga/_kwargs_handler.py` & `helper_for_maxi-1.1.4/maximyoga/_kwargs_handler.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/maximyoga/_repr_iterable.py` & `helper_for_maxi-1.1.4/maximyoga/_repr_iterable.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.3/setup.cfg` & `helper_for_maxi-1.1.4/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 656c 7065 725f 666f 725f 6d61   = helper_for_ma
 00000020: 7869 0d0a 7665 7273 696f 6e20 3d20 312e  xi..version = 1.
-00000030: 312e 330d 0a61 7574 686f 7220 3d20 4d61  1.3..author = Ma
+00000030: 312e 340d 0a61 7574 686f 7220 3d20 4d61  1.4..author = Ma
 00000040: 7869 204d 796f 6761 0d0a 6465 7363 7269  xi Myoga..descri
 00000050: 7074 696f 6e20 3d20 436f 6e74 6169 6e73  ption = Contains
 00000060: 2061 6c6c 2046 756e 6374 696f 6e73 0d0a   all Functions..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000090: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 000000a0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
 000000b0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
 000000c0: 6e0d 0a70 726f 6a65 6374 5f75 726c 7320  n..project_urls 
 000000d0: 3d20 0d0a 0947 6974 6875 6220 3d20 6874  = ...Github = ht
 000000e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000000f0: 2f43 6174 4d61 7869 4d79 6f67 612f 6865  /CatMaxiMyoga/he
 00000100: 6c70 6572 5f66 6f72 5f6d 6178 692f 7472  lper_for_maxi/tr
-00000110: 6565 2f6d 6169 6e2f 312e 312e 332f 7061  ee/main/1.1.3/pa
+00000110: 6565 2f6d 6169 6e2f 312e 312e 342f 7061  ee/main/1.1.4/pa
 00000120: 636b 6167 650d 0a09 4368 616e 6765 6c6f  ckage...Changelo
 00000130: 6720 3d20 6874 7470 733a 2f2f 6769 7468  g = https://gith
 00000140: 7562 2e63 6f6d 2f43 6174 4d61 7869 4d79  ub.com/CatMaxiMy
 00000150: 6f67 612f 6865 6c70 6572 5f66 6f72 5f6d  oga/helper_for_m
 00000160: 6178 692f 626c 6f62 2f6d 6169 6e2f 312e  axi/blob/main/1.
-00000170: 312e 332f 4348 414e 4745 4c4f 472e 6d64  1.3/CHANGELOG.md
+00000170: 312e 342f 4348 414e 4745 4c4f 472e 6d64  1.4/CHANGELOG.md
 00000180: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
 00000190: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
 000001a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 000001b0: 6e20 3a3a 2033 0d0a 0944 6576 656c 6f70  n :: 3...Develop
 000001c0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
 000001d0: 202d 2041 6c70 6861 0d0a 094f 7065 7261   - Alpha...Opera
 000001e0: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
```
