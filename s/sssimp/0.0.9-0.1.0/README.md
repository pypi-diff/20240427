# Comparing `tmp/sssimp-0.0.9.tar.gz` & `tmp/sssimp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sssimp-0.0.9.tar", last modified: Tue Nov  9 00:45:24 2021, max compression
+gzip compressed data, was "sssimp-0.1.0.tar", last modified: Sat Apr 27 06:07:27 2024, max compression
```

## Comparing `sssimp-0.0.9.tar` & `sssimp-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,67 @@
-drwxr-xr-x   0 tina      (1000) tina      (1000)        0 2021-11-09 00:45:24.419856 sssimp-0.0.9/
--rw-r--r--   0 tina      (1000) tina      (1000)     1061 2021-10-29 00:35:39.000000 sssimp-0.0.9/LICENSE
--rw-r--r--   0 tina      (1000) tina      (1000)       27 2021-11-05 17:39:38.000000 sssimp-0.0.9/MANIFEST.in
--rw-r--r--   0 tina      (1000) tina      (1000)     6064 2021-11-09 00:45:24.419856 sssimp-0.0.9/PKG-INFO
--rw-r--r--   0 tina      (1000) tina      (1000)     5784 2021-11-05 18:02:38.000000 sssimp-0.0.9/README.md
--rw-r--r--   0 tina      (1000) tina      (1000)        0 2021-11-05 17:39:38.000000 sssimp-0.0.9/pyproject.toml
--rw-r--r--   0 tina      (1000) tina      (1000)      463 2021-11-09 00:45:24.419856 sssimp-0.0.9/setup.cfg
-drwxr-xr-x   0 tina      (1000) tina      (1000)        0 2021-11-09 00:45:24.416856 sssimp-0.0.9/src/
-drwxr-xr-x   0 tina      (1000) tina      (1000)        0 2021-11-09 00:45:24.417857 sssimp-0.0.9/src/sssimp/
--rw-r--r--   0 tina      (1000) tina      (1000)      703 2021-11-09 00:45:07.000000 sssimp-0.0.9/src/sssimp/__init__.py
--rw-r--r--   0 tina      (1000) tina      (1000)     2205 2021-11-09 00:44:54.000000 sssimp-0.0.9/src/sssimp/__main__.py
--rw-r--r--   0 tina      (1000) tina      (1000)      543 2021-11-05 17:39:38.000000 sssimp-0.0.9/src/sssimp/config.py
--rw-r--r--   0 tina      (1000) tina      (1000)      401 2021-11-05 18:02:38.000000 sssimp-0.0.9/src/sssimp/filters.py
-drwxr-xr-x   0 tina      (1000) tina      (1000)        0 2021-11-09 00:45:24.418856 sssimp-0.0.9/src/sssimp/generators/
--rw-r--r--   0 tina      (1000) tina      (1000)      922 2021-11-05 18:04:34.000000 sssimp-0.0.9/src/sssimp/generators/css.py
--rw-r--r--   0 tina      (1000) tina      (1000)     1641 2021-11-05 18:02:38.000000 sssimp-0.0.9/src/sssimp/generators/html.py
--rw-r--r--   0 tina      (1000) tina      (1000)     3208 2021-11-05 18:02:38.000000 sssimp-0.0.9/src/sssimp/generators/markdown.py
--rw-r--r--   0 tina      (1000) tina      (1000)      514 2021-11-05 18:02:38.000000 sssimp-0.0.9/src/sssimp/utils.py
-drwxr-xr-x   0 tina      (1000) tina      (1000)        0 2021-11-09 00:45:24.418856 sssimp-0.0.9/src/sssimp.egg-info/
--rw-r--r--   0 tina      (1000) tina      (1000)     6064 2021-11-09 00:45:24.000000 sssimp-0.0.9/src/sssimp.egg-info/PKG-INFO
--rw-r--r--   0 tina      (1000) tina      (1000)      425 2021-11-09 00:45:24.000000 sssimp-0.0.9/src/sssimp.egg-info/SOURCES.txt
--rw-r--r--   0 tina      (1000) tina      (1000)        1 2021-11-09 00:45:24.000000 sssimp-0.0.9/src/sssimp.egg-info/dependency_links.txt
--rw-r--r--   0 tina      (1000) tina      (1000)       16 2021-11-09 00:45:24.000000 sssimp-0.0.9/src/sssimp.egg-info/requires.txt
--rw-r--r--   0 tina      (1000) tina      (1000)        7 2021-11-09 00:45:24.000000 sssimp-0.0.9/src/sssimp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.647998 sssimp-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 06:07:22.000000 sssimp-0.1.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-27 06:07:22.000000 sssimp-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-27 06:07:22.000000 sssimp-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-27 06:07:22.000000 sssimp-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-27 06:07:22.000000 sssimp-0.1.0/DEVELOPER_README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-27 06:07:22.000000 sssimp-0.1.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-27 06:07:22.000000 sssimp-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 06:07:22.000000 sssimp-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-27 06:07:27.647998 sssimp-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-27 06:07:22.000000 sssimp-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/01-basic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/01-basic/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/01-basic/input/content/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/01-basic/input/content/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/01-basic/input/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/01-basic/input/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/01-basic/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/01-basic/output/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/content/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/content/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/content/post/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/content/post/first.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/templates/post.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/output/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/output/post/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/output/post/first.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/03-emojis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/03-emojis/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/03-emojis/input/content/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/03-emojis/input/content/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/03-emojis/input/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/03-emojis/input/templates/content.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/03-emojis/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/03-emojis/output/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-27 06:07:22.000000 sssimp-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 06:07:27.647998 sssimp-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/src/sssimp/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.647998 sssimp-0.1.0/src/sssimp/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/generators/css.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/generators/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/generators/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/generators/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.647998 sssimp-0.1.0/src/sssimp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.647998 sssimp-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-27 06:07:22.000000 sssimp-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-27 06:07:22.000000 sssimp-0.1.0/tests/test_examples.py
```

### Comparing `sssimp-0.0.9/LICENSE` & `sssimp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sssimp-0.0.9/PKG-INFO` & `sssimp-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,195 +1,224 @@
-Metadata-Version: 2.1
-Name: sssimp
-Version: 0.0.9
-Summary: A simple static website generator
-Home-page: https://github.com/Tina-otoge/sssimp
-Author: Tina
-Author-email: me@tina.moe
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sssimp 🐍
-Simple Static SIte Maker in Python
+
+The **S**tatic **S**ite **S**olution **I**n **M**odern **P**ython
+
+It's simp with 3 s!
 
 A simple tool to generate a static website while being able to use powerful HTML
 templates (Jinja2), Markdown files converted to HTML, and other preprocessors.
 
