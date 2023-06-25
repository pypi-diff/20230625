# Comparing `tmp/pyeletrica-0.0.1.tar.gz` & `tmp/pyeletrica-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeletrica-0.0.1.tar", last modified: Sun Jun 25 16:55:05 2023, max compression
+gzip compressed data, was "pyeletrica-0.0.2.tar", last modified: Sun Jun 25 18:40:51 2023, max compression
```

## Comparing `pyeletrica-0.0.1.tar` & `pyeletrica-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 16:55:05.581463 pyeletrica-0.0.1/
--rw-rw-rw-   0        0        0     1106 2023-06-22 22:51:37.000000 pyeletrica-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3935 2023-06-25 16:55:05.570490 pyeletrica-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2147 2023-06-25 16:51:31.000000 pyeletrica-0.0.1/README.md
--rw-rw-rw-   0        0        0      811 2023-06-25 16:50:05.000000 pyeletrica-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 16:55:05.582459 pyeletrica-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 16:55:05.421893 pyeletrica-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 16:55:05.479733 pyeletrica-0.0.1/src/pyeletrica/
--rw-rw-rw-   0        0        0       54 2023-06-25 16:48:22.000000 pyeletrica-0.0.1/src/pyeletrica/__init__.py
--rw-rw-rw-   0        0        0     8262 2023-06-23 08:09:49.000000 pyeletrica-0.0.1/src/pyeletrica/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 16:55:05.559519 pyeletrica-0.0.1/src/pyeletrica.egg-info/
--rw-rw-rw-   0        0        0     3935 2023-06-25 16:55:05.000000 pyeletrica-0.0.1/src/pyeletrica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-25 16:55:05.000000 pyeletrica-0.0.1/src/pyeletrica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 16:55:05.000000 pyeletrica-0.0.1/src/pyeletrica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-25 16:55:05.000000 pyeletrica-0.0.1/src/pyeletrica.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-06-25 16:55:05.000000 pyeletrica-0.0.1/src/pyeletrica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-25 16:55:05.000000 pyeletrica-0.0.1/src/pyeletrica.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 18:40:51.566014 pyeletrica-0.0.2/
+-rw-rw-rw-   0        0        0     1106 2023-06-22 22:51:37.000000 pyeletrica-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3935 2023-06-25 18:40:51.557036 pyeletrica-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2147 2023-06-25 16:51:31.000000 pyeletrica-0.0.2/README.md
+-rw-rw-rw-   0        0        0      749 2023-06-25 18:33:20.000000 pyeletrica-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 18:40:51.566014 pyeletrica-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 18:40:51.424393 pyeletrica-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 18:40:51.476254 pyeletrica-0.0.2/src/pyeletrica/
+-rw-rw-rw-   0        0        0     8320 2023-06-25 18:33:10.000000 pyeletrica-0.0.2/src/pyeletrica/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:40:51.546066 pyeletrica-0.0.2/src/pyeletrica.egg-info/
+-rw-rw-rw-   0        0        0     3935 2023-06-25 18:40:51.000000 pyeletrica-0.0.2/src/pyeletrica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-25 18:40:51.000000 pyeletrica-0.0.2/src/pyeletrica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 18:40:51.000000 pyeletrica-0.0.2/src/pyeletrica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-25 18:40:51.000000 pyeletrica-0.0.2/src/pyeletrica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-25 18:40:51.000000 pyeletrica-0.0.2/src/pyeletrica.egg-info/top_level.txt
```

### Comparing `pyeletrica-0.0.1/LICENSE` & `pyeletrica-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeletrica-0.0.1/PKG-INFO` & `pyeletrica-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeletrica
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fundamental tools for electrical engineers.
 Author-email: Hugo Everaldo Salvador Bezerra <hugoesb@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hugo Everaldo Salvador Bezerra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyeletrica-0.0.1/README.md` & `pyeletrica-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyeletrica-0.0.1/pyproject.toml` & `pyeletrica-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["matplotlib", "numpy", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyeletrica"
-version = "0.0.1"
+version = "0.0.2"
 description = "Fundamental tools for electrical engineers."
 readme = "README.md"
 authors = [{ name = "Hugo Everaldo Salvador Bezerra", email = "hugoesb@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -19,11 +19,8 @@
     "matplotlib",
     "numpy",
     'tomli; python_version < "3.12"',
 ]
 requires-python = ">=3.6"
 
 [project.urls]
-"Homepage" = "https://github.com/hugoesb/pyeletrica"
-
-[project.scripts]
-pyeletrica = "pyeletrica.__main__:main"
+"Homepage" = "https://github.com/hugoesb/pyeletrica"
```

### Comparing `pyeletrica-0.0.1/src/pyeletrica/__main__.py` & `pyeletrica-0.0.2/src/pyeletrica/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Version of pyeletrica package
+__version__ = "0.0.2"
+
 import numpy as np
 import matplotlib.pyplot as plt
 
 def sind(angle):
     '''
     Compute sine of angle, where angle is in degrees.
```

### Comparing `pyeletrica-0.0.1/src/pyeletrica.egg-info/PKG-INFO` & `pyeletrica-0.0.2/src/pyeletrica.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeletrica
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fundamental tools for electrical engineers.
 Author-email: Hugo Everaldo Salvador Bezerra <hugoesb@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hugo Everaldo Salvador Bezerra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

