# Comparing `tmp/yter-3.1.0.tar.gz` & `tmp/yter-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yter-3.1.0.tar", last modified: Sun Jun 25 06:08:50 2023, max compression
+gzip compressed data, was "yter-3.1.1.tar", last modified: Sun Jun 25 06:14:17 2023, max compression
```

## Comparing `yter-3.1.0.tar` & `yter-3.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 06:08:50.558651 yter-3.1.0/
--rw-rw-rw-   0        0        0     1081 2023-03-09 15:02:41.000000 yter-3.1.0/LICENSE
--rw-rw-rw-   0        0        0       18 2023-03-09 15:02:41.000000 yter-3.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2566 2023-06-25 06:08:50.557642 yter-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1920 2023-06-25 05:48:44.000000 yter-3.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 06:08:50.558651 yter-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0      926 2023-03-09 15:02:41.000000 yter-3.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:08:50.497688 yter-3.1.0/test/
--rw-rw-rw-   0        0        0     3893 2023-05-29 14:39:48.000000 yter-3.1.0/test/test_fun.py
--rw-rw-rw-   0        0        0     1287 2023-06-14 05:23:52.000000 yter-3.1.0/test/test_key.py
--rw-rw-rw-   0        0        0      158 2023-03-09 15:02:41.000000 yter-3.1.0/test/test_star.py
--rw-rw-rw-   0        0        0     2406 2023-06-25 06:01:16.000000 yter-3.1.0/test/test_ytr.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:08:50.538052 yter-3.1.0/yter/
--rw-rw-rw-   0        0        0      434 2023-06-25 06:06:04.000000 yter-3.1.0/yter/__init__.py
--rw-rw-rw-   0        0        0    11952 2023-06-22 02:44:16.000000 yter-3.1.0/yter/_fun.py
--rw-rw-rw-   0        0        0     4846 2023-06-25 06:04:23.000000 yter-3.1.0/yter/_key.py
--rw-rw-rw-   0        0        0     8539 2023-06-25 05:53:26.000000 yter-3.1.0/yter/_ytr.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:08:50.555649 yter-3.1.0/yter.egg-info/
--rw-rw-rw-   0        0        0     2566 2023-06-25 06:08:50.000000 yter-3.1.0/yter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-25 06:08:50.000000 yter-3.1.0/yter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 06:08:50.000000 yter-3.1.0/yter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-25 06:08:50.000000 yter-3.1.0/yter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 15:10:32.000000 yter-3.1.0/yter.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-25 06:14:17.437763 yter-3.1.1/
+-rw-rw-rw-   0        0        0     1081 2023-03-09 15:02:41.000000 yter-3.1.1/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-03-09 15:02:41.000000 yter-3.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2566 2023-06-25 06:14:17.437763 yter-3.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1920 2023-06-25 06:12:57.000000 yter-3.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 06:14:17.437763 yter-3.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      926 2023-03-09 15:02:41.000000 yter-3.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:14:17.415844 yter-3.1.1/test/
+-rw-rw-rw-   0        0        0     3893 2023-05-29 14:39:48.000000 yter-3.1.1/test/test_fun.py
+-rw-rw-rw-   0        0        0     1287 2023-06-14 05:23:52.000000 yter-3.1.1/test/test_key.py
+-rw-rw-rw-   0        0        0      158 2023-03-09 15:02:41.000000 yter-3.1.1/test/test_star.py
+-rw-rw-rw-   0        0        0     2406 2023-06-25 06:01:16.000000 yter-3.1.1/test/test_ytr.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:14:17.420352 yter-3.1.1/yter/
+-rw-rw-rw-   0        0        0      434 2023-06-25 06:06:04.000000 yter-3.1.1/yter/__init__.py
+-rw-rw-rw-   0        0        0    11952 2023-06-22 02:44:16.000000 yter-3.1.1/yter/_fun.py
+-rw-rw-rw-   0        0        0     4846 2023-06-25 06:04:23.000000 yter-3.1.1/yter/_key.py
+-rw-rw-rw-   0        0        0     8539 2023-06-25 05:53:26.000000 yter-3.1.1/yter/_ytr.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:14:17.436756 yter-3.1.1/yter.egg-info/
+-rw-rw-rw-   0        0        0     2566 2023-06-25 06:14:17.000000 yter-3.1.1/yter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-25 06:14:17.000000 yter-3.1.1/yter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 06:14:17.000000 yter-3.1.1/yter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-25 06:14:17.000000 yter-3.1.1/yter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 15:10:32.000000 yter-3.1.1/yter.egg-info/zip-safe
```

### Comparing `yter-3.1.0/LICENSE` & `yter-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yter-3.1.0/PKG-INFO` & `yter-3.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yter
-Version: 3.1.0
+Version: 3.1.1
 Summary: Clever, quick iterators that make your smile whiter
 Home-page: https://gitlab.com/shredwheat/yter
 Author: Peter Shinners
 Author-email: pete@shinners.org
 License: MIT
 Keywords: iterator itertools
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 # yter
 
-Version 3.1.0
+Version 3.1.1
 2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
 This will work with versions of Python 2.6+ and 3.2+.
```

### Comparing `yter-3.1.0/README.md` & `yter-3.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # yter
 
-Version 3.1.0
+Version 3.1.1
 2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
 This will work with versions of Python 2.6+ and 3.2+.
```

### Comparing `yter-3.1.0/setup.py` & `yter-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `yter-3.1.0/test/test_fun.py` & `yter-3.1.1/test/test_fun.py`

 * *Files identical despite different names*

### Comparing `yter-3.1.0/test/test_key.py` & `yter-3.1.1/test/test_key.py`

 * *Files identical despite different names*

### Comparing `yter-3.1.0/test/test_ytr.py` & `yter-3.1.1/test/test_ytr.py`

 * *Files identical despite different names*

### Comparing `yter-3.1.0/yter/_fun.py` & `yter-3.1.1/yter/_fun.py`

 * *Files identical despite different names*

### Comparing `yter-3.1.0/yter/_key.py` & `yter-3.1.1/yter/_key.py`

 * *Files identical despite different names*

### Comparing `yter-3.1.0/yter/_ytr.py` & `yter-3.1.1/yter/_ytr.py`

 * *Files identical despite different names*

### Comparing `yter-3.1.0/yter.egg-info/PKG-INFO` & `yter-3.1.1/yter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yter
-Version: 3.1.0
+Version: 3.1.1
 Summary: Clever, quick iterators that make your smile whiter
 Home-page: https://gitlab.com/shredwheat/yter
 Author: Peter Shinners
 Author-email: pete@shinners.org
 License: MIT
 Keywords: iterator itertools
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 # yter
 
-Version 3.1.0
+Version 3.1.1
 2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
 This will work with versions of Python 2.6+ and 3.2+.
```

