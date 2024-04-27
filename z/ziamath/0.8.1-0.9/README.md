# Comparing `tmp/ziamath-0.8.1.tar.gz` & `tmp/ziamath-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziamath-0.8.1.tar", last modified: Sun May 28 20:57:35 2023, max compression
+gzip compressed data, was "ziamath-0.9.tar", last modified: Fri Dec 29 19:03:46 2023, max compression
```

## Comparing `ziamath-0.8.1.tar` & `ziamath-0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 20:57:35.737459 ziamath-0.8.1/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1065 2023-04-22 17:44:45.000000 ziamath-0.8.1/LICENSE.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1730 2023-05-28 20:57:35.737459 ziamath-0.8.1/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      573 2023-05-17 03:54:18.000000 ziamath-0.8.1/README.md
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       80 2023-04-22 17:44:41.000000 ziamath-0.8.1/pyproject.toml
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1298 2023-05-28 20:57:35.739460 ziamath-0.8.1/setup.cfg
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 20:57:35.709445 ziamath-0.8.1/ziamath/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      432 2023-05-28 20:56:36.000000 ziamath-0.8.1/ziamath/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2096 2023-05-22 01:13:13.000000 ziamath-0.8.1/ziamath/__main__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1899 2023-05-28 20:46:33.000000 ziamath-0.8.1/ziamath/config.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10494 2023-05-20 17:39:12.000000 ziamath-0.8.1/ziamath/drawable.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    40482 2023-04-15 17:19:13.000000 ziamath-0.8.1/ziamath/escape_codes.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      998 2023-04-15 17:19:13.000000 ziamath-0.8.1/ziamath/escapes.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 20:57:35.716448 ziamath-0.8.1/ziamath/fonts/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1517704 2023-04-15 17:19:13.000000 ziamath-0.8.1/ziamath/fonts/STIXTwoMath-Regular.ttf
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2023-04-15 17:19:13.000000 ziamath-0.8.1/ziamath/fonts/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      793 2023-05-16 02:20:45.000000 ziamath-0.8.1/ziamath/mathfont.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    26767 2023-05-20 22:51:50.000000 ziamath-0.8.1/ziamath/mathtable.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 20:57:35.737459 ziamath-0.8.1/ziamath/nodes/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      453 2023-05-21 22:28:30.000000 ziamath-0.8.1/ziamath/nodes/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4453 2023-05-19 01:50:35.000000 ziamath-0.8.1/ziamath/nodes/menclose.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5347 2023-05-28 01:58:50.000000 ziamath-0.8.1/ziamath/nodes/mfenced.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4252 2023-05-20 22:02:32.000000 ziamath-0.8.1/ziamath/nodes/mfrac.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7591 2023-05-28 02:13:47.000000 ziamath-0.8.1/ziamath/nodes/mnode.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3343 2023-05-27 03:44:25.000000 ziamath-0.8.1/ziamath/nodes/mnumber.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3634 2023-05-28 01:59:40.000000 ziamath-0.8.1/ziamath/nodes/moperator.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4330 2023-05-20 03:46:23.000000 ziamath-0.8.1/ziamath/nodes/mroot.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6311 2023-05-21 17:26:37.000000 ziamath-0.8.1/ziamath/nodes/mrow.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2440 2023-05-20 21:57:21.000000 ziamath-0.8.1/ziamath/nodes/mspace.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11336 2023-05-27 03:42:46.000000 ziamath-0.8.1/ziamath/nodes/msubsup.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3579 2023-05-20 21:59:03.000000 ziamath-0.8.1/ziamath/nodes/mtable.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10389 2023-05-20 18:34:20.000000 ziamath-0.8.1/ziamath/nodes/munderover.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1993 2023-05-18 01:26:19.000000 ziamath-0.8.1/ziamath/nodes/nodetools.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    36431 2023-05-28 02:10:18.000000 ziamath-0.8.1/ziamath/operators.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    80668 2023-05-20 22:40:49.000000 ziamath-0.8.1/ziamath/operators_mml4.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2023-04-15 17:19:13.000000 ziamath-0.8.1/ziamath/py.typed
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     9856 2023-05-28 20:47:36.000000 ziamath-0.8.1/ziamath/styles.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    22219 2023-05-27 01:09:49.000000 ziamath-0.8.1/ziamath/zmath.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 20:57:35.714447 ziamath-0.8.1/ziamath.egg-info/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1730 2023-05-28 20:57:35.000000 ziamath-0.8.1/ziamath.egg-info/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      903 2023-05-28 20:57:35.000000 ziamath-0.8.1/ziamath.egg-info/SOURCES.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-05-28 20:57:35.000000 ziamath-0.8.1/ziamath.egg-info/dependency_links.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-05-19 21:05:39.000000 ziamath-0.8.1/ziamath.egg-info/not-zip-safe
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       28 2023-05-28 20:57:35.000000 ziamath-0.8.1/ziamath.egg-info/requires.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        8 2023-05-28 20:57:35.000000 ziamath-0.8.1/ziamath.egg-info/top_level.txt
+drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2023-12-29 19:03:45.997800 ziamath-0.9/
+-rw-rw-r--   0 collin    (1000) collin    (1000)     1065 2023-12-10 21:15:26.000000 ziamath-0.9/LICENSE.txt
+-rw-r--r--   0 collin    (1000) collin    (1000)     1835 2023-12-29 19:03:45.997800 ziamath-0.9/PKG-INFO
+-rw-rw-r--   0 collin    (1000) collin    (1000)      573 2023-12-10 21:15:26.000000 ziamath-0.9/README.md
+-rw-rw-r--   0 collin    (1000) collin    (1000)       80 2023-12-10 21:15:26.000000 ziamath-0.9/pyproject.toml
+-rw-rw-r--   0 collin    (1000) collin    (1000)     1336 2023-12-29 19:03:45.997800 ziamath-0.9/setup.cfg
+drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2023-12-29 19:03:45.993800 ziamath-0.9/ziamath/
+-rw-rw-r--   0 collin    (1000) collin    (1000)      446 2023-12-29 18:10:58.000000 ziamath-0.9/ziamath/__init__.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     2096 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/__main__.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     1899 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/config.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    10564 2023-12-23 22:02:08.000000 ziamath-0.9/ziamath/drawable.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    40482 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/escape_codes.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)      998 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/escapes.py
+drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2023-12-29 19:03:45.997800 ziamath-0.9/ziamath/fonts/
+-rw-rw-r--   0 collin    (1000) collin    (1000)  1517704 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/fonts/STIXTwoMath-Regular.ttf
+-rw-rw-r--   0 collin    (1000) collin    (1000)        0 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/fonts/__init__.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)      793 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/mathfont.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    26901 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/mathtable.py
+drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2023-12-29 19:03:45.997800 ziamath-0.9/ziamath/nodes/
+-rw-rw-r--   0 collin    (1000) collin    (1000)      453 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/nodes/__init__.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     4453 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/nodes/menclose.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     5884 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/nodes/mfenced.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     4658 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/nodes/mfrac.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     8327 2023-12-29 16:54:09.000000 ziamath-0.9/ziamath/nodes/mnode.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     5352 2023-12-29 17:04:23.000000 ziamath-0.9/ziamath/nodes/mnumber.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     3634 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/nodes/moperator.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     4330 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/nodes/mroot.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     6534 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/nodes/mrow.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     2470 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/nodes/mspace.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    11853 2023-12-29 17:16:03.000000 ziamath-0.9/ziamath/nodes/msubsup.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     3579 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/nodes/mtable.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    10528 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/nodes/munderover.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     1994 2023-12-23 22:00:44.000000 ziamath-0.9/ziamath/nodes/nodetools.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    36375 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/operators.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)        0 2023-12-10 21:15:26.000000 ziamath-0.9/ziamath/py.typed
+-rw-rw-r--   0 collin    (1000) collin    (1000)     9876 2023-12-23 22:02:08.000000 ziamath-0.9/ziamath/styles.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)     1451 2023-12-29 03:51:03.000000 ziamath-0.9/ziamath/tex.py
+-rw-rw-r--   0 collin    (1000) collin    (1000)    21130 2023-12-23 22:02:09.000000 ziamath-0.9/ziamath/zmath.py
+drwxrwxr-x   0 collin    (1000) collin    (1000)        0 2023-12-29 19:03:45.997800 ziamath-0.9/ziamath.egg-info/
+-rw-r--r--   0 collin    (1000) collin    (1000)     1835 2023-12-29 19:03:45.000000 ziamath-0.9/ziamath.egg-info/PKG-INFO
+-rw-rw-r--   0 collin    (1000) collin    (1000)      892 2023-12-29 19:03:45.000000 ziamath-0.9/ziamath.egg-info/SOURCES.txt
+-rw-rw-r--   0 collin    (1000) collin    (1000)        1 2023-12-29 19:03:45.000000 ziamath-0.9/ziamath.egg-info/dependency_links.txt
+-rw-rw-r--   0 collin    (1000) collin    (1000)        1 2023-12-29 03:12:05.000000 ziamath-0.9/ziamath.egg-info/not-zip-safe
+-rw-rw-r--   0 collin    (1000) collin    (1000)       26 2023-12-29 19:03:45.000000 ziamath-0.9/ziamath.egg-info/requires.txt
+-rw-rw-r--   0 collin    (1000) collin    (1000)        8 2023-12-29 19:03:45.000000 ziamath-0.9/ziamath.egg-info/top_level.txt
```

### Comparing `ziamath-0.8.1/LICENSE.txt` & `ziamath-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ziamath-0.8.1/PKG-INFO` & `ziamath-0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: ziamath
-Version: 0.8.1
+Version: 0.9
 Summary: Render MathML and LaTeX Math to SVG in pure Python without Latex installation
 Home-page: https://ziamath.readthedocs.io
 Author: Collin J. Delker
 Author-email: code@collindelker.com
 License: MIT
 Project-URL: Documentation, https://ziamath.readthedocs.io
 Project-URL: Source Code, https://github.com/cdelker/ziamath
 Keywords: MathML,LaTeX,math,font,truetype,opentype,svg
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: ziafont>=0.7
+Requires-Dist: latex2mathml
 
 # ziamath
 
 Render MathML or LaTeX Math expressions as SVG using pure Python. Does not require a Latex installation, nor a network connection.
 
 Ziamath comes with the STIXTwoMath-Regular font installed for use by default.
 Other Math-enabled Open Type fonts (TTF or OTF files) may also be used.
