# Comparing `tmp/data_prep_lab-0.1.4.tar.gz` & `tmp/data_prep_lab-0.1.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_lab-0.1.4.tar", last modified: Fri Apr 26 06:47:03 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

