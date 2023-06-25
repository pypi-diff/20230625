# Comparing `tmp/rmy-0.1.1.tar.gz` & `tmp/rmy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmy-0.1.1.tar", max compression
+gzip compressed data, was "rmy-0.1.2.tar", max compression
```

## Comparing `rmy-0.1.1.tar` & `rmy-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-06-11 20:31:23.956812 rmy-0.1.1/LICENSE
--rw-r--r--   0        0        0      824 2023-06-13 20:55:51.596825 rmy-0.1.1/README.md
--rw-r--r--   0        0        0     1306 2023-06-13 20:58:00.585595 rmy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-13 20:28:42.319559 rmy-0.1.1/rmy/__init__.py
--rw-r--r--   0        0        0      350 2023-06-11 20:31:23.957694 rmy-0.1.1/rmy/abc.py
--rw-r--r--   0        0        0     8790 2023-06-13 20:16:31.807840 rmy-0.1.1/rmy/client_async.py
--rw-r--r--   0        0        0     2973 2023-06-13 20:14:14.297858 rmy-0.1.1/rmy/client_sync.py
--rw-r--r--   0        0        0     1604 2023-06-13 11:34:38.724113 rmy-0.1.1/rmy/common.py
--rw-r--r--   0        0        0     2410 2023-06-13 09:29:04.848659 rmy-0.1.1/rmy/connection.py
--rw-r--r--   0        0        0      429 2023-06-12 14:14:59.271940 rmy-0.1.1/rmy/pubsub.py
--rw-r--r--   0        0        0     8339 2023-06-13 20:28:06.769688 rmy-0.1.1/rmy/server.py
--rw-r--r--   0        0        0     1477 1970-01-01 00:00:00.000000 rmy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-11 20:31:23.956812 rmy-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1325 2023-06-25 09:49:45.108911 rmy-0.1.2/README.md
+-rw-r--r--   0        0        0     1677 2023-06-25 09:53:06.262494 rmy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      583 2023-06-25 09:52:35.536752 rmy-0.1.2/rmy/__init__.py
+-rw-r--r--   0        0        0      554 2023-06-20 06:58:29.140288 rmy-0.1.2/rmy/abc.py
+-rw-r--r--   0        0        0    11641 2023-06-24 09:22:09.871746 rmy-0.1.2/rmy/client_async.py
+-rw-r--r--   0        0        0     2263 2023-06-24 11:38:31.569083 rmy-0.1.2/rmy/client_sync.py
+-rw-r--r--   0        0        0     1325 2023-06-22 15:27:41.453103 rmy-0.1.2/rmy/common.py
+-rw-r--r--   0        0        0     2582 2023-06-20 17:35:21.011981 rmy-0.1.2/rmy/connection.py
+-rw-r--r--   0        0        0    10248 2023-06-24 10:07:16.682039 rmy-0.1.2/rmy/server.py
+-rw-r--r--   0        0        0     1853 1970-01-01 00:00:00.000000 rmy-0.1.2/PKG-INFO
```

### Comparing `rmy-0.1.1/LICENSE` & `rmy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rmy-0.1.1/rmy/client_async.py` & `rmy-0.1.2/rmy/client_async.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,232 +1,312 @@
+from __future__ import annotations
+
 import asyncio
 import contextlib
 import inspect
+import queue
 from collections.abc import AsyncIterable
 from functools import partial
 from itertools import count
-from typing import Any, AsyncIterator, Callable, Optional
+from typing import TYPE_CHECKING, Any, AsyncIterator, Callable, Dict, Optional
 
 import anyio
-from anyio.abc import TaskStatus
+import anyio.abc
+import asyncstdlib
 
-from .abc import Connection
-from .common import UserException, cancel_task_on_exit, closing_scope, scoped_insert
+from .abc import AsyncSink, Connection
+from .common import UserException, cancel_task_on_exit, scoped_insert
 from .connection import connect_to_tcp_server
 
 
+if TYPE_CHECKING:
+    from .client_sync import SyncClient
+
+
 OK = "OK"
 CLOSE_SENTINEL = "Close sentinel"
-CLOSE_STREAM = "Close stream"
 CANCELLED_TASK = "Cancelled task"
 EXCEPTION = "Exception"
 USER_EXCEPTION = "UserException"
 CREATE_OBJECT = "Create object"
 DELETE_OBJECT = "Delete object"
 FETCH_OBJECT = "Fetch object"
 GET_ATTRIBUTE = "Get attribute"
+SET_ATTRIBUTE = "Set attribute"
 ASYNC_ITERATOR = "Async iterator"
