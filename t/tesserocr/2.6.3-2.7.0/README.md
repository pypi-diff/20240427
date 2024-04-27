# Comparing `tmp/tesserocr-2.6.3.tar.gz` & `tmp/tesserocr-2.7.0-cp311-cp311-manylinux_2_28_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesserocr-2.6.3.tar", last modified: Thu Mar 28 16:57:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

