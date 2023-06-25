# Comparing `tmp/testless_autocomplete-0.0.109.tar.gz` & `tmp/testless_autocomplete-0.0.110.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_autocomplete-0.0.109.tar", last modified: Sun Jun 25 18:38:08 2023, max compression
+gzip compressed data, was "testless_autocomplete-0.0.110.tar", last modified: Sun Jun 25 18:44:21 2023, max compression
```

## Comparing `testless_autocomplete-0.0.109.tar` & `testless_autocomplete-0.0.110.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:38:08.657611 testless_autocomplete-0.0.109/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       44 2023-06-25 18:12:56.000000 testless_autocomplete-0.0.109/MANIFEST.in
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 18:38:08.657424 testless_autocomplete-0.0.109/PKG-INFO
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.109/README.md
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 18:38:08.657661 testless_autocomplete-0.0.109/setup.cfg
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      894 2023-06-25 18:37:59.000000 testless_autocomplete-0.0.109/setup.py
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:38:08.653329 testless_autocomplete-0.0.109/testless_autocomplete/
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:38:08.656998 testless_autocomplete-0.0.109/testless_autocomplete/src/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.109/testless_autocomplete/src/ngram.csv
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:44:21.280335 testless_autocomplete-0.0.110/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       44 2023-06-25 18:12:56.000000 testless_autocomplete-0.0.110/MANIFEST.in
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 18:44:21.280165 testless_autocomplete-0.0.110/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.110/README.md
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 18:44:21.280376 testless_autocomplete-0.0.110/setup.cfg
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      894 2023-06-25 18:41:17.000000 testless_autocomplete-0.0.110/setup.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:44:21.278039 testless_autocomplete-0.0.110/testless_autocomplete/
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:44:21.279791 testless_autocomplete-0.0.110/testless_autocomplete/src/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.110/testless_autocomplete/src/ngram.csv
```

### Comparing `testless_autocomplete-0.0.109/setup.py` & `testless_autocomplete-0.0.110/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="testless_autocomplete",
-    version="0.0.109",
+    version="0.0.110",
     description="Auto Complete Package",
     package_data={
         '../Auto_Complete': ['Auto_Complete/*'],
     },
     package_dir={"": "../Auto_Complete/Auto_Complete"},
     packages=find_packages(where="../Auto_Complete/Auto_Complete"),
     long_description=long_description,
```

### Comparing `testless_autocomplete-0.0.109/testless_autocomplete/src/ngram.csv` & `testless_autocomplete-0.0.110/testless_autocomplete/src/ngram.csv`

 * *Files identical despite different names*

