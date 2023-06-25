# Comparing `tmp/testless_autocomplete-0.0.102.tar.gz` & `tmp/testless_autocomplete-0.0.103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_autocomplete-0.0.102.tar", last modified: Sun Jun 25 17:48:49 2023, max compression
+gzip compressed data, was "testless_autocomplete-0.0.103.tar", last modified: Sun Jun 25 18:06:58 2023, max compression
```

## Comparing `testless_autocomplete-0.0.102.tar` & `testless_autocomplete-0.0.103.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 17:48:49.104905 testless_autocomplete-0.0.102/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       61 2023-06-25 17:47:46.000000 testless_autocomplete-0.0.102/MANIFEST.in
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 17:48:49.104745 testless_autocomplete-0.0.102/PKG-INFO
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.102/README.md
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 17:48:49.104952 testless_autocomplete-0.0.102/setup.cfg
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      771 2023-06-25 17:48:05.000000 testless_autocomplete-0.0.102/setup.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-25 18:06:58.872711 testless_autocomplete-0.0.103/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       61 2023-06-25 17:47:46.000000 testless_autocomplete-0.0.103/MANIFEST.in
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      495 2023-06-25 18:06:58.872541 testless_autocomplete-0.0.103/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      156 2023-06-25 15:07:09.000000 testless_autocomplete-0.0.103/README.md
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-25 18:06:58.872757 testless_autocomplete-0.0.103/setup.cfg
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      865 2023-06-25 18:06:48.000000 testless_autocomplete-0.0.103/setup.py
```

### Comparing `testless_autocomplete-0.0.102/setup.py` & `testless_autocomplete-0.0.103/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="testless_autocomplete",
-    version="0.0.102",
+    version="0.0.103",
     description="Auto Complete Package",
+    package_data={
+        'testless_autocomplete': ['src/*.txt'],
+    },
     package_dir={"": "../Auto_Complete"},
     packages=find_packages(where="../Auto_Complete"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="TestLess",
+    zip_safe=False,
     include_package_data=True,
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
```