-
 ## Why?
 
 I wanted a simple way to generate static websites and I like Jinja2. I had
 previous experiences working with Jekyll but it seemed like too much work to
 setup everytime and overkill for the job as it supports many features I don't
 necessarily use.
 
+One of the main goals with sssimp is being able to generate a usable website
+without any configuration file or dependency. You only install the sssimp
+package and run it.
+
 ## Installing
 
+Requirement: Python 3.8 or later
+
 ```
-pip install sssimp
+pip install --user sssimp
 ```
 
 ## How to use
 
 Create a folder called `input`, it will hold the data to generate the site.
 
-Running `python -m sssimp` will generate content in the `output` folder.
+Running `sssimp` will generate content in the `output` folder.
 
-Here is an example script for UNIX that will regenerate the site everytime a
-file changes, useful during development:
-```bash
-trap "echo Exited!; exit 1;" SIGINT SIGTERM
+Input and output destination can be changed:
 
-while true; do
-	python -m venv .venv
-	source .venv/bin/activate
-	pip install --upgrade sssimp
-	python -m sssimp
-
-	echo Waiting for change
-	watch -g ls -lR .
-done
+```bash
+sssimp --input ../some-other/input-dir ~/some-other/output-dir
 ```
 
+Use `python -m sssimp --help` for more details.
+
 ## Generators
 
 - Files placed in `input/content` will be directly copied to the `output` folder
 
-  Example:  
+  Example:
   `input/content/favicon.png` -> `output/favicon.png`
 
 - HTML files with the suffix .html placed in `input/content` will be parsed as
-  Jinja2 templates, they can use templates defined in `input/templates`.  
+  Jinja2 templates, they can use templates defined in `input/templates`.
   See the [Jinja2 documentation](https://jinja.palletsprojects.com/en/3.0.x/templates/)
 
-  Example:  
-  `input/content/index.html` -> `output/index.html`  
-  Starting with content  
+  Example:
+  `input/content/index.html` -> `output/index.html`
+  Starting with content
+
   ```jinja2
   {% extends "base.html" %}
 
   ...
   ```
+
   Will use the template `input/templates/base.html`
 
 - CSS files in `input/css` will be merged together in a single file
   `output/bundle.css`
 
 - Markdown files with the suffix .md placed in `input/content` will be parsed to
   HTML and passed to a template with the same name as their parent folder as the
   parameter `markdown`
 
-  Example:  
-  `./input/content/post/hello-world.md` -> `./output/post/hello-world.html`  
-  Using the template `./input/templates/post.html`  
+  Example:
+  `./input/content/post/hello-world.md` -> `./output/post/hello-world.html`
+  Using the template `./input/templates/post.html`
   Generated with context `{'markdown': 'the markdown file converted to HTML'}`
 
   The template name can be overriden using the markdown meta argument "template"
 
-  Example:  
-  `./input/content/post/special.md` -> `./output/post/special.html`  
-  Starting with content  
+  Example:
+  `./input/content/post/special.md` -> `./output/post/special.html`
+  Starting with content
+
   ```md
   ---
   template: special.html
   ---
 
   ...
   ```
+
   Will use the template `./input/templates/special.html` instead of `post.html`
-  
-  ## Examples
-  
-  See [the `example` branch for an example input folder](https://github.com/Tina-otoge/sssimp/tree/example)
 
+- Files placed in `input/data` will exposes their content in templates inside
+  the `data` variable. They can be in either YAML or JSON. The path is part of
+  their position in the data structure tree.
+
+  Example:
+  `./input/data/categories/tech.yml`
+  With content
+
+  ```yaml
+  description: Nerdy stuff
+  color: #121212
+  related:
+    - computers
+    - dev
+  ```
+
+  Will populate the `data` variable in templates as so:
+
+  ```json
+  {
+    "categories": [
+      {
+        "tech": {
+          "description": "Nerdy stuff",
+          "color": "#121212",
+          "related": ["computers", "dev"]
+        }
+      }
+    ]
+  }
+  ```
+
+## Examples
+
+  See [the `example` branch for an example input folder](https://github.com/Tina-otoge/sssimp/tree/example)
+  or my personal website https://github.com/Tina-otoge/tina-simp for a real-world example.
 
 ## Additional Jinja2 filters
 
 - `|a` makes any relative path point to the top of the output folder.
 
-  Example:  
+  Example:
   `input/content/blog/post/tech/2021/11/some-post.html`
-  -> `output/blog/post/tech/2021/11/some-post.html`  
+  -> `output/blog/post/tech/2021/11/some-post.html`
   With content
+
   ```html
   <link rel="stylesheet" href="{{ "style.css"|a }}">
   ```
+
   Will be rendered as `"../../../../style.css"`
 
   See also [the `<base>` element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/base)
 
 ## Additional Jinja2 variables
 
 - `page` is a `sssimp.generators.html.Page`, it contains many information about
 the current document. Markdown files are an instance of
 `sssimp.generators.markdown.MarkdownPage` instead, which inherits from `Page`
 
   This variable itself contains many useful variables:
-  - `page.last_modified` and `page.created_at` (may be the same on Linux)
+  - `page.modified_at` and `page.created_at` (`modified_at` forcibly set to `None` if same as `created_at`)
   - `page.href`: The path to the file relative to the output folder
   - `page.src`: A `pathlib.Path` object of the source file in the input folder
   - `page.target` A `pathlib.Path` object of the target file in the output
 folder
   - `page.name`: Shortcut for `page.target.name`, the filename of the outputed
     file
   - `page.parent`: Shortcut for `page.target.parent`, the name of the parent
 directory in the output folder
 file
   - `page.meta`: The Markdown meta variables, prefixing a var with `=` will
     interpret it as raw JSON
     Example
+
     ```markdown
     ---
     some_var: some value
     something_else: 42
     some_tags:= ["tag1", "tag2"]
     ---
 
     My cool blog post
     ...
     ```
+
     The meta variable will always contain a `template` which will resolve to the
     parent directory name with .html appended if none is set in the meta fields.
 
     The `page.meta` variable is `None` for raw HTML pages, this avoids KeyErrors
     when trying to filter pages by a specific meta variable.
 - `plain_text`[^md]: A plain text representation of the Markdown file
 - `markdown`[^md]: The Markdown content converted to HTML
 - `meta`[^md]: A shortcut for `page.meta`
 - `title`[^md]: Returns `page.meta.title` if it exists, else the filename with
   the characters `-` and `_` replaced by whitespaces, the suffix removed and the
   first letter capitalized.
 
-  Example:  
+  Example:
   `input/content/some-cool-page.md`'s title is "Some cool page"
 - `BUNDLE_FILE` always evaluates to `"bundle.css"` for now
 - `BUNDLE_TIME` modification time of the latest updated file in `input/css`,
   very useful to make the browser refresh the file only if any of the CSS files
   changed.
 
   Example:
+
   ```html
   <link rel="stylesheet" href="{{ BUNDLE_FILE}}?{{ BUNDLE_TIME }}">
   ```
+
 - `PAGES` a list of `sssimp.generators.html.Page` objects containing every HTML
   and Markdown files sourced by the site. You can loop over it to generate an
   index. In conjunction with looking up meta values it can be used to filter by
   content type.
 
   Example:
+
   ```html+jinja
   {% for page in PAGES if page.meta.template == 'post.html' %}
   <a href="{{ page.href }}">{{ page.title }}</a>
   <div class="tags">
     {% for tag in page.meta.tags %}
     <span class="tag">{{ tag }}</span>
     {% endfor %}
   </div>
   Posted on <time>{{ page.created_at }}</time>
   {% endfor %}
   ```
 
 [^md]: Markdown only
-
-
```

