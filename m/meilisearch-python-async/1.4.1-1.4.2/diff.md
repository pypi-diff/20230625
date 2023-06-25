# Comparing `tmp/meilisearch_python_async-1.4.1.tar.gz` & `tmp/meilisearch_python_async-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_async-1.4.1.tar", max compression
+gzip compressed data, was "meilisearch_python_async-1.4.2.tar", max compression
```

## Comparing `meilisearch_python_async-1.4.1.tar` & `meilisearch_python_async-1.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-06-20 15:19:01.840695 meilisearch_python_async-1.4.1/LICENSE
--rw-r--r--   0        0        0     5759 2023-06-20 15:19:01.840695 meilisearch_python_async-1.4.1/README.md
--rw-r--r--   0        0        0      151 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/__init__.py
--rw-r--r--   0        0        0     2759 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/_http_requests.py
--rw-r--r--   0        0        0       18 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/_version.py
--rw-r--r--   0        0        0    22205 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/client.py
--rw-r--r--   0        0        0     2085 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/errors.py
--rw-r--r--   0        0        0    89041 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/index.py
--rw-r--r--   0        0        0        0 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/__init__.py
--rw-r--r--   0        0        0     1576 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/client.py
--rw-r--r--   0        0        0      202 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/documents.py
--rw-r--r--   0        0        0       95 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/health.py
--rw-r--r--   0        0        0      392 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/index.py
--rw-r--r--   0        0        0     1285 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/search.py
--rw-r--r--   0        0        0     1119 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/settings.py
--rw-r--r--   0        0        0      769 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/task.py
--rw-r--r--   0        0        0      215 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/version.py
--rw-r--r--   0        0        0        0 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/py.typed
--rw-r--r--   0        0        0    11932 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/task.py
--rw-r--r--   0        0        0     2286 2023-06-20 15:19:01.848693 meilisearch_python_async-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     6968 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/LICENSE
+-rw-r--r--   0        0        0     5759 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/README.md
+-rw-r--r--   0        0        0      151 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/__init__.py
+-rw-r--r--   0        0        0     2759 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/_http_requests.py
+-rw-r--r--   0        0        0       18 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/_version.py
+-rw-r--r--   0        0        0    22205 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/client.py
+-rw-r--r--   0        0        0     2085 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/errors.py
+-rw-r--r--   0        0        0    89041 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/index.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/__init__.py
+-rw-r--r--   0        0        0     1576 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/client.py
+-rw-r--r--   0        0        0      202 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/documents.py
+-rw-r--r--   0        0        0       95 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/health.py
+-rw-r--r--   0        0        0      392 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/index.py
+-rw-r--r--   0        0        0     1285 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/search.py
+-rw-r--r--   0        0        0     1119 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/settings.py
+-rw-r--r--   0        0        0      769 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/task.py
+-rw-r--r--   0        0        0      215 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/version.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/py.typed
+-rw-r--r--   0        0        0    11932 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/task.py
+-rw-r--r--   0        0        0     2243 2023-06-25 13:09:51.138898 meilisearch_python_async-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.2/PKG-INFO
```

### Comparing `meilisearch_python_async-1.4.1/LICENSE` & `meilisearch_python_async-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.1/README.md` & `meilisearch_python_async-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.1/meilisearch_python_async/_http_requests.py` & `meilisearch_python_async-1.4.2/meilisearch_python_async/_http_requests.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.1/meilisearch_python_async/client.py` & `meilisearch_python_async-1.4.2/meilisearch_python_async/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.1/meilisearch_python_async/errors.py` & `meilisearch_python_async-1.4.2/meilisearch_python_async/errors.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.1/meilisearch_python_async/index.py` & `meilisearch_python_async-1.4.2/meilisearch_python_async/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.1/meilisearch_python_async/models/client.py` & `meilisearch_python_async-1.4.2/meilisearch_python_async/models/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.1/meilisearch_python_async/models/search.py` & `meilisearch_python_async-1.4.2/meilisearch_python_async/models/search.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.1/meilisearch_python_async/models/settings.py` & `meilisearch_python_async-1.4.2/meilisearch_python_async/models/settings.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.1/meilisearch_python_async/models/task.py` & `meilisearch_python_async-1.4.2/meilisearch_python_async/models/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.1/meilisearch_python_async/task.py` & `meilisearch_python_async-1.4.2/meilisearch_python_async/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.1/pyproject.toml` & `meilisearch_python_async-1.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [tool.poetry]
 name = "meilisearch-python-async"
-version = "1.4.1"
+version = "1.4.2"
 description = "A Python async client for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-async"
 homepage = "https://github.com/sanders41/meilisearch-python-async"
 documentation = "https://meilisearch-python-async.paulsanders.dev"
 keywords = ["meilisearch", "async", "python"]
 classifiers=[
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Typing :: Typed",
 ]
 include = ["meilisearch_python_async/py.typed"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 httpx = ">=0.17"
 pydantic = ">=1.8"
 aiofiles = ">=0.7"
 camel-converter = ">=1.0.0"
 PyJWT = ">=2.3.0"
 
 [tool.poetry.group.dev.dependencies]
@@ -88,9 +87,9 @@
 module = ["tests.*"]
 disallow_untyped_defs = false
 
 [tool.ruff]
 select=["E", "F", "UP", "I001", "T201", "T203"]
 ignore=["E501"]
 line-length = 100
-target-version = "py37"
+target-version = "py38"
 fix = true
```

### Comparing `meilisearch_python_async-1.4.1/PKG-INFO` & `meilisearch_python_async-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-async
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python async client for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-async
 License: MIT
 Keywords: meilisearch,async,python
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: PyJWT (>=2.3.0)
 Requires-Dist: aiofiles (>=0.7)
```

