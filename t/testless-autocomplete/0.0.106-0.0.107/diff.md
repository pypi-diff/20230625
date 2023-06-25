# Comparing `tmp/testless_autocomplete-0.0.106.tar.gz` & `tmp/testless_autocomplete-0.0.107.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_autocomplete-0.0.106.tar", last modified: Sun Jun 25 18:28:09 2023, max compression
+gzip compressed data, was "testless_autocomplete-0.0.107.tar", last modified: Sun Jun 25 18:31:52 2023, max compression
```

## Comparing `testless_autocomplete-0.0.106.tar` & `testless_autocomplete-0.0.107.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:28:09.203199 testless_autocomplete-0.0.106/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       44 2023-06-25 18:12:56.000000 testless_autocomplete-0.0.106/MANIFEST.in
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 18:28:09.203040 testless_autocomplete-0.0.106/PKG-INFO
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.106/README.md
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 18:28:09.203244 testless_autocomplete-0.0.106/setup.cfg
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      882 2023-06-25 18:27:59.000000 testless_autocomplete-0.0.106/setup.py
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:28:09.200662 testless_autocomplete-0.0.106/testless_autocomplete/
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:28:09.202817 testless_autocomplete-0.0.106/testless_autocomplete/src/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.106/testless_autocomplete/src/ngram.csv
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:31:52.256517 testless_autocomplete-0.0.107/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       44 2023-06-25 18:12:56.000000 testless_autocomplete-0.0.107/MANIFEST.in
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 18:31:52.256332 testless_autocomplete-0.0.107/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.107/README.md
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 18:31:52.256583 testless_autocomplete-0.0.107/setup.cfg
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      882 2023-06-25 18:31:11.000000 testless_autocomplete-0.0.107/setup.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:31:52.253727 testless_autocomplete-0.0.107/testless_autocomplete/
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:31:52.255889 testless_autocomplete-0.0.107/testless_autocomplete/src/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.107/testless_autocomplete/src/ngram.csv
```

### Comparing `testless_autocomplete-0.0.106/setup.py` & `testless_autocomplete-0.0.107/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="testless_autocomplete",
-    version="0.0.106",
+    version="0.0.107",
     description="Auto Complete Package",
     package_data={
         '../Auto_Complete/testless_autocomplete': ['src/*.csv'],
     },
     package_dir={"": "../Auto_Complete"},
     packages=find_packages(where="../Auto_Complete"),
     long_description=long_description,
```

### Comparing `testless_autocomplete-0.0.106/testless_autocomplete/src/ngram.csv` & `testless_autocomplete-0.0.107/testless_autocomplete/src/ngram.csv`

 * *Files identical despite different names*

