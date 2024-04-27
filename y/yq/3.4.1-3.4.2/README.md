# Comparing `tmp/yq-3.4.1.tar.gz` & `tmp/yq-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yq-3.4.1.tar", last modified: Wed Apr 17 23:37:50 2024, max compression
+gzip compressed data, was "yq-3.4.2.tar", last modified: Fri Apr 26 17:48:26 2024, max compression
```

## Comparing `yq-3.4.1.tar` & `yq-3.4.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:37:50.491276 yq-3.4.1/
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:37:50.474407 yq-3.4.1/.github/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       18 2023-10-23 21:28:59.000000 yq-3.4.1/.github/FUNDING.yml
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:37:50.474948 yq-3.4.1/.github/workflows/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      945 2024-04-15 18:14:25.000000 yq-3.4.1/.github/workflows/ci.yml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      477 2023-10-23 21:28:59.000000 yq-3.4.1/.gitignore
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8429 2024-04-17 23:37:27.000000 yq-3.4.1/Changes.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10273 2023-10-23 21:28:59.000000 yq-3.4.1/LICENSE
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       41 2023-10-23 21:28:59.000000 yq-3.4.1/MANIFEST.in
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      478 2023-10-23 21:28:59.000000 yq-3.4.1/Makefile
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8985 2024-04-17 23:37:50.490663 yq-3.4.1/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7731 2024-04-17 23:14:42.000000 yq-3.4.1/README.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      696 2023-10-23 21:29:01.000000 yq-3.4.1/SECURITY.md
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2542 2024-04-15 18:14:25.000000 yq-3.4.1/common.mk
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:37:50.478911 yq-3.4.1/docs/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:28:59.000000 yq-3.4.1/docs/changelog.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3515 2024-04-17 23:37:27.000000 yq-3.4.1/docs/cli-doc-tomlq.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3897 2024-04-17 23:37:27.000000 yq-3.4.1/docs/cli-doc-xq.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     4503 2024-04-17 23:37:27.000000 yq-3.4.1/docs/cli-doc.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      806 2023-10-23 21:28:59.000000 yq-3.4.1/docs/conf.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      248 2023-10-23 21:28:59.000000 yq-3.4.1/docs/index.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        8 2023-10-23 21:28:59.000000 yq-3.4.1/docs/toc.html
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      416 2024-04-15 18:14:25.000000 yq-3.4.1/pyproject.toml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       38 2024-04-17 23:37:50.491355 yq-3.4.1/setup.cfg
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1677 2024-04-17 23:37:23.000000 yq-3.4.1/setup.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:37:50.481151 yq-3.4.1/test/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3468 2023-10-23 21:28:59.000000 yq-3.4.1/test/cfn.yml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      306 2023-10-23 21:28:59.000000 yq-3.4.1/test/doc.yml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-10-23 21:28:59.000000 yq-3.4.1/test/filter.jq
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    15999 2024-04-17 22:09:44.000000 yq-3.4.1/test/test.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:37:50.484325 yq-3.4.1/yq/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    13702 2024-04-17 23:37:06.000000 yq-3.4.1/yq/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:28:58.000000 yq-3.4.1/yq/__main__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3531 2024-04-17 22:10:09.000000 yq-3.4.1/yq/dumper.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8391 2024-04-17 22:13:00.000000 yq-3.4.1/yq/loader.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6212 2023-10-23 21:28:58.000000 yq-3.4.1/yq/parser.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:37:50.488031 yq-3.4.1/yq/tomlq/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:11:04.000000 yq-3.4.1/yq/tomlq/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       63 2024-04-17 23:12:35.000000 yq-3.4.1/yq/tomlq/__main__.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:37:50.488907 yq-3.4.1/yq/xq/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:10:04.000000 yq-3.4.1/yq/xq/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       63 2024-04-17 23:10:50.000000 yq-3.4.1/yq/xq/__main__.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:37:50.489627 yq-3.4.1/yq.egg-info/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8985 2024-04-17 23:37:50.000000 yq-3.4.1/yq.egg-info/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      633 2024-04-17 23:37:50.000000 yq-3.4.1/yq.egg-info/SOURCES.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2024-04-17 23:37:50.000000 yq-3.4.1/yq.egg-info/dependency_links.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       63 2024-04-17 23:37:50.000000 yq-3.4.1/yq.egg-info/entry_points.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      107 2024-04-17 23:37:50.000000 yq-3.4.1/yq.egg-info/requires.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        3 2024-04-17 23:37:50.000000 yq-3.4.1/yq.egg-info/top_level.txt
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-26 17:48:26.526201 yq-3.4.2/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-26 17:48:26.507455 yq-3.4.2/.github/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       18 2023-10-23 21:28:59.000000 yq-3.4.2/.github/FUNDING.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-26 17:48:26.508189 yq-3.4.2/.github/workflows/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      945 2024-04-15 18:14:25.000000 yq-3.4.2/.github/workflows/ci.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      477 2024-04-26 17:36:00.000000 yq-3.4.2/.gitignore
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8528 2024-04-26 17:48:13.000000 yq-3.4.2/Changes.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10273 2023-10-23 21:28:59.000000 yq-3.4.2/LICENSE
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       41 2023-10-23 21:28:59.000000 yq-3.4.2/MANIFEST.in
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      478 2023-10-23 21:28:59.000000 yq-3.4.2/Makefile
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8985 2024-04-26 17:48:26.525583 yq-3.4.2/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7731 2024-04-17 23:14:42.000000 yq-3.4.2/README.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      696 2023-10-23 21:29:01.000000 yq-3.4.2/SECURITY.md
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2542 2024-04-15 18:14:25.000000 yq-3.4.2/common.mk
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-26 17:48:26.512739 yq-3.4.2/docs/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:28:59.000000 yq-3.4.2/docs/changelog.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3515 2024-04-26 17:48:14.000000 yq-3.4.2/docs/cli-doc-tomlq.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3995 2024-04-26 17:48:13.000000 yq-3.4.2/docs/cli-doc-xq.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     4735 2024-04-26 17:48:13.000000 yq-3.4.2/docs/cli-doc.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      806 2023-10-23 21:28:59.000000 yq-3.4.2/docs/conf.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      248 2023-10-23 21:28:59.000000 yq-3.4.2/docs/index.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        8 2023-10-23 21:28:59.000000 yq-3.4.2/docs/toc.html
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      416 2024-04-26 17:36:00.000000 yq-3.4.2/pyproject.toml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       38 2024-04-26 17:48:26.526282 yq-3.4.2/setup.cfg
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1677 2024-04-26 17:48:09.000000 yq-3.4.2/setup.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-26 17:48:26.514663 yq-3.4.2/test/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3468 2023-10-23 21:28:59.000000 yq-3.4.2/test/cfn.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      306 2023-10-23 21:28:59.000000 yq-3.4.2/test/doc.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-10-23 21:28:59.000000 yq-3.4.2/test/filter.jq
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    15999 2024-04-17 22:09:44.000000 yq-3.4.2/test/test.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-26 17:48:26.518940 yq-3.4.2/yq/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    13702 2024-04-26 17:36:00.000000 yq-3.4.2/yq/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:28:58.000000 yq-3.4.2/yq/__main__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3531 2024-04-17 22:10:09.000000 yq-3.4.2/yq/dumper.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8391 2024-04-17 22:13:00.000000 yq-3.4.2/yq/loader.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6212 2023-10-23 21:28:58.000000 yq-3.4.2/yq/parser.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-26 17:48:26.522815 yq-3.4.2/yq/tomlq/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:11:04.000000 yq-3.4.2/yq/tomlq/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       63 2024-04-17 23:12:35.000000 yq-3.4.2/yq/tomlq/__main__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      160 2024-04-26 17:48:26.000000 yq-3.4.2/yq/version.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-26 17:48:26.523737 yq-3.4.2/yq/xq/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-17 23:10:04.000000 yq-3.4.2/yq/xq/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       63 2024-04-17 23:10:50.000000 yq-3.4.2/yq/xq/__main__.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-26 17:48:26.524485 yq-3.4.2/yq.egg-info/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8985 2024-04-26 17:48:26.000000 yq-3.4.2/yq.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      647 2024-04-26 17:48:26.000000 yq-3.4.2/yq.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2024-04-26 17:48:26.000000 yq-3.4.2/yq.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       63 2024-04-26 17:48:26.000000 yq-3.4.2/yq.egg-info/entry_points.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      107 2024-04-26 17:48:26.000000 yq-3.4.2/yq.egg-info/requires.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        3 2024-04-26 17:48:26.000000 yq-3.4.2/yq.egg-info/top_level.txt
```

### Comparing `yq-3.4.1/.github/workflows/ci.yml` & `yq-3.4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/Changes.rst` & `yq-3.4.2/Changes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Changes for v3.4.2 (2024-04-26)
+===============================
+
+Constrain setuptools_scm version
+
 Changes for v3.4.1 (2024-04-17)
 ===============================
 
 -  Add module entry points for xq and tomlq
 
 Changes for v3.4.0 (2024-04-17)
 ===============================
