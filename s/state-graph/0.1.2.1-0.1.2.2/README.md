# Comparing `tmp/state_graph-0.1.2.1.tar.gz` & `tmp/state_graph-0.1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "state_graph-0.1.2.1.tar", last modified: Sat Apr 27 12:28:28 2024, max compression
+gzip compressed data, was "state_graph-0.1.2.2.tar", last modified: Sat Apr 27 12:33:12 2024, max compression
```

## Comparing `state_graph-0.1.2.1.tar` & `state_graph-0.1.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 12:28:28.690584 state_graph-0.1.2.1/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      198 2024-04-27 12:28:28.690421 state_graph-0.1.2.1/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-04-27 12:28:28.690637 state_graph-0.1.2.1/setup.cfg
--rw-r--r--   0 salamanderxing   (501) staff       (20)      321 2024-04-27 12:28:27.000000 state_graph-0.1.2.1/setup.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 12:28:28.689460 state_graph-0.1.2.1/state_graph/
--rw-r--r--   0 salamanderxing   (501) staff       (20)    20212 2024-04-27 12:28:06.000000 state_graph-0.1.2.1/state_graph/__init__.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 12:28:28.690248 state_graph-0.1.2.1/state_graph.egg-info/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      198 2024-04-27 12:28:28.000000 state_graph-0.1.2.1/state_graph.egg-info/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)      206 2024-04-27 12:28:28.000000 state_graph-0.1.2.1/state_graph.egg-info/SOURCES.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-04-27 12:28:28.000000 state_graph-0.1.2.1/state_graph.egg-info/dependency_links.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       51 2024-04-27 12:28:28.000000 state_graph-0.1.2.1/state_graph.egg-info/requires.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       12 2024-04-27 12:28:28.000000 state_graph-0.1.2.1/state_graph.egg-info/top_level.txt
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 12:33:12.747562 state_graph-0.1.2.2/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      198 2024-04-27 12:33:12.747378 state_graph-0.1.2.2/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-04-27 12:33:12.747602 state_graph-0.1.2.2/setup.cfg
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      321 2024-04-27 12:33:09.000000 state_graph-0.1.2.2/setup.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 12:33:12.746396 state_graph-0.1.2.2/state_graph/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    20216 2024-04-27 12:32:23.000000 state_graph-0.1.2.2/state_graph/__init__.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 12:33:12.747185 state_graph-0.1.2.2/state_graph.egg-info/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      198 2024-04-27 12:33:12.000000 state_graph-0.1.2.2/state_graph.egg-info/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      206 2024-04-27 12:33:12.000000 state_graph-0.1.2.2/state_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-04-27 12:33:12.000000 state_graph-0.1.2.2/state_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       51 2024-04-27 12:33:12.000000 state_graph-0.1.2.2/state_graph.egg-info/requires.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       12 2024-04-27 12:33:12.000000 state_graph-0.1.2.2/state_graph.egg-info/top_level.txt
```

### Comparing `state_graph-0.1.2.1/state_graph/__init__.py` & `state_graph-0.1.2.2/state_graph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,16 +503,16 @@
                 });
             """
                 )
             )
 
         # return out_html
 
-        if destination is None:
-            destination = "."
+        # if destination is None:
+        #     destination = "."
         if destination is not None:
             with open(os.path.join(destination, "graph.html"), "w") as f:
                 f.write(out_html)
         else:
             display(HTML(out_html))
```

