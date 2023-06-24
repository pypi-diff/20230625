# Comparing `tmp/hmmix-0.6.6.tar.gz` & `tmp/hmmix-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hmmix-0.6.6.tar", last modified: Thu Jun 22 21:00:18 2023, max compression
+gzip compressed data, was "dist/hmmix-0.6.7.tar", last modified: Sat Jun 24 23:31:24 2023, max compression
```

## Comparing `hmmix-0.6.6.tar` & `hmmix-0.6.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-22 21:00:18.000000 hmmix-0.6.6/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    35149 2022-05-11 17:42:22.000000 hmmix-0.6.6/LICENSE.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34626 2023-06-22 21:00:18.000000 hmmix-0.6.6/PKG-INFO
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34092 2023-02-27 21:20:22.000000 hmmix-0.6.6/README.md
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       38 2023-06-22 21:00:18.000000 hmmix-0.6.6/setup.cfg
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      994 2023-06-22 19:56:41.000000 hmmix-0.6.6/setup.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     8599 2023-06-22 20:59:26.000000 hmmix-0.6.6/src/bcf_vcf.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    15245 2023-06-22 20:45:50.000000 hmmix-0.6.6/src/helper_functions.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    13669 2023-03-03 06:04:46.000000 hmmix-0.6.6/src/hmm_functions.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34626 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/PKG-INFO
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      411 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/SOURCES.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        1 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/dependency_links.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       36 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/entry_points.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       29 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/requires.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       77 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/top_level.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    16030 2023-06-22 20:45:54.000000 hmmix-0.6.6/src/main.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2007 2022-10-25 01:10:14.000000 hmmix-0.6.6/src/make_mutationrate.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     4281 2022-10-25 01:10:46.000000 hmmix-0.6.6/src/make_test_data.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-22 21:00:18.000000 hmmix-0.6.6/test/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2725 2022-05-26 04:20:02.000000 hmmix-0.6.6/test/test.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     3106 2022-06-02 06:35:33.000000 hmmix-0.6.6/test/test2.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      541 2022-06-08 21:55:04.000000 hmmix-0.6.6/test/test_main.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        0 2022-07-12 05:40:51.000000 hmmix-0.6.6/test/testfred.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-24 23:31:24.000000 hmmix-0.6.7/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    35149 2022-05-11 17:42:22.000000 hmmix-0.6.7/LICENSE.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34626 2023-06-24 23:31:24.000000 hmmix-0.6.7/PKG-INFO
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34092 2023-06-24 23:30:17.000000 hmmix-0.6.7/README.md
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       38 2023-06-24 23:31:24.000000 hmmix-0.6.7/setup.cfg
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      994 2023-06-24 23:30:06.000000 hmmix-0.6.7/setup.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-24 23:31:24.000000 hmmix-0.6.7/src/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     8599 2023-06-22 20:59:26.000000 hmmix-0.6.7/src/bcf_vcf.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    15297 2023-06-24 23:29:17.000000 hmmix-0.6.7/src/helper_functions.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    13669 2023-03-03 06:04:46.000000 hmmix-0.6.7/src/hmm_functions.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-24 23:31:24.000000 hmmix-0.6.7/src/hmmix.egg-info/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34626 2023-06-24 23:31:23.000000 hmmix-0.6.7/src/hmmix.egg-info/PKG-INFO
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      411 2023-06-24 23:31:24.000000 hmmix-0.6.7/src/hmmix.egg-info/SOURCES.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        1 2023-06-24 23:31:23.000000 hmmix-0.6.7/src/hmmix.egg-info/dependency_links.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       36 2023-06-24 23:31:23.000000 hmmix-0.6.7/src/hmmix.egg-info/entry_points.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       29 2023-06-24 23:31:24.000000 hmmix-0.6.7/src/hmmix.egg-info/requires.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       77 2023-06-24 23:31:24.000000 hmmix-0.6.7/src/hmmix.egg-info/top_level.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    16030 2023-06-24 23:30:54.000000 hmmix-0.6.7/src/main.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2007 2022-10-25 01:10:14.000000 hmmix-0.6.7/src/make_mutationrate.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     4281 2022-10-25 01:10:46.000000 hmmix-0.6.7/src/make_test_data.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-24 23:31:24.000000 hmmix-0.6.7/test/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2725 2022-05-26 04:20:02.000000 hmmix-0.6.7/test/test.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     3106 2022-06-02 06:35:33.000000 hmmix-0.6.7/test/test2.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      541 2022-06-08 21:55:04.000000 hmmix-0.6.7/test/test_main.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        0 2022-07-12 05:40:51.000000 hmmix-0.6.7/test/testfred.py
```

### Comparing `hmmix-0.6.6/LICENSE.txt` & `hmmix-0.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.6/PKG-INFO` & `hmmix-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmix
-Version: 0.6.6
+Version: 0.6.7
 Summary: Find introgressed segments
 Home-page: https://github.com/LauritsSkov/Introgression-detection
 Author: Laurits Skov and Moises Coll Macia
 Author-email: lauritsskov2@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hmmix-0.6.6/README.md` & `hmmix-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.6/setup.py` & `hmmix-0.6.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='hmmix', 