```

### Comparing `yq-3.4.1/LICENSE` & `yq-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/PKG-INFO` & `yq-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yq
-Version: 3.4.1
+Version: 3.4.2
 Summary: Command-line YAML/XML processor - jq wrapper for YAML/XML documents
 Home-page: https://github.com/kislyuk/yq
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `yq-3.4.1/README.rst` & `yq-3.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/SECURITY.md` & `yq-3.4.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/common.mk` & `yq-3.4.2/common.mk`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/docs/cli-doc-tomlq.txt` & `yq-3.4.2/docs/cli-doc-tomlq.txt`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/docs/cli-doc-xq.txt` & `yq-3.4.2/docs/cli-doc-xq.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 usage: xq [options] <jq filter> [input file...]
+          [--version]
           [jq_filter] [files ...]
 
 xq: Command-line XML processor - jq wrapper for XML documents
 
 xq transcodes XML documents to JSON and passes them to jq.
 See https://github.com/kislyuk/xq for more information.
 
 positional arguments:
   jq_filter
   files
 
 options:
   -h, --help            show this help message and exit
   --xml-output, -x      Transcode jq JSON output back into XML and emit it
+  --xml-item-depth 123  Specify depth of items to emit (default 0; use a positive integer to stream large docs)
   --xml-dtd             Preserve XML Document Type Definition (disables streaming of multiple docs)
   --xml-root XML_ROOT   When transcoding back to XML, envelope the output in an element with this name
-  --xml-force-list XML_FORCE_LIST
-                        Tag name to pass to force_list parameter of xmltodict.parse(). Can be used multiple times.
+  --xml-force-list ELT  Emit a list for elements with this name even if they occur only once (option can repeat)
   --in-place, -i        Edit files in place (no backup - use caution)
   --version             show program's version number and exit
 
 jq - commandline JSON processor [version 1.7]
 
 Usage:	jq [options] <jq filter> [file...]
 	jq [options] --args <jq filter> [strings...]
```

