# Comparing `tmp/ezelf-0.0.2.tar.gz` & `tmp/ezelf-0.0.3.tar.gz`

## Comparing `ezelf-0.0.2.tar` & `ezelf-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 ezelf-0.0.2/tox.ini
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ezelf-0.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ezelf-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ezelf-0.0.2/src/ezelf/__init__.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 ezelf-0.0.2/src/ezelf/main.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ezelf-0.0.2/src/ezelf/simple.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ezelf-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 ezelf-0.0.2/tests/test_simple.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 ezelf-0.0.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 ezelf-0.0.2/LICENSE
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ezelf-0.0.2/README.md
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 ezelf-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 ezelf-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 ezelf-0.0.3/tox.ini
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ezelf-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ezelf-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ezelf-0.0.3/src/ezelf/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ezelf-0.0.3/src/ezelf/__main__.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 ezelf-0.0.3/src/ezelf/main.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ezelf-0.0.3/src/ezelf/simple.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ezelf-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 ezelf-0.0.3/tests/test_simple.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 ezelf-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 ezelf-0.0.3/LICENSE
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ezelf-0.0.3/README.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 ezelf-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 ezelf-0.0.3/PKG-INFO
```

### Comparing `ezelf-0.0.2/tox.ini` & `ezelf-0.0.3/tox.ini`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.2/.github/workflows/release.yml` & `ezelf-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.2/.github/workflows/test.yml` & `ezelf-0.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.2/src/ezelf/main.py` & `ezelf-0.0.3/src/ezelf/main.py`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.2/.gitignore` & `ezelf-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.2/LICENSE` & `ezelf-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.2/PKG-INFO` & `ezelf-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezelf
-Version: 0.0.2
+Version: 0.0.3
 Summary: A elf for ezpie
 License: MIT License
         
         Copyright (c) 2023 ez-pie
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -24,11 +24,11 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: typer
+Requires-Dist: typer[all]
 Description-Content-Type: text/markdown
 
 # ez-elf
```

