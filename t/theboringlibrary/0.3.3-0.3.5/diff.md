# Comparing `tmp/theboringlibrary-0.3.3.tar.gz` & `tmp/theboringlibrary-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theboringlibrary-0.3.3.tar", max compression
+gzip compressed data, was "theboringlibrary-0.3.5.tar", max compression
```

## Comparing `theboringlibrary-0.3.3.tar` & `theboringlibrary-0.3.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-24 20:23:51.766579 theboringlibrary-0.3.3/LICENSE
--rw-r--r--   0        0        0       37 2023-06-24 20:23:51.766579 theboringlibrary-0.3.3/README.md
--rw-r--r--   0        0        0      526 2023-06-24 20:23:51.770579 theboringlibrary-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-24 20:23:51.770579 theboringlibrary-0.3.3/src/theboringlibrary/__init__.py
--rw-r--r--   0        0        0      121 2023-06-24 20:23:51.770579 theboringlibrary-0.3.3/src/theboringlibrary/core.py
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 theboringlibrary-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-25 05:48:28.123220 theboringlibrary-0.3.5/LICENSE
+-rw-r--r--   0        0        0       37 2023-06-25 05:48:28.123220 theboringlibrary-0.3.5/README.md
+-rw-r--r--   0        0        0      526 2023-06-25 05:48:28.123220 theboringlibrary-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-25 05:48:28.123220 theboringlibrary-0.3.5/src/theboringlibrary/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-25 05:48:28.123220 theboringlibrary-0.3.5/src/theboringlibrary/core.py
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 theboringlibrary-0.3.5/PKG-INFO
```

### Comparing `theboringlibrary-0.3.3/LICENSE` & `theboringlibrary-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `theboringlibrary-0.3.3/pyproject.toml` & `theboringlibrary-0.3.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "theboringlibrary"
-version = "0.3.3"
+version = "0.3.5"
 description = "It does nothing!"
 authors = ["Stefano Frassetto <frassetto.stefano@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "theboringlibrary", from = "src" }
 ]
```

### Comparing `theboringlibrary-0.3.3/PKG-INFO` & `theboringlibrary-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theboringlibrary
-Version: 0.3.3
+Version: 0.3.5
 Summary: It does nothing!
 Author: Stefano Frassetto
 Author-email: frassetto.stefano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

