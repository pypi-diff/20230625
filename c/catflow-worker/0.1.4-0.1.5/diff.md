# Comparing `tmp/catflow-worker-0.1.4.tar.gz` & `tmp/catflow-worker-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catflow-worker-0.1.4.tar", last modified: Sun Jun 25 01:07:26 2023, max compression
+gzip compressed data, was "catflow-worker-0.1.5.tar", last modified: Sun Jun 25 17:12:04 2023, max compression
```

## Comparing `catflow-worker-0.1.4.tar` & `catflow-worker-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:07:26.853200 catflow-worker-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:07:26.845200 catflow-worker-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:07:26.849200 catflow-worker-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-25 01:07:26.853200 catflow-worker-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:07:26.849200 catflow-worker-0.1.4/catflow_worker/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/catflow_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/catflow_worker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-25 01:07:26.000000 catflow-worker-0.1.4/catflow_worker/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/catflow_worker/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/catflow_worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:07:26.849200 catflow-worker-0.1.4/catflow_worker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-25 01:07:26.000000 catflow-worker-0.1.4/catflow_worker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-25 01:07:26.000000 catflow-worker-0.1.4/catflow_worker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 01:07:26.000000 catflow-worker-0.1.4/catflow_worker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-25 01:07:26.000000 catflow-worker-0.1.4/catflow_worker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-25 01:07:26.000000 catflow-worker-0.1.4/catflow_worker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 01:07:26.853200 catflow-worker-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:07:26.853200 catflow-worker-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/tests/mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-25 01:05:34.000000 catflow-worker-0.1.4/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/catflow_worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/catflow_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/catflow_worker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/catflow_worker/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/catflow_worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/catflow_worker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/tests/mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/tests/test_worker.py
```

### Comparing `catflow-worker-0.1.4/.github/workflows/ci.yml` & `catflow-worker-0.1.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.4/.gitignore` & `catflow-worker-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.4/LICENSE` & `catflow-worker-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.4/PKG-INFO` & `catflow-worker-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catflow-worker
-Version: 0.1.4
+Version: 0.1.5
 Summary: Consumer/publisher loop for workers in an object recognition pipeline
 Author-email: Ian Kilgore <iank@iank.org>
 License: MIT License
         
         Copyright (c) 2023 Ian Kilgore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `catflow-worker-0.1.4/README.md` & `catflow-worker-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.4/catflow_worker/main.py` & `catflow-worker-0.1.5/catflow_worker/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 
 async def example_handler(
     msg: str, key: str, s3: Any, bucket: str
 ) -> Tuple[bool, List[Tuple[str, str]]]:
     """Example message handler function
 
     Queries S3 for metadata about the object in the message and displays it."""
-    print(f"[*] Message received ({key}): {msg}")
-    s3obj = await s3.get_object(Bucket=bucket, Key=msg)
-    obj_info = s3obj["ResponseMetadata"]["HTTPHeaders"]
-    print(f"[-] Content-Type {obj_info['content-type']}")
-    print(f"[-] Content-Length {obj_info['content-length']}")
+    print(f"[*] Message received ({key}):")
+
+    for s3key in msg:
+        s3obj = await s3.get_object(Bucket=bucket, Key=s3key)
+        obj_info = s3obj["ResponseMetadata"]["HTTPHeaders"]
+        print(f"[-] {s3key}:")
+        print(f"    Content-Type {obj_info['content-type']}")
+        print(f"    Content-Length {obj_info['content-length']}")
 
     return True, []
 
 
 async def shutdown(worker, task):
     await worker.shutdown()
     task.cancel()
```

### Comparing `catflow-worker-0.1.4/catflow_worker/worker.py` & `catflow-worker-0.1.5/catflow_worker/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Callable, Any
 import os
 import aio_pika
 import aioboto3
+import json
 
 
 class Producer:
     @classmethod
     async def create(cls, url, exchange_name):
         self = Producer()
         self.connection = await aio_pika.connect_robust(url)
@@ -63,25 +64,27 @@
             await queue.bind(self.producer.exchange, routing_key=self.topics)
 
             # Wait for messages
             async with queue.iterator() as queue_iter:
                 async for message in queue_iter:
                     # Call handler for each message
                     ok, responses = await self.handler(
-                        message.body.decode(), message.routing_key, s3, bucket_name
+                        json.loads(message.body), message.routing_key, s3, bucket_name
                     )
                     # Acknowledge if the handler has succeeded, but we'll assume
                     # that if they've provided responses AND a failure status that
                     # they still want the responses to be sent, so we'll hold off
                     # on exiting
                     if ok:
                         await message.ack()
 
                     # Send responses
                     for response in responses:
                         routing_key, message = response
-                        await self.producer.send_to_rabbitmq(routing_key, message)
+                        await self.producer.send_to_rabbitmq(
+                            routing_key, json.dumps(message)
+                        )
 
                     # Exit if the handler has failed
                     if not ok:
                         await self.producer.close()
                         return False
