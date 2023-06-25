# Comparing `tmp/degex-0.0.22.tar.gz` & `tmp/degex-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degex-0.0.22.tar", last modified: Sun Jun 25 21:16:45 2023, max compression
+gzip compressed data, was "degex-0.0.23.tar", last modified: Sun Jun 25 21:26:38 2023, max compression
```

## Comparing `degex-0.0.22.tar` & `degex-0.0.23.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:16:45.535497 degex-0.0.22/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-03-21 13:23:11.000000 degex-0.0.22/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-03-21 13:23:11.000000 degex-0.0.22/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:16:45.535355 degex-0.0.22/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      291 2023-05-26 15:02:30.000000 degex-0.0.22/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:16:45.534162 degex-0.0.22/degex/
--rw-r--r--   0 solst      (501) staff       (20)       23 2023-06-25 21:16:40.000000 degex-0.0.22/degex/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    18909 2023-06-25 21:16:40.000000 degex-0.0.22/degex/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)    21038 2023-06-25 21:16:40.000000 degex-0.0.22/degex/adata.py
--rw-r--r--   0 solst      (501) staff       (20)    21299 2023-05-26 15:02:24.000000 degex-0.0.22/degex/branches.py
--rw-r--r--   0 solst      (501) staff       (20)      531 2023-06-25 21:16:40.000000 degex-0.0.22/degex/core.py
--rw-r--r--   0 solst      (501) staff       (20)    21040 2023-05-26 15:02:24.000000 degex-0.0.22/degex/granger.py
--rw-r--r--   0 solst      (501) staff       (20)     2850 2023-06-25 21:16:40.000000 degex-0.0.22/degex/plots.py
--rw-r--r--   0 solst      (501) staff       (20)     4892 2023-06-25 21:16:40.000000 degex-0.0.22/degex/preprocessing.py
--rw-r--r--   0 solst      (501) staff       (20)     2601 2023-06-25 21:16:40.000000 degex-0.0.22/degex/static.py
--rw-r--r--   0 solst      (501) staff       (20)     2564 2023-06-25 21:16:40.000000 degex-0.0.22/degex/types.py
--rw-r--r--   0 solst      (501) staff       (20)     2109 2023-06-25 21:16:40.000000 degex-0.0.22/degex/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:16:45.535141 degex-0.0.22/degex.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:16:45.000000 degex-0.0.22/degex.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      438 2023-06-25 21:16:45.000000 degex-0.0.22/degex.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-25 21:16:45.000000 degex-0.0.22/degex.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       32 2023-06-25 21:16:45.000000 degex-0.0.22/degex.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-05-26 15:02:38.000000 degex-0.0.22/degex.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      165 2023-06-25 21:16:45.000000 degex-0.0.22/degex.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        6 2023-06-25 21:16:45.000000 degex-0.0.22/degex.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)     1095 2023-06-25 21:16:25.000000 degex-0.0.22/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-25 21:16:45.535538 degex-0.0.22/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2541 2023-03-21 13:23:12.000000 degex-0.0.22/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:26:38.680722 degex-0.0.23/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-03-21 13:23:11.000000 degex-0.0.23/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-03-21 13:23:11.000000 degex-0.0.23/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:26:38.680577 degex-0.0.23/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      291 2023-05-26 15:02:30.000000 degex-0.0.23/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:26:38.679552 degex-0.0.23/degex/
+-rw-r--r--   0 solst      (501) staff       (20)       23 2023-06-25 21:26:28.000000 degex-0.0.23/degex/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    18909 2023-06-25 21:26:28.000000 degex-0.0.23/degex/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)    21038 2023-06-25 21:26:28.000000 degex-0.0.23/degex/adata.py
+-rw-r--r--   0 solst      (501) staff       (20)    21299 2023-05-26 15:02:24.000000 degex-0.0.23/degex/branches.py
+-rw-r--r--   0 solst      (501) staff       (20)      531 2023-06-25 21:26:28.000000 degex-0.0.23/degex/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    21040 2023-05-26 15:02:24.000000 degex-0.0.23/degex/granger.py
+-rw-r--r--   0 solst      (501) staff       (20)     2850 2023-06-25 21:26:28.000000 degex-0.0.23/degex/plots.py
+-rw-r--r--   0 solst      (501) staff       (20)     4892 2023-06-25 21:26:28.000000 degex-0.0.23/degex/preprocessing.py
+-rw-r--r--   0 solst      (501) staff       (20)     2601 2023-06-25 21:26:28.000000 degex-0.0.23/degex/static.py
+-rw-r--r--   0 solst      (501) staff       (20)     2564 2023-06-25 21:26:28.000000 degex-0.0.23/degex/types.py
+-rw-r--r--   0 solst      (501) staff       (20)     2109 2023-06-25 21:26:28.000000 degex-0.0.23/degex/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:26:38.680400 degex-0.0.23/degex.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      438 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       32 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-05-26 15:02:38.000000 degex-0.0.23/degex.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      165 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        6 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)     1095 2023-06-25 21:26:26.000000 degex-0.0.23/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-25 21:26:38.680760 degex-0.0.23/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2541 2023-03-21 13:23:12.000000 degex-0.0.23/setup.py
```

### Comparing `degex-0.0.22/LICENSE` & `degex-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `degex-0.0.22/PKG-INFO` & `degex-0.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degex
-Version: 0.0.22
+Version: 0.0.23
 Summary: Detect Gene Expression in Single-CEll data
 Home-page: https://github.com/dsm-72/degex
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python single cell detect gene expression spot marker genes
 Classifier: Development Status :: 4 - Beta
```

### Comparing `degex-0.0.22/degex/_modidx.py` & `degex-0.0.23/degex/_modidx.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.22/degex/adata.py` & `degex-0.0.23/degex/adata.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.22/degex/branches.py` & `degex-0.0.23/degex/branches.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.22/degex/core.py` & `degex-0.0.23/degex/core.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.22/degex/granger.py` & `degex-0.0.23/degex/granger.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.22/degex/plots.py` & `degex-0.0.23/degex/plots.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.22/degex/preprocessing.py` & `degex-0.0.23/degex/preprocessing.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.22/degex/static.py` & `degex-0.0.23/degex/static.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.22/degex/types.py` & `degex-0.0.23/degex/types.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.22/degex/utils.py` & `degex-0.0.23/degex/utils.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.22/degex.egg-info/PKG-INFO` & `degex-0.0.23/degex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degex
-Version: 0.0.22
+Version: 0.0.23
 Summary: Detect Gene Expression in Single-CEll data
 Home-page: https://github.com/dsm-72/degex
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python single cell detect gene expression spot marker genes
 Classifier: Development Status :: 4 - Beta
```

### Comparing `degex-0.0.22/settings.ini` & `degex-0.0.23/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = degex
 lib_name = degex
-version = 0.0.22
+version = 0.0.23
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = degex
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `degex-0.0.22/setup.py` & `degex-0.0.23/setup.py`

 * *Files identical despite different names*

