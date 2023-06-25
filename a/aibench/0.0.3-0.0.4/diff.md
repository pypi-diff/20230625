# Comparing `tmp/aibench-0.0.3.tar.gz` & `tmp/aibench-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibench-0.0.3.tar", last modified: Sun Jun 25 15:34:28 2023, max compression
+gzip compressed data, was "aibench-0.0.4.tar", last modified: Sun Jun 25 15:37:56 2023, max compression
```

## Comparing `aibench-0.0.3.tar` & `aibench-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:34:28.574787 aibench-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-25 15:34:28.578787 aibench-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-25 15:34:18.000000 aibench-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:34:28.574787 aibench-0.0.3/aibench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-25 15:34:28.000000 aibench-0.0.3/aibench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-25 15:34:28.000000 aibench-0.0.3/aibench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:34:28.000000 aibench-0.0.3/aibench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-25 15:34:28.000000 aibench-0.0.3/aibench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 15:34:28.000000 aibench-0.0.3/aibench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:34:28.574787 aibench-0.0.3/aibenchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-25 15:34:18.000000 aibench-0.0.3/aibenchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-25 15:34:18.000000 aibench-0.0.3/aibenchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-25 15:34:18.000000 aibench-0.0.3/aibenchmark/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-25 15:34:18.000000 aibench-0.0.3/aibenchmark/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-25 15:34:18.000000 aibench-0.0.3/aibenchmark/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-25 15:34:18.000000 aibench-0.0.3/aibenchmark/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:34:28.574787 aibench-0.0.3/aibenchmark/scrapers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 15:34:18.000000 aibench-0.0.3/aibenchmark/scrapers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-25 15:34:18.000000 aibench-0.0.3/aibenchmark/scrapers/papers_with_code_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-25 15:34:28.578787 aibench-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-25 15:34:18.000000 aibench-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:34:28.574787 aibench-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-25 15:34:18.000000 aibench-0.0.3/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-25 15:34:18.000000 aibench-0.0.3/tests/test_classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-25 15:34:18.000000 aibench-0.0.3/tests/test_nlp_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-25 15:34:18.000000 aibench-0.0.3/tests/test_regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:56.751932 aibench-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-25 15:37:56.751932 aibench-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-25 15:37:44.000000 aibench-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-25 15:37:44.000000 aibench-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:56.751932 aibench-0.0.4/aibench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-25 15:37:56.000000 aibench-0.0.4/aibench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-25 15:37:56.000000 aibench-0.0.4/aibench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:37:56.000000 aibench-0.0.4/aibench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-25 15:37:56.000000 aibench-0.0.4/aibench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 15:37:56.000000 aibench-0.0.4/aibench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:56.751932 aibench-0.0.4/aibenchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:56.751932 aibench-0.0.4/aibenchmark/scrapers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/scrapers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/scrapers/papers_with_code_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-25 15:37:56.751932 aibench-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-25 15:37:44.000000 aibench-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:56.751932 aibench-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-25 15:37:44.000000 aibench-0.0.4/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-25 15:37:44.000000 aibench-0.0.4/tests/test_classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-25 15:37:44.000000 aibench-0.0.4/tests/test_nlp_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-25 15:37:44.000000 aibench-0.0.4/tests/test_regression_metrics.py
```

### Comparing `aibench-0.0.3/README.rst` & `aibench-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `aibench-0.0.3/aibench.egg-info/SOURCES.txt` & `aibench-0.0.4/aibench.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 README.rst
 setup.cfg
 setup.py
 aibench.egg-info/PKG-INFO
 aibench.egg-info/SOURCES.txt
 aibench.egg-info/dependency_links.txt
 aibench.egg-info/requires.txt
```

### Comparing `aibench-0.0.3/aibenchmark/benchmark.py` & `aibench-0.0.4/aibenchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.3/aibenchmark/dataset.py` & `aibench-0.0.4/aibenchmark/dataset.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.3/aibenchmark/metrics.py` & `aibench-0.0.4/aibenchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.3/aibenchmark/scrapers/papers_with_code_scraper.py` & `aibench-0.0.4/aibenchmark/scrapers/papers_with_code_scraper.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.3/setup.py` & `aibench-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aibench',
-    version='0.0.3',
-    long_description='Benchmark your AI model against popular benchmarks',
+    version='0.0.4',
     license='MIT',
     author="Based Labs",
     author_email='',
     packages=find_packages(exclude=["tests"]),
     url='https://github.com/BasedLabs/aibenchmark/',
     keywords='ai benchmark metrics',
     install_requires=[
```

### Comparing `aibench-0.0.3/tests/test_benchmark.py` & `aibench-0.0.4/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.3/tests/test_classification_metrics.py` & `aibench-0.0.4/tests/test_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.3/tests/test_regression_metrics.py` & `aibench-0.0.4/tests/test_regression_metrics.py`

 * *Files identical despite different names*

