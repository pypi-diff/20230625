# Comparing `tmp/scrapy_db-0.0.2.tar.gz` & `tmp/scrapy_db-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_db-0.0.2.tar", max compression
+gzip compressed data, was "scrapy_db-0.0.3.tar", max compression
```

## Comparing `scrapy_db-0.0.2.tar` & `scrapy_db-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-06-07 10:34:22.421846 scrapy_db-0.0.2/LICENSE
--rw-r--r--   0        0        0     1547 2023-06-24 10:48:36.684160 scrapy_db-0.0.2/README.md
--rw-r--r--   0        0        0     1216 2023-06-24 11:35:28.967379 scrapy_db-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      107 2023-06-24 11:35:44.984063 scrapy_db-0.0.2/scrapy_db/__init__.py
--rw-r--r--   0        0        0     5350 2023-06-14 03:38:46.820214 scrapy_db-0.0.2/scrapy_db/db.py
--rw-r--r--   0        0        0      475 2023-06-13 15:04:25.223531 scrapy_db-0.0.2/scrapy_db/defaults.py
--rw-r--r--   0        0        0     3256 2023-06-15 02:02:42.898109 scrapy_db-0.0.2/scrapy_db/dupefilter.py
--rw-r--r--   0        0        0     2473 2023-06-14 03:15:23.908321 scrapy_db-0.0.2/scrapy_db/queue.py
--rw-r--r--   0        0        0     4381 2023-06-13 15:04:25.224164 scrapy_db-0.0.2/scrapy_db/scheduler.py
--rw-r--r--   0        0        0     4705 2023-06-13 15:04:25.224356 scrapy_db-0.0.2/scrapy_db/spiders.py
--rw-r--r--   0        0        0     1089 2023-06-13 15:04:25.224584 scrapy_db-0.0.2/scrapy_db/utils.py
--rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 scrapy_db-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-25 06:43:42.306864 scrapy_db-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1759 2023-06-25 06:43:42.306864 scrapy_db-0.0.3/README.md
+-rw-r--r--   0        0        0     1216 2023-06-25 06:43:42.306864 scrapy_db-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-06-25 06:43:42.306864 scrapy_db-0.0.3/scrapy_db/__init__.py
+-rw-r--r--   0        0        0     5352 2023-06-25 06:43:42.306864 scrapy_db-0.0.3/scrapy_db/db.py
+-rw-r--r--   0        0        0      475 2023-06-25 06:43:42.306864 scrapy_db-0.0.3/scrapy_db/defaults.py
+-rw-r--r--   0        0        0     3258 2023-06-25 06:43:42.306864 scrapy_db-0.0.3/scrapy_db/dupefilter.py
+-rw-r--r--   0        0        0     2490 2023-06-25 06:43:42.306864 scrapy_db-0.0.3/scrapy_db/queue.py
+-rw-r--r--   0        0        0     4381 2023-06-25 06:43:42.306864 scrapy_db-0.0.3/scrapy_db/scheduler.py
+-rw-r--r--   0        0        0     4705 2023-06-25 06:43:42.306864 scrapy_db-0.0.3/scrapy_db/spiders.py
+-rw-r--r--   0        0        0     1089 2023-06-25 06:43:42.306864 scrapy_db-0.0.3/scrapy_db/utils.py
+-rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 scrapy_db-0.0.3/PKG-INFO
```

### Comparing `scrapy_db-0.0.2/LICENSE` & `scrapy_db-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.2/README.md` & `scrapy_db-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -55,7 +55,12 @@
 ## Use
 
 Clone the current project and run the example crawler in example-project to experience it.
 
 ## ❗️Notice
 
 This repository is still under development and may be unstable.
