# Comparing `tmp/testless_autocomplete-0.0.108.tar.gz` & `tmp/testless_autocomplete-0.0.109.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_autocomplete-0.0.108.tar", last modified: Sun Jun 25 18:35:25 2023, max compression
+gzip compressed data, was "testless_autocomplete-0.0.109.tar", last modified: Sun Jun 25 18:38:08 2023, max compression
```

## Comparing `testless_autocomplete-0.0.108.tar` & `testless_autocomplete-0.0.109.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:35:25.368915 testless_autocomplete-0.0.108/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       44 2023-06-25 18:12:56.000000 testless_autocomplete-0.0.108/MANIFEST.in
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 18:35:25.368740 testless_autocomplete-0.0.108/PKG-INFO
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.108/README.md
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 18:35:25.368960 testless_autocomplete-0.0.108/setup.cfg
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      866 2023-06-25 18:35:05.000000 testless_autocomplete-0.0.108/setup.py
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:35:25.366297 testless_autocomplete-0.0.108/testless_autocomplete/
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:35:25.368405 testless_autocomplete-0.0.108/testless_autocomplete/src/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.108/testless_autocomplete/src/ngram.csv
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:38:08.657611 testless_autocomplete-0.0.109/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       44 2023-06-25 18:12:56.000000 testless_autocomplete-0.0.109/MANIFEST.in
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 18:38:08.657424 testless_autocomplete-0.0.109/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.109/README.md
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 18:38:08.657661 testless_autocomplete-0.0.109/setup.cfg
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      894 2023-06-25 18:37:59.000000 testless_autocomplete-0.0.109/setup.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:38:08.653329 testless_autocomplete-0.0.109/testless_autocomplete/
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:38:08.656998 testless_autocomplete-0.0.109/testless_autocomplete/src/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.109/testless_autocomplete/src/ngram.csv
```

### Comparing `testless_autocomplete-0.0.108/setup.py` & `testless_autocomplete-0.0.109/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="testless_autocomplete",
-    version="0.0.108",
+    version="0.0.109",
     description="Auto Complete Package",
     package_data={
         '../Auto_Complete': ['Auto_Complete/*'],
     },
-    package_dir={"": "../Auto_Complete"},
-    packages=find_packages(where="../Auto_Complete"),
+    package_dir={"": "../Auto_Complete/Auto_Complete"},
+    packages=find_packages(where="../Auto_Complete/Auto_Complete"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="TestLess",
     zip_safe=False,
     include_package_data=True,
     license="MIT",
     classifiers=[
```

### Comparing `testless_autocomplete-0.0.108/testless_autocomplete/src/ngram.csv` & `testless_autocomplete-0.0.109/testless_autocomplete/src/ngram.csv`

 * *Files identical despite different names*