### Comparing `sssimp-0.0.9/README.md` & `sssimp-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,175 +1,229 @@
+Metadata-Version: 2.1
+Name: sssimp
+Version: 0.1.0
+Summary: The Static Site Solution In Modern Python
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: jinja2
+Requires-Dist: markdown
+Requires-Dist: pymdown-extensions
+Requires-Dist: pyyaml
+
 # sssimp 🐍
-Simple Static SIte Maker in Python
+
+The **S**tatic **S**ite **S**olution **I**n **M**odern **P**ython
+
+It's simp with 3 s!
 
 A simple tool to generate a static website while being able to use powerful HTML
 templates (Jinja2), Markdown files converted to HTML, and other preprocessors.
 
-
 ## Why?
 
 I wanted a simple way to generate static websites and I like Jinja2. I had
 previous experiences working with Jekyll but it seemed like too much work to
 setup everytime and overkill for the job as it supports many features I don't
 necessarily use.
 
+One of the main goals with sssimp is being able to generate a usable website
+without any configuration file or dependency. You only install the sssimp
+package and run it.
+
 ## Installing
 
+Requirement: Python 3.8 or later
+
 ```
-pip install sssimp
+pip install --user sssimp
 ```
 
 ## How to use
 
 Create a folder called `input`, it will hold the data to generate the site.
 
