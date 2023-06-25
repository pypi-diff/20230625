# Comparing `tmp/enformer_dna_diff-1.1.tar.gz` & `tmp/enformer_dna_diff-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enformer_dna_diff-1.1.tar", last modified: Sun Jun 25 15:13:46 2023, max compression
+gzip compressed data, was "enformer_dna_diff-1.2.tar", last modified: Sun Jun 25 15:32:23 2023, max compression
```

## Comparing `enformer_dna_diff-1.1.tar` & `enformer_dna_diff-1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1063 2023-06-10 15:19:31.000000 enformer_dna_diff-1.1/LICENSE
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/PKG-INFO
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1707 2023-06-10 15:19:19.000000 enformer_dna_diff-1.1/README.md
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/enformer_dna_diff/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       43 2023-06-09 23:02:20.000000 enformer_dna_diff-1.1/enformer_dna_diff/__init__.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     3851 2023-06-09 23:02:20.000000 enformer_dna_diff-1.1/enformer_dna_diff/enformer.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    12998 2023-06-25 15:13:11.000000 enformer_dna_diff-1.1/enformer_dna_diff/enformerops.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    33364 2023-06-08 16:34:50.000000 enformer_dna_diff-1.1/enformer_dna_diff/main_script.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    11745 2023-06-09 14:09:05.000000 enformer_dna_diff-1.1/enformer_dna_diff/real_main_script.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2511 2023-06-25 15:13:07.000000 enformer_dna_diff-1.1/enformer_dna_diff/utils.py
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:13:45.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/PKG-INFO
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      433 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/SOURCES.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)        1 2023-06-25 15:13:45.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/dependency_links.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2409 2023-06-25 15:13:45.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/requires.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       18 2023-06-25 15:13:45.000000 enformer_dna_diff-1.1/enformer_dna_diff.egg-info/top_level.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2013 2023-06-09 23:02:20.000000 enformer_dna_diff-1.1/get_data.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       38 2023-06-25 15:13:46.000000 enformer_dna_diff-1.1/setup.cfg
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      554 2023-06-25 15:12:38.000000 enformer_dna_diff-1.1/setup.py
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1063 2023-06-10 15:19:31.000000 enformer_dna_diff-1.2/LICENSE
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/PKG-INFO
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1707 2023-06-10 15:19:19.000000 enformer_dna_diff-1.2/README.md
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       43 2023-06-09 23:02:20.000000 enformer_dna_diff-1.2/enformer_dna_diff/__init__.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     3851 2023-06-09 23:02:20.000000 enformer_dna_diff-1.2/enformer_dna_diff/enformer.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    12998 2023-06-25 15:31:15.000000 enformer_dna_diff-1.2/enformer_dna_diff/enformerops.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    33364 2023-06-08 16:34:50.000000 enformer_dna_diff-1.2/enformer_dna_diff/main_script.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    11745 2023-06-09 14:09:05.000000 enformer_dna_diff-1.2/enformer_dna_diff/real_main_script.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2511 2023-06-25 15:31:19.000000 enformer_dna_diff-1.2/enformer_dna_diff/utils.py
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/PKG-INFO
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      433 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)        1 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2383 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/requires.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       18 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/enformer_dna_diff.egg-info/top_level.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2013 2023-06-09 23:02:20.000000 enformer_dna_diff-1.2/get_data.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       38 2023-06-25 15:32:23.000000 enformer_dna_diff-1.2/setup.cfg
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      554 2023-06-25 15:31:26.000000 enformer_dna_diff-1.2/setup.py
```

### Comparing `enformer_dna_diff-1.1/LICENSE` & `enformer_dna_diff-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.1/README.md` & `enformer_dna_diff-1.2/README.md`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.1/enformer_dna_diff/enformer.py` & `enformer_dna_diff-1.2/enformer_dna_diff/enformer.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.1/enformer_dna_diff/enformerops.py` & `enformer_dna_diff-1.2/enformer_dna_diff/enformerops.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.1/enformer_dna_diff/main_script.py` & `enformer_dna_diff-1.2/enformer_dna_diff/main_script.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.1/enformer_dna_diff/real_main_script.py` & `enformer_dna_diff-1.2/enformer_dna_diff/real_main_script.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.1/enformer_dna_diff/utils.py` & `enformer_dna_diff-1.2/enformer_dna_diff/utils.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.1/enformer_dna_diff.egg-info/requires.txt` & `enformer_dna_diff-1.2/enformer_dna_diff.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,45 +6,45 @@
 asttokens==2.2.1
 astunparse==1.6.3
 attrs==21.4.0
 backcall==0.2.0
 binaryornot==0.4.4
 cachetools==5.3.1
 certifi==2023.5.7
-chardet==5.1.0
-charset-normalizer==3.1.0
+chardet==4.0.0
+charset-normalizer==2.0.12
 click==8.1.3
 cloudpickle==2.2.1
 colorlog==6.7.0
 comm==0.1.3
 contourpy==1.1.0
 cookiecutter==2.1.1
 cycler==0.11.0
 debugpy==1.6.7
-decorator==5.1.1
+decorator==4.0.6
 deprecation==2.1.0
 dm-tree==0.1.8
 etils==1.3.0
 executing==1.2.0
 flatbuffers==23.5.26
 fonttools==4.40.0
 future==0.18.3
 gast==0.4.0
 gffutils==0.11.1
-google-auth==2.20.0
+google-auth==2.17.3
 google-auth-oauthlib==1.0.0
 google-pasta==0.2.0
 googleapis-common-protos==1.59.1
 grpcio==1.56.0
 h5py==3.9.0
 idna==3.4
 igv-notebook==0.5.2
 importlib-resources==5.12.0
-ipykernel==6.23.3
-ipython==8.14.0
+ipykernel==5.5.6
+ipython==7.34.0
 jax==0.4.13
 jedi==0.18.2
 Jinja2==3.1.2
 jinja2-time==0.2.0
 joblib==1.2.0
 jupyter_client==8.3.0
 jupyter_core==5.3.1
@@ -92,16 +92,15 @@
 pyranges==0.0.127
 python-dateutil==2.8.2
 python-slugify==8.0.1
 pytz==2023.3
 PyYAML==6.0
 pyzmq==25.1.0
 related==0.7.3
-requests==2.31.0
-requests-oauthlib==1.3.1
+requests==2.27.1
 rsa==4.9
 scipy==1.10.1
 seaborn==0.12.2
 simplejson==3.19.1
 six==1.16.0
 sorted-nearest==0.0.39
 stack-data==0.6.2
@@ -116,18 +115,18 @@
 tensorflow-io-gcs-filesystem==0.32.0
 tensorflow-metadata==1.13.1
 tensorflow-probability==0.20.1
 termcolor==2.3.0
 text-unidecode==1.3
 tinydb==4.8.0
 toml==0.10.2
-tornado==6.3.2
+tornado==6.3.1
 tqdm==4.65.0
 traitlets==5.9.0
 typing_extensions==4.6.3
 tzdata==2023.3
-urllib3==1.26.16
+urllib3==1.24.3
 wcwidth==0.2.6
 Werkzeug==2.3.6
 wget==3.2
 wrapt==1.14.1
 zipp==3.15.0
```

### Comparing `enformer_dna_diff-1.1/get_data.py` & `enformer_dna_diff-1.2/get_data.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.1/setup.py` & `enformer_dna_diff-1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required_libraries = f.read().splitlines()
 # import ipdb;ipdb.set_trace()
 setup(
     name="enformer_dna_diff",
-    version="1.1",
+    version="1.2",
     packages=find_packages(),
     install_requires=required_libraries,
     scripts=['get_data.py'],
     author="Tin M. Tunjic",
     author_email="tunjictin@gmail.com",
     description="This is a package for that combines DeepMind Enformer model with DNA Diffusion project",
     url="https://github.com/ttunja/Enformer_DNA_Diffusion.git"
```

