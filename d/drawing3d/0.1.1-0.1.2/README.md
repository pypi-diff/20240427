# Comparing `tmp/drawing3d-0.1.1.tar.gz` & `tmp/drawing3d-0.1.2-cp39-cp39-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drawing3d-0.1.1.tar", last modified: Mon Apr  8 01:18:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

