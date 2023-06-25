# Comparing `tmp/dsr_agent-0.0.3.tar.gz` & `tmp/dsr_agent-0.0.4.tar.gz`

## Comparing `dsr_agent-0.0.3.tar` & `dsr_agent-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/dsr_agent/__init__.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/dsr_agent/dsr_agent_pb2.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/dsr_agent/dsr_agent_pb2.pyi
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/dsr_agent/dsr_agent_pb2_grpc.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/dsr_agent/grpc_agent.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/dsr_agent/http_agent.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/dsr_agent/logger.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/dsr_agent/message_package.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/dsr_agent/protos/dsr_agent.proto
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/LICENSE
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/README.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dsr_agent-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/dsr_agent/__init__.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/dsr_agent/dsr_agent_pb2.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/dsr_agent/dsr_agent_pb2.pyi
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/dsr_agent/dsr_agent_pb2_grpc.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/dsr_agent/grpc_agent.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/dsr_agent/http_agent.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/dsr_agent/logger.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/dsr_agent/message_package.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/dsr_agent/protos/dsr_agent.proto
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/LICENSE
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/README.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 dsr_agent-0.0.4/PKG-INFO
```

### Comparing `dsr_agent-0.0.3/dsr_agent/dsr_agent_pb2.py` & `dsr_agent-0.0.4/dsr_agent/dsr_agent_pb2.py`

 * *Files identical despite different names*

### Comparing `dsr_agent-0.0.3/dsr_agent/dsr_agent_pb2.pyi` & `dsr_agent-0.0.4/dsr_agent/dsr_agent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dsr_agent-0.0.3/dsr_agent/dsr_agent_pb2_grpc.py` & `dsr_agent-0.0.4/dsr_agent/dsr_agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dsr_agent-0.0.3/dsr_agent/grpc_agent.py` & `dsr_agent-0.0.4/dsr_agent/grpc_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from multiprocessing import Process
 from multiprocessing.pool import ThreadPool
 import threading
 import time
 import grpc
-from message_package import MessagePackage
-from http_agent import AppType
-from logger import logger
+from dsr_agent import dsr_agent_pb2_grpc
+from dsr_agent.message_package import MessagePackage
+from dsr_agent.http_agent import AppType
+from dsr_agent.logger import logger
 from datetime import datetime, timedelta
-import dsr_agent_pb2_grpc
 
 class GRPCAgent:
 	def __init__(
 		self: AppType,
 		*,
 		agent_id: str = "dataspire-agent",
 		agent_name: str = "DataSpire Agent",
```

### Comparing `dsr_agent-0.0.3/dsr_agent/http_agent.py` & `dsr_agent-0.0.4/dsr_agent/http_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime, timedelta
 import json
 import threading
 from typing import TypeVar
-from logger import logger
+from dsr_agent.logger import logger
 import requests
 
-from message_package import MessagePackage
+from dsr_agent.message_package import MessagePackage
 
 AppType = TypeVar("AppType")
 
 class HttpAgent:
 	def __init__(
 		self: AppType,
 		*,
```

### Comparing `dsr_agent-0.0.3/dsr_agent/message_package.py` & `dsr_agent-0.0.4/dsr_agent/message_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import time
 from datetime import datetime
-from dsr_agent_pb2 import GRPCMessagePackage
+from dsr_agent.dsr_agent_pb2 import GRPCMessagePackage
 
 class MessagePackage:
 	def __init__(
 		self,
 		agent: str  = "DataSpire",
 		agent_id: str = "dataspire-agent",
 		deadline: datetime = datetime.now()
```

### Comparing `dsr_agent-0.0.3/dsr_agent/protos/dsr_agent.proto` & `dsr_agent-0.0.4/dsr_agent/protos/dsr_agent.proto`

 * *Files identical despite different names*

### Comparing `dsr_agent-0.0.3/LICENSE` & `dsr_agent-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dsr_agent-0.0.3/pyproject.toml` & `dsr_agent-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dsr_agent"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="An Quach", email="anquach.dev@gmail.com" },
 ]
 description = "A agent helper support send data out the service"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dsr_agent-0.0.3/PKG-INFO` & `dsr_agent-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dsr_agent
-Version: 0.0.3
+Version: 0.0.4
 Summary: A agent helper support send data out the service
 Project-URL: Homepage, https://anquach.dev
 Project-URL: Bug Tracker, https://github.com/anthoai97/dsr_python_agent
 Author-email: An Quach <anquach.dev@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-# Generate gRPC code
+## Generate gRPC code
 ```
 python -m grpc_tools.protoc -I./protos --python_out=. --pyi_out=. --grpc_python_out=. ./protos/dsr_agent.proto
-```
+```
```

