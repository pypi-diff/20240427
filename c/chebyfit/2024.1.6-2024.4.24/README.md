# Comparing `tmp/chebyfit-2024.1.6.tar.gz` & `tmp/chebyfit-2024.4.24-cp311-cp311-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chebyfit-2024.1.6.tar", last modified: Sun Jan  7 08:31:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