-Running `python -m sssimp` will generate content in the `output` folder.
+Running `sssimp` will generate content in the `output` folder.
 
-Here is an example script for UNIX that will regenerate the site everytime a
-file changes, useful during development:
-```bash
-trap "echo Exited!; exit 1;" SIGINT SIGTERM
+Input and output destination can be changed:
 
-while true; do
-	python -m venv .venv
-	source .venv/bin/activate
-	pip install --upgrade sssimp
-	python -m sssimp
-
-	echo Waiting for change
-	watch -g ls -lR .
-done
+```bash
+sssimp --input ../some-other/input-dir ~/some-other/output-dir
 ```
 
+Use `python -m sssimp --help` for more details.
+
 ## Generators
 
 - Files placed in `input/content` will be directly copied to the `output` folder
 
-  Example:  
+  Example:
   `input/content/favicon.png` -> `output/favicon.png`
 
 - HTML files with the suffix .html placed in `input/content` will be parsed as
-  Jinja2 templates, they can use templates defined in `input/templates`.  
+  Jinja2 templates, they can use templates defined in `input/templates`.
   See the [Jinja2 documentation](https://jinja.palletsprojects.com/en/3.0.x/templates/)
 
-  Example:  
-  `input/content/index.html` -> `output/index.html`  
-  Starting with content  
+  Example:
+  `input/content/index.html` -> `output/index.html`
+  Starting with content
+
   ```jinja2
   {% extends "base.html" %}
 
   ...
   ```
+
   Will use the template `input/templates/base.html`
 
 - CSS files in `input/css` will be merged together in a single file
   `output/bundle.css`
 
 - Markdown files with the suffix .md placed in `input/content` will be parsed to
   HTML and passed to a template with the same name as their parent folder as the
   parameter `markdown`
 
-  Example:  
-  `./input/content/post/hello-world.md` -> `./output/post/hello-world.html`  
-  Using the template `./input/templates/post.html`  
+  Example:
+  `./input/content/post/hello-world.md` -> `./output/post/hello-world.html`
+  Using the template `./input/templates/post.html`
   Generated with context `{'markdown': 'the markdown file converted to HTML'}`
 
   The template name can be overriden using the markdown meta argument "template"
 
-  Example:  
-  `./input/content/post/special.md` -> `./output/post/special.html`  
-  Starting with content  
+  Example:
+  `./input/content/post/special.md` -> `./output/post/special.html`
+  Starting with content
+
   ```md
   ---
   template: special.html
   ---
 
   ...
   ```
+
   Will use the template `./input/templates/special.html` instead of `post.html`
-  
-  ## Examples
-  
-  See [the `example` branch for an example input folder](https://github.com/Tina-otoge/sssimp/tree/example)
 
+- Files placed in `input/data` will exposes their content in templates inside
+  the `data` variable. They can be in either YAML or JSON. The path is part of
+  their position in the data structure tree.
+
+  Example:
+  `./input/data/categories/tech.yml`
+  With content
+
+  ```yaml
+  description: Nerdy stuff
+  color: #121212
+  related:
+    - computers
+    - dev
+  ```
+
+  Will populate the `data` variable in templates as so:
+
+  ```json
+  {
+    "categories": [
+      {
+        "tech": {
+          "description": "Nerdy stuff",
+          "color": "#121212",
+          "related": ["computers", "dev"]
+        }
+      }
+    ]
+  }
+  ```
+
+## Examples
+
+  See [the `example` branch for an example input folder](https://github.com/Tina-otoge/sssimp/tree/example)
+  or my personal website https://github.com/Tina-otoge/tina-simp for a real-world example.
 
 ## Additional Jinja2 filters
 
 - `|a` makes any relative path point to the top of the output folder.
 
-  Example:  
+  Example:
   `input/content/blog/post/tech/2021/11/some-post.html`
-  -> `output/blog/post/tech/2021/11/some-post.html`  
+  -> `output/blog/post/tech/2021/11/some-post.html`
   With content
+
   ```html
   <link rel="stylesheet" href="{{ "style.css"|a }}">
   ```
+
   Will be rendered as `"../../../../style.css"`
 
   See also [the `<base>` element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/base)
 
 ## Additional Jinja2 variables
 
 - `page` is a `sssimp.generators.html.Page`, it contains many information about
 the current document. Markdown files are an instance of
 `sssimp.generators.markdown.MarkdownPage` instead, which inherits from `Page`
 
   This variable itself contains many useful variables:
-  - `page.last_modified` and `page.created_at` (may be the same on Linux)
+  - `page.modified_at` and `page.created_at` (`modified_at` forcibly set to `None` if same as `created_at`)
   - `page.href`: The path to the file relative to the output folder
   - `page.src`: A `pathlib.Path` object of the source file in the input folder
   - `page.target` A `pathlib.Path` object of the target file in the output
 folder
   - `page.name`: Shortcut for `page.target.name`, the filename of the outputed
     file
   - `page.parent`: Shortcut for `page.target.parent`, the name of the parent
 directory in the output folder
 file
   - `page.meta`: The Markdown meta variables, prefixing a var with `=` will
     interpret it as raw JSON
     Example
+
     ```markdown
     ---
     some_var: some value
     something_else: 42
     some_tags:= ["tag1", "tag2"]
     ---
 
     My cool blog post
     ...
     ```
+
     The meta variable will always contain a `template` which will resolve to the
     parent directory name with .html appended if none is set in the meta fields.
 
     The `page.meta` variable is `None` for raw HTML pages, this avoids KeyErrors
     when trying to filter pages by a specific meta variable.
 - `plain_text`[^md]: A plain text representation of the Markdown file
 - `markdown`[^md]: The Markdown content converted to HTML
 - `meta`[^md]: A shortcut for `page.meta`
 - `title`[^md]: Returns `page.meta.title` if it exists, else the filename with
   the characters `-` and `_` replaced by whitespaces, the suffix removed and the
   first letter capitalized.
 
-  Example:  
+  Example:
   `input/content/some-cool-page.md`'s title is "Some cool page"
 - `BUNDLE_FILE` always evaluates to `"bundle.css"` for now
 - `BUNDLE_TIME` modification time of the latest updated file in `input/css`,
   very useful to make the browser refresh the file only if any of the CSS files
   changed.
 
   Example:
+
   ```html
   <link rel="stylesheet" href="{{ BUNDLE_FILE}}?{{ BUNDLE_TIME }}">
   ```
+
 - `PAGES` a list of `sssimp.generators.html.Page` objects containing every HTML
   and Markdown files sourced by the site. You can loop over it to generate an
   index. In conjunction with looking up meta values it can be used to filter by
   content type.
 
   Example:
+
   ```html+jinja
   {% for page in PAGES if page.meta.template == 'post.html' %}
   <a href="{{ page.href }}">{{ page.title }}</a>
   <div class="tags">
     {% for tag in page.meta.tags %}
     <span class="tag">{{ tag }}</span>
     {% endfor %}
