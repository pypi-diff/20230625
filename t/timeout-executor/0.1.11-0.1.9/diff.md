# Comparing `tmp/timeout_executor-0.1.11.tar.gz` & `tmp/timeout_executor-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeout_executor-0.1.11.tar", max compression
+gzip compressed data, was "timeout_executor-0.1.9.tar", max compression
```

## Comparing `timeout_executor-0.1.11.tar` & `timeout_executor-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,26 @@
--rw-r--r--   0        0        0     1075 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/LICENSE
--rw-r--r--   0        0        0     1197 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/README.md
--rw-r--r--   0        0        0     3749 2023-06-25 10:18:24.509222 timeout_executor-0.1.11/pyproject.toml
--rw-r--r--   0        0        0      183 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/__init__.py
--rw-r--r--   0        0        0       64 2023-06-25 10:18:24.561222 timeout_executor-0.1.11/src/timeout_executor/_version.py
--rw-r--r--   0        0        0      144 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/concurrent/__init__.py
--rw-r--r--   0        0        0        0 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/concurrent/futures/__init__.py
--rw-r--r--   0        0        0      112 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/concurrent/futures/_billiard/__init__.py
--rw-r--r--   0        0        0    24976 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/concurrent/futures/_billiard/process.py
--rw-r--r--   0        0        0      112 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/concurrent/futures/_joblib/__init__.py
--rw-r--r--   0        0        0     1998 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/concurrent/futures/_joblib/process.py
--rw-r--r--   0        0        0      112 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/concurrent/futures/_multiprocessing/__init__.py
--rw-r--r--   0        0        0    24325 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/concurrent/futures/_multiprocessing/process.py
--rw-r--r--   0        0        0     1648 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/concurrent/main.py
--rw-r--r--   0        0        0     8032 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/executor.py
--rw-r--r--   0        0        0      151 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/log.py
--rw-r--r--   0        0        0      129 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/__init__.py
--rw-r--r--   0        0        0      130 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/_billiard/__init__.py
--rw-r--r--   0        0        0     2940 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/_billiard/patch.py
--rw-r--r--   0        0        0     1373 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/_cloudpickle.py
--rw-r--r--   0        0        0     1336 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/_dill.py
--rw-r--r--   0        0        0      130 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/_joblib/__init__.py
--rw-r--r--   0        0        0      353 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/_joblib/patch.py
--rw-r--r--   0        0        0      130 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/_multiprocessing/__init__.py
--rw-r--r--   0        0        0     2833 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/_multiprocessing/patch.py
--rw-r--r--   0        0        0      993 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/base.py
--rw-r--r--   0        0        0      112 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/lock.py
--rw-r--r--   0        0        0     1128 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/pickler/main.py
--rw-r--r--   0        0        0        0 2023-06-25 10:18:07.273150 timeout_executor-0.1.11/src/timeout_executor/py.typed
--rw-r--r--   0        0        0      754 2023-06-25 10:18:07.277150 timeout_executor-0.1.11/src/timeout_executor/readonly.py
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 timeout_executor-0.1.11/PKG-INFO
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

### Comparing `timeout_executor-0.1.11/LICENSE` & `timeout_executor-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.11/pyproject.toml` & `timeout_executor-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "timeout-executor"
-version = "0.1.11"                                             # will be replaced
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
 cloudpickle = { version = ">=2.2.1", optional = true }
-joblib = { version = "^1.2.0", optional = true }
 
 [tool.poetry.extras]
-all = ['billiard', "joblib", 'dill', 'cloudpickle']
+all = ['billiard', 'dill', 'cloudpickle']
 billiard = ['billiard', 'dill']
-joblib = ["joblib"]
 dill = ['dill']
 cloudpickle = ['cloudpickle']
 
 [tool.poetry.group.dev.dependencies]
 ruff = "0.0.275"
 black = "23.3.0"
 ipykernel = "^6.23.3"
```

### Comparing `timeout_executor-0.1.11/src/timeout_executor/concurrent/futures/_billiard/process.py` & `timeout_executor-0.1.9/src/timeout_executor/concurrent/futures/_billiard/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,15 +380,16 @@
         )
         return _chain_from_iterable_of_lists(results)
 
     @override
     def shutdown(
         self,
         wait: bool = True,  # noqa: FBT001
-        cancel_futures: bool = False,  # noqa: FBT001
+        *,
+        cancel_futures: bool = False,
     ) -> None:
         with self._shutdown_lock:
             self._cancel_pending_futures = cancel_futures
             self._shutdown_thread = True
             if self._executor_manager_thread_wakeup is not None:
                 # Wake up queue management thread
                 self._executor_manager_thread_wakeup.wakeup()
```

### Comparing `timeout_executor-0.1.11/src/timeout_executor/concurrent/futures/_multiprocessing/process.py` & `timeout_executor-0.1.9/src/timeout_executor/concurrent/futures/_multiprocessing/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,16 @@
         )
         return _chain_from_iterable_of_lists(results)
 
     @override
     def shutdown(
         self,
         wait: bool = True,  # noqa: FBT001
-        cancel_futures: bool = False,  # noqa: FBT001
+        *,
+        cancel_futures: bool = False,
     ) -> None:
         with self._shutdown_lock:
             self._cancel_pending_futures = cancel_futures
             self._shutdown_thread = True
             if self._executor_manager_thread_wakeup is not None:
                 # Wake up queue management thread
                 self._executor_manager_thread_wakeup.wakeup()
