# Comparing `tmp/PyNyaaTa-202306252027.tar.gz` & `tmp/PyNyaaTa-202306252028-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNyaaTa-202306252027.tar", last modified: Sun Jun 25 20:27:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

