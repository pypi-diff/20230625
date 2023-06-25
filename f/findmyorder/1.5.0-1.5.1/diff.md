# Comparing `tmp/findmyorder-1.5.0.tar.gz` & `tmp/findmyorder-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.5.0.tar", max compression
+gzip compressed data, was "findmyorder-1.5.1.tar", max compression
```

## Comparing `findmyorder-1.5.0.tar` & `findmyorder-1.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-25 19:44:47.031006 findmyorder-1.5.0/LICENSE
--rw-r--r--   0        0        0     1995 2023-06-25 19:44:47.031006 findmyorder-1.5.0/README.md
--rw-r--r--   0        0        0      113 2023-06-25 19:44:47.859005 findmyorder-1.5.0/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-06-25 19:44:47.031006 findmyorder-1.5.0/findmyorder/config.py
--rw-r--r--   0        0        0     2265 2023-06-25 19:44:47.031006 findmyorder-1.5.0/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5555 2023-06-25 19:44:47.031006 findmyorder-1.5.0/findmyorder/main.py
--rw-r--r--   0        0        0     2132 2023-06-25 19:44:47.859005 findmyorder-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-25 20:15:21.306655 findmyorder-1.5.1/LICENSE
+-rw-r--r--   0        0        0     1995 2023-06-25 20:15:21.306655 findmyorder-1.5.1/README.md
+-rw-r--r--   0        0        0      113 2023-06-25 20:15:22.022675 findmyorder-1.5.1/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-06-25 20:15:21.306655 findmyorder-1.5.1/findmyorder/config.py
+-rw-r--r--   0        0        0     2265 2023-06-25 20:15:21.306655 findmyorder-1.5.1/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5555 2023-06-25 20:15:21.306655 findmyorder-1.5.1/findmyorder/main.py
+-rw-r--r--   0        0        0     2132 2023-06-25 20:15:22.022675 findmyorder-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.5.1/PKG-INFO
```

### Comparing `findmyorder-1.5.0/LICENSE` & `findmyorder-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.0/README.md` & `findmyorder-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.0/findmyorder/config.py` & `findmyorder-1.5.1/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.0/findmyorder/default_settings.toml` & `findmyorder-1.5.1/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.0/findmyorder/main.py` & `findmyorder-1.5.1/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.0/pyproject.toml` & `findmyorder-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.5.0"
+version = "1.5.1"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
```

### Comparing `findmyorder-1.5.0/PKG-INFO` & `findmyorder-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.5.0
+Version: 1.5.1
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

