# Comparing `tmp/erroraffirmations-0.1.0rc0.tar.gz` & `tmp/erroraffirmations-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erroraffirmations-0.1.0rc0.tar", last modified: Sun Jun 25 10:41:51 2023, max compression
+gzip compressed data, was "erroraffirmations-0.1.0rc1.tar", last modified: Sun Jun 25 11:50:16 2023, max compression
```

## Comparing `erroraffirmations-0.1.0rc0.tar` & `erroraffirmations-0.1.0rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:41:51.298630 erroraffirmations-0.1.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-25 10:41:42.000000 erroraffirmations-0.1.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-25 10:41:51.298630 erroraffirmations-0.1.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-25 10:41:42.000000 erroraffirmations-0.1.0rc0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:41:51.298630 erroraffirmations-0.1.0rc0/erroraffirmations/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-25 10:41:42.000000 erroraffirmations-0.1.0rc0/erroraffirmations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-25 10:41:42.000000 erroraffirmations-0.1.0rc0/erroraffirmations/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-06-25 10:41:42.000000 erroraffirmations-0.1.0rc0/erroraffirmations/affirmations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:41:51.298630 erroraffirmations-0.1.0rc0/erroraffirmations/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-25 10:41:42.000000 erroraffirmations-0.1.0rc0/erroraffirmations/data/affirmations.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:41:51.298630 erroraffirmations-0.1.0rc0/erroraffirmations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-25 10:41:51.000000 erroraffirmations-0.1.0rc0/erroraffirmations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 10:41:51.000000 erroraffirmations-0.1.0rc0/erroraffirmations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 10:41:51.000000 erroraffirmations-0.1.0rc0/erroraffirmations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-25 10:41:51.000000 erroraffirmations-0.1.0rc0/erroraffirmations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 10:41:51.000000 erroraffirmations-0.1.0rc0/erroraffirmations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 10:41:51.000000 erroraffirmations-0.1.0rc0/erroraffirmations.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-25 10:41:42.000000 erroraffirmations-0.1.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-25 10:41:51.298630 erroraffirmations-0.1.0rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:41:51.298630 erroraffirmations-0.1.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-25 10:41:42.000000 erroraffirmations-0.1.0rc0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-25 10:41:42.000000 erroraffirmations-0.1.0rc0/tests/test_functionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-06-25 10:41:42.000000 erroraffirmations-0.1.0rc0/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/erroraffirmations/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/erroraffirmations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/erroraffirmations/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/erroraffirmations/affirmations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/erroraffirmations/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/erroraffirmations/data/affirmations.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/tests/test_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/tests/test_interface.py
```

### Comparing `erroraffirmations-0.1.0rc0/LICENSE` & `erroraffirmations-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `erroraffirmations-0.1.0rc0/PKG-INFO` & `erroraffirmations-0.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erroraffirmations
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: Affirmative error messages for Python
 Author-email: Thomas Gessey-Jones <thomasgesseyjones@gmail.com>
 Maintainer-email: Thomas Gessey-Jones <thomasgesseyjones@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Thomas Gessey-Jones
         
@@ -31,37 +31,41 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Bug Tracking
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 ========================================================
 ErrorAffirmations: Affirmative error messages for Python
 ========================================================
 
 Introduction
 ------------
 
 :ErrorAffirmations: Affirmative error messages for Python
 :Author: Thomas Gessey-Jones
-:Version: 0.1.0-rc
+:Version: 0.1.0-rc.1
 :Homepage: https://github.com/ThomasGesseyJones/ErrorAffirmations
 
 .. image:: https://img.shields.io/badge/python-3.7+-blue.svg
    :target: https://www.python.org/downloads/
    :alt: Python version
 .. image:: https://github.com/ThomasGesseyJones/ErrorAffirmations/actions/workflows/CI.yaml/badge.svg
    :target: https://github.com/ThomasGesseyJones/ErrorAffirmations/actions/workflows/CI.yaml
    :alt: Testing Status
 .. image:: https://codecov.io/gh/ThomasGesseyJones/ErrorAffirmations/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/ThomasGesseyJones/ErrorAffirmations
    :alt: Test Coverage Status
+.. image:: https://readthedocs.org/projects/erroraffirmations/badge/?version=latest
+   :target: https://erroraffirmations.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg
    :target: https://github.com/ThomasGesseyJones/ErrorAffirmations/blob/main/LICENSE
    :alt: License information
 
 
 ``ErrorAffirmations`` is a Python library that provides affirmative error messages, to help you feel better about your
 errors.
```

### Comparing `erroraffirmations-0.1.0rc0/README.rst` & `erroraffirmations-0.1.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 ========================================================
 
 Introduction
 ------------
 
 :ErrorAffirmations: Affirmative error messages for Python
 :Author: Thomas Gessey-Jones
