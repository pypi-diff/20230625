# Comparing `tmp/mloptimizer-0.5.8.tar.gz` & `tmp/mloptimizer-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mloptimizer-0.5.8.tar", last modified: Sat Jun 24 10:43:44 2023, max compression
+gzip compressed data, was "mloptimizer-0.5.9.tar", last modified: Sun Jun 25 10:12:25 2023, max compression
```

## Comparing `mloptimizer-0.5.8.tar` & `mloptimizer-0.5.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:44.900845 mloptimizer-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-24 10:43:44.900845 mloptimizer-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:44.896845 mloptimizer-0.5.8/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1954444 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/data/data_sample.csv
--rw-r--r--   0 runner    (1001) docker     (123)   694332 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/data/data_sample_test.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1260187 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/data/data_sample_train.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:44.896845 mloptimizer-0.5.8/mloptimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/genoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/model_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:44.900845 mloptimizer-0.5.8/mloptimizer/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/test_TreeOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/test_XGBClassifierOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/test_alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/test_genoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/test_param.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:44.900845 mloptimizer-0.5.8/mloptimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-24 10:43:44.000000 mloptimizer-0.5.8/mloptimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-24 10:43:44.000000 mloptimizer-0.5.8/mloptimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:43:44.000000 mloptimizer-0.5.8/mloptimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-24 10:43:44.000000 mloptimizer-0.5.8/mloptimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-24 10:43:44.000000 mloptimizer-0.5.8/mloptimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 10:43:44.900845 mloptimizer-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:25.444268 mloptimizer-0.5.9/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1954444 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/data/data_sample.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   694332 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/data/data_sample_test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1260187 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/data/data_sample_train.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/mloptimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/genoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/model_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/mloptimizer/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/test_TreeOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/test_XGBClassifierOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/test_alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/test_genoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/test_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/mloptimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-25 10:12:25.000000 mloptimizer-0.5.9/mloptimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-25 10:12:25.000000 mloptimizer-0.5.9/mloptimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 10:12:25.000000 mloptimizer-0.5.9/mloptimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-25 10:12:25.000000 mloptimizer-0.5.9/mloptimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 10:12:25.000000 mloptimizer-0.5.9/mloptimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/setup.py
```

### Comparing `mloptimizer-0.5.8/LICENSE` & `mloptimizer-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/PKG-INFO` & `mloptimizer-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.5.8
+Version: 0.5.9
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mloptimizer-0.5.8/README.md` & `mloptimizer-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/data/data_sample.csv` & `mloptimizer-0.5.9/data/data_sample.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/data/data_sample_test.csv` & `mloptimizer-0.5.9/data/data_sample_test.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/data/data_sample_train.csv` & `mloptimizer-0.5.9/data/data_sample_train.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/mloptimizer/alg_wrapper.py` & `mloptimizer-0.5.9/mloptimizer/alg_wrapper.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/mloptimizer/genoptimizer.py` & `mloptimizer-0.5.9/mloptimizer/genoptimizer.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/mloptimizer/miscellaneous.py` & `mloptimizer-0.5.9/mloptimizer/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/mloptimizer/model_evaluation.py` & `mloptimizer-0.5.9/mloptimizer/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/mloptimizer/plots.py` & `mloptimizer-0.5.9/mloptimizer/plots.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/mloptimizer/test/test_TreeOptimizer.py` & `mloptimizer-0.5.9/mloptimizer/test/test_TreeOptimizer.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/mloptimizer/test/test_XGBClassifierOptimizer.py` & `mloptimizer-0.5.9/mloptimizer/test/test_XGBClassifierOptimizer.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/mloptimizer/test/test_alg_wrapper.py` & `mloptimizer-0.5.9/mloptimizer/test/test_alg_wrapper.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/mloptimizer/test/test_genoptimizer.py` & `mloptimizer-0.5.9/mloptimizer/test/test_genoptimizer.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/mloptimizer/test/test_param.py` & `mloptimizer-0.5.9/mloptimizer/test/test_param.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/mloptimizer.egg-info/PKG-INFO` & `mloptimizer-0.5.9/mloptimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.5.8
+Version: 0.5.9
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mloptimizer-0.5.8/mloptimizer.egg-info/SOURCES.txt` & `mloptimizer-0.5.9/mloptimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.8/setup.py` & `mloptimizer-0.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     name="mloptimizer",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.5.8",  # Required
+    version="0.5.9",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="mloptimizer is a Python library "
                 "for optimizing hyperparameters of machine learning algorithms using genetic algorithms.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
@@ -111,25 +111,26 @@
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     install_requires=[
         "catboost>=1.1.1",
         "deap>=1.3.3",
         "joblib>=1.2.0",
-        "keras>=2.11.0",
-        "numpy>=1.24.1",
+        "keras>=2.12.0",
+        #"numpy>=1.24.1",
         "pandas>=1.5.3",
         "python-dateutil>=2.8.1",
         "pytz>=2022.7.1",
         "scikit-learn>=1.2.1",
         "scipy>=1.10.0",
         "seaborn==0.12.2",
         "six>=1.15.0",
-        "tensorflow>=2.11.0",
-        "xgboost>=1.7.3"
+        "tensorflow>=2.12.0",
+        "xgboost>=1.7.3",
+        "matplotlib~=3.7.1"
     ],  # Optional
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

