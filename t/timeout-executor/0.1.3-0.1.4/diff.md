# Comparing `tmp/timeout_executor-0.1.3.tar.gz` & `tmp/timeout_executor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeout_executor-0.1.3.tar", max compression
+gzip compressed data, was "timeout_executor-0.1.4.tar", max compression
```

## Comparing `timeout_executor-0.1.3.tar` & `timeout_executor-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1075 2023-06-24 22:19:45.167285 timeout_executor-0.1.3/LICENSE
--rw-r--r--   0        0        0      765 2023-06-24 22:19:45.167285 timeout_executor-0.1.3/README.md
--rw-r--r--   0        0        0     3625 2023-06-24 22:19:59.511464 timeout_executor-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-24 22:19:59.543465 timeout_executor-0.1.3/src/timeout_executor/__init__.py
--rw-r--r--   0        0        0       81 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/concurrent/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/concurrent/futures/__init__.py
--rw-r--r--   0        0        0      112 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/concurrent/futures/_billiard/__init__.py
--rw-r--r--   0        0        0    24971 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/concurrent/futures/_billiard/process.py
--rw-r--r--   0        0        0      112 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/concurrent/futures/_multiprocessing/__init__.py
--rw-r--r--   0        0        0    24320 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/concurrent/futures/_multiprocessing/process.py
--rw-r--r--   0        0        0     8485 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/executor.py
--rw-r--r--   0        0        0      151 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/log.py
--rw-r--r--   0        0        0      129 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/pickler/__init__.py
--rw-r--r--   0        0        0      130 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/pickler/_billiard/__init__.py
--rw-r--r--   0        0        0     2940 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/pickler/_billiard/patch.py
--rw-r--r--   0        0        0     1373 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/pickler/_cloudpickle.py
--rw-r--r--   0        0        0     1336 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/pickler/_dill.py
--rw-r--r--   0        0        0      130 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/pickler/_multiprocessing/__init__.py
--rw-r--r--   0        0        0     2833 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/pickler/_multiprocessing/patch.py
--rw-r--r--   0        0        0      993 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/pickler/base.py
--rw-r--r--   0        0        0      112 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/pickler/lock.py
--rw-r--r--   0        0        0      978 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/pickler/main.py
--rw-r--r--   0        0        0        0 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/py.typed
--rw-r--r--   0        0        0      754 2023-06-24 22:19:45.171285 timeout_executor-0.1.3/src/timeout_executor/readonly.py
--rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 timeout_executor-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/LICENSE
+-rw-r--r--   0        0        0      765 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/README.md
+-rw-r--r--   0        0        0     3625 2023-06-24 22:27:42.860052 timeout_executor-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-24 22:27:42.900053 timeout_executor-0.1.4/src/timeout_executor/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/__init__.py
+-rw-r--r--   0        0        0      112 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_billiard/__init__.py
+-rw-r--r--   0        0        0    24971 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_billiard/process.py
+-rw-r--r--   0        0        0      112 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    24320 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_multiprocessing/process.py
+-rw-r--r--   0        0        0     8485 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/executor.py
+-rw-r--r--   0        0        0      151 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/log.py
+-rw-r--r--   0        0        0      129 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/__init__.py
+-rw-r--r--   0        0        0      130 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_billiard/__init__.py
+-rw-r--r--   0        0        0     2940 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_billiard/patch.py
+-rw-r--r--   0        0        0     1373 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_cloudpickle.py
+-rw-r--r--   0        0        0     1336 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_dill.py
+-rw-r--r--   0        0        0      130 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_multiprocessing/__init__.py
+-rw-r--r--   0        0        0     2833 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_multiprocessing/patch.py
+-rw-r--r--   0        0        0      993 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/base.py
+-rw-r--r--   0        0        0      112 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/lock.py
+-rw-r--r--   0        0        0      978 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/main.py
+-rw-r--r--   0        0        0        0 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/py.typed
+-rw-r--r--   0        0        0      754 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/readonly.py
+-rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 timeout_executor-0.1.4/PKG-INFO
```

### Comparing `timeout_executor-0.1.3/LICENSE` & `timeout_executor-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/README.md` & `timeout_executor-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/pyproject.toml` & `timeout_executor-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timeout-executor"
-version = "0.1.3" # will be replaced
+version = "0.1.4" # will be replaced
 description = "execute with timeout"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/timeout-executor"
 repository = "https://github.com/phi-friday/timeout-executor"
 packages = [{ include = "timeout_executor", from = "src" }]
```

### Comparing `timeout_executor-0.1.3/src/timeout_executor/concurrent/futures/_billiard/process.py` & `timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_billiard/process.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/src/timeout_executor/concurrent/futures/_multiprocessing/process.py` & `timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_multiprocessing/process.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/src/timeout_executor/executor.py` & `timeout_executor-0.1.4/src/timeout_executor/executor.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/src/timeout_executor/pickler/_billiard/patch.py` & `timeout_executor-0.1.4/src/timeout_executor/pickler/_billiard/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/src/timeout_executor/pickler/_cloudpickle.py` & `timeout_executor-0.1.4/src/timeout_executor/pickler/_cloudpickle.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/src/timeout_executor/pickler/_dill.py` & `timeout_executor-0.1.4/src/timeout_executor/pickler/_dill.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/src/timeout_executor/pickler/_multiprocessing/patch.py` & `timeout_executor-0.1.4/src/timeout_executor/pickler/_multiprocessing/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/src/timeout_executor/pickler/base.py` & `timeout_executor-0.1.4/src/timeout_executor/pickler/base.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/src/timeout_executor/pickler/main.py` & `timeout_executor-0.1.4/src/timeout_executor/pickler/main.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/src/timeout_executor/readonly.py` & `timeout_executor-0.1.4/src/timeout_executor/readonly.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.3/PKG-INFO` & `timeout_executor-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeout-executor
-Version: 0.1.3
+Version: 0.1.4
 Summary: execute with timeout
 Home-page: https://github.com/phi-friday/timeout-executor
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

