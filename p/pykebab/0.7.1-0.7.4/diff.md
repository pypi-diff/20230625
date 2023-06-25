# Comparing `tmp/pykebab-0.7.1.tar.gz` & `tmp/pykebab-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykebab-0.7.1.tar", max compression
+gzip compressed data, was "pykebab-0.7.4.tar", max compression
```

## Comparing `pykebab-0.7.1.tar` & `pykebab-0.7.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      821 2022-11-06 03:32:21.214628 pykebab-0.7.1/kebab/__init__.py
--rw-r--r--   0        0        0     3920 2022-11-06 03:32:21.214802 pykebab-0.7.1/kebab/aws.py
--rw-r--r--   0        0        0       40 2022-11-06 03:32:21.214897 pykebab-0.7.1/kebab/cli/__init__.py
--rw-r--r--   0        0        0     1801 2023-01-05 03:45:44.147407 pykebab-0.7.1/kebab/cli/cli.py
--rw-r--r--   0        0        0      798 2023-02-03 08:02:22.409418 pykebab-0.7.1/kebab/constants.py
--rw-r--r--   0        0        0       42 2022-11-06 03:32:21.215088 pykebab-0.7.1/kebab/exceptions.py
--rw-r--r--   0        0        0     2587 2023-01-05 03:45:44.147717 pykebab-0.7.1/kebab/k8s.py
--rw-r--r--   0        0        0      773 2023-03-28 07:51:19.037015 pykebab-0.7.1/kebab/loader.py
--rw-r--r--   0        0        0     2381 2023-06-21 14:37:29.161728 pykebab-0.7.1/kebab/magic.py
--rw-r--r--   0        0        0     2108 2023-03-25 11:13:55.662982 pykebab-0.7.1/kebab/openers.py
--rw-r--r--   0        0        0    21801 2023-06-25 17:48:09.649543 pykebab-0.7.1/kebab/sources.py
--rw-r--r--   0        0        0     4825 2023-01-05 03:45:44.148106 pykebab-0.7.1/kebab/utils.py
--rw-r--r--   0        0        0     1025 2023-06-25 17:57:18.409306 pykebab-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/__init__.py
+-rw-r--r--   0        0        0     3920 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/aws.py
+-rw-r--r--   0        0        0       40 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/cli/__init__.py
+-rw-r--r--   0        0        0     1801 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/cli/cli.py
+-rw-r--r--   0        0        0      798 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/constants.py
+-rw-r--r--   0        0        0       42 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/exceptions.py
+-rw-r--r--   0        0        0     2587 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/k8s.py
+-rw-r--r--   0        0        0      773 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/loader.py
+-rw-r--r--   0        0        0     2368 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/magic.py
+-rw-r--r--   0        0        0     2108 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/openers.py
+-rw-r--r--   0        0        0    21801 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/sources.py
+-rw-r--r--   0        0        0     4825 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/utils.py
+-rw-r--r--   0        0        0     1025 2023-06-25 18:26:03.118172 pykebab-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.7.4/PKG-INFO
```

### Comparing `pykebab-0.7.1/kebab/__init__.py` & `pykebab-0.7.4/kebab/__init__.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.1/kebab/aws.py` & `pykebab-0.7.4/kebab/aws.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.1/kebab/cli/cli.py` & `pykebab-0.7.4/kebab/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.1/kebab/constants.py` & `pykebab-0.7.4/kebab/constants.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.1/kebab/k8s.py` & `pykebab-0.7.4/kebab/k8s.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.1/kebab/loader.py` & `pykebab-0.7.4/kebab/loader.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.1/kebab/magic.py` & `pykebab-0.7.4/kebab/magic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import time
-
 from kebab.sources import KebabSource, literal
 
 
 class Field:
     def __init__(
         self,
         config_name=None,
```

### Comparing `pykebab-0.7.1/kebab/openers.py` & `pykebab-0.7.4/kebab/openers.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.1/kebab/sources.py` & `pykebab-0.7.4/kebab/sources.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.1/kebab/utils.py` & `pykebab-0.7.4/kebab/utils.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.1/pyproject.toml` & `pykebab-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykebab"
-version = "0.7.1"
+version = "0.7.4"
 description = ""
 authors = ["Yangming Huang <leonmax@gmail.com>"]
 packages = [
     { include = "kebab" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `pykebab-0.7.1/PKG-INFO` & `pykebab-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykebab
-Version: 0.7.1
+Version: 0.7.4
 Summary: 
 Author: Yangming Huang
 Author-email: leonmax@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

