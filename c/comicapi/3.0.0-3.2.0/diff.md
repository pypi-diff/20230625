# Comparing `tmp/comicapi-3.0.0.tar.gz` & `tmp/comicapi-3.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comicapi-3.0.0.tar", last modified: Sun May 28 08:16:14 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

