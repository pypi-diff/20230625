# Comparing `tmp/pillar1-0.1.8.34.tar.gz` & `tmp/pillar1-0.1.8.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.34.tar", last modified: Sun Jun 25 01:03:19 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.35.tar", last modified: Sun Jun 25 01:04:38 2023, max compression
```

## Comparing `pillar1-0.1.8.34.tar` & `pillar1-0.1.8.35.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:03:19.152919 pillar1-0.1.8.34/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:03:19.152792 pillar1-0.1.8.34/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.34/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:03:19.152039 pillar1-0.1.8.34/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.34/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.34/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.34/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     5526 2023-06-25 01:03:17.000000 pillar1-0.1.8.34/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:03:19.152598 pillar1-0.1.8.34/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:03:19.000000 pillar1-0.1.8.34/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 01:03:19.000000 pillar1-0.1.8.34/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 01:03:19.000000 pillar1-0.1.8.34/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 01:03:19.000000 pillar1-0.1.8.34/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 01:03:19.152960 pillar1-0.1.8.34/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 01:03:18.000000 pillar1-0.1.8.34/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:04:38.479721 pillar1-0.1.8.35/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:04:38.479524 pillar1-0.1.8.35/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.35/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:04:38.478632 pillar1-0.1.8.35/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.35/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.35/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.35/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     5511 2023-06-25 01:04:36.000000 pillar1-0.1.8.35/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:04:38.479238 pillar1-0.1.8.35/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:04:38.000000 pillar1-0.1.8.35/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 01:04:38.000000 pillar1-0.1.8.35/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 01:04:38.000000 pillar1-0.1.8.35/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 01:04:38.000000 pillar1-0.1.8.35/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 01:04:38.479779 pillar1-0.1.8.35/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 01:04:38.000000 pillar1-0.1.8.35/setup.py
```

### Comparing `pillar1-0.1.8.34/PKG-INFO` & `pillar1-0.1.8.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.34
+Version: 0.1.8.35
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.34/README.md` & `pillar1-0.1.8.35/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.34/pillar1/constants.py` & `pillar1-0.1.8.35/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.34/pillar1/constants_original.py` & `pillar1-0.1.8.35/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.34/pillar1/pillar1.py` & `pillar1-0.1.8.35/pillar1/pillar1.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     'f40b-instruct': {
         'context': '',
         'stop_token': '<|endoftext|>'
     },
     'starcoderplus': {
         'free': {
             'context': cn.STARCODER_BETA,
-            'prepend': '<|user|>Given this `claims` table description:',
-            'append': '<|end|>',
+            'prepend': 'Given this `claims` table description:',
+            'append': '',
             'stop_token': '<|end|>',
             'API_URL': 'https://api-inference.huggingface.co/models/bigcode/starcoderplus',
             'replaces': {'': '', }
         }
     },
     'starchat-beta': {
         'free': {
```

### Comparing `pillar1-0.1.8.34/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.35/pillar1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.34
+Version: 0.1.8.35
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.34/setup.py` & `pillar1-0.1.8.35/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.34',
+    version='0.1.8.35',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

