# Comparing `tmp/autoremove-torrents-1.5.4.tar.gz` & `tmp/autoremove_torrents-1.5.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\autoremove-torrents-1.5.4.tar", last modified: Sun Jun 19 15:08:44 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