```

### Comparing `ziamath-0.8.1/README.md` & `ziamath-0.9/README.md`

 * *Files identical despite different names*

### Comparing `ziamath-0.8.1/setup.cfg` & `ziamath-0.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Intended Audience :: Education
 	Intended Audience :: Science/Research
 	Intended Audience :: End Users/Desktop
 	Intended Audience :: Developers
 	Topic :: Scientific/Engineering :: Mathematics
 
 [options]
 packages = find:
 zip_safe = False
 python_requires = >= 3.8
 include_package_data = True
 install_requires = 
-	ziafont>=0.6a1
+	ziafont>=0.7
 	latex2mathml
 
 [options.package_data]
 ziamath = 
 	py.typed
 ziamath.fonts = 
 	*.ttf
```

### Comparing `ziamath-0.8.1/ziamath/__main__.py` & `ziamath-0.9/ziamath/__main__.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8.1/ziamath/config.py` & `ziamath-0.9/ziamath/config.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8.1/ziamath/drawable.py` & `ziamath-0.9/ziamath/drawable.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         Args:
             glyph: The glyph to draw
             char: unicode character represented by the glyph
             size: point size
             style: font MathStyle
     '''
     def __init__(self, glyph: SimpleGlyph, char: str, size: float,
-                 style: MathStyle = None, **kwargs):
+                 style: Optional[MathStyle] = None, **kwargs):
         super().__init__()
         self.glyph = glyph
         self.char = char
         self.size = size
         self.phantom = kwargs.get('phantom', False)
         self.style = style if style else MathStyle()
         self._funits_to_pts = self.size / self.glyph.font.info.layout.unitsperem
@@ -103,15 +103,15 @@
         x += self.funit_to_points(self.glyph.advance())
         return x, y
 
 
 class HLine(Drawable):
     ''' Horizontal Line. '''
     def __init__(self, length: float, lw: float,
-                 style: MathStyle = None, **kwargs):
+                 style: Optional[MathStyle] = None, **kwargs):
         super().__init__()
         self.length = length
         self.lw = lw
         self.phantom = kwargs.get('phantom', False)
         self.bbox = BBox(0, self.length, -self.lw/2, self.lw/2)
         self.style = style if style else MathStyle()
 
@@ -135,15 +135,15 @@
                 bar.attrib['fill'] = str(self.style.mathcolor)
         return x+self.length, y
 
 
 class VLine(Drawable):
     ''' Vertical Line. '''
     def __init__(self, height: float, lw: float,
-                 style: MathStyle = None, **kwargs):
+                 style: Optional[MathStyle] = None, **kwargs):
         super().__init__()
         self.height = height
         self.lw = lw
         self.phantom = kwargs.get('phantom', False)
         self.bbox = BBox(0, self.lw, 0, self.height)
         self.style = style if style else MathStyle()
 
@@ -167,16 +167,16 @@
                 bar.attrib['fill'] = str(self.style.mathcolor)
         return x, y
 
 
 class Box(Drawable):
     ''' Box '''
     def __init__(self, width: float, height: float, lw: float,
-                 cornerradius: float = None,
-                 style: MathStyle = None, **kwargs):
+                 cornerradius: Optional[float] = None,
+                 style: Optional[MathStyle] = None, **kwargs):
         super().__init__()
         self.width = width
         self.height = height
         self.cornerradius = cornerradius
         self.lw = lw
         self.phantom = kwargs.get('phantom', False)
         self.bbox = BBox(0, self.width, 0, self.height)
@@ -205,15 +205,15 @@
         return x+self.width, y
 
 
 class Diagonal(Drawable):
     ''' Diagonal Line - corners of Box '''
     def __init__(self, width: float, height: float, lw: float,
                  arrow: bool = False,
-                 style: MathStyle = None, **kwargs):
+                 style: Optional[MathStyle] = None, **kwargs):
         super().__init__()
         self.width = width
         self.height = height
         self.lw = lw
         self.arrow = arrow
         self.phantom = kwargs.get('phantom', False)
         self.bbox = BBox(0, self.width, 0, self.height)
@@ -257,15 +257,15 @@
 
         return x+self.width, y
 
 
 class Ellipse(Drawable):
     ''' Ellipse '''
     def __init__(self, width: float, height: float, lw: float,
-                 style: MathStyle = None, **kwargs):
+                 style: Optional[MathStyle] = None, **kwargs):
         super().__init__()
         self.width = width
         self.height = height
         self.lw = lw
         self.phantom = kwargs.get('phantom', False)
         self.bbox = BBox(0, self.width, 0, self.height)
         self.style = style if style else MathStyle()
```

### Comparing `ziamath-0.8.1/ziamath/escape_codes.py` & `ziamath-0.9/ziamath/escape_codes.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8.1/ziamath/escapes.py` & `ziamath-0.9/ziamath/escapes.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8.1/ziamath/fonts/STIXTwoMath-Regular.ttf` & `ziamath-0.9/ziamath/fonts/STIXTwoMath-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ziamath-0.8.1/ziamath/mathfont.py` & `ziamath-0.9/ziamath/mathfont.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8.1/ziamath/mathtable.py` & `ziamath-0.9/ziamath/mathtable.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,19 +411,23 @@
             ymax = int(glyphs[-1].path.bbox.ymax + offsets[-1])
         else:
             xmin = int(glyphs[0].path.bbox.xmin)
             xmax = int(glyphs[-1].path.bbox.xmax + offsets[-1])
             ymin = min([g.path.bbox.ymin for g in glyphs])
             ymax = max([g.path.bbox.ymax for g in glyphs])
         bbox = BBox(xmin, xmax, ymin, ymax)
+        self._xadvance = max([g.advance() for g in glyphs])
         super().__init__(index, [], bbox, font)
 
     def advance(self, nextchr=None) -> float:
         ''' X-advance '''
-        return self.bbox.xmax
+        if self.vert:
+            return self._xadvance
+        else:
+            return self.bbox.xmax
 
     def svgpath(self, x0: float = 0, y0: float = 0,
                 scale_factor: float = 1) -> Optional[ET.Element]:
         ''' Get svg <path> element for glyph, normalized to 12-point font '''
         element = ET.Element('g')
 
         for glyph, ofst in zip(self.glyphs, self.offsets):
```

### Comparing `ziamath-0.8.1/ziamath/nodes/menclose.py` & `ziamath-0.9/ziamath/nodes/menclose.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8.1/ziamath/nodes/mfenced.py` & `ziamath-0.9/ziamath/nodes/mfenced.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 ''' <mfenced> math element '''
 from typing import Union
 from itertools import chain, zip_longest
+from contextlib import suppress
 import xml.etree.ElementTree as ET
 
 from ziafont.fonttypes import BBox
 
 from .. import operators
 from ..drawable import Glyph
 from .mnode import Mnode
-from .msubsup import Msub, Msup, Msubsup
-from .mfrac import Mfrac
 
 
 class Mfenced(Mnode, tag='mfenced'):
     ''' Mfence element. Puts contents in parenthesis or other fence glyphs, with
         optional separators between components.
     '''
     def __init__(self, element: ET.Element, parent: 'Mnode', **kwargs):
         super().__init__(element, parent, **kwargs)
         self.openchr = element.get('open', '(')
         self.closechr = element.get('close', ')')
         self.separators = element.get('separators', ',').replace(' ', '')
+        self._xadvance = 0.
         self._setup(**kwargs)
 
+    def xadvance(self) -> float:
+        ''' X-advance for the Mrow '''
+        return self._xadvance
+
     def _setup(self, **kwargs) -> None:
         separator_elms = [ET.fromstring(f'<mo>{k}</mo>') for k in self.separators]
         fencedelms: Union[list[ET.Element], ET.Element] = []
         # Insert separators
         if len(self.element) > 1 and len(self.separators) > 0:
             fencedelms = list(chain.from_iterable(zip_longest(
                     self.element, separator_elms, fillvalue=separator_elms[-1])))   # flatten
@@ -46,79 +50,87 @@
         mglyph = Glyph(
             openglyph, self.openchr, self.glyphsize, self.style, **kwargs)
         if len(mrow.nodes) == 0:
             # Opening fence with nothing in it
             fencebbox = mglyph.bbox
             xadvance = mglyph.xadvance()
         else:
-            # height-adjusted fence glyph variant
-            openglyph = self.font.math.variant_minmax(openglyph.index,
-                                                      self.points_to_units(mrow.bbox.ymin),
-                                                      self.points_to_units(mrow.bbox.ymax))
+            ymin = self.points_to_units(mrow.bbox.ymin)
+            if 'minsize' in self.element.attrib:
+                ymax = self.points_to_units(self.size_px(self.element.get('minsize', '0'))) + ymin
+                openglyph = self.font.math.variant(openglyph.index, ymax-ymin)
+            else:
+                ymax = self.points_to_units(mrow.bbox.ymax)# + ymin
+                openglyph = self.font.math.variant_minmax(openglyph.index,
+                                                          ymin,
+                                                          ymax)
+
             oglyph = Glyph(openglyph, self.openchr, self.glyphsize,
                            self.style, **kwargs)
-
+            
             if self.closechr:
                 closeglyph = self.font.glyph(self.closechr)
-                closeglyph = self.font.math.variant_minmax(closeglyph.index,
-                                                           self.points_to_units(mrow.bbox.ymin),
-                                                           self.points_to_units(mrow.bbox.ymax))
+                if 'minsize' in self.element.attrib:
+                    closeglyph = self.font.math.variant(closeglyph.index, ymax-ymin)
+                else:
+                    closeglyph = self.font.math.variant_minmax(closeglyph.index,
+                                                           ymin,
+                                                           ymax)
                 cglyph = Glyph(closeglyph, self.closechr, self.glyphsize,
                                self.style, **kwargs)
 
             # Rebuild the mrow with the height parameter to get stretchy
             # \middle fences
             mrowelm = ET.Element('mrow')
             mrowelm.extend(fencedelms)
             mrow = Mnode.fromelement(mrowelm, parent=self, height=oglyph.bbox.ymax-oglyph.bbox.ymin)
             fencebbox = mrow.bbox
             xadvance = mrow.xadvance()
 
         self.nodes = []
-        x = yofst = base = 0.
+        x = xmax = yofst = base = 0.
         yglyphmin = yglyphmax = 0.
-        try:
+        with suppress(AttributeError):
             if self.parent.leftsibling():
                 x += self.size_px('verythinmathspace')
-        except AttributeError:
-            pass
 
         if self.openchr:
-            params = operators.get_params(self.openchr, 'prefix')
-            rspace = self.size_px(params.get('rspace', '0'))
             self.nodes.append(oglyph)
             self.nodexy.append((x, yofst))
+            params = operators.get_params(self.openchr, 'prefix')
             x += self.units_to_points(openglyph.advance())
-            x += rspace
+            x += self.size_px(params.get('rspace', '0'))
+            xmax = x
             yglyphmin = min(-yofst+oglyph.bbox.ymin, yglyphmin)
             yglyphmax = max(-yofst+oglyph.bbox.ymax, yglyphmax)
-
+        
+        x += mrow.bbox.xmin
         if len(fencedelms) > 0:
             self.nodes.append(mrow)
             self.nodexy.append((x, base))
+            xmax = max(xmax, x+mrow.bbox.xmax)
             x += xadvance
 
         if self.closechr:
-            try:
+            with suppress(IndexError, AttributeError):
                 # Mfrac, Msub adds space to right, remove it for fence
-                if isinstance(mrow.nodes[-1], (Msub, Msup, Msubsup)):
+                if mrow.nodes[-1].mtag in ['msub', 'msup', 'msubsup']:
                     x -= self.units_to_points(self.font.math.consts.spaceAfterScript)
-                elif isinstance(mrow.nodes[-1], Mfrac):
-                    x -= self.size_px('verythinmathspace')
-            except (IndexError, AttributeError):
-                pass
+                elif mrow.nodes[-1].mtag == 'mfrac':
+                    x -= self.size_px('thinmathspace')
 
             if (lastg := mrow.lastglyph()):
                 if (italicx := self.font.math.italicsCorrection.getvalue(lastg.index)):
                     x += mrow.units_to_points(italicx)
                         
             params = operators.get_params(self.closechr, 'postfix')
-            lspace = self.size_px(params.get('lspace', '0'))
-            x += lspace
+            x += self.size_px(params.get('lspace', '0'))
 
             self.nodes.append(cglyph)
             self.nodexy.append((x, yofst))
             x += self.units_to_points(closeglyph.advance())
+            xmax = max(xmax, x)
             yglyphmin = min(-yofst+cglyph.bbox.ymin, yglyphmin)
             yglyphmax = max(-yofst+cglyph.bbox.ymax, yglyphmax)
 
-        self.bbox = BBox(0, x, min(yglyphmin, fencebbox.ymin), max(yglyphmax, fencebbox.ymax))
+        self.bbox = BBox(0, xmax, min(yglyphmin, fencebbox.ymin), max(yglyphmax, fencebbox.ymax))
+        self._xadvance = xmax
```

### Comparing `ziamath-0.8.1/ziamath/nodes/mfrac.py` & `ziamath-0.9/ziamath/nodes/mfrac.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ''' <mfrac> math element '''
 from xml.etree import ElementTree as ET
 
 from ziafont.fonttypes import BBox
 
 from ..styles import parse_style
+from ..config import config
 from ..drawable import HLine
 from . import Mnode
 
 
 class Mfrac(Mnode, tag='mfrac'):
     ''' Fraction node '''
     # TODO: bevelled attribute for x/y fractions with slanty bar
@@ -29,17 +30,22 @@
         kwargs['frac'] = True
         kwargs.pop('sup', None)
         self.numerator = Mnode.fromelement(self.element[0], parent=self, **kwargs)
         self.denominator = Mnode.fromelement(self.element[1], parent=self, **kwargs)
         self._setup(**kwargs)
 
     def _setup(self, **kwargs) -> None:
-
-        linethick = self.units_to_points(self.font.math.consts.fractionRuleThickness)
+        # Keep fraction bar same thickness as minus sign
+        fbar_glyphsize = max(
+            self.size*(self.font.math.consts.scriptPercentScaleDown/100)**max(0, self.style.scriptlevel-1),
+            self.font.basesize*config.minsizefraction)
+        fracbar_pts_per_unit = fbar_glyphsize/self.font.info.layout.unitsperem
+        linethick = fracbar_pts_per_unit * self.font.math.consts.fractionRuleThickness
         if 'linethickness' in self.element.attrib:
+            # User parameter overrides thickness
             lt = self.element.get('linethickness', '')
             try:
                 linethick = self.size_px(lt)
             except ValueError:
                 linethick = {'thin': linethick * .5,
                              'thick': linethick * 2}.get(lt, linethick)
```

### Comparing `ziamath-0.8.1/ziamath/nodes/mnode.py` & `ziamath-0.9/ziamath/nodes/mnode.py`

 * *Files 8% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     def lastchar(self) -> Optional[str]:
         ''' Get the last character in this node '''
         try:
             return self.nodes[-1].lastchar()
         except IndexError:
             return None
 
-    def size_px(self, size: str, fontsize: float = None) -> float:
+    def size_px(self, size: str, fontsize: Optional[float] = None) -> float:
         ''' Get size in points from the attribute string '''
         if fontsize is None:
             fontsize = self.glyphsize
 
         numsize = {"veryverythinmathspace": f'{1/18}em',
                    "verythinmathspace": f'{2/18}em',
                    "thinmathspace": f'{3/18}em',
@@ -144,24 +144,50 @@
                    "negativethinmathspace": f'{-3/18}em',
                    "negativemediummathspace": f'{-4/18}em',
                    "negativethickmathspace": f'{-5/18}em',
                    "negativeverythickmathspace": f'{-6/18}em',
                    "negativeveryverythickmathspace": f'{-7/18}em',
                    }.get(size, size)
 
-        numsize = numsize.rstrip('px')
         try:
-            pxsize = float(numsize)
+            # Plain number, or value in px
+            pxsize = float(numsize.rstrip('px'))
         except ValueError as exc:
-            if numsize.endswith('em'):
-                pxsize = float(numsize[:-2]) * fontsize
-            elif numsize.endswith('pt'):
-                pxsize = float(numsize[:-2]) * 1.333  # 1.333 points to pixels
-            else:
-                pxsize = 0
+            pass
+        else:
+            return pxsize
+
+        try:
+            # Units are always last 2 chars
+            units = numsize[-2:]
+            value = float(numsize[:-2])
+        except ValueError:
+            return 0
+
+        # Conversion values from:
+        # https://tex.stackexchange.com/questions/8260/what-are-the-various-units-ex-em-in-pt-bp-dd-pc-expressed-in-mm
+        UNITS_TO_PT = {
+            'pt': 1,
+            'mm': 2.84526,
+            'cm': 28.45274,
+            'ex': 4.30554,
+            'em': 10.00002,
+            'bp': 1.00374,
+            'dd': 1.07,
+            'pc': 12,
+            'in': 72.27,
+            'mu': 0.5555,
+        }
+        # Convert units to points, then to pixels (= 1.333 px/pt)
+        pxsize = value * UNITS_TO_PT.get(units, 0) * 1.333
+
+        if units in ['em', 'ex', 'mu']:
+            # These are fontsize dependent, table is based
+            # on 10-point font
+            pxsize *= fontsize/10
         return pxsize
 
     def draw(self, x: float, y: float, svg: ET.Element) -> tuple[float, float]:
         ''' Draw the node on the SVG
 
             Args:
                 x: Horizontal position in SVG coordinates
