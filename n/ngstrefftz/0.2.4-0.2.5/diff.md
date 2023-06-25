# Comparing `tmp/ngstrefftz-0.2.4-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/ngstrefftz-0.2.5-cp39-cp39-macosx_10_15_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 837254 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx   567608 b- defN 23-Apr-28 13:16 ngstents/_pytents.so
--rw-r--r--  2.0 unx     1688 b- defN 23-Apr-28 13:12 ngstrefftz/__init__.py
--rwxr-xr-x  2.0 unx  2227832 b- defN 23-Apr-28 13:17 ngstrefftz/_trefftz.so
--rw-r--r--  2.0 unx     7650 b- defN 23-Apr-28 13:17 ngstrefftz-0.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      667 b- defN 23-Apr-28 13:17 ngstrefftz-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-28 13:17 ngstrefftz-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-28 13:17 ngstrefftz-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      641 b- defN 23-Apr-28 13:17 ngstrefftz-0.2.4.dist-info/RECORD
-8 files, 2806214 bytes uncompressed, 836148 bytes compressed:  70.2%
+Zip file size: 1385537 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1688 b- defN 23-Jun-25 09:27 ngstrefftz/__init__.py
+-rwxr-xr-x  2.0 unx  1059000 b- defN 23-Jun-25 09:22 ngstrefftz-0.2.5.data/data/ngstents/_pytents.so
+-rw-r--r--  2.0 unx     1688 b- defN 23-Jun-25 09:20 ngstrefftz-0.2.5.data/data/ngstrefftz/__init__.py
+-rwxr-xr-x  2.0 unx  4090056 b- defN 23-Jun-25 09:27 ngstrefftz-0.2.5.data/data/ngstrefftz/_trefftz.so
+-rw-r--r--  2.0 unx     7650 b- defN 23-Jun-25 09:27 ngstrefftz-0.2.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      680 b- defN 23-Jun-25 09:27 ngstrefftz-0.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-25 09:27 ngstrefftz-0.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-25 09:27 ngstrefftz-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      802 b- defN 23-Jun-25 09:27 ngstrefftz-0.2.5.dist-info/RECORD
+9 files, 5161683 bytes uncompressed, 1384149 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
-Filename: ngstents/_pytents.so
+Filename: ngstrefftz/__init__.py
 Comment: 
 
-Filename: ngstrefftz/__init__.py
+Filename: ngstrefftz-0.2.5.data/data/ngstents/_pytents.so
+Comment: 
+
+Filename: ngstrefftz-0.2.5.data/data/ngstrefftz/__init__.py
 Comment: 
 
-Filename: ngstrefftz/_trefftz.so
+Filename: ngstrefftz-0.2.5.data/data/ngstrefftz/_trefftz.so
 Comment: 
 
-Filename: ngstrefftz-0.2.4.dist-info/LICENSE
+Filename: ngstrefftz-0.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: ngstrefftz-0.2.4.dist-info/METADATA
+Filename: ngstrefftz-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: ngstrefftz-0.2.4.dist-info/WHEEL
+Filename: ngstrefftz-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: ngstrefftz-0.2.4.dist-info/top_level.txt
+Filename: ngstrefftz-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ngstrefftz-0.2.4.dist-info/RECORD
+Filename: ngstrefftz-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ngstrefftz-0.2.4.dist-info/LICENSE` & `ngstrefftz-0.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ngstrefftz-0.2.4.dist-info/METADATA` & `ngstrefftz-0.2.5.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.2.4
+Version: 0.2.5
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
-Requires-Python: >=3.8
+License: LGPL2.1
+Platform: UNKNOWN
 License-File: LICENSE
 Requires-Dist: ngsolve (>=6.2.2301)
 
 NGSTrefftz provides a framework to implement Trefftz finite element spaces for NGSolve, with several Trefftz spaces already implemented. Additionally, Trefftz-DG on tent-pitched meshes for the acoustic wave equation is implemented using meshes provided by ngstents. Furthermore, the package includes an implementation of the embedded Trefftz method.
+
```

