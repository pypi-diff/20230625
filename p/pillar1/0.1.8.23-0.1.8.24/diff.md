# Comparing `tmp/pillar1-0.1.8.23.tar.gz` & `tmp/pillar1-0.1.8.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.23.tar", last modified: Sun Jun 25 00:11:16 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.24.tar", last modified: Sun Jun 25 00:13:07 2023, max compression
```

## Comparing `pillar1-0.1.8.23.tar` & `pillar1-0.1.8.24.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:11:16.461077 pillar1-0.1.8.23/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:11:16.460925 pillar1-0.1.8.23/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.23/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:11:16.459968 pillar1-0.1.8.23/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.23/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2249 2023-06-23 19:09:33.000000 pillar1-0.1.8.23/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.23/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     4857 2023-06-24 23:46:09.000000 pillar1-0.1.8.23/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:11:16.460698 pillar1-0.1.8.23/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:11:16.000000 pillar1-0.1.8.23/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 00:11:16.000000 pillar1-0.1.8.23/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 00:11:16.000000 pillar1-0.1.8.23/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 00:11:16.000000 pillar1-0.1.8.23/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 00:11:16.461138 pillar1-0.1.8.23/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 00:11:16.000000 pillar1-0.1.8.23/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:13:07.337143 pillar1-0.1.8.24/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:13:07.337029 pillar1-0.1.8.24/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.24/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:13:07.336381 pillar1-0.1.8.24/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.24/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2249 2023-06-23 19:09:33.000000 pillar1-0.1.8.24/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.24/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     4922 2023-06-25 00:13:04.000000 pillar1-0.1.8.24/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:13:07.336853 pillar1-0.1.8.24/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:13:07.000000 pillar1-0.1.8.24/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 00:13:07.000000 pillar1-0.1.8.24/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 00:13:07.000000 pillar1-0.1.8.24/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 00:13:07.000000 pillar1-0.1.8.24/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 00:13:07.337185 pillar1-0.1.8.24/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 00:13:07.000000 pillar1-0.1.8.24/setup.py
```

### Comparing `pillar1-0.1.8.23/PKG-INFO` & `pillar1-0.1.8.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.23
+Version: 0.1.8.24
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.23/README.md` & `pillar1-0.1.8.24/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.23/pillar1/constants.py` & `pillar1-0.1.8.24/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.23/pillar1/constants_original.py` & `pillar1-0.1.8.24/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.23/pillar1/pillar1.py` & `pillar1-0.1.8.24/pillar1/pillar1.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     },
     'starchat-beta': {
         'free': {
             'context': cn.STARCODER_BETA,
             'prepend': '<|user|>Given this `claim_item` table description:',
             'append': '(only return DataBricks-compatible SQL code)<|end|>',
             'stop_token': '<|end|>',
-            'API_URL': '',
+            'API_URL': 'https://api-inference.huggingface.co/models/bigcode/starcoderplus',
             'replaces': {'': '', }
         }
     }
 }
 
 
 class Model:
```

### Comparing `pillar1-0.1.8.23/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.24/pillar1.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.23
+Version: 0.1.8.24
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.23/setup.py` & `pillar1-0.1.8.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.23',
+    version='0.1.8.24',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

