# Comparing `tmp/pdf4llm-0.0.6.tar.gz` & `tmp/pdf4llm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf4llm-0.0.6.tar", last modified: Wed Apr 24 21:15:24 2024, max compression
+gzip compressed data, was "pdf4llm-0.0.7.tar", last modified: Sat Apr 27 10:55:17 2024, max compression
```

## Comparing `pdf4llm-0.0.6.tar` & `pdf4llm-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 21:15:24.194383 pdf4llm-0.0.6/
--rw-rw-rw-   0        0        0     1740 2024-04-24 21:15:24.193386 pdf4llm-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2024-04-24 14:40:20.000000 pdf4llm-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 21:15:24.174385 pdf4llm-0.0.6/pdf4llm/
--rw-rw-rw-   0        0        0       46 2024-04-22 23:14:44.000000 pdf4llm-0.0.6/pdf4llm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 21:15:24.190403 pdf4llm-0.0.6/pdf4llm/helpers/
--rw-rw-rw-   0        0        0    13775 2024-04-23 08:06:26.000000 pdf4llm-0.0.6/pdf4llm/helpers/pymupdf_rag.py
-drwxrwxrwx   0        0        0        0 2024-04-24 21:15:24.191385 pdf4llm-0.0.6/pdf4llm.egg-info/
--rw-rw-rw-   0        0        0     1740 2024-04-24 21:15:24.000000 pdf4llm-0.0.6/pdf4llm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-04-24 21:15:24.000000 pdf4llm-0.0.6/pdf4llm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 21:15:24.000000 pdf4llm-0.0.6/pdf4llm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-24 21:15:24.000000 pdf4llm-0.0.6/pdf4llm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 21:15:24.000000 pdf4llm-0.0.6/pdf4llm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 21:15:24.194383 pdf4llm-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      967 2024-04-24 21:14:17.000000 pdf4llm-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:55:17.601847 pdf4llm-0.0.7/
+-rw-rw-rw-   0        0        0     1740 2024-04-27 10:55:17.600848 pdf4llm-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2024-04-24 14:40:20.000000 pdf4llm-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 10:55:17.585338 pdf4llm-0.0.7/pdf4llm/
+-rw-rw-rw-   0        0        0       46 2024-04-22 23:14:44.000000 pdf4llm-0.0.7/pdf4llm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:55:17.599848 pdf4llm-0.0.7/pdf4llm/helpers/
+-rw-rw-rw-   0        0        0    14027 2024-04-27 10:43:44.000000 pdf4llm-0.0.7/pdf4llm/helpers/pymupdf_rag.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:55:17.600848 pdf4llm-0.0.7/pdf4llm.egg-info/
+-rw-rw-rw-   0        0        0     1740 2024-04-27 10:55:17.000000 pdf4llm-0.0.7/pdf4llm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-04-27 10:55:17.000000 pdf4llm-0.0.7/pdf4llm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 10:55:17.000000 pdf4llm-0.0.7/pdf4llm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-27 10:55:17.000000 pdf4llm-0.0.7/pdf4llm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 10:55:17.000000 pdf4llm-0.0.7/pdf4llm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 10:55:17.601847 pdf4llm-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      967 2024-04-27 10:54:38.000000 pdf4llm-0.0.7/setup.py
```

### Comparing `pdf4llm-0.0.6/PKG-INFO` & `pdf4llm-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf4llm
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyMuPDF Utilities for LLM/RAG
 Home-page: https://github.com/pymupdf/RAG
 Author: Artifex
 Author-email: support@artifex.com
 License: GNU AFFERO GPL 3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pdf4llm-0.0.6/README.md` & `pdf4llm-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pdf4llm-0.0.6/pdf4llm/helpers/pymupdf_rag.py` & `pdf4llm-0.0.7/pdf4llm/helpers/pymupdf_rag.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,20 +77,27 @@
                 ]:
                     fontsz = round(span["size"])
                     count = fontsizes.get(fontsz, 0) + len(span["text"].strip())
                     fontsizes[fontsz] = count
 
             # maps a fontsize to a string of multiple # header tag characters
             self.header_id = {}
-            if body_limit is None:  # body text fontsize if not provided
-                body_limit = sorted(
+
+            # If not provided, choose the most frequent font size as body text.
+            # If no text at all on all pages, just use 12
+            if body_limit is None:
+                temp = sorted(
                     [(k, v) for k, v in fontsizes.items()],
                     key=lambda i: i[1],
                     reverse=True,
-                )[0][0]
+                )
+                if temp:
+                    body_limit = temp[0][0]
+                else:
+                    body_limit = 12
 
             sizes = sorted(
                 [f for f in fontsizes.keys() if f > body_limit], reverse=True
             )
 
             # make the header tag dictionary
             for i, size in enumerate(sizes):
@@ -306,14 +313,15 @@
     return md_string
 
 
 if __name__ == "__main__":
     import os
     import sys
     import time
+    import pathlib
 
     try:
         filename = sys.argv[1]
     except IndexError:
         print(f"Usage:\npython {os.path.basename(__file__)} input.pdf")
         sys.exit()
 
@@ -339,12 +347,11 @@
         if wrong_pages != set():  # if any invalid numbers given, exit.
             sys.exit(f"Page number(s) {wrong_pages} not in '{doc}'.")
 
     # get the markdown string
     md_string = to_markdown(doc, pages=pages)
 
     # output to a text file with extension ".md"
-    out = open(doc.name.replace(".pdf", ".md"), "w")
-    out.write(md_string)
-    out.close()
+    outname = doc.name.replace(".pdf", ".md")
+    pathlib.Path(outname).write_bytes(md_string.encode())
     t1 = time.perf_counter()  # stop timer
     print(f"Markdown creation time for {doc.name=} {round(t1-t0,2)} sec.")
```

### Comparing `pdf4llm-0.0.6/pdf4llm.egg-info/PKG-INFO` & `pdf4llm-0.0.7/pdf4llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf4llm
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyMuPDF Utilities for LLM/RAG
 Home-page: https://github.com/pymupdf/RAG
 Author: Artifex
 Author-email: support@artifex.com
 License: GNU AFFERO GPL 3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pdf4llm-0.0.6/setup.py` & `pdf4llm-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3",
     "Topic :: Utilities",
 ]
 requires = ["pymupdf>=1.24.2"]
 
 setuptools.setup(
     name="pdf4llm",
-    version="0.0.6",
+    version="0.0.7",
     author="Artifex",
     author_email="support@artifex.com",
     description="PyMuPDF Utilities for LLM/RAG",
     packages=setuptools.find_packages(),
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requires,
```