-    version = '0.6.6',
+    version = '0.6.7',
     description='Find introgressed segments',
     py_modules=['bcf_vcf', 'helper_functions', 'hmm_functions', 'main', 'make_mutationrate', 'make_test_data'],
     package_dir={'': 'src'},
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `hmmix-0.6.6/src/bcf_vcf.py` & `hmmix-0.6.7/src/bcf_vcf.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.6/src/helper_functions.py` & `hmmix-0.6.7/src/helper_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,22 +275,23 @@
                 individuals_in_vcffile = line.strip().split()[9:]
 
             if not line.startswith('#'):
 
                 chrom, pos, _, ref_allele, alt_allele = line.strip().split()[0:5]
                 ID =  f'{chrom}_{pos}'
                 genotypes = [x.split(':')[0] for x in line.strip().split()[9:]]
+                all_bases = [ref_allele] + alt_allele.split(',')
 
                 ancestral_base, derived_base = obs[ID]
                 found_in = []
 
                 for original_genotype, individual in zip(genotypes, individuals_in_vcffile):
 
                     if '.' not in original_genotype:
-                        genotype = convert_to_bases(original_genotype, ref_allele, alt_allele)   
+                        genotype = convert_to_bases(original_genotype, all_bases)   
 
                         if genotype.count(derived_base) > 0:
                             found_in.append(individual)
 
                 if len(found_in) > 0:
                     shared_with[ID] = '|'.join(found_in)
```

### Comparing `hmmix-0.6.6/src/hmm_functions.py` & `hmmix-0.6.7/src/hmm_functions.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.6/src/hmmix.egg-info/PKG-INFO` & `hmmix-0.6.7/src/hmmix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmix
-Version: 0.6.6
+Version: 0.6.7
 Summary: Find introgressed segments
 Home-page: https://github.com/LauritsSkov/Introgression-detection
 Author: Laurits Skov and Moises Coll Macia
 Author-email: lauritsskov2@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hmmix-0.6.6/src/main.py` & `hmmix-0.6.7/src/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from hmm_functions import TrainModel, DecodeModel, write_HMM_to_file, read_HMM_parameters_from_file, Write_Decoded_output
 from bcf_vcf import make_out_group, make_ingroup_obs
 from make_test_data import create_test_data
 from make_mutationrate import make_mutation_rate
 from helper_functions import Load_observations_weights_mutrates, handle_individuals_input, handle_infiles, combined_files
 
 
-VERSION = '0.6.6'
+VERSION = '0.6.7'
 
 
 def print_script_usage():
     toprint = f'''
 Script for identifying introgressed archaic segments (version: {VERSION})
 
 > Turorial:
```

### Comparing `hmmix-0.6.6/src/make_mutationrate.py` & `hmmix-0.6.7/src/make_mutationrate.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.6/src/make_test_data.py` & `hmmix-0.6.7/src/make_test_data.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.6/test/test.py` & `hmmix-0.6.7/test/test.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.6/test/test2.py` & `hmmix-0.6.7/test/test2.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.6/test/test_main.py` & `hmmix-0.6.7/test/test_main.py`

 * *Files identical despite different names*

