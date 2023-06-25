# Comparing `tmp/enformer_dna_diff-1.3.tar.gz` & `tmp/enformer_dna_diff-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enformer_dna_diff-1.3.tar", last modified: Sun Jun 25 15:43:58 2023, max compression
+gzip compressed data, was "enformer_dna_diff-1.4.tar", last modified: Sun Jun 25 16:28:17 2023, max compression
```

## Comparing `enformer_dna_diff-1.3.tar` & `enformer_dna_diff-1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1063 2023-06-10 15:19:31.000000 enformer_dna_diff-1.3/LICENSE
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/PKG-INFO
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1707 2023-06-10 15:19:19.000000 enformer_dna_diff-1.3/README.md
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       43 2023-06-09 23:02:20.000000 enformer_dna_diff-1.3/enformer_dna_diff/__init__.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     3851 2023-06-09 23:02:20.000000 enformer_dna_diff-1.3/enformer_dna_diff/enformer.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    12998 2023-06-25 15:42:54.000000 enformer_dna_diff-1.3/enformer_dna_diff/enformerops.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    33364 2023-06-08 16:34:50.000000 enformer_dna_diff-1.3/enformer_dna_diff/main_script.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    11745 2023-06-09 14:09:05.000000 enformer_dna_diff-1.3/enformer_dna_diff/real_main_script.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2511 2023-06-25 15:42:57.000000 enformer_dna_diff-1.3/enformer_dna_diff/utils.py
-drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/PKG-INFO
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      433 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/SOURCES.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)        1 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/dependency_links.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2381 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/requires.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       18 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/enformer_dna_diff.egg-info/top_level.txt
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2013 2023-06-09 23:02:20.000000 enformer_dna_diff-1.3/get_data.py
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       38 2023-06-25 15:43:58.000000 enformer_dna_diff-1.3/setup.cfg
--rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      554 2023-06-25 15:42:45.000000 enformer_dna_diff-1.3/setup.py
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 16:28:17.000000 enformer_dna_diff-1.4/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1063 2023-06-10 15:19:31.000000 enformer_dna_diff-1.4/LICENSE
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 16:28:17.000000 enformer_dna_diff-1.4/PKG-INFO
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     1707 2023-06-10 15:19:19.000000 enformer_dna_diff-1.4/README.md
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 16:28:17.000000 enformer_dna_diff-1.4/enformer_dna_diff/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       43 2023-06-09 23:02:20.000000 enformer_dna_diff-1.4/enformer_dna_diff/__init__.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     3851 2023-06-09 23:02:20.000000 enformer_dna_diff-1.4/enformer_dna_diff/enformer.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    12998 2023-06-25 15:42:54.000000 enformer_dna_diff-1.4/enformer_dna_diff/enformerops.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    33364 2023-06-08 16:34:50.000000 enformer_dna_diff-1.4/enformer_dna_diff/main_script.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)    11745 2023-06-09 14:09:05.000000 enformer_dna_diff-1.4/enformer_dna_diff/real_main_script.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2511 2023-06-25 15:42:57.000000 enformer_dna_diff-1.4/enformer_dna_diff/utils.py
+drwxr-xr-x   0 tinmtunjic (424494613) Domain Users (424400513)        0 2023-06-25 16:28:17.000000 enformer_dna_diff-1.4/enformer_dna_diff.egg-info/
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      297 2023-06-25 16:28:17.000000 enformer_dna_diff-1.4/enformer_dna_diff.egg-info/PKG-INFO
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      433 2023-06-25 16:28:17.000000 enformer_dna_diff-1.4/enformer_dna_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)        1 2023-06-25 16:28:17.000000 enformer_dna_diff-1.4/enformer_dna_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2283 2023-06-25 16:28:17.000000 enformer_dna_diff-1.4/enformer_dna_diff.egg-info/requires.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       18 2023-06-25 16:28:17.000000 enformer_dna_diff-1.4/enformer_dna_diff.egg-info/top_level.txt
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)     2013 2023-06-09 23:02:20.000000 enformer_dna_diff-1.4/get_data.py
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)       38 2023-06-25 16:28:17.000000 enformer_dna_diff-1.4/setup.cfg
+-rw-r--r--   0 tinmtunjic (424494613) Domain Users (424400513)      554 2023-06-25 16:27:45.000000 enformer_dna_diff-1.4/setup.py
```

### Comparing `enformer_dna_diff-1.3/LICENSE` & `enformer_dna_diff-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.3/README.md` & `enformer_dna_diff-1.4/README.md`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.3/enformer_dna_diff/enformer.py` & `enformer_dna_diff-1.4/enformer_dna_diff/enformer.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.3/enformer_dna_diff/enformerops.py` & `enformer_dna_diff-1.4/enformer_dna_diff/enformerops.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.3/enformer_dna_diff/main_script.py` & `enformer_dna_diff-1.4/enformer_dna_diff/main_script.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.3/enformer_dna_diff/real_main_script.py` & `enformer_dna_diff-1.4/enformer_dna_diff/real_main_script.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.3/enformer_dna_diff/utils.py` & `enformer_dna_diff-1.4/enformer_dna_diff/utils.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.3/enformer_dna_diff.egg-info/requires.txt` & `enformer_dna_diff-1.4/enformer_dna_diff.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 absl-py==1.4.0
 argcomplete==3.1.1
 argh==0.28.1
-array-record==0.4.0
+array-record==0.3.0
 arrow==1.2.3
 asttokens==2.2.1
 astunparse==1.6.3
 attrs==21.4.0
 backcall==0.2.0
 binaryornot==0.4.4
 cachetools==5.3.1
@@ -15,118 +15,115 @@
 click==8.1.3
 cloudpickle==2.2.1
 colorlog==6.7.0
 comm==0.1.3
 contourpy==1.1.0
 cookiecutter==2.1.1
 cycler==0.11.0
-debugpy==1.6.7
-decorator==5.1.1
+debugpy==1.6.6
+decorator==4.4.2
 deprecation==2.1.0
 dm-tree==0.1.8
 etils==1.3.0
 executing==1.2.0
 flatbuffers==23.5.26
 fonttools==4.40.0
 future==0.18.3
 gast==0.4.0
 gffutils==0.11.1
 google-auth==2.17.3
 google-auth-oauthlib==1.0.0
 google-pasta==0.2.0
 googleapis-common-protos==1.59.1
-grpcio==1.56.0
-h5py==3.9.0
+grpcio==1.54.2
+h5py==3.8.0
 idna==3.4
 igv-notebook==0.5.2
 importlib-resources==5.12.0
 ipykernel==5.5.6
 ipython==7.34.0
-jax==0.4.13
+jax==0.4.10
 jedi==0.18.2
 Jinja2==3.1.2
 jinja2-time==0.2.0
 joblib==1.2.0
-jupyter_client==8.3.0
+jupyter-client==6.1.12
 jupyter_core==5.3.1
 keras==2.12.0
 kipoi==0.8.6
 kipoi-conda==0.3.1
 kipoi-utils==0.7.7
-kipoiseq==0.7.1
+kipoiseq==0.5.2
 kiwisolver==1.4.4
 libclang==16.0.0
 Markdown==3.4.3
 MarkupSafe==2.1.3
-matplotlib==3.6.3
+matplotlib==3.7.1
 matplotlib-inline==0.1.6
 ml-dtypes==0.2.0
-natsort==8.4.0
+natsort==8.3.1
 ncls==0.0.68
 nest-asyncio==1.5.6
 numpy==1.22.4
-nvidia-cublas-cu11==11.10.3.66
-nvidia-cuda-nvrtc-cu11==11.7.99
-nvidia-cuda-runtime-cu11==11.7.99
-nvidia-cudnn-cu11==8.5.0.96
 oauthlib==3.2.2
 opt-einsum==3.3.0
 packaging==23.1
 pandas==1.5.3
 parso==0.8.3
 pexpect==4.8.0
 pickleshare==0.7.5
-Pillow==9.5.0
-platformdirs==3.8.0
+Pillow==8.4.0
+platformdirs==3.7.0
 promise==2.3
 prompt-toolkit==3.0.38
-protobuf==4.23.3
+protobuf==3.20.3
 psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pyasn1==0.5.0
 pyasn1-modules==0.3.0
 pyBigWig==0.3.22
 pyfaidx==0.7.2.1
-Pygments==2.15.1
+Pygments==2.14.0
 pyparsing==3.1.0
 pyranges==0.0.127
 python-dateutil==2.8.2
 python-slugify==8.0.1
-pytz==2023.3
+pytz==2022.7.1
 PyYAML==6.0
-pyzmq==25.1.0
+pyzmq==23.2.1
 related==0.7.3
 requests==2.27.1
 rsa==4.9
 scipy==1.10.1
 seaborn==0.12.2
 simplejson==3.19.1
 six==1.16.0
 sorted-nearest==0.0.39
 stack-data==0.6.2
-tabulate==0.9.0
+tabulate==0.8.10
 tensorboard==2.12.3
-tensorboard-data-server==0.7.0
+tensorboard-data-server==0.7.1
 tensorflow==2.12.0
 tensorflow-datasets==4.9.2
 tensorflow-estimator==2.12.0
 tensorflow-gcs-config==2.12.0
 tensorflow-hub==0.13.0
 tensorflow-io-gcs-filesystem==0.32.0
 tensorflow-metadata==1.13.1
 tensorflow-probability==0.20.1
+tensorstore==0.1.38
 termcolor==2.3.0
 text-unidecode==1.3
 tinydb==4.8.0
 toml==0.10.2
 tornado==6.3.1
 tqdm==4.65.0
-traitlets==5.9.0
+traitlets==5.7.1
 typing_extensions==4.6.3
 tzdata==2023.3
-urllib3==1.25
+urllib3==1.26.16
 wcwidth==0.2.6
 Werkzeug==2.3.6
 wget==3.2
 wrapt==1.14.1
 zipp==3.15.0
```

### Comparing `enformer_dna_diff-1.3/get_data.py` & `enformer_dna_diff-1.4/get_data.py`

 * *Files identical despite different names*

### Comparing `enformer_dna_diff-1.3/setup.py` & `enformer_dna_diff-1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required_libraries = f.read().splitlines()
 # import ipdb;ipdb.set_trace()
 setup(
     name="enformer_dna_diff",
-    version="1.3",
+    version="1.4",
     packages=find_packages(),
     install_requires=required_libraries,
     scripts=['get_data.py'],
     author="Tin M. Tunjic",
     author_email="tunjictin@gmail.com",
     description="This is a package for that combines DeepMind Enformer model with DNA Diffusion project",
     url="https://github.com/ttunja/Enformer_DNA_Diffusion.git"
```

