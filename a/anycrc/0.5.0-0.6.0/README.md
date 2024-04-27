# Comparing `tmp/anycrc-0.5.0.tar.gz` & `tmp/anycrc-0.6.0-cp311-cp311-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.5.0.tar", last modified: Fri Apr 26 01:16:21 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

