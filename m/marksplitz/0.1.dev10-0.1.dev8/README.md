# Comparing `tmp/marksplitz-0.1.dev10.tar.gz` & `tmp/marksplitz-0.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marksplitz-0.1.dev10.tar", last modified: Sat Apr 27 14:52:47 2024, max compression
+gzip compressed data, was "marksplitz-0.1.dev8.tar", last modified: Sun Apr 14 15:38:55 2024, max compression
```

## Comparing `marksplitz-0.1.dev10.tar` & `marksplitz-0.1.dev8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-27 14:52:47.016859 marksplitz-0.1.dev10/
--rw-rw-r--   0 bill      (1000) bill      (1000)     1079 2024-02-17 16:02:31.000000 marksplitz-0.1.dev10/LICENSE.txt
--rw-r--r--   0 bill      (1000) bill      (1000)     4625 2024-04-27 14:52:47.016859 marksplitz-0.1.dev10/PKG-INFO
--rw-rw-r--   0 bill      (1000) bill      (1000)     3116 2024-04-26 15:13:11.000000 marksplitz-0.1.dev10/README.md
--rw-rw-r--   0 bill      (1000) bill      (1000)     1576 2024-04-13 15:30:00.000000 marksplitz-0.1.dev10/pyproject.toml
--rw-rw-r--   0 bill      (1000) bill      (1000)       38 2024-04-27 14:52:47.016859 marksplitz-0.1.dev10/setup.cfg
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-27 14:52:47.012859 marksplitz-0.1.dev10/src/
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-27 14:52:47.016859 marksplitz-0.1.dev10/src/marksplitz/
--rw-rw-r--   0 bill      (1000) bill      (1000)        0 2024-04-02 18:07:46.000000 marksplitz-0.1.dev10/src/marksplitz/__init__.py
--rw-rw-r--   0 bill      (1000) bill      (1000)    18598 2024-04-26 22:56:11.000000 marksplitz-0.1.dev10/src/marksplitz/marksplitz.py
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-27 14:52:47.016859 marksplitz-0.1.dev10/src/marksplitz.egg-info/
--rw-r--r--   0 bill      (1000) bill      (1000)     4625 2024-04-27 14:52:47.000000 marksplitz-0.1.dev10/src/marksplitz.egg-info/PKG-INFO
--rw-rw-r--   0 bill      (1000) bill      (1000)      347 2024-04-27 14:52:47.000000 marksplitz-0.1.dev10/src/marksplitz.egg-info/SOURCES.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        1 2024-04-27 14:52:47.000000 marksplitz-0.1.dev10/src/marksplitz.egg-info/dependency_links.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       58 2024-04-27 14:52:47.000000 marksplitz-0.1.dev10/src/marksplitz.egg-info/entry_points.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        8 2024-04-27 14:52:47.000000 marksplitz-0.1.dev10/src/marksplitz.egg-info/requires.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       11 2024-04-27 14:52:47.000000 marksplitz-0.1.dev10/src/marksplitz.egg-info/top_level.txt
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-27 14:52:47.016859 marksplitz-0.1.dev10/tests/
--rw-rw-r--   0 bill      (1000) bill      (1000)    11535 2024-04-16 19:16:56.000000 marksplitz-0.1.dev10/tests/test_marksplitz.py
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-14 15:38:55.390491 marksplitz-0.1.dev8/
+-rw-rw-r--   0 bill      (1000) bill      (1000)     1079 2024-02-17 16:02:31.000000 marksplitz-0.1.dev8/LICENSE.txt
+-rw-r--r--   0 bill      (1000) bill      (1000)     3887 2024-04-14 15:38:55.390491 marksplitz-0.1.dev8/PKG-INFO
+-rw-rw-r--   0 bill      (1000) bill      (1000)     2379 2024-04-14 14:57:01.000000 marksplitz-0.1.dev8/README.md
+-rw-rw-r--   0 bill      (1000) bill      (1000)     1576 2024-04-13 15:30:00.000000 marksplitz-0.1.dev8/pyproject.toml
+-rw-rw-r--   0 bill      (1000) bill      (1000)       38 2024-04-14 15:38:55.390491 marksplitz-0.1.dev8/setup.cfg
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-14 15:38:55.386491 marksplitz-0.1.dev8/src/
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-14 15:38:55.386491 marksplitz-0.1.dev8/src/marksplitz/
+-rw-rw-r--   0 bill      (1000) bill      (1000)        0 2024-04-02 18:07:46.000000 marksplitz-0.1.dev8/src/marksplitz/__init__.py
+-rw-rw-r--   0 bill      (1000) bill      (1000)    17592 2024-04-14 15:29:33.000000 marksplitz-0.1.dev8/src/marksplitz/marksplitz.py
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-14 15:38:55.390491 marksplitz-0.1.dev8/src/marksplitz.egg-info/
+-rw-r--r--   0 bill      (1000) bill      (1000)     3887 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/PKG-INFO
+-rw-rw-r--   0 bill      (1000) bill      (1000)      347 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/SOURCES.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)        1 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/dependency_links.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)       58 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/entry_points.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)        8 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/requires.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)       11 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/top_level.txt
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-14 15:38:55.390491 marksplitz-0.1.dev8/tests/
+-rw-rw-r--   0 bill      (1000) bill      (1000)     9974 2024-04-13 15:34:02.000000 marksplitz-0.1.dev8/tests/test_marksplitz.py
```

### Comparing `marksplitz-0.1.dev10/LICENSE.txt` & `marksplitz-0.1.dev8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `marksplitz-0.1.dev10/PKG-INFO` & `marksplitz-0.1.dev8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marksplitz
-Version: 0.1.dev10
+Version: 0.1.dev8
 Summary: Command-line utility to split a Markdown file into linked static web pages.
 Author-email: Bill Melvin <bill@billmelvin.com>
 License: MIT License
         
         Copyright (c) 2024-present William Melvin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -21,32 +21,14 @@
 
 # marksplitz
 
 Command-line utility to split a Markdown file into linked static web pages.
 
 > Development work in progress.
 
-## Directive Comments
-
-The following HTML comments can be placed in the source Markdown document to alter the generated HTML.
-
-`<!-- title: new-title -->` 
-
-- Replace the default HTML **title** for the page.
-
-`<!-- class: class-1 class-2 -->` 
-
-- Add one or more classes to the `content` div.
-- Use to apply styles to multiple pages via a `custom.css` file. 
-
-`<!-- id: id-value -->` 
-
-- Add `id="id-value"` to the `content` div.
-- Use to apply styles to a specific page via a `custom.css` file. 
-
 ## Command-line Usage
 
 ```
 usage: marksplitz [-h] [-o OUTPUT_DIR] [-n OUTPUT_NAME] [-i IMAGES_SUBDIR]
                      [-c CSS_FILE]
                      markdown_file
 
