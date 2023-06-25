# Comparing `tmp/atro-pyparser-0.0.1.tar.gz` & `tmp/atro-pyparser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pyparser-0.0.1.tar", last modified: Fri Jun 23 17:26:19 2023, max compression
+gzip compressed data, was "atro-pyparser-0.0.2.tar", last modified: Sun Jun 25 09:36:15 2023, max compression
```

## Comparing `atro-pyparser-0.0.1.tar` & `atro-pyparser-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 17:26:19.166986 atro-pyparser-0.0.1/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      752 2023-06-23 17:26:19.166986 atro-pyparser-0.0.1/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pyparser-0.0.1/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 17:26:19.166986 atro-pyparser-0.0.1/atro_pyparser.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      752 2023-06-23 17:26:19.000000 atro-pyparser-0.0.1/atro_pyparser.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      223 2023-06-23 17:26:19.000000 atro-pyparser-0.0.1/atro_pyparser.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-23 17:26:19.000000 atro-pyparser-0.0.1/atro_pyparser.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)       20 2023-06-23 17:26:19.000000 atro-pyparser-0.0.1/atro_pyparser.egg-info/requires.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        9 2023-06-23 17:26:19.000000 atro-pyparser-0.0.1/atro_pyparser.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 17:26:19.166986 atro-pyparser-0.0.1/pyparser/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      426 2023-06-23 17:21:44.000000 atro-pyparser-0.0.1/pyparser/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-23 17:26:19.166986 atro-pyparser-0.0.1/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)      998 2023-06-23 17:26:02.000000 atro-pyparser-0.0.1/setup.py
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:36:15.404256 atro-pyparser-0.0.2/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      752 2023-06-25 09:36:15.404256 atro-pyparser-0.0.2/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pyparser-0.0.2/README.md
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:36:15.404256 atro-pyparser-0.0.2/atro_pyparser.egg-info/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      752 2023-06-25 09:36:15.000000 atro-pyparser-0.0.2/atro_pyparser.egg-info/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      223 2023-06-25 09:36:15.000000 atro-pyparser-0.0.2/atro_pyparser.egg-info/SOURCES.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-25 09:36:15.000000 atro-pyparser-0.0.2/atro_pyparser.egg-info/dependency_links.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       20 2023-06-25 09:36:15.000000 atro-pyparser-0.0.2/atro_pyparser.egg-info/requires.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        9 2023-06-25 09:36:15.000000 atro-pyparser-0.0.2/atro_pyparser.egg-info/top_level.txt
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:36:15.404256 atro-pyparser-0.0.2/pyparser/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      426 2023-06-25 09:35:42.000000 atro-pyparser-0.0.2/pyparser/__init__.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-25 09:36:15.404256 atro-pyparser-0.0.2/setup.cfg
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      994 2023-06-25 09:36:09.000000 atro-pyparser-0.0.2/setup.py
```

### Comparing `atro-pyparser-0.0.1/PKG-INFO` & `atro-pyparser-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pyparser
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple parsing wrapper around argparse. It works with atro-pylog otherwise its just about the same.
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pyparser-0.0.1/atro_pyparser.egg-info/PKG-INFO` & `atro-pyparser-0.0.2/atro_pyparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pyparser
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple parsing wrapper around argparse. It works with atro-pylog otherwise its just about the same.
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pyparser-0.0.1/setup.py` & `atro-pyparser-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import find_packages, setup
 
 setup(
     name="atro-pyparser",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     author="Atropos",
     author_email="pypi.rising@atro.xyz",
     description="A simple parsing wrapper around argparse. It works with atro-pylog otherwise its just about the same.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atropos/atro-pylog",
     install_requires=[
         "atro-pylog",
         "argparse",
-        ],
+    ],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

