# Comparing `tmp/pydlutils-0.0.1.tar.gz` & `tmp/pydlutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydlutils-0.0.1.tar", last modified: Fri Jun 16 11:26:49 2023, max compression
+gzip compressed data, was "pydlutils-0.0.2.tar", last modified: Sun Jun 25 10:43:57 2023, max compression
```

## Comparing `pydlutils-0.0.1.tar` & `pydlutils-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
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
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:43:57.843368 pydlutils-0.0.2/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1964 2023-06-25 10:43:57.843368 pydlutils-0.0.2/PKG-INFO
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      796 2023-06-16 11:56:23.000000 pydlutils-0.0.2/README.md
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:43:57.839368 pydlutils-0.0.2/pydlutils/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 10:29:03.000000 pydlutils-0.0.2/pydlutils/__init__.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:43:57.843368 pydlutils-0.0.2/pydlutils/basic/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.2/pydlutils/basic/__init__.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1802 2023-06-16 11:56:23.000000 pydlutils-0.0.2/pydlutils/basic/registry.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1746 2023-06-16 11:56:23.000000 pydlutils-0.0.2/pydlutils/basic/yaml.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:43:57.843368 pydlutils-0.0.2/pydlutils/thirdparty/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.2/pydlutils/thirdparty/__init__.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:43:57.843368 pydlutils-0.0.2/pydlutils/torch/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.2/pydlutils/torch/__init__.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      355 2023-06-16 11:56:23.000000 pydlutils-0.0.2/pydlutils/torch/registry.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      645 2023-06-16 11:56:23.000000 pydlutils-0.0.2/pydlutils/torch/seed.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:43:57.843368 pydlutils-0.0.2/pydlutils.egg-info/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1964 2023-06-25 10:43:57.000000 pydlutils-0.0.2/pydlutils.egg-info/PKG-INFO
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      397 2023-06-25 10:43:57.000000 pydlutils-0.0.2/pydlutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        1 2023-06-25 10:43:57.000000 pydlutils-0.0.2/pydlutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       31 2023-06-25 10:43:57.000000 pydlutils-0.0.2/pydlutils.egg-info/requires.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       10 2023-06-25 10:43:57.000000 pydlutils-0.0.2/pydlutils.egg-info/top_level.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       38 2023-06-25 10:43:57.843368 pydlutils-0.0.2/setup.cfg
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1965 2023-06-25 10:43:14.000000 pydlutils-0.0.2/setup.py
```

### Comparing `pydlutils-0.0.1/PKG-INFO` & `pydlutils-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlutils
-Version: 0.0.1
+Version: 0.0.2
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

### Comparing `pydlutils-0.0.1/README.md` & `pydlutils-0.0.2/README.md`

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

### Comparing `pydlutils-0.0.1/pydlutils/basic/registry.py` & `pydlutils-0.0.2/pydlutils/basic/registry.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.1/pydlutils/basic/yaml.py` & `pydlutils-0.0.2/pydlutils/basic/yaml.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.1/pydlutils.egg-info/PKG-INFO` & `pydlutils-0.0.2/pydlutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlutils
-Version: 0.0.1
+Version: 0.0.2
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

### Comparing `pydlutils-0.0.1/setup.py` & `pydlutils-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import os
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
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

