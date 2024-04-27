# Comparing `tmp/autodoc_pydantic-2.1.0.tar.gz` & `tmp/autodoc_pydantic-2.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodoc_pydantic-2.1.0.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

