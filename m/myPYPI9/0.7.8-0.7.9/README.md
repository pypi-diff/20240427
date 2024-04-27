# Comparing `tmp/mypypi9-0.7.8.tar.gz` & `tmp/myPYPI9-0.7.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypypi9-0.7.8.tar", last modified: Sat Apr 27 06:21:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

