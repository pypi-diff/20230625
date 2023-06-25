# Comparing `tmp/easybio-0.3.2.tar.gz` & `tmp/easybio-0.3.5-py3.10.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybio-0.3.2.tar", last modified: Sun May 14 12:49:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

