# Comparing `tmp/state_graph-0.1.1.tar.gz` & `tmp/state_graph-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "state_graph-0.1.1.tar", last modified: Sat Apr 27 11:24:29 2024, max compression
+gzip compressed data, was "state_graph-0.1.2.tar", last modified: Sat Apr 27 12:22:41 2024, max compression
```

## Comparing `state_graph-0.1.1.tar` & `state_graph-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 11:24:29.355243 state_graph-0.1.1/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      196 2024-04-27 11:24:29.355071 state_graph-0.1.1/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-04-27 11:24:29.355279 state_graph-0.1.1/setup.cfg
--rw-r--r--   0 salamanderxing   (501) staff       (20)      276 2024-04-27 11:24:10.000000 state_graph-0.1.1/setup.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 11:24:29.353998 state_graph-0.1.1/state_graph/
--rw-r--r--   0 salamanderxing   (501) staff       (20)    19491 2024-04-27 11:23:37.000000 state_graph-0.1.1/state_graph/__init__.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 11:24:29.354900 state_graph-0.1.1/state_graph.egg-info/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      196 2024-04-27 11:24:29.000000 state_graph-0.1.1/state_graph.egg-info/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)      206 2024-04-27 11:24:29.000000 state_graph-0.1.1/state_graph.egg-info/SOURCES.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-04-27 11:24:29.000000 state_graph-0.1.1/state_graph.egg-info/dependency_links.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       51 2024-04-27 11:24:29.000000 state_graph-0.1.1/state_graph.egg-info/requires.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       12 2024-04-27 11:24:29.000000 state_graph-0.1.1/state_graph.egg-info/top_level.txt
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 12:22:41.810512 state_graph-0.1.2/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      196 2024-04-27 12:22:41.810311 state_graph-0.1.2/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-04-27 12:22:41.810566 state_graph-0.1.2/setup.cfg
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      319 2024-04-27 12:22:38.000000 state_graph-0.1.2/setup.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 12:22:41.809325 state_graph-0.1.2/state_graph/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    19525 2024-04-27 12:16:08.000000 state_graph-0.1.2/state_graph/__init__.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 12:22:41.810101 state_graph-0.1.2/state_graph.egg-info/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      196 2024-04-27 12:22:41.000000 state_graph-0.1.2/state_graph.egg-info/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      206 2024-04-27 12:22:41.000000 state_graph-0.1.2/state_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-04-27 12:22:41.000000 state_graph-0.1.2/state_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       51 2024-04-27 12:22:41.000000 state_graph-0.1.2/state_graph.egg-info/requires.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       12 2024-04-27 12:22:41.000000 state_graph-0.1.2/state_graph.egg-info/top_level.txt
```

### Comparing `state_graph-0.1.1/state_graph/__init__.py` & `state_graph-0.1.2/state_graph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,22 +480,23 @@
         </head>
         <body style="background-color: #222; padding: 0; margin:0;">
             <div class="mermaid">
                 {mermaid_diagram}
             </div>
         </body>
         </html>"""
+        return out_html
 
         # if destination is None:
         #     destination = "."
-        if destination is not None:
-            with open(os.path.join(destination, "graph.html"), "w") as f:
-                f.write(out_html)
-        else:
-            display(HTML(out_html))
+        # if destination is not None:
+        #     with open(os.path.join(destination, "graph.html"), "w") as f:
+        #         f.write(out_html)
+        # else:
+        #     display(HTML(out_html))
 
 
 async def main():
 
     async def stream_token(token: str):
         print(token)
```

