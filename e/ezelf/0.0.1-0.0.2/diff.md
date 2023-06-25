# Comparing `tmp/ezelf-0.0.1.tar.gz` & `tmp/ezelf-0.0.2.tar.gz`

## Comparing `ezelf-0.0.1.tar` & `ezelf-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 ezelf-0.0.1/tox.ini
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ezelf-0.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ezelf-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ezelf-0.0.1/src/ezelf/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ezelf-0.0.1/src/ezelf/simple.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ezelf-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 ezelf-0.0.1/tests/test_simple.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 ezelf-0.0.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 ezelf-0.0.1/LICENSE
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ezelf-0.0.1/README.md
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 ezelf-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ezelf-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 ezelf-0.0.2/tox.ini
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ezelf-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ezelf-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ezelf-0.0.2/src/ezelf/__init__.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 ezelf-0.0.2/src/ezelf/main.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ezelf-0.0.2/src/ezelf/simple.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ezelf-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 ezelf-0.0.2/tests/test_simple.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 ezelf-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 ezelf-0.0.2/LICENSE
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ezelf-0.0.2/README.md
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 ezelf-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 ezelf-0.0.2/PKG-INFO
```

### Comparing `ezelf-0.0.1/tox.ini` & `ezelf-0.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.1/.github/workflows/test.yml` & `ezelf-0.0.2/.github/workflows/test.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # this file is *not* meant to cover or endorse the use of GitHub Actions, but rather to
 # help test this project
 
 name: Test
 
-on: [push, pull_request]
+on:
+  push:
+    branches: [ "main" ]
+  pull_request:
+    branches: [ "main" ]
 
 jobs:
   test:
     strategy:
       matrix:
         python: ['3.7', '3.8', '3.9', '3.10']
         platform: [ubuntu-latest, macos-latest, windows-latest]
     runs-on: ${{ matrix.platform }}
     steps:
-    - name: Checkout
-      uses: actions/checkout@v3
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python }}
     - name: Install test dependencies
       run: python -m pip install -U tox
     - name: Test
```

### Comparing `ezelf-0.0.1/.gitignore` & `ezelf-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.1/LICENSE` & `ezelf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.1/PKG-INFO` & `ezelf-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezelf
-Version: 0.0.1
+Version: 0.0.2
 Summary: A elf for ezpie
 License: MIT License
         
         Copyright (c) 2023 ez-pie
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -24,10 +24,11 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: typer
 Description-Content-Type: text/markdown
 
 # ez-elf
```

