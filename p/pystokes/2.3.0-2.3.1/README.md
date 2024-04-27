# Comparing `tmp/pystokes-2.3.0.tar.gz` & `tmp/pystokes-2.3.1-cp310-cp310-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystokes-2.3.0.tar", last modified: Tue Mar 26 13:40:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

