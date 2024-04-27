# Comparing `tmp/TidalPy-0.5.2.tar.gz` & `tmp/TidalPy-0.5.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TidalPy-0.5.2.tar", last modified: Thu Feb 22 21:54:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

