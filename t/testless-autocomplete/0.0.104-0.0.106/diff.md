# Comparing `tmp/testless_autocomplete-0.0.104.tar.gz` & `tmp/testless_autocomplete-0.0.106.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_autocomplete-0.0.104.tar", last modified: Sun Jun 25 18:09:49 2023, max compression
+gzip compressed data, was "testless_autocomplete-0.0.106.tar", last modified: Sun Jun 25 18:28:09 2023, max compression
```

## Comparing `testless_autocomplete-0.0.104.tar` & `testless_autocomplete-0.0.106.tar`

### file list

```diff
@@ -1,6 +1,9 @@
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:09:49.283278 testless_autocomplete-0.0.104/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       61 2023-06-25 17:47:46.000000 testless_autocomplete-0.0.104/MANIFEST.in
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 18:09:49.283086 testless_autocomplete-0.0.104/PKG-INFO
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.104/README.md
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 18:09:49.283324 testless_autocomplete-0.0.104/setup.cfg
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      865 2023-06-25 18:09:45.000000 testless_autocomplete-0.0.104/setup.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:28:09.203199 testless_autocomplete-0.0.106/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       44 2023-06-25 18:12:56.000000 testless_autocomplete-0.0.106/MANIFEST.in
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 18:28:09.203040 testless_autocomplete-0.0.106/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.106/README.md
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 18:28:09.203244 testless_autocomplete-0.0.106/setup.cfg
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      882 2023-06-25 18:27:59.000000 testless_autocomplete-0.0.106/setup.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:28:09.200662 testless_autocomplete-0.0.106/testless_autocomplete/
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:28:09.202817 testless_autocomplete-0.0.106/testless_autocomplete/src/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.106/testless_autocomplete/src/ngram.csv
```

### Comparing `testless_autocomplete-0.0.104/setup.py` & `testless_autocomplete-0.0.106/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="testless_autocomplete",
-    version="0.0.104",
+    version="0.0.106",
     description="Auto Complete Package",
     package_data={
-        'testless_autocomplete': ['src/*.csv'],
+        '../Auto_Complete/testless_autocomplete': ['src/*.csv'],
     },
     package_dir={"": "../Auto_Complete"},
     packages=find_packages(where="../Auto_Complete"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="TestLess",
     zip_safe=False,
```

