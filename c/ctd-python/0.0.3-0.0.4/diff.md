# Comparing `tmp/ctd-python-0.0.3.tar.gz` & `tmp/ctd-python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctd-python-0.0.3.tar", last modified: Sun Jun 25 20:58:09 2023, max compression
+gzip compressed data, was "ctd-python-0.0.4.tar", last modified: Sun Jun 25 21:06:13 2023, max compression
```

## Comparing `ctd-python-0.0.3.tar` & `ctd-python-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 20:58:09.817692 ctd-python-0.0.3/
--rw-r--r--   0 john       (501) staff       (20)     1600 2023-06-25 20:58:09.817050 ctd-python-0.0.3/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      970 2023-06-25 20:53:40.000000 ctd-python-0.0.3/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 20:58:09.813120 ctd-python-0.0.3/ctd/
--rw-r--r--   0 john       (501) staff       (20)     2414 2023-06-25 20:57:09.000000 ctd-python-0.0.3/ctd/__init__.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 20:58:09.816163 ctd-python-0.0.3/ctd_python.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     1600 2023-06-25 20:58:09.000000 ctd-python-0.0.3/ctd_python.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      203 2023-06-25 20:58:09.000000 ctd-python-0.0.3/ctd_python.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-06-25 20:58:09.000000 ctd-python-0.0.3/ctd_python.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       16 2023-06-25 20:58:09.000000 ctd-python-0.0.3/ctd_python.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        4 2023-06-25 20:58:09.000000 ctd-python-0.0.3/ctd_python.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-06-25 20:58:09.817825 ctd-python-0.0.3/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)      436 2023-06-25 20:57:13.000000 ctd-python-0.0.3/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 21:06:13.303824 ctd-python-0.0.4/
+-rw-r--r--   0 john       (501) staff       (20)     1604 2023-06-25 21:06:13.303173 ctd-python-0.0.4/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      974 2023-06-25 21:03:16.000000 ctd-python-0.0.4/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 21:06:13.299074 ctd-python-0.0.4/ctd/
+-rw-r--r--   0 john       (501) staff       (20)     2396 2023-06-25 21:04:11.000000 ctd-python-0.0.4/ctd/__init__.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 21:06:13.302359 ctd-python-0.0.4/ctd_python.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     1604 2023-06-25 21:06:13.000000 ctd-python-0.0.4/ctd_python.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      203 2023-06-25 21:06:13.000000 ctd-python-0.0.4/ctd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-06-25 21:06:13.000000 ctd-python-0.0.4/ctd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       16 2023-06-25 21:06:13.000000 ctd-python-0.0.4/ctd_python.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        4 2023-06-25 21:06:13.000000 ctd-python-0.0.4/ctd_python.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2023-06-25 21:06:13.303990 ctd-python-0.0.4/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)      436 2023-06-25 21:05:56.000000 ctd-python-0.0.4/setup.py
```

### Comparing `ctd-python-0.0.3/PKG-INFO` & `ctd-python-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
         
@@ -13,15 +13,15 @@
         ```
         pip3 install ctd-python
         ```
         
         ### import the package in order to pull the data
         
         ```
-        from ctd import get_df
+        from ctd import get_data
         ```
         
         ## The package offers the following resources as DataFrames
         
         - GeneInteractionTypes
         - ChemicalPathwaysEnriched
         - GeneDisease
@@ -32,15 +32,15 @@
         - Genes
         - ChemicalGeneInteractions
         - Chemicals
         - Diseases
         
         ### Get the Gene Information for TNF
         ```
-        gene_df = get_df('Genes')
+        gene_df = get_data('Genes')
         tnf_df = gene_df[gene_df['GeneSymbol'] == 'TNF']
         ```
         
         ### Get Chemical Interactions for TNF
         ```
         chem_gene_df = get_data('ChemicalGeneInteractions')
         tnf_chem_df = chem_gene_df[chem_gene_df['GeneSymbol'] == 'TNF']
```

### Comparing `ctd-python-0.0.3/README.md` & `ctd-python-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```
 pip3 install ctd-python
 ```
 
 ### import the package in order to pull the data
 
 ```
-from ctd import get_df
+from ctd import get_data
 ```
 
 ## The package offers the following resources as DataFrames
 
 - GeneInteractionTypes
 - ChemicalPathwaysEnriched
 - GeneDisease
@@ -26,15 +26,15 @@
 - Genes
 - ChemicalGeneInteractions
 - Chemicals
 - Diseases
 
 ### Get the Gene Information for TNF
 ```
-gene_df = get_df('Genes')
+gene_df = get_data('Genes')
 tnf_df = gene_df[gene_df['GeneSymbol'] == 'TNF']
 ```
 
 ### Get Chemical Interactions for TNF
 ```
 chem_gene_df = get_data('ChemicalGeneInteractions')
 tnf_chem_df = chem_gene_df[chem_gene_df['GeneSymbol'] == 'TNF']
```

### Comparing `ctd-python-0.0.3/ctd/__init__.py` & `ctd-python-0.0.4/ctd/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-import os
-import gzip
-import shutil
-import logging
-import requests
-import pandas as pd
-
 RESOURCES = {
     'GeneInteractionTypes': 'CTD_chem_gene_ixn_types',
     'ChemicalPathwaysEnriched': 'CTD_chem_pathways_enriched',
     'GeneDisease': 'CTD_genes_diseases',
     'GenePathways': 'CTD_genes_pathways',
     'DiseasePathways': 'CTD_diseases_pathways',
     'ChemocalPhenoTypeInteractions': 'CTD_pheno_term_ixns',
@@ -40,14 +33,16 @@
     unzipped_filename = os.path.join(UNZIPPED_DATA_DIR, url.split('/')[-1].replace('.gz', ''))
 
     if os.path.isfile(unzipped_filename):
         return
 
     with requests.get(url, stream=True) as r:
         r.raise_for_status()
+        print('----local_filename----')
+        print(local_filename)
         with open(local_filename, 'wb') as f:
             for chunk in r.iter_content(chunk_size=8192):
                 f.write(chunk)
 
     with gzip.open(local_filename, 'rb') as f_in:
         with open(unzipped_filename, 'wb') as f_out:
             shutil.copyfileobj(f_in, f_out)
```

### Comparing `ctd-python-0.0.3/ctd_python.egg-info/PKG-INFO` & `ctd-python-0.0.4/ctd_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
         
@@ -13,15 +13,15 @@
         ```
         pip3 install ctd-python
         ```
         
         ### import the package in order to pull the data
         
         ```
-        from ctd import get_df
+        from ctd import get_data
         ```
         
         ## The package offers the following resources as DataFrames
         
         - GeneInteractionTypes
         - ChemicalPathwaysEnriched
         - GeneDisease
@@ -32,15 +32,15 @@
         - Genes
         - ChemicalGeneInteractions
         - Chemicals
         - Diseases
         
         ### Get the Gene Information for TNF
         ```
-        gene_df = get_df('Genes')
+        gene_df = get_data('Genes')
         tnf_df = gene_df[gene_df['GeneSymbol'] == 'TNF']
         ```
         
         ### Get Chemical Interactions for TNF
         ```
         chem_gene_df = get_data('ChemicalGeneInteractions')
         tnf_chem_df = chem_gene_df[chem_gene_df['GeneSymbol'] == 'TNF']
```

