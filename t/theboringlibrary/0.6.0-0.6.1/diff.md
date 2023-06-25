# Comparing `tmp/theboringlibrary-0.6.0.tar.gz` & `tmp/theboringlibrary-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theboringlibrary-0.6.0.tar", max compression
+gzip compressed data, was "theboringlibrary-0.6.1.tar", max compression
```

## Comparing `theboringlibrary-0.6.0.tar` & `theboringlibrary-0.6.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-25 07:57:03.493673 theboringlibrary-0.6.0/LICENSE
--rw-r--r--   0        0        0      219 2023-06-25 07:57:03.493673 theboringlibrary-0.6.0/README.md
--rw-r--r--   0        0        0     1095 2023-06-25 07:57:03.493673 theboringlibrary-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-25 07:57:03.493673 theboringlibrary-0.6.0/src/theboringlibrary/__init__.py
--rw-r--r--   0        0        0      290 2023-06-25 07:57:03.493673 theboringlibrary-0.6.0/src/theboringlibrary/core.py
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 theboringlibrary-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-25 10:29:51.004037 theboringlibrary-0.6.1/LICENSE
+-rw-r--r--   0        0        0      687 2023-06-25 10:29:51.004037 theboringlibrary-0.6.1/README.md
+-rw-r--r--   0        0        0     1095 2023-06-25 10:29:51.004037 theboringlibrary-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-06-25 10:29:51.004037 theboringlibrary-0.6.1/src/theboringlibrary/__init__.py
+-rw-r--r--   0        0        0      316 2023-06-25 10:29:51.004037 theboringlibrary-0.6.1/src/theboringlibrary/core.py
+-rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 theboringlibrary-0.6.1/PKG-INFO
```

### Comparing `theboringlibrary-0.6.0/LICENSE` & `theboringlibrary-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `theboringlibrary-0.6.0/pyproject.toml` & `theboringlibrary-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "theboringlibrary"
-version = "0.6.0"
+version = "0.6.1"
 description = "It does nothing!"
 authors = ["Stefano Frassetto <frassetto.stefano@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "theboringlibrary", from = "src" }
 ]
```