### Comparing `yq-3.4.1/docs/cli-doc.txt` & `yq-3.4.2/docs/cli-doc.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 usage: yq [options] <jq filter> [input file...]
-          [--indentless-lists] [--in-place] [--version]
+          [--indentless-lists] [--explicit-start] [--explicit-end]
+          [--in-place] [--version]
           [jq_filter] [files ...]
 
 yq: Command-line YAML processor - jq wrapper for YAML documents
 
 yq transcodes YAML documents to JSON and passes them to jq.
 See https://github.com/kislyuk/yq for more information.
 
@@ -19,14 +20,16 @@
                         Transcode jq JSON output back into YAML and emit it. Preserve YAML tags and styles by representing them as extra items in their enclosing mappings and sequences while in JSON. This option is incompatible with jq filters that do not expect these extra items.
   --yaml-output-grammar-version {1.1,1.2}, --yml-out-ver {1.1,1.2}
                         When using --yaml-output, specify output grammar (the default is 1.1 and will be changed to 1.2 in a future version). Setting this to 1.2 will cause strings like 'on' and 'no' to be emitted unquoted.
   --width WIDTH, -w WIDTH
                         When using --yaml-output, specify string wrap width
   --indentless-lists, --indentless
                         When using --yaml-output, indent block style lists (sequences) with 0 spaces instead of 2
+  --explicit-start      When using --yaml-output, always emit explicit document start ("---")
+  --explicit-end        When using --yaml-output, always emit explicit document end ("...")
   --in-place, -i        Edit files in place (no backup - use caution)
   --version             show program's version number and exit
 
 jq - commandline JSON processor [version 1.7]
 
 Usage:	jq [options] <jq filter> [file...]
 	jq [options] --args <jq filter> [strings...]
```

### Comparing `yq-3.4.1/docs/conf.py` & `yq-3.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/setup.py` & `yq-3.4.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="yq",
-    version="3.4.1",
+    version="3.4.2",
     url="https://github.com/kislyuk/yq",
     license="Apache Software License",
     author="Andrey Kislyuk",
     author_email="kislyuk@gmail.com",
     description="Command-line YAML/XML processor - jq wrapper for YAML/XML documents",
     long_description=open("README.rst").read(),
     python_requires=">=3.6",
     use_scm_version={
         "write_to": "yq/version.py",
     },
-    setup_requires=["setuptools_scm >= 3.4.3"],
+    setup_requires=["setuptools_scm >= 7, <8"],
     install_requires=[
         "PyYAML >= 5.3.1",
         "xmltodict >= 0.11.0",
         "tomlkit >= 0.11.6",
         "argcomplete >= 1.8.1",
     ],
     extras_require={
```

### Comparing `yq-3.4.1/test/cfn.yml` & `yq-3.4.2/test/cfn.yml`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/test/test.py` & `yq-3.4.2/test/test.py`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/yq/__init__.py` & `yq-3.4.2/yq/__init__.py`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/yq/dumper.py` & `yq-3.4.2/yq/dumper.py`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/yq/loader.py` & `yq-3.4.2/yq/loader.py`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/yq/parser.py` & `yq-3.4.2/yq/parser.py`

 * *Files identical despite different names*

### Comparing `yq-3.4.1/yq.egg-info/PKG-INFO` & `yq-3.4.2/yq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yq
-Version: 3.4.1
+Version: 3.4.2
 Summary: Command-line YAML/XML processor - jq wrapper for YAML/XML documents
 Home-page: https://github.com/kislyuk/yq
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `yq-3.4.1/yq.egg-info/SOURCES.txt` & `yq-3.4.2/yq.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 test/filter.jq
 test/test.py
 yq/__init__.py
 yq/__main__.py
 yq/dumper.py
 yq/loader.py
 yq/parser.py
+yq/version.py
 yq.egg-info/PKG-INFO
 yq.egg-info/SOURCES.txt
 yq.egg-info/dependency_links.txt
 yq.egg-info/entry_points.txt
 yq.egg-info/requires.txt
 yq.egg-info/top_level.txt
 yq/tomlq/__init__.py
```