```

### Comparing `ziamath-0.8.1/ziamath/nodes/mnumber.py` & `ziamath-0.9/ziamath/nodes/moperator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,97 @@
-''' <mn> number math element '''
+''' <mo> Math Operator Element '''
 import xml.etree.ElementTree as ET
 
 from ziafont.fonttypes import BBox
 
-from ..styles import styledstr, auto_italic
+from ..styles import styledstr
 from ..drawable import Glyph
-from .nodetools import subglyph, elementtext
-from .mnode import Mnode
+from .. import operators
+from . import Mnode
+from .nodetools import elementtext, subglyph
 
 
-class Mnumber(Mnode, tag='mn'):
-    ''' Mnumber node <mn> '''
+class Moperator(Mnode, tag='mo'):
+    ''' Operator math element '''
     def __init__(self, element: ET.Element, parent: 'Mnode', **kwargs):
         super().__init__(element, parent, **kwargs)
-        self.string = self._getstring()
+        self.string = styledstr(elementtext(self.element), self.style.mathvariant)
+        self.form = element.get('form', 'infix')
+
+        # Load parameters from operators table for deciding how much space
+        # to add on either side of the operator
+        self.params = operators.get_params(self.string, self.form)
+        self.params.update(element.attrib)
+        self.width = kwargs.get('width', None)
+        self.height = kwargs.get('height', None)
+
+        minsize = self.size_px(element.get('minsize', '0'))
+        maxsize = self.size_px(element.get('maxsize', '0'))
+        mathsize = self.size_px(self.style.mathsize)
+        if self.height:
+            if minsize:
+                self.height = max(self.height, minsize)
+            if maxsize:
+                self.height = min(self.height, maxsize)
+        else:
+            if mathsize:
+                self.height = mathsize
+            elif minsize:
+                self.height = minsize
+            elif maxsize:
+                self.height = maxsize
+
+        if self.string in ['|', '‖', '∣', '❘'] and self.params.get('fence') == 'true':
+            # Hack around weird spacing with \middle operators
+            self.params['rspace'] = 'thinmathspace'
+
         self._setup(**kwargs)
 
