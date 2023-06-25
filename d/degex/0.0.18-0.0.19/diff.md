# Comparing `tmp/degex-0.0.18.tar.gz` & `tmp/degex-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degex-0.0.18.tar", last modified: Sun Jun 25 16:11:16 2023, max compression
+gzip compressed data, was "degex-0.0.19.tar", last modified: Sun Jun 25 21:04:28 2023, max compression
```

## Comparing `degex-0.0.18.tar` & `degex-0.0.19.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 16:11:16.073119 degex-0.0.18/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-03-21 13:23:11.000000 degex-0.0.18/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-03-21 13:23:11.000000 degex-0.0.18/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 16:11:16.072983 degex-0.0.18/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      291 2023-05-26 15:02:30.000000 degex-0.0.18/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 16:11:16.071546 degex-0.0.18/degex/
--rw-r--r--   0 solst      (501) staff       (20)       23 2023-06-25 16:06:57.000000 degex-0.0.18/degex/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    18909 2023-06-25 16:06:57.000000 degex-0.0.18/degex/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)    21047 2023-06-25 16:06:57.000000 degex-0.0.18/degex/adata.py
--rw-r--r--   0 solst      (501) staff       (20)    21299 2023-05-26 15:02:24.000000 degex-0.0.18/degex/branches.py
--rw-r--r--   0 solst      (501) staff       (20)      531 2023-06-25 16:06:57.000000 degex-0.0.18/degex/core.py
--rw-r--r--   0 solst      (501) staff       (20)    21040 2023-05-26 15:02:24.000000 degex-0.0.18/degex/granger.py
--rw-r--r--   0 solst      (501) staff       (20)     2850 2023-06-25 16:06:57.000000 degex-0.0.18/degex/plots.py
--rw-r--r--   0 solst      (501) staff       (20)     4892 2023-06-25 16:06:57.000000 degex-0.0.18/degex/preprocessing.py
--rw-r--r--   0 solst      (501) staff       (20)     2601 2023-06-25 16:06:57.000000 degex-0.0.18/degex/static.py
--rw-r--r--   0 solst      (501) staff       (20)     2564 2023-06-25 16:06:57.000000 degex-0.0.18/degex/types.py
--rw-r--r--   0 solst      (501) staff       (20)     2109 2023-06-25 16:06:57.000000 degex-0.0.18/degex/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 16:11:16.072769 degex-0.0.18/degex.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 16:11:16.000000 degex-0.0.18/degex.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      438 2023-06-25 16:11:16.000000 degex-0.0.18/degex.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-25 16:11:16.000000 degex-0.0.18/degex.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       32 2023-06-25 16:11:16.000000 degex-0.0.18/degex.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-05-26 15:02:38.000000 degex-0.0.18/degex.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      225 2023-06-25 16:11:16.000000 degex-0.0.18/degex.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        6 2023-06-25 16:11:16.000000 degex-0.0.18/degex.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)     1098 2023-06-25 16:06:57.000000 degex-0.0.18/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-25 16:11:16.073161 degex-0.0.18/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2541 2023-03-21 13:23:12.000000 degex-0.0.18/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:04:28.102074 degex-0.0.19/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-03-21 13:23:11.000000 degex-0.0.19/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-03-21 13:23:11.000000 degex-0.0.19/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:04:28.101938 degex-0.0.19/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      291 2023-05-26 15:02:30.000000 degex-0.0.19/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:04:28.100643 degex-0.0.19/degex/
+-rw-r--r--   0 solst      (501) staff       (20)       23 2023-06-25 21:04:22.000000 degex-0.0.19/degex/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    18909 2023-06-25 21:04:22.000000 degex-0.0.19/degex/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)    21053 2023-06-25 21:04:22.000000 degex-0.0.19/degex/adata.py
+-rw-r--r--   0 solst      (501) staff       (20)    21299 2023-05-26 15:02:24.000000 degex-0.0.19/degex/branches.py
+-rw-r--r--   0 solst      (501) staff       (20)      531 2023-06-25 21:04:22.000000 degex-0.0.19/degex/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    21040 2023-05-26 15:02:24.000000 degex-0.0.19/degex/granger.py
+-rw-r--r--   0 solst      (501) staff       (20)     2850 2023-06-25 21:04:22.000000 degex-0.0.19/degex/plots.py
+-rw-r--r--   0 solst      (501) staff       (20)     4892 2023-06-25 21:04:22.000000 degex-0.0.19/degex/preprocessing.py
+-rw-r--r--   0 solst      (501) staff       (20)     2601 2023-06-25 21:04:22.000000 degex-0.0.19/degex/static.py
+-rw-r--r--   0 solst      (501) staff       (20)     2564 2023-06-25 21:04:22.000000 degex-0.0.19/degex/types.py
+-rw-r--r--   0 solst      (501) staff       (20)     2109 2023-06-25 21:04:22.000000 degex-0.0.19/degex/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:04:28.101754 degex-0.0.19/degex.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      438 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       32 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-05-26 15:02:38.000000 degex-0.0.19/degex.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      165 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        6 2023-06-25 21:04:28.000000 degex-0.0.19/degex.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)     1095 2023-06-25 21:04:20.000000 degex-0.0.19/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-25 21:04:28.102114 degex-0.0.19/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2541 2023-03-21 13:23:12.000000 degex-0.0.19/setup.py
```

### Comparing `degex-0.0.18/LICENSE` & `degex-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `degex-0.0.18/PKG-INFO` & `degex-0.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degex
-Version: 0.0.18
+Version: 0.0.19
 Summary: Detect Gene Expression in Single-CEll data
 Home-page: https://github.com/dsm-72/degex
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python single cell detect gene expression spot marker genes
 Classifier: Development Status :: 4 - Beta
```