```

### Comparing `sssimp-0.0.9/src/sssimp/generators/css.py` & `sssimp-0.1.0/src/sssimp/generators/css.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 import logging
+
 import sssimp
 from sssimp import config, jinja
 from sssimp.utils import mkdir, path_strip
 
-
-BUNDLE_FILE = 'bundle.css'
+BUNDLE_FILE = "bundle.css"
 OUT_FILE = sssimp.OUTPUT_DIR / BUNDLE_FILE
-CSS_DIR = sssimp.INPUT_DIR / 'css'
+CSS_DIR = sssimp.INPUT_DIR / "css"
 css_files = None
 
+
 def prepare():
     global css_files
-    jinja.globals['BUNDLE_FILE'] = BUNDLE_FILE
+    jinja.globals["BUNDLE_FILE"] = BUNDLE_FILE
     css_files = list(
         [CSS_DIR / file for file in config.CSS_FILES]
-        if config.CSS_FILES else
-        CSS_DIR.glob('**/*.css')
+        if config.CSS_FILES
+        else CSS_DIR.glob("**/*.css")
     )
-    jinja.globals['BUNDLE_TIME'] = max(x.stat().st_ctime for x in css_files)
+    if css_files:
+        jinja.globals["BUNDLE_TIME"] = max(x.stat().st_ctime for x in css_files)
+
 
 def main():
