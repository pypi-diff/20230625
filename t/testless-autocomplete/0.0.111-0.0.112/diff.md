# Comparing `tmp/testless_autocomplete-0.0.111.tar.gz` & `tmp/testless_autocomplete-0.0.112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_autocomplete-0.0.111.tar", last modified: Sun Jun 25 18:49:20 2023, max compression
+gzip compressed data, was "testless_autocomplete-0.0.112.tar", last modified: Sun Jun 25 19:23:08 2023, max compression
```

## Comparing `testless_autocomplete-0.0.111.tar` & `testless_autocomplete-0.0.112.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:49:20.791819 testless_autocomplete-0.0.111/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       36 2023-06-25 18:48:55.000000 testless_autocomplete-0.0.111/MANIFEST.in
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 18:49:20.791547 testless_autocomplete-0.0.111/PKG-INFO
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.111/README.md
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 18:49:20.791865 testless_autocomplete-0.0.111/setup.cfg
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      894 2023-06-25 18:49:08.000000 testless_autocomplete-0.0.111/setup.py
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:49:20.787635 testless_autocomplete-0.0.111/testless_autocomplete/
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:49:20.791201 testless_autocomplete-0.0.111/testless_autocomplete/src/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    15990 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.111/testless_autocomplete/src/AutoComplete.ipynb
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      542 2023-06-25 17:45:37.000000 testless_autocomplete-0.0.111/testless_autocomplete/src/AutoCompleteAPI.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.111/testless_autocomplete/src/__init__.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)     1262 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.111/testless_autocomplete/src/model.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.111/testless_autocomplete/src/ngram.csv
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      756 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.111/testless_autocomplete/src/preprocessing.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 19:23:08.573151 testless_autocomplete-0.0.112/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       36 2023-06-25 18:48:55.000000 testless_autocomplete-0.0.112/MANIFEST.in
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 19:23:08.572948 testless_autocomplete-0.0.112/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.112/README.md
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 19:23:08.573205 testless_autocomplete-0.0.112/setup.cfg
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      866 2023-06-25 19:22:57.000000 testless_autocomplete-0.0.112/setup.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 19:23:08.568630 testless_autocomplete-0.0.112/testless_autocomplete/
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 19:23:08.572414 testless_autocomplete-0.0.112/testless_autocomplete/src/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    15990 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.112/testless_autocomplete/src/AutoComplete.ipynb
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      528 2023-06-25 19:20:58.000000 testless_autocomplete-0.0.112/testless_autocomplete/src/AutoCompleteAPI.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.112/testless_autocomplete/src/__init__.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)     1262 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.112/testless_autocomplete/src/model.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.112/testless_autocomplete/src/ngram.csv
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      756 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.112/testless_autocomplete/src/preprocessing.py
```

### Comparing `testless_autocomplete-0.0.111/setup.py` & `testless_autocomplete-0.0.112/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="testless_autocomplete",
-    version="0.0.111",
+    version="0.0.112",
     description="Auto Complete Package",
     package_data={
         '../Auto_Complete': ['Auto_Complete/*'],
     },
-    package_dir={"": "../Auto_Complete/Auto_Complete"},
-    packages=find_packages(where="../Auto_Complete/Auto_Complete"),
+    package_dir={"": "../Auto_Complete"},
+    packages=find_packages(where="../Auto_Complete"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="TestLess",
     zip_safe=False,
     include_package_data=True,
     license="MIT",
     classifiers=[
```

### Comparing `testless_autocomplete-0.0.111/testless_autocomplete/src/AutoComplete.ipynb` & `testless_autocomplete-0.0.112/testless_autocomplete/src/AutoComplete.ipynb`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.111/testless_autocomplete/src/AutoCompleteAPI.py` & `testless_autocomplete-0.0.112/testless_autocomplete/src/AutoCompleteAPI.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,13 +6,13 @@
     # if text is empty or contains only spaces, return an empty list
     try:
 
         if text == '':
             return {'words': []}
         words = preprocess_text(text)
         # with autocomplete.app_context():
-        data = pd.read_csv('Auto_Complete/testless_autocomplete/src/ngram.csv')
+        data = pd.read_csv('testless_autocomplete/src/ngram.csv')
 
         data.set_index('ngram', inplace=True)        
         return {'words': data.loc[words[-1]]['next_word']} 
     except:
         return {'words': []}
```

### Comparing `testless_autocomplete-0.0.111/testless_autocomplete/src/model.py` & `testless_autocomplete-0.0.112/testless_autocomplete/src/model.py`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.111/testless_autocomplete/src/ngram.csv` & `testless_autocomplete-0.0.112/testless_autocomplete/src/ngram.csv`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.111/testless_autocomplete/src/preprocessing.py` & `testless_autocomplete-0.0.112/testless_autocomplete/src/preprocessing.py`

 * *Files identical despite different names*

