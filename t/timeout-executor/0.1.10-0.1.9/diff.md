# Comparing `tmp/timeout_executor-0.1.10.tar.gz` & `tmp/timeout_executor-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeout_executor-0.1.10.tar", max compression
+gzip compressed data, was "timeout_executor-0.1.9.tar", max compression
```

## Comparing `timeout_executor-0.1.10.tar` & `timeout_executor-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1075 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/LICENSE
--rw-r--r--   0        0        0     1197 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/README.md
--rw-r--r--   0        0        0     3670 2023-06-25 02:04:42.478151 timeout_executor-0.1.10/pyproject.toml
--rw-r--r--   0        0        0      183 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/__init__.py
--rw-r--r--   0        0        0       64 2023-06-25 02:04:42.518152 timeout_executor-0.1.10/src/timeout_executor/_version.py
--rw-r--r--   0        0        0      144 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/concurrent/__init__.py
--rw-r--r--   0        0        0        0 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/concurrent/futures/__init__.py
--rw-r--r--   0        0        0      112 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/concurrent/futures/_billiard/__init__.py
--rw-r--r--   0        0        0    24971 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/concurrent/futures/_billiard/process.py
--rw-r--r--   0        0        0      112 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/concurrent/futures/_multiprocessing/__init__.py
--rw-r--r--   0        0        0    24320 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/concurrent/futures/_multiprocessing/process.py
--rw-r--r--   0        0        0     1344 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/concurrent/main.py
--rw-r--r--   0        0        0     7493 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/executor.py
--rw-r--r--   0        0        0      151 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/log.py
--rw-r--r--   0        0        0      129 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/pickler/__init__.py
--rw-r--r--   0        0        0      130 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/pickler/_billiard/__init__.py
--rw-r--r--   0        0        0     2940 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/pickler/_billiard/patch.py
--rw-r--r--   0        0        0     1373 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/pickler/_cloudpickle.py
--rw-r--r--   0        0        0     1336 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/pickler/_dill.py
--rw-r--r--   0        0        0      130 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/pickler/_multiprocessing/__init__.py
--rw-r--r--   0        0        0     2833 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/pickler/_multiprocessing/patch.py
--rw-r--r--   0        0        0      993 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/pickler/base.py
--rw-r--r--   0        0        0      112 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/pickler/lock.py
--rw-r--r--   0        0        0     1128 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/pickler/main.py
--rw-r--r--   0        0        0        0 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/py.typed
--rw-r--r--   0        0        0      754 2023-06-25 02:04:28.361922 timeout_executor-0.1.10/src/timeout_executor/readonly.py
--rw-r--r--   0        0        0     2255 1970-01-01 00:00:00.000000 timeout_executor-0.1.10/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-24 23:17:10.429253 timeout_executor-0.1.9/LICENSE
+-rw-r--r--   0        0        0      765 2023-06-24 23:17:10.429253 timeout_executor-0.1.9/README.md
+-rw-r--r--   0        0        0     3668 2023-06-24 23:17:23.413655 timeout_executor-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-06-24 23:17:10.429253 timeout_executor-0.1.9/src/timeout_executor/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-24 23:17:23.453656 timeout_executor-0.1.9/src/timeout_executor/_version.py
+-rw-r--r--   0        0        0       81 2023-06-24 23:17:10.429253 timeout_executor-0.1.9/src/timeout_executor/concurrent/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 23:17:10.429253 timeout_executor-0.1.9/src/timeout_executor/concurrent/futures/__init__.py
+-rw-r--r--   0        0        0      112 2023-06-24 23:17:10.429253 timeout_executor-0.1.9/src/timeout_executor/concurrent/futures/_billiard/__init__.py
+-rw-r--r--   0        0        0    24971 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/concurrent/futures/_billiard/process.py
+-rw-r--r--   0        0        0      112 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/concurrent/futures/_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    24320 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/concurrent/futures/_multiprocessing/process.py
+-rw-r--r--   0        0        0     8485 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/executor.py
+-rw-r--r--   0        0        0      151 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/log.py
+-rw-r--r--   0        0        0      129 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/pickler/__init__.py
+-rw-r--r--   0        0        0      130 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/pickler/_billiard/__init__.py
+-rw-r--r--   0        0        0     2940 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/pickler/_billiard/patch.py
+-rw-r--r--   0        0        0     1373 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/pickler/_cloudpickle.py
+-rw-r--r--   0        0        0     1336 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/pickler/_dill.py
+-rw-r--r--   0        0        0      130 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/pickler/_multiprocessing/__init__.py
+-rw-r--r--   0        0        0     2833 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/pickler/_multiprocessing/patch.py
+-rw-r--r--   0        0        0      993 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/pickler/base.py
+-rw-r--r--   0        0        0      112 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/pickler/lock.py
+-rw-r--r--   0        0        0      978 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/pickler/main.py
+-rw-r--r--   0        0        0        0 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/py.typed
+-rw-r--r--   0        0        0      754 2023-06-24 23:17:10.433254 timeout_executor-0.1.9/src/timeout_executor/readonly.py
+-rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 timeout_executor-0.1.9/PKG-INFO
```

### Comparing `timeout_executor-0.1.10/LICENSE` & `timeout_executor-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.10/pyproject.toml` & `timeout_executor-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [tool.poetry]
 name = "timeout-executor"
