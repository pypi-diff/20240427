# Comparing `tmp/termux-api-1.2.5.2.tar.gz` & `tmp/termux_api-1.2.5.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termux-api-1.2.5.2.tar", last modified: Mon Jun  5 18:22:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