### Comparing `degex-0.0.18/degex/_modidx.py` & `degex-0.0.19/degex/_modidx.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.18/degex/adata.py` & `degex-0.0.19/degex/adata.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         print(adata.obs[key].value_counts())
     return adata
 
 # %% ../nbs/03_adata.ipynb 13
 def stack_batchs(
     *adatas: AnnDatas, 
     idx_to_time: dict,
-    idx_to_batch: dict=None,
+    idx_to_batch: dict = None,
     batch_to_timepoint: dict = None,
     print_counts: bool = False
 ) -> AnnData:    
     """
     Concatenates the each one of the `adata`s in  
     `adatas` to a single `adata` instance.
     
@@ -252,15 +252,15 @@
         }
     """
     time_to_num = time_to_num_from_idx_to_time(idx_to_time)
 
     replace_batch = idx_to_time if idx_to_batch is None else idx_to_batch
     replace_times = time_to_num if batch_to_timepoint is None else batch_to_timepoint
 
-    adata = stack(*adatas, BATCH, replace=replace_batch)
+    adata = stack(*adatas, key=BATCH, replace=replace_batch)
     adata.obs[TIMEPOINT] = adata.obs[BATCH].replace(replace_times)
     
     if print_counts:
         print(adata.obs[BATCH].value_counts())
     return adata
 
 # %% ../nbs/03_adata.ipynb 15
```

### Comparing `degex-0.0.18/degex/branches.py` & `degex-0.0.19/degex/branches.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.18/degex/core.py` & `degex-0.0.19/degex/core.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.18/degex/granger.py` & `degex-0.0.19/degex/granger.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.18/degex/plots.py` & `degex-0.0.19/degex/plots.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.18/degex/preprocessing.py` & `degex-0.0.19/degex/preprocessing.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.18/degex/static.py` & `degex-0.0.19/degex/static.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.18/degex/types.py` & `degex-0.0.19/degex/types.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.18/degex/utils.py` & `degex-0.0.19/degex/utils.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.18/degex.egg-info/PKG-INFO` & `degex-0.0.19/degex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degex
-Version: 0.0.18
+Version: 0.0.19
 Summary: Detect Gene Expression in Single-CEll data
 Home-page: https://github.com/dsm-72/degex
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python single cell detect gene expression spot marker genes
 Classifier: Development Status :: 4 - Beta
```

### Comparing `degex-0.0.18/settings.ini` & `degex-0.0.19/settings.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = degex
 lib_name = degex
-version = 0.0.18
+version = 0.0.19
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = degex
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -23,15 +23,17 @@
 description = Detect Gene Expression in Single-CEll data
 keywords = nbdev jupyter notebook python single cell detect gene expression spot marker genes
 language = English
 status = 3
 user = dsm-72
 conda_user = dsm-72
 host = github
-requirements = ipykernel pandas==1.3.5 scipy requests natsort seaborn scikit-learn numpy graphtools matplotlib==3.7.0 ipywidgets scanpy==1.9.2 anndata==0.8.0 scprep gseapy phate python-slugify magic-impute meld DiffusionEMD scrublet
+requirements = pandas scipy seaborn scikit-learn numpy graphtools matplotlib==3.7.0 scanpy==1.9.2 anndata==0.8.0
+pip_requirements = phate scprep magic-impute meld scrublet gseapy DiffusionEMD
+conda_requirements = bioconda::gseapy
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
```

### Comparing `degex-0.0.18/setup.py` & `degex-0.0.19/setup.py`

 * *Files identical despite different names*

