# Comparing `tmp/timeout_executor-0.1.4.tar.gz` & `tmp/timeout_executor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeout_executor-0.1.4.tar", max compression
+gzip compressed data, was "timeout_executor-0.1.5.tar", max compression
```

## Comparing `timeout_executor-0.1.4.tar` & `timeout_executor-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1075 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/LICENSE
--rw-r--r--   0        0        0      765 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/README.md
--rw-r--r--   0        0        0     3625 2023-06-24 22:27:42.860052 timeout_executor-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-24 22:27:42.900053 timeout_executor-0.1.4/src/timeout_executor/__init__.py
--rw-r--r--   0        0        0       81 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/__init__.py
--rw-r--r--   0        0        0      112 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_billiard/__init__.py
--rw-r--r--   0        0        0    24971 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_billiard/process.py
--rw-r--r--   0        0        0      112 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_multiprocessing/__init__.py
--rw-r--r--   0        0        0    24320 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_multiprocessing/process.py
--rw-r--r--   0        0        0     8485 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/executor.py
--rw-r--r--   0        0        0      151 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/log.py
--rw-r--r--   0        0        0      129 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/__init__.py
--rw-r--r--   0        0        0      130 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_billiard/__init__.py
--rw-r--r--   0        0        0     2940 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_billiard/patch.py
--rw-r--r--   0        0        0     1373 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_cloudpickle.py
--rw-r--r--   0        0        0     1336 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_dill.py
--rw-r--r--   0        0        0      130 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_multiprocessing/__init__.py
--rw-r--r--   0        0        0     2833 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/_multiprocessing/patch.py
--rw-r--r--   0        0        0      993 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/base.py
--rw-r--r--   0        0        0      112 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/lock.py
--rw-r--r--   0        0        0      978 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/pickler/main.py
--rw-r--r--   0        0        0        0 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/py.typed
--rw-r--r--   0        0        0      754 2023-06-24 22:27:27.923652 timeout_executor-0.1.4/src/timeout_executor/readonly.py
--rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 timeout_executor-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-24 22:47:53.309379 timeout_executor-0.1.5/LICENSE
+-rw-r--r--   0        0        0      765 2023-06-24 22:47:53.309379 timeout_executor-0.1.5/README.md
+-rw-r--r--   0        0        0     3718 2023-06-24 22:48:06.925436 timeout_executor-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-24 22:48:06.965436 timeout_executor-0.1.5/src/timeout_executor/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-24 22:47:53.309379 timeout_executor-0.1.5/src/timeout_executor/concurrent/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 22:47:53.309379 timeout_executor-0.1.5/src/timeout_executor/concurrent/futures/__init__.py
+-rw-r--r--   0        0        0      112 2023-06-24 22:47:53.309379 timeout_executor-0.1.5/src/timeout_executor/concurrent/futures/_billiard/__init__.py
+-rw-r--r--   0        0        0    24971 2023-06-24 22:47:53.309379 timeout_executor-0.1.5/src/timeout_executor/concurrent/futures/_billiard/process.py
+-rw-r--r--   0        0        0      112 2023-06-24 22:47:53.309379 timeout_executor-0.1.5/src/timeout_executor/concurrent/futures/_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    24320 2023-06-24 22:47:53.309379 timeout_executor-0.1.5/src/timeout_executor/concurrent/futures/_multiprocessing/process.py
+-rw-r--r--   0        0        0     8485 2023-06-24 22:47:53.309379 timeout_executor-0.1.5/src/timeout_executor/executor.py
+-rw-r--r--   0        0        0      151 2023-06-24 22:47:53.309379 timeout_executor-0.1.5/src/timeout_executor/log.py
+-rw-r--r--   0        0        0      129 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/pickler/__init__.py
+-rw-r--r--   0        0        0      130 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/pickler/_billiard/__init__.py
+-rw-r--r--   0        0        0     2940 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/pickler/_billiard/patch.py
+-rw-r--r--   0        0        0     1373 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/pickler/_cloudpickle.py
+-rw-r--r--   0        0        0     1336 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/pickler/_dill.py
+-rw-r--r--   0        0        0      130 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/pickler/_multiprocessing/__init__.py
+-rw-r--r--   0        0        0     2833 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/pickler/_multiprocessing/patch.py
+-rw-r--r--   0        0        0      993 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/pickler/base.py
+-rw-r--r--   0        0        0      112 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/pickler/lock.py
+-rw-r--r--   0        0        0      978 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/pickler/main.py
+-rw-r--r--   0        0        0        0 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/py.typed
+-rw-r--r--   0        0        0      754 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/readonly.py
+-rw-r--r--   0        0        0      411 2023-06-24 22:47:53.313380 timeout_executor-0.1.5/src/timeout_executor/version.py
+-rw-r--r--   0        0        0     1886 1970-01-01 00:00:00.000000 timeout_executor-0.1.5/PKG-INFO
```

### Comparing `timeout_executor-0.1.4/LICENSE` & `timeout_executor-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/README.md` & `timeout_executor-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/pyproject.toml` & `timeout_executor-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "timeout-executor"
-version = "0.1.4" # will be replaced
+version = "0.1.5"                                             # will be replaced
 description = "execute with timeout"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/timeout-executor"
 repository = "https://github.com/phi-friday/timeout-executor"
 packages = [{ include = "timeout_executor", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 anyio = ">=3.7.0"
 typing-extensions = ">=4.6.3"
+tomli = { version = "^2.0.1", python = "<3.11" }
 billiard = { version = ">=4.0.0", optional = true }
 dill = { version = ">=0.3.6", optional = true }
 cloudpickle = { version = ">=2.2.1", optional = true }
 
 [tool.poetry.extras]
 all = ['billiard', 'dill', 'cloudpickle']
 billiard = ['billiard', 'dill']
```

### Comparing `timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_billiard/process.py` & `timeout_executor-0.1.5/src/timeout_executor/concurrent/futures/_billiard/process.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/src/timeout_executor/concurrent/futures/_multiprocessing/process.py` & `timeout_executor-0.1.5/src/timeout_executor/concurrent/futures/_multiprocessing/process.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/src/timeout_executor/executor.py` & `timeout_executor-0.1.5/src/timeout_executor/executor.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/src/timeout_executor/pickler/_billiard/patch.py` & `timeout_executor-0.1.5/src/timeout_executor/pickler/_billiard/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/src/timeout_executor/pickler/_cloudpickle.py` & `timeout_executor-0.1.5/src/timeout_executor/pickler/_cloudpickle.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/src/timeout_executor/pickler/_dill.py` & `timeout_executor-0.1.5/src/timeout_executor/pickler/_dill.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/src/timeout_executor/pickler/_multiprocessing/patch.py` & `timeout_executor-0.1.5/src/timeout_executor/pickler/_multiprocessing/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/src/timeout_executor/pickler/base.py` & `timeout_executor-0.1.5/src/timeout_executor/pickler/base.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/src/timeout_executor/pickler/main.py` & `timeout_executor-0.1.5/src/timeout_executor/pickler/main.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/src/timeout_executor/readonly.py` & `timeout_executor-0.1.5/src/timeout_executor/readonly.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.4/PKG-INFO` & `timeout_executor-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeout-executor
-Version: 0.1.4
+Version: 0.1.5
 Summary: execute with timeout
 Home-page: https://github.com/phi-friday/timeout-executor
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Provides-Extra: billiard
 Provides-Extra: cloudpickle
 Provides-Extra: dill
 Requires-Dist: anyio (>=3.7.0)
 Requires-Dist: billiard (>=4.0.0) ; extra == "all" or extra == "billiard"
 Requires-Dist: cloudpickle (>=2.2.1) ; extra == "all" or extra == "cloudpickle"
 Requires-Dist: dill (>=0.3.6) ; extra == "all" or extra == "billiard" or extra == "dill"
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: typing-extensions (>=4.6.3)
 Project-URL: Repository, https://github.com/phi-friday/timeout-executor
 Description-Content-Type: text/markdown
 
 # timeout-executor
 
 ## how to install
```

