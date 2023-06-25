# Comparing `tmp/theboringlibrary-0.6.3.tar.gz` & `tmp/theboringlibrary-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theboringlibrary-0.6.3.tar", max compression
+gzip compressed data, was "theboringlibrary-0.6.4.tar", max compression
```

## Comparing `theboringlibrary-0.6.3.tar` & `theboringlibrary-0.6.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-25 11:00:59.760021 theboringlibrary-0.6.3/LICENSE
--rw-r--r--   0        0        0      687 2023-06-25 11:00:59.760021 theboringlibrary-0.6.3/README.md
--rw-r--r--   0        0        0     1095 2023-06-25 11:00:59.760021 theboringlibrary-0.6.3/pyproject.toml
--rw-r--r--   0        0        0       56 2023-06-25 11:00:59.760021 theboringlibrary-0.6.3/src/theboringlibrary/__init__.py
--rw-r--r--   0        0        0      316 2023-06-25 11:00:59.764021 theboringlibrary-0.6.3/src/theboringlibrary/core.py
--rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 theboringlibrary-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-25 11:09:29.090710 theboringlibrary-0.6.4/LICENSE
+-rw-r--r--   0        0        0      687 2023-06-25 11:09:29.090710 theboringlibrary-0.6.4/README.md
+-rw-r--r--   0        0        0     1095 2023-06-25 11:09:29.090710 theboringlibrary-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-06-25 11:09:29.090710 theboringlibrary-0.6.4/src/theboringlibrary/__init__.py
+-rw-r--r--   0        0        0      316 2023-06-25 11:09:29.094710 theboringlibrary-0.6.4/src/theboringlibrary/core.py
+-rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 theboringlibrary-0.6.4/PKG-INFO
```

### Comparing `theboringlibrary-0.6.3/LICENSE` & `theboringlibrary-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `theboringlibrary-0.6.3/README.md` & `theboringlibrary-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `theboringlibrary-0.6.3/pyproject.toml` & `theboringlibrary-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "theboringlibrary"
-version = "0.6.3"
+version = "0.6.4"
 description = "It does nothing!"
 authors = ["Stefano Frassetto <frassetto.stefano@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "theboringlibrary", from = "src" }
 ]
```

### Comparing `theboringlibrary-0.6.3/PKG-INFO` & `theboringlibrary-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theboringlibrary
-Version: 0.6.3
+Version: 0.6.4
 Summary: It does nothing!
 Author: Stefano Frassetto
 Author-email: frassetto.stefano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: theboringlibrary Version: 0.6.3 Summary: It does
+Metadata-Version: 2.1 Name: theboringlibrary Version: 0.6.4 Summary: It does
 nothing! Author: Stefano Frassetto Author-email: frassetto.stefano@gmail.com
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: dev Requires-Dist: coverage[toml]
 (>=7.2.7,<8.0.0) ; extra == "dev" Requires-Dist: mkdocs (>=1.4.3,<2.0.0) ;
 extra == "dev" Requires-Dist: mkdocs-gen-files (>=0.5.0,<0.6.0) ; extra ==
 "dev" Requires-Dist: mkdocs-material (>=9.1.17,<10.0.0) ; extra == "dev"
```

