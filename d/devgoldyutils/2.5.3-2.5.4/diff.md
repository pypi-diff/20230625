# Comparing `tmp/devgoldyutils-2.5.3.tar.gz` & `tmp/devgoldyutils-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devgoldyutils-2.5.3.tar", last modified: Tue May 30 19:39:44 2023, max compression
+gzip compressed data, was "devgoldyutils-2.5.4.tar", last modified: Sun Jun 25 14:48:15 2023, max compression
```

## Comparing `devgoldyutils-2.5.3.tar` & `devgoldyutils-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 goldy     (1001) goldy     (1001)        0 2023-05-30 19:39:44.594946 devgoldyutils-2.5.3/
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       53 2023-05-14 16:10:00.000000 devgoldyutils-2.5.3/.gitignore
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)    35148 2023-05-14 16:10:00.000000 devgoldyutils-2.5.3/LICENSE
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       32 2023-02-01 17:19:33.000000 devgoldyutils-2.5.3/MANIFEST.in
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       23 2023-05-14 16:10:00.000000 devgoldyutils-2.5.3/Makefile
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)    42017 2023-05-30 19:39:44.593190 devgoldyutils-2.5.3/PKG-INFO
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      440 2023-05-30 19:25:40.000000 devgoldyutils-2.5.3/README.md
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      284 2023-05-30 19:38:13.000000 devgoldyutils-2.5.3/demo.py
-drwxrwxrwx   0 goldy     (1001) goldy     (1001)        0 2023-05-30 19:39:44.573689 devgoldyutils-2.5.3/devgoldyutils/
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      498 2023-05-30 19:36:29.000000 devgoldyutils-2.5.3/devgoldyutils/__init__.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     1497 2023-05-14 19:34:30.000000 devgoldyutils-2.5.3/devgoldyutils/better_get.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     1520 2023-05-14 16:10:00.000000 devgoldyutils-2.5.3/devgoldyutils/colours.py
-drwxrwxrwx   0 goldy     (1001) goldy     (1001)        0 2023-05-30 19:39:44.590429 devgoldyutils-2.5.3/devgoldyutils/console/
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      340 2023-05-14 16:10:00.000000 devgoldyutils-2.5.3/devgoldyutils/console/__init__.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      326 2023-05-14 16:10:00.000000 devgoldyutils-2.5.3/devgoldyutils/console/colours.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     1295 2023-05-14 16:10:00.000000 devgoldyutils-2.5.3/devgoldyutils/console/legacy_colours.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     4376 2023-05-14 16:52:57.000000 devgoldyutils-2.5.3/devgoldyutils/dict_classes.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      382 2023-05-14 16:10:00.000000 devgoldyutils-2.5.3/devgoldyutils/errors.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     1634 2023-05-14 16:52:08.000000 devgoldyutils-2.5.3/devgoldyutils/file_configs.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     1715 2023-05-14 16:10:00.000000 devgoldyutils-2.5.3/devgoldyutils/logging.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      352 2023-05-30 19:38:53.000000 devgoldyutils-2.5.3/devgoldyutils/strings.py
-drwxrwxrwx   0 goldy     (1001) goldy     (1001)        0 2023-05-30 19:39:44.584449 devgoldyutils-2.5.3/devgoldyutils.egg-info/
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)    42017 2023-05-30 19:39:44.000000 devgoldyutils-2.5.3/devgoldyutils.egg-info/PKG-INFO
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      576 2023-05-30 19:39:44.000000 devgoldyutils-2.5.3/devgoldyutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)        1 2023-05-30 19:39:44.000000 devgoldyutils-2.5.3/devgoldyutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       14 2023-05-30 19:39:44.000000 devgoldyutils-2.5.3/devgoldyutils.egg-info/requires.txt
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       14 2023-05-30 19:39:44.000000 devgoldyutils-2.5.3/devgoldyutils.egg-info/top_level.txt
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     1252 2023-05-30 19:39:24.000000 devgoldyutils-2.5.3/pyproject.toml
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       38 2023-05-30 19:39:44.595174 devgoldyutils-2.5.3/setup.cfg
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-06-25 14:48:15.872490 devgoldyutils-2.5.4/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       53 2023-05-14 16:10:00.000000 devgoldyutils-2.5.4/.gitignore
+-rw-r--r--   0 goldy     (1001) goldy     (1001)    35148 2023-05-14 16:10:00.000000 devgoldyutils-2.5.4/LICENSE
+-rwxr-xr-x   0 goldy     (1001) goldy     (1001)       32 2023-02-01 17:19:33.000000 devgoldyutils-2.5.4/MANIFEST.in
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       23 2023-05-14 16:10:00.000000 devgoldyutils-2.5.4/Makefile
+-rw-r--r--   0 goldy     (1001) goldy     (1001)    42040 2023-06-25 14:48:15.871490 devgoldyutils-2.5.4/PKG-INFO
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      440 2023-05-30 19:25:40.000000 devgoldyutils-2.5.4/README.md
+-rwxr-xr-x   0 goldy     (1001) goldy     (1001)      284 2023-06-25 14:44:52.000000 devgoldyutils-2.5.4/demo.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-06-25 14:48:15.870490 devgoldyutils-2.5.4/devgoldyutils/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      746 2023-06-25 14:41:35.000000 devgoldyutils-2.5.4/devgoldyutils/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1497 2023-05-14 19:34:30.000000 devgoldyutils-2.5.4/devgoldyutils/better_get.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1520 2023-05-14 16:10:00.000000 devgoldyutils-2.5.4/devgoldyutils/colours.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-06-25 14:48:15.871490 devgoldyutils-2.5.4/devgoldyutils/console/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      340 2023-05-14 16:10:00.000000 devgoldyutils-2.5.4/devgoldyutils/console/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      326 2023-05-14 16:10:00.000000 devgoldyutils-2.5.4/devgoldyutils/console/colours.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1295 2023-05-14 16:10:00.000000 devgoldyutils-2.5.4/devgoldyutils/console/legacy_colours.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     4376 2023-05-14 16:52:57.000000 devgoldyutils-2.5.4/devgoldyutils/dict_classes.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      382 2023-05-14 16:10:00.000000 devgoldyutils-2.5.4/devgoldyutils/errors.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1634 2023-05-14 16:52:08.000000 devgoldyutils-2.5.4/devgoldyutils/file_configs.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1715 2023-05-14 16:10:00.000000 devgoldyutils-2.5.4/devgoldyutils/logging.py
+-rwxr-xr-x   0 goldy     (1001) goldy     (1001)      352 2023-05-30 19:38:53.000000 devgoldyutils-2.5.4/devgoldyutils/strings.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-06-25 14:48:15.870490 devgoldyutils-2.5.4/devgoldyutils.egg-info/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)    42040 2023-06-25 14:48:15.000000 devgoldyutils-2.5.4/devgoldyutils.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      576 2023-06-25 14:48:15.000000 devgoldyutils-2.5.4/devgoldyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        1 2023-06-25 14:48:15.000000 devgoldyutils-2.5.4/devgoldyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       24 2023-06-25 14:48:15.000000 devgoldyutils-2.5.4/devgoldyutils.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       14 2023-06-25 14:48:15.000000 devgoldyutils-2.5.4/devgoldyutils.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1303 2023-06-25 14:35:58.000000 devgoldyutils-2.5.4/pyproject.toml
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       38 2023-06-25 14:48:15.872490 devgoldyutils-2.5.4/setup.cfg
```

### Comparing `devgoldyutils-2.5.3/LICENSE` & `devgoldyutils-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5.3/PKG-INFO` & `devgoldyutils-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devgoldyutils
-Version: 2.5.3
+Version: 2.5.4
 Summary: My own utils library I use throughout all my python projects.
 Author-email: Goldy <goldy@devgoldy.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,14 +688,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: pprint
 License-File: LICENSE
 
 <div align="center">
 
   # ⚒ devgoldyutils
   
   <sub>My own utils library I use throughout all my python projects.</sub>
