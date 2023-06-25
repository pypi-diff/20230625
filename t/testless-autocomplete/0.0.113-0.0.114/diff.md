# Comparing `tmp/testless_autocomplete-0.0.113.tar.gz` & `tmp/testless_autocomplete-0.0.114.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_autocomplete-0.0.113.tar", last modified: Sun Jun 25 19:48:34 2023, max compression
+gzip compressed data, was "testless_autocomplete-0.0.114.tar", last modified: Sun Jun 25 20:30:07 2023, max compression
```

## Comparing `testless_autocomplete-0.0.113.tar` & `testless_autocomplete-0.0.114.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 19:48:34.953907 testless_autocomplete-0.0.113/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       36 2023-06-25 18:48:55.000000 testless_autocomplete-0.0.113/MANIFEST.in
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 19:48:34.953664 testless_autocomplete-0.0.113/PKG-INFO
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.113/README.md
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 19:48:34.953983 testless_autocomplete-0.0.113/setup.cfg
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      867 2023-06-25 19:47:44.000000 testless_autocomplete-0.0.113/setup.py
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 19:48:34.948380 testless_autocomplete-0.0.113/testless_autocomplete/
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 19:48:34.952971 testless_autocomplete-0.0.113/testless_autocomplete/src/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    15990 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.113/testless_autocomplete/src/AutoComplete.ipynb
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      591 2023-06-25 19:41:35.000000 testless_autocomplete-0.0.113/testless_autocomplete/src/AutoCompleteAPI.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.113/testless_autocomplete/src/__init__.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)     1262 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.113/testless_autocomplete/src/model.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.113/testless_autocomplete/src/ngram.csv
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      756 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.113/testless_autocomplete/src/preprocessing.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 20:30:07.052637 testless_autocomplete-0.0.114/
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 20:30:07.049120 testless_autocomplete-0.0.114/Auto_Complete/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-22 21:16:29.000000 testless_autocomplete-0.0.114/Auto_Complete/__init__.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 20:30:07.050545 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      553 2023-06-25 20:19:23.000000 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/AutoCompleteAPI.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      184 2023-06-25 20:08:40.000000 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/__init__.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)     1262 2023-06-22 21:50:10.000000 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/model.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-22 21:40:11.000000 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/ngram.csv
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      756 2023-06-22 21:39:36.000000 testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/preprocessing.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       54 2023-06-25 20:27:59.000000 testless_autocomplete-0.0.114/MANIFEST.in
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      337 2023-06-25 20:30:07.052432 testless_autocomplete-0.0.114/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 20:30:07.052684 testless_autocomplete-0.0.114/setup.cfg
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      809 2023-06-25 20:30:01.000000 testless_autocomplete-0.0.114/setup.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 20:30:07.052138 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      337 2023-06-25 20:30:06.000000 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      517 2023-06-25 20:30:07.000000 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        1 2023-06-25 20:30:06.000000 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       45 2023-06-25 20:30:06.000000 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/requires.txt
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       14 2023-06-25 20:30:06.000000 testless_autocomplete-0.0.114/testless_autocomplete.egg-info/top_level.txt
```

### Comparing `testless_autocomplete-0.0.113/setup.py` & `testless_autocomplete-0.0.114/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from setuptools import find_packages, setup
 
-with open("README.md", "r") as f:
+with open("Auto_Complete/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="testless_autocomplete",
-    version="0.0.113",
+    version="0.0.114",
     description="Auto Complete Package",
-    package_data={
-        '../Auto_Complete/': ['Auto_Complete/*'],
-    },
-    package_dir={"": "../Auto_Complete"},
-    packages=find_packages(where="../Auto_Complete"),
+    packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="TestLess",
-    zip_safe=False,
+    package_data={
+        '/Auto_Complete': ['/testless_autocomplete/ngram.csv'],
+    },
     include_package_data=True,
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
-    install_requires=["bson >= 0.5.10"],
+     install_requires=["bson >= 0.5.10"],
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
-    },
+    }
     
 )
```

### Comparing `testless_autocomplete-0.0.113/testless_autocomplete/src/AutoCompleteAPI.py` & `testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/AutoCompleteAPI.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from .preprocessing import preprocess_text
 import pandas as pd
 
 
 def autocomplete(text):
     # if text is empty or contains only spaces, return an empty list
     try:
-
         if text == '':
             return {'words': []}
         words = preprocess_text(text)
         # with autocomplete.app_context():
-        data = pd.read_csv('/Auto_Complete/Auto_Complete/testless_autocomplete/src/ngram.csv')
-        
-        print("HIIIII")
+        data = pd.read_csv('Auto_Complete/testless_autocomplete/ngram.csv')
+
 
-        data.set_index('ngram', inplace=True)        
+        data.set_index('ngram', inplace=True)
         return {'words': data.loc[words[-1]]['next_word']} 
     except:
+        print("Error")
         return {'words': []} 
-
```

### Comparing `testless_autocomplete-0.0.113/testless_autocomplete/src/model.py` & `testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/model.py`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.113/testless_autocomplete/src/ngram.csv` & `testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/ngram.csv`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.113/testless_autocomplete/src/preprocessing.py` & `testless_autocomplete-0.0.114/Auto_Complete/testless_autocomplete/preprocessing.py`

 * *Files identical despite different names*

