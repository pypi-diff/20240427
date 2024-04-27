# Comparing `tmp/mypycounts-0.1.0.tar.gz` & `tmp/mypycounts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypycounts-0.1.0.tar", max compression
+gzip compressed data, was "mypycounts-0.2.0.tar", max compression
```

## Comparing `mypycounts-0.1.0.tar` & `mypycounts-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,13 @@
--rw-r--r--   0        0        0     1102 2024-04-21 13:39:59.692788 mypycounts-0.1.0/LICENSE
--rw-r--r--   0        0        0      598 2024-04-23 07:54:14.126122 mypycounts-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1048 2024-04-22 23:06:05.907872 mypycounts-0.1.0/README.md
--rw-r--r--   0        0        0      114 2024-04-21 13:40:07.740082 mypycounts-0.1.0/src/mypycounts/__init__.py
--rw-r--r--   0        0        0     1640 2024-04-23 04:37:42.362253 mypycounts-0.1.0/src/mypycounts/mypycounts.py
--rw-r--r--   0        0        0      844 2024-04-23 10:44:55.317935 mypycounts-0.1.0/src/mypycounts/plotting.py
--rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 mypycounts-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3297 2024-04-26 15:24:58.946177 mypycounts-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1102 2024-04-21 13:39:59.692788 mypycounts-0.2.0/LICENSE
+-rw-r--r--   0        0        0      841 2024-04-27 12:59:06.437641 mypycounts-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1048 2024-04-22 23:06:05.907872 mypycounts-0.2.0/README.md
+-rw-r--r--   0        0        0      237 2024-04-23 14:26:38.866783 mypycounts-0.2.0/src/mypycounts/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 14:39:02.712000 mypycounts-0.2.0/src/mypycounts/data/__init__.py
+-rw-r--r--   0        0        0   198827 2024-04-24 10:21:36.289989 mypycounts-0.2.0/src/mypycounts/data/flatland.txt
+-rw-r--r--   0        0        0      411 2024-04-24 15:47:19.721085 mypycounts-0.2.0/src/mypycounts/datasets.py
+-rw-r--r--   0        0        0     1658 2024-04-24 10:43:10.438920 mypycounts-0.2.0/src/mypycounts/mypycounts.py
+-rw-r--r--   0        0        0      994 2024-04-24 16:42:25.126079 mypycounts-0.2.0/src/mypycounts/plotting.py
+-rw-r--r--   0        0        0       79 2024-04-22 21:42:21.909026 mypycounts-0.2.0/tests/einstein.txt
+-rw-r--r--   0        0        0     1880 2024-04-24 15:04:12.862626 mypycounts-0.2.0/tests/test_mypycounts.py
+-rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 mypycounts-0.2.0/PKG-INFO
```

### Comparing `mypycounts-0.1.0/LICENSE` & `mypycounts-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypycounts-0.1.0/pyproject.toml` & `mypycounts-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 [tool.poetry]
 name = "mypycounts"
-version = "0.1.0"
+version = "0.2.0"
 description = "A package for counting words and others."
 authors = ["Emmanuel Arkoh-Nelson"]
 license = "MIT"
 readme = "README.md"
+include = ["tests/*", "CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 matplotlib = ">=3.8.4"
+click-option-group = { version = "*", python = ">=3.9,<4" }  # Specify Python version constraint
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 jupyter = "^1.0.0"
 myst-nb = {version = "^1.1.0", python = "^3.9"}
 sphinx-autoapi = "^3.0.0"
 sphinx-rtd-theme = "^2.0.0"
+python-semantic-release = "^9.5.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.semantic_release]
+version_variable = "pyproject.toml:version"
```

### Comparing `mypycounts-0.1.0/README.md` & `mypycounts-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mypycounts-0.1.0/src/mypycounts/mypycounts.py` & `mypycounts-0.2.0/src/mypycounts/mypycounts.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     str
         Text file contents.
 
     Examples
     --------
     >>> load_text("text.txt")
     """
-    with open(input_file, "r") as file:
+    with open(input_file, "r", encoding="utf-8") as file:
         text = file.read()
     return text
 
 def clean_text(text):
     """Lowercase and remove punctuation from a string.
 
     Parameters
```

### Comparing `mypycounts-0.1.0/src/mypycounts/plotting.py` & `mypycounts-0.2.0/src/mypycounts/plotting.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import matplotlib.pyplot as plt
+from collections import Counter
 
 def plot_words(word_counts, n=10):
-    """plot a bar chart of word counts.
+    """Plot a bar chart of word counts.
     
     Parameters
     ----------
     word_counts : collections.Counter
         Counter object of word counts.
     n : int, optional
         Plot the top n words. By default, 10.
@@ -19,14 +20,16 @@
     --------
     >>> from pycounts.pycounts import count_words
     >>> from pycounts.plotting import plot_words
     >>> counts = count_words("text.txt")
     >>> plot_words(counts)
     """
     
+    if not isinstance(word_counts, Counter):
+        raise TypeError("'word_counts' should be type of 'Counter'.")
     top_n_words = word_counts.most_common(n)
     word, count = zip(*top_n_words)
     fig = plt.bar(range(n), count)
     plt.xticks(range(n), word, rotation=45)
     plt.xlabel("Word")
     plt.ylabel("Count")
     return fig
```

### Comparing `mypycounts-0.1.0/PKG-INFO` & `mypycounts-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: mypycounts
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package for counting words and others.
 License: MIT
 Author: Emmanuel Arkoh-Nelson
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click-option-group ; python_version >= "3.9" and python_version < "4"
 Requires-Dist: matplotlib (>=3.8.4)
 Description-Content-Type: text/markdown
 
 # mypycounts
 
 A package for counting words and others.
```

