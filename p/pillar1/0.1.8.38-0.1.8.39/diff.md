# Comparing `tmp/pillar1-0.1.8.38.tar.gz` & `tmp/pillar1-0.1.8.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.38.tar", last modified: Sun Jun 25 01:34:02 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.39.tar", last modified: Sun Jun 25 01:41:08 2023, max compression
```

## Comparing `pillar1-0.1.8.38.tar` & `pillar1-0.1.8.39.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:34:02.354701 pillar1-0.1.8.38/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:34:02.354520 pillar1-0.1.8.38/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.38/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:34:02.353607 pillar1-0.1.8.38/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.38/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.38/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.38/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     5631 2023-06-25 01:34:00.000000 pillar1-0.1.8.38/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:34:02.354278 pillar1-0.1.8.38/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:34:02.000000 pillar1-0.1.8.38/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 01:34:02.000000 pillar1-0.1.8.38/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 01:34:02.000000 pillar1-0.1.8.38/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 01:34:02.000000 pillar1-0.1.8.38/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 01:34:02.354752 pillar1-0.1.8.38/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 01:34:02.000000 pillar1-0.1.8.38/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:41:08.594061 pillar1-0.1.8.39/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:41:08.593919 pillar1-0.1.8.39/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.39/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:41:08.593160 pillar1-0.1.8.39/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.39/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.39/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.39/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     6168 2023-06-25 01:41:00.000000 pillar1-0.1.8.39/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:41:08.593719 pillar1-0.1.8.39/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:41:08.000000 pillar1-0.1.8.39/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 01:41:08.000000 pillar1-0.1.8.39/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 01:41:08.000000 pillar1-0.1.8.39/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 01:41:08.000000 pillar1-0.1.8.39/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 01:41:08.594103 pillar1-0.1.8.39/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 01:41:08.000000 pillar1-0.1.8.39/setup.py
```

### Comparing `pillar1-0.1.8.38/PKG-INFO` & `pillar1-0.1.8.39/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.38
+Version: 0.1.8.39
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.38/README.md` & `pillar1-0.1.8.39/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.38/pillar1/constants.py` & `pillar1-0.1.8.39/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.38/pillar1/constants_original.py` & `pillar1-0.1.8.39/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.38/pillar1/pillar1.py` & `pillar1-0.1.8.39/pillar1/pillar1.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     },
     'starcoderplus': {
         'free': {
             'prepend': 'Given this `claims` table description:',
             'append': '',
             'stop_token': '<|end|>',
             'API_URL': 'https://api-inference.huggingface.co/models/bigcode/starcoderplus',
-            'replaces': {'': '', }
+            'replaces': {'': '', },
+            'placeholder_beg': {'pattern': '```sql', 'index': 1},
+            'placeholder_end': {'pattern': '```', 'index': 0}
         }
     },
     'starchat-beta': {
         'free': {
             'prepend': '<|user|>Given this `claims` table description:',
             'append': '<|end|>',
             'stop_token': '<|end|>',
@@ -66,14 +68,22 @@
 
     def code(self):
         self.cleaned_code = self.response.replace(self.prompt, '').strip()
         ELS_TO_REMOVE = ['<pre>', '<code>', '</code>', '</pre>']
         for curr_el_to_remove in ELS_TO_REMOVE:
             self.cleaned_code = self.cleaned_code.replace(curr_el_to_remove, '')
 
+        placeholder_beg = self.curr_model.get('placeholder_beg')
+        if placeholder_beg:
+            self.cleaned_code = self.cleaned_code.split(placeholder_beg['pattern'])[placeholder_beg['index']]
+
+        placeholder_end = self.curr_model.get('placeholder_end')
+        if placeholder_end:
+            self.cleaned_code = self.cleaned_code.split(placeholder_end['pattern'])[placeholder_end['index']]
+
         # self.cleaned_code = self.cleaned_code.split('<|assistant|>')[1].split('<|end|>')[0].strip().replace(' claim_item;', ' uc_beesbridge.abacus.claim_item;').replace(
         #    ' claim_item ',
         #    ' uc_beesbridge.abacus.claim_item ').replace(
         #    ' claim_item\n', ' uc_beesbridge.abacus.claim_item\n')
 
         self.cleaned_code = self.cleaned_code.strip()
         print(self.cleaned_code)
```

### Comparing `pillar1-0.1.8.38/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.39/pillar1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.38
+Version: 0.1.8.39
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.38/setup.py` & `pillar1-0.1.8.39/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.38',
+    version='0.1.8.39',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

