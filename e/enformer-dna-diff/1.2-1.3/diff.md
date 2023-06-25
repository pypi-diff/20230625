# Comparing `tmp/enformer_dna_diff-1.2.tar.gz` & `tmp/enformer_dna_diff-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enformer_dna_diff-1.2.tar", last modified: Sun Jun 25 15:32:23 2023, max compression
+gzip compressed data, was "enformer_dna_diff-1.3.tar", last modified: Sun Jun 25 15:43:58 2023, max compression
```

## Comparing `enformer_dna_diff-1.2.tar` & `enformer_dna_diff-1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1063 2023-06-10 15:19:31.000000 enformer_dna_diff-1.2/LICENSE
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/PKG-INFO
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1707 2023-06-10 15:19:19.000000 enformer_dna_diff-1.2/README.md
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       43 2023-06-09 23:02:20.000000 enformer_dna_diff-1.2/enformer_dna_diff/__init__.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     3851 2023-06-09 23:02:20.000000 enformer_dna_diff-1.2/enformer_dna_diff/enformer.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    12998 2023-06-25 15:31:15.000000 enformer_dna_diff-1.2/enformer_dna_diff/enformerops.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    33364 2023-06-08 16:34:50.000000 enformer_dna_diff-1.2/enformer_dna_diff/main_script.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    11745 2023-06-09 14:09:05.000000 enformer_dna_diff-1.2/enformer_dna_diff/real_main_script.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2511 2023-06-25 15:31:19.000000 enformer_dna_diff-1.2/enformer_dna_diff/utils.py
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/PKG-INFO
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      433 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/SOURCES.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)        1 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/dependency_links.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2383 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/requires.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       18 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/top_level.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2013 2023-06-09 23:02:20.000000 enformer_dna_diff-1.2/get_data.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       38 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/setup.cfg
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      554 2023-06-25 15:31:26.000000 enformer_dna_diff-1.2/setup.py
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1063 2023-06-10 15:19:31.000000 enformer_dna_diff-1.3/LICENSE
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/PKG-INFO
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1707 2023-06-10 15:19:19.000000 enformer_dna_diff-1.3/README.md
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       43 2023-06-09 23:02:20.000000 enformer_dna_diff-1.3/enformer_dna_diff/__init__.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     3851 2023-06-09 23:02:20.000000 enformer_dna_diff-1.3/enformer_dna_diff/enformer.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    12998 2023-06-25 15:42:54.000000 enformer_dna_diff-1.3/enformer_dna_diff/enformerops.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    33364 2023-06-08 16:34:50.000000 enformer_dna_diff-1.3/enformer_dna_diff/main_script.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    11745 2023-06-09 14:09:05.000000 enformer_dna_diff-1.3/enformer_dna_diff/real_main_script.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2511 2023-06-25 15:42:57.000000 enformer_dna_diff-1.3/enformer_dna_diff/utils.py
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/PKG-INFO
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      433 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)        1 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2381 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/requires.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       18 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/top_level.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2013 2023-06-09 23:02:20.000000 enformer_dna_diff-1.3/get_data.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       38 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/setup.cfg
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      554 2023-06-25 15:42:45.000000 enformer_dna_diff-1.3/setup.py
```

### Comparing `enformer_dna_diff-1.2/LICENSE` & `enformer_dna_diff-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.2/README.md` & `enformer_dna_diff-1.3/README.md`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.2/enformer_dna_diff/enformer.py` & `enformer_dna_diff-1.3/enformer_dna_diff/enformer.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.2/enformer_dna_diff/enformerops.py` & `enformer_dna_diff-1.3/enformer_dna_diff/enformerops.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.2/enformer_dna_diff/main_script.py` & `enformer_dna_diff-1.3/enformer_dna_diff/main_script.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.2/enformer_dna_diff/real_main_script.py` & `enformer_dna_diff-1.3/enformer_dna_diff/real_main_script.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.2/enformer_dna_diff/utils.py` & `enformer_dna_diff-1.3/enformer_dna_diff/utils.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.2/enformer_dna_diff.egg-info/requires.txt` & `enformer_dna_diff-1.3/enformer_dna_diff.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 cloudpickle==2.2.1
 colorlog==6.7.0
 comm==0.1.3
 contourpy==1.1.0
 cookiecutter==2.1.1
 cycler==0.11.0
 debugpy==1.6.7
-decorator==4.0.6
+decorator==5.1.1
 deprecation==2.1.0
 dm-tree==0.1.8
 etils==1.3.0
 executing==1.2.0
 flatbuffers==23.5.26
 fonttools==4.40.0
 future==0.18.3
@@ -120,13 +120,13 @@
 tinydb==4.8.0
 toml==0.10.2
 tornado==6.3.1
 tqdm==4.65.0
 traitlets==5.9.0
 typing_extensions==4.6.3
 tzdata==2023.3
-urllib3==1.24.3
+urllib3==1.25
 wcwidth==0.2.6
 Werkzeug==2.3.6
 wget==3.2
 wrapt==1.14.1
 zipp==3.15.0
```

### Comparing `enformer_dna_diff-1.2/get_data.py` & `enformer_dna_diff-1.3/get_data.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.2/setup.py` & `enformer_dna_diff-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required_libraries = f.read().splitlines()
 # import ipdb;ipdb.set_trace()
 setup(
     name="enformer_dna_diff",
-    version="1.2",
+    version="1.3",
     packages=find_packages(),
     install_requires=required_libraries,
     scripts=['get_data.py'],
     author="Tin M. Tunjic",
     author_email="tunjictin@gmail.com",
     description="This is a package for that combines DeepMind Enformer model with DNA Diffusion project",
     url="https://github.com/ttunja/Enformer_DNA_Diffusion.git"
```

