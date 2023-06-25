# Comparing `tmp/degex-0.0.19.tar.gz` & `tmp/degex-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degex-0.0.19.tar", last modified: Sun Jun 25 21:04:28 2023, max compression
+gzip compressed data, was "degex-0.0.20.tar", last modified: Sun Jun 25 21:09:33 2023, max compression
```

## Comparing `degex-0.0.19.tar` & `degex-0.0.20.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:04:28.102074 degex-0.0.19/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-03-21 13:23:11.000000 degex-0.0.19/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-03-21 13:23:11.000000 degex-0.0.19/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:04:28.101938 degex-0.0.19/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      291 2023-05-26 15:02:30.000000 degex-0.0.19/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:04:28.100643 degex-0.0.19/degex/
--rw-r--r--   0 solst      (501) staff       (20)       23 2023-06-25 21:04:22.000000 degex-0.0.19/degex/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    18909 2023-06-25 21:04:22.000000 degex-0.0.19/degex/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)    21053 2023-06-25 21:04:22.000000 degex-0.0.19/degex/adata.py
--rw-r--r--   0 solst      (501) staff       (20)    21299 2023-05-26 15:02:24.000000 degex-0.0.19/degex/branches.py
--rw-r--r--   0 solst      (501) staff       (20)      531 2023-06-25 21:04:22.000000 degex-0.0.19/degex/core.py
--rw-r--r--   0 solst      (501) staff       (20)    21040 2023-05-26 15:02:24.000000 degex-0.0.19/degex/granger.py
--rw-r--r--   0 solst      (501) staff       (20)     2850 2023-06-25 21:04:22.000000 degex-0.0.19/degex/plots.py
--rw-r--r--   0 solst      (501) staff       (20)     4892 2023-06-25 21:04:22.000000 degex-0.0.19/degex/preprocessing.py
--rw-r--r--   0 solst      (501) staff       (20)     2601 2023-06-25 21:04:22.000000 degex-0.0.19/degex/static.py
--rw-r--r--   0 solst      (501) staff       (20)     2564 2023-06-25 21:04:22.000000 degex-0.0.19/degex/types.py
--rw-r--r--   0 solst      (501) staff       (20)     2109 2023-06-25 21:04:22.000000 degex-0.0.19/degex/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:04:28.101754 degex-0.0.19/degex.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      438 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       32 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-05-26 15:02:38.000000 degex-0.0.19/degex.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      165 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        6 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)     1095 2023-06-25 21:04:20.000000 degex-0.0.19/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-25 21:04:28.102114 degex-0.0.19/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2541 2023-03-21 13:23:12.000000 degex-0.0.19/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:09:33.136165 degex-0.0.20/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-03-21 13:23:11.000000 degex-0.0.20/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-03-21 13:23:11.000000 degex-0.0.20/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:09:33.136034 degex-0.0.20/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      291 2023-05-26 15:02:30.000000 degex-0.0.20/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:09:33.134606 degex-0.0.20/degex/
+-rw-r--r--   0 solst      (501) staff       (20)       23 2023-06-25 21:09:29.000000 degex-0.0.20/degex/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    18909 2023-06-25 21:09:29.000000 degex-0.0.20/degex/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)    21056 2023-06-25 21:09:29.000000 degex-0.0.20/degex/adata.py
+-rw-r--r--   0 solst      (501) staff       (20)    21299 2023-05-26 15:02:24.000000 degex-0.0.20/degex/branches.py
+-rw-r--r--   0 solst      (501) staff       (20)      531 2023-06-25 21:09:29.000000 degex-0.0.20/degex/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    21040 2023-05-26 15:02:24.000000 degex-0.0.20/degex/granger.py
+-rw-r--r--   0 solst      (501) staff       (20)     2850 2023-06-25 21:09:29.000000 degex-0.0.20/degex/plots.py
+-rw-r--r--   0 solst      (501) staff       (20)     4892 2023-06-25 21:09:29.000000 degex-0.0.20/degex/preprocessing.py
+-rw-r--r--   0 solst      (501) staff       (20)     2601 2023-06-25 21:09:29.000000 degex-0.0.20/degex/static.py
+-rw-r--r--   0 solst      (501) staff       (20)     2564 2023-06-25 21:09:29.000000 degex-0.0.20/degex/types.py
+-rw-r--r--   0 solst      (501) staff       (20)     2109 2023-06-25 21:09:29.000000 degex-0.0.20/degex/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:09:33.135848 degex-0.0.20/degex.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:09:33.000000 degex-0.0.20/degex.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      438 2023-06-25 21:09:33.000000 degex-0.0.20/degex.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-25 21:09:33.000000 degex-0.0.20/degex.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       32 2023-06-25 21:09:33.000000 degex-0.0.20/degex.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-05-26 15:02:38.000000 degex-0.0.20/degex.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      165 2023-06-25 21:09:33.000000 degex-0.0.20/degex.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        6 2023-06-25 21:09:33.000000 degex-0.0.20/degex.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)     1095 2023-06-25 21:09:29.000000 degex-0.0.20/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-25 21:09:33.136222 degex-0.0.20/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2541 2023-03-21 13:23:12.000000 degex-0.0.20/setup.py
```

### Comparing `degex-0.0.19/LICENSE` & `degex-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `degex-0.0.19/PKG-INFO` & `degex-0.0.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degex
-Version: 0.0.19
+Version: 0.0.20
 Summary: Detect Gene Expression in Single-CEll data
 Home-page: https://github.com/dsm-72/degex
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python single cell detect gene expression spot marker genes
 Classifier: Development Status :: 4 - Beta
```