-    def _getstring(self) -> str:
-        ''' Get the styled string for this node '''
-        text = elementtext(self.element)
-        return styledstr(text, self.style.mathvariant)
-
-    def _setup(self, **kwargs) -> None:
-        ymin = 9999.
-        ymax = -9999.
-        x = 0.
-
-        if (leftsibling := self.leftsibling()) and leftsibling.mtag == 'mfenced':
-            x = self.size_px('verythinmathspace')
-
-        for i, char in enumerate(self.string):
-            glyph = self.font.glyph(char)
-            if kwargs.get('sup') or kwargs.get('sub'):
-                glyph = subglyph(glyph, self.font)
-
-            self.nodes.append(
-                Glyph(glyph, char, self.glyphsize, self.style, **kwargs))
-
-            if self.nodes[-1].bbox.xmin < 0:
-                # don't let glyphs run together if xmin < 0
-                x -= self.nodes[-1].bbox.xmin
-            
+    def _setup(self, **kwargs):
+        glyphs = [self.font.glyph(char) for char in self.string]
+
+        if kwargs.get('sup') or kwargs.get('sub'):
+            addspace = False  # Dont add lspace/rspace when in super/subscripts
+            glyphs = [subglyph(g, self.font) for g in glyphs]
+        else:
+            addspace = True
+
+        x = xmax = 0
+        self.nodes = []
+
+        # Add lspace
+        if addspace:
+            x += self.size_px(self.params.get('lspace', '0'))
+
+        ymin = 999
+        ymax = -999
+        for glyph, char in zip(glyphs, self.string):
+            if self.params.get('largeop') == 'true' and self.style.displaystyle:
+                minh = self.font.math.consts.displayOperatorMinHeight
+                glyph = self.font.math.variant(glyph.index, minh, vert=True)
+
+            if self.width:
+                glyph = self.font.math.variant(
+                    glyph.index, self.points_to_units(self.width), vert=False)
+            elif (self.height
+                    and self.params.get('stretchy', 'false') != 'false'):
+                glyph = self.font.math.variant(
+                    glyph.index, self.points_to_units(self.height), vert=True)
 
