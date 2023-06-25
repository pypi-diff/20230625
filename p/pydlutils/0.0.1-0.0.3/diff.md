# Comparing `tmp/pydlutils-0.0.1.tar.gz` & `tmp/pydlutils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydlutils-0.0.1.tar", last modified: Fri Jun 16 11:26:49 2023, max compression
+gzip compressed data, was "pydlutils-0.0.3.tar", last modified: Sun Jun 25 10:54:23 2023, max compression
```

## Comparing `pydlutils-0.0.1.tar` & `pydlutils-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,46 @@
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:26:49.417774 pydlutils-0.0.1/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1868 2023-06-16 11:26:49.417774 pydlutils-0.0.1/PKG-INFO
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      748 2023-06-16 11:19:25.000000 pydlutils-0.0.1/README.md
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:26:49.417774 pydlutils-0.0.1/pydlutils/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 10:29:03.000000 pydlutils-0.0.1/pydlutils/__init__.py
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:26:49.417774 pydlutils-0.0.1/pydlutils/basic/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 10:41:55.000000 pydlutils-0.0.1/pydlutils/basic/__init__.py
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1802 2023-06-16 10:29:03.000000 pydlutils-0.0.1/pydlutils/basic/registry.py
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1746 2023-06-16 10:35:20.000000 pydlutils-0.0.1/pydlutils/basic/yaml.py
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:26:49.417774 pydlutils-0.0.1/pydlutils/thirdparty/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 10:41:40.000000 pydlutils-0.0.1/pydlutils/thirdparty/__init__.py
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:26:49.417774 pydlutils-0.0.1/pydlutils/torch/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 10:41:26.000000 pydlutils-0.0.1/pydlutils/torch/__init__.py
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:26:49.417774 pydlutils-0.0.1/pydlutils.egg-info/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1868 2023-06-16 11:26:49.000000 pydlutils-0.0.1/pydlutils.egg-info/PKG-INFO
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      345 2023-06-16 11:26:49.000000 pydlutils-0.0.1/pydlutils.egg-info/SOURCES.txt
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        1 2023-06-16 11:26:49.000000 pydlutils-0.0.1/pydlutils.egg-info/dependency_links.txt
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       31 2023-06-16 11:26:49.000000 pydlutils-0.0.1/pydlutils.egg-info/requires.txt
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       10 2023-06-16 11:26:49.000000 pydlutils-0.0.1/pydlutils.egg-info/top_level.txt
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       38 2023-06-16 11:26:49.417774 pydlutils-0.0.1/setup.cfg
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     2085 2023-06-16 11:26:21.000000 pydlutils-0.0.1/setup.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:54:23.514193 pydlutils-0.0.3/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1964 2023-06-25 10:54:23.514193 pydlutils-0.0.3/PKG-INFO
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      796 2023-06-16 11:56:23.000000 pydlutils-0.0.3/README.md
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:54:23.506193 pydlutils-0.0.3/pydlutils/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/__init__.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:54:23.510193 pydlutils-0.0.3/pydlutils/basic/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.3/pydlutils/basic/__init__.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1802 2023-06-16 11:56:23.000000 pydlutils-0.0.3/pydlutils/basic/registry.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1746 2023-06-16 11:56:23.000000 pydlutils-0.0.3/pydlutils/basic/yaml.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:54:23.510193 pydlutils-0.0.3/pydlutils/thirdparty/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.3/pydlutils/thirdparty/__init__.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:54:23.514193 pydlutils-0.0.3/pydlutils/thirdparty/colmap/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:49:23.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/__init__.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    23189 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/build.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     3756 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/build_windows_app.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     4805 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/bundler_to_ply.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2644 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/clang_format_code.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     5449 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/crawl_camera_specs.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    12581 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/database.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     3430 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/export_inlier_matches.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     3237 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/export_inlier_pairs.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     6693 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/export_to_bundler.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     6570 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/export_to_visualsfm.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     6378 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/flickr_downloader.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2692 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/merge_ply_files.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     4817 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/nvm_to_ply.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    26202 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/plyfile.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     5222 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/read_write_dense.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     5069 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/read_write_fused_vis.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    21497 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/read_write_model.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2475 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/test_read_write_dense.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2686 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/test_read_write_fused_vis.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     4812 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/test_read_write_model.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     7090 2023-06-16 10:29:03.000000 pydlutils-0.0.3/pydlutils/thirdparty/colmap/visualize_model.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:54:23.514193 pydlutils-0.0.3/pydlutils/torch/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.3/pydlutils/torch/__init__.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      355 2023-06-16 11:56:23.000000 pydlutils-0.0.3/pydlutils/torch/registry.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      645 2023-06-16 11:56:23.000000 pydlutils-0.0.3/pydlutils/torch/seed.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:54:23.506193 pydlutils-0.0.3/pydlutils.egg-info/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1964 2023-06-25 10:54:23.000000 pydlutils-0.0.3/pydlutils.egg-info/PKG-INFO
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1447 2023-06-25 10:54:23.000000 pydlutils-0.0.3/pydlutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        1 2023-06-25 10:54:23.000000 pydlutils-0.0.3/pydlutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       31 2023-06-25 10:54:23.000000 pydlutils-0.0.3/pydlutils.egg-info/requires.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       10 2023-06-25 10:54:23.000000 pydlutils-0.0.3/pydlutils.egg-info/top_level.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       38 2023-06-25 10:54:23.514193 pydlutils-0.0.3/setup.cfg
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1965 2023-06-25 10:54:02.000000 pydlutils-0.0.3/setup.py
```

### Comparing `pydlutils-0.0.1/PKG-INFO` & `pydlutils-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlutils
-Version: 0.0.1
+Version: 0.0.3
 Summary: Utility library for deep learning
 Home-page: https://github.com/zebincai/pydlutils
 Author: zebincai
 Author-email: 1028798080@qq.com
 License: Apache
 Download-URL: https://github.com/zebincai/pydlutils/tags
 Description: # pydlutils
