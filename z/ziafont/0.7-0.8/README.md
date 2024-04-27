# Comparing `tmp/ziafont-0.7.tar.gz` & `tmp/ziafont-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziafont-0.7.tar", last modified: Fri Dec 29 18:57:12 2023, max compression
+gzip compressed data, was "ziafont-0.8.tar", last modified: Sat Apr 27 14:37:41 2024, max compression
```

## Comparing `ziafont-0.7.tar` & `ziafont-0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2023-12-29 18:57:12.975767 ziafont-0.7/
--rw-rw-r--   0 collin    (1000) collin    (1000)     1065 2023-12-10 21:15:20.000000 ziafont-0.7/LICENSE.txt
--rw-r--r--   0 collin    (1000) collin    (1000)     1847 2023-12-29 18:57:12.975767 ziafont-0.7/PKG-INFO
--rw-rw-r--   0 collin    (1000) collin    (1000)      749 2023-12-10 21:15:20.000000 ziafont-0.7/README.md
--rw-rw-r--   0 collin    (1000) collin    (1000)       80 2023-12-10 21:15:20.000000 ziafont-0.7/pyproject.toml
--rw-rw-r--   0 collin    (1000) collin    (1000)     1191 2023-12-29 18:57:12.975767 ziafont-0.7/setup.cfg
-drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2023-12-29 18:57:12.971767 ziafont-0.7/ziafont/
--rw-rw-r--   0 collin    (1000) collin    (1000)       77 2023-12-29 18:09:17.000000 ziafont-0.7/ziafont/__init__.py
--rw-rw-r--   0 collin    (1000) collin    (1000)     3549 2023-12-10 21:15:20.000000 ziafont-0.7/ziafont/cmap.py
--rw-rw-r--   0 collin    (1000) collin    (1000)      579 2023-12-10 21:15:20.000000 ziafont-0.7/ziafont/config.py
--rw-rw-r--   0 collin    (1000) collin    (1000)    26460 2023-12-29 03:29:14.000000 ziafont-0.7/ziafont/font.py
--rw-rw-r--   0 collin    (1000) collin    (1000)     2876 2023-12-29 03:27:36.000000 ziafont-0.7/ziafont/fontread.py
-drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2023-12-29 18:57:12.975767 ziafont-0.7/ziafont/fonts/
--rw-rw-r--   0 collin    (1000) collin    (1000)   757076 2023-12-10 21:15:20.000000 ziafont-0.7/ziafont/fonts/DejaVuSans.ttf
--rw-rw-r--   0 collin    (1000) collin    (1000)        0 2023-12-10 21:15:20.000000 ziafont-0.7/ziafont/fonts/__init__.py
--rw-rw-r--   0 collin    (1000) collin    (1000)     1974 2023-12-10 21:15:20.000000 ziafont-0.7/ziafont/fonttypes.py
--rw-rw-r--   0 collin    (1000) collin    (1000)     7609 2023-12-29 03:27:37.000000 ziafont-0.7/ziafont/glyph.py
--rw-rw-r--   0 collin    (1000) collin    (1000)    24741 2023-12-10 21:15:20.000000 ziafont-0.7/ziafont/glyphcff.py
--rw-rw-r--   0 collin    (1000) collin    (1000)     7293 2023-12-10 21:15:20.000000 ziafont-0.7/ziafont/glyphglyf.py
--rw-rw-r--   0 collin    (1000) collin    (1000)    10801 2023-12-10 21:15:20.000000 ziafont-0.7/ziafont/glyphinspect.py
--rw-rw-r--   0 collin    (1000) collin    (1000)    15473 2023-12-29 03:31:43.000000 ziafont-0.7/ziafont/gpos.py
--rw-rw-r--   0 collin    (1000) collin    (1000)    25498 2023-12-29 03:27:37.000000 ziafont-0.7/ziafont/gsub.py
--rw-rw-r--   0 collin    (1000) collin    (1000)        0 2023-12-10 21:15:20.000000 ziafont-0.7/ziafont/py.typed
--rw-rw-r--   0 collin    (1000) collin    (1000)     6410 2023-12-10 21:15:20.000000 ziafont-0.7/ziafont/svgpath.py
--rw-rw-r--   0 collin    (1000) collin    (1000)     6616 2023-12-10 21:15:20.000000 ziafont-0.7/ziafont/tables.py
-drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2023-12-29 18:57:12.975767 ziafont-0.7/ziafont.egg-info/
--rw-r--r--   0 collin    (1000) collin    (1000)     1847 2023-12-29 18:57:12.000000 ziafont-0.7/ziafont.egg-info/PKG-INFO
--rw-rw-r--   0 collin    (1000) collin    (1000)      534 2023-12-29 18:57:12.000000 ziafont-0.7/ziafont.egg-info/SOURCES.txt
--rw-rw-r--   0 collin    (1000) collin    (1000)        1 2023-12-29 18:57:12.000000 ziafont-0.7/ziafont.egg-info/dependency_links.txt
--rw-rw-r--   0 collin    (1000) collin    (1000)        1 2023-12-29 03:11:54.000000 ziafont-0.7/ziafont.egg-info/not-zip-safe
--rw-rw-r--   0 collin    (1000) collin    (1000)        8 2023-12-29 18:57:12.000000 ziafont-0.7/ziafont.egg-info/top_level.txt
+drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2024-04-27 14:37:41.075144 ziafont-0.8/
+-rw-rw-r--   0 collin    (1000) collin    (1000)     1065 2024-04-21 14:52:33.000000 ziafont-0.8/LICENSE.txt
+-rw-r--r--   0 collin    (1000) collin    (1000)     1847 2024-04-27 14:37:41.075144 ziafont-0.8/PKG-INFO
+-rw-rw-r--   0 collin    (1000) collin    (1000)      749 2023-12-10 21:15:20.000000 ziafont-0.8/README.md
+-rw-rw-r--   0 collin    (1000) collin    (1000)       80 2023-12-10 21:15:20.000000 ziafont-0.8/pyproject.toml
+-rw-rw-r--   0 collin    (1000) collin    (1000)     1191 2024-04-27 14:37:41.075144 ziafont-0.8/setup.cfg
+drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2024-04-27 14:37:41.071144 ziafont-0.8/ziafont/
+-rw-rw-r--   0 collin    (1000) collin    (1000)       77 2024-04-27 03:31:13.000000 ziafont-0.8/ziafont/__init__.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     3549 2023-12-10 21:15:20.000000 ziafont-0.8/ziafont/cmap.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)      579 2023-12-10 21:15:20.000000 ziafont-0.8/ziafont/config.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    26750 2024-02-27 02:36:56.000000 ziafont-0.8/ziafont/font.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     2876 2023-12-29 03:27:36.000000 ziafont-0.8/ziafont/fontread.py
+drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2024-04-27 14:37:41.075144 ziafont-0.8/ziafont/fonts/
+-rw-rw-r--   0 collin    (1000) collin    (1000)   757076 2023-12-10 21:15:20.000000 ziafont-0.8/ziafont/fonts/DejaVuSans.ttf
+-rw-rw-r--   0 collin    (1000) collin    (1000)        0 2023-12-10 21:15:20.000000 ziafont-0.8/ziafont/fonts/__init__.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     1974 2023-12-10 21:15:20.000000 ziafont-0.8/ziafont/fonttypes.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     7609 2023-12-29 03:27:37.000000 ziafont-0.8/ziafont/glyph.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    24741 2023-12-10 21:15:20.000000 ziafont-0.8/ziafont/glyphcff.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     7293 2023-12-10 21:15:20.000000 ziafont-0.8/ziafont/glyphglyf.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    10801 2023-12-10 21:15:20.000000 ziafont-0.8/ziafont/glyphinspect.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    15473 2023-12-29 03:31:43.000000 ziafont-0.8/ziafont/gpos.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    25498 2023-12-29 03:27:37.000000 ziafont-0.8/ziafont/gsub.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)        0 2023-12-10 21:15:20.000000 ziafont-0.8/ziafont/py.typed
+-rw-rw-r--   0 collin    (1000) collin    (1000)     6410 2023-12-10 21:15:20.000000 ziafont-0.8/ziafont/svgpath.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     6616 2023-12-10 21:15:20.000000 ziafont-0.8/ziafont/tables.py
+drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2024-04-27 14:37:41.075144 ziafont-0.8/ziafont.egg-info/
+-rw-r--r--   0 collin    (1000) collin    (1000)     1847 2024-04-27 14:37:41.000000 ziafont-0.8/ziafont.egg-info/PKG-INFO
+-rw-rw-r--   0 collin    (1000) collin    (1000)      534 2024-04-27 14:37:41.000000 ziafont-0.8/ziafont.egg-info/SOURCES.txt
+-rw-rw-r--   0 collin    (1000) collin    (1000)        1 2024-04-27 14:37:41.000000 ziafont-0.8/ziafont.egg-info/dependency_links.txt
+-rw-rw-r--   0 collin    (1000) collin    (1000)        1 2023-12-29 03:11:54.000000 ziafont-0.8/ziafont.egg-info/not-zip-safe
+-rw-rw-r--   0 collin    (1000) collin    (1000)        8 2024-04-27 14:37:41.000000 ziafont-0.8/ziafont.egg-info/top_level.txt
```

### Comparing `ziafont-0.7/LICENSE.txt` & `ziafont-0.8/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021-2023 Collin J. Delker
+Copyright (c) 2021-2024 Collin J. Delker
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ziafont-0.7/PKG-INFO` & `ziafont-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziafont
-Version: 0.7
+Version: 0.8
 Summary: Convert TTF/OTF font glyphs to SVG paths
 Home-page: https://ziafont.readthedocs.io
 Author: Collin J. Delker
 Author-email: code@collindelker.com
 License: MIT
 Project-URL: Documentation, https://ziafont.readthedocs.io
 Project-URL: Source Code, https://github.com/cdelker/ziafont
