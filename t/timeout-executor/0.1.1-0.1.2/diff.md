# Comparing `tmp/timeout_executor-0.1.1.tar.gz` & `tmp/timeout_executor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeout_executor-0.1.1.tar", max compression
+gzip compressed data, was "timeout_executor-0.1.2.tar", max compression
```

## Comparing `timeout_executor-0.1.1.tar` & `timeout_executor-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1075 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/LICENSE
--rw-r--r--   0        0        0      765 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/README.md
--rw-r--r--   0        0        0     3484 2023-06-24 21:57:11.287044 timeout_executor-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-24 21:57:11.327046 timeout_executor-0.1.1/src/timeout_executor/__init__.py
--rw-r--r--   0        0        0       81 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/__init__.py
--rw-r--r--   0        0        0      112 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_billiard/__init__.py
--rw-r--r--   0        0        0    24971 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_billiard/process.py
--rw-r--r--   0        0        0      112 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_multiprocessing/__init__.py
--rw-r--r--   0        0        0    24320 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_multiprocessing/process.py
--rw-r--r--   0        0        0     8485 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/executor.py
--rw-r--r--   0        0        0      151 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/log.py
--rw-r--r--   0        0        0      129 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/__init__.py
--rw-r--r--   0        0        0      130 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_billiard/__init__.py
--rw-r--r--   0        0        0     2940 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_billiard/patch.py
--rw-r--r--   0        0        0     1373 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_cloudpickle.py
--rw-r--r--   0        0        0     1336 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_dill.py
--rw-r--r--   0        0        0      130 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_multiprocessing/__init__.py
--rw-r--r--   0        0        0     2833 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/_multiprocessing/patch.py
--rw-r--r--   0        0        0      993 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/base.py
--rw-r--r--   0        0        0      112 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/lock.py
--rw-r--r--   0        0        0      978 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/pickler/main.py
--rw-r--r--   0        0        0        0 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/py.typed
--rw-r--r--   0        0        0      754 2023-06-24 21:56:57.710736 timeout_executor-0.1.1/src/timeout_executor/readonly.py
--rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 timeout_executor-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-24 22:09:38.963995 timeout_executor-0.1.2/LICENSE
+-rw-r--r--   0        0        0      765 2023-06-24 22:09:38.963995 timeout_executor-0.1.2/README.md
+-rw-r--r--   0        0        0     3503 2023-06-24 22:10:01.772582 timeout_executor-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-06-24 22:10:01.828583 timeout_executor-0.1.2/src/timeout_executor/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-24 22:09:38.963995 timeout_executor-0.1.2/src/timeout_executor/concurrent/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 22:09:38.963995 timeout_executor-0.1.2/src/timeout_executor/concurrent/futures/__init__.py
+-rw-r--r--   0        0        0      112 2023-06-24 22:09:38.963995 timeout_executor-0.1.2/src/timeout_executor/concurrent/futures/_billiard/__init__.py
+-rw-r--r--   0        0        0    24971 2023-06-24 22:09:38.963995 timeout_executor-0.1.2/src/timeout_executor/concurrent/futures/_billiard/process.py
+-rw-r--r--   0        0        0      112 2023-06-24 22:09:38.963995 timeout_executor-0.1.2/src/timeout_executor/concurrent/futures/_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    24320 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/concurrent/futures/_multiprocessing/process.py
+-rw-r--r--   0        0        0     8485 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/executor.py
+-rw-r--r--   0        0        0      151 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/log.py
+-rw-r--r--   0        0        0      129 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/pickler/__init__.py
+-rw-r--r--   0        0        0      130 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/pickler/_billiard/__init__.py
+-rw-r--r--   0        0        0     2940 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/pickler/_billiard/patch.py
+-rw-r--r--   0        0        0     1373 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/pickler/_cloudpickle.py
+-rw-r--r--   0        0        0     1336 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/pickler/_dill.py
+-rw-r--r--   0        0        0      130 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/pickler/_multiprocessing/__init__.py
+-rw-r--r--   0        0        0     2833 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/pickler/_multiprocessing/patch.py
+-rw-r--r--   0        0        0      993 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/pickler/base.py
+-rw-r--r--   0        0        0      112 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/pickler/lock.py
+-rw-r--r--   0        0        0      978 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/pickler/main.py
+-rw-r--r--   0        0        0        0 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/py.typed
+-rw-r--r--   0        0        0      754 2023-06-24 22:09:38.967995 timeout_executor-0.1.2/src/timeout_executor/readonly.py
+-rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 timeout_executor-0.1.2/PKG-INFO
```

### Comparing `timeout_executor-0.1.1/LICENSE` & `timeout_executor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/README.md` & `timeout_executor-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/pyproject.toml` & `timeout_executor-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timeout-executor"
-version = "0.1.1"
+version = "0.1.2" # will be replaced
 description = "execute with timeout"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 packages = [{ include = "timeout_executor", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_billiard/process.py` & `timeout_executor-0.1.2/src/timeout_executor/concurrent/futures/_billiard/process.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/src/timeout_executor/concurrent/futures/_multiprocessing/process.py` & `timeout_executor-0.1.2/src/timeout_executor/concurrent/futures/_multiprocessing/process.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/src/timeout_executor/executor.py` & `timeout_executor-0.1.2/src/timeout_executor/executor.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/src/timeout_executor/pickler/_billiard/patch.py` & `timeout_executor-0.1.2/src/timeout_executor/pickler/_billiard/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/src/timeout_executor/pickler/_cloudpickle.py` & `timeout_executor-0.1.2/src/timeout_executor/pickler/_cloudpickle.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/src/timeout_executor/pickler/_dill.py` & `timeout_executor-0.1.2/src/timeout_executor/pickler/_dill.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/src/timeout_executor/pickler/_multiprocessing/patch.py` & `timeout_executor-0.1.2/src/timeout_executor/pickler/_multiprocessing/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/src/timeout_executor/pickler/base.py` & `timeout_executor-0.1.2/src/timeout_executor/pickler/base.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/src/timeout_executor/pickler/main.py` & `timeout_executor-0.1.2/src/timeout_executor/pickler/main.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/src/timeout_executor/readonly.py` & `timeout_executor-0.1.2/src/timeout_executor/readonly.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.1/PKG-INFO` & `timeout_executor-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeout-executor
-Version: 0.1.1
+Version: 0.1.2
 Summary: execute with timeout
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

