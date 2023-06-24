# Comparing `tmp/timeout_executor-0.1.0.tar.gz` & `tmp/timeout_executor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeout_executor-0.1.0.tar", max compression
+gzip compressed data, was "timeout_executor-0.1.1.tar", max compression
```

## Comparing `timeout_executor-0.1.0.tar` & `timeout_executor-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1075 2023-06-24 18:57:49.731226 timeout_executor-0.1.0/LICENSE
--rw-r--r--   0        0        0      765 2023-06-24 19:15:52.875687 timeout_executor-0.1.0/README.md
--rw-r--r--   0        0        0     3490 2023-06-24 19:09:31.055727 timeout_executor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      135 2023-06-24 18:44:40.610196 timeout_executor-0.1.0/src/timeout_executor/__init__.py
--rw-r--r--   0        0        0       81 2023-06-24 13:13:22.836431 timeout_executor-0.1.0/src/timeout_executor/concurrent/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 13:23:12.941786 timeout_executor-0.1.0/src/timeout_executor/concurrent/futures/__init__.py
--rw-r--r--   0        0        0      112 2023-06-24 13:20:26.594599 timeout_executor-0.1.0/src/timeout_executor/concurrent/futures/_billiard/__init__.py
--rw-r--r--   0        0        0    24971 2023-06-24 18:21:58.955242 timeout_executor-0.1.0/src/timeout_executor/concurrent/futures/_billiard/process.py
--rw-r--r--   0        0        0      112 2023-06-24 14:30:00.257966 timeout_executor-0.1.0/src/timeout_executor/concurrent/futures/_multiprocessing/__init__.py
--rw-r--r--   0        0        0    24320 2023-06-24 18:22:28.152841 timeout_executor-0.1.0/src/timeout_executor/concurrent/futures/_multiprocessing/process.py
--rw-r--r--   0        0        0     8485 2023-06-24 18:44:38.337910 timeout_executor-0.1.0/src/timeout_executor/executor.py
--rw-r--r--   0        0        0      151 2023-06-24 18:44:35.358139 timeout_executor-0.1.0/src/timeout_executor/log.py
--rw-r--r--   0        0        0      129 2023-06-24 17:40:26.200720 timeout_executor-0.1.0/src/timeout_executor/pickler/__init__.py
--rw-r--r--   0        0        0      130 2023-06-24 17:25:18.137632 timeout_executor-0.1.0/src/timeout_executor/pickler/_billiard/__init__.py
--rw-r--r--   0        0        0     2940 2023-06-24 18:41:41.877459 timeout_executor-0.1.0/src/timeout_executor/pickler/_billiard/patch.py
--rw-r--r--   0        0        0     1373 2023-06-24 18:44:47.358727 timeout_executor-0.1.0/src/timeout_executor/pickler/_cloudpickle.py
--rw-r--r--   0        0        0     1336 2023-06-24 18:44:46.290169 timeout_executor-0.1.0/src/timeout_executor/pickler/_dill.py
--rw-r--r--   0        0        0      130 2023-06-24 17:25:21.946999 timeout_executor-0.1.0/src/timeout_executor/pickler/_multiprocessing/__init__.py
--rw-r--r--   0        0        0     2833 2023-06-24 18:42:16.509400 timeout_executor-0.1.0/src/timeout_executor/pickler/_multiprocessing/patch.py
--rw-r--r--   0        0        0      993 2023-06-24 18:44:44.803851 timeout_executor-0.1.0/src/timeout_executor/pickler/base.py
--rw-r--r--   0        0        0      112 2023-06-24 18:44:43.625524 timeout_executor-0.1.0/src/timeout_executor/pickler/lock.py
--rw-r--r--   0        0        0      978 2023-06-24 18:44:42.021868 timeout_executor-0.1.0/src/timeout_executor/pickler/main.py
--rw-r--r--   0        0        0        0 2023-06-24 18:47:54.967104 timeout_executor-0.1.0/src/timeout_executor/py.typed
--rw-r--r--   0        0        0      754 2023-06-24 18:44:33.410284 timeout_executor-0.1.0/src/timeout_executor/readonly.py
--rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 timeout_executor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/LICENSE
+-rw-r--r--   0        0        0      765 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/README.md
+-rw-r--r--   0        0        0     3484 2023-06-24 21:57:11.287044 timeout_executor-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-24 21:57:11.327046 timeout_executor-0.1.1/src/timeout_executor/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/__init__.py
+-rw-r--r--   0        0        0      112 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_billiard/__init__.py
+-rw-r--r--   0        0        0    24971 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_billiard/process.py
+-rw-r--r--   0        0        0      112 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    24320 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_multiprocessing/process.py
+-rw-r--r--   0        0        0     8485 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/executor.py
+-rw-r--r--   0        0        0      151 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/log.py
+-rw-r--r--   0        0        0      129 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/__init__.py
+-rw-r--r--   0        0        0      130 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_billiard/__init__.py
+-rw-r--r--   0        0        0     2940 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_billiard/patch.py
+-rw-r--r--   0        0        0     1373 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_cloudpickle.py
+-rw-r--r--   0        0        0     1336 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_dill.py
+-rw-r--r--   0        0        0      130 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_multiprocessing/__init__.py
+-rw-r--r--   0        0        0     2833 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_multiprocessing/patch.py
+-rw-r--r--   0        0        0      993 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/base.py
+-rw-r--r--   0        0        0      112 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/lock.py
+-rw-r--r--   0        0        0      978 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/main.py
+-rw-r--r--   0        0        0        0 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/py.typed
+-rw-r--r--   0        0        0      754 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/readonly.py
+-rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 timeout_executor-0.1.1/PKG-INFO
```

### Comparing `timeout_executor-0.1.0/LICENSE` & `timeout_executor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/README.md` & `timeout_executor-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/pyproject.toml` & `timeout_executor-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "timeout-executor"
-version = "0.1.0"
+version = "0.1.1"
 description = "execute with timeout"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 packages = [{ include = "timeout_executor", from = "src" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8"
 anyio = ">=3.7.0"
 typing-extensions = ">=4.6.3"
 billiard = { version = ">=4.0.0", optional = true }
 dill = { version = ">=0.3.6", optional = true }
 cloudpickle = { version = ">=2.2.1", optional = true }
 
 [tool.poetry.extras]
```

### Comparing `timeout_executor-0.1.0/src/timeout_executor/concurrent/futures/_billiard/process.py` & `timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_billiard/process.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/src/timeout_executor/concurrent/futures/_multiprocessing/process.py` & `timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_multiprocessing/process.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/src/timeout_executor/executor.py` & `timeout_executor-0.1.1/src/timeout_executor/executor.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/src/timeout_executor/pickler/_billiard/patch.py` & `timeout_executor-0.1.1/src/timeout_executor/pickler/_billiard/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/src/timeout_executor/pickler/_cloudpickle.py` & `timeout_executor-0.1.1/src/timeout_executor/pickler/_cloudpickle.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/src/timeout_executor/pickler/_dill.py` & `timeout_executor-0.1.1/src/timeout_executor/pickler/_dill.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/src/timeout_executor/pickler/_multiprocessing/patch.py` & `timeout_executor-0.1.1/src/timeout_executor/pickler/_multiprocessing/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/src/timeout_executor/pickler/base.py` & `timeout_executor-0.1.1/src/timeout_executor/pickler/base.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/src/timeout_executor/pickler/main.py` & `timeout_executor-0.1.1/src/timeout_executor/pickler/main.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/src/timeout_executor/readonly.py` & `timeout_executor-0.1.1/src/timeout_executor/readonly.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.0/PKG-INFO` & `timeout_executor-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: timeout-executor
-Version: 0.1.0
+Version: 0.1.1
 Summary: execute with timeout
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
```