-version = "0.1.10"                                             # will be replaced
+version = "0.1.9" # will be replaced
 description = "execute with timeout"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/timeout-executor"
 repository = "https://github.com/phi-friday/timeout-executor"
-packages = [{ include = "timeout_executor", from = "src" }]
+packages = [
+    { include = "timeout_executor", from = "src" },
+    { include = "pyproject.toml" },
+]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 anyio = ">=3.7.0"
 typing-extensions = ">=4.6.3"
 billiard = { version = ">=4.0.0", optional = true }
 dill = { version = ">=0.3.6", optional = true }
```

### Comparing `timeout_executor-0.1.10/src/timeout_executor/concurrent/futures/_billiard/process.py` & `timeout_executor-0.1.9/src/timeout_executor/concurrent/futures/_billiard/process.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.10/src/timeout_executor/concurrent/futures/_multiprocessing/process.py` & `timeout_executor-0.1.9/src/timeout_executor/concurrent/futures/_multiprocessing/process.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.10/src/timeout_executor/executor.py` & `timeout_executor-0.1.9/src/timeout_executor/executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import importlib
+import sys
 from concurrent.futures import wait
 from functools import lru_cache, partial
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Coroutine,
@@ -13,35 +14,38 @@
     TypeVar,
     overload,
 )
 
 import anyio
 from typing_extensions import ParamSpec
 
-from timeout_executor.concurrent import get_context_executor
 from timeout_executor.log import logger
 from timeout_executor.pickler import monkey_patch, monkey_unpatch
-from timeout_executor.pickler.lock import patch_lock
 
 if TYPE_CHECKING:
     from threading import RLock
 
     from anyio.abc import ObjectSendStream
 
-    from timeout_executor.concurrent.futures import _billiard as billiard_future
-    from timeout_executor.concurrent.futures import (
-        _multiprocessing as multiprocessing_future,
-    )
-    from timeout_executor.concurrent.main import ContextType
-    from timeout_executor.pickler.main import PicklerType
+    from .concurrent.futures import _billiard as billiard_future
+    from .concurrent.futures import _multiprocessing as multiprocessing_future
 
 __all__ = ["TimeoutExecutor", "get_executor"]
 
 ParamT = ParamSpec("ParamT")
 ResultT = TypeVar("ResultT")