+            self.nodes.append(Glyph(
+                glyph, char, self.glyphsize, self.style, **kwargs))
             self.nodexy.append((x, 0))
-            nextglyph = self.font.glyph(self.string[i+1]) if i < len(self.string)-1 else None
-            x += self.units_to_points(glyph.advance(nextchr=nextglyph))
+            xmax = max(xmax, x + self.units_to_points(glyph.path.bbox.xmax))
+            x += self.units_to_points(glyph.advance())
             ymin = min(ymin, self.units_to_points(glyph.path.bbox.ymin))
             ymax = max(ymax, self.units_to_points(glyph.path.bbox.ymax))
 
+        if addspace:
+            x += self.size_px(self.params.get('rspace', '0'))
+            xmax = max(xmax, x)
+
         try:
-            xmin = self.nodes[0].bbox.xmin
-            xmax = self.nodexy[-1][0] + max(self.nodes[-1].bbox.xmax,
-                                            self.units_to_points(glyph.advance()))
+            xmin = self.units_to_points(glyphs[0].path.bbox.xmin)
         except IndexError:
-            xmin = 0.
-            xmax = x
+            xmin = 0
+        
         self.bbox = BBox(xmin, xmax, ymin, ymax)
-
-
-class Midentifier(Mnumber, tag='mi'):
-    ''' Number node <mn> '''
-    def _getstring(self) -> str:
-        ''' Get the styled string for the identifier. Applies
-            italics if single-char identifier, and extra whitespace
-            if function (eg 'sin')
-        '''
-        text = elementtext(self.element)
-        if (len(text) == 1
-                and not self.style.mathvariant.italic
-                and not self.style.mathvariant.normal
-                and auto_italic(text)):
-            self.style.mathvariant.italic = True
-
-        if len(text) > 1:
-            text = '\U00002009' + text
-            if self.parent.mtag not in ['msub', 'msup', 'msubsup']:
-                text = text + '\U00002009'
-
-        return styledstr(text, self.style.mathvariant)
-
-
-class Mtext(Mnumber, tag='mtext'):
-    ''' Text Node <mtext> '''
-    def _getstring(self) -> str:
-        string = ''
-        if self.element.text:
-            # Don't use elementtext() since it strips whitespace
-            string = styledstr(self.element.text, self.style.mathvariant)
-        return string
-
-    def _setup(self, **kwargs) -> None:
-        self.font.language('DFLT', '')  # Allow standard kerning to apply
-        super()._setup(**kwargs)
-        self.font.language('math', '')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ziamath-0.8.1/ziamath/nodes/mroot.py` & `ziamath-0.9/ziamath/nodes/mroot.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8.1/ziamath/nodes/mrow.py` & `ziamath-0.9/ziamath/nodes/mrow.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,16 +13,21 @@
 from .mnode import Mnode
 
 
 class Mrow(Mnode, tag='mrow'):
     ''' Math row, list of vertically aligned Mnodes '''
     def __init__(self, element: ET.Element, parent: 'Mnode', **kwargs):
         super().__init__(element, parent, **kwargs)
+        self._xadvance = 0.
         self._setup(**kwargs)
 
+    def xadvance(self) -> float:
+        ''' X-advance for the Mrow '''
+        return self._xadvance
+
     def _break_lines(self) -> list[list[ET.Element]]:
         ''' Break mrow into lines - to handle mspace linebreak (// in latex) '''
         lines = []
         line: list[ET.Element] = []
         for i, child in enumerate(self.element):
             if child.tag == 'mi' and elementtext(child) in operators.names:
                 # Workaround for some latex2mathml operators coming back as identifiers
@@ -55,14 +60,15 @@
                       2 * self.units_to_points(self.font.math.consts.mathLeading))
             self.nodexy.append((0, y))
         xmin = min([n.bbox.xmin for n in self.nodes])
         xmax = max([n.bbox.xmax for n in self.nodes])
         ymin = -y+self.nodes[-1].bbox.ymin
         ymax = self.nodes[0].bbox.ymax
         self.bbox = BBox(xmin, xmax, ymin, ymax)
+        self._xadvance = max([n.xadvance() for n in self.nodes])
 
     def _setup_single_line(self, line: list[ET.Element], **kwargs) -> None:
         ''' Single line mrow '''
         ymax = -9999
         ymin = 9999
         height = kwargs.pop('height', None)
         i = 0
@@ -110,14 +116,15 @@
             self.nodexy.append((x, 0))
             xmax = max(xmax, x + node.bbox.xmax)
             xmin = min([nxy[0]+n.bbox.xmin for nxy, n in zip(self.nodexy, self.nodes)])
             ymax = max(ymax, node.bbox.ymax)
             ymin = min(ymin, node.bbox.ymin)
             x += node.xadvance()
         self.bbox = BBox(xmin, xmax, ymin, ymax)
+        self._xadvance = x
 
     def _setup(self, **kwargs) -> None:
         kwargs = copy(kwargs)
         self.nodes = []
 
         lines = self._break_lines()
         if len(lines) > 1:
