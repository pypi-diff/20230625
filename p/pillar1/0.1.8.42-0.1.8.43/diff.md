# Comparing `tmp/pillar1-0.1.8.42.tar.gz` & `tmp/pillar1-0.1.8.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.42.tar", last modified: Sun Jun 25 02:28:32 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.43.tar", last modified: Sun Jun 25 02:42:38 2023, max compression
```

## Comparing `pillar1-0.1.8.42.tar` & `pillar1-0.1.8.43.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:28:32.601556 pillar1-0.1.8.42/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 02:28:32.601424 pillar1-0.1.8.42/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.42/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:28:32.600687 pillar1-0.1.8.42/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.42/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.42/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.42/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     6644 2023-06-25 02:28:27.000000 pillar1-0.1.8.42/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:28:32.601236 pillar1-0.1.8.42/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 02:28:32.000000 pillar1-0.1.8.42/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 02:28:32.000000 pillar1-0.1.8.42/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 02:28:32.000000 pillar1-0.1.8.42/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 02:28:32.000000 pillar1-0.1.8.42/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 02:28:32.601599 pillar1-0.1.8.42/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 02:28:32.000000 pillar1-0.1.8.42/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:42:38.746700 pillar1-0.1.8.43/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 02:42:38.746560 pillar1-0.1.8.43/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.43/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:42:38.745704 pillar1-0.1.8.43/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.43/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.43/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.43/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     6561 2023-06-25 02:42:12.000000 pillar1-0.1.8.43/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:42:38.746343 pillar1-0.1.8.43/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 02:42:38.000000 pillar1-0.1.8.43/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 02:42:38.000000 pillar1-0.1.8.43/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 02:42:38.000000 pillar1-0.1.8.43/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 02:42:38.000000 pillar1-0.1.8.43/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 02:42:38.746745 pillar1-0.1.8.43/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 02:42:38.000000 pillar1-0.1.8.43/setup.py
```

### Comparing `pillar1-0.1.8.42/PKG-INFO` & `pillar1-0.1.8.43/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.42
+Version: 0.1.8.43
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.42/README.md` & `pillar1-0.1.8.43/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.42/pillar1/constants.py` & `pillar1-0.1.8.43/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.42/pillar1/constants_original.py` & `pillar1-0.1.8.43/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.42/pillar1/pillar1.py` & `pillar1-0.1.8.43/pillar1/pillar1.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,35 +5,44 @@
 import requests
 
 
 class MODELS:
     STARCODERPLUS = 'starcoderplus'
     STARCHAT_BETA = 'starchat-beta'
     FALCON_40B_INSTRUCT = 'f40b-instruct'
+    FALCON_40B = 'f40b'
 
 
 MODELS_META = {
     'f40b-instruct': {
         'stop_token': '<|endoftext|>'
     },
+    'f40b': {
+        'free': {
+            'prepend': 'Given this `claims` table description:',
+            'stop_token': '<|endoftext|>'
+        },
+        'hosted': {
+            'prepend': 'Given this `claims` table description:',
+            'stop_token': '<|endoftext|>'
+        }
+    },
     'starcoderplus': {
         'free': {
             'prepend': 'Given this `claims` table description:',
             'append': '',
             'stop_token': '<|end|>',
             'API_URL': 'https://api-inference.huggingface.co/models/bigcode/starcoderplus',
-            'replaces': {'': '', },
             'placeholder_beg': {'pattern': '```sql', 'index': 1},
             'placeholder_end': {'pattern': '```', 'index': 0}
         },
         'hosted': {
             'prepend': 'Given this `claims` table description:',
             'append': '',
             'stop_token': '<|end|>',
-            'replaces': {'': '', },
             'placeholder_beg': {'pattern': '```sql', 'index': 1},
             'placeholder_end': {'pattern': '```', 'index': 0}
         }
     },
     'starchat-beta': {
         'free': {
             'prepend': '<|user|>Given this `claims` table description:',
@@ -90,19 +99,14 @@
             except Exception:
                 pass
 
         ELS_TO_REMOVE = ['<pre>', '<code>', '</code>', '</pre>']
         for curr_el_to_remove in ELS_TO_REMOVE:
             self.cleaned_code = self.cleaned_code.replace(curr_el_to_remove, '')
 
-        # self.cleaned_code = self.cleaned_code.split('<|assistant|>')[1].split('<|end|>')[0].strip().replace(' claim_item;', ' uc_beesbridge.abacus.claim_item;').replace(
-        #    ' claim_item ',
-        #    ' uc_beesbridge.abacus.claim_item ').replace(
-        #    ' claim_item\n', ' uc_beesbridge.abacus.claim_item\n')
-
         self.cleaned_code = self.cleaned_code.strip()
         print(self.cleaned_code)
 
     def execute(self):
         spark = SparkSession.builder.getOrCreate()
         self.result = spark.sql(self.cleaned_code)
         return self.result
```

### Comparing `pillar1-0.1.8.42/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.43/pillar1.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.42
+Version: 0.1.8.43
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.42/setup.py` & `pillar1-0.1.8.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.42',
+    version='0.1.8.43',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

