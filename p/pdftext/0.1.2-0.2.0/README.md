# Comparing `tmp/pdftext-0.1.2.tar.gz` & `tmp/pdftext-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftext-0.1.2.tar", max compression
+gzip compressed data, was "pdftext-0.2.0.tar", max compression
```

## Comparing `pdftext-0.1.2.tar` & `pdftext-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11269 2024-04-26 05:34:48.558207 pdftext-0.1.2/LICENSE
--rw-r--r--   0        0        0     6486 2024-04-26 05:34:48.558207 pdftext-0.1.2/README.md
--rw-r--r--   0        0        0     1198 2024-04-26 05:34:48.558207 pdftext-0.1.2/extract_text.py
--rw-r--r--   0        0        0    18905 2024-04-26 05:34:48.562207 pdftext-0.1.2/models/dt.joblib
--rw-r--r--   0        0        0     2225 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/extraction.py
--rw-r--r--   0        0        0     5786 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/inference.py
--rw-r--r--   0        0        0      153 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/model.py
--rw-r--r--   0        0        0     3186 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/pdf/chars.py
--rw-r--r--   0        0        0     3353 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/pdf/utils.py
--rw-r--r--   0        0        0     2129 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/postprocessing.py
--rw-r--r--   0        0        0      478 2024-04-26 05:34:48.562207 pdftext-0.1.2/pdftext/settings.py
--rw-r--r--   0        0        0      856 2024-04-26 05:34:48.562207 pdftext-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7462 1970-01-01 00:00:00.000000 pdftext-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11269 2024-04-26 19:13:32.439225 pdftext-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6599 2024-04-26 19:13:32.443225 pdftext-0.2.0/README.md
+-rw-r--r--   0        0        0     1198 2024-04-26 19:13:32.443225 pdftext-0.2.0/extract_text.py
+-rw-r--r--   0        0        0    16601 2024-04-26 19:13:32.443225 pdftext-0.2.0/models/dt.joblib
+-rw-r--r--   0        0        0     1850 2024-04-26 19:13:32.443225 pdftext-0.2.0/pdftext/extraction.py
+-rw-r--r--   0        0        0     5867 2024-04-26 19:13:32.443225 pdftext-0.2.0/pdftext/inference.py
+-rw-r--r--   0        0        0      153 2024-04-26 19:13:32.443225 pdftext-0.2.0/pdftext/model.py
+-rw-r--r--   0        0        0     3721 2024-04-26 19:13:32.443225 pdftext-0.2.0/pdftext/pdf/chars.py
+-rw-r--r--   0        0        0     4859 2024-04-26 19:13:32.443225 pdftext-0.2.0/pdftext/pdf/utils.py
+-rw-r--r--   0        0        0     2129 2024-04-26 19:13:32.443225 pdftext-0.2.0/pdftext/postprocessing.py
+-rw-r--r--   0        0        0      478 2024-04-26 19:13:32.443225 pdftext-0.2.0/pdftext/settings.py
+-rw-r--r--   0        0        0      856 2024-04-26 19:13:32.443225 pdftext-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7575 1970-01-01 00:00:00.000000 pdftext-0.2.0/PKG-INFO
```

### Comparing `pdftext-0.1.2/LICENSE` & `pdftext-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftext-0.1.2/README.md` & `pdftext-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
       - `char_idx` - the index of the character on the page (from `0` to number of characters, in original pdf order)
       - `font` this is font info straight from the pdf, see [this pdfium code](https://pdfium.googlesource.com/pdfium/+/refs/heads/main/public/fpdf_text.h)
         - `size` - the size of the font used for the character
         - `weight` - font weight
         - `name` - font name, may be None
         - `flags` - font flags, in the format of the `PDF spec 1.7 Section 5.7.1 Font Descriptor Flags`
 
+If the pdf is rotated, the bboxes will be relative to the rotated page (they're rotated after being extracted).
+
 # Programmatic usage
 
 Extract plain text:
 
 ```python
 from pdftext.extraction import plain_text_output
```

### Comparing `pdftext-0.1.2/extract_text.py` & `pdftext-0.2.0/extract_text.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.1.2/pdftext/extraction.py` & `pdftext-0.2.0/pdftext/extraction.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,28 +32,18 @@
     pages = _get_pages(pdf_path, model)
     for page in pages:
         for block in page["blocks"]:
             bad_keys = [key for key in block.keys() if key not in ["lines", "bbox"]]
             for key in bad_keys:
                 del block[key]
             for line in block["lines"]:
-                line_box = None
                 bad_keys = [key for key in line.keys() if key not in ["chars", "bbox"]]
                 for key in bad_keys:
                     del line[key]
                 for char in line["chars"]:
-                    char["bbox"] = unnormalize_bbox(char["bbox"], page["bbox"])
+                    char["bbox"] = unnormalize_bbox(char["bbox"], page["width"], page["height"])
                     char["char"] = postprocess_text(char["char"])
-                    if line_box is None:
-                        line_box = char["bbox"]
-                    else:
-                        line_box = [
-                            min(line_box[0], char["bbox"][0]),
-                            min(line_box[1], char["bbox"][1]),
-                            max(line_box[2], char["bbox"][2]),
-                            max(line_box[3], char["bbox"][3]),
-                        ]
-                line["bbox"] = line_box
-            block["bbox"] = unnormalize_bbox(block["bbox"], page["bbox"])
+                line["bbox"] = unnormalize_bbox(line["bbox"], page["width"], page["height"])
+            block["bbox"] = unnormalize_bbox(block["bbox"], page["width"], page["height"])
         if sort:
             page["blocks"] = sort_blocks(page["blocks"])
     return pages
```

### Comparing `pdftext-0.1.2/pdftext/inference.py` & `pdftext-0.2.0/pdftext/inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,15 +86,22 @@
     block = {"lines": []}
     return block
 
 
 def infer_single_page(text_chars):
     prev_char = None
 
-    blocks = {"blocks": []}
+    blocks = {
+        "blocks": [],
+        "page": text_chars["page"],
+        "rotation": text_chars["rotation"],
+        "bbox": text_chars["bbox"],
+        "width": text_chars["width"],
+        "height": text_chars["height"],
+    }
     block = {"lines": []}
     line = {"spans": []}
     span = {"chars": []}
     for i, char_info in enumerate(text_chars["chars"]):
         if prev_char:
             training_row = create_training_row(char_info, prev_char, block, line)
             sorted_keys = sorted(training_row.keys())
@@ -121,17 +128,14 @@
     if len(span["chars"]) > 0:
         update_span(line, span)
     if len(line["spans"]) > 0:
         update_line(block, line)
     if len(block["lines"]) > 0:
         update_block(blocks, block)
 
-    blocks["page"] = text_chars["page"]
-    blocks["rotation"] = text_chars["rotation"]
-    blocks["bbox"] = text_chars["bbox"]
     return blocks
 
 
 def inference(text_chars, model):
     # Create generators and get first training row from each
     generators = [infer_single_page(text_page) for text_page in text_chars]
     next_prediction = {}
```

### Comparing `pdftext-0.1.2/pdftext/pdf/chars.py` & `pdftext-0.2.0/pdftext/pdf/chars.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,25 +27,40 @@
     pdf = pdfium.PdfDocument(pdf_path)
     blocks = []
 
     for page_idx in range(len(pdf)):
         page = pdf.get_page(page_idx)
         text_page = page.get_textpage()
         mediabox = page.get_mediabox()
-        bl_origin = mediabox[0] == 0 and mediabox[1] == 0
-
+        page_rotation = page.get_rotation()
         bbox = page.get_bbox()
-        page_width = math.ceil(bbox[2] - bbox[0])
+        page_width = math.ceil(abs(bbox[2] - bbox[0]))
+        page_height = math.ceil(abs(bbox[1] - bbox[3]))
+        bbox = pdfium_page_bbox_to_device_bbox(page, bbox, page_width, page_height, page_rotation)
+
+        # Recalculate page width and height with new bboxes
+        page_width = math.ceil(abs(bbox[2] - bbox[0]))
         page_height = math.ceil(abs(bbox[1] - bbox[3]))
 
+        # Flip width and height if rotated
+        if page_rotation == 90 or page_rotation == 270:
+            page_width, page_height = page_height, page_width
+
+        bl_origin = all([
+            mediabox[0] == 0,
+            mediabox[1] == 0
+        ])
+
         text_chars = {
             "chars": [],
             "page": page_idx,
-            "rotation": page.get_rotation(),
-            "bbox": pdfium_page_bbox_to_device_bbox(page, bbox, page_width, page_height)
+            "rotation": page_rotation,
+            "bbox": bbox,
+            "width": page_width,
+            "height": page_height,
         }
 
         fontname = None
         fontflags = None
         total_chars = text_page.count_chars()
         for i in range(total_chars):
             char = pdfium_c.FPDFText_GetUnicode(text_page, i)
@@ -55,16 +70,16 @@
             if fontname is None or i % fontname_sample_freq == 0:
                 prev_fontname = fontname
                 fontname, fontflags = get_fontname(text_page, i)
                 update_previous_fonts(text_chars, i, fontname, fontflags, prev_fontname, text_page, fontname_sample_freq)
 
             rotation = pdfium_c.FPDFText_GetCharAngle(text_page, i)
             rotation = rotation * 180 / math.pi # convert from radians to degrees
-            coords = text_page.get_charbox(i, loose=True)
-            device_coords = page_bbox_to_device_bbox(page, coords, page_width, page_height, bl_origin, normalize=True)
+            coords = text_page.get_charbox(i, loose=False)
+            device_coords = page_bbox_to_device_bbox(page, coords, page_width, page_height, bl_origin, page_rotation, normalize=True)
 
             char_info = {
                 "font": {
                     "size": fontsize,
                     "weight": fontweight,
                     "name": fontname,
                     "flags": fontflags
```

### Comparing `pdftext-0.1.2/pdftext/postprocessing.py` & `pdftext-0.2.0/pdftext/postprocessing.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.1.2/pyproject.toml` & `pdftext-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdftext"
-version = "0.1.2"
+version = "0.2.0"
 description = "Extract structured text from pdfs quickly"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/VikParuchuri/pdftext"
 keywords = ["pdf", "text", "extraction"]
 packages = [
```

### Comparing `pdftext-0.1.2/PKG-INFO` & `pdftext-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftext
-Version: 0.1.2
+Version: 0.2.0
 Summary: Extract structured text from pdfs quickly
 Home-page: https://github.com/VikParuchuri/pdftext
 License: Apache-2.0
 Keywords: pdf,text,extraction
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -78,14 +78,16 @@
       - `char_idx` - the index of the character on the page (from `0` to number of characters, in original pdf order)
       - `font` this is font info straight from the pdf, see [this pdfium code](https://pdfium.googlesource.com/pdfium/+/refs/heads/main/public/fpdf_text.h)
         - `size` - the size of the font used for the character
         - `weight` - font weight
         - `name` - font name, may be None
         - `flags` - font flags, in the format of the `PDF spec 1.7 Section 5.7.1 Font Descriptor Flags`
 
+If the pdf is rotated, the bboxes will be relative to the rotated page (they're rotated after being extracted).
+
 # Programmatic usage
 
 Extract plain text:
 
 ```python
 from pdftext.extraction import plain_text_output
```