```

### Comparing `catflow-worker-0.1.4/catflow_worker.egg-info/PKG-INFO` & `catflow-worker-0.1.5/catflow_worker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catflow-worker
-Version: 0.1.4
+Version: 0.1.5
 Summary: Consumer/publisher loop for workers in an object recognition pipeline
 Author-email: Ian Kilgore <iank@iank.org>
 License: MIT License
         
         Copyright (c) 2023 Ian Kilgore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `catflow-worker-0.1.4/pyproject.toml` & `catflow-worker-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.4/tests/mock_server.py` & `catflow-worker-0.1.5/tests/mock_server.py`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.4/tests/test_worker.py` & `catflow-worker-0.1.5/tests/test_worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 import catflow_worker
 import asyncio
 import aioboto3
 from io import BytesIO
 import os
+import json
 
 from .mock_server import start_service
 from .mock_server import stop_process
 
 AMQP_EXCHANGE = "catflow-worker-pytest"
 S3_ENDPOINT_URL = "http://localhost:5002"
 AWS_BUCKET_NAME = "catflow-test"
@@ -44,18 +45,21 @@
     )
     async with session.client("s3", endpoint_url=S3_ENDPOINT_URL) as s3:
         await s3.create_bucket(Bucket=AWS_BUCKET_NAME)
         await s3.upload_fileobj(
             BytesIO(bytes("filecontents1", "utf-8")), AWS_BUCKET_NAME, "test1"
         )
         await s3.upload_fileobj(
-            BytesIO(bytes("filecontents2", "utf-8")), AWS_BUCKET_NAME, "test2"
+            BytesIO(bytes("filecontentsbatch1", "utf-8")), AWS_BUCKET_NAME, "testbatch1"
         )
         await s3.upload_fileobj(
-            BytesIO(bytes("filecontents2", "utf-8")), AWS_BUCKET_NAME, "test3"
+            BytesIO(bytes("filecontentsbatch2", "utf-8")), AWS_BUCKET_NAME, "testbatch2"
+        )
+        await s3.upload_fileobj(
+            BytesIO(bytes("filecontents3", "utf-8")), AWS_BUCKET_NAME, "fail3"
         )
 
     # Declare an exchange, we'll publish some test data to it
     channel = rabbitmq.channel()
     channel.exchange_declare(exchange=AMQP_EXCHANGE, exchange_type="topic")
 
     # Declare and bind a queue to receive 'responses' from the worker
@@ -65,48 +69,56 @@
     )
 
     # Set up test handler and run it
     messages_received = []
     files_received = []
 
     async def _handler(msg, key, s3, bucket):
-        s3obj = await s3.get_object(Bucket=bucket, Key=msg)
         nonlocal messages_received
         nonlocal files_received
 
         messages_received.append(key)
-        file_content = await s3obj["Body"].read()
-        files_received.append(file_content.decode("utf-8"))
+
+        for s3_key in msg:
+            s3obj = await s3.get_object(Bucket=bucket, Key=s3_key)
+            file_content = await s3obj["Body"].read()
+            files_received.append(file_content.decode("utf-8"))
 
         if key == "test.key1":
-            return True, [("test-response.key", file_content.decode("utf-8"))]
+            return True, [("test-response.key", [file_content.decode("utf-8")])]
         else:
             return True, []
 
     worker = await catflow_worker.Worker.create(
         _handler, "catflow-worker-testq", "test.*"
     )
     task = asyncio.create_task(worker.work())
 
     # Give the consumer a chance to connect and declare its queue, then publish messages
     await asyncio.sleep(1)
-    channel.basic_publish(AMQP_EXCHANGE, "test.key1", "test1")
-    channel.basic_publish(AMQP_EXCHANGE, "test.key2", "test2")
-    channel.basic_publish(AMQP_EXCHANGE, "fail.key3", "fail3")
+    channel.basic_publish(AMQP_EXCHANGE, "test.key1", json.dumps(["test1"]))
+    channel.basic_publish(
+        AMQP_EXCHANGE, "test.key2", json.dumps(["testbatch1", "testbatch2"])
+    )
+    channel.basic_publish(AMQP_EXCHANGE, "fail.key3", json.dumps(["fail3"]))
 
     # Wait a moment then shut it down
     await asyncio.sleep(1)
     await worker.shutdown()
     task.cancel()
     try:
         await task
     except asyncio.CancelledError:
         pass
 
+    assert len(messages_received) == 2
+    assert len(files_received) == 3
     assert set(messages_received) == set(["test.key1", "test.key2"])
-    assert set(files_received) == set(["filecontents1", "filecontents2"])
+    assert set(files_received) == set(
+        ["filecontents1", "filecontentsbatch1", "filecontentsbatch2"]
+    )
 
     _, _, body = channel.basic_get("pytest-responses")
-    assert body.decode() == "filecontents1"
+    assert json.loads(body) == ["filecontents1"]
 
     method_frame, _, _ = channel.basic_get("pytest-responses")
     assert method_frame is None, "too many responses"
```

