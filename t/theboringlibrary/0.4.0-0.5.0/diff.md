# Comparing `tmp/theboringlibrary-0.4.0.tar.gz` & `tmp/theboringlibrary-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theboringlibrary-0.4.0.tar", max compression
+gzip compressed data, was "theboringlibrary-0.5.0.tar", max compression
```

## Comparing `theboringlibrary-0.4.0.tar` & `theboringlibrary-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-25 07:05:38.992352 theboringlibrary-0.4.0/LICENSE
--rw-r--r--   0        0        0      219 2023-06-25 07:05:38.992352 theboringlibrary-0.4.0/README.md
--rw-r--r--   0        0        0      759 2023-06-25 07:05:38.992352 theboringlibrary-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-25 07:05:38.992352 theboringlibrary-0.4.0/src/theboringlibrary/__init__.py
--rw-r--r--   0        0        0      216 2023-06-25 07:05:38.992352 theboringlibrary-0.4.0/src/theboringlibrary/core.py
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 theboringlibrary-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-25 07:23:36.183331 theboringlibrary-0.5.0/LICENSE
+-rw-r--r--   0        0        0      219 2023-06-25 07:23:36.183331 theboringlibrary-0.5.0/README.md
+-rw-r--r--   0        0        0      839 2023-06-25 07:23:36.183331 theboringlibrary-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-25 07:23:36.183331 theboringlibrary-0.5.0/src/theboringlibrary/__init__.py
+-rw-r--r--   0        0        0      290 2023-06-25 07:23:36.183331 theboringlibrary-0.5.0/src/theboringlibrary/core.py
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 theboringlibrary-0.5.0/PKG-INFO
```

### Comparing `theboringlibrary-0.4.0/LICENSE` & `theboringlibrary-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `theboringlibrary-0.4.0/pyproject.toml` & `theboringlibrary-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "theboringlibrary"
-version = "0.4.0"
+version = "0.5.0"
 description = "It does nothing!"
 authors = ["Stefano Frassetto <frassetto.stefano@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "theboringlibrary", from = "src" }
 ]
 
@@ -23,13 +23,16 @@
     "pytest-cov",
     "coverage",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-v --cov=./src --cov-report=html --cov-append"
 
+[tool.poetry.scripts]
+theboringlibrary = "theboringlibrary.core:print_nothing"
+
 [tool.coverage.report]
 omit = ["tests"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `theboringlibrary-0.4.0/PKG-INFO` & `theboringlibrary-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theboringlibrary
-Version: 0.4.0
+Version: 0.5.0
 Summary: It does nothing!
 Author: Stefano Frassetto
 Author-email: frassetto.stefano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

