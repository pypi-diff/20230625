# Comparing `tmp/lfinancial-0.0.2.tar.gz` & `tmp/lfinancial-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.0.2.tar", last modified: Tue Jun 20 16:59:06 2023, max compression
+gzip compressed data, was "lfinancial-0.0.3.tar", last modified: Sun Jun 25 09:50:29 2023, max compression
```

## Comparing `lfinancial-0.0.2.tar` & `lfinancial-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-20 16:59:06.642574 lfinancial-0.0.2/
--rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-20 16:59:06.642483 lfinancial-0.0.2/PKG-INFO
--rw-r--r--   0 lzy        (501) staff       (20)       68 2023-06-20 16:50:45.000000 lfinancial-0.0.2/README.md
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-20 16:59:06.641989 lfinancial-0.0.2/lfinancial/
--rw-r--r--   0 lzy        (501) staff       (20)       33 2023-06-20 16:21:35.000000 lfinancial-0.0.2/lfinancial/__init__.py
--rw-r--r--   0 lzy        (501) staff       (20)      155 2023-06-20 16:56:11.000000 lfinancial-0.0.2/lfinancial/financial.py
--rw-r--r--   0 lzy        (501) staff       (20)      741 2023-06-20 16:56:11.000000 lfinancial-0.0.2/lfinancial/generators.py
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-20 16:59:06.642335 lfinancial-0.0.2/lfinancial.egg-info/
--rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-20 16:59:06.000000 lfinancial-0.0.2/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 lzy        (501) staff       (20)      226 2023-06-20 16:59:06.000000 lfinancial-0.0.2/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 lzy        (501) staff       (20)        1 2023-06-20 16:59:06.000000 lfinancial-0.0.2/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 lzy        (501) staff       (20)       11 2023-06-20 16:59:06.000000 lfinancial-0.0.2/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 lzy        (501) staff       (20)       38 2023-06-20 16:59:06.642603 lfinancial-0.0.2/setup.cfg
--rw-r--r--   0 lzy        (501) staff       (20)      568 2023-06-20 16:58:21.000000 lfinancial-0.0.2/setup.py
+drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-25 09:50:29.996655 lfinancial-0.0.3/
+-rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-25 09:50:29.996537 lfinancial-0.0.3/PKG-INFO
+-rw-r--r--   0 lzy        (501) staff       (20)       68 2023-06-21 09:04:34.000000 lfinancial-0.0.3/README.md
+drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-25 09:50:29.995993 lfinancial-0.0.3/lfinancial/
+-rw-r--r--   0 lzy        (501) staff       (20)       33 2023-06-21 09:04:34.000000 lfinancial-0.0.3/lfinancial/__init__.py
+-rw-r--r--   0 lzy        (501) staff       (20)      328 2023-06-25 09:43:45.000000 lfinancial-0.0.3/lfinancial/financial.py
+drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-25 09:50:29.996391 lfinancial-0.0.3/lfinancial.egg-info/
+-rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-25 09:50:29.000000 lfinancial-0.0.3/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 lzy        (501) staff       (20)      201 2023-06-25 09:50:29.000000 lfinancial-0.0.3/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 lzy        (501) staff       (20)        1 2023-06-25 09:50:29.000000 lfinancial-0.0.3/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 lzy        (501) staff       (20)       11 2023-06-25 09:50:29.000000 lfinancial-0.0.3/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 lzy        (501) staff       (20)       38 2023-06-25 09:50:29.996690 lfinancial-0.0.3/setup.cfg
+-rw-r--r--   0 lzy        (501) staff       (20)      568 2023-06-25 09:50:21.000000 lfinancial-0.0.3/setup.py
```

### Comparing `lfinancial-0.0.2/setup.py` & `lfinancial-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 excluded_packages = ["docs", "tests", "tests.*"]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lfinancial',
-    version='0.0.2',
+    version='0.0.3',
     author='zaneliu',
     author_email='lzy291980138@163.com',
     description='Generate financial test data',
     packages=['lfinancial'],
     install_requires=[],
     classifiers=[
         'Programming Language :: Python :: 3',
```

