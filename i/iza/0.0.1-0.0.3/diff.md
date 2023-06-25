# Comparing `tmp/iza-0.0.1.tar.gz` & `tmp/iza-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iza-0.0.1.tar", last modified: Sun Jun 25 20:33:52 2023, max compression
+gzip compressed data, was "iza-0.0.3.tar", last modified: Sun Jun 25 21:25:25 2023, max compression
```

## Comparing `iza-0.0.1.tar` & `iza-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 20:33:52.045989 iza-0.0.1/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 iza-0.0.1/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 iza-0.0.1/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2118 2023-06-25 20:33:52.045797 iza-0.0.1/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1348 2023-06-24 20:51:36.000000 iza-0.0.1/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 20:33:52.043550 iza-0.0.1/iza/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-25 20:31:33.000000 iza-0.0.1/iza/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    13717 2023-06-25 20:32:26.000000 iza-0.0.1/iza/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     2046 2023-06-25 20:31:33.000000 iza-0.0.1/iza/commands.py
--rw-r--r--   0 solst      (501) staff       (20)    14824 2023-06-25 20:31:33.000000 iza-0.0.1/iza/nbs.py
--rw-r--r--   0 solst      (501) staff       (20)     4983 2023-06-25 20:31:33.000000 iza-0.0.1/iza/plots.py
--rw-r--r--   0 solst      (501) staff       (20)      448 2023-06-25 20:31:33.000000 iza-0.0.1/iza/rich.py
--rw-r--r--   0 solst      (501) staff       (20)     8038 2023-06-25 20:31:33.000000 iza-0.0.1/iza/static.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-25 20:31:33.000000 iza-0.0.1/iza/typer.py
--rw-r--r--   0 solst      (501) staff       (20)     3092 2023-06-25 20:31:33.000000 iza-0.0.1/iza/types.py
--rw-r--r--   0 solst      (501) staff       (20)    38180 2023-06-25 20:31:33.000000 iza-0.0.1/iza/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 20:33:52.045091 iza-0.0.1/iza.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2118 2023-06-25 20:33:52.000000 iza-0.0.1/iza.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      377 2023-06-25 20:33:52.000000 iza-0.0.1/iza.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-25 20:33:52.000000 iza-0.0.1/iza.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       70 2023-06-25 20:33:52.000000 iza-0.0.1/iza.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-24 20:04:21.000000 iza-0.0.1/iza.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-25 20:33:52.000000 iza-0.0.1/iza.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        4 2023-06-25 20:33:52.000000 iza-0.0.1/iza.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)     1013 2023-06-24 21:10:42.000000 iza-0.0.1/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-25 20:33:52.046045 iza-0.0.1/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-06-24 19:23:39.000000 iza-0.0.1/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:25:25.463561 iza-0.0.3/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 iza-0.0.3/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 iza-0.0.3/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2118 2023-06-25 21:25:25.463426 iza-0.0.3/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1348 2023-06-24 20:51:36.000000 iza-0.0.3/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:25:25.461841 iza-0.0.3/iza/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-25 21:25:01.000000 iza-0.0.3/iza/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    13717 2023-06-25 21:25:01.000000 iza-0.0.3/iza/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     2046 2023-06-25 21:25:01.000000 iza-0.0.3/iza/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)    14824 2023-06-25 21:25:01.000000 iza-0.0.3/iza/nbs.py
+-rw-r--r--   0 solst      (501) staff       (20)     4983 2023-06-25 21:25:01.000000 iza-0.0.3/iza/plots.py
+-rw-r--r--   0 solst      (501) staff       (20)      448 2023-06-25 21:25:01.000000 iza-0.0.3/iza/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)     8038 2023-06-25 21:25:01.000000 iza-0.0.3/iza/static.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-25 21:25:01.000000 iza-0.0.3/iza/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)     3092 2023-06-25 21:25:01.000000 iza-0.0.3/iza/types.py
+-rw-r--r--   0 solst      (501) staff       (20)    38180 2023-06-25 21:25:01.000000 iza-0.0.3/iza/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:25:25.463216 iza-0.0.3/iza.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2118 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      377 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       70 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-24 20:04:21.000000 iza-0.0.3/iza.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        4 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      816 2023-06-25 21:24:59.000000 iza-0.0.3/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-25 21:25:25.463605 iza-0.0.3/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-06-24 19:23:39.000000 iza-0.0.3/setup.py
```

### Comparing `iza-0.0.1/LICENSE` & `iza-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iza-0.0.1/PKG-INFO` & `iza-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iza
-Version: 0.0.1
+Version: 0.0.3
 Summary: chaos package of utilities; a nod to izalith
 Home-page: https://github.com/dsm-72/iza
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iza-0.0.1/README.md` & `iza-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `iza-0.0.1/iza/_modidx.py` & `iza-0.0.3/iza/_modidx.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.1/iza/commands.py` & `iza-0.0.3/iza/commands.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.1/iza/nbs.py` & `iza-0.0.3/iza/nbs.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.1/iza/plots.py` & `iza-0.0.3/iza/plots.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.1/iza/static.py` & `iza-0.0.3/iza/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,18 +169,18 @@
 # Layer storing PCA embedding in adata.obsm
 X_PCA = f'{X_}{PCA}'
 
 # Layer storing PCA embedding just on HVGs in adata.obsm
 X_PCA_HVG = f'{X_}{PCA}_{HVG}'
 
 # Layer storing PHATE embedding just in adata.obsm
-X_PHATE = f'{X_}{PHATE}_{HVG}'
+X_PHATE = f'{X_}{PHATE}'
 
 # Layer storing PHATE embedding just on HVGs in adata.obsm
-X_PHATE_HVG = f'{X_}{MAGIC}'
+X_PHATE_HVG = f'{X_}{PHATE}_{HVG}'
 
 # %% ../nbs/01_static.ipynb 27
 ADATA = 'adata'
 MATRIX = 'matrix'
 FEATURES = 'features'
 SENSITIVITY = 'sensitivity'
```

### Comparing `iza-0.0.1/iza/types.py` & `iza-0.0.3/iza/types.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.1/iza/utils.py` & `iza-0.0.3/iza/utils.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.1/iza.egg-info/PKG-INFO` & `iza-0.0.3/iza.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iza
-Version: 0.0.1
+Version: 0.0.3
 Summary: chaos package of utilities; a nod to izalith
 Home-page: https://github.com/dsm-72/iza
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iza-0.0.1/setup.py` & `iza-0.0.3/setup.py`

 * *Files identical despite different names*

