# Comparing `tmp/taospy-2.7.8.tar.gz` & `tmp/taospy-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taospy-2.7.8.tar", max compression
+gzip compressed data, was "taospy-2.7.9.tar", max compression
```

## Comparing `taospy-2.7.8.tar` & `taospy-2.7.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2023-06-14 06:15:15.071206 taospy-2.7.8/LICENSE
--rw-r--r--   0        0        0    28015 2023-06-14 06:15:15.071206 taospy-2.7.8/README.md
--rw-r--r--   0        0        0     1268 2023-06-14 06:15:15.075206 taospy-2.7.8/pyproject.toml
--rw-r--r--   0        0        0     1471 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/__init__.py
--rw-r--r--   0        0        0       22 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/_version.py
--rw-r--r--   0        0        0    20562 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/bind.py
--rw-r--r--   0        0        0    50847 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/cinterface.py
--rw-r--r--   0        0        0    10000 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/connection.py
--rw-r--r--   0        0        0     1255 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/constants.py
--rw-r--r--   0        0        0    10333 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/cursor.py
--rw-r--r--   0        0        0     2587 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/error.py
--rw-r--r--   0        0        0    11914 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/field.py
--rw-r--r--   0        0        0     4055 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/field_v3.py
--rw-r--r--   0        0        0      224 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/precision.py
--rw-r--r--   0        0        0     7493 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/result.py
--rw-r--r--   0        0        0      398 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/schemaless.py
--rw-r--r--   0        0        0     3856 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/sqlalchemy.py
--rw-r--r--   0        0        0     2396 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/statement.py
--rw-r--r--   0        0        0      964 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/subscription.py
--rw-r--r--   0        0        0     8014 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/tmq.py
--rw-r--r--   0        0        0     1548 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/utils.py
--rw-r--r--   0        0        0     1802 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/__init__.py
--rw-r--r--   0        0        0     4733 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/connection.py
--rw-r--r--   0        0        0     3725 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/cursor.py
--rw-r--r--   0        0        0     1233 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/errors.py
--rw-r--r--   0        0        0     6673 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/restclient.py
--rw-r--r--   0        0        0     2191 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/sqlalchemy.py
--rw-r--r--   0        0        0    30309 1970-01-01 00:00:00.000000 taospy-2.7.8/setup.py
--rw-r--r--   0        0        0    28806 1970-01-01 00:00:00.000000 taospy-2.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-25 02:42:49.191829 taospy-2.7.9/LICENSE
+-rw-r--r--   0        0        0    28015 2023-06-25 02:42:49.191829 taospy-2.7.9/README.md
+-rw-r--r--   0        0        0     1268 2023-06-25 02:42:49.195829 taospy-2.7.9/pyproject.toml
+-rw-r--r--   0        0        0     1471 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/_version.py
+-rw-r--r--   0        0        0    20562 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/bind.py
+-rw-r--r--   0        0        0    54078 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/cinterface.py
+-rw-r--r--   0        0        0    10000 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/connection.py
+-rw-r--r--   0        0        0     1255 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/constants.py
+-rw-r--r--   0        0        0    10333 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/cursor.py
+-rw-r--r--   0        0        0     2587 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/error.py
+-rw-r--r--   0        0        0    11914 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/field.py
+-rw-r--r--   0        0        0     4055 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/field_v3.py
+-rw-r--r--   0        0        0      224 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/precision.py
+-rw-r--r--   0        0        0     7493 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/result.py
+-rw-r--r--   0        0        0      398 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/schemaless.py
+-rw-r--r--   0        0        0     3856 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/sqlalchemy.py
+-rw-r--r--   0        0        0     2396 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/statement.py
+-rw-r--r--   0        0        0      964 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/subscription.py
+-rw-r--r--   0        0        0     9428 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/tmq.py
+-rw-r--r--   0        0        0     1548 2023-06-25 02:42:49.195829 taospy-2.7.9/taos/utils.py
+-rw-r--r--   0        0        0     1802 2023-06-25 02:42:49.195829 taospy-2.7.9/taosrest/__init__.py
+-rw-r--r--   0        0        0     4732 2023-06-25 02:42:49.195829 taospy-2.7.9/taosrest/connection.py
+-rw-r--r--   0        0        0     3725 2023-06-25 02:42:49.195829 taospy-2.7.9/taosrest/cursor.py
+-rw-r--r--   0        0        0     1233 2023-06-25 02:42:49.195829 taospy-2.7.9/taosrest/errors.py
+-rw-r--r--   0        0        0     6673 2023-06-25 02:42:49.195829 taospy-2.7.9/taosrest/restclient.py
+-rw-r--r--   0        0        0     2191 2023-06-25 02:42:49.195829 taospy-2.7.9/taosrest/sqlalchemy.py
+-rw-r--r--   0        0        0    30309 1970-01-01 00:00:00.000000 taospy-2.7.9/setup.py
+-rw-r--r--   0        0        0    28806 1970-01-01 00:00:00.000000 taospy-2.7.9/PKG-INFO
```

### Comparing `taospy-2.7.8/LICENSE` & `taospy-2.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/README.md` & `taospy-2.7.9/README.md`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/pyproject.toml` & `taospy-2.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taospy"
-version = "2.7.8"
+version = "2.7.9"
 description = "TDengine connector for python"
 authors = ["Taosdata Inc. <support@taosdata.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "taos" },
   { include = "taosrest" },
```

