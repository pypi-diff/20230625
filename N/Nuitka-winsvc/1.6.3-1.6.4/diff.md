# Comparing `tmp/Nuitka-winsvc-1.6.3.tar.gz` & `tmp/Nuitka_winsvc-1.6.4-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nuitka-winsvc-1.6.3.tar", last modified: Fri Jun 16 02:38:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