### Comparing `degex-0.0.19/degex/_modidx.py` & `degex-0.0.20/degex/_modidx.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.19/degex/adata.py` & `degex-0.0.20/degex/adata.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
 
 def var_starts_with_pattern(name:str, patterns: Optional[Sequence[str]] = None) -> Tuple[str, tuple]:
     if patterns is None:
         patterns = (f'{name.lower()}_', )
     return name, patterns
 
 def make_var_starts_with(var_starts_with: Optional[Dict[str, tuple]] = dict()):
-    return {k: var_starts_with_pattern(v) for k, v in var_starts_with.items()}
+    return {k: var_starts_with_pattern(k, v) for k, v in var_starts_with.items()}
 
 
 def calc_qc_stats(
     adata: AnnData,
     qc_vars: Dict[str, tuple] = QC_VARS,
 ) -> AnnData:
     f"""
```

### Comparing `degex-0.0.19/degex/branches.py` & `degex-0.0.20/degex/branches.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.19/degex/core.py` & `degex-0.0.20/degex/core.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.19/degex/granger.py` & `degex-0.0.20/degex/granger.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.19/degex/plots.py` & `degex-0.0.20/degex/plots.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.19/degex/preprocessing.py` & `degex-0.0.20/degex/preprocessing.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.19/degex/static.py` & `degex-0.0.20/degex/static.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.19/degex/types.py` & `degex-0.0.20/degex/types.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.19/degex/utils.py` & `degex-0.0.20/degex/utils.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.19/degex.egg-info/PKG-INFO` & `degex-0.0.20/degex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degex
-Version: 0.0.19
+Version: 0.0.20
 Summary: Detect Gene Expression in Single-CEll data
 Home-page: https://github.com/dsm-72/degex
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python single cell detect gene expression spot marker genes
 Classifier: Development Status :: 4 - Beta
```

### Comparing `degex-0.0.19/settings.ini` & `degex-0.0.20/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = degex
 lib_name = degex
-version = 0.0.19
+version = 0.0.20
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = degex
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `degex-0.0.19/setup.py` & `degex-0.0.20/setup.py`

 * *Files identical despite different names*