```

### Comparing `ziamath-0.8.1/ziamath/nodes/mspace.py` & `ziamath-0.9/ziamath/nodes/mspace.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         if width:
             xmax = xmin + adjust(width, xmax-xmin)
         if height:
             ymax = adjust(height, ymax)
         if depth:
             ymin = -adjust(depth, ymin)
         self.bbox = BBox(xmin, xmax, ymin, ymax)
+        self._xadvance = xmax
 
 
 class Mphantom(Mrow, tag='mphantom'):
     ''' Phantom element. Takes up space but not drawn. '''
     def _setup(self, **kwargs) -> None:
         kwargs['phantom'] = True
         super()._setup(**kwargs)
```

### Comparing `ziamath-0.8.1/ziamath/nodes/msubsup.py` & `ziamath-0.9/ziamath/nodes/msubsup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import xml.etree.ElementTree as ET
 
 from ziafont.fonttypes import BBox
 
 from ..mathfont import MathFont
 from .. import operators
 from .mnode import Mnode
+from .nodetools import elementtext
 
 
 def place_super(base: Mnode, superscript: Mnode, font: MathFont) -> tuple[float, float, float]:
     ''' Superscript. Can be above the operator (like sum) or regular super '''
     if base.params.get('movablelimits') == 'true' and base.style.displaystyle:
         x = (-(base.bbox.xmax - base.bbox.xmin) / 2
              - (superscript.bbox.xmax - superscript.bbox.xmin) / 2)
@@ -38,14 +39,19 @@
         if superscript.mtag in ['mi', 'mn']:
             if firstg and lastg and lastg.index >= 0 and font.math.kernInfo:  # assembled glyphs have idx<0
                 kern, shiftup = font.math.kernsuper(lastg, firstg)
                 x += base.units_to_points(kern)
 
         supy = base.units_to_points(-shiftup)
         xadvance = x + superscript.bbox.xmax
+
+        if base.mtag == 'mi' and len(elementtext(base.element)) > 1:
+            # Add a little space after functions, such as sin^2
+            xadvance += base.size_px('verythinmathspace')
+
     return x, supy, xadvance
 
 
 def place_sub(base: Mnode, subscript: Mnode, font: MathFont) -> tuple[float, float, float]:
     ''' Calculate subscript. Can be below the operator (like sum) or regular sub '''
     if base.params.get('movablelimits') == 'true' and base.style.displaystyle:
         x = -(base.bbox.xmax - base.bbox.xmin) / 2 - (subscript.bbox.xmax - subscript.bbox.xmin) / 2
@@ -72,18 +78,21 @@
             # Ignoring vertical kern otherwise subscripts don't line up
             # across the row which looks weird
             kern, _ = font.math.kernsub(lastg, firstg)
             x += base.units_to_points(kern)
 
         if base.mtag in ['mi', 'mn'] or (base.mtag == 'mo' and not base.string):  # type: ignore
             shiftdn = font.math.consts.subscriptShiftDown
+        elif base.mtag == 'mover' and base._isaccent:  # type: ignore
+            shiftdn = font.math.consts.subscriptShiftDown
         else:
             shiftdn = max(font.math.consts.subscriptShiftDown,
-                      firstg.bbox.ymax - font.math.consts.subscriptTopMax if firstg else 0,
-                      font.math.consts.subscriptBaselineDropMin - base.points_to_units(base.bbox.ymin))
+                          firstg.bbox.ymax - font.math.consts.subscriptTopMax if firstg else 0,
+                          font.math.consts.subscriptBaselineDropMin - base.points_to_units(base.bbox.ymin))
+
         suby = base.units_to_points(shiftdn)
         xadvance = x + subscript.xadvance()
     return x, suby, xadvance
 
 
 class Msup(Mnode, tag='msup'):
     ''' Superscript Node '''
@@ -127,15 +136,18 @@
         self.increase_child_scriptlevel(self.element[1])
         self.subscript = Mnode.fromelement(self.element[1], parent=self, **kwargs)
         self._setup(**kwargs)
 
     def _setup(self, **kwargs) -> None:
         self.nodes.append(self.base)
         self.nodexy.append((0, 0))
-        x = self.base.xadvance()
+        if self.base.mtag == 'mover' and self.base._isaccent:  # type: ignore
+            x = self.base.base_xadvance  # type: ignore
+        else:
+            x = self.base.xadvance()
 
         subx, suby, xadv = place_sub(self.base, self.subscript, self.font)
         self.nodes.append(self.subscript)
         self.nodexy.append((x + subx, suby))
 
         xmin = min(self.base.bbox.xmin, x+subx+self.subscript.bbox.xmin)
         xmax = max(x + xadv, self.base.bbox.xmax, x+subx+self.subscript.bbox.xmax)
```

### Comparing `ziamath-0.8.1/ziamath/nodes/mtable.py` & `ziamath-0.9/ziamath/nodes/mtable.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8.1/ziamath/nodes/munderover.py` & `ziamath-0.9/ziamath/nodes/munderover.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,32 +42,32 @@
 
         Returns:
             x, y: position for over node
     '''
     # Center the node by default
     x = (((base.bbox.xmax - base.bbox.xmin) - (over.bbox.xmax-over.bbox.xmin)) / 2
          - over.bbox.xmin)
-    
+
     if ((lastg := base.lastglyph())
             and node_is_singlechar(base)
             and not isinstance(over, drawable.HLine)):
         # Italic adjustment and font-specific accent attachment,
         # if base is a single glyph
         if (italicx := font.math.italicsCorrection.getvalue(lastg.index)):
             x += base.units_to_points(italicx)
 
         # Use font-specific accent attachment if defined
         if (basex := font.math.topattachment(lastg.index)):
             x = base.units_to_points(basex)
-            
+
             if (node_is_singlechar(over)
                     and (attachx := font.math.topattachment(over.lastglyph().index))):  # type: ignore
                 x -= over.units_to_points(attachx)
             else:
-                x -= (over.bbox.xmax-over.bbox.xmin)/2
+                x -= (over.bbox.xmax-over.bbox.xmin)/2 + over.bbox.xmin
 
     y = -base.bbox.ymax - base.units_to_points(font.math.consts.overbarVerticalGap)
     y += over.bbox.ymin
     return x, y
 
 
 def place_under(base: Mnode,
@@ -147,16 +147,18 @@
         xmin = min(overx+self.over.bbox.xmin, basex+self.base.bbox.xmin)
         xmax = max(overx+self.over.bbox.xmax, basex+self.base.bbox.xmax)
         ymin = self.base.bbox.ymin
         ymax = -overy + self.over.bbox.ymax
         self.bbox = BBox(xmin, xmax, ymin, ymax)
         if not self._isaccent:
             self._xadvance = self.base.xadvance()
+            self.base_xadvance = self._xadvance  # For attaching subscripts
         else:
             self._xadvance = xmax
+            self.base_xadvance = basex + self.base.xadvance()
 
     def xadvance(self) -> float:
         return self._xadvance
 
     def lastglyph(self) -> Optional[SimpleGlyph]:
         ''' Get the last glyph in this node '''
         return self.base.lastglyph()
```

### Comparing `ziamath-0.8.1/ziamath/nodes/nodetools.py` & `ziamath-0.9/ziamath/nodes/nodetools.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             return False
         else:
             return node_is_singlechar(node.nodes[0])  # type:ignore
     return hasattr(node, 'string') and len(node.string) == 1  # type:ignore
 
 
 def subglyph(glyph: SimpleGlyph, font: MathFont) -> SimpleGlyph:
-    ''' Substitute glyphs using font GSUB ssty feature. This
+    r''' Substitute glyphs using font GSUB ssty feature. This
         substitutes glyphs like \prime for use in sub/superscripts.
     '''
     if font.gsub:
         glyphids = font.gsub.sub([glyph.index], font.features)
         if glyphids[0] != glyph.index:
             glyph = font.glyph_fromid(glyphids[0])
     return glyph
