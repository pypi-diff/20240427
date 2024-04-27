# Comparing `tmp/cgepy-0.7.3.tar.gz` & `tmp/cgepy-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgepy-0.7.3.tar", max compression
+gzip compressed data, was "cgepy-0.7.4.tar", max compression
```

## Comparing `cgepy-0.7.3.tar` & `cgepy-0.7.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1095 2023-12-09 08:27:12.937737 cgepy-0.7.3/LICENSE.md
--rw-r--r--   0        0        0     1130 2023-12-09 09:21:49.807954 cgepy-0.7.3/README.md
--rw-r--r--   0        0        0     1929 2023-12-09 10:08:08.089675 cgepy-0.7.3/cge/__init__.py
--rw-r--r--   0        0        0      125 2023-12-09 08:24:57.379852 cgepy-0.7.3/cge/_exceptions.py
--rw-r--r--   0        0        0      522 2023-12-09 09:39:33.236546 cgepy-0.7.3/cge/_partial.py
--rw-r--r--   0        0        0      937 2023-12-09 10:22:00.985574 cgepy-0.7.3/cge/colors.py
--rw-r--r--   0        0        0      114 2023-12-09 09:02:11.633813 cgepy-0.7.3/cge/ext/__init__.py
--rw-r--r--   0        0        0      383 2023-12-09 10:04:24.341473 cgepy-0.7.3/cge/ext/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1479 2023-12-09 09:02:11.633839 cgepy-0.7.3/cge/ext/legacy/func.py
--rw-r--r--   0        0        0     1305 2023-12-09 09:02:11.633800 cgepy-0.7.3/cge/ext/legacy/text.py
--rw-r--r--   0        0        0      423 2023-12-09 10:20:23.886576 cgepy-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     1889 1970-01-01 00:00:00.000000 cgepy-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-12-09 08:27:12.937737 cgepy-0.7.4/LICENSE.md
+-rw-r--r--   0        0        0     1130 2023-12-09 09:21:49.807954 cgepy-0.7.4/README.md
+-rw-r--r--   0        0        0     1887 2024-04-27 21:14:33.068524 cgepy-0.7.4/cge/__init__.py
+-rw-r--r--   0        0        0      125 2023-12-09 08:24:57.379852 cgepy-0.7.4/cge/_exceptions.py
+-rw-r--r--   0        0        0      516 2024-02-24 05:46:11.593562 cgepy-0.7.4/cge/_partial.py
+-rw-r--r--   0        0        0      448 2024-04-27 21:13:53.425478 cgepy-0.7.4/cge/_screenclear.py
+-rw-r--r--   0        0        0      842 2024-02-11 22:39:21.923603 cgepy-0.7.4/cge/colors.py
+-rw-r--r--   0        0        0      114 2023-12-09 09:02:11.633813 cgepy-0.7.4/cge/ext/__init__.py
+-rw-r--r--   0        0        0      383 2023-12-09 10:04:24.341473 cgepy-0.7.4/cge/ext/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1479 2023-12-09 09:02:11.633839 cgepy-0.7.4/cge/ext/legacy/func.py
+-rw-r--r--   0        0        0     1305 2023-12-09 09:02:11.633800 cgepy-0.7.4/cge/ext/legacy/text.py
+-rw-r--r--   0        0        0      423 2024-04-27 21:16:05.743726 cgepy-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1889 1970-01-01 00:00:00.000000 cgepy-0.7.4/PKG-INFO
```

### Comparing `cgepy-0.7.3/LICENSE.md` & `cgepy-0.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cgepy-0.7.3/README.md` & `cgepy-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `cgepy-0.7.3/cge/__init__.py` & `cgepy-0.7.4/cge/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-__version__ = "0.7.3"
+__version__ = "0.7.4"
 
 # Import required modules
 
 from .colors import Presets
 from ._partial import out
 from ._exceptions import Exceptions
+from ._screenclear import ClearingMethod
 from .ext import clear
 
-# Initialize settings
+# Defualt settings
 
-spritecolor = Presets.red()
-background = Presets.blue()
+spritecolor = Presets.RED
+background = Presets.BLUE
 
 # Classes
 
 class Grid:
 
 	def __init__(self, size:int = 20):
 		self.sprites = []
@@ -26,41 +27,38 @@
 	def Clear(self):
 		"""Clears the grid context. Does not erase sprites."""
 		self.ctx = [[background for i in range(self.size)] for i in range(self.size)]
 		
 	def Write(self, pos, new):
 		"""Change the color value of a position on the grid."""
 		try:
-			self.ctx[pos[1][0]] = new
+			self.ctx[pos[1]][pos[0]] = new
 
 		except IndexError:
 			e = "Grid index out of range"
 			raise Exceptions.GridError(e)
+		
 	def w(self, pos, new):
-		"""Change the color value of a position on the grid."""
-		try:
-			self.ctx[pos[1][0]] = new
-
-		except IndexError:
-			e = "Grid index out of range"
-			raise Exceptions.GridError(e)
+		"""Shortcut method for Grid.Write()"""
+		self.Write(pos, new)
 
-	def Update(self, screenclearing = True):
+	def Update(self, clearingmethod:ClearingMethod = ClearingMethod.STANDARD):
 		"""Prints the grid to the screen using a buffer."""
+
 		tmp = self.ctx.copy()
 
 		if self.sprites != []:
 
 			for sprite in self.sprites:
 				tmp[sprite.pos[1]][sprite.pos[0]] = sprite.color
 
 		if len(tmp)%2 == 1:
-			tmp.append([Presets.none() for i in range(self.size)])
+			tmp.append([Presets.EMPTY for i in range(self.size)])
 		
-		out(tmp, screenclearing)  
+		out(tmp, clearingmethod)  
 
 class Sprite:
 
 	def __init__(self, pos = (0,0), color = spritecolor):
 		self.pos = pos
 		self.color = color
```

### Comparing `cgepy-0.7.3/cge/colors.py` & `cgepy-0.7.4/cge/colors.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 		else:
 			self.background = ""
 			self.fore = ""
 
 	
 
 class Presets:
-	def black(): return Color(0,0,0)
-	def red(): return Color(200,0,0)
-	def yellow(): return Color(200,200,0)
-	def green(): return Color(0,200,0)
-	def blue(): return Color(0,0,200)
-	def magenta(): return Color(200,0,200)
-	def white(): return Color(200,200,200)
-	def none(): return Color(0,0,0,True)
+	BLACK = Color(0,0,0)
+	RED = Color(200,0,0)
+	YELLOW = Color(200,200,0)
+	GREEN = Color(0,200,0)
+	BLUE = Color(0,0,200)
+	MAGENTA = Color(200,0,200)
+	WHITE = Color(200,200,200)
+	EMPTY = Color(0,0,0,True)
```

### Comparing `cgepy-0.7.3/cge/ext/legacy/func.py` & `cgepy-0.7.4/cge/ext/legacy/func.py`

 * *Files identical despite different names*

### Comparing `cgepy-0.7.3/cge/ext/legacy/text.py` & `cgepy-0.7.4/cge/ext/legacy/text.py`

 * *Files identical despite different names*

### Comparing `cgepy-0.7.3/PKG-INFO` & `cgepy-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgePy
-Version: 0.7.3
+Version: 0.7.4
 Summary: A lightweight terminal graphics engine
 Home-page: https://github.com/catbox305/cge
 License: MIT
 Author: catbox305
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

