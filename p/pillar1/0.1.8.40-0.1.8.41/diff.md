# Comparing `tmp/pillar1-0.1.8.40.tar.gz` & `tmp/pillar1-0.1.8.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.40.tar", last modified: Sun Jun 25 02:13:48 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.41.tar", last modified: Sun Jun 25 02:16:47 2023, max compression
```

## Comparing `pillar1-0.1.8.40.tar` & `pillar1-0.1.8.41.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:13:48.114672 pillar1-0.1.8.40/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 02:13:48.114534 pillar1-0.1.8.40/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.40/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:13:48.113615 pillar1-0.1.8.40/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.40/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.40/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.40/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     6500 2023-06-25 01:55:56.000000 pillar1-0.1.8.40/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:13:48.114338 pillar1-0.1.8.40/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 02:13:48.000000 pillar1-0.1.8.40/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 02:13:48.000000 pillar1-0.1.8.40/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 02:13:48.000000 pillar1-0.1.8.40/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 02:13:48.000000 pillar1-0.1.8.40/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 02:13:48.114719 pillar1-0.1.8.40/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 02:13:47.000000 pillar1-0.1.8.40/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:16:47.256267 pillar1-0.1.8.41/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 02:16:47.256144 pillar1-0.1.8.41/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.41/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:16:47.255452 pillar1-0.1.8.41/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.41/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.41/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.41/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     6644 2023-06-25 02:16:45.000000 pillar1-0.1.8.41/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:16:47.255956 pillar1-0.1.8.41/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 02:16:47.000000 pillar1-0.1.8.41/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 02:16:47.000000 pillar1-0.1.8.41/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 02:16:47.000000 pillar1-0.1.8.41/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 02:16:47.000000 pillar1-0.1.8.41/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 02:16:47.256307 pillar1-0.1.8.41/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 02:16:46.000000 pillar1-0.1.8.41/setup.py
```

### Comparing `pillar1-0.1.8.40/PKG-INFO` & `pillar1-0.1.8.41/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.40
+Version: 0.1.8.41
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.40/README.md` & `pillar1-0.1.8.41/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.40/pillar1/constants.py` & `pillar1-0.1.8.41/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.40/pillar1/constants_original.py` & `pillar1-0.1.8.41/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.40/pillar1/pillar1.py` & `pillar1-0.1.8.41/pillar1/pillar1.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,19 +78,25 @@
         self.cleaned_code = self.response.replace(self.prompt, '').strip()
         ELS_TO_REMOVE = ['<pre>', '<code>', '</code>', '</pre>']
         for curr_el_to_remove in ELS_TO_REMOVE:
             self.cleaned_code = self.cleaned_code.replace(curr_el_to_remove, '')
 
         placeholder_beg = self.curr_model.get('placeholder_beg')
         if placeholder_beg:
-            self.cleaned_code = self.cleaned_code.split(placeholder_beg['pattern'])[placeholder_beg['index']]
+            try:
+                self.cleaned_code = self.cleaned_code.split(placeholder_beg['pattern'])[placeholder_beg['index']]
+            except Exception:
+                pass
 
         placeholder_end = self.curr_model.get('placeholder_end')
         if placeholder_end:
-            self.cleaned_code = self.cleaned_code.split(placeholder_end['pattern'])[placeholder_end['index']]
+            try:
+                self.cleaned_code = self.cleaned_code.split(placeholder_end['pattern'])[placeholder_end['index']]
+            except Exception:
+                pass
 
         # self.cleaned_code = self.cleaned_code.split('<|assistant|>')[1].split('<|end|>')[0].strip().replace(' claim_item;', ' uc_beesbridge.abacus.claim_item;').replace(
         #    ' claim_item ',
         #    ' uc_beesbridge.abacus.claim_item ').replace(
         #    ' claim_item\n', ' uc_beesbridge.abacus.claim_item\n')
 
         self.cleaned_code = self.cleaned_code.strip()
```

### Comparing `pillar1-0.1.8.40/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.41/pillar1.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.40
+Version: 0.1.8.41
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.40/setup.py` & `pillar1-0.1.8.41/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.40',
+    version='0.1.8.41',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