@@ -75,16 +57,14 @@
                         exist, it is created with the default style.
 ```
 
 ## Reference
 
 ### CSS
 
-Customizing the generated HTML output requires using CSS.
-
 - MDN Guide: [Learn to style HTML using CSS](https://developer.mozilMDNla.org/en-US/docs/Learn/CSS)
 - MDN Reference: [CSS: Cascading Style Sheets](https://developer.mozilla.org/en-US/docs/Web/CSS)
   - [Basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout/Basic_concepts_of_flexbox)
   - [Class selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/Class_selectors)
 
 ### Packages Used
 
@@ -92,10 +72,8 @@
     - [docs](https://mistune.lepture.com/en/latest/)
 
 ### Project Tools
 
 - [uv](https://github.com/astral-sh/uv#readme) - Environment management (in place of `pip`)
 - [Ruff](https://docs.astral.sh/ruff/) - Linter and code formatter
 - [pytest](https://docs.pytest.org/en/stable/) - Testing framework
-- [build](https://build.pypa.io/en/stable/index.html) - Python packaging build frontend
-- [twine](https://twine.readthedocs.io/en/latest/) - Utility for publishing Python packages
 - [Just](https://github.com/casey/just#readme) - Command runner
```

### Comparing `marksplitz-0.1.dev10/README.md` & `marksplitz-0.1.dev8/src/marksplitz.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+Metadata-Version: 2.1
+Name: marksplitz
+Version: 0.1.dev8
+Summary: Command-line utility to split a Markdown file into linked static web pages.
+Author-email: Bill Melvin <bill@billmelvin.com>
+License: MIT License
+        
+        Copyright (c) 2024-present William Melvin
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+Keywords: markdown,converter,html,slideshow
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: mistune
+
 # marksplitz
 
 Command-line utility to split a Markdown file into linked static web pages.
 
 > Development work in progress.
 
