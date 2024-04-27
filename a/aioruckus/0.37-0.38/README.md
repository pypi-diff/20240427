# Comparing `tmp/aioruckus-0.37.tar.gz` & `tmp/aioruckus-0.38-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioruckus-0.37.tar", last modified: Sun Dec 17 03:31:54 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

