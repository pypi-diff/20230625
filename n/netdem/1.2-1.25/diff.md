# Comparing `tmp/netdem-1.2-cp38-cp38-manylinux2014_aarch64.whl.zip` & `tmp/netdem-1.25-cp311-cp311-macosx_13_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,21 @@
-Zip file size: 3962920 bytes, number of entries: 6
--rw-rw-r--  2.0 unx       23 b- defN 23-Jun-22 14:31 netdem/__init__.py
--rw-r--r--  2.0 unx 12730776 b- defN 23-Jun-23 15:26 netdem/pynetdem.cpython-38-aarch64-linux-gnu.so
--rw-rw-r--  2.0 unx     1428 b- defN 23-Jun-25 01:39 netdem-1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx      112 b- defN 23-Jun-25 01:39 netdem-1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-25 01:39 netdem-1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      467 b- defN 23-Jun-25 01:39 netdem-1.2.dist-info/RECORD
-6 files, 12732813 bytes uncompressed, 3962080 bytes compressed:  68.9%
+Zip file size: 7846874 bytes, number of entries: 19
+-rw-rw-r--  2.0 unx     1688 b- defN 23-Jun-25 07:42 netdem-1.25.dist-info/RECORD
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-24 23:41 netdem-1.25.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-24 23:41 netdem-1.25.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     1429 b- defN 23-Jun-24 23:41 netdem-1.25.dist-info/METADATA
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-05 13:16 netdem/__init__.py
+-rwxr-xr-x  2.0 unx 11551856 b- defN 23-Jun-25 07:42 netdem/pynetdem.cpython-311-darwin.so
+-rw-r--r--  2.0 unx   592160 b- defN 23-Jun-25 07:42 netdem/.dylibs/libopen-pal.40.dylib
+-rw-r--r--  2.0 unx   314256 b- defN 23-Jun-25 07:42 netdem/.dylibs/libhwloc.15.dylib
+-rw-r--r--  2.0 unx    53344 b- defN 23-Jun-25 07:42 netdem/.dylibs/libevent_pthreads-2.1.7.dylib
+-rwxr-xr-x  2.0 unx  5596304 b- defN 23-Jun-25 07:42 netdem/.dylibs/Python
+-rw-r--r--  2.0 unx  1857504 b- defN 23-Jun-25 07:42 netdem/.dylibs/libgfortran.5.dylib
+-r--r--r--  2.0 unx   290416 b- defN 23-Jun-25 07:42 netdem/.dylibs/libboost_math_tr1-mt.dylib
+-rw-r--r--  2.0 unx  1218160 b- defN 23-Jun-25 07:42 netdem/.dylibs/libmpi.40.dylib
+-rw-r--r--  2.0 unx   351488 b- defN 23-Jun-25 07:42 netdem/.dylibs/libquadmath.0.dylib
+-rw-r--r--  2.0 unx   160224 b- defN 23-Jun-25 07:42 netdem/.dylibs/libgcc_s.1.1.dylib
+-r--r--r--  2.0 unx   718544 b- defN 23-Jun-25 07:42 netdem/.dylibs/libopen-rte.40.dylib
+-r--r--r--  2.0 unx   452320 b- defN 23-Jun-25 07:42 netdem/.dylibs/libgmp.10.dylib
+-r--r--r--  2.0 unx   469776 b- defN 23-Jun-25 07:42 netdem/.dylibs/libmpfr.6.dylib
+-r--r--r--  2.0 unx   203648 b- defN 23-Jun-25 07:42 netdem/.dylibs/libevent_core-2.1.7.dylib
+19 files, 23833257 bytes uncompressed, 7844180 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,19 +1,58 @@
+Filename: netdem-1.25.dist-info/RECORD
+Comment: 
+
+Filename: netdem-1.25.dist-info/WHEEL
+Comment: 
+
+Filename: netdem-1.25.dist-info/top_level.txt
+Comment: 
+
+Filename: netdem-1.25.dist-info/METADATA
+Comment: 
+
 Filename: netdem/__init__.py
 Comment: 
 
-Filename: netdem/pynetdem.cpython-38-aarch64-linux-gnu.so
+Filename: netdem/pynetdem.cpython-311-darwin.so
+Comment: 
+
+Filename: netdem/.dylibs/libopen-pal.40.dylib
+Comment: 
+
+Filename: netdem/.dylibs/libhwloc.15.dylib
+Comment: 
+
+Filename: netdem/.dylibs/libevent_pthreads-2.1.7.dylib
+Comment: 
+
+Filename: netdem/.dylibs/Python
+Comment: 
+
+Filename: netdem/.dylibs/libgfortran.5.dylib
+Comment: 
+
+Filename: netdem/.dylibs/libboost_math_tr1-mt.dylib
+Comment: 
+
+Filename: netdem/.dylibs/libmpi.40.dylib
+Comment: 
+
+Filename: netdem/.dylibs/libquadmath.0.dylib
+Comment: 
+
+Filename: netdem/.dylibs/libgcc_s.1.1.dylib
 Comment: 
 
-Filename: netdem-1.2.dist-info/METADATA
+Filename: netdem/.dylibs/libopen-rte.40.dylib
 Comment: 
 
-Filename: netdem-1.2.dist-info/WHEEL
+Filename: netdem/.dylibs/libgmp.10.dylib
 Comment: 
 
-Filename: netdem-1.2.dist-info/top_level.txt
+Filename: netdem/.dylibs/libmpfr.6.dylib
 Comment: 
 
-Filename: netdem-1.2.dist-info/RECORD
+Filename: netdem/.dylibs/libevent_core-2.1.7.dylib
 Comment: 
 
 Zip file comment:
```

## Comparing `netdem-1.2.dist-info/METADATA` & `netdem-1.25.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netdem
-Version: 1.2
+Version: 1.25
 Summary: A neural network machine learning enabled DEM framework for computational particle mechanics.
 Home-page: https://apaam.github.io/netdem_docs/
 Author: APAAM
 Author-email: lai.zhengshou@outlook.com
 Description-Content-Type: text/markdown
 
 # NetDEM
```

