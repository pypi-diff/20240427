# Comparing `tmp/google_sheet_writer-0.0.3.tar.gz` & `tmp/google_sheet_writer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_sheet_writer-0.0.3.tar", last modified: Sat Mar 30 17:54:47 2024, max compression
+gzip compressed data, was "google_sheet_writer-0.0.4.tar", last modified: Sat Apr 27 21:57:37 2024, max compression
```

## Comparing `google_sheet_writer-0.0.3.tar` & `google_sheet_writer-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2024-03-30 17:54:47.051733 google_sheet_writer-0.0.3/
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1061 2024-03-05 21:26:13.000000 google_sheet_writer-0.0.3/LICENSE.md
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1158 2024-03-30 17:54:47.051557 google_sheet_writer-0.0.3/PKG-INFO
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      654 2024-03-05 21:26:13.000000 google_sheet_writer-0.0.3/README.md
-drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2024-03-30 17:54:47.050670 google_sheet_writer-0.0.3/google_sheet_writer/
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      360 2024-03-05 21:26:14.000000 google_sheet_writer-0.0.3/google_sheet_writer/__init__.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    21142 2024-03-30 17:26:21.000000 google_sheet_writer-0.0.3/google_sheet_writer/classes.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       22 2024-03-30 17:54:20.000000 google_sheet_writer-0.0.3/google_sheet_writer/version.py
-drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2024-03-30 17:54:47.051384 google_sheet_writer-0.0.3/google_sheet_writer.egg-info/
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1158 2024-03-30 17:54:47.000000 google_sheet_writer-0.0.3/google_sheet_writer.egg-info/PKG-INFO
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      337 2024-03-30 17:54:47.000000 google_sheet_writer-0.0.3/google_sheet_writer.egg-info/SOURCES.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)        1 2024-03-30 17:54:47.000000 google_sheet_writer-0.0.3/google_sheet_writer.egg-info/dependency_links.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       27 2024-03-30 17:54:47.000000 google_sheet_writer-0.0.3/google_sheet_writer.egg-info/requires.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       20 2024-03-30 17:54:47.000000 google_sheet_writer-0.0.3/google_sheet_writer.egg-info/top_level.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       38 2024-03-30 17:54:47.051794 google_sheet_writer-0.0.3/setup.cfg
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1043 2024-03-05 21:26:13.000000 google_sheet_writer-0.0.3/setup.py
+drwxr-xr-x   0 pecheny  (1432018558) 593637566        0 2024-04-27 21:57:37.445590 google_sheet_writer-0.0.4/
+-rw-r--r--   0 pecheny  (1432018558) 593637566     1061 2024-03-05 21:26:13.000000 google_sheet_writer-0.0.4/LICENSE.md
+-rw-r--r--   0 pecheny  (1432018558) 593637566     1158 2024-04-27 21:57:37.445415 google_sheet_writer-0.0.4/PKG-INFO
+-rw-r--r--   0 pecheny  (1432018558) 593637566      654 2024-03-05 21:26:13.000000 google_sheet_writer-0.0.4/README.md
+drwxr-xr-x   0 pecheny  (1432018558) 593637566        0 2024-04-27 21:57:37.444541 google_sheet_writer-0.0.4/google_sheet_writer/
+-rw-r--r--   0 pecheny  (1432018558) 593637566      360 2024-03-05 21:26:14.000000 google_sheet_writer-0.0.4/google_sheet_writer/__init__.py
+-rw-r--r--   0 pecheny  (1432018558) 593637566    21987 2024-04-27 18:07:51.000000 google_sheet_writer-0.0.4/google_sheet_writer/classes.py
+-rw-r--r--   0 pecheny  (1432018558) 593637566       22 2024-04-27 21:57:09.000000 google_sheet_writer-0.0.4/google_sheet_writer/version.py
+drwxr-xr-x   0 pecheny  (1432018558) 593637566        0 2024-04-27 21:57:37.445234 google_sheet_writer-0.0.4/google_sheet_writer.egg-info/
+-rw-r--r--   0 pecheny  (1432018558) 593637566     1158 2024-04-27 21:57:37.000000 google_sheet_writer-0.0.4/google_sheet_writer.egg-info/PKG-INFO
+-rw-r--r--   0 pecheny  (1432018558) 593637566      337 2024-04-27 21:57:37.000000 google_sheet_writer-0.0.4/google_sheet_writer.egg-info/SOURCES.txt
+-rw-r--r--   0 pecheny  (1432018558) 593637566        1 2024-04-27 21:57:37.000000 google_sheet_writer-0.0.4/google_sheet_writer.egg-info/dependency_links.txt
+-rw-r--r--   0 pecheny  (1432018558) 593637566       27 2024-04-27 21:57:37.000000 google_sheet_writer-0.0.4/google_sheet_writer.egg-info/requires.txt
+-rw-r--r--   0 pecheny  (1432018558) 593637566       20 2024-04-27 21:57:37.000000 google_sheet_writer-0.0.4/google_sheet_writer.egg-info/top_level.txt
+-rw-r--r--   0 pecheny  (1432018558) 593637566       38 2024-04-27 21:57:37.445641 google_sheet_writer-0.0.4/setup.cfg
+-rw-r--r--   0 pecheny  (1432018558) 593637566     1043 2024-03-05 21:26:13.000000 google_sheet_writer-0.0.4/setup.py
```

### Comparing `google_sheet_writer-0.0.3/LICENSE.md` & `google_sheet_writer-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `google_sheet_writer-0.0.3/PKG-INFO` & `google_sheet_writer-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_sheet_writer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Easy wrapper around gspread and gspread-formatting
 Home-page: https://gitlab.com/peczony/google_sheet_writer
 Author: Alexander Pecheny
 Author-email: ap@pecheny.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `google_sheet_writer-0.0.3/README.md` & `google_sheet_writer-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `google_sheet_writer-0.0.3/google_sheet_writer/classes.py` & `google_sheet_writer-0.0.4/google_sheet_writer/classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,24 @@
     DataValidationRule,
     TextFormat,
     batch_updater,
     get_conditional_format_rules,
 )
 
 WORKAROUND = "___workaround"
+CURSOR_FUNCTIONS = (
+    "add_block",
+    "hblock",
+    "hblock_n",
+    "vblock",
+    "vblock_n",
+    "shift",
+    "clone",
+    "clone_shift",
+)
 
 
 class Cf:
     LEFT = CellFormat(horizontalAlignment="LEFT")
     CENTER = CellFormat(horizontalAlignment="CENTER")
     RIGHT = CellFormat(horizontalAlignment="RIGHT")
     TOP = CellFormat(verticalAlignment="TOP")
@@ -201,30 +211,50 @@
         return Cursor(self.wks, self.x + x, self.y + y)
 
     def replace(self, x=None, y=None):
         new_x = self.x if x is None else x
         new_y = self.y if y is None else y
         return Cursor(self.wks, new_x, new_y)
 
-    def as_cell(self):
-        return rowcol_to_a1(self.y, self.x)
-
-    def as_cell_full(self):
-        return f"'{self.wks.ws.title}'!{self.as_cell()}"
+    def as_cell(self, fixed_row=False, fixed_col=False, full=False):
+        col = col_to_a(self.x)
+        row = str(self.y)
+        if fixed_row:
+            row = "$" + row
+        if fixed_col:
+            col = "$" + col
+        formatted = col + row
+        if full:
+            formatted = f"'{self.wks.ws.title}'!{formatted}"
+        return formatted
+
+    def as_cell_full(self, **kwargs):
+        kwargs["full"] = True
+        return self.as_cell(**kwargs)
 
     def __repr__(self):
         return f"Cursor({self.wks.ws.title} {self.x}, {self.y})"
 
     def __format__(self, spec):
-        if spec == "f":
-            return self.as_cell_full()
-        elif spec == "":
-            return self.as_cell()
+        spec = list(spec)
+        full = "f" in spec
+        if "p" in spec:
+            if "pr" in spec:
+                fixed_row = True
+                fixed_col = False
+            elif "pc" in spec:
+                fixed_row = False
+                fixed_col = True
+            else:
+                fixed_row = True
+                fixed_col = True
         else:
-            raise ValueError(f"Invalid format specifier {spec}")
+            fixed_row = False
+            fixed_col = False
+        return self.as_cell(full=full, fixed_col=fixed_col, fixed_row=fixed_row)
 
     def set_col_width(self, width):
         self.wks.parent.fmt[self.wks.ws.title]["column_widths"][self.x] = width
 
     def set_row_height(self, height):
         self.wks.parent.fmt[self.wks.ws.title]["row_heights"][self.y] = height
 
@@ -359,24 +389,15 @@
         self.parent = parent
         self.cursor = Cursor(self)
         self.defer = defer
         self.hidden = hidden
         self.init_format = init_format
         self.force_max_col = force_max_col
         self.force_max_row = force_max_row
-        for func in (
-            "add_block",
-            "hblock",
-            "hblock_n",
-            "vblock",
-            "vblock_n",
-            "shift",
-            "clone",
-            "clone_shift",
-        ):
+        for func in CURSOR_FUNCTIONS:
 
             def func_gen(name):
                 def _func(*args, **kwargs):
                     return getattr(self.cursor, name)(*args, **kwargs)
 
                 return _func
 
@@ -396,14 +417,20 @@
 
     def set_cell_format(self, range_, cell_format):
         self.parent.fmt[self.ws.title]["cell_ranges"].insert(0, (range_, cell_format))
 
     def add_to_batch_clear(self, rng):
         self.parent.batch_clear_ranges.append(absolute_range_name(self.ws.title, rng))
 
+    def max_col(self):
+        return max(c.col for c in self.parent.cells[self.ws.title])
+
+    def max_row(self):
+        return max(c.row for c in self.parent.cells[self.ws.title])
+
 
 def new_fmt():
     return {
         "conditional_format_rules": [],
         "cell_ranges": [],
         "merged_cells": [],
         "dv_cell_ranges": [],
@@ -518,14 +545,15 @@
             self.spreadsheet.del_worksheet(self.worksheets[name].ws)
             self.worksheets.pop(name, None)
             self.sleep()
         if name not in self.worksheets:
             print(f"Adding worksheet {name}...")
             new_ws = self.spreadsheet.add_worksheet(name, 200, 60)
             self.worksheets[name] = wrap_ws(new_ws)
+            self.sleep()
         return self.worksheets[name]
 
     def sleep(self):
         if self.throttle:
             time.sleep(self.throttle)
 
     def format(self):
@@ -614,14 +642,15 @@
             print("Applying formatting...")
             self.formatter.execute()
             self.sleep()
 
         if reqs:
             print("Hiding columns and rows...")
             self.spreadsheet.batch_update({"requests": reqs})
+            self.sleep()
 
     def submit_ws(self, name):
         if name in self.ignore:
             return
         cells = self.cells[name]
         if cells:
             print(f"Writing cells for worksheet {name}...")
@@ -656,14 +685,15 @@
                     max_col = cell.col
             cells = []
             for row in range(1, max_row + 1):
                 for col in range(1, max_col + 1):
                     cells.append(Cell(row=row, col=col, value=""))
             print(f"Setting sheet size for {name} to row={max_row}, col={max_col}...")
             self.worksheets[name].ws.update_cells(cells)
+            self.sleep()
             if name in self.submit_order:
                 continue
             elif self.worksheets[name].defer:
                 deferred.append(name)
             else:
                 normal.append(name)
         self.submit_order.extend(normal)
```

### Comparing `google_sheet_writer-0.0.3/google_sheet_writer.egg-info/PKG-INFO` & `google_sheet_writer-0.0.4/google_sheet_writer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_sheet_writer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Easy wrapper around gspread and gspread-formatting
 Home-page: https://gitlab.com/peczony/google_sheet_writer
 Author: Alexander Pecheny
 Author-email: ap@pecheny.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `google_sheet_writer-0.0.3/setup.py` & `google_sheet_writer-0.0.4/setup.py`

 * *Files identical despite different names*