-## Directive Comments
-
-The following HTML comments can be placed in the source Markdown document to alter the generated HTML.
-
-`<!-- title: new-title -->` 
-
-- Replace the default HTML **title** for the page.
-
-`<!-- class: class-1 class-2 -->` 
-
-- Add one or more classes to the `content` div.
-- Use to apply styles to multiple pages via a `custom.css` file. 
-
-`<!-- id: id-value -->` 
-
-- Add `id="id-value"` to the `content` div.
-- Use to apply styles to a specific page via a `custom.css` file. 
-
 ## Command-line Usage
 
 ```
 usage: marksplitz [-h] [-o OUTPUT_DIR] [-n OUTPUT_NAME] [-i IMAGES_SUBDIR]
                      [-c CSS_FILE]
                      markdown_file
 
@@ -54,16 +57,14 @@
                         exist, it is created with the default style.
 ```
 
 ## Reference
 
 ### CSS
 
-Customizing the generated HTML output requires using CSS.
-
 - MDN Guide: [Learn to style HTML using CSS](https://developer.mozilMDNla.org/en-US/docs/Learn/CSS)
 - MDN Reference: [CSS: Cascading Style Sheets](https://developer.mozilla.org/en-US/docs/Web/CSS)
   - [Basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout/Basic_concepts_of_flexbox)
   - [Class selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/Class_selectors)
 
 ### Packages Used
 
@@ -71,10 +72,8 @@
     - [docs](https://mistune.lepture.com/en/latest/)
 
 ### Project Tools
 
 - [uv](https://github.com/astral-sh/uv#readme) - Environment management (in place of `pip`)
 - [Ruff](https://docs.astral.sh/ruff/) - Linter and code formatter
 - [pytest](https://docs.pytest.org/en/stable/) - Testing framework
-- [build](https://build.pypa.io/en/stable/index.html) - Python packaging build frontend
-- [twine](https://twine.readthedocs.io/en/latest/) - Utility for publishing Python packages
 - [Just](https://github.com/casey/just#readme) - Command runner
```

### Comparing `marksplitz-0.1.dev10/pyproject.toml` & `marksplitz-0.1.dev8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `marksplitz-0.1.dev10/src/marksplitz/marksplitz.py` & `marksplitz-0.1.dev8/src/marksplitz/marksplitz.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime
 from pathlib import Path
 from textwrap import dedent, indent
 from typing import NamedTuple
 
 import mistune
 
-__version__ = "0.1.dev10"
+__version__ = "0.1.dev8"
 
 
 run_dt = datetime.now()
 
 
 class AppOptions(NamedTuple):
     md_path: Path
@@ -64,17 +64,16 @@
             display: flex;
             align-items: center;
             justify-content: center;
             min-height: 600px;
         }
         .content {
             border: 1px solid silver;
-            padding: 2rem 10%;
-            width: 900px;
-            max-width: 90%;
+            padding: 2rem;
+            width: 800px;
         }
         .text-center { text-align: center; }
         .nav-link {
             padding-top: 2rem;
             width: 3rem;
         }
         .nav-link a {
@@ -170,31 +169,25 @@
     """
     if prev_page:
         case_prev = dedent(
             f"""\
             case "ArrowLeft":
                 window.location.href = "{prev_page}";
                 break;
-            case "PageUp":
-                window.location.href = "{prev_page}";
-                break;
             """
         )
     else:
         case_prev = ""
 
     if next_page:
         case_next = dedent(
             f"""\
             case "ArrowRight":
                 window.location.href = "{next_page}";
                 break;
-            case "PageDown":
-                window.location.href = "{next_page}";
-                break;
             """
         )
     else:
         case_next = ""
 
     s = dedent(
         """\
@@ -271,16 +264,16 @@
     return s
 
 
 def write_index(out_path: Path, items: list[tuple[str, str]]) -> None:
     """Write an index file with links to the pages.
 
     The file is named 'index.html' and is written to the output directory.
-    The parameter 'items' is a list of tuples containing the filename,
-    title, and heading level of each page.
+    The parameter 'items' is a list of tuples containing the filename and
+    title of each page.
     """
     index_file = out_path / "index.html"
     print(f"Writing '{index_file}'")
     with index_file.open("w") as f:
         f.write(
             dedent(
                 """\
@@ -297,31 +290,27 @@
                         padding: 0.3rem;
                     }
                     .container { display: flex; justify-content: center; }
                     .content { max-width: 900px; }
                     a:link, a:visited { color: navy; text-decoration: none; }
                     a:hover { text-decoration: underline; }
                   </style>
-                  <link rel="stylesheet" type="text/css" href="custom.css">
                   <base target="_blank">
                 </head>
                 <body>
                 <div class="container">
                 <div class="content">
                 <h1>Index of Pages</h1>
                 <ol>
                 """
             )
         )
 
-        for filename, title, level in items:
-            f.write(
-                f'  <li class="index-lev-{level}"><a href="{filename}">{title}</a>'
-                "</li>\n"
-            )
+        for filename, title in items:
+            f.write(f'  <li><a href="{filename}">{title}</a></li>\n')
 
         f.write(
             dedent(
                 """\
                 </ol>
                 </div>
                 </div>
@@ -452,68 +441,55 @@
             if not src_file.is_file():
                 continue
             dst_file = dst_path / src_file.name
             print(f"Copy '{src_file}'\n  to '{dst_file}'")
             shutil.copy2(src_file, dst_file)
 
 
-def get_page_heading(num: int, text: str) -> tuple[str, int]:
-    """Return the first heading in the text and its heading-level.
+def get_page_title(num: int, text: str) -> str:
+    """Return the first heading in the text as the page title.
 
-    If there is no heading, return a default heading level and title.
+    If there is no heading, return a default title.
     """
-    heading_level = 1
     lines = text.splitlines()
     for line in lines:
         s = line.strip()
         if s.startswith("#"):
-            a = s.split(" ", 1)
-            heading_level = a[0].count("#")
-            return (a[1].strip(), heading_level)
-    return (f"Page {num}", heading_level)
+            return s.split(" ", 1)[1]
+    return f"Page {num}"
 
 
-def extract_title_comments(num: int, text: str) -> tuple[str, str, int]:
+def extract_title_comments(num: int, text: str) -> tuple[str, str]:
     """Extract the title from a comment in the text.
 
     Returns a tuple of the text, with title-comments removed, and the title
     extracted from the comments.
 
     There should only be one title comment in the text. If there is more than
     one, the last one is used.
 
-    If there is no title comment, the first Markdown heading in the text is used
-    as the title.
-
-    The headling level is based on the first Markdown heading in the text.
-
-    Returns a tuple of the text, the title, and the heading level.
+    The text and title are returned as strings.
     """
     title = ""
 
-    # TODO: Should a title-comment also be able to set heading-level?
-    # If so, leading '#' characters could be used same as in Markdown.
-
     # Look for, and remove, a title comment.
     out_lines = []
     lines = text.splitlines(keepends=True)
     for line in lines:
         s = line.strip()
         if s.startswith("<!-- title: "):
             title = s[12:-3].strip()
         else:
             out_lines.append(line)
 
-    heading, heading_level = get_page_heading(num, text)
-
     # If there was no title comment, use the first heading as the title.
     if not title:
-        title = heading
+        title = get_page_title(num, text)
 
-    return "".join(out_lines), title, heading_level
+    return "".join(out_lines), title
 
 
 def extract_class_comments(text: str) -> tuple[str, str]:
     """Extract classes from comments in the text.
 
     Returns a tuple of the text, with class-comments removed, and the
     classes extracted from the comments. If there are multiple classes
@@ -592,25 +568,25 @@
             )
         else:
             css_link = ""
 
         index_items = []
 
         for num, text in enumerate(pages, start=1):
-            md, pg_title, heading_level = extract_title_comments(num, text)
+            md, pg_title = extract_title_comments(num, text)
 
             md, add_classes = extract_class_comments(md)
 
             md, add_id = extract_id_comments(md)
 
             filename, prev_page, next_page = output_filenames(
                 opts.output_name, num, len(pages)
             )
 
-            index_items.append((filename, pg_title, heading_level))
+            index_items.append((filename, pg_title))
 
             html = html_head(
                 f"{num}. {pg_title}", num, prev_page, css_link, add_classes, add_id
             )
 
             html += mistune.html(md)
```

### Comparing `marksplitz-0.1.dev10/tests/test_marksplitz.py` & `marksplitz-0.1.dev8/tests/test_marksplitz.py`

 * *Files 15% similar despite different names*

```diff
@@ -354,78 +354,7 @@
     assert 'div id="page-002" class="container' in text2
 
     assert (out_dir / "page-003.html").exists()
     text3 = (out_dir / "page-003.html").read_text()
     assert 'div id="my-id" class="content' in text3
     assert "<!-- id:" not in text3
     assert 'div id="page-003" class="container' in text3
-
-
-def test_index_item_levels(tmp_path):
-    md_file = tmp_path / "test.md"
-    md_file.write_text(
-        dedent(
-            """
-            # Test
-
-            ## Section 1
-
-            Section 1 content.
-
-            ---
-
-            ## Section 2
-
-            Section 2 content.
-
-            ---
-
-            ### Section 2.1
-
-            Section 2.1 content.
-
-            ---
-
-            #### Section 2.1.1
-
-            Section 2.1.1 content.
-
-            ---
-
-            ### Section 2.2
-
-            Section 2.2 content.
-
-            ---
-
-            ## Section 3
-
-            Section 3 content.
-
-            """
-        )
-    )
-
-    out_dir = md_file.parent / "Output"
-    out_dir.mkdir()
-
-    args = [str(md_file), "-o", str(out_dir)]
-    marksplitz.main(args)
-
-    index_file = out_dir / "index.html"
-    assert index_file.exists()
-
-    index_text = index_file.read_text()
-    assert '<link rel="stylesheet" type="text/css" href="custom.css">' in index_text
-    assert '<li class="index-lev-1"><a href="page-001.html">Test</a>' in index_text
-    assert '<li class="index-lev-2"><a href="page-002.html">Section 2</a>' in index_text
-    assert (
-        '<li class="index-lev-3"><a href="page-003.html">Section 2.1</a>' in index_text
-    )
-    assert (
-        '<li class="index-lev-4"><a href="page-004.html">Section 2.1.1</a>'
-        in index_text
-    )
-    assert (
-        '<li class="index-lev-3"><a href="page-005.html">Section 2.2</a>' in index_text
-    )
-    assert '<li class="index-lev-2"><a href="page-006.html">Section 3</a>' in index_text
```