+    if not css_files:
+        logging.debug("No CSS files found, skipping")
+        return
     mkdir(OUT_FILE)
-    with open(OUT_FILE, 'w') as out:
+    with open(OUT_FILE, "w") as out:
         for file in css_files:
             relative_path = path_strip(file, CSS_DIR)
-            logging.info(f'Bundling {relative_path}')
-            print(f'/** bundle:{relative_path} **/', file=out)
+            logging.info(f"Bundling {relative_path}")
+            print(f"/** bundle:{relative_path} **/", file=out)
             with open(file) as css_file:
                 out.write(css_file.read())
             print(file=out)
```

### Comparing `sssimp-0.0.9/src/sssimp/generators/html.py` & `sssimp-0.1.0/src/sssimp/generators/html.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,75 +1,84 @@
-import logging
 import functools
+import logging
+from datetime import datetime
+from pathlib import Path
+
 import sssimp
 from sssimp import jinja
 from sssimp.utils import mkdir, path_strip
 
-
 PAGES = set()
 
 
 class Page:
     def __init__(self, src, target):
         self.src = src
         self.target = target
         self.vars = {
-            'page': self,
+            "page": self,
         }
         self.meta = None
 
     def __str__(self):
         return str(self.target)
 
     @property
     def created_at(self):
-        return self.stat.st_ctime
+        return datetime.fromtimestamp(self.stat.st_ctime)
 
     @property
-    def last_modified(self):
-        return self.stat.st_mtime
+    def updated_at(self):
+        time = datetime.fromtimestamp(self.stat.st_mtime)
+        if time == self.created_at:
+            return None
+        return time
 
     @property
-    @functools.cache
+    # TODO 3.9+: @functools.cache
+    # 3.8 compat:
+    @functools.lru_cache()
     def stat(self):
         return self.src.stat()
 
     @property
     def href(self):
-        return path_strip(self.target, sssimp.OUTPUT_DIR)
+        return "/".join(Path(path_strip(self.target, sssimp.OUTPUT_DIR)).parts)
 
     @property
     def name(self):
         return self.target.name
 
     @property
     def parent(self):
         return self.target.parent
 
     def get_template(self):
         with open(self.src) as f:
             content = f.read()
         return jinja.from_string(content)
 
-    @functools.cache
+    # TODO 3.9+: @functools.cache
+    # 3.8 compat:
+    @functools.lru_cache()
     def render(self):
-        return self.get_template().render(**self.vars)
+        return self.get_template().render(**self.vars) + "\n"
 
     def write(self, target=None):
         target = target or self.target
         mkdir(self.target)
-        with open(self.target, 'w') as f:
-            logging.info(f'Generating {self.target}')
+        with open(self.target, "w") as f:
+            logging.info(f"Generating {self.target}")
             f.write(self.render())
 
 
 def prepare():
