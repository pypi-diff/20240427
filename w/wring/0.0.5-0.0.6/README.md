# Comparing `tmp/wring-0.0.5.tar.gz` & `tmp/wring-0.0.6.tar.gz`

## Comparing `wring-0.0.5.tar` & `wring-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 wring-0.0.5/mkdocs.yml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/_app.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/_version.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/csv.py
--rw-r--r--   0        0        0    26143 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/omx.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/py.typed
--rw-r--r--   0        0        0     8906 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/tar_zst.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 wring-0.0.5/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 wring-0.0.5/LICENSE
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 wring-0.0.5/README.md
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 wring-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 wring-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 wring-0.0.6/mkdocs.yml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 wring-0.0.6/src/wring/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 wring-0.0.6/src/wring/_app.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wring-0.0.6/src/wring/_version.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 wring-0.0.6/src/wring/csv.py
+-rw-r--r--   0        0        0    26143 2020-02-02 00:00:00.000000 wring-0.0.6/src/wring/omx.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wring-0.0.6/src/wring/py.typed
+-rw-r--r--   0        0        0    10095 2020-02-02 00:00:00.000000 wring-0.0.6/src/wring/tar_zst.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 wring-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 wring-0.0.6/LICENSE
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 wring-0.0.6/README.md
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 wring-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 wring-0.0.6/PKG-INFO
```

### Comparing `wring-0.0.5/mkdocs.yml` & `wring-0.0.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `wring-0.0.5/src/wring/csv.py` & `wring-0.0.6/src/wring/csv.py`

 * *Files identical despite different names*

### Comparing `wring-0.0.5/src/wring/omx.py` & `wring-0.0.6/src/wring/omx.py`

 * *Files identical despite different names*

### Comparing `wring-0.0.5/src/wring/tar_zst.py` & `wring-0.0.6/src/wring/tar_zst.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # based on https://gist.github.com/scivision/ad241e9cf0474e267240e196d7545eca
 
 import os
 import tarfile
 import tempfile
+import time
 from pathlib import Path
 from typing import Optional
 
 import typer
 import zstandard
 from rich import console, print
 
@@ -22,14 +23,15 @@
     ----------
     archive: pathlib.Path or str
       .zst file to extract
     out_path: pathlib.Path or str
       directory to extract files and directories to
     """
     c = console.Console()
+    t = time.time()
 
     if zstandard is None:
         raise ImportError("pip install zstandard")
 
     archive = Path(archive).expanduser()
     out_path = Path(out_path).expanduser().resolve()
     # need .resolve() in case intermediate relative dir doesn't exist
@@ -41,41 +43,63 @@
         with c.status("decompressing..."):
             with tempfile.TemporaryFile(suffix=".tar") as ofh:
                 with archive.open("rb") as ifh:
                     dctx.copy_stream(ifh, ofh)
                 ofh.seek(0)
                 with tarfile.open(fileobj=ofh) as z:
                     z.extractall(out_path)
-        c.print(f"extracted to {out_path}")
+        c.print(f"extracted to {out_path} in {time.time() - t:.1f} seconds")
         return
 
     if archive.suffix == ".part000":
         archive_part0 = archive
     else:
         archive_part0 = archive.with_name(archive.name + ".part000")
 
     if archive_part0.exists():
-        c.print(f"extracting from {archive}")
-        with c.status("decompressing multipart tar") as s:
-            dobj = dctx.decompressobj()
-            n = 0
-            with tempfile.TemporaryFile(suffix=".tar") as ofh:
+        c.print(f"extracting from {archive.with_suffix('')}")
+        try:
+            from split_file_reader import SplitFileReader
+        except ImportError:
+            with c.status("decompressing multipart tar") as s:
+                dobj = dctx.decompressobj()
+                n = 0
+                with tempfile.TemporaryFile(suffix=".tar") as ofh:
+                    while archive_part0.with_suffix(f".part{n:03}").exists():
+                        with archive_part0.with_suffix(f".part{n:03}").open(
+                            "rb"
+                        ) as ifh:
+                            s.update(f"reading part{n:03}")
+                            blob = dobj.decompress(ifh.read())
+                            s.update(f"writing part{n:03} to temp.tar")
+                            ofh.write(blob)
+                        n += 1
+                    s.update(f"extracting from temp.tar to {out_path}")
+                    ofh.seek(0)
+                    with tarfile.open(fileobj=ofh) as z:
+                        z.extractall(out_path)
+            c.print(f"extracted to {out_path} in {time.time() - t:.1f} seconds")
+            return
+        else:
+            with c.status("decompressing multipart tar via split-file-reader") as s:
+                filepaths = []
+                n = 0
                 while archive_part0.with_suffix(f".part{n:03}").exists():
-                    with archive_part0.with_suffix(f".part{n:03}").open("rb") as ifh:
-                        s.update(f"reading part{n:03}")
-                        blob = dobj.decompress(ifh.read())
-                        s.update(f"writing part{n:03} to temp.tar")
-                        ofh.write(blob)
+                    filepaths.append(
+                        archive_part0.with_suffix(f".part{n:03}").resolve()
+                    )
                     n += 1
-                s.update(f"extracting from temp.tar to {out_path}")
-                ofh.seek(0)
-                with tarfile.open(fileobj=ofh) as z:
-                    z.extractall(out_path)
-        c.print(f"extracted to {out_path}")
-        return
+                with SplitFileReader(filepaths) as sfr:
+                    with dctx.stream_reader(sfr) as z:
+                        with tarfile.open(fileobj=z, mode="r:") as tarf:
+                            for member in tarf:
+                                s.update(f"extracting {member.name}")
+                                tarf.extract(member, out_path)
+            c.print(f"extracted to {out_path} in {time.time() - t:.1f} seconds")
+            return
     raise FileNotFoundError(archive)
 
 
 def compress_zst(in_path: Path, archive: Path):
     """
     Compress a directory into a .tar.zst file.
```

### Comparing `wring-0.0.5/.gitignore` & `wring-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `wring-0.0.5/LICENSE` & `wring-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wring-0.0.5/pyproject.toml` & `wring-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "pyarrow",
   "rich",
+  "split-file-reader",
   "typer",
   "zstandard",
 ]
 description = "A tool to compress multiple CSV data files into parquet"
 dynamic = ["version"]
 keywords = []
 license = "MIT"
```

### Comparing `wring-0.0.5/PKG-INFO` & `wring-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wring
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool to compress multiple CSV data files into parquet
 Project-URL: Documentation, https://jpn--.github.io/wring
 Project-URL: Issues, https://github.com/jpn--/wring/issues
 Project-URL: Source, https://github.com/jpn--/wring
 Author: Jeff Newman
 License-Expression: MIT
 License-File: LICENSE
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: pyarrow
 Requires-Dist: rich
+Requires-Dist: split-file-reader
 Requires-Dist: typer
 Requires-Dist: zstandard
 Provides-Extra: docs
 Requires-Dist: mkdocs-click; extra == 'docs'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin~=1.1.0; extra == 'docs'
 Requires-Dist: mkdocs-material~=8.5.4; extra == 'docs'
 Requires-Dist: mkdocs-typer; extra == 'docs'
```

