# Comparing `tmp/datawise-0.0.20.tar.gz` & `tmp/datawise-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.20.tar", max compression
+gzip compressed data, was "datawise-0.0.21.tar", max compression
```

## Comparing `datawise-0.0.20.tar` & `datawise-0.0.21.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.20/LICENSE
--rw-r--r--   0        0        0     6750 2023-06-24 02:47:18.454410 datawise-0.0.20/README.md
--rw-r--r--   0        0        0     5600 2023-06-20 11:36:16.459385 datawise-0.0.20/datawise/__init__.py
--rw-r--r--   0        0        0      636 2023-06-20 11:29:08.510434 datawise-0.0.20/datawise/exceptions.py
--rw-r--r--   0        0        0      589 2023-06-24 02:47:02.780550 datawise-0.0.20/pyproject.toml
--rw-r--r--   0        0        0     7308 1970-01-01 00:00:00.000000 datawise-0.0.20/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.21/LICENSE
+-rw-r--r--   0        0        0     6750 2023-06-24 02:47:18.454410 datawise-0.0.21/README.md
+-rw-r--r--   0        0        0     5600 2023-06-20 11:36:16.459385 datawise-0.0.21/datawise/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-25 18:46:09.256341 datawise-0.0.21/datawise/exceptions.py
+-rw-r--r--   0        0        0      589 2023-06-25 18:50:43.652759 datawise-0.0.21/pyproject.toml
+-rw-r--r--   0        0        0     7308 1970-01-01 00:00:00.000000 datawise-0.0.21/PKG-INFO
```

### Comparing `datawise-0.0.20/LICENSE` & `datawise-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.20/README.md` & `datawise-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `datawise-0.0.20/datawise/__init__.py` & `datawise-0.0.21/datawise/__init__.py`

 * *Files identical despite different names*

### Comparing `datawise-0.0.20/datawise/exceptions.py` & `datawise-0.0.21/datawise/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,16 @@
     self.msg = msg
     super().__init__(f"Error: {self.msg}")
 
 class DataWiseInternalError(DataWiseError):
   """
   Raised when an internal error occurs
   """
+  def __init__(self, error_msg=""):
+    super().__init__(error_msg)
 
 class BadRequestError(DataWiseError):
   """
   Raised when a bad request happens
   """
   def __init__(self, error_msg=""):
     super().__init__(error_msg)
```

### Comparing `datawise-0.0.20/pyproject.toml` & `datawise-0.0.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datawise"
-version = "0.0.20"
+version = "0.0.21"
 description = "AI Assistant for Python Data Analytics"
 authors = ["DataWise Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
```

### Comparing `datawise-0.0.20/PKG-INFO` & `datawise-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawise
-Version: 0.0.20
+Version: 0.0.21
 Summary: AI Assistant for Python Data Analytics
 Author: DataWise Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