```

### Comparing `timeout_executor-0.1.11/src/timeout_executor/executor.py` & `timeout_executor-0.1.9/src/timeout_executor/executor.py`

 * *Files 9% similar despite different names*

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
@@ -13,36 +14,38 @@
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
-    from timeout_executor.concurrent.futures import _joblib as joblib_future
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
@@ -55,14 +58,15 @@
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
@@ -103,15 +107,15 @@
             pickable func result
         """
         executor = get_executor(self._select[0], self._select[1])
         with executor(1, initializer=self._partial_init()) as pool:
             future = pool.submit(func, *args, **kwargs)
             wait([future], timeout=self.timeout)
             if not future.done():
-                pool.shutdown(False, True)  # noqa: FBT003
+                pool.shutdown(wait=False, cancel_futures=True)
                 error_msg = f"timeout > {self.timeout}s"
                 raise TimeoutError(error_msg)
             return future.result()
 
     async def apply_async(
         self,
         func: Callable[ParamT, Coroutine[None, None, ResultT]],
@@ -141,15 +145,15 @@
                     *args,
                     _timeout=self.timeout,
                     **kwargs,
                 )
                 coro = asyncio.wrap_future(future)
                 return await coro
             except TimeoutError:
-                pool.shutdown(False, True)  # noqa: FBT003
+                pool.shutdown(wait=False, cancel_futures=True)
                 raise
 
 
 @overload
 def get_executor(
     context: Literal["multiprocessing"] | None = ...,
     pickler: PicklerType | None = ...,
@@ -163,63 +167,59 @@
     pickler: PicklerType | None = ...,
 ) -> type[billiard_future.ProcessPoolExecutor]:
     ...
 
 
 @overload
 def get_executor(
-    context: Literal["joblib"] = ...,
-    pickler: PicklerType | None = ...,
-) -> type[joblib_future.ProcessPoolExecutor]:
-    ...
-
-
-@overload
-def get_executor(
     context: str = ...,
     pickler: PicklerType | None = ...,
 ) -> (
     type[billiard_future.ProcessPoolExecutor]
     | type[multiprocessing_future.ProcessPoolExecutor]
-    | type[joblib_future.ProcessPoolExecutor]
 ):
     ...
 
 
 def get_executor(
     context: ContextType | str | None = None,
     pickler: PicklerType | None = None,
 ) -> (
     type[billiard_future.ProcessPoolExecutor]
     | type[multiprocessing_future.ProcessPoolExecutor]
-    | type[joblib_future.ProcessPoolExecutor]
 ):
     """get pool executor
 
     Args:
         context: billiard or multiprocessing. Defaults to None.
 
     Returns:
         ProcessPoolExecutor
     """
     context, pickler = _validate_context_and_pickler(context, pickler)
-    executor = get_context_executor(context)
-    if context == "joblib" and pickler == "pickle":
-        return executor
-
+    future_module = importlib.import_module(
+        f".concurrent.futures._{context}",
+        __package__,
+    )
+    executor = future_module.ProcessPoolExecutor
     _patch_or_unpatch(context, pickler)
+
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
@@ -229,17 +229,14 @@
             logger.warning("billiard will use dill")
             pickler = "dill"
         elif _check_deps("cloudpickle"):
             logger.warning("billiard will use cloudpickle")
             pickler = "cloudpickle"
         else:
             raise ModuleNotFoundError("Billiard needs dill or cloudpickle")
-    elif context == "joblib" and pickler != "pickle":
-        logger.warning("Joblib uses self-implemented lib.")
-        pickler = "pickle"
 
     return context, pickler
 
 
 def _patch_or_unpatch(context: ContextType, pickler: PicklerType) -> None:
     if pickler == "pickle":
         monkey_unpatch(context)
@@ -290,14 +287,38 @@
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

### Comparing `timeout_executor-0.1.11/src/timeout_executor/pickler/_billiard/patch.py` & `timeout_executor-0.1.9/src/timeout_executor/pickler/_billiard/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.11/src/timeout_executor/pickler/_cloudpickle.py` & `timeout_executor-0.1.9/src/timeout_executor/pickler/_cloudpickle.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.11/src/timeout_executor/pickler/_dill.py` & `timeout_executor-0.1.9/src/timeout_executor/pickler/_dill.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.11/src/timeout_executor/pickler/_multiprocessing/patch.py` & `timeout_executor-0.1.9/src/timeout_executor/pickler/_multiprocessing/patch.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.11/src/timeout_executor/pickler/base.py` & `timeout_executor-0.1.9/src/timeout_executor/pickler/base.py`

 * *Files identical despite different names*

### Comparing `timeout_executor-0.1.11/src/timeout_executor/readonly.py` & `timeout_executor-0.1.9/src/timeout_executor/readonly.py`

 * *Files identical despite different names*