### Comparing `taospy-2.7.8/taos/__init__.py` & `taospy-2.7.9/taos/__init__.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/bind.py` & `taospy-2.7.9/taos/bind.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/cinterface.py` & `taospy-2.7.9/taos/cinterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1773,14 +1773,133 @@
 
 
 def tmq_get_res_type(message):
     # type: (c_void_p) -> int
     return _libtaos.tmq_get_res_type(message)
 
 
+class TmqTopicAssignment(Structure):
+    _fields_ = [
+        ("_vg_id", c_int32),
+        ("_current_offset", c_int64),
+        ("_begin", c_int64),
+        ("_end", c_int64),
+    ]
+
+    @property
+    def vg_id(self):
+        return self._vg_id
+
+    @property
+    def current_offset(self):
+        return self._current_offset
+
+    @property
+    def begin(self):
+        return self._begin
+
+    @property
+    def end(self):
+        return self._end
+
+    def __str__(self):
+        return "vg_id: %s, current_offset: %s, begin: %s, end: %s" % (
+            self.vg_id, self.current_offset, self.begin, self.end
+        )
+
+
+class TmqTopicAssignments(Structure):
+
+    def __init__(self, assignments, count):
+        self._assignments = []
+        if isinstance(assignments, c_void_p):
+            self._assignments = cast(assignments, POINTER(TmqTopicAssignment))
+        if isinstance(assignments, POINTER(TmqTopicAssignment)):
+            self._assignments = assignments
+        self._count = count
+        self._iter = 0
+
+    def as_ptr(self):
+        return self._assignments
+
+    @property
+    def count(self):
+        return self._count
+
+    @property
+    def assignments(self):
+        return self._assignments
+
+    def next(self):
+        return self._next()
+
+    def _next(self):
+        if self._iter < self.count:
+            assignment = self._assignments[self._iter]
+            self._iter += 1
+            return assignment
+        else:
+            raise StopIteration
+
+    def __next__(self):
+        return self._next()
+
+    def __getitem__(self, item):
+        return self._assignments[item]
+
+    def __iter__(self):
+        self._iter = 0
+        return self
+
+    def __len__(self):
+        return self._count
+
+
+try:
+    _libtaos.tmq_get_topic_assignment.argstype = (c_void_p, c_char_p, c_void_p, POINTER(c_int))
+    _libtaos.tmq_get_topic_assignment.restype = c_int
+except Exception as err:
+    _UNSUPPORTED["tmq_get_topic_assignment"] = err
+
+
+def tmq_get_topic_assignment(tmq, topic_name):
+    # type: (c_void_p, str) -> List[()]
+
+    _check_if_supported()
+    num_of_assignment = c_int()
+    assignment = c_void_p()
+    assignments = []
+    code = _libtaos.tmq_get_topic_assignment(tmq, c_char_p(topic_name.encode('utf-8')), byref(assignment),
+                                             ctypes.byref(num_of_assignment))
+    if code != 0:
+        raise TmqError(msg="failed on tmq_get_topic_assignment()", errno=code)
+
+    tmq_assignments = TmqTopicAssignments(assignment, num_of_assignment.value)
+
+    for tmq_assignment in tmq_assignments:
+        assignments.append(
+            (tmq_assignment.vg_id, tmq_assignment.current_offset, tmq_assignment.begin, tmq_assignment.end))
+
+    _libtaos.tmq_free_assignment(assignment)
+    return assignments
+
+
+try:
+    _libtaos.tmq_offset_seek.argstype = (c_void_p, c_char_p, c_int32, c_int64)
+    _libtaos.tmq_offset_seek.restype = c_int
+except Exception as err:
+    _UNSUPPORTED["tmq_offset_seek"] = err
+
+
+def tmq_offset_seek(tmq, topic_name, vgroup_id, offset):
+    code = _libtaos.tmq_offset_seek(tmq, c_char_p(topic_name.encode('utf-8')), c_int32(vgroup_id), c_int64(offset))
+    if code != 0:
+        raise TmqError(msg="failed on tmq_offset_seek()", errno=code)
+
+
 class CTaosInterface(object):
     def __init__(self, config=None, tz=None):
         """
         Function to initialize the class
         @host     : str, hostname to connect
         @user     : str, username to connect to server
         @password : str, password to connect to server
```

### Comparing `taospy-2.7.8/taos/connection.py` & `taospy-2.7.9/taos/connection.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/constants.py` & `taospy-2.7.9/taos/constants.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/cursor.py` & `taospy-2.7.9/taos/cursor.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/error.py` & `taospy-2.7.9/taos/error.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/field.py` & `taospy-2.7.9/taos/field.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/field_v3.py` & `taospy-2.7.9/taos/field_v3.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/result.py` & `taospy-2.7.9/taos/result.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/sqlalchemy.py` & `taospy-2.7.9/taos/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/statement.py` & `taospy-2.7.9/taos/statement.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/subscription.py` & `taospy-2.7.9/taos/subscription.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taos/tmq.py` & `taospy-2.7.9/taos/tmq.py`

 * *Files 12% similar despite different names*

```diff
@@ -140,14 +140,25 @@
             return
         taos_free_result(self.msg)
 
     def __iter__(self):
         return iter(self.value())
 
 
+class TopicPartition:
+
+    def __init__(self, topic, partition, offset):
+        self.topic = topic  # type: str
+        self.partition = partition  # type: int
+        self.offset = offset  # type: int
+
+    def __str__(self):
+        return "TopicPartition(topic=%s, partition=%s, offset=%s)" % (self.topic, self.partition, self.offset)
+
+
 class Consumer:
     default_config = {
         'group.id',
         'client.id',
         'msg.with.table.name',
         'enable.auto.commit',
         'auto.commit.interval.ms',
@@ -182,25 +193,33 @@
     def subscribe(self, topics):
         # type ([str]) -> None
         """
         Set subscription to supplied list of topics.
         :param list(str) topics: List of topics (strings) to subscribe to.
         """
         if not topics or len(topics) == 0:
-            raise TmqError('Unset topic for Consumer')
+            raise TmqError("Unset topic for Consumer")
 
-        topic_list = tmq_list_new()
-        for topic in topics:
-            res = tmq_list_append(topic_list, topic)
-            if res != 0:
-                raise TmqError(msg="fail on parse topics", errno=res)
-        tmq_subscribe(self._tmq, topic_list)
+        class TmqListInner:
+            def __init__(self, topics) -> None:
+                self.ptr = tmq_list_new()
+                for topic in topics:
+                    self.append(topic)
+
+            def append(self, item: str):
+                res = tmq_list_append(self.ptr, item)
+                if res != 0:
+                    raise TmqError(msg="fail on parse topics", errno=res)
+
+            def __del__(self):
+                tmq_list_destroy(self.ptr)
 
+        topic_list = TmqListInner(topics)
+        tmq_subscribe(self._tmq, topic_list.ptr)
         self._subscribed = True
-        tmq_list_destroy(topic_list)
 
     def unsubscribe(self):
         """
         Remove current subscription.
         """
         tmq_unsubscribe(self._tmq)
         self._subscribed = False
@@ -222,14 +241,37 @@
             raise TmqError(msg='unsubscribe topic')
 
         msg = tmq_consumer_poll(self._tmq, wait_time=mill_timeout)
         if msg:
             return Message(msg=msg)
         return None
 
+    def assignment(self):
+        """
+        Returns the current partition assignment as a list of TopicPartition tuples.
+        """
+        topics = tmq_subscription(self._tmq)
+        if not topics:
+            return None
+
+        topic_partitions = []
+        for topic in topics:
+            assignments = tmq_get_topic_assignment(self._tmq, topic)
+            for assignment in assignments:
+                topic_partitions.append(
+                    TopicPartition(topic=topic, partition=assignment[0], offset=assignment[1]))
+        return topic_partitions
+
+    def seek(self, partition):
+        # type (TopicPartition) -> None
+        """
+        Set consume position for partition to offset.
+        """
+        tmq_offset_seek(self._tmq, partition.topic, partition.partition, partition.offset)
+
     def close(self):
         """
         Close down and terminate the Kafka Consumer.
         """
         if self._tmq:
             tmq_consumer_close(self._tmq)
             self._tmq = None
```

### Comparing `taospy-2.7.8/taos/utils.py` & `taospy-2.7.9/taos/utils.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taosrest/__init__.py` & `taospy-2.7.9/taosrest/__init__.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taosrest/connection.py` & `taospy-2.7.9/taosrest/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     @property
     def server_info(self):
         resp = self._client.sql("select server_version()")
         if len(resp["data"]) > 0:
             return resp["data"][0][0]
         return ""
 
-    def execute(self, sql: str, req_id: Optional[int] = None) -> Optional[dict]:
+    def execute(self, sql: str, req_id: Optional[int] = None) -> Optional[int]:
         """
         execute none query statement and return affected row count.
         If there is not a column named "affected_rows" in response, then None is returned.
         """
         resp = self._client.sql(sql, req_id=req_id)
         if resp["column_meta"][0][0] == "affected_rows":
             return resp["data"][0][0]
```

### Comparing `taospy-2.7.8/taosrest/cursor.py` & `taospy-2.7.9/taosrest/cursor.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taosrest/errors.py` & `taospy-2.7.9/taosrest/errors.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taosrest/restclient.py` & `taospy-2.7.9/taosrest/restclient.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/taosrest/sqlalchemy.py` & `taospy-2.7.9/taosrest/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.8/setup.py` & `taospy-2.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 entry_points = \
 {'sqlalchemy.dialects': ['taos = taos.sqlalchemy:TaosDialect',
                          'taosrest = taosrest.sqlalchemy:TaosRestDialect',
                          'taosws = taos.sqlalchemy:TaosWsDialect']}
 
 setup_kwargs = {
     'name': 'taospy',
-    'version': '2.7.8',
+    'version': '2.7.9',
     'description': 'TDengine connector for python',
     'long_description': '# TDengine Connector for Python\n\n| Github Workflow | PyPI Version | PyPI Downloads | CodeCov |\n| --------------- | ------------ | -------------- | ------- |\n| ![workflow](https://img.shields.io/github/actions/workflow/status/taosdata/taos-connector-python/test.yml) | ![PyPI](https://img.shields.io/pypi/v/taospy) | ![PyPI](https://img.shields.io/pypi/dm/taospy) | [![codecov](https://codecov.io/gh/taosdata/taos-connector-python/branch/main/graph/badge.svg?token=BDANN3DBXS)](https://codecov.io/gh/taosdata/taos-connector-python) |\n\n\n\n\n[TDengine](https://github.com/taosdata/TDengine) connector for Python enables python programs to access TDengine, using\nan API which is compliant with the Python DB API 2.0 (PEP-249). It contains two modules:\n\n1. The `taos` module. It uses TDengine C client library for client server communications.\n2. The `taosrest` module. It wraps TDengine RESTful API to Python DB API 2.0 (PEP-249). With this module, you do not need to install the TDengine C client library.\n\n## Install taospy\n\nYou can use `pip` to install the connector from PyPI:\n\n```bash\npip install taospy\n```\n\nOr with git url:\n\n```bash\npip install git+https://github.com/taosdata/taos-connector-python.git\n```\n\nNote: taospy v2.7.2 requirs Python 3.6+. The early versions of taospy from v2.5.0 to v2.7.1 require Python 3.7+.\n\n## Source Code\n\n[TDengine](https://github.com/taosdata/TDengine) connector for Python source code is hosted\non [GitHub](https://github.com/taosdata/taos-connector-python).\n\n## Install taos-ws-py\n\n### Install with taospy\n\n```bash\npip install taospy[ws]\n```\n\n### Install taos-ws-py only\n\n```bash\npip install taos-ws-py\n```\n\nNote: The taosws module is provided by taos-ws-py package separately from v2.7.2. It is part of early version of taospy.\ntaos-ws-py requires Python 3.7+.\n\n### Query with PEP-249 API using `taosws`\n\n```python\nimport taosws\n\n# all parameters are optional\nconn = taosws.connect("taosws://root:taosdata@localhost:6041")\ncursor = conn.cursor()\n\ncursor.execute("show databases")\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taosws\n\n# all parameters are optional\nconn = taosws.connect("taosws://root:taosdata@localhost:6041")\ncursor = conn.cursor()\n\ncursor.execute("show databases", req_id=1)\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\n### Query with query method using `taosws`\n\n```python\nfrom taosws import *\n\nconn = connect("taosws://root:taosdata@localhost:6041")\nresult = conn.query("show databases")\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nfrom taosws import *\n\nconn = connect("taosws://root:taosdata@localhost:6041")\nresult = conn.query("show databases", req_id=1)\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\n### Read with Pandas using `taosws`\n\n#### Method one\n\n```python\nimport pandas\nimport taosws\n\nconn = taosws.connect("taosws://root:taosdata@localhost:6041")\ndf: pandas.DataFrame = pandas.read_sql("show databases", conn)\ndf\n```\n\n#### Method Two\n\n```python\nimport pandas\nfrom sqlalchemy import create_engine\n\nengine = create_engine("taosws://root:taosdata@localhost:6041")\ndf: pandas.DataFrame = pandas.read_sql("show databases", engine)\ndf\n```\n\n## Examples for `taosrest` Module\n\n### Query with PEP-249 API\n\n```python\nimport taosrest\n\n# all parameters are optional\nconn = taosrest.connect(url="http://localhost:6041",\n                        user="root",\n                        password="taosdata")\ncursor = conn.cursor()\n\ncursor.execute("show databases")\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taosrest\n\n# all parameters are optional\nconn = taosrest.connect(url="http://localhost:6041",\n                        user="root",\n                        password="taosdata")\ncursor = conn.cursor()\n\ncursor.execute("show databases", req_id=1)\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\n### Query with query method\n\n```python\nfrom taosrest import connect, TaosRestConnection, Result\n\nconn: TaosRestConnection = connect()\nresult: Result = conn.query("show databases")\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nfrom taosrest import connect, TaosRestConnection, Result\n\nconn: TaosRestConnection = connect()\nresult: Result = conn.query("show databases", req_id=1)\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\n### Read with Pandas\n\n#### Method one\n\n```python\nimport pandas\nimport taos\n\nconn = taos.connect()\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", conn)\n```\n\n#### Method two\n\n```python\nimport pandas\nimport taosrest\n\nconn = taosrest.connect()\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", conn)\n```\n\n#### Method three\n\n```python\nimport pandas\nfrom sqlalchemy import create_engine\n\nengine = create_engine("taosrest://root:taosdata@localhost:6041")\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", engine)\n```\n\n## Examples for `taos` Module\n\n### Connect options\n\nSupported config options:\n\n- **config**: TDengine client configuration directory, by default use "/etc/taos/".\n- **host**: TDengine server host, by default use "localhost".\n- **user**: TDengine user name, default is "root".\n- **password**: TDengine user password, default is "taosdata".\n- **database**: Default connection database name, empty if not set.\n- **timezone**: Timezone for timestamp type (which is `datetime` object with tzinfo in python) no matter what the host\'s\n  timezone is.\n\n```python\nimport taos\n\n# 1. with empty options, connect TDengine by default options\n#   that means:\n#     - use /etc/taos/taos.cfg as default configuration file\n#     - use "localhost" if not set in config file\n#     - use "root" as default username\n#     - use "taosdata" as default password\n#     - use 6030 as default port if not set in config file\n#     - use local timezone datetime as timestamp\nconn = taos.connect()\n# 2. with full set options, default db: log, use UTC datetime.\nconn = taos.connect(host=\'localhost\',\n                    user=\'root\',\n                    password=\'taosdata\',\n                    database=\'log\',\n                    config=\'/etc/taos\',\n                    timezone=\'UTC\')\n```\n\nNote that, the datetime formatted string will contain timezone information when timezone set. For example:\n\n```python\n# without timezone(local timezone depends on your machine)\n\'1969-12-31 16:00:00\'\n# with timezone UTC\n\'1969-12-31 16:00:00+00:00\'\n```\n\n### Query with PEP-249 API\n\n```python\nimport taos\n\nconn = taos.connect()\ncursor = conn.cursor()\n\ncursor.execute("show databases")\nresults = cursor.fetchall()\nfor row in results:\n    print(row)\n\ncursor.close()\nconn.close()\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taos\n\nconn = taos.connect()\ncursor = conn.cursor()\n\ncursor.execute("show databases", req_id=1)\nresults = cursor.fetchall()\nfor row in results:\n    print(row)\n\ncursor.close()\nconn.close()\n```\n\n#### Execute many\n\nMethod execute_many is supported:\n\nThere are two ways to use execute_many.\n\nThe first way is to pass a data_set as a list of dictionaries, where each dictionary will be expanded into a complete\nstatement.\n\n```python\nimport taos\n\nconn = taos.connect()\ncursor = conn.cursor()\n\ndb_name = "test_db"\n\ncursor.execute(f"DROP DATABASE IF EXISTS {db_name}")\ncursor.execute(f"CREATE DATABASE {db_name}")\ncursor.execute(f"USE {db_name}")\n\ncursor.execute("create stable stb (ts timestamp, v1 int) tags(t1 int)")\n\ncreate_table_data = [\n    {\n        "name": "tb1",\n        "t1": 1,\n    },\n    {\n        "name": "tb2",\n        "t1": 2,\n    },\n    {\n        "name": "tb3",\n        "t1": 3,\n    }\n]\n\ncursor.execute_many(\n    "create table {name} using stb tags({t1})",\n    create_table_data,\n)\n\n```\n\nThe second way is to pass a data_set as a list of tuples, where each tuple represents a different row of the same\ntable, and each value within the tuple will become a data row in the SQL statement. All the data together will form a\ncomplete SQL statement.\n\n```python\nimport taos\n\nconn = taos.connect()\ncursor = conn.cursor()\n\ndb_name = "test_db"\n\ncursor.execute(f"USE {db_name}")\n\ndata_set = [\n    (\'2018-10-03 14:38:05.100\', 219),\n    (\'2018-10-03 14:38:15.300\', 218),\n    (\'2018-10-03 14:38:16.800\', 221),\n]\n\ntable_name = "tb1"\n\ncursor.execute_many(f"insert into {table_name} values", data_set)\n\n```\n\n[Example: Insert many lines in one execute](./examples/cursor_execute_many.py)\n\n### Query with objective API\n\n```python\nimport taos\n\nconn = taos.connect()\nconn.execute("create database if not exists pytest")\n\nresult = conn.query("show databases")\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n\nresult.close()\nconn.execute("drop database pytest")\nconn.close()\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taos\n\nconn = taos.connect()\nconn.execute("create database if not exists pytest", req_id=1)\n\nresult = conn.query("show databases")\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n\nresult.close()\nconn.execute("drop database pytest")\nconn.close()\n```\n\n### Query with async API\n\n```python\nfrom taos import *\nfrom ctypes import *\nimport time\n\n\ndef fetch_callback(p_param, p_result, num_of_rows):\n    print("fetched ", num_of_rows, "rows")\n    p = cast(p_param, POINTER(Counter))\n    result = TaosResult(p_result)\n\n    if num_of_rows == 0:\n        print("fetching completed")\n        p.contents.done = True\n        result.close()\n        return\n\n    if num_of_rows < 0:\n        p.contents.done = True\n        result.check_error(num_of_rows)\n        result.close()\n        return None\n\n    for row in result.rows_iter(num_of_rows):\n        # print(row)\n        pass\n\n    p.contents.count += result.row_count\n    result.fetch_rows_a(fetch_callback, p_param)\n\n\ndef query_callback(p_param, p_result, code):\n    # type: (c_void_p, c_void_p, c_int) -> None\n    if p_result is None:\n        return\n\n    result = TaosResult(p_result)\n    if code == 0:\n        result.fetch_rows_a(fetch_callback, p_param)\n\n    result.check_error(code)\n\n\nclass Counter(Structure):\n    _fields_ = [("count", c_int), ("done", c_bool)]\n\n    def __str__(self):\n        return "{ count: %d, done: %s }" % (self.count, self.done)\n\n\ndef test_query(conn):\n    # type: (TaosConnection) -> None\n    counter = Counter(count=0)\n    conn.query_a("select * from log.log", query_callback, byref(counter))\n\n    while not counter.done:\n        print("wait query callback")\n        time.sleep(1)\n\n    print(counter)\n    conn.close()\n\n\nif __name__ == "__main__":\n    test_query(connect())\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nfrom taos import *\nfrom ctypes import *\nimport time\n\n\ndef fetch_callback(p_param, p_result, num_of_rows):\n    print("fetched ", num_of_rows, "rows")\n    p = cast(p_param, POINTER(Counter))\n    result = TaosResult(p_result)\n\n    if num_of_rows == 0:\n        print("fetching completed")\n        p.contents.done = True\n        result.close()\n        return\n\n    if num_of_rows < 0:\n        p.contents.done = True\n        result.check_error(num_of_rows)\n        result.close()\n        return None\n\n    for row in result.rows_iter(num_of_rows):\n        # print(row)\n        pass\n\n    p.contents.count += result.row_count\n    result.fetch_rows_a(fetch_callback, p_param)\n\n\ndef query_callback(p_param, p_result, code):\n    # type: (c_void_p, c_void_p, c_int) -> None\n    if p_result is None:\n        return\n\n    result = TaosResult(p_result)\n    if code == 0:\n        result.fetch_rows_a(fetch_callback, p_param)\n\n    result.check_error(code)\n\n\nclass Counter(Structure):\n    _fields_ = [("count", c_int), ("done", c_bool)]\n\n    def __str__(self):\n        return "{ count: %d, done: %s }" % (self.count, self.done)\n\n\ndef test_query(conn):\n    # type: (TaosConnection) -> None\n    counter = Counter(count=0)\n    conn.query_a("select * from log.log", query_callback, byref(counter), req_id=1)\n\n    while not counter.done:\n        print("wait query callback")\n        time.sleep(1)\n\n    print(counter)\n    conn.close()\n\n\nif __name__ == "__main__":\n    test_query(connect())\n```\n\n### Statement API - Bind row after row\n\n```python\nfrom taos import *\n\nconn = connect()\n\ndbname = "pytest_taos_stmt"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s" % dbname)\nconn.select_db(dbname)\n\nconn.execute(\n    "create table if not exists log(ts timestamp, bo bool, nil tinyint, \\\n        ti tinyint, si smallint, ii int, bi bigint, tu tinyint unsigned, \\\n        su smallint unsigned, iu int unsigned, bu bigint unsigned, \\\n        ff float, dd double, bb binary(100), nn nchar(100), tt timestamp)",\n)\n\nstmt = conn.statement("insert into log values(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)")\n\nparams = new_bind_params(16)\nparams[0].timestamp(1626861392589)\nparams[1].bool(True)\nparams[2].tinyint(None)\nparams[3].tinyint(2)\nparams[4].smallint(3)\nparams[5].int(4)\nparams[6].bigint(5)\nparams[7].tinyint_unsigned(6)\nparams[8].smallint_unsigned(7)\nparams[9].int_unsigned(8)\nparams[10].bigint_unsigned(9)\nparams[11].float(10.1)\nparams[12].double(10.11)\nparams[13].binary("hello")\nparams[14].nchar("stmt")\nparams[15].timestamp(1626861392589)\nstmt.bind_param(params)\n\nparams[0].timestamp(1626861392590)\nparams[15].timestamp(None)\nstmt.bind_param(params)\nstmt.execute()\n\nassert stmt.affected_rows == 2\n\nresult = conn.query("select * from log")\n\nfor row in result:\n    print(row)\n```\n\n### Statement API - Bind multi rows\n\n```python\nfrom taos import *\n\nconn = connect()\n\ndbname = "pytest_taos_stmt"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s" % dbname)\nconn.select_db(dbname)\n\nconn.execute(\n    "create table if not exists log(ts timestamp, bo bool, nil tinyint, \\\n        ti tinyint, si smallint, ii int, bi bigint, tu tinyint unsigned, \\\n        su smallint unsigned, iu int unsigned, bu bigint unsigned, \\\n        ff float, dd double, bb binary(100), nn nchar(100), tt timestamp)",\n)\n\nstmt = conn.statement("insert into log values(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)")\n\nparams = new_multi_binds(16)\nparams[0].timestamp((1626861392589, 1626861392590, 1626861392591))\nparams[1].bool((True, None, False))\nparams[2].tinyint([-128, -128, None])  # -128 is tinyint null\nparams[3].tinyint([0, 127, None])\nparams[4].smallint([3, None, 2])\nparams[5].int([3, 4, None])\nparams[6].bigint([3, 4, None])\nparams[7].tinyint_unsigned([3, 4, None])\nparams[8].smallint_unsigned([3, 4, None])\nparams[9].int_unsigned([3, 4, None])\nparams[10].bigint_unsigned([3, 4, None])\nparams[11].float([3, None, 1])\nparams[12].double([3, None, 1.2])\nparams[13].binary(["abc", "dddafadfadfadfadfa", None])\nparams[14].nchar(["涛思数据", None, "a long string with 中文字符"])\nparams[15].timestamp([None, None, 1626861392591])\nstmt.bind_param_batch(params)\nstmt.execute()\n\nassert stmt.affected_rows == 3\n\nresult = conn.query("select * from log")\nfor row in result:\n    print(row)\n```\n\n### Subscription\n\n```python\nimport taos\nimport random\n\nconn = taos.connect()\ndbname = "pytest_taos_subscribe"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s" % dbname)\nconn.select_db(dbname)\nconn.execute("create table if not exists log(ts timestamp, n int)")\nfor i in range(10):\n    conn.execute("insert into log values(now, %d)" % i)\n\nsub = conn.subscribe(False, "test", "select * from log", 1000)\nprint("# consume from begin")\nfor ts, n in sub.consume():\n    print(ts, n)\n\nprint("# consume new data")\nfor i in range(5):\n    conn.execute("insert into log values(now, %d)(now+1s, %d)" % (i, i))\n    result = sub.consume()\n    for ts, n in result:\n        print(ts, n)\n\nsub.close(True)\nprint("# keep progress consume")\nsub = conn.subscribe(False, "test", "select * from log", 1000)\nresult = sub.consume()\nrows = result.fetch_all()\n# consume from latest subscription needs root privilege(for /var/lib/taos).\nassert result.row_count == 0\nprint("## consumed ", len(rows), "rows")\n\nprint("# consume with a stop condition")\nfor i in range(10):\n    conn.execute("insert into log values(now, %d)" % random.randint(0, 10))\n    result = sub.consume()\n    try:\n        ts, n = next(result)\n        print(ts, n)\n        if n > 5:\n            result.stop_query()\n            print("## stopped")\n            break\n    except StopIteration:\n        continue\n\nsub.close()\n# sub.close()\n\nconn.execute("drop database if exists %s" % dbname)\n# conn.close()\n```\n\n### Subscription asynchronously with callback\n\n```python\nfrom taos import *\nfrom ctypes import *\n\nimport time\n\n\ndef subscribe_callback(p_sub, p_result, p_param, errno):\n    # type: (c_void_p, c_void_p, c_void_p, c_int) -> None\n    print("# fetch in callback")\n    result = TaosResult(c_void_p(p_result))\n    result.check_error(errno)\n    for row in result.rows_iter():\n        ts, n = row()\n        print(ts, n)\n\n\ndef test_subscribe_callback(conn):\n    # type: (TaosConnection) -> None\n    dbname = "pytest_taos_subscribe_callback"\n    try:\n        print("drop if exists")\n        conn.execute("drop database if exists %s" % dbname)\n        print("create database")\n        conn.execute("create database if not exists %s" % dbname)\n        print("create table")\n        # conn.execute("use %s" % dbname)\n        conn.execute("create table if not exists %s.log(ts timestamp, n int)" % dbname)\n\n        print("# subscribe with callback")\n        sub = conn.subscribe(False, "test", "select * from %s.log" % dbname, 1000, subscribe_callback)\n\n        for i in range(10):\n            conn.execute("insert into %s.log values(now, %d)" % (dbname, i))\n            time.sleep(0.7)\n\n        sub.close()\n\n        conn.execute("drop database if exists %s" % dbname)\n        # conn.close()\n    except Exception as err:\n        conn.execute("drop database if exists %s" % dbname)\n        # conn.close()\n        raise err\n\n\nif __name__ == "__main__":\n    test_subscribe_callback(connect())\n```\n\n### Insert with line protocol\n\n```python\nimport taos\nfrom taos import SmlProtocol, SmlPrecision\n\nconn = taos.connect()\ndbname = "pytest_line"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s precision \'us\'" % dbname)\nconn.select_db(dbname)\n\nlines = [\n    \'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"pass",c2=false,c4=4f64 1626006833639000000\',\n]\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED)\nprint("inserted")\n\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED)\n\nresult = conn.query("show tables")\nfor row in result:\n    print(row)\n\nconn.execute("drop database if exists %s" % dbname)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taos\nfrom taos import SmlProtocol, SmlPrecision\n\nconn = taos.connect()\ndbname = "pytest_line"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s precision \'us\'" % dbname)\nconn.select_db(dbname)\n\nlines = [\n    \'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"pass",c2=false,c4=4f64 1626006833639000000\',\n]\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED, req_id=1)\nprint("inserted")\n\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED, req_id=2)\n\nresult = conn.query("show tables")\nfor row in result:\n    print(row)\n\nconn.execute("drop database if exists %s" % dbname)\n```\n\nInsert with schemaless raw data.\n\n```python\nimport taos\nfrom taos import utils\nfrom taos import TaosConnection\nfrom taos.cinterface import *\nfrom taos.error import OperationalError, SchemalessError\n\nconn = taos.connect()\ndbname = "taos_schemaless_insert"\ntry:\n    conn.execute("drop database if exists %s" % dbname)\n\n    if taos.IS_V3:\n        conn.execute("create database if not exists %s schemaless 1 precision \'ns\'" % dbname)\n    else:\n        conn.execute("create database if not exists %s update 2 precision \'ns\'" % dbname)\n\n    conn.select_db(dbname)\n\n    lines = \'\'\'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\n    st,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin, abc",c2=true,c4=5f64,c5=5f64,c6=7u64 1626006933640000000\n    stf,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n\n    res = conn.schemaless_insert_raw(lines, 1, 0)\n    print("affected rows: ", res)\n    assert (res == 3)\n\n    lines = \'\'\'stf,t1=5i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n    res = conn.schemaless_insert_raw(lines, 1, 0)\n    print("affected rows: ", res)\n    assert (res == 1)\n\n    result = conn.query("select * from st")\n    dict2 = result.fetch_all_into_dict()\n    print(dict2)\n    print(result.row_count)\n\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n    assert (result.row_count == 2)\n\n    # error test\n    lines = \'\'\',t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\'\'\'\n    try:\n        res = conn.schemaless_insert_raw(lines, 1, 0)\n        print(res)\n        # assert(False)\n    except SchemalessError as err:\n        print(\'**** error: \', err)\n        # assert (err.msg == \'Invalid data format\')\n\n    result = conn.query("select * from st")\n    print(result.row_count)\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\nexcept InterfaceError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept SchemalessError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept Exception as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\n    raise err\n\n```\n\nPass optional ttl in the parameters.\n\n```python\nimport taos\nfrom taos import utils\nfrom taos import TaosConnection\nfrom taos.cinterface import *\nfrom taos.error import OperationalError, SchemalessError\n\nconn = taos.connect()\ndbname = "taos_schemaless_insert"\ntry:\n    conn.execute("drop database if exists %s" % dbname)\n\n    if taos.IS_V3:\n        conn.execute("create database if not exists %s schemaless 1 precision \'ns\'" % dbname)\n    else:\n        conn.execute("create database if not exists %s update 2 precision \'ns\'" % dbname)\n\n    conn.select_db(dbname)\n\n    lines = \'\'\'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\n    st,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin, abc",c2=true,c4=5f64,c5=5f64,c6=7u64 1626006933640000000\n    stf,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n\n    ttl = 1000\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl)\n    print("affected rows: ", res)\n    assert (res == 3)\n\n    lines = \'\'\'stf,t1=5i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n    ttl = 1000\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl)\n    print("affected rows: ", res)\n    assert (res == 1)\n\n    result = conn.query("select * from st")\n    dict2 = result.fetch_all_into_dict()\n    print(dict2)\n    print(result.row_count)\n\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n    assert (result.row_count == 2)\n\n    # error test\n    lines = \'\'\',t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\'\'\'\n    try:\n        ttl = 1000\n        res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl)\n        print(res)\n        # assert(False)\n    except SchemalessError as err:\n        print(\'**** error: \', err)\n        # assert (err.msg == \'Invalid data format\')\n\n    result = conn.query("select * from st")\n    print(result.row_count)\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\nexcept InterfaceError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept Exception as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\n    raise err\n```\n\nPass optional req_id in the parameters.\n\n```python\nimport taos\nfrom taos import utils\nfrom taos import TaosConnection\nfrom taos.cinterface import *\nfrom taos.error import OperationalError, SchemalessError\n\nconn = taos.connect()\ndbname = "taos_schemaless_insert"\ntry:\n    conn.execute("drop database if exists %s" % dbname)\n\n    if taos.IS_V3:\n        conn.execute("create database if not exists %s schemaless 1 precision \'ns\'" % dbname)\n    else:\n        conn.execute("create database if not exists %s update 2 precision \'ns\'" % dbname)\n\n    conn.select_db(dbname)\n\n    lines = \'\'\'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\n    st,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin, abc",c2=true,c4=5f64,c5=5f64,c6=7u64 1626006933640000000\n    stf,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n\n    ttl = 1000\n    req_id = utils.gen_req_id()\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl, req_id=req_id)\n    print("affected rows: ", res)\n    assert (res == 3)\n\n    lines = \'\'\'stf,t1=5i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n    ttl = 1000\n    req_id = utils.gen_req_id()\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl, req_id=req_id)\n    print("affected rows: ", res)\n    assert (res == 1)\n\n    result = conn.query("select * from st")\n    dict2 = result.fetch_all_into_dict()\n    print(dict2)\n    print(result.row_count)\n\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n    assert (result.row_count == 2)\n\n    # error test\n    lines = \'\'\',t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\'\'\'\n    try:\n        ttl = 1000\n        req_id = utils.gen_req_id()\n        res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl, req_id=req_id)\n        print(res)\n        # assert(False)\n    except SchemalessError as err:\n        print(\'**** error: \', err)\n        # assert (err.msg == \'Invalid data format\')\n\n    result = conn.query("select * from st")\n    print(result.row_count)\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\nexcept InterfaceError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept Exception as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\n    raise err\n\n```\n\n### Read with Pandas\n\n#### Method one\n\n```python\nimport pandas\nimport taos\n\nconn = taos.connect()\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", conn)\n```\n\n#### Method Two\n\n```python\nimport pandas\nfrom sqlalchemy import create_engine\n\nengine = create_engine("taos://root:taosdata@localhost:6030/log")\ndf: pandas.DataFrame = pandas.read_sql("select * from logs", engine)\n```\n\n## Limitation\n\n- `taosrest` is designed to use with taosAdapter. If your TDengine version is older than v2.4.0.0, taosAdapter may not\n  be available.\n\n## License\n\nWe use MIT license for Python connector.\n',
     'author': 'Taosdata Inc.',
     'author_email': 'support@taosdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `taospy-2.7.8/PKG-INFO` & `taospy-2.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taospy
-Version: 2.7.8
+Version: 2.7.9
 Summary: TDengine connector for python
 License: MIT
 Author: Taosdata Inc.
 Author-email: support@taosdata.com
 Requires-Python: >=3.6.2,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

