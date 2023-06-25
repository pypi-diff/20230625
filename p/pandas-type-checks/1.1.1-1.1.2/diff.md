# Comparing `tmp/pandas-type-checks-1.1.1.tar.gz` & `tmp/pandas_type_checks-1.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-type-checks-1.1.1.tar", last modified: Thu Sep  8 15:08:06 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