@@ -20,14 +20,20 @@
         
         2. third party
             place modules which come from other repositories.
         
         3. torch
             place torch related high level api.
         
+        ## Installation
+        
+        ```
+        pip install pydlutils
+        ```
+        
         ## Build and Upload
         ```
         # build
         python setup.py sdist bdist_wheel
         # upload
         twine upload dist/*
         ```
```

### Comparing `pydlutils-0.0.1/README.md` & `pydlutils-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 2. third party
     place modules which come from other repositories.
 
 3. torch
     place torch related high level api.
 
+## Installation
+
+```
+pip install pydlutils
+```
+
 ## Build and Upload
 ```
 # build
 python setup.py sdist bdist_wheel
 # upload
 twine upload dist/*
 ```
```

### Comparing `pydlutils-0.0.1/pydlutils/basic/registry.py` & `pydlutils-0.0.3/pydlutils/basic/registry.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.1/pydlutils/basic/yaml.py` & `pydlutils-0.0.3/pydlutils/basic/yaml.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.1/pydlutils.egg-info/PKG-INFO` & `pydlutils-0.0.3/pydlutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlutils
-Version: 0.0.1
+Version: 0.0.3
 Summary: Utility library for deep learning
 Home-page: https://github.com/zebincai/pydlutils
 Author: zebincai
 Author-email: 1028798080@qq.com
 License: Apache
 Download-URL: https://github.com/zebincai/pydlutils/tags
 Description: # pydlutils
@@ -20,14 +20,20 @@
         
         2. third party
             place modules which come from other repositories.
         
         3. torch
             place torch related high level api.
         
+        ## Installation
+        
+        ```
+        pip install pydlutils
+        ```
+        
         ## Build and Upload
         ```
         # build
         python setup.py sdist bdist_wheel
         # upload
         twine upload dist/*
         ```
```

### Comparing `pydlutils-0.0.1/setup.py` & `pydlutils-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import os
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.3'
 DESCRIPTION = 'Utility library for deep learning'
 
 
 def main():
-    cwd = os.path.dirname(os.path.abspath(__file__))
     INSTALL_REQUIRES = []
     DEPENDENCY_LINKS = []
 
-    # with open(f"{cwd}/requirements.txt", "r") as file:
     with open("./requirements.txt", "r") as file:
         for line in file.readlines():
             line = line.strip()
             if (not line) or line.startswith("#"):
                 continue
             if line.startswith("git+"):
                 DEPENDENCY_LINKS.append(line)
```

