# Comparing `tmp/ogms-0.1.2-py3.7.egg` & `tmp/ogms-0.1.4-py3.7.egg`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1203 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      786 b- defN 23-Jun-21 16:56 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat      170 b- defN 23-Jun-21 16:56 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-21 16:56 EGG-INFO/dependency_links.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-21 16:56 EGG-INFO/requires.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-21 16:56 EGG-INFO/top_level.txt
+Zip file size: 1214 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      786 b- defN 23-Jun-25 11:31 EGG-INFO/PKG-INFO
+-rw-rw-rw-  2.0 fat      180 b- defN 23-Jun-25 11:31 EGG-INFO/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-25 11:31 EGG-INFO/dependency_links.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-25 11:31 EGG-INFO/requires.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-25 11:31 EGG-INFO/top_level.txt
 -rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-21 16:56 EGG-INFO/zip-safe
-6 files, 977 bytes uncompressed, 473 bytes compressed:  51.6%
+6 files, 987 bytes uncompressed, 484 bytes compressed:  51.0%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ogms
-Version: 0.1.2
+Version: 0.1.4
 Summary: Python Framework
 Home-page: UNKNOWN
 Author: Fengyuan Zhang
 Author-email: franklinzhang@foxmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

## EGG-INFO/SOURCES.txt

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 ogms.egg-info/PKG-INFO
 ogms.egg-info/SOURCES.txt
 ogms.egg-info/dependency_links.txt
 ogms.egg-info/requires.txt
 ogms.egg-info/top_level.txt
 ogms.egg-info/zip-safe
```

