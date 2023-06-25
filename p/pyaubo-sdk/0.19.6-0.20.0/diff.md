# Comparing `tmp/pyaubo_sdk-0.19.6-cp39-cp39-win_amd64.whl.zip` & `tmp/pyaubo_sdk-0.20.0-cp311-cp311-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,7 @@
-Zip file size: 584467 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat  1838592 b- defN 23-Mar-16 08:44 pyaubo_sdk.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      381 b- defN 23-Mar-16 08:44 pyaubo_sdk.cp39-win_amd64.pyd.manifest
--rw-rw-rw-  2.0 fat     2459 b- defN 23-Mar-16 08:44 pyaubo_sdk-0.19.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Mar-16 08:44 pyaubo_sdk-0.19.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Mar-16 08:44 pyaubo_sdk-0.19.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      497 b- defN 23-Mar-16 08:44 pyaubo_sdk-0.19.6.dist-info/RECORD
-6 files, 1842030 bytes uncompressed, 583567 bytes compressed:  68.3%
+Zip file size: 2044447 bytes, number of entries: 5
+-rwxr-xr-x  2.0 unx  5908264 b- defN 23-Jun-25 08:59 pyaubo_sdk.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     2369 b- defN 23-Jun-25 08:59 pyaubo_sdk-0.20.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-25 08:59 pyaubo_sdk-0.20.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-25 08:59 pyaubo_sdk-0.20.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      416 b- defN 23-Jun-25 08:59 pyaubo_sdk-0.20.0.dist-info/RECORD
+5 files, 5911163 bytes uncompressed, 2043673 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,19 +1,16 @@
-Filename: pyaubo_sdk.cp39-win_amd64.pyd
+Filename: pyaubo_sdk.cpython-311-x86_64-linux-gnu.so
 Comment: 
 
-Filename: pyaubo_sdk.cp39-win_amd64.pyd.manifest
+Filename: pyaubo_sdk-0.20.0.dist-info/METADATA
 Comment: 
 
-Filename: pyaubo_sdk-0.19.6.dist-info/METADATA
+Filename: pyaubo_sdk-0.20.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyaubo_sdk-0.19.6.dist-info/WHEEL
+Filename: pyaubo_sdk-0.20.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyaubo_sdk-0.19.6.dist-info/top_level.txt
-Comment: 
-
-Filename: pyaubo_sdk-0.19.6.dist-info/RECORD
+Filename: pyaubo_sdk-0.20.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyaubo_sdk-0.19.6.dist-info/METADATA` & `pyaubo_sdk-0.20.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 Metadata-Version: 2.1
 Name: pyaubo-sdk
-Version: 0.19.6
+Version: 0.20.0
 Summary: A Python interface for controlling aubo robot 
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6, <=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: cmake
-Requires-Dist: Cmake-version (>=3.16) ; extra == 'cmake'
-Provides-Extra: g_
-Requires-Dist: version (>=7.x.x) ; extra == 'g_'
 
 <div align="center">
   <h1 align="center">aubo_sdk</h1>
   <h3 align="center">
     ARCS controller software secondary development interface
   </h3>
 </div>
@@ -54,23 +47,22 @@
 If you only want to the use the Python interface, you can install pyaubo_sdk through pip:
 
 ```bash
 pip3 install pyaubo_sdk
 ```
 
 ### Prebuilt python wheels support matrix: ###
-|                | Python3.7 | Python3.8 | Python3.9 | Python3.10 |
-| :------------: | :-------: | :-------: | :-------: | :--------: |
-|   linux x64    |     ✅     |     ✅     |     ✅     |     ✅      |
-| windows 64 bit |           |           |     ✅     |     ✅      |
+|                | Python3.6 | Python3.7 | Python3.8 | Python3.9 | Python3.10 | Python3.11 |
+| :------------: | :-------: | :-------: | :-------: | :-------: | :--------: | :--------: |
+|   linux x64    |     ✅     |     ✅     |     ✅     |     ✅     |     ✅      |     ✅      |
+| windows 64 bit |     ✅     |     ✅     |     ✅     |     ✅     |     ✅      |     ✅      |
 
 ### Dependencies ###
 *  If you're running Linux , you may need to install gcc-7/g++-7
 *  If you're running windows , you may need to install visual studio 2019 or later
 
 ### Compatible Operating Systems ###
 Currently tested on:
 
 *  Ubuntu 16.04 
 *  Debian 10 (Buster)
 *  Windows 10  x64
-
```

