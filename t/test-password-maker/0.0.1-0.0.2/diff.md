# Comparing `tmp/test_password_maker-0.0.1.tar.gz` & `tmp/test_password_maker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_password_maker-0.0.1.tar", last modified: Sun Jun 25 03:56:05 2023, max compression
+gzip compressed data, was "test_password_maker-0.0.2.tar", last modified: Sun Jun 25 04:04:12 2023, max compression
```

## Comparing `test_password_maker-0.0.1.tar` & `test_password_maker-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 hansohee   (501) staff       (20)        0 2023-06-25 03:56:05.159319 test_password_maker-0.0.1/
--rw-r--r--   0 hansohee   (501) staff       (20)      486 2023-06-25 03:56:05.159113 test_password_maker-0.0.1/PKG-INFO
--rw-r--r--   0 hansohee   (501) staff       (20)       42 2023-06-25 03:50:02.000000 test_password_maker-0.0.1/README
--rw-r--r--   0 hansohee   (501) staff       (20)       38 2023-06-25 03:56:05.159380 test_password_maker-0.0.1/setup.cfg
--rw-r--r--   0 hansohee   (501) staff       (20)      631 2023-06-25 03:55:49.000000 test_password_maker-0.0.1/setup.py
-drwxr-xr-x   0 hansohee   (501) staff       (20)        0 2023-06-25 03:56:05.157150 test_password_maker-0.0.1/test_password_maker/
--rw-r--r--   0 hansohee   (501) staff       (20)        0 2023-06-25 03:44:57.000000 test_password_maker-0.0.1/test_password_maker/__init__.py
--rw-r--r--   0 hansohee   (501) staff       (20)      380 2023-06-25 03:48:31.000000 test_password_maker-0.0.1/test_password_maker/password.py
-drwxr-xr-x   0 hansohee   (501) staff       (20)        0 2023-06-25 03:56:05.158866 test_password_maker-0.0.1/test_password_maker.egg-info/
--rw-r--r--   0 hansohee   (501) staff       (20)      486 2023-06-25 03:56:05.000000 test_password_maker-0.0.1/test_password_maker.egg-info/PKG-INFO
--rw-r--r--   0 hansohee   (501) staff       (20)      251 2023-06-25 03:56:05.000000 test_password_maker-0.0.1/test_password_maker.egg-info/SOURCES.txt
--rw-r--r--   0 hansohee   (501) staff       (20)        1 2023-06-25 03:56:05.000000 test_password_maker-0.0.1/test_password_maker.egg-info/dependency_links.txt
--rw-r--r--   0 hansohee   (501) staff       (20)       20 2023-06-25 03:56:05.000000 test_password_maker-0.0.1/test_password_maker.egg-info/top_level.txt
+drwxr-xr-x   0 hansohee   (501) staff       (20)        0 2023-06-25 04:04:12.452802 test_password_maker-0.0.2/
+-rw-r--r--   0 hansohee   (501) staff       (20)      486 2023-06-25 04:04:12.452646 test_password_maker-0.0.2/PKG-INFO
+-rw-r--r--   0 hansohee   (501) staff       (20)       42 2023-06-25 03:50:02.000000 test_password_maker-0.0.2/README
+-rw-r--r--   0 hansohee   (501) staff       (20)       38 2023-06-25 04:04:12.452848 test_password_maker-0.0.2/setup.cfg
+-rw-r--r--   0 hansohee   (501) staff       (20)      631 2023-06-25 04:04:10.000000 test_password_maker-0.0.2/setup.py
+drwxr-xr-x   0 hansohee   (501) staff       (20)        0 2023-06-25 04:04:12.451272 test_password_maker-0.0.2/test/
+-rw-r--r--   0 hansohee   (501) staff       (20)       85 2023-06-25 03:59:17.000000 test_password_maker-0.0.2/test/test.py
+drwxr-xr-x   0 hansohee   (501) staff       (20)        0 2023-06-25 04:04:12.451624 test_password_maker-0.0.2/test_password_maker/
+-rw-r--r--   0 hansohee   (501) staff       (20)        0 2023-06-25 03:44:57.000000 test_password_maker-0.0.2/test_password_maker/__init__.py
+-rw-r--r--   0 hansohee   (501) staff       (20)      383 2023-06-25 04:00:49.000000 test_password_maker-0.0.2/test_password_maker/password.py
+drwxr-xr-x   0 hansohee   (501) staff       (20)        0 2023-06-25 04:04:12.452408 test_password_maker-0.0.2/test_password_maker.egg-info/
+-rw-r--r--   0 hansohee   (501) staff       (20)      486 2023-06-25 04:04:12.000000 test_password_maker-0.0.2/test_password_maker.egg-info/PKG-INFO
+-rw-r--r--   0 hansohee   (501) staff       (20)      264 2023-06-25 04:04:12.000000 test_password_maker-0.0.2/test_password_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 hansohee   (501) staff       (20)        1 2023-06-25 04:04:12.000000 test_password_maker-0.0.2/test_password_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 hansohee   (501) staff       (20)       20 2023-06-25 04:04:12.000000 test_password_maker-0.0.2/test_password_maker.egg-info/top_level.txt
```

### Comparing `test_password_maker-0.0.1/setup.py` & `test_password_maker-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="test_password_maker",
-    version="0.0.1",
+    version="0.0.2",
     author="Sohee Han",
     author_email="eng.sohee@gmail.com",
     description="package build test",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nicecoding1/",
     packages=setuptools.find_packages(),
```