```

### Comparing `ziafont-0.7/README.md` & `ziafont-0.8/README.md`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/setup.cfg` & `ziafont-0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/cmap.py` & `ziafont-0.8/ziafont/cmap.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/config.py` & `ziafont-0.8/ziafont/config.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/font.py` & `ziafont-0.8/ziafont/font.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,20 @@
         self.valign = valign
         self.color = color
         self.rotation = rotation
         self.rotation_mode = rotation_mode
         self.size = size if size else config.fontsize
         self.linespacing = linespacing
         if font is None or isinstance(font, str):
-            self.font = Font(font)
+            if font in loadedfonts:
+                self.font = loadedfonts[font]
+            else:
+                # Load the font and cache it for later
+                self.font = Font(font)
+                loadedfonts[str(font)] = self.font
         else:
             self.font = font
         self._symbols = self._buildstring()
 
     def svgxml(self) -> ET.Element:
         ''' Get SVG XML element '''
         svg = ET.Element('svg')
@@ -592,15 +597,15 @@
                         if not placexy.mkmk:  # Relative to base glyph
                             dx = dy = 0
                         dx += (placexy.dx - xadvance) * scale
                         dy += -placexy.dy * scale
                     else:
                         dx = dy = 0
                 else:
-                    dx = dy = 0  # Don't reset, may need these for mark-to-mark p[
+                    dx = dy = 0  # Don't reset, may need these for mark-to-mark
 
                 lineglyphs.append((glyph, x+dx, dy))                
                 xadvance = glyph.advance(nextglyph)
                 x += xadvance * scale
 
             if glyph.bbox.xmax > xadvance:
                 # Make linewidth a bit wider to grab right edge
@@ -621,21 +626,24 @@
             else:  # halign = 'left'
                 leftshift = 0
             for glyph, x, dy in lineglyphs:
                 elm = glyph.place(x+leftshift, yvals[lineidx]+dy, self.size)
                 if elm is not None:
                     word.append(elm)
 
-        ymin = yvals[0] - self.font.info.layout.ymax*scale
-        ymax = yvals[-1] - self.font.info.layout.ymin*scale
+        ymax = yvals[-1] - min(glyph[0].bbox.ymin for glyph in allglyphs[-1])*scale
+        ymin = yvals[0] - max(glyph[0].bbox.ymax for glyph in allglyphs[0])*scale
 
         if not config.svg2:
             symbols = []
         return Symbols(word, symbols, totwidth, xmin, ymin, ymax)
 
     def getsize(self) -> tuple[float, float]:
         ''' Calculate width and height (including ascent/descent) of string '''
         return self._symbols.width, self._symbols.ymax-self._symbols.ymin
 
     def getyofst(self) -> float:
         ''' Y-shift from bottom of bbox to 0 '''
         return -self._symbols.ymax
+
+
+loadedfonts: Dict[str, Font] = {}
```

