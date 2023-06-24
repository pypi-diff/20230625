# Comparing `tmp/pillar1-0.1.8.20.tar.gz` & `tmp/pillar1-0.1.8.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.20.tar", last modified: Sat Jun 24 22:49:56 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.21.tar", last modified: Sat Jun 24 23:25:31 2023, max compression
```

## Comparing `pillar1-0.1.8.20.tar` & `pillar1-0.1.8.21.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 22:49:56.048370 pillar1-0.1.8.20/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-24 22:49:56.048255 pillar1-0.1.8.20/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.20/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 22:49:56.047510 pillar1-0.1.8.20/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.20/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2249 2023-06-23 19:09:33.000000 pillar1-0.1.8.20/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.20/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     4649 2023-06-24 22:49:47.000000 pillar1-0.1.8.20/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 22:49:56.048048 pillar1-0.1.8.20/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-24 22:49:56.000000 pillar1-0.1.8.20/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-24 22:49:56.000000 pillar1-0.1.8.20/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-24 22:49:56.000000 pillar1-0.1.8.20/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-24 22:49:56.000000 pillar1-0.1.8.20/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-24 22:49:56.048407 pillar1-0.1.8.20/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-24 22:49:55.000000 pillar1-0.1.8.20/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 23:25:31.818911 pillar1-0.1.8.21/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-24 23:25:31.818763 pillar1-0.1.8.21/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.21/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 23:25:31.817188 pillar1-0.1.8.21/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.21/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2249 2023-06-23 19:09:33.000000 pillar1-0.1.8.21/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.21/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     4621 2023-06-24 23:25:19.000000 pillar1-0.1.8.21/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 23:25:31.818560 pillar1-0.1.8.21/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-24 23:25:31.000000 pillar1-0.1.8.21/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-24 23:25:31.000000 pillar1-0.1.8.21/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-24 23:25:31.000000 pillar1-0.1.8.21/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-24 23:25:31.000000 pillar1-0.1.8.21/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-24 23:25:31.818957 pillar1-0.1.8.21/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-24 23:25:31.000000 pillar1-0.1.8.21/setup.py
```

### Comparing `pillar1-0.1.8.20/PKG-INFO` & `pillar1-0.1.8.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.20
+Version: 0.1.8.21
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.20/README.md` & `pillar1-0.1.8.21/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.20/pillar1/constants.py` & `pillar1-0.1.8.21/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.20/pillar1/constants_original.py` & `pillar1-0.1.8.21/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.20/pillar1/pillar1.py` & `pillar1-0.1.8.21/pillar1/pillar1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import boto3
 from pyspark.sql import SparkSession
 import pillar1.constants as cn
-from enum import Enum
 
 
-class MODELS(Enum):
+class MODELS:
     STARCHAT_BETA = 'starchat-beta'
     FALCON_40B_INSTRUCT = 'f40b-instruct'
 
 
 MODELS_META = {
     'f40b-instruct': {
         'context': '',
```

### Comparing `pillar1-0.1.8.20/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.21/pillar1.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.20
+Version: 0.1.8.21
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.20/setup.py` & `pillar1-0.1.8.21/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.20',
+    version='0.1.8.21',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