-AWAITABLE = "Awaitable"
-FUNCTION = "Function"
+MOVE_ASYNC_ITERATOR = "Move Async iterator"
+METHOD = "Function"
 ITER_ASYNC_ITERATOR = "Iter async iterator"
 STREAM_BUFFER_SIZE = 10
 
 SERVER_OBJECT_ID = 0
 
+ASYNC_SETATTR_ERROR_MESSAGE = "Cannot set attribute on remote object in async mode. Use setattr method instead. \
+We intentionally do not support setting attributes using assignment operator on remote objects in async mode. \
+This is because it is not a good practice not too wait until a remote operation completes."
+
+ASYNC_GENERATOR_OVERFLOWED_MESSAGE = "Async generator overflowed."
+
+REQUEST_CODES = (METHOD, GET_ATTRIBUTE, CREATE_OBJECT, FETCH_OBJECT, SET_ATTRIBUTE)
+
+
+class IterationBufferSync(AsyncSink):
+    def __init__(self, size: int) -> None:
+        self._overflowed = False
+        self._size = size
+        self._queue = queue.SimpleQueue()
+
+    def send_nowait(self, value: Any):
+        self._queue.put_nowait(value)
+        if self._queue.qsize() >= self._size:
+            self._overflowed = True
+            raise asyncio.QueueFull()
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self._overflowed:
+            raise OverflowError(ASYNC_GENERATOR_OVERFLOWED_MESSAGE)
+        return self._queue.get()
+
+
+class IterationBufferAsync(AsyncSink):
+    def __init__(self, size: int) -> None:
+        self._overflowed = False
+        self._queue = asyncio.Queue(maxsize=size)
+
+    def send_nowait(self, value: Any):
+        try:
+            self._queue.put_nowait(value)
+        except asyncio.QueueFull:
+            self._overflowed = True
+            raise
+
+    def __aiter__(self):
+        return self
+
+    async def __anext__(self):
+        if self._overflowed:
+            raise OverflowError(ASYNC_GENERATOR_OVERFLOWED_MESSAGE)
+        return await self._queue.get()
 
-class Result(AsyncIterable):
+
+class AsyncCallResult(AsyncIterable):
     def __init__(self, client, object_id: int, function: Callable, args, kwargs):
-        self.client: "AsyncClient" = client
+        self.client: AsyncClient = client
         self.object_id = object_id
         self.function = function
         self.args = args
         self.kwargs = kwargs
 
     def __await__(self):
         return asyncio.create_task(
             self.client.execute_request(
-                AWAITABLE,
+                METHOD,
                 (self.object_id, self.function, self.args, self.kwargs),
                 is_cancellable=True,
                 include_code=False,
             )
         ).__await__()
 
     def __aiter__(self):