### Comparing `ziafont-0.7/ziafont/fontread.py` & `ziafont-0.8/ziafont/fontread.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/fonts/DejaVuSans.ttf` & `ziafont-0.8/ziafont/fonts/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/fonttypes.py` & `ziafont-0.8/ziafont/fonttypes.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/glyph.py` & `ziafont-0.8/ziafont/glyph.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/glyphcff.py` & `ziafont-0.8/ziafont/glyphcff.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/glyphglyf.py` & `ziafont-0.8/ziafont/glyphglyf.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/glyphinspect.py` & `ziafont-0.8/ziafont/glyphinspect.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/gpos.py` & `ziafont-0.8/ziafont/gpos.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/gsub.py` & `ziafont-0.8/ziafont/gsub.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/svgpath.py` & `ziafont-0.8/ziafont/svgpath.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont/tables.py` & `ziafont-0.8/ziafont/tables.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.7/ziafont.egg-info/PKG-INFO` & `ziafont-0.8/ziafont.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziafont
-Version: 0.7
+Version: 0.8
 Summary: Convert TTF/OTF font glyphs to SVG paths
 Home-page: https://ziafont.readthedocs.io
 Author: Collin J. Delker
 Author-email: code@collindelker.com
 License: MIT
 Project-URL: Documentation, https://ziafont.readthedocs.io
 Project-URL: Source Code, https://github.com/cdelker/ziafont
```

### Comparing `ziafont-0.7/ziafont.egg-info/SOURCES.txt` & `ziafont-0.8/ziafont.egg-info/SOURCES.txt`

 * *Files identical despite different names*