-    for file in sssimp.CONTENT_DIR.glob('**/*.html'):
+    for file in sssimp.CONTENT_DIR.glob("**/*.html"):
         target = sssimp.OUTPUT_DIR / path_strip(file, sssimp.CONTENT_DIR)
         PAGES.add(Page(src=file, target=target))
         sssimp.IGNORE_ASSETS.add(str(file))
 
 
 def main():
-    jinja.globals['PAGES'] = PAGES
+    jinja.globals["pages"] = PAGES
     for page in PAGES:
         page.write()
```

### Comparing `sssimp-0.0.9/src/sssimp.egg-info/PKG-INFO` & `sssimp-0.1.0/src/sssimp.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,195 +1,235 @@
 Metadata-Version: 2.1
 Name: sssimp
-Version: 0.0.9
-Summary: A simple static website generator
-Home-page: https://github.com/Tina-otoge/sssimp
-Author: Tina
-Author-email: me@tina.moe
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 0.1.0
+Summary: The Static Site Solution In Modern Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jinja2
+Requires-Dist: markdown
+Requires-Dist: pymdown-extensions
+Requires-Dist: pyyaml
 
 # sssimp 🐍
-Simple Static SIte Maker in Python
+
+The **S**tatic **S**ite **S**olution **I**n **M**odern **P**ython
+
+It's simp with 3 s!
 
 A simple tool to generate a static website while being able to use powerful HTML
 templates (Jinja2), Markdown files converted to HTML, and other preprocessors.
 
-
 ## Why?
 
 I wanted a simple way to generate static websites and I like Jinja2. I had
 previous experiences working with Jekyll but it seemed like too much work to
 setup everytime and overkill for the job as it supports many features I don't
 necessarily use.
 
+One of the main goals with sssimp is being able to generate a usable website
+without any configuration file or dependency. You only install the sssimp
+package and run it.
+
 ## Installing
 
+Requirement: Python 3.8 or later
+
 ```
-pip install sssimp
+pip install --user sssimp
 ```
 
 ## How to use
 
 Create a folder called `input`, it will hold the data to generate the site.
 
-Running `python -m sssimp` will generate content in the `output` folder.
+Running `sssimp` will generate content in the `output` folder.
 
