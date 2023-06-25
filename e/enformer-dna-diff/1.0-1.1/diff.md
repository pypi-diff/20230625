# Comparing `tmp/enformer_dna_diff-1.0.tar.gz` & `tmp/enformer_dna_diff-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enformer_dna_diff-1.0.tar", last modified: Sun Jun 11 12:39:39 2023, max compression
+gzip compressed data, was "enformer_dna_diff-1.1.tar", last modified: Sun Jun 25 15:13:46 2023, max compression
```

## Comparing `enformer_dna_diff-1.0.tar` & `enformer_dna_diff-1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-11 12:39:39.000000 enformer_dna_diff-1.0/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1063 2023-06-10 15:19:31.000000 enformer_dna_diff-1.0/LICENSE
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-11 12:39:39.000000 enformer_dna_diff-1.0/PKG-INFO
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1707 2023-06-10 15:19:19.000000 enformer_dna_diff-1.0/README.md
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-11 12:39:39.000000 enformer_dna_diff-1.0/enformer_dna_diff/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       43 2023-06-09 23:02:20.000000 enformer_dna_diff-1.0/enformer_dna_diff/__init__.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     3851 2023-06-09 23:02:20.000000 enformer_dna_diff-1.0/enformer_dna_diff/enformer.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    12998 2023-06-09 23:02:20.000000 enformer_dna_diff-1.0/enformer_dna_diff/enformerops.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    33364 2023-06-08 16:34:50.000000 enformer_dna_diff-1.0/enformer_dna_diff/main_script.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    11745 2023-06-09 14:09:05.000000 enformer_dna_diff-1.0/enformer_dna_diff/real_main_script.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2511 2023-06-09 23:02:20.000000 enformer_dna_diff-1.0/enformer_dna_diff/utils.py
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-11 12:39:39.000000 enformer_dna_diff-1.0/enformer_dna_diff.egg-info/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-11 12:39:38.000000 enformer_dna_diff-1.0/enformer_dna_diff.egg-info/PKG-INFO
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      433 2023-06-11 12:39:38.000000 enformer_dna_diff-1.0/enformer_dna_diff.egg-info/SOURCES.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)        1 2023-06-11 12:39:38.000000 enformer_dna_diff-1.0/enformer_dna_diff.egg-info/dependency_links.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     3524 2023-06-11 12:39:38.000000 enformer_dna_diff-1.0/enformer_dna_diff.egg-info/requires.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       18 2023-06-11 12:39:38.000000 enformer_dna_diff-1.0/enformer_dna_diff.egg-info/top_level.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2013 2023-06-09 23:02:20.000000 enformer_dna_diff-1.0/get_data.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       38 2023-06-11 12:39:39.000000 enformer_dna_diff-1.0/setup.cfg
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      554 2023-06-09 23:09:50.000000 enformer_dna_diff-1.0/setup.py
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1063 2023-06-10 15:19:31.000000 enformer_dna_diff-1.1/LICENSE
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/PKG-INFO
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1707 2023-06-10 15:19:19.000000 enformer_dna_diff-1.1/README.md
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/enformer_dna_diff/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       43 2023-06-09 23:02:20.000000 enformer_dna_diff-1.1/enformer_dna_diff/__init__.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     3851 2023-06-09 23:02:20.000000 enformer_dna_diff-1.1/enformer_dna_diff/enformer.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    12998 2023-06-25 15:13:11.000000 enformer_dna_diff-1.1/enformer_dna_diff/enformerops.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    33364 2023-06-08 16:34:50.000000 enformer_dna_diff-1.1/enformer_dna_diff/main_script.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    11745 2023-06-09 14:09:05.000000 enformer_dna_diff-1.1/enformer_dna_diff/real_main_script.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2511 2023-06-25 15:13:07.000000 enformer_dna_diff-1.1/enformer_dna_diff/utils.py
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:13:45.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/PKG-INFO
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      433 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)        1 2023-06-25 15:13:45.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2409 2023-06-25 15:13:45.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/requires.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       18 2023-06-25 15:13:45.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/top_level.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2013 2023-06-09 23:02:20.000000 enformer_dna_diff-1.1/get_data.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       38 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/setup.cfg
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      554 2023-06-25 15:12:38.000000 enformer_dna_diff-1.1/setup.py
```

### Comparing `enformer_dna_diff-1.0/LICENSE` & `enformer_dna_diff-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.0/README.md` & `enformer_dna_diff-1.1/README.md`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.0/enformer_dna_diff/enformer.py` & `enformer_dna_diff-1.1/enformer_dna_diff/enformer.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.0/enformer_dna_diff/enformerops.py` & `enformer_dna_diff-1.1/enformer_dna_diff/enformerops.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.0/enformer_dna_diff/main_script.py` & `enformer_dna_diff-1.1/enformer_dna_diff/main_script.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.0/enformer_dna_diff/real_main_script.py` & `enformer_dna_diff-1.1/enformer_dna_diff/real_main_script.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.0/enformer_dna_diff/utils.py` & `enformer_dna_diff-1.1/enformer_dna_diff/utils.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.0/get_data.py` & `enformer_dna_diff-1.1/get_data.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.0/setup.py` & `enformer_dna_diff-1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required_libraries = f.read().splitlines()
 # import ipdb;ipdb.set_trace()
 setup(
     name="enformer_dna_diff",
-    version="1.0",
+    version="1.1",
     packages=find_packages(),
     install_requires=required_libraries,
     scripts=['get_data.py'],
     author="Tin M. Tunjic",
     author_email="tunjictin@gmail.com",
     description="This is a package for that combines DeepMind Enformer model with DNA Diffusion project",
     url="https://github.com/ttunja/Enformer_DNA_Diffusion.git"
```

