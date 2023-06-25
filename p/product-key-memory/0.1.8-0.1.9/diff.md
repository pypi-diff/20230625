# Comparing `tmp/product_key_memory-0.1.8.tar.gz` & `tmp/product_key_memory-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/product_key_memory-0.1.8.tar", last modified: Tue Jun  9 06:46:04 2020, max compression
+gzip compressed data, was "dist/product_key_memory-0.1.9.tar", last modified: Tue Jun  9 15:06:37 2020, max compression
```

## Comparing `product_key_memory-0.1.8.tar` & `product_key_memory-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-06-09 06:46:04.000000 product_key_memory-0.1.8/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-06-09 06:46:04.000000 product_key_memory-0.1.8/product_key_memory/
--rw-rw-r--   0 phil      (1000) phil      (1000)      110 2020-06-09 06:19:03.000000 product_key_memory-0.1.8/product_key_memory/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3843 2020-06-09 06:19:03.000000 product_key_memory-0.1.8/product_key_memory/product_key_memory.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2423 2020-06-09 06:45:38.000000 product_key_memory-0.1.8/product_key_memory/evonorm.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      602 2020-06-09 06:46:04.000000 product_key_memory-0.1.8/PKG-INFO
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-06-09 06:46:04.000000 product_key_memory-0.1.8/product_key_memory.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)      329 2020-06-09 06:46:03.000000 product_key_memory-0.1.8/product_key_memory.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       19 2020-06-09 06:46:03.000000 product_key_memory-0.1.8/product_key_memory.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2020-06-09 06:46:03.000000 product_key_memory-0.1.8/product_key_memory.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      602 2020-06-09 06:46:03.000000 product_key_memory-0.1.8/product_key_memory.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)        6 2020-06-09 06:46:03.000000 product_key_memory-0.1.8/product_key_memory.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2020-06-09 06:46:04.000000 product_key_memory-0.1.8/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      719 2020-06-09 06:45:51.000000 product_key_memory-0.1.8/setup.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2777 2020-06-09 06:19:03.000000 product_key_memory-0.1.8/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      159 2020-06-09 15:05:58.000000 product_key_memory-0.1.9/product_key_memory/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3843 2020-06-09 06:19:03.000000 product_key_memory-0.1.9/product_key_memory/product_key_memory.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2423 2020-06-09 06:45:38.000000 product_key_memory-0.1.9/product_key_memory/evonorm.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      602 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/PKG-INFO
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      329 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       19 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      602 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)        6 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)      719 2020-06-09 15:05:38.000000 product_key_memory-0.1.9/setup.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2777 2020-06-09 06:19:03.000000 product_key_memory-0.1.9/README.md
```

### Comparing `product_key_memory-0.1.8/product_key_memory/product_key_memory.py` & `product_key_memory-0.1.9/product_key_memory/product_key_memory.py`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.1.8/product_key_memory/evonorm.py` & `product_key_memory-0.1.9/product_key_memory/evonorm.py`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.1.8/PKG-INFO` & `product_key_memory-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: product_key_memory
-Version: 0.1.8
+Version: 0.1.9
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: transformers,artificial intelligence
```

### Comparing `product_key_memory-0.1.8/product_key_memory.egg-info/PKG-INFO` & `product_key_memory-0.1.9/product_key_memory.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: product-key-memory
-Version: 0.1.8
+Version: 0.1.9
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: transformers,artificial intelligence
```

### Comparing `product_key_memory-0.1.8/setup.py` & `product_key_memory-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'product_key_memory',
   packages = find_packages(),
-  version = '0.1.8',
+  version = '0.1.9',
   license='MIT',
   description = 'Product Key Memory',
   author = 'Aran Komatsuzaki, Phil Wang',
   author_email = 'aran1234321@gmail.com, lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/product-key-memory',
   keywords = ['transformers', 'artificial intelligence'],
   install_requires=[
```

### Comparing `product_key_memory-0.1.8/README.md` & `product_key_memory-0.1.9/README.md`

 * *Files identical despite different names*