-Here is an example script for UNIX that will regenerate the site everytime a
-file changes, useful during development:
-```bash
-trap "echo Exited!; exit 1;" SIGINT SIGTERM
+Input and output destination can be changed:
 
-while true; do
-	python -m venv .venv
-	source .venv/bin/activate
-	pip install --upgrade sssimp
-	python -m sssimp
-
-	echo Waiting for change
-	watch -g ls -lR .
-done
+```bash
+sssimp --input ../some-other/input-dir ~/some-other/output-dir
 ```
 
+Use `python -m sssimp --help` for more details.
+
 ## Generators
 
 - Files placed in `input/content` will be directly copied to the `output` folder
 
-  Example:  
+  Example:
   `input/content/favicon.png` -> `output/favicon.png`
 
 - HTML files with the suffix .html placed in `input/content` will be parsed as
-  Jinja2 templates, they can use templates defined in `input/templates`.  
+  Jinja2 templates, they can use templates defined in `input/templates`.
   See the [Jinja2 documentation](https://jinja.palletsprojects.com/en/3.0.x/templates/)
 
-  Example:  
-  `input/content/index.html` -> `output/index.html`  
-  Starting with content  
+  Example:
+  `input/content/index.html` -> `output/index.html`
+  Starting with content
+
   ```jinja2
   {% extends "base.html" %}
 
   ...
   ```
+
   Will use the template `input/templates/base.html`
 
 - CSS files in `input/css` will be merged together in a single file
   `output/bundle.css`
 
 - Markdown files with the suffix .md placed in `input/content` will be parsed to
   HTML and passed to a template with the same name as their parent folder as the
   parameter `markdown`
 
-  Example:  
-  `./input/content/post/hello-world.md` -> `./output/post/hello-world.html`  
-  Using the template `./input/templates/post.html`  
+  Example:
+  `./input/content/post/hello-world.md` -> `./output/post/hello-world.html`
+  Using the template `./input/templates/post.html`
   Generated with context `{'markdown': 'the markdown file converted to HTML'}`
 
   The template name can be overriden using the markdown meta argument "template"
 
-  Example:  
-  `./input/content/post/special.md` -> `./output/post/special.html`  
-  Starting with content  
+  Example:
+  `./input/content/post/special.md` -> `./output/post/special.html`
+  Starting with content
+
   ```md
   ---
   template: special.html
   ---
 
   ...
   ```
+
   Will use the template `./input/templates/special.html` instead of `post.html`
-  
-  ## Examples
-  
-  See [the `example` branch for an example input folder](https://github.com/Tina-otoge/sssimp/tree/example)
 
+- Files placed in `input/data` will exposes their content in templates inside
+  the `data` variable. They can be in either YAML or JSON. The path is part of
+  their position in the data structure tree.
+
+  Example:
+  `./input/data/categories/tech.yml`
+  With content
+
+  ```yaml
+  description: Nerdy stuff
+  color: #121212
+  related:
+    - computers
+    - dev
+  ```
+
+  Will populate the `data` variable in templates as so:
+
+  ```json
+  {
+    "categories": [
+      {
+        "tech": {
+          "description": "Nerdy stuff",
+          "color": "#121212",
+          "related": ["computers", "dev"]
+        }
+      }
+    ]
+  }
+  ```
+
+## Examples
+
+  See [the `example` branch for an example input folder](https://github.com/Tina-otoge/sssimp/tree/example)
+  or my personal website https://github.com/Tina-otoge/tina-simp for a real-world example.
 
 ## Additional Jinja2 filters
 
 - `|a` makes any relative path point to the top of the output folder.
 
-  Example:  
+  Example:
   `input/content/blog/post/tech/2021/11/some-post.html`
-  -> `output/blog/post/tech/2021/11/some-post.html`  
+  -> `output/blog/post/tech/2021/11/some-post.html`
   With content
+
   ```html
   <link rel="stylesheet" href="{{ "style.css"|a }}">
   ```
+
   Will be rendered as `"../../../../style.css"`
 
   See also [the `<base>` element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/base)
 
 ## Additional Jinja2 variables
 
 - `page` is a `sssimp.generators.html.Page`, it contains many information about
 the current document. Markdown files are an instance of
 `sssimp.generators.markdown.MarkdownPage` instead, which inherits from `Page`
 
   This variable itself contains many useful variables:
-  - `page.last_modified` and `page.created_at` (may be the same on Linux)
+  - `page.modified_at` and `page.created_at` (`modified_at` forcibly set to `None` if same as `created_at`)
   - `page.href`: The path to the file relative to the output folder
   - `page.src`: A `pathlib.Path` object of the source file in the input folder
   - `page.target` A `pathlib.Path` object of the target file in the output
 folder
   - `page.name`: Shortcut for `page.target.name`, the filename of the outputed
     file
   - `page.parent`: Shortcut for `page.target.parent`, the name of the parent
 directory in the output folder
 file
   - `page.meta`: The Markdown meta variables, prefixing a var with `=` will
     interpret it as raw JSON
     Example
+
     ```markdown
     ---
     some_var: some value
     something_else: 42
     some_tags:= ["tag1", "tag2"]
     ---
 
     My cool blog post
     ...
     ```
+
     The meta variable will always contain a `template` which will resolve to the
     parent directory name with .html appended if none is set in the meta fields.
 
     The `page.meta` variable is `None` for raw HTML pages, this avoids KeyErrors
     when trying to filter pages by a specific meta variable.
 - `plain_text`[^md]: A plain text representation of the Markdown file
 - `markdown`[^md]: The Markdown content converted to HTML
 - `meta`[^md]: A shortcut for `page.meta`
 - `title`[^md]: Returns `page.meta.title` if it exists, else the filename with
   the characters `-` and `_` replaced by whitespaces, the suffix removed and the
   first letter capitalized.
 
-  Example:  
+  Example:
   `input/content/some-cool-page.md`'s title is "Some cool page"
 - `BUNDLE_FILE` always evaluates to `"bundle.css"` for now
 - `BUNDLE_TIME` modification time of the latest updated file in `input/css`,
   very useful to make the browser refresh the file only if any of the CSS files
   changed.
 
   Example:
+
   ```html
   <link rel="stylesheet" href="{{ BUNDLE_FILE}}?{{ BUNDLE_TIME }}">
   ```
+
 - `PAGES` a list of `sssimp.generators.html.Page` objects containing every HTML
   and Markdown files sourced by the site. You can loop over it to generate an
   index. In conjunction with looking up meta values it can be used to filter by
   content type.
 
   Example:
+
   ```html+jinja
   {% for page in PAGES if page.meta.template == 'post.html' %}
   <a href="{{ page.href }}">{{ page.title }}</a>
   <div class="tags">
     {% for tag in page.meta.tags %}
     <span class="tag">{{ tag }}</span>
     {% endfor %}
   </div>
   Posted on <time>{{ page.created_at }}</time>
   {% endfor %}
   ```
 
 [^md]: Markdown only
-
-
```