-:Version: 0.1.0-rc
+:Version: 0.1.0-rc.1
 :Homepage: https://github.com/ThomasGesseyJones/ErrorAffirmations
 
 .. image:: https://img.shields.io/badge/python-3.7+-blue.svg
    :target: https://www.python.org/downloads/
    :alt: Python version
 .. image:: https://github.com/ThomasGesseyJones/ErrorAffirmations/actions/workflows/CI.yaml/badge.svg
    :target: https://github.com/ThomasGesseyJones/ErrorAffirmations/actions/workflows/CI.yaml
    :alt: Testing Status
 .. image:: https://codecov.io/gh/ThomasGesseyJones/ErrorAffirmations/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/ThomasGesseyJones/ErrorAffirmations
    :alt: Test Coverage Status
+.. image:: https://readthedocs.org/projects/erroraffirmations/badge/?version=latest
+   :target: https://erroraffirmations.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg
    :target: https://github.com/ThomasGesseyJones/ErrorAffirmations/blob/main/LICENSE
    :alt: License information
 
 
 ``ErrorAffirmations`` is a Python library that provides affirmative error messages, to help you feel better about your
 errors.
```

### Comparing `erroraffirmations-0.1.0rc0/erroraffirmations/affirmations.py` & `erroraffirmations-0.1.0rc1/erroraffirmations/affirmations.py`

 * *Files identical despite different names*

### Comparing `erroraffirmations-0.1.0rc0/erroraffirmations/data/affirmations.txt` & `erroraffirmations-0.1.0rc1/erroraffirmations/data/affirmations.txt`

 * *Files identical despite different names*

### Comparing `erroraffirmations-0.1.0rc0/erroraffirmations.egg-info/PKG-INFO` & `erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erroraffirmations
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: Affirmative error messages for Python
 Author-email: Thomas Gessey-Jones <thomasgesseyjones@gmail.com>
 Maintainer-email: Thomas Gessey-Jones <thomasgesseyjones@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Thomas Gessey-Jones
         
@@ -31,37 +31,41 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Bug Tracking
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 ========================================================
 ErrorAffirmations: Affirmative error messages for Python
 ========================================================
 
 Introduction
 ------------
 
 :ErrorAffirmations: Affirmative error messages for Python
 :Author: Thomas Gessey-Jones
-:Version: 0.1.0-rc
+:Version: 0.1.0-rc.1
 :Homepage: https://github.com/ThomasGesseyJones/ErrorAffirmations
 
 .. image:: https://img.shields.io/badge/python-3.7+-blue.svg
    :target: https://www.python.org/downloads/
    :alt: Python version
 .. image:: https://github.com/ThomasGesseyJones/ErrorAffirmations/actions/workflows/CI.yaml/badge.svg
    :target: https://github.com/ThomasGesseyJones/ErrorAffirmations/actions/workflows/CI.yaml
    :alt: Testing Status
 .. image:: https://codecov.io/gh/ThomasGesseyJones/ErrorAffirmations/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/ThomasGesseyJones/ErrorAffirmations
    :alt: Test Coverage Status
+.. image:: https://readthedocs.org/projects/erroraffirmations/badge/?version=latest
+   :target: https://erroraffirmations.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg
    :target: https://github.com/ThomasGesseyJones/ErrorAffirmations/blob/main/LICENSE
    :alt: License information
 
 
 ``ErrorAffirmations`` is a Python library that provides affirmative error messages, to help you feel better about your
 errors.
```

### Comparing `erroraffirmations-0.1.0rc0/pyproject.toml` & `erroraffirmations-0.1.0rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -26,10 +26,11 @@
 [project.urls]
 "Homepage" = "https://github.com/ThomasGesseyJones/ErrorAffirmations"
 "Bug Tracker" = "https://github.com/ThomasGesseyJones/ErrorAffirmations/issues"
 
 [project.optional-dependencies]
 test = ["packaging", "flake8", "pydocstyle", "pytest", "pytest-cov",
     "pre-commit"]
+docs = ["sphinx", "sphinx_rtd_theme", "numpydoc"]
 
 [tool.setuptools.dynamic]
 version = {attr = "erroraffirmations._version.__version__"}
```

### Comparing `erroraffirmations-0.1.0rc0/tests/test_examples.py` & `erroraffirmations-0.1.0rc1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `erroraffirmations-0.1.0rc0/tests/test_functionality.py` & `erroraffirmations-0.1.0rc1/tests/test_functionality.py`

 * *Files identical despite different names*

### Comparing `erroraffirmations-0.1.0rc0/tests/test_interface.py` & `erroraffirmations-0.1.0rc1/tests/test_interface.py`

 * *Files identical despite different names*

