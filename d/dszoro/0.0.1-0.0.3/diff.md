# Comparing `tmp/dszoro-0.0.1.tar.gz` & `tmp/dszoro-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dszoro-0.0.1.tar", last modified: Sat Jun 24 13:39:36 2023, max compression
+gzip compressed data, was "dszoro-0.0.3.tar", last modified: Sun Jun 25 07:28:05 2023, max compression
```

## Comparing `dszoro-0.0.1.tar` & `dszoro-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 13:39:36.703391 dszoro-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-06-24 13:21:48.000000 dszoro-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3331 2023-06-24 13:39:36.703391 dszoro-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2883 2023-06-24 13:28:53.000000 dszoro-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-06-24 13:24:03.000000 dszoro-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      590 2023-06-24 13:39:36.706216 dszoro-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-24 13:39:36.673548 dszoro-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-24 13:39:36.698274 dszoro-0.0.1/src/dszoro.egg-info/
--rw-rw-rw-   0        0        0     3331 2023-06-24 13:39:36.000000 dszoro-0.0.1/src/dszoro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-06-24 13:39:36.000000 dszoro-0.0.1/src/dszoro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 13:39:36.000000 dszoro-0.0.1/src/dszoro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-24 13:39:36.000000 dszoro-0.0.1/src/dszoro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-24 13:39:36.702281 dszoro-0.0.1/src/mypackage/
--rw-rw-rw-   0        0        0        0 2023-06-24 13:22:36.000000 dszoro-0.0.1/src/mypackage/__init__.py
--rw-rw-rw-   0        0        0     5370 2023-06-24 13:38:22.000000 dszoro-0.0.1/src/mypackage/main.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:28:05.847593 dszoro-0.0.3/
+-rw-rw-rw-   0        0        0     5370 2023-06-25 07:27:21.000000 dszoro-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3331 2023-06-25 07:28:05.847593 dszoro-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2883 2023-06-24 13:28:53.000000 dszoro-0.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-24 13:24:03.000000 dszoro-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      590 2023-06-25 07:28:05.851137 dszoro-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 07:28:05.801086 dszoro-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 07:28:05.840530 dszoro-0.0.3/src/dszoro.egg-info/
+-rw-rw-rw-   0        0        0     3331 2023-06-25 07:28:05.000000 dszoro-0.0.3/src/dszoro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-25 07:28:05.000000 dszoro-0.0.3/src/dszoro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 07:28:05.000000 dszoro-0.0.3/src/dszoro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-25 07:28:05.000000 dszoro-0.0.3/src/dszoro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 07:28:05.845403 dszoro-0.0.3/src/mypackage/
+-rw-rw-rw-   0        0        0        0 2023-06-24 13:22:36.000000 dszoro-0.0.3/src/mypackage/__init__.py
+-rw-rw-rw-   0        0        0     5370 2023-06-24 13:38:22.000000 dszoro-0.0.3/src/mypackage/hello.py
```

### Comparing `dszoro-0.0.1/PKG-INFO` & `dszoro-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dszoro
-Version: 0.0.1
+Version: 0.0.3
 Summary: A small example package
 Author: Zoro
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dszoro-0.0.1/README.md` & `dszoro-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dszoro-0.0.1/setup.cfg` & `dszoro-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 737a 6f72 6f0d 0a76 6572 7369   = dszoro..versi
-00000020: 6f6e 203d 2030 2e30 2e31 0d0a 6175 7468  on = 0.0.1..auth
+00000020: 6f6e 203d 2030 2e30 2e33 0d0a 6175 7468  on = 0.0.3..auth
 00000030: 6f72 203d 205a 6f72 6f0d 0a61 7574 686f  or = Zoro..autho
 00000040: 725f 656d 6169 6c20 3d20 6175 7468 6f72  r_email = author
 00000050: 4065 7861 6d70 6c65 2e63 6f6d 0d0a 6465  @example.com..de
 00000060: 7363 7269 7074 696f 6e20 3d20 4120 736d  scription = A sm
 00000070: 616c 6c20 6578 616d 706c 6520 7061 636b  all example pack
 00000080: 6167 650d 0a6c 6f6e 675f 6465 7363 7269  age..long_descri
 00000090: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
```

### Comparing `dszoro-0.0.1/src/dszoro.egg-info/PKG-INFO` & `dszoro-0.0.3/src/dszoro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dszoro
-Version: 0.0.1
+Version: 0.0.3
 Summary: A small example package
 Author: Zoro
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dszoro-0.0.1/src/mypackage/main.py` & `dszoro-0.0.3/LICENSE`

 * *Files identical despite different names*

