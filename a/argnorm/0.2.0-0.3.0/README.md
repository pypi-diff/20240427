# Comparing `tmp/argnorm-0.2.0.tar.gz` & `tmp/argnorm-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argnorm-0.2.0.tar", last modified: Tue Mar 26 12:32:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

