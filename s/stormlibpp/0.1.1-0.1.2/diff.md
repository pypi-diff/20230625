# Comparing `tmp/stormlibpp-0.1.1.tar.gz` & `tmp/stormlibpp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stormlibpp-0.1.1.tar", last modified: Sat Jun 24 18:41:55 2023, max compression
+gzip compressed data, was "stormlibpp-0.1.2.tar", last modified: Sun Jun 25 16:32:57 2023, max compression
```

## Comparing `stormlibpp-0.1.1.tar` & `stormlibpp-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:41:55.004569 stormlibpp-0.1.1/
--rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-24 17:20:21.000000 stormlibpp-0.1.1/LICENSE
--rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-24 18:41:55.004427 stormlibpp-0.1.1/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      108 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/README.md
--rw-r--r--   0 gormo      (501) staff       (20)      557 2023-06-24 18:41:50.000000 stormlibpp-0.1.1/pyproject.toml
--rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-24 18:41:55.004613 stormlibpp-0.1.1/setup.cfg
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:41:55.001406 stormlibpp-0.1.1/src/
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:41:55.002697 stormlibpp-0.1.1/src/stormlibpp/
--rw-r--r--   0 gormo      (501) staff       (20)      566 2023-06-24 18:41:50.000000 stormlibpp-0.1.1/src/stormlibpp/__init__.py
--rw-r--r--   0 gormo      (501) staff       (20)      448 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/src/stormlibpp/errors.py
--rw-r--r--   0 gormo      (501) staff       (20)     5746 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/src/stormlibpp/stormpkg.py
--rw-r--r--   0 gormo      (501) staff       (20)     1396 2023-06-24 18:39:56.000000 stormlibpp-0.1.1/src/stormlibpp/telepath.py
--rw-r--r--   0 gormo      (501) staff       (20)      618 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/src/stormlibpp/utils.py
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:41:55.003487 stormlibpp-0.1.1/src/stormlibpp.egg-info/
--rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-24 18:41:54.000000 stormlibpp-0.1.1/src/stormlibpp.egg-info/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      417 2023-06-24 18:41:55.000000 stormlibpp-0.1.1/src/stormlibpp.egg-info/SOURCES.txt
--rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-24 18:41:54.000000 stormlibpp-0.1.1/src/stormlibpp.egg-info/dependency_links.txt
--rw-r--r--   0 gormo      (501) staff       (20)       17 2023-06-24 18:41:54.000000 stormlibpp-0.1.1/src/stormlibpp.egg-info/requires.txt
--rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-24 18:41:54.000000 stormlibpp-0.1.1/src/stormlibpp.egg-info/top_level.txt
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:41:55.004207 stormlibpp-0.1.1/tests/
--rw-r--r--   0 gormo      (501) staff       (20)     1241 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/tests/test_stormpkg.py
--rw-r--r--   0 gormo      (501) staff       (20)      720 2023-06-24 18:41:02.000000 stormlibpp-0.1.1/tests/test_telepath.py
--rw-r--r--   0 gormo      (501) staff       (20)      419 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 16:32:57.509036 stormlibpp-0.1.2/
+-rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-24 17:20:21.000000 stormlibpp-0.1.2/LICENSE
+-rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-25 16:32:57.508900 stormlibpp-0.1.2/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      108 2023-06-24 18:31:15.000000 stormlibpp-0.1.2/README.md
+-rw-r--r--   0 gormo      (501) staff       (20)      557 2023-06-25 16:32:52.000000 stormlibpp-0.1.2/pyproject.toml
+-rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-25 16:32:57.509079 stormlibpp-0.1.2/setup.cfg
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 16:32:57.506551 stormlibpp-0.1.2/src/
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 16:32:57.507672 stormlibpp-0.1.2/src/stormlibpp/
+-rw-r--r--   0 gormo      (501) staff       (20)      604 2023-06-25 16:32:52.000000 stormlibpp-0.1.2/src/stormlibpp/__init__.py
+-rw-r--r--   0 gormo      (501) staff       (20)      663 2023-06-25 16:25:46.000000 stormlibpp-0.1.2/src/stormlibpp/errors.py
+-rw-r--r--   0 gormo      (501) staff       (20)     8097 2023-06-25 16:31:12.000000 stormlibpp-0.1.2/src/stormlibpp/stormpkg.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1289 2023-06-24 18:47:22.000000 stormlibpp-0.1.2/src/stormlibpp/telepath.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1465 2023-06-25 16:27:18.000000 stormlibpp-0.1.2/src/stormlibpp/utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 16:32:57.508291 stormlibpp-0.1.2/src/stormlibpp.egg-info/
+-rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-25 16:32:57.000000 stormlibpp-0.1.2/src/stormlibpp.egg-info/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      417 2023-06-25 16:32:57.000000 stormlibpp-0.1.2/src/stormlibpp.egg-info/SOURCES.txt
+-rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-25 16:32:57.000000 stormlibpp-0.1.2/src/stormlibpp.egg-info/dependency_links.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       17 2023-06-25 16:32:57.000000 stormlibpp-0.1.2/src/stormlibpp.egg-info/requires.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-25 16:32:57.000000 stormlibpp-0.1.2/src/stormlibpp.egg-info/top_level.txt
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 16:32:57.508690 stormlibpp-0.1.2/tests/
+-rw-r--r--   0 gormo      (501) staff       (20)     1644 2023-06-25 16:20:13.000000 stormlibpp-0.1.2/tests/test_stormpkg.py
+-rw-r--r--   0 gormo      (501) staff       (20)      481 2023-06-24 18:47:22.000000 stormlibpp-0.1.2/tests/test_telepath.py
+-rw-r--r--   0 gormo      (501) staff       (20)      419 2023-06-24 18:31:15.000000 stormlibpp-0.1.2/tests/test_utils.py
```

### Comparing `stormlibpp-0.1.1/LICENSE` & `stormlibpp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stormlibpp-0.1.1/PKG-INFO` & `stormlibpp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormlibpp
-Version: 0.1.1
+Version: 0.1.2
 Summary: The stormlibpp Python package
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stormlibpp-0.1.1/pyproject.toml` & `stormlibpp-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stormlibpp"
-version = "0.1.1"
+version = "0.1.2"
 description = "The stormlibpp Python package"
 readme = "README.md"
 requires-python = ">=3.11"
 
 # Fill in dependencies here.
 dependencies = [
     "synapse==2.139.0"
```

### Comparing `stormlibpp-0.1.1/src/stormlibpp/__init__.py` & `stormlibpp-0.1.2/src/stormlibpp/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 
     synapse.common -> s_common
     synapse.exc -> s_exc
     synapse.genpkg -> s_genpkg
 
 """
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 
 import synapse.common as s_common
 import synapse.exc as s_exc
 import synapse.tools.genpkg as s_genpkg
+import synapse.lib.parser as s_parser
 
 from . import errors
 from . import utils
 from .stormpkg import StormPkg
 from .telepath import (genDefaultTelepathRetn, TelepathRetn)
```

### Comparing `stormlibpp-0.1.1/src/stormlibpp/telepath.py` & `stormlibpp-0.1.2/src/stormlibpp/telepath.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,12 +32,7 @@
     """Generate a default TelepathRetn return object, or the given subclass.
 
     Default values have a ``status`` of ``True``, an empty ``mesg``, and
     ``data`` is set to the ``default_data`` arg - which defaults to ``None``.
     """
 
     return obj(status=True, mesg="", data=default_data)
-
-
-class BoolRetn(TelepathRetn):
-    """A TelepathRetn where ``data`` is a boolean value."""
-    data: bool
```

### Comparing `stormlibpp-0.1.1/src/stormlibpp.egg-info/PKG-INFO` & `stormlibpp-0.1.2/src/stormlibpp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormlibpp
-Version: 0.1.1
+Version: 0.1.2
 Summary: The stormlibpp Python package
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

