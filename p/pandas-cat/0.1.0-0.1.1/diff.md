# Comparing `tmp/pandas-cat-0.1.0.tar.gz` & `tmp/pandas-cat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-cat-0.1.0.tar", last modified: Wed Apr 19 20:31:43 2023, max compression
+gzip compressed data, was "pandas-cat-0.1.1.tar", last modified: Sun Jun 25 20:18:07 2023, max compression
```

## Comparing `pandas-cat-0.1.0.tar` & `pandas-cat-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 20:31:43.633246 pandas-cat-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-04-18 20:32:42.000000 pandas-cat-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4220 2023-04-19 20:31:43.633246 pandas-cat-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3599 2023-04-19 19:30:26.000000 pandas-cat-0.1.0/README.md
--rw-rw-rw-   0        0        0      190 2023-04-18 20:31:47.000000 pandas-cat-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 20:31:43.633246 pandas-cat-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1218 2023-04-19 11:52:39.000000 pandas-cat-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:31:43.590530 pandas-cat-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 20:31:43.618498 pandas-cat-0.1.0/src/pandas_cat/
--rw-rw-rw-   0        0        0       35 2023-04-17 21:17:22.000000 pandas-cat-0.1.0/src/pandas_cat/__init__.py
--rw-rw-rw-   0        0        0    17963 2023-04-19 20:27:01.000000 pandas-cat-0.1.0/src/pandas_cat/pandas_cat.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:31:43.633246 pandas-cat-0.1.0/src/pandas_cat/templates/
--rw-rw-rw-   0        0        0    11804 2023-04-17 20:41:53.000000 pandas-cat-0.1.0/src/pandas_cat/templates/default_0_1_0.tem
-drwxrwxrwx   0        0        0        0 2023-04-19 20:31:43.633246 pandas-cat-0.1.0/src/pandas_cat.egg-info/
--rw-rw-rw-   0        0        0     4220 2023-04-19 20:31:43.000000 pandas-cat-0.1.0/src/pandas_cat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-04-19 20:31:43.000000 pandas-cat-0.1.0/src/pandas_cat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 20:31:43.000000 pandas-cat-0.1.0/src/pandas_cat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-19 20:31:43.000000 pandas-cat-0.1.0/src/pandas_cat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-19 20:31:43.000000 pandas-cat-0.1.0/src/pandas_cat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 20:18:07.536927 pandas-cat-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-04-18 20:32:42.000000 pandas-cat-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4220 2023-06-25 20:18:07.536927 pandas-cat-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3599 2023-04-19 19:30:26.000000 pandas-cat-0.1.1/README.md
+-rw-rw-rw-   0        0        0      190 2023-04-18 20:31:47.000000 pandas-cat-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 20:18:07.536927 pandas-cat-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2023-06-25 20:13:30.000000 pandas-cat-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:18:07.506231 pandas-cat-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 20:18:07.521293 pandas-cat-0.1.1/src/pandas_cat/
+-rw-rw-rw-   0        0        0       46 2023-06-25 20:14:05.000000 pandas-cat-0.1.1/src/pandas_cat/__init__.py
+-rw-rw-rw-   0        0        0    17963 2023-06-25 20:15:38.000000 pandas-cat-0.1.1/src/pandas_cat/pandas_cat.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:18:07.536927 pandas-cat-0.1.1/src/pandas_cat/templates/
+-rw-rw-rw-   0        0        0    11804 2023-04-17 20:41:53.000000 pandas-cat-0.1.1/src/pandas_cat/templates/default_0_1_0.tem
+drwxrwxrwx   0        0        0        0 2023-06-25 20:18:07.536927 pandas-cat-0.1.1/src/pandas_cat.egg-info/
+-rw-rw-rw-   0        0        0     4220 2023-06-25 20:18:07.000000 pandas-cat-0.1.1/src/pandas_cat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-06-25 20:18:07.000000 pandas-cat-0.1.1/src/pandas_cat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 20:18:07.000000 pandas-cat-0.1.1/src/pandas_cat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-25 20:18:07.000000 pandas-cat-0.1.1/src/pandas_cat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-25 20:18:07.000000 pandas-cat-0.1.1/src/pandas_cat.egg-info/top_level.txt
```

### Comparing `pandas-cat-0.1.0/LICENSE` & `pandas-cat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-cat-0.1.0/PKG-INFO` & `pandas-cat-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-cat
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pandas categorical profiling. Generates html profile report for categorical dataset. Also provides several handful functions.
 Home-page: https://petrmasa.com/pandas-cat
 Author: (C) Copyright 2022 - 2023 Petr Masa & LBC
 Author-email: code@cleverminer.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pandas-cat-0.1.0/README.md` & `pandas-cat-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pandas-cat-0.1.0/setup.py` & `pandas-cat-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pandas-cat",
-    version="0.1.0",
+    version="0.1.1",
     author="(C) Copyright 2022 - 2023 Petr Masa & LBC",
     author_email="code@cleverminer.org",
     description="Pandas categorical profiling. Generates html profile report for categorical dataset. Also provides several handful functions.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://petrmasa.com/pandas-cat",
     license = "MIT",
```

### Comparing `pandas-cat-0.1.0/src/pandas_cat/pandas_cat.py` & `pandas-cat-0.1.1/src/pandas_cat/pandas_cat.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import scipy.stats as ss
 
 class pandas_cat:
     """
     Pandas categorical profiling. Creates html report with profile of categorical dataset. Provides also other useful functions.
     """
 
-    version_string = "0.1.0"
+    version_string = "0.1.1"
     template_name = "default_0_1_0.tem"
 
     def __init(self):
         """
         Initializes a class.
 
         """
```

### Comparing `pandas-cat-0.1.0/src/pandas_cat/templates/default_0_1_0.tem` & `pandas-cat-0.1.1/src/pandas_cat/templates/default_0_1_0.tem`

 * *Files identical despite different names*

### Comparing `pandas-cat-0.1.0/src/pandas_cat.egg-info/PKG-INFO` & `pandas-cat-0.1.1/src/pandas_cat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-cat
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pandas categorical profiling. Generates html profile report for categorical dataset. Also provides several handful functions.
 Home-page: https://petrmasa.com/pandas-cat
 Author: (C) Copyright 2022 - 2023 Petr Masa & LBC
 Author-email: code@cleverminer.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

