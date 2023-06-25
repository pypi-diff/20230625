# Comparing `tmp/testless_autocomplete-0.0.114.tar.gz` & `tmp/testless_autocomplete-0.0.115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_autocomplete-0.0.114.tar", last modified: Sun Jun 25 20:30:07 2023, max compression
+gzip compressed data, was "testless_autocomplete-0.0.115.tar", last modified: Sun Jun 25 21:10:12 2023, max compression
```

## Comparing `testless_autocomplete-0.0.114.tar` & `testless_autocomplete-0.0.115.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 20:30:07.052637 testless_autocomplete-0.0.114/
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 20:30:07.049120 testless_autocomplete-0.0.114/Auto_Complete/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-22 21:16:29.000000 testless_autocomplete-0.0.114/Auto_Complete/__init__.py
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 20:30:07.050545 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      553 2023-06-25 20:19:23.000000 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/AutoCompleteAPI.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      184 2023-06-25 20:08:40.000000 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/__init__.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)     1262 2023-06-22 21:50:10.000000 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/model.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-22 21:40:11.000000 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/ngram.csv
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      756 2023-06-22 21:39:36.000000 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/preprocessing.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       54 2023-06-25 20:27:59.000000 testless_autocomplete-0.0.114/MANIFEST.in
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      337 2023-06-25 20:30:07.052432 testless_autocomplete-0.0.114/PKG-INFO
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 20:30:07.052684 testless_autocomplete-0.0.114/setup.cfg
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      809 2023-06-25 20:30:01.000000 testless_autocomplete-0.0.114/setup.py
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 20:30:07.052138 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      337 2023-06-25 20:30:06.000000 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/PKG-INFO
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      517 2023-06-25 20:30:07.000000 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/SOURCES.txt
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        1 2023-06-25 20:30:06.000000 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/dependency_links.txt
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       45 2023-06-25 20:30:06.000000 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/requires.txt
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       14 2023-06-25 20:30:06.000000 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/top_level.txt
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 21:10:12.407964 testless_autocomplete-0.0.115/
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 21:10:12.403946 testless_autocomplete-0.0.115/Auto_Complete/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-22 21:16:29.000000 testless_autocomplete-0.0.115/Auto_Complete/__init__.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 21:10:12.405803 testless_autocomplete-0.0.115/Auto_Complete/testless_autocomplete/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      560 2023-06-25 21:09:29.000000 testless_autocomplete-0.0.115/Auto_Complete/testless_autocomplete/AutoCompleteAPI.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      184 2023-06-25 20:08:40.000000 testless_autocomplete-0.0.115/Auto_Complete/testless_autocomplete/__init__.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)     1262 2023-06-22 21:50:10.000000 testless_autocomplete-0.0.115/Auto_Complete/testless_autocomplete/model.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-22 21:40:11.000000 testless_autocomplete-0.0.115/Auto_Complete/testless_autocomplete/ngram.csv
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      756 2023-06-22 21:39:36.000000 testless_autocomplete-0.0.115/Auto_Complete/testless_autocomplete/preprocessing.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       54 2023-06-25 20:27:59.000000 testless_autocomplete-0.0.115/MANIFEST.in
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      337 2023-06-25 21:10:12.407478 testless_autocomplete-0.0.115/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 21:10:12.408098 testless_autocomplete-0.0.115/setup.cfg
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      809 2023-06-25 21:10:00.000000 testless_autocomplete-0.0.115/setup.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 21:10:12.407237 testless_autocomplete-0.0.115/testless_autocomplete.egg-info/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      337 2023-06-25 21:10:12.000000 testless_autocomplete-0.0.115/testless_autocomplete.egg-info/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      517 2023-06-25 21:10:12.000000 testless_autocomplete-0.0.115/testless_autocomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        1 2023-06-25 21:10:12.000000 testless_autocomplete-0.0.115/testless_autocomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       45 2023-06-25 21:10:12.000000 testless_autocomplete-0.0.115/testless_autocomplete.egg-info/requires.txt
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       14 2023-06-25 21:10:12.000000 testless_autocomplete-0.0.115/testless_autocomplete.egg-info/top_level.txt
```

### Comparing `testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/AutoCompleteAPI.py` & `testless_autocomplete-0.0.115/Auto_Complete/testless_autocomplete/AutoCompleteAPI.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from .preprocessing import preprocess_text
 import pandas as pd
-
+import os
 
 def autocomplete(text):
     # if text is empty or contains only spaces, return an empty list
     try:
         if text == '':
             return {'words': []}
         words = preprocess_text(text)
-        # with autocomplete.app_context():
-        data = pd.read_csv('Auto_Complete/testless_autocomplete/ngram.csv')
-
+        
+        datapath = os.path.join(os.path.dirname(__file__), 'ngram.csv')
+        data = pd.read_csv(datapath)
 
         data.set_index('ngram', inplace=True)
         return {'words': data.loc[words[-1]]['next_word']} 
     except:
         print("Error")
         return {'words': []}
```

### Comparing `testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/model.py` & `testless_autocomplete-0.0.115/Auto_Complete/testless_autocomplete/model.py`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/ngram.csv` & `testless_autocomplete-0.0.115/Auto_Complete/testless_autocomplete/ngram.csv`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/preprocessing.py` & `testless_autocomplete-0.0.115/Auto_Complete/testless_autocomplete/preprocessing.py`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.114/setup.py` & `testless_autocomplete-0.0.115/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("Auto_Complete/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="testless_autocomplete",
-    version="0.0.114",
+    version="0.0.115",
     description="Auto Complete Package",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="TestLess",
     package_data={
         '/Auto_Complete': ['/testless_autocomplete/ngram.csv'],
```

### Comparing `testless_autocomplete-0.0.114/testless_autocomplete.egg-info/SOURCES.txt` & `testless_autocomplete-0.0.115/testless_autocomplete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

