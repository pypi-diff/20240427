# Comparing `tmp/pyayay-0.1.0a2.tar.gz` & `tmp/pyayay-0.1.1-pp39-pypy39_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyayay-0.1.0a2.tar", last modified: Sat Apr 27 17:23:11 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