```

### Comparing `ziamath-0.8.1/ziamath/operators.py` & `ziamath-0.9/ziamath/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
     ('∋', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &SuchThat;
     ('⫤', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &DoubleLeftTee;
     ('⊨', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &DoubleRightTee;
     ('⊤', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &DownTee;
     ('⊣', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &LeftTee;
     ('⊢', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &RightTee;
     ('⥰', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &RoundImplies;
-    ('|', 'infix'): {'stretchy': 'true',  'lspace': 'verythinmathspace', 'rspace': 'verythinmathspace'},
-    ('‖', 'infix'): {'stretchy': 'true',  'lspace': 'verythinmathspace', 'rspace': 'verythinmathspace'},
+    ('|', 'infix'): {'stretchy': 'true',  'lspace': '0em', 'rspace': '0em'},
+    ('‖', 'infix'): {'stretchy': 'true',  'lspace': '0em', 'rspace': '0em'},
     ('||', 'infix'): {'lspace': '0em', 'rspace': '0em'},
     ('⩔', 'infix'): {'stretchy': 'true',  'lspace': 'mediummathspace', 'rspace': 'mediummathspace'},  # &Or;
     ('&&', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},
     ('⩓', 'infix'): {'stretchy': 'true',  'lspace': 'mediummathspace', 'rspace': 'mediummathspace'},  # &And;
     ('&', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},
     ('!', 'prefix'): {'lspace': '0em', 'rspace': 'thickmathspace'},
     ('⫬', 'prefix'): {'lspace': '0em', 'rspace': 'thickmathspace'},  # &Not;
```

### Comparing `ziamath-0.8.1/ziamath/styles.py` & `ziamath-0.9/ziamath/styles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ''' Apply italic, bold, and other font styles by shifting the unstyled ASCII
     characters [A-Z, a-z, and 0-9] to their higher unicode alternatives. Note
     this does not check whether the new character glyph exists in the font.
 '''
 from __future__ import annotations
-from typing import Any, MutableMapping
+from typing import Optional, Any, MutableMapping
 from collections import ChainMap, namedtuple
 from dataclasses import dataclass, field, asdict
 from xml.etree import ElementTree as ET
 
 from .config import config
 
 
@@ -56,15 +56,15 @@
     if 'displaystyle' in params:
         dstyle = params.get('displaystyle') in ['true', True]
     elif 'display' in params:
         dstyle = params.get('display', 'block') != 'inline'
     return dstyle
 
 
-def parse_style(element: ET.Element, parent_style: MathStyle = None) -> MathStyle:
+def parse_style(element: ET.Element, parent_style: Optional[MathStyle] = None) -> MathStyle:
     ''' Read element style attributes into MathStyle '''
     params: MutableMapping[str, Any]
     if parent_style:
         params = ChainMap(element.attrib, asdict(parent_style))
         parent_variant = parent_style.mathvariant
     else:
         params = element.attrib
```

### Comparing `ziamath-0.8.1/ziamath/zmath.py` & `ziamath-0.9/ziamath/zmath.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,22 @@
 import re
 from collections import ChainMap
 from math import inf, cos, sin, radians
 from itertools import zip_longest
 import importlib.resources as pkg_resources
 import xml.etree.ElementTree as ET
 
-from latex2mathml.converter import convert  # type: ignore
-import latex2mathml.commands  # type: ignore
-
 import ziafont as zf
 from ziafont.glyph import fmt
 from .mathfont import MathFont
 from .nodes import Mnode
 from .styles import parse_style
 from .escapes import unescape
 from .config import config
+from .tex import tex2mml
 
 
 Halign = Literal['left', 'center', 'right']
 Valign = Literal['top', 'center', 'base', 'axis', 'bottom']
 
 
 def denamespace(element: ET.Element) -> ET.Element:
@@ -33,45 +31,14 @@
     if element.tag.startswith('{'):
         element.tag = element.tag.split('}')[1]
     for elm in element:
         denamespace(elm)
     return element
 
 
-def declareoperator(name: str) -> None:
-    r''' Declare a new operator name, similar to Latex ``\DeclareMathOperator`` command.
-
-        Args:
-            name: Name of operator, should start with a ``\``.
-                Example: ``declareoperator(r'\myfunc')``
-    '''
-    latex2mathml.commands.FUNCTIONS = latex2mathml.commands.FUNCTIONS + (name,)
-
-
-def tex2mml(tex: str, inline: bool = False) -> str:
-    ''' Convert Latex to MathML. Do some hacky preprocessing to work around
-        some issues with generated MathML that ziamath doesn't support yet.
-    '''
-    tex = re.sub(r'\\binom{(.+?)}{(.+?)}', r'\\left( \1 \\atop \2 \\right)', tex)
-    # latex2mathml bug requires space after mathrm
-    tex = re.sub(r'\\mathrm{(.+?)}', r'\\mathrm {\1}', tex)
-    tex = tex.replace('||', '‖')
-    if config.decimal_separator == ',':
-        # Replace , with {,} to remove right space
-        # (must be surrounded by digits)
-        tex = re.sub(r'([0-9]),([0-9])', r'\1{,}\2', tex)
-
-    mml = convert(tex, display='inline' if inline else 'block')
-
-    # Replace some operators with "stretchy" variants
-    mml = re.sub(r'<mo>&#x0005E;', r'<mo>&#x00302;', mml)  # widehat
-    mml = re.sub(r'<mo>&#x0007E;', r'<mo>&#x00303;', mml)  # widetilde
-    return mml
-
-
 def apply_mstyle(element: ET.Element) -> ET.Element:
     ''' Take attributes defined in <mstyle> elements and add them
         to all the child elements, removing the original <mstyle>
     '''
     def flatten_attrib(element: ET.Element) -> None:
         for child in element:
             if element.tag == 'mstyle':
@@ -91,15 +58,15 @@
 
         Args:
             mathml: MathML expression, in string or XML Element
             size: Base font size, pixels
             font: Filename of font file. Must contain MATH typesetting table.
     '''
     def __init__(self, mathml: Union[str, ET.Element],
-                 size: float = None, font: str = None):
+                 size: Optional[float] = None, font: Optional[str] = None):
         self.size = size if size else config.math.fontsize
         font = font if font else config.math.mathfont
 
         self.font: MathFont
         if font is None:
             self.font = loadedfonts['default']
         elif font in loadedfonts:
@@ -117,16 +84,16 @@
         self.mathml = mathml
         self.style = parse_style(mathml)
         self.element = mathml
         self.mtag = 'math'
         self.node = Mnode.fromelement(mathml, parent=self)  # type: ignore
 
     @classmethod
-    def fromlatex(cls, latex: str, size: float = None, mathstyle: str = None,
-                  font: str = None, color: str = None, inline: bool = False):
+    def fromlatex(cls, latex: str, size: Optional[float] = None, mathstyle: Optional[str] = None,
+                  font: Optional[str] = None, color: Optional[str] = None, inline: bool = False):
         ''' Create Math Renderer from a single LaTeX expression. Requires
             latex2mathml Python package.
 
             Args:
                 latex: Latex string
                 size: Base font size
                 mathstyle: Style parameter for math, equivalent to "mathvariant" MathML attribute
@@ -142,31 +109,31 @@
             mathml = ET.tostring(mathml, encoding='unicode')
         if color:
             mathml = ET.fromstring(mathml)
             mathml.attrib['mathcolor'] = color
         return cls(mathml, size, font)
 
     @classmethod
-    def fromlatextext(cls, latex: str, size: float = 24, mathstyle: str = None,
-                      textstyle: str = None, font: str = None,
-                      color: str = None):
+    def fromlatextext(cls, latex: str, size: float = 24, mathstyle: Optional[str] = None,
+                      textstyle: Optional[str] = None, font: Optional[str] = None,
+                      color: Optional[str] = None):
         ''' Create Math Renderer from a sentence containing zero or more LaTeX
             expressions delimited by $..$, resulting in single MathML element.
             Requires latex2mathml Python package.
 
             Args:
                 latex: string
                 size: Base font size
                 mathstyle: Style parameter for math, equivalent to "mathvariant" MathML attribute
                 textstyle: Style parameter for text, equivalent to "mathvariant" MathML attribute
                 font: Font file name
                 color: Color parameter, equivalent to "mathcolor" attribute
         '''
         warnings.warn(r'fromlatextext is deprecated. Use ziamath.Text or \text{} command.', DeprecationWarning, stacklevel=2)
-        
+
         # Extract each $..$, convert to MathML, but the raw text in <mtext>, and join
         # into a single <math>
         parts = re.split(r'(\$+.*?\$+)', latex)
         texts = parts[::2]
         maths = [tex2mml(p.replace('$', ''), inline=not p.startswith('$$')) for p in parts[1::2]]
         mathels = [ET.fromstring(m) for m in maths]   # Convert to xml, but drop opening <math>
 
@@ -246,15 +213,15 @@
 
     def _repr_svg_(self):
         ''' Jupyter SVG representation '''
         return self.svg()
 
     @classmethod
     def mathml2svg(cls, mathml: Union[str, ET.Element],
-                   size: float = None, font: str = None):
+                   size: Optional[float] = None, font: Optional[str] = None):
         ''' Shortcut to just return SVG string directly '''
         return cls(mathml, size=size, font=font).svg()
 
     def getsize(self) -> tuple[float, float]:
         ''' Get size of rendered text '''
         return (self.node.bbox.xmax - self.node.bbox.xmin,
                 self.node.bbox.ymax - self.node.bbox.ymin)
@@ -271,16 +238,16 @@
             latex: Latex string
             size: Base font size
             mathstyle: Style parameter for math, equivalent to "mathvariant" MathML attribute
             font: Font file name
             color: Color parameter, equivalent to "mathcolor" attribute
             inline: Use inline math mode (default is block mode)
         '''
-    def __init__(self, latex: str, size: float = None, mathstyle: str = None,
-                 font: str = None, color: str = None, inline: bool = False):
+    def __init__(self, latex: str, size: Optional[float] = None, mathstyle: Optional[str] = None,
+                 font: Optional[str] = None, color: Optional[str] = None, inline: bool = False):
         self.latex = latex
 
         mathml: Union[str, ET.Element]
         mathml = tex2mml(latex, inline=inline)
         if mathstyle:
             mathml = ET.fromstring(mathml)
             mathml.attrib['mathvariant'] = mathstyle
@@ -308,17 +275,17 @@
             valign: vertical alignment
             rotation: Rotation angle in degrees
             rotation_mode: Either 'default' or 'anchor', to
                 mimic Matplotlib behavoir. See:
                 https://matplotlib.org/stable/gallery/text_labels_and_annotations/demo_text_rotation_mode.html
 
     '''
-    def __init__(self, s, textfont: str = None, mathfont: str = None,
-                 mathstyle: str = None, size: float = None, linespacing: float = None,
-                 color: str = None,
+    def __init__(self, s, textfont: Optional[str] = None, mathfont: Optional[str] = None,
+                 mathstyle: Optional[str] = None, size: Optional[float] = None, linespacing: Optional[float] = None,
+                 color: Optional[str] = None,
                  halign: str = 'left', valign: str = 'base',
                  rotation: float = 0, rotation_mode: str = 'anchor'):
         self.str = s
         self.mathfont = mathfont
         self.mathstyle = mathstyle
         self.size = size if size else config.text.fontsize
         self.linespacing = linespacing if linespacing else config.text.linespacing
@@ -367,29 +334,29 @@
 
     def save(self, fname):
         ''' Save expression to SVG file '''
         with open(fname, 'w') as f:
             f.write(self.svg())
 
     def drawon(self, svg: ET.Element, x: float = 0, y: float = 0,
-               halign: str = None, valign: str = None) -> ET.Element:
+               halign: Optional[str] = None, valign: Optional[str] = None) -> ET.Element:
         ''' Draw text on existing SVG element
 
             Args:
                 svg: Element to draw on
                 x: x-position
                 y: y-position
                 halign: Horizontal alignment
                 valign: Vertical alignment
         '''
         svgelm, _ = self._drawon(svg, x, y, halign, valign)
         return svgelm
 
     def _drawon(self, svg: ET.Element, x: float = 0, y: float = 0,
-                halign: str = None, valign: str = None) -> Tuple[ET.Element, Tuple[float, float, float, float]]:
+                halign: Optional[str] = None, valign: Optional[str] = None) -> Tuple[ET.Element, Tuple[float, float, float, float]]:
         ''' Draw text on existing SVG element
 
             Args:
                 svg: Element to draw on
                 x: x-position
                 y: y-position
                 halign: Horizontal alignment
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ziamath-0.8.1/ziamath.egg-info/PKG-INFO` & `ziamath-0.9/ziamath.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: ziamath
-Version: 0.8.1
+Version: 0.9
 Summary: Render MathML and LaTeX Math to SVG in pure Python without Latex installation
 Home-page: https://ziamath.readthedocs.io
 Author: Collin J. Delker
 Author-email: code@collindelker.com
 License: MIT
 Project-URL: Documentation, https://ziamath.readthedocs.io
 Project-URL: Source Code, https://github.com/cdelker/ziamath
 Keywords: MathML,LaTeX,math,font,truetype,opentype,svg
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: ziafont>=0.7
+Requires-Dist: latex2mathml
 
 # ziamath
 
 Render MathML or LaTeX Math expressions as SVG using pure Python. Does not require a Latex installation, nor a network connection.
 
 Ziamath comes with the STIXTwoMath-Regular font installed for use by default.
 Other Math-enabled Open Type fonts (TTF or OTF files) may also be used.
```

### Comparing `ziamath-0.8.1/ziamath.egg-info/SOURCES.txt` & `ziamath-0.9/ziamath.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 ziamath/config.py
 ziamath/drawable.py
 ziamath/escape_codes.py
 ziamath/escapes.py
 ziamath/mathfont.py
 ziamath/mathtable.py
 ziamath/operators.py
-ziamath/operators_mml4.py
 ziamath/py.typed
 ziamath/styles.py
+ziamath/tex.py
 ziamath/zmath.py
 ziamath.egg-info/PKG-INFO
 ziamath.egg-info/SOURCES.txt
 ziamath.egg-info/dependency_links.txt
 ziamath.egg-info/not-zip-safe
 ziamath.egg-info/requires.txt
 ziamath.egg-info/top_level.txt
```