+IPYTHON_SHELL_NAMES = frozenset(
+    {
+        "ZMQInteractiveShell",
+        "TerminalInteractiveShell",
+    },
+)
+
+ContextType = Literal["billiard", "multiprocessing"]
+PicklerType = Literal["pickle", "dill", "cloudpickle"]
 
 
 class TimeoutExecutor:
     """exec with timeout"""
 
     def __init__(
         self,
@@ -54,14 +58,15 @@
         self._args = ()
         self._kwargs = {}
         self._select = (context, pickler)
 
     @property
     def lock(self) -> RLock:
         """patch lock"""
+        from timeout_executor.pickler.lock import patch_lock
 
         return patch_lock
 
     def _partial_init(self) -> Callable[[], Any] | None:
         if self._init is None:
             return None
         return partial(self._init, *self._args, **self._kwargs)
@@ -187,26 +192,34 @@
     Args:
         context: billiard or multiprocessing. Defaults to None.
 
     Returns:
         ProcessPoolExecutor
     """
     context, pickler = _validate_context_and_pickler(context, pickler)
-    executor = get_context_executor(context)
+    future_module = importlib.import_module(
+        f".concurrent.futures._{context}",
+        __package__,
+    )
+    executor = future_module.ProcessPoolExecutor
     _patch_or_unpatch(context, pickler)
 
     return executor
 
 
 def _validate_context_and_pickler(
     context: Any,
     pickler: Any,
 ) -> tuple[ContextType, PicklerType]:
     if not context:
-        context = "multiprocessing"
+        context = (
+            "billiard"
+            if _is_jupyter() and _check_deps("billiard")
+            else "multiprocessing"
+        )
     if not pickler:
         if _check_deps("dill"):
             pickler = "dill"
         elif _check_deps("cloudpickle"):
             pickler = "cloudpickle"
         else:
             pickler = "pickle"
@@ -274,14 +287,38 @@
     **kwargs: Any,
 ) -> None:
     async with _stream:
         result = await func(*args, **kwargs)
         await _stream.send(result)
 
 
+def _is_jupyter() -> bool:
+    frame = sys._getframe()  # noqa: SLF001
+    while frame.f_back:
+        if "get_ipython" in frame.f_globals:
+            ipython_func = frame.f_globals.get("get_ipython", None)
+            if callable(ipython_func):
+                return _is_jupyter_from_shell(ipython_func())
+        frame = frame.f_back
+    if "get_ipython" in frame.f_globals:
+        ipython_func = frame.f_globals.get("get_ipython", None)
+        if callable(ipython_func):
+            return _is_jupyter_from_shell(ipython_func())
+    return False
+
+
+def _is_jupyter_from_shell(shell: Any) -> bool:
+    try:
+        shell_name: str = type(shell).__name__
+    except NameError:
+        return False
+
+    return shell_name in IPYTHON_SHELL_NAMES
+
+
 @lru_cache
 def _check_deps(module_name: str) -> bool:
     try:
         importlib.import_module(module_name)
     except (ImportError, ModuleNotFoundError):
         return False
     else:
```

### Comparing `timeout_executor-0.1.10/src/timeout_executor/pickler/_billiard/patch.py` & `timeout_executor-0.1.9/src/timeout_executor/pickler/_billiard/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.10/src/timeout_executor/pickler/_cloudpickle.py` & `timeout_executor-0.1.9/src/timeout_executor/pickler/_cloudpickle.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.10/src/timeout_executor/pickler/_dill.py` & `timeout_executor-0.1.9/src/timeout_executor/pickler/_dill.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.10/src/timeout_executor/pickler/_multiprocessing/patch.py` & `timeout_executor-0.1.9/src/timeout_executor/pickler/_multiprocessing/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.10/src/timeout_executor/pickler/base.py` & `timeout_executor-0.1.9/src/timeout_executor/pickler/base.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.10/src/timeout_executor/readonly.py` & `timeout_executor-0.1.9/src/timeout_executor/readonly.py`

 * *Files identical despite different names*

