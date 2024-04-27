# Comparing `tmp/trustllm-0.2.4.tar.gz` & `tmp/trustllm-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustllm-0.2.4.tar", last modified: Mon Feb  5 10:21:01 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