```

### Comparing `devgoldyutils-2.5.3/devgoldyutils/better_get.py` & `devgoldyutils-2.5.4/devgoldyutils/better_get.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5.3/devgoldyutils/colours.py` & `devgoldyutils-2.5.4/devgoldyutils/colours.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5.3/devgoldyutils/console/legacy_colours.py` & `devgoldyutils-2.5.4/devgoldyutils/console/legacy_colours.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5.3/devgoldyutils/dict_classes.py` & `devgoldyutils-2.5.4/devgoldyutils/dict_classes.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5.3/devgoldyutils/file_configs.py` & `devgoldyutils-2.5.4/devgoldyutils/file_configs.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5.3/devgoldyutils/logging.py` & `devgoldyutils-2.5.4/devgoldyutils/logging.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5.3/devgoldyutils.egg-info/PKG-INFO` & `devgoldyutils-2.5.4/devgoldyutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devgoldyutils
-Version: 2.5.3
+Version: 2.5.4
 Summary: My own utils library I use throughout all my python projects.
 Author-email: Goldy <goldy@devgoldy.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,14 +688,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: pprint
 License-File: LICENSE
 
 <div align="center">
 
   # ⚒ devgoldyutils
   
   <sub>My own utils library I use throughout all my python projects.</sub>
```

### Comparing `devgoldyutils-2.5.3/devgoldyutils.egg-info/SOURCES.txt` & `devgoldyutils-2.5.4/devgoldyutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5.3/pyproject.toml` & `devgoldyutils-2.5.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -18,18 +18,23 @@
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
 	'Programming Language :: Python :: 3.11'
 ]
 dependencies = [
-    "prettyprinter"
+    
 ]
 
-version = "2.5.3"
+version = "2.5.4"
+
+[project.optional-dependencies]
+pprint = [
+    "prettyprinter"
+]
 
 [project.urls]
 GitHub = "https://github.com/THEGOLDENPRO/devgoldyutils"
 BugTracker = "https://github.com/THEGOLDENPRO/devgoldyutils/issues"
 ChangeLog = "https://github.com/THEGOLDENPRO/devgoldyutils/master/CHANGELOG.md"
 
 [build-system]
```

