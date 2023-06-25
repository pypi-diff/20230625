# Comparing `tmp/theboringlibrary-0.5.0.tar.gz` & `tmp/theboringlibrary-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theboringlibrary-0.5.0.tar", max compression
+gzip compressed data, was "theboringlibrary-0.6.0.tar", max compression
```

## Comparing `theboringlibrary-0.5.0.tar` & `theboringlibrary-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-25 07:23:36.183331 theboringlibrary-0.5.0/LICENSE
--rw-r--r--   0        0        0      219 2023-06-25 07:23:36.183331 theboringlibrary-0.5.0/README.md
--rw-r--r--   0        0        0      839 2023-06-25 07:23:36.183331 theboringlibrary-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-25 07:23:36.183331 theboringlibrary-0.5.0/src/theboringlibrary/__init__.py
--rw-r--r--   0        0        0      290 2023-06-25 07:23:36.183331 theboringlibrary-0.5.0/src/theboringlibrary/core.py
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 theboringlibrary-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-25 07:57:03.493673 theboringlibrary-0.6.0/LICENSE
+-rw-r--r--   0        0        0      219 2023-06-25 07:57:03.493673 theboringlibrary-0.6.0/README.md
+-rw-r--r--   0        0        0     1095 2023-06-25 07:57:03.493673 theboringlibrary-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-25 07:57:03.493673 theboringlibrary-0.6.0/src/theboringlibrary/__init__.py
+-rw-r--r--   0        0        0      290 2023-06-25 07:57:03.493673 theboringlibrary-0.6.0/src/theboringlibrary/core.py
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 theboringlibrary-0.6.0/PKG-INFO
```

### Comparing `theboringlibrary-0.5.0/LICENSE` & `theboringlibrary-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `theboringlibrary-0.5.0/pyproject.toml` & `theboringlibrary-0.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 [tool.poetry]
 name = "theboringlibrary"
-version = "0.5.0"
+version = "0.6.0"
 description = "It does nothing!"
 authors = ["Stefano Frassetto <frassetto.stefano@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "theboringlibrary", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pytest = {version = "^7.3.2", optional = true}
 mkdocs = {version = "^1.4.3", optional = true}
 pytest-cov = "^4.1.0"
 coverage = {version = "^7.2.7", extras = ["toml"]}
+mkdocs-material = {version = "^9.1.17", optional = true}
+mkdocs-gen-files = {version = "^0.5.0", optional = true}
+mkdocstrings = {version = "^0.22.0", optional = true, extras = ["python"]}
 
 [tool.poetry.extras]
 
 dev  = [
     "pytest",
     "mkdocs",
     "pytest-cov",
     "coverage",
+    "mkdocs-material",
+    "mkdocstrings",
+    "mkdocs-gen-files",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-v --cov=./src --cov-report=html --cov-append"
 
 [tool.poetry.scripts]
 theboringlibrary = "theboringlibrary.core:print_nothing"
```

### Comparing `theboringlibrary-0.5.0/PKG-INFO` & `theboringlibrary-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: theboringlibrary
-Version: 0.5.0
+Version: 0.6.0
 Summary: It does nothing!
 Author: Stefano Frassetto
 Author-email: frassetto.stefano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Requires-Dist: coverage[toml] (>=7.2.7,<8.0.0) ; extra == "dev"
 Requires-Dist: mkdocs (>=1.4.3,<2.0.0) ; extra == "dev"
+Requires-Dist: mkdocs-gen-files (>=0.5.0,<0.6.0) ; extra == "dev"
+Requires-Dist: mkdocs-material (>=9.1.17,<10.0.0) ; extra == "dev"
+Requires-Dist: mkdocstrings[python] (>=0.22.0,<0.23.0) ; extra == "dev"
 Requires-Dist: pytest (>=7.3.2,<8.0.0) ; extra == "dev"
 Requires-Dist: pytest-cov (>=4.1.0,<5.0.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 [![codecov](https://codecov.io/gh/stefanondisponibile/theboringlibrary/branch/develop/graph/badge.svg?token=8VHJ01UKLX)](https://codecov.io/gh/stefanondisponibile/theboringlibrary)
 
 # theboringlibrary
```

