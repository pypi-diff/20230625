# Comparing `tmp/xia_gpt-0.1.0-cp311-none-macosx_11_0_x86_64.whl.zip` & `tmp/xia_gpt-0.1.1-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 88563 bytes, number of entries: 7
--rw-r--r--  2.0 unx       76 b- defN 23-Jun-25 20:30 xia_gpt/__init__.py
--rw-r--r--  2.0 unx   254672 b- defN 23-Jun-25 20:31 xia_gpt/gpt.cpython-311-darwin.so
--rw-r--r--  2.0 unx      151 b- defN 23-Jun-25 20:31 xia_gpt-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      563 b- defN 23-Jun-25 20:31 xia_gpt-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      109 b- defN 23-Jun-25 20:31 xia_gpt-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-25 20:31 xia_gpt-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      554 b- defN 23-Jun-25 20:31 xia_gpt-0.1.0.dist-info/RECORD
-7 files, 256133 bytes uncompressed, 87579 bytes compressed:  65.8%
+Zip file size: 75385 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-25 20:32 xia_gpt/__init__.py
+-rw-r--r--  2.0 unx   201544 b- defN 23-Jun-25 20:33 xia_gpt/gpt.cpython-39-darwin.so
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-25 20:33 xia_gpt-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      600 b- defN 23-Jun-25 20:33 xia_gpt-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-25 20:33 xia_gpt-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-25 20:33 xia_gpt-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      553 b- defN 23-Jun-25 20:33 xia_gpt-0.1.1.dist-info/RECORD
+7 files, 203040 bytes uncompressed, 74403 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_gpt/__init__.py
 Comment: 
 
-Filename: xia_gpt/gpt.cpython-311-darwin.so
+Filename: xia_gpt/gpt.cpython-39-darwin.so
 Comment: 
 
-Filename: xia_gpt-0.1.0.dist-info/LICENSE.txt
+Filename: xia_gpt-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_gpt-0.1.0.dist-info/METADATA
+Filename: xia_gpt-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_gpt-0.1.0.dist-info/WHEEL
+Filename: xia_gpt-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_gpt-0.1.0.dist-info/top_level.txt
+Filename: xia_gpt-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_gpt-0.1.0.dist-info/RECORD
+Filename: xia_gpt-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_gpt/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_gpt.gpt import Gpt
 
 __all__ = [
     "Gpt"
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

