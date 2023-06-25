# Comparing `tmp/theboringlibrary-0.3.5.tar.gz` & `tmp/theboringlibrary-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theboringlibrary-0.3.5.tar", max compression
+gzip compressed data, was "theboringlibrary-0.4.0.tar", max compression
```

## Comparing `theboringlibrary-0.3.5.tar` & `theboringlibrary-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-25 05:48:28.123220 theboringlibrary-0.3.5/LICENSE
--rw-r--r--   0        0        0       37 2023-06-25 05:48:28.123220 theboringlibrary-0.3.5/README.md
--rw-r--r--   0        0        0      526 2023-06-25 05:48:28.123220 theboringlibrary-0.3.5/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-25 05:48:28.123220 theboringlibrary-0.3.5/src/theboringlibrary/__init__.py
--rw-r--r--   0        0        0      121 2023-06-25 05:48:28.123220 theboringlibrary-0.3.5/src/theboringlibrary/core.py
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 theboringlibrary-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-25 07:05:38.992352 theboringlibrary-0.4.0/LICENSE
+-rw-r--r--   0        0        0      219 2023-06-25 07:05:38.992352 theboringlibrary-0.4.0/README.md
+-rw-r--r--   0        0        0      759 2023-06-25 07:05:38.992352 theboringlibrary-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-25 07:05:38.992352 theboringlibrary-0.4.0/src/theboringlibrary/__init__.py
+-rw-r--r--   0        0        0      216 2023-06-25 07:05:38.992352 theboringlibrary-0.4.0/src/theboringlibrary/core.py
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 theboringlibrary-0.4.0/PKG-INFO
```

### Comparing `theboringlibrary-0.3.5/LICENSE` & `theboringlibrary-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `theboringlibrary-0.3.5/pyproject.toml` & `theboringlibrary-0.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 [tool.poetry]
 name = "theboringlibrary"
-version = "0.3.5"
+version = "0.4.0"
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
+pytest-cov = "^4.1.0"
+coverage = {version = "^7.2.7", extras = ["toml"]}
 
 [tool.poetry.extras]
 
 dev  = [
     "pytest",
-    "mkdocs"
+    "mkdocs",
+    "pytest-cov",
+    "coverage",
 ]
 
+[tool.pytest.ini_options]
+addopts = "-v --cov=./src --cov-report=html --cov-append"
+
+[tool.coverage.report]
+omit = ["tests"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