-        return self.client.evaluate_async_generator(
+        return self.client._evaluate_async_generator(
             self.object_id, self.function, self.args, self.kwargs
         )
 
 
 def decode_result(code, result, include_code=True):
-    if code in (CANCELLED_TASK, OK, AWAITABLE, ASYNC_ITERATOR):
+    if code in (CANCELLED_TASK, OK, ASYNC_ITERATOR):
         return (code, result) if include_code else result
     if code == USER_EXCEPTION:
         raise UserException(result)
     if code == EXCEPTION:
         if isinstance(result, Exception):
             raise result
         raise Exception(result)
     else:
         raise Exception(f"Unexpected code {code} received.")
 
 
+def decode_iteration_result(code, result):
+    if code in (CLOSE_SENTINEL, CANCELLED_TASK):
+        return True, None
+    return False, decode_result(code, result, include_code=False)
+
+
 class RemoteObject:
     def __init__(self, client, object_id: int):
         self.client = client
         self.object_id = object_id
 
 
+def __setattr_forbidden__(_self, _name, _value):
+    raise AttributeError(ASYNC_SETATTR_ERROR_MESSAGE)
+
+
 class AsyncClient:
-    def __init__(self, task_group, connection: Connection) -> None:
-        self.task_group = task_group
+    def __init__(
+        self, connection: Connection, async_buffer_size: int = STREAM_BUFFER_SIZE
+    ) -> None:
         self.connection = connection
+        self._async_buffer_size = async_buffer_size
         self.request_id = count()
         self.object_id = count()
         self.pending_requests = {}
-        self.async_generators_streams = {}
+        self._iteraton_buffers: Dict[int, AsyncSink] = {}
         self.remote_objects = {}
-        self.closed = False
-
-    def close(self):
-        self.closed = True
 
-    async def send(self, *args):
-        if self.closed:
-            raise RuntimeError("Client closed.")
+    async def _send(self, *args):
         await self.connection.send(args)
 
-    def send_nowait(self, *args):
-        if self.closed:
-            raise RuntimeError("Client closed.")
+    def _send_nowait(self, *args):
         self.connection.send_nowait(args)
 
-    async def process_messages_from_server(
-        self, task_status: TaskStatus = anyio.TASK_STATUS_IGNORED
+    async def _process_messages_from_server(
+        self, task_status: anyio.abc.TaskStatus = anyio.TASK_STATUS_IGNORED
     ):
         task_status.started()
         async for code, message_id, status, result in self.connection:
-            if code in (FUNCTION, AWAITABLE, GET_ATTRIBUTE, CREATE_OBJECT, FETCH_OBJECT):
-                future = self.pending_requests.get(message_id)
-                if future:
+            if code in REQUEST_CODES:
+                if future := self.pending_requests.get(message_id):
                     future.set_result((status, result))
             elif code == ITER_ASYNC_ITERATOR:
-                sink = self.async_generators_streams.get(message_id)
-                if sink:
-                    try:
-                        sink.send_nowait((status, result))
-                    except anyio.WouldBlock as e:
-                        sink.close()
+                if queue := self._iteraton_buffers.get(message_id):
+                    queue.send_nowait((status, result))
             elif code == CANCELLED_TASK:
                 print("Task cancelled.", message_id, status, result)
             else:
                 print(f"Unexpected code {code} received.")
 
     @contextlib.contextmanager
-    def submit_request(self, code, args, is_cancellable=False):
+    def _submit_request(self, code, args, is_cancellable=False):
         request_id = next(self.request_id)
         future = asyncio.Future()
         with scoped_insert(self.pending_requests, request_id, future):
-            self.send_nowait(code, request_id, args)
+            self._send_nowait(code, request_id, args)
             try:
                 yield future
             except anyio.get_cancelled_exc_class():
                 if is_cancellable:
-                    self.cancel_task(request_id)
+                    self._cancel_request_no_wait(request_id)
                 raise
 
     async def execute_request(self, code, args, is_cancellable=False, include_code=True) -> Any:
-        with self.submit_request(code, args, is_cancellable) as future:
+        with self._submit_request(code, args, is_cancellable) as future:
             return decode_result(*(await future), include_code=include_code)
 
-    async def get_attribute(self, object_id: int, name: str):
+    async def _get_attribute(self, object_id: int, name: str):
         return await self.execute_request(GET_ATTRIBUTE, (object_id, name), include_code=False)
 
-    def remote_method(self, object_id: int, function: Callable, *args, **kwargs) -> Any:
-        return Result(self, object_id, function, args, kwargs)
+    async def _set_attribute(self, object_id: int, name: str, value: Any):
+        return await self.execute_request(
+            SET_ATTRIBUTE, (object_id, name, value), include_code=False
+        )
+
+    def _call_method_remotely(self, object_id: int, function: Callable, *args, **kwargs) -> Any:
+        return AsyncCallResult(self, object_id, function, args, kwargs)
 
-    def cancel_task(self, request_id: int):
-        self.send_nowait(CANCELLED_TASK, request_id, None)
+    def _cancel_request_no_wait(self, request_id: int):
+        self._send_nowait(CANCELLED_TASK, request_id, None)
         self.pending_requests.pop(request_id, None)
 
-    async def evaluate_async_generator(self, object_id, function, args, kwargs):
-        iterator_id = await self.execute_request(
-            FUNCTION,
+    async def _cancel_request(self, request_id: int):
+        self._cancel_request_no_wait(request_id)
+        await self.connection.drain()
+
+    async def _evaluate_async_generator(self, object_id, function, args, kwargs):
+        push_or_pull, generator_id = await self.execute_request(
+            METHOD,
             (object_id, function, args, kwargs),
             is_cancellable=True,
             include_code=False,
         )
-        async for value in self.iter_async_generator(iterator_id):
-            yield value
-
-    async def iter_async_generator(self, iterator_id: int):
-        sink, stream = anyio.create_memory_object_stream(STREAM_BUFFER_SIZE)
+        queue = IterationBufferAsync(self._async_buffer_size)
         request_id = next(self.request_id)
-        with scoped_insert(self.async_generators_streams, request_id, sink):
-            await self.send(ITER_ASYNC_ITERATOR, request_id, iterator_id)
+        with scoped_insert(self._iteraton_buffers, request_id, queue):
+            await self._send(ITER_ASYNC_ITERATOR, request_id, (generator_id,))
             try:
-                async for code, value in stream:
-                    if code == OK:
-                        yield value
-                    elif code in (CLOSE_SENTINEL, CANCELLED_TASK):
+                async for index, (terminated, value) in asyncstdlib.enumerate(
+                    asyncstdlib.starmap(decode_iteration_result, queue)
+                ):
+                    if terminated:
                         break
-                    elif code == USER_EXCEPTION:
-                        raise UserException(value)
-                    else:
-                        raise Exception(value)
+                    yield value
+                    if not push_or_pull:
+                        await self._send(MOVE_ASYNC_ITERATOR, generator_id, (index + 1,))
+            finally:
+                await self._cancel_request(request_id)
+
+    @contextlib.asynccontextmanager
+    async def _remote_sync_generator_iter(self, iterator_id: int):
+        queue = IterationBufferSync(self._async_buffer_size)
+        request_id = next(self.request_id)
+        with scoped_insert(self._iteraton_buffers, request_id, queue):
+            try:
+                await self._send(ITER_ASYNC_ITERATOR, request_id, (iterator_id,))
+                yield queue
             finally:
-                self.cancel_task(request_id)
+                await self._cancel_request(request_id)
 
     @contextlib.asynccontextmanager
     async def create_remote_object(
-        self, object_class, args=(), kwarg={}, sync_client: Optional["SyncClient"] = None
+        self, object_class, args=(), kwarg={}, sync_client: Optional[SyncClient] = None
     ):
         object_id = await self.execute_request(
             CREATE_OBJECT, (object_class, args, kwarg), include_code=False
         )
         try:
-            yield await self.fetch_remote_object(object_id, sync_client)
+            yield await self._fetch_remote_object(object_id, sync_client)
         finally:
             with anyio.CancelScope(shield=True):
-                await self.send(DELETE_OBJECT, 0, object_id)
+                await self._send(DELETE_OBJECT, 0, object_id)
 
-    async def fetch_remote_object(
-        self, object_id: int = SERVER_OBJECT_ID, sync_client: Optional["SyncClient"] = None
+    async def _fetch_remote_object(
+        self, object_id: int = SERVER_OBJECT_ID, sync_client: Optional[SyncClient] = None
     ) -> Any:
         if object_id not in self.remote_objects:
             object_class = await self.execute_request(FETCH_OBJECT, object_id, include_code=False)
-            __getattr__ = partial(self.get_attribute, object_id)
+            setattr = partial(self._set_attribute, object_id)
+            __getattr__ = partial(self._get_attribute, object_id)
             if sync_client:
-                __getattr__ = sync_client.wrap_awaitable(__getattr__)
+                __getattr__ = sync_client._wrap_awaitable(__getattr__)
+                setattr = __setattr__ = sync_client._wrap_awaitable(setattr)
+            else:
+                __setattr__ = __setattr_forbidden__
             object_class = type(
                 f"{object_class.__name__}Proxy",
                 (RemoteObject, object_class),
-                {"__getattr__": __getattr__},
+                {"__getattr__": __getattr__, "setattr": setattr, "__setattr__": __setattr__},
             )
             remote_object = object_class.__new__(object_class)
-            RemoteObject.__init__(remote_object, self, object_id)
+            object.__setattr__(remote_object, "client", self)
+            object.__setattr__(remote_object, "object_id", object_id)
             for name in dir(object_class):
                 if name.startswith("__") and name.endswith("__"):
                     continue
                 attribute = getattr(object_class, name)
                 if inspect.isfunction(attribute):
-                    method = partial(self.remote_method, object_id, attribute)
+                    method = partial(self._call_method_remotely, object_id, attribute)
                     if sync_client:
-                        method = sync_client.wrap_function(object_id, attribute)
-                    setattr(remote_object, name, method)
+                        method = sync_client._wrap_function(object_id, attribute)
+                    object.__setattr__(remote_object, name, method)
             self.remote_objects[object_id] = remote_object
         return self.remote_objects[object_id]
 
+    async def fetch_remote_object(self, object_id: int = SERVER_OBJECT_ID):
+        return await self._fetch_remote_object(object_id)
+
 
 @contextlib.asynccontextmanager
-async def _create_async_client(task_group, connection: Connection) -> AsyncIterator[AsyncClient]:
-    with closing_scope(AsyncClient(task_group, connection)) as client:
-        with cancel_task_on_exit(client.process_messages_from_server()):
-            yield client
+async def create_async_client(connection: Connection) -> AsyncIterator[AsyncClient]:
+    client = AsyncClient(connection)
+    with cancel_task_on_exit(client._process_messages_from_server()):
+        yield client
 
 
 @contextlib.asynccontextmanager
 async def connect(host_name: str, port: int) -> AsyncIterator[AsyncClient]:
     async with anyio.create_task_group() as task_group:
         async with connect_to_tcp_server(host_name, port) as connection:
-            async with _create_async_client(task_group, connection) as client:
+            async with create_async_client(connection) as client:
                 yield client
```

### Comparing `rmy-0.1.1/rmy/client_sync.py` & `rmy-0.1.2/rmy/client_sync.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,66 @@
 import contextlib
+import itertools
 from typing import Iterator
 
 import anyio
-import janus
 
 from .client_async import (
     ASYNC_ITERATOR,
-    AWAITABLE,
-    CLOSE_STREAM,
-    EXCEPTION,
-    FUNCTION,
+    MOVE_ASYNC_ITERATOR,
     OK,
+    METHOD,
     SERVER_OBJECT_ID,
     AsyncClient,
     connect,
+    decode_iteration_result,
 )
-from .common import cancel_task_on_exit
 
 
 class SyncClient:
     def __init__(self, portal, async_client) -> None:
         self.portal = portal
         self.async_client: AsyncClient = async_client
 
-    @contextlib.asynccontextmanager
-    async def remote_async_iterate(self, iterator_id):
-        queue = janus.Queue()
-
-        async def forward_to_main_thread():
-            try:
-                async for value in self.async_client.iter_async_generator(iterator_id):
-                    await queue.async_q.put((OK, value))
-            except anyio.get_cancelled_exc_class():
-                raise
-            except Exception as e:
-                await queue.async_q.put((EXCEPTION, e))
-            finally:
-                await queue.async_q.put((CLOSE_STREAM, None))
-
-        def result_sync_iterator():
-            while True:
-                code, message = queue.sync_q.get()
-                if code in CLOSE_STREAM:
-                    queue.close()
-                    break
-                if code is EXCEPTION:
-                    queue.close()
-                    raise message
-                yield message
-
-        with cancel_task_on_exit(forward_to_main_thread()):
-            yield result_sync_iterator()
-
-    def sync_generator(self, iterator_id: int):
+    def _sync_generator_iter(self, push_or_pull, generator_id):
         with self.portal.wrap_async_context_manager(
-            self.remote_async_iterate(iterator_id)
+            self.async_client._remote_sync_generator_iter(generator_id)
         ) as sync_iterator:
-            yield from sync_iterator
+            for index, (terminated, value) in enumerate(itertools.starmap(decode_iteration_result, sync_iterator)):
+                if terminated:
+                    break
+                yield value
+                if not push_or_pull:
+                    self.portal.call(self.async_client._send, MOVE_ASYNC_ITERATOR, generator_id, (index + 1,))
 
-    def wrap_function(self, object_id, function):
+    def _wrap_function(self, object_id, function):
         def result(*args, **kwargs):
             code, result = self.portal.call(
-                self.async_client.execute_request, FUNCTION, (object_id, function, args, kwargs)
+                self.async_client.execute_request, METHOD, (object_id, function, args, kwargs)
             )
-            if code == AWAITABLE:
+            if code == OK:
                 return result
             elif code == ASYNC_ITERATOR:
-                return self.sync_generator(result)
+                return self._sync_generator_iter(*result)
 
         return result
 
-    def create_remote_object(self, object_class, args=(), kwarg={}):
-        return self.portal.wrap_async_context_manager(
-            self.async_client.create_remote_object(object_class, args, kwarg, sync_client=self)
-        )
-
-    def wrap_awaitable(self, method):
+    def _wrap_awaitable(self, method):
         def result(_self, *args, **kwargs):
             return self.portal.call(method, *args, **kwargs)
 
         return result
 
     def fetch_remote_object(self, object_id: int = SERVER_OBJECT_ID):
-        return self.portal.call(self.async_client.fetch_remote_object, object_id, self)
+        return self.portal.call(self.async_client._fetch_remote_object, object_id, self)
+
+    def create_remote_object(self, object_class, args=(), kwarg={}):
+        return self.portal.wrap_async_context_manager(
+            self.async_client.create_remote_object(object_class, args, kwarg, sync_client=self)
+        )
 
 
 @contextlib.contextmanager
 def create_sync_client(host_name: str, port: int) -> Iterator[SyncClient]:
     with anyio.start_blocking_portal("asyncio") as portal:
         with portal.wrap_async_context_manager(connect(host_name, port)) as async_client:
             yield SyncClient(portal, async_client)
```

### Comparing `rmy-0.1.1/rmy/common.py` & `rmy-0.1.2/rmy/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,33 +32,23 @@
 def scoped_iter(iterable):
     try:
         yield iterable
     finally:
         iterable.close()
 
 
-closing_scope = scoped_iter
-
-
 @contextlib.contextmanager
 def cancel_task_on_exit(coroutine: Coroutine):
     task = asyncio.create_task(coroutine)
     try:
         yield task
     finally:
         task.cancel()
 
 
-@contextlib.asynccontextmanager
-async def execute_cancellable_coroutine(method, *args, **kwargs):
-    async with anyio.create_task_group() as task_group:
-        task_group.start_soon(method, *args, **kwargs)
-        yield task_group.cancel_scope
-
-
 async def cancel_task_group_on_signal(task_group: anyio.abc.TaskGroup):
     with anyio.open_signal_receiver(signal.SIGINT, signal.SIGTERM) as signals:
         async for signum in signals:
             if signum == signal.SIGINT:
                 print("Ctrl+C pressed!")
             else:
                 print(f"Received signal {signum}, terminating.")
```

### Comparing `rmy-0.1.1/rmy/connection.py` & `rmy-0.1.2/rmy/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,22 +35,30 @@
         self.throw_on_eof = throw_on_eof
         self._closing = False
 
     def send_nowait(self, message: Tuple[Any, ...]):
         message_as_bytes = self.serialize(message)
         self.writer.write(struct.pack(FORMAT, len(message_as_bytes)) + message_as_bytes)
 
+    async def drain(self):
+        await self.writer.drain()
+
     async def send(self, message: Tuple[Any, ...]):
         self.send_nowait(message)
         try:
             await self.writer.drain()
         except ConnectionResetError:
             if self.throw_on_eof:
                 raise
 
+    def close(self):
+        self._closing = True
+        self.writer.close()
+        self.reader.feed_eof()
+
     async def __anext__(self):
         try:
             length = await self.reader.readexactly(SIZE_LENGTH)
             return self.deserialize(
                 await self.reader.readexactly(struct.unpack(FORMAT, length)[0])
             )
         except (IncompleteReadError, ConnectionResetError, BrokenPipeError):
```

### Comparing `rmy-0.1.1/rmy/server.py` & `rmy-0.1.2/rmy/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,126 @@
+from __future__ import annotations
+
 import asyncio
 import contextlib
 import traceback
 from itertools import count
 from typing import Any
-
+import inspect
 import anyio
 import anyio.abc
 import asyncstdlib
 
 from .abc import Connection
 from .client_async import (
     ASYNC_ITERATOR,
-    AWAITABLE,
     CANCELLED_TASK,
     CLOSE_SENTINEL,
     CREATE_OBJECT,
     DELETE_OBJECT,
     EXCEPTION,
     FETCH_OBJECT,
-    FUNCTION,
     GET_ATTRIBUTE,
     ITER_ASYNC_ITERATOR,
+    MOVE_ASYNC_ITERATOR,
+    METHOD,
     OK,
+    SET_ATTRIBUTE,
     USER_EXCEPTION,
 )
-from .common import (
-    UserException,
-    cancel_task_group_on_signal,
-    cancel_task_on_exit,
-    execute_cancellable_coroutine,
-    print_error_stack,
-    scoped_insert,
-)
+from .common import UserException, cancel_task_group_on_signal, scoped_insert
 from .connection import TCPConnection
 
 
+async def wrap_sync_generator(sync_generator):
+    for value in sync_generator:
+        yield value
+
+
+async def wrap_coroutine(coroutine):
+    return OK, await coroutine
+
+
 class ClientSession:
     def __init__(self, server, task_group, connection: Connection) -> None:
-        self.session_manager: "SessionManager" = server
+        self.session_manager: Server = server
         self.task_group = task_group
         self.connection = connection
         self.running_tasks = {}
-        self.pending_async_generators = {}
+        self.pending_generators = {}
         self.own_objects = set()
+        self.synchronization_indexes = {}
 
     async def send(self, code: str, request_id: int, status: str, value: Any):
         await self.connection.send((code, request_id, status, value))
 
     def send_nowait(self, code: str, request_id: int, status: str, value: Any):
         self.connection.send_nowait((code, request_id, status, value))
 
-    async def evaluate_coroutine_or_async_generator(
-        self, request_id, task_type, coroutine_or_async_generator
+    async def iterate_through_async_generator_unsync(
+        self, request_id: int, iterator_id: int, coroutine_or_async_generator
     ):
-        code, result = CLOSE_SENTINEL, None
-        try:
-            if asyncio.iscoroutine(coroutine_or_async_generator):
-                code, result = AWAITABLE, await coroutine_or_async_generator
-            else:
-                async with asyncstdlib.scoped_iter(coroutine_or_async_generator) as aiter:
-                    async for value in aiter:
-                        await self.send(task_type, request_id, OK, value)
+        async with asyncstdlib.scoped_iter(coroutine_or_async_generator) as aiter:
+            async for value in aiter:
+                await self.send(ITER_ASYNC_ITERATOR, request_id, OK, value)
+        return CLOSE_SENTINEL, None
+
+    async def iterate_through_async_generator_sync(
+        self, request_id: int, iterator_id: int, coroutine_or_async_generator
+    ):
+        index_and_event = [0, anyio.Event()]
+        with scoped_insert(self.synchronization_indexes, iterator_id, index_and_event):
+            async with asyncstdlib.scoped_iter(coroutine_or_async_generator) as aiter:
+                async for index, value in asyncstdlib.enumerate(aiter):
+                    await self.send(ITER_ASYNC_ITERATOR, request_id, OK, value)
+                    if index >= index_and_event[0]:
+                        await index_and_event[1].wait()
+            return CLOSE_SENTINEL, None
+
+    def iterate_generator(self, request_id: int, iterator_id: int):
+        if not (generator := self.pending_generators.pop(iterator_id, None)):
+            return
+        push, generator = generator
+        method = (
+            self.iterate_through_async_generator_unsync
+            if push
+            else self.iterate_through_async_generator_sync
+        )
+        self.cancellable_run_task(
+            request_id, ITER_ASYNC_ITERATOR, method(request_id, iterator_id, generator)
+        )
 
+    async def run_task(self, request_id, task_code, coroutine_or_async_generator):
+        status, result = EXCEPTION, None
+        try:
+            status, result = await coroutine_or_async_generator
         except anyio.get_cancelled_exc_class():
-            code = CANCELLED_TASK
+            status = CANCELLED_TASK
             raise
         except UserException as e:
-            code, result = USER_EXCEPTION, e.args[0]
+            status, result = USER_EXCEPTION, e.args[0]
         except Exception:
-            code, result = EXCEPTION, traceback.format_exc()
-            raise
+            status, result = EXCEPTION, traceback.format_exc()
         finally:
             with anyio.CancelScope(shield=True):
-                await self.send(task_type, request_id, code, result)
+                await self.send(task_code, request_id, status, result)
 
-    async def run_task(self, request_id, task_type, coroutine_or_async_context):
-        try:
-            async with execute_cancellable_coroutine(
-                self.evaluate_coroutine_or_async_generator,
-                request_id,
-                task_type,
-                coroutine_or_async_context,
-            ) as self.running_tasks[request_id]:
-                pass
-        finally:
-            self.running_tasks.pop(request_id, None)
+    def cancellable_run_task(self, request_id, task_code, coroutine_or_async_context):
+        async def task():
+            task_group = anyio.create_task_group()
+            with scoped_insert(self.running_tasks, request_id, task_group.cancel_scope.cancel):
+                async with task_group:
+                    task_group.start_soon(
+                        self.run_task,
+                        request_id,
+                        task_code,
+                        coroutine_or_async_context,
+                    )
+
+        self.task_group.start_soon(task)
 
     async def create_object(self, request_id, object_class, args, kwarg):
         object_id = next(self.session_manager.object_id)
         code, message = OK, object_id
         try:
             self.session_manager.objects[object_id] = object_class(
                 self.session_manager.server_object, *args, **kwarg
@@ -102,100 +134,105 @@
         maybe_object = self.session_manager.objects.get(object_id)
         if maybe_object is not None:
             await self.send(FETCH_OBJECT, request_id, OK, maybe_object.__class__)
         else:
             await self.send(FETCH_OBJECT, request_id, EXCEPTION, f"Object {object_id} not found")
 
     async def get_attribute(self, request_id, object_id, name):
-        code, message = OK, None
+        code, value = OK, None
         try:
             value = getattr(self.session_manager.objects[object_id], name)
-            await self.send(GET_ATTRIBUTE, request_id, OK, value)
         except Exception as e:
-            code, message = EXCEPTION, e
-        await self.send(GET_ATTRIBUTE, request_id, code, message)
+            code, value = EXCEPTION, e
+        await self.send(GET_ATTRIBUTE, request_id, code, value)
+
+    async def set_attribute(self, request_id, object_id, name, value):
+        code, result = OK, None
+        try:
+            setattr(self.session_manager.objects[object_id], name, value)
+        except Exception as e:
+            code, result = EXCEPTION, e
+        await self.send(SET_ATTRIBUTE, request_id, code, result)
 
     async def cancel_running_task(self, request_id: int):
-        running_task = self.running_tasks.get(request_id)
-        if running_task:
-            running_task.cancel()
-            await running_task
+        if running_task := self.running_tasks.get(request_id):
+            running_task()
+
+    def move_async_generator_index(self, request_id: int, index: int):
+        if index_and_event := self.synchronization_indexes.get(request_id, None):
+            index_and_event[1].set()
+            index_and_event[0] = index
+            index_and_event[1] = anyio.Event()
+
+    async def evaluate_method(self, request_id, task_code, object_id, method, args, kwargs):
+        result = method(self.session_manager.objects[object_id], *args, **kwargs)
+        if inspect.iscoroutine(result):
+            self.cancellable_run_task(request_id, task_code, wrap_coroutine(result))
+        elif inspect.isasyncgen(result) or inspect.isgenerator(result):
+            is_async = inspect.isasyncgen(result)
+            self.pending_generators[request_id] = (is_async, result)
+            await self.send(task_code, request_id, ASYNC_ITERATOR, (is_async, request_id))
+        else:
+            await self.send(task_code, request_id, OK, result)
 
     async def process_messages(self):
-        async for code, request_id, payload in self.connection:
+        async for task_code, request_id, payload in self.connection:
             try:
-                if code in (FUNCTION, AWAITABLE):
-                    object_id, function, args, kwargs = payload
-                    coroutine_or_async_context = function(
-                        self.session_manager.objects[object_id], *args, **kwargs
-                    )
-                    if code != FUNCTION or asyncio.iscoroutine(coroutine_or_async_context):
-                        self.task_group.start_soon(
-                            self.run_task,
-                            request_id,
-                            code,
-                            coroutine_or_async_context,
-                        )
-                    else:
-                        self.pending_async_generators[request_id] = coroutine_or_async_context
-                        await self.send(code, request_id, ASYNC_ITERATOR, request_id)
-                elif code == CANCELLED_TASK:
+                if task_code == METHOD:
+                    await self.evaluate_method(request_id, task_code, *payload)
+                elif task_code == CANCELLED_TASK:
                     await self.cancel_running_task(request_id)
-                elif code == ITER_ASYNC_ITERATOR:
-                    self.task_group.start_soon(
-                        self.run_task,
-                        request_id,
-                        code,
-                        self.pending_async_generators.pop(payload),
-                    )
-                elif code == GET_ATTRIBUTE:
+                elif task_code == ITER_ASYNC_ITERATOR:
+                    self.iterate_generator(request_id, *payload)
+                elif task_code == GET_ATTRIBUTE:
                     await self.get_attribute(request_id, *payload)
-                elif code == CREATE_OBJECT:
+                elif task_code == SET_ATTRIBUTE:
+                    await self.set_attribute(request_id, *payload)
+                elif task_code == CREATE_OBJECT:
                     await self.create_object(request_id, *payload)
-                elif code == FETCH_OBJECT:
+                elif task_code == FETCH_OBJECT:
                     await self.fetch_object(request_id, payload)
-                elif code == DELETE_OBJECT:
+                elif task_code == MOVE_ASYNC_ITERATOR:
+                    self.move_async_generator_index(request_id, *payload)
+                elif task_code == DELETE_OBJECT:
                     self.session_manager.objects.pop(payload, None)
                     self.own_objects.discard(payload)
                 else:
-                    raise Exception(f"Unknown code {repr(code)} with payload {repr(payload)}")
+                    raise Exception(f"Unknown code {repr(task_code)} with payload {repr(payload)}")
             except anyio.get_cancelled_exc_class():
                 raise
             except Exception:
                 stack = traceback.format_exc()
-                await self.send(code, request_id, EXCEPTION, stack)
+                await self.send(task_code, request_id, EXCEPTION, stack)
 
     async def aclose(self):
         self.task_group.cancel_scope.cancel()
         for object_id in self.own_objects:
             self.session_manager.objects.pop(object_id, None)
 
 
-class SessionManager:
+class Server:
     def __init__(self, server_object: Any) -> None:
         self.server_object = server_object
         self.client_sessions = {}
         self.client_session_id = count()
         self.object_id = count()
         self.objects = {next(self.object_id): server_object}
 
     @contextlib.asynccontextmanager
     async def on_new_connection(self, connection: Connection):
-        with print_error_stack():
-            async with anyio.create_task_group() as task_group:
-                client_session = ClientSession(self, task_group, connection)
-                with scoped_insert(
-                    self.client_sessions, next(self.client_session_id), client_session
-                ):
-                    async with asyncstdlib.closing(client_session):
-                        yield client_session
+        async with anyio.create_task_group() as session_task_group:
+            client_session = ClientSession(self, session_task_group, connection)
+            with scoped_insert(self.client_sessions, next(self.client_session_id), client_session):
+                async with asyncstdlib.closing(client_session):
+                    yield client_session
 
 
 async def _serve_tcp(port: int, server_object: Any):
-    session_manager = SessionManager(server_object)
+    session_manager = Server(server_object)
 
     async def on_new_connection_raw(reader, writer):
         async with session_manager.on_new_connection(
             TCPConnection(reader, writer, throw_on_eof=False)
         ) as client_core:
             await client_core.process_messages()
```