+
+## Why is there this library
+
+Because I have a huge request pool, I don't have that much memory for redis to save it, so, I thought about database, I
+created it with reference to scrapy-redis and it works fine.
```

### Comparing `scrapy_db-0.0.2/pyproject.toml` & `scrapy_db-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapy-db"
-version = "0.0.2"
+version = "0.0.3"
 description = "Similar to [scrapy-redis](https://github.com/rmax/scrapy-redis), using the database as a queue, database-based scrapy components."
 authors = ["libra146 <shumeipai146@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "scrapy_db" }]
 license = "GPL-3.0-only"
 homepage = "https://github.com/libra146/scrapy-db/blob/main/README.md"
 repository = "https://github.com/libra146/scrapy-db"
```

### Comparing `scrapy_db-0.0.2/scrapy_db/db.py` & `scrapy_db-0.0.3/scrapy_db/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,22 +75,22 @@
     attrs_.update(attrs)
     return type(f'{name.capitalize()}Model', (Model,), attrs_)  # noqa
 
 
 # A dictionary that stores the fields of the model class
 _params = {
     'dupelifter': {
-        'key': CharField(),
+        'key_': CharField(),
     },
     'start_url': {
         'start_url': CharField(),
         'deleted': BooleanField(default=False)
     },
     'queue': {
-        'key': CharField(max_length=10000),
+        'key_': CharField(max_length=10000),
         'score': IntegerField(index=True),
         'deleted': BooleanField(default=False)
     }
 }
 
 
 def db_require(fun):
```

### Comparing `scrapy_db-0.0.2/scrapy_db/dupefilter.py` & `scrapy_db-0.0.3/scrapy_db/dupefilter.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         Returns True if the request has already been made
 
         :param request: Request object
         :return: Whether the request has been made
         """
         # request_fingerprint remove warnings
         fp = fingerprint(request).hex()
-        added = self.table.db.select().where(self.table.db.key == fp).count()
-        self.table.push(**{'key': fp})
+        added = self.table.db.select().where(self.table.db.key_ == fp).count()
+        self.table.push(**{'key_': fp})
         return added != 0
 
     @classmethod
     def from_spider(cls, spider):
         """
         Create an instance through spider
```

### Comparing `scrapy_db-0.0.2/scrapy_db/queue.py` & `scrapy_db-0.0.3/scrapy_db/queue.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,43 +48,43 @@
         obj = self.serializer.loads(encoded_request)
         return request_from_dict(obj, spider=self.spider)
 
     def __len__(self):
         return len(self.db)
 
     def push(self, request):
-        self.db.push(**{'key': self._encode_request(request)})
+        self.db.push(**{'key_': self._encode_request(request)})
 
     def pop(self, timeout=0):
         raise NotImplementedError
 
     def clear(self):
         self.db.drop_table()
 
 
 class FifoQueue(Base):
 
     def pop(self, timeout=0):
         result = self.db.pop(timeout, desc=False)
         if result:
-            return self._decode_request(result)
+            return self._decode_request(result.key_)
 
 
 class PriorityQueue(Base):
 
     def push(self, request):
         data = self._encode_request(request)
         score = -request.priority
-        self.db.push(**{'key': data, 'score': score})
+        self.db.push(**{'key_': data, 'score': score})
 
     def pop(self, timeout=0):
         result = self.db.pop_by_score(timeout)
         if result:
-            return self._decode_request(result)
+            return self._decode_request(result.key_)
 
 
 class LifoQueue(Base):
 
     def pop(self, timeout=0):
         result = self.db.pop(timeout)
         if result:
-            return self._decode_request(result)
+            return self._decode_request(result.key_)
```

### Comparing `scrapy_db-0.0.2/scrapy_db/scheduler.py` & `scrapy_db-0.0.3/scrapy_db/scheduler.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.2/scrapy_db/spiders.py` & `scrapy_db-0.0.3/scrapy_db/spiders.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.2/scrapy_db/utils.py` & `scrapy_db-0.0.3/scrapy_db/utils.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.2/PKG-INFO` & `scrapy_db-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-db
-Version: 0.0.2
+Version: 0.0.3
 Summary: Similar to [scrapy-redis](https://github.com/rmax/scrapy-redis), using the database as a queue, database-based scrapy components.
 Home-page: https://github.com/libra146/scrapy-db/blob/main/README.md
 License: GPL-3.0-only
 Author: libra146
 Author-email: shumeipai146@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -80,7 +80,12 @@
 
 Clone the current project and run the example crawler in example-project to experience it.
 
 ## ❗️Notice
 
 This repository is still under development and may be unstable.
 
+## Why is there this library
+
+Because I have a huge request pool, I don't have that much memory for redis to save it, so, I thought about database, I
+created it with reference to scrapy-redis and it works fine.
+
```

