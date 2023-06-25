# Comparing `tmp/pillar1-0.1.8.27.tar.gz` & `tmp/pillar1-0.1.8.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.27.tar", last modified: Sun Jun 25 00:30:37 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.28.tar", last modified: Sun Jun 25 00:32:28 2023, max compression
```

## Comparing `pillar1-0.1.8.27.tar` & `pillar1-0.1.8.28.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:30:37.560905 pillar1-0.1.8.27/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:30:37.560764 pillar1-0.1.8.27/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.27/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:30:37.560016 pillar1-0.1.8.27/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.27/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2249 2023-06-23 19:09:33.000000 pillar1-0.1.8.27/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.27/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     5498 2023-06-25 00:30:34.000000 pillar1-0.1.8.27/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:30:37.560555 pillar1-0.1.8.27/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:30:37.000000 pillar1-0.1.8.27/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 00:30:37.000000 pillar1-0.1.8.27/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 00:30:37.000000 pillar1-0.1.8.27/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 00:30:37.000000 pillar1-0.1.8.27/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 00:30:37.560947 pillar1-0.1.8.27/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 00:30:37.000000 pillar1-0.1.8.27/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:32:28.070490 pillar1-0.1.8.28/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:32:28.070356 pillar1-0.1.8.28/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.28/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:32:28.069691 pillar1-0.1.8.28/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.28/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2249 2023-06-23 19:09:33.000000 pillar1-0.1.8.28/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.28/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     5477 2023-06-25 00:32:23.000000 pillar1-0.1.8.28/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:32:28.070180 pillar1-0.1.8.28/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:32:28.000000 pillar1-0.1.8.28/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 00:32:28.000000 pillar1-0.1.8.28/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 00:32:28.000000 pillar1-0.1.8.28/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 00:32:28.000000 pillar1-0.1.8.28/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 00:32:28.070532 pillar1-0.1.8.28/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 00:32:27.000000 pillar1-0.1.8.28/setup.py
```

### Comparing `pillar1-0.1.8.27/PKG-INFO` & `pillar1-0.1.8.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.27
+Version: 0.1.8.28
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.27/README.md` & `pillar1-0.1.8.28/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.27/pillar1/constants.py` & `pillar1-0.1.8.28/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.27/pillar1/constants_original.py` & `pillar1-0.1.8.28/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.27/pillar1/pillar1.py` & `pillar1-0.1.8.28/pillar1/pillar1.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     'f40b-instruct': {
         'context': '',
         'stop_token': '<|endoftext|>'
     },
     'starcoderplus': {
         'free': {
             'context': cn.STARCODER_BETA,
-            'prepend': '',  # '<|user|>Given this `claim_item` table description:',
-            'append': '',  # '(only return DataBricks-compatible SQL code)<|end|>',
-            'stop_token': '',  # '<|end|>',
+            'prepend': '<|user|>Given this `claim_item` table description:',
+            'append': '(only return DataBricks-compatible SQL code)<|end|>',
+            'stop_token': '<|end|>',
             'API_URL': 'https://api-inference.huggingface.co/models/bigcode/starcoderplus',
             'replaces': {'': '', }
         }
     },
     'starchat-beta': {
         'free': {
             'context': cn.STARCODER_BETA,
```

### Comparing `pillar1-0.1.8.27/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.28/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.27
+Version: 0.1.8.28
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.27/setup.py` & `pillar1-0.1.8.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.27',
+    version='0.1.8.28',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

