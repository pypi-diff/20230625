# Comparing `tmp/uuid05-0.0.2.tar.gz` & `tmp/uuid05-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uuid05-0.0.2.tar", last modified: Fri Jun 23 18:58:03 2023, max compression
+gzip compressed data, was "uuid05-0.0.3.tar", last modified: Sun Jun 25 05:47:04 2023, max compression
```

## Comparing `uuid05-0.0.2.tar` & `uuid05-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 18:58:03.075288 uuid05-0.0.2/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1097 2023-06-23 18:04:54.000000 uuid05-0.0.2/LICENSE
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4549 2023-06-23 18:58:03.071288 uuid05-0.0.2/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4174 2023-06-23 18:57:50.000000 uuid05-0.0.2/README.md
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 18:58:03.071288 uuid05-0.0.2/cli/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1075 2023-06-23 18:57:50.000000 uuid05-0.0.2/cli/uuid05
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-06-23 18:58:03.075288 uuid05-0.0.2/setup.cfg
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      569 2023-06-23 18:57:50.000000 uuid05-0.0.2/setup.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 18:58:03.071288 uuid05-0.0.2/uuid05/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     3325 2023-06-23 18:57:50.000000 uuid05-0.0.2/uuid05/__init__.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 18:58:03.071288 uuid05-0.0.2/uuid05.egg-info/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4549 2023-06-23 18:58:03.000000 uuid05-0.0.2/uuid05.egg-info/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      176 2023-06-23 18:58:03.000000 uuid05-0.0.2/uuid05.egg-info/SOURCES.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-06-23 18:58:03.000000 uuid05-0.0.2/uuid05.egg-info/dependency_links.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        7 2023-06-23 18:58:03.000000 uuid05-0.0.2/uuid05.egg-info/top_level.txt
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 05:47:04.127478 uuid05-0.0.3/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1097 2023-06-23 16:59:40.000000 uuid05-0.0.3/LICENSE
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5110 2023-06-25 05:47:04.127478 uuid05-0.0.3/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4735 2023-06-25 05:44:07.000000 uuid05-0.0.3/README.md
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 05:47:04.127478 uuid05-0.0.3/cli/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1246 2023-06-25 05:45:22.000000 uuid05-0.0.3/cli/uuid05
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-06-25 05:47:04.127478 uuid05-0.0.3/setup.cfg
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      569 2023-06-25 05:42:31.000000 uuid05-0.0.3/setup.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 05:47:04.127478 uuid05-0.0.3/uuid05/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3644 2023-06-25 05:44:00.000000 uuid05-0.0.3/uuid05/__init__.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 05:47:04.127478 uuid05-0.0.3/uuid05.egg-info/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5110 2023-06-25 05:47:04.000000 uuid05-0.0.3/uuid05.egg-info/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      176 2023-06-25 05:47:04.000000 uuid05-0.0.3/uuid05.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-06-25 05:47:04.000000 uuid05-0.0.3/uuid05.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        7 2023-06-25 05:47:04.000000 uuid05-0.0.3/uuid05.egg-info/top_level.txt
```

### Comparing `uuid05-0.0.2/LICENSE` & `uuid05-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uuid05-0.0.2/PKG-INFO` & `uuid05-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: uuid05
-Version: 0.0.2
-Summary: Compact human-readable almost unique identifiers for temporary objects in small non-synchronizing distributed systems.
-Home-page: https://github.com/strizhechenko/uuid05
-Author: Oleg Strizhechenko
-Author-email: oleg.strizhechenko@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 **UUID05** - compact human-readable almost unique identifiers for temporary objects
 in small non-synchronizing distributed systems.
 
 Well, it's not really unique (that's why 0.5) and collisions are possible
 but probability is low and it's probably acceptable.
 
 The library have zero dependencies and provides you with a class: `UUID05` based on `int` with two additional methods:
@@ -44,19 +33,33 @@
 ```
 
 ## Using
 
 ``` python
 from uuid05 import UUID05
 
-# May be parametrized by workers: int, ttl: int, precision: int
-# defaults are: workers=10, ttl=2 days, precision=1
+# basic usage
 uid = UUID05.make()
 suffix: str = uid.as_b64()
 object_name: str = f'autotest_object_{suffix}'
+
+# .make() may be parametrized by workers: int, ttl: int, precision: int
+# defaults are: workers=10, ttl=2 days, precision=1
+uid: int = UUID05.make(workers=16, ttl=86400, precision=6)  # 1419554951415
+uid.as_b64()  # 'AUqEXzNy'
+
+# you may also want to just shorten your existing integer identifiers.
+suffix: str = UUID05(123123123123).as_b64()
+assert suffix == 'HKq1w7M'
+
+# How to get maximum UUID value/length with given params?
+max_value = UUID05.max_value(machines=16, ttl=86400, precision=6)  # 1586399913600
+len(str(max_value)) == 13
+len(max_value.as_b64()) == 8  # AXFczaaA
+len(f'autotest_object_{max_value.as_b64()}') == 23  # autotest_object_AXFczaaA
 ```
 
 It can be also used as an utility from command-line:
 
 ``` shell
 $ uuid05
 61503153
@@ -90,15 +93,16 @@
 
 ## When UUID05 is useless
 
 - If your system isn't distributed. Local counter in memory or file will work better.
 - If your objects are persistent - you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid). 
 - If you need to generate multiple UIDs for multiple object really _quick_:
   - generate one and reuse it, using a semantic or loop variable as a suffix;
-  - pass **precision** argument to `uuid05()`. It scales automatically with worker count, but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
+  - pass **precision** argument to `uuid05()`. It scales automatically with worker count,
+    but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
     - `precision=3` argument will use milliseconds.
     - `precision=6` for microseconds.
   - if `precision=6` is not enough stop trying to make your identifier compact.
 - If you believe that semi-persistent data is a testing antipattern,
   and it should be cleared by testing system before or after each run.
 
 ## Development
```

### Comparing `uuid05-0.0.2/README.md` & `uuid05-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: uuid05
+Version: 0.0.3
+Summary: Compact human-readable almost unique identifiers for temporary objects in small non-synchronizing distributed systems.
+Home-page: https://github.com/strizhechenko/uuid05
+Author: Oleg Strizhechenko
+Author-email: oleg.strizhechenko@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 **UUID05** - compact human-readable almost unique identifiers for temporary objects
 in small non-synchronizing distributed systems.
 
 Well, it's not really unique (that's why 0.5) and collisions are possible
 but probability is low and it's probably acceptable.
 
 The library have zero dependencies and provides you with a class: `UUID05` based on `int` with two additional methods:
@@ -33,19 +44,33 @@
 ```
 
 ## Using
 
 ``` python
 from uuid05 import UUID05
 
-# May be parametrized by workers: int, ttl: int, precision: int
-# defaults are: workers=10, ttl=2 days, precision=1
+# basic usage
 uid = UUID05.make()
 suffix: str = uid.as_b64()
 object_name: str = f'autotest_object_{suffix}'
+
+# .make() may be parametrized by workers: int, ttl: int, precision: int
+# defaults are: workers=10, ttl=2 days, precision=1
+uid: int = UUID05.make(workers=16, ttl=86400, precision=6)  # 1419554951415
+uid.as_b64()  # 'AUqEXzNy'
+
+# you may also want to just shorten your existing integer identifiers.
+suffix: str = UUID05(123123123123).as_b64()
+assert suffix == 'HKq1w7M'
+
+# How to get maximum UUID value/length with given params?
+max_value = UUID05.max_value(machines=16, ttl=86400, precision=6)  # 1586399913600
+len(str(max_value)) == 13
+len(max_value.as_b64()) == 8  # AXFczaaA
+len(f'autotest_object_{max_value.as_b64()}') == 23  # autotest_object_AXFczaaA
 ```
 
 It can be also used as an utility from command-line:
 
 ``` shell
 $ uuid05
 61503153
@@ -79,15 +104,16 @@
 
 ## When UUID05 is useless
 
 - If your system isn't distributed. Local counter in memory or file will work better.
 - If your objects are persistent - you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid). 
 - If you need to generate multiple UIDs for multiple object really _quick_:
   - generate one and reuse it, using a semantic or loop variable as a suffix;
-  - pass **precision** argument to `uuid05()`. It scales automatically with worker count, but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
+  - pass **precision** argument to `uuid05()`. It scales automatically with worker count,
+    but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
     - `precision=3` argument will use milliseconds.
     - `precision=6` for microseconds.
   - if `precision=6` is not enough stop trying to make your identifier compact.
 - If you believe that semi-persistent data is a testing antipattern,
   and it should be cleared by testing system before or after each run.
 
 ## Development
```

### Comparing `uuid05-0.0.2/cli/uuid05` & `uuid05-0.0.3/cli/uuid05`

 * *Files 27% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 def main():
     parser = ArgumentParser()
     parser.add_argument('-w', '--workers', type=int, help='Amount of worker processes.')
     parser.add_argument('-t', '--ttl', type=int, help='How many seconds an object lives before being deleted.')
     parser.add_argument('-p', '--precision', type=int, help='Increase up to 6 if you create objects frequently.')
     parser.add_argument('-b', '--base64', action='store_true', help='Use base64 to compact it event more')
     parser.add_argument('-a', '--altchars', type=str, help='Alternative characters for b64encode')
+    parser.add_argument('-m', '--max-value', action='store_true', help='Return maximum possible value for given params')
     args = parser.parse_args()
     kwargs = {}
     if args.workers:
         kwargs['workers'] = args.workers
     if args.ttl:
         kwargs['ttl'] = args.ttl
     if args.precision:
         kwargs['precision'] = args.precision
-    uid: UUID05 = UUID05.make(**kwargs)
+    uid: UUID05 = UUID05.max_value(**kwargs) if args.max_value else UUID05.make(**kwargs)
     print((uid.as_b64(altchars=args.altchars.encode()) if args.altchars else uid.as_b64()) if args.base64 else uid)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `uuid05-0.0.2/setup.py` & `uuid05-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import setup
 
 setup(
     name='uuid05',
-    version='0.0.2',
+    version='0.0.3',
     packages=['uuid05'],
     url='https://github.com/strizhechenko/uuid05',
     license='MIT',
     author='Oleg Strizhechenko',
     author_email='oleg.strizhechenko@gmail.com',
     description='Compact human-readable almost unique identifiers for temporary objects in '
                 'small non-synchronizing distributed systems.',
```

### Comparing `uuid05-0.0.2/uuid05/__init__.py` & `uuid05-0.0.3/uuid05/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 
 class UUID05(int):
     def as_b64(self, *args, **kwargs) -> str:
         """
         If you're using uuid05 results as strings and want it to be more compact, and being integer or not doesn't matter
         you may use this function to encode it to base64. You can transparently pass arguments of b64encode function here.
         As there's not decoding assumed padding symbols are removed.
-        %timeit b64(uuid05()) - 2.87 µs ± 13.9 ns per loop @ 3.2GHz
+        %timeit UUID05.make().as_b64() - 2.87 µs ± 13.9 ns per loop @ 3.2 GHz
+        %timeit UUID05.make().as_b64() - 1.54 µs ± 5.25 ns per loop @ 3.8 GHz
+        %timeit UUID05(1333).as_b64() - 608 ns ± 2.68 ns per loop (with static UUID (skips generation))
         >>> UUID05(34714).as_b64(altchars=b'_-')
         'h5o'
         >>> UUID05(11402098).as_b64(altchars=b'_-')
         'rfty'
         >>> UUID05(3136979908).as_b64(altchars=b'_-')
         'uvqDxA'
         >>> UUID05(29136919548).as_b64(altchars=b'_-')
@@ -32,15 +34,17 @@
 
     @classmethod
     def make(cls, workers=10, ttl=2 * day, precision=0) -> 'UUID05':
         """
         Compact human-readable unique identifiers for temporary objects in small non-synchronizing distributed systems.
         If your objects are persistent - you'd better use nanoid.
         If you need to generate multiple UIDs for multiple object at once - generate one and use loop variable as suffix.
-        %timeit uuid05() - 2.1 µs ± 2.08 ns per loop @ 3.2GHz
+        %timeit UUID05.make() - 2.1 µs ± 2.08 ns per loop @ 3.2GHz
+        %timeit UUID05.make() - 849 ns ± 1.73 ns per loop @ 3.8GHz
+        %timeit UUID05.make() - 717 ns ± 1.76 ns per loop @ 4.7GHz
         :arg workers - count of hosts in a system;
         :arg ttl - how many seconds a temporary object lives in a system (maximum) before being deleted;
         :arg precision (optional) - you can override (increase) a precision if objects are created frequently (max - 6);
         >>> assert UUID05.make(2, 3600) <= 132400
         >>> assert UUID05.make(10, 3600) <= 932400
         >>> assert UUID05.make(10, 3600, precision=2) <= 9356400
         >>> assert UUID05.make(10, 2 * 86400) <= 91555200
@@ -49,24 +53,24 @@
         """
         precision = min(6, precision or int(workers ** (1 / 4)))
         run_id = worker_id % (workers - 1)
         time_id = int((time() % ttl) * 10 ** precision)
         return UUID05(f'{run_id}{time_id}')
 
     @classmethod
-    def uuid05_max_value(cls, machines=10, ttl=2 * day, precision=0) -> 'UUID05':
+    def max_value(cls, workers=10, ttl=2 * day, precision=0) -> 'UUID05':
         """:returns - maximum value of an uuid05 with given params"""
-        precision = min(precision or int(machines ** (1 / 4)), 6)
-        run_id = machines - 1
+        precision = min(precision or int(workers ** (1 / 4)), 6)
+        run_id = workers - 1
         time_id = ttl * ((10 ** precision) - 1)
         return UUID05(f'{run_id}{time_id}')
 
 
 if __name__ == '__main__':
     from random import randint
     for _ttl in 3600, 2 * 86400:
         for _workers in 2, 4, 10, 16, 32, 256:
             worker_id = randint(0, _workers)
             example_value = UUID05.make(_workers, _ttl)
-            max_value = UUID05.uuid05_max_value(_workers, _ttl)
+            max_value = UUID05.max_value(_workers, _ttl)
             max_in_b64 = max_value.as_b64(altchars=b'-_')
             print(f'| {_ttl} | {_workers} | {worker_id} | {example_value} | {max_value} | {max_in_b64} |')
```

### Comparing `uuid05-0.0.2/uuid05.egg-info/PKG-INFO` & `uuid05-0.0.3/uuid05.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uuid05
-Version: 0.0.2
+Version: 0.0.3
 Summary: Compact human-readable almost unique identifiers for temporary objects in small non-synchronizing distributed systems.
 Home-page: https://github.com/strizhechenko/uuid05
 Author: Oleg Strizhechenko
 Author-email: oleg.strizhechenko@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -44,19 +44,33 @@
 ```
 
 ## Using
 
 ``` python
 from uuid05 import UUID05
 
-# May be parametrized by workers: int, ttl: int, precision: int
-# defaults are: workers=10, ttl=2 days, precision=1
+# basic usage
 uid = UUID05.make()
 suffix: str = uid.as_b64()
 object_name: str = f'autotest_object_{suffix}'
+
+# .make() may be parametrized by workers: int, ttl: int, precision: int
+# defaults are: workers=10, ttl=2 days, precision=1
+uid: int = UUID05.make(workers=16, ttl=86400, precision=6)  # 1419554951415
+uid.as_b64()  # 'AUqEXzNy'
+
+# you may also want to just shorten your existing integer identifiers.
+suffix: str = UUID05(123123123123).as_b64()
+assert suffix == 'HKq1w7M'
+
+# How to get maximum UUID value/length with given params?
+max_value = UUID05.max_value(machines=16, ttl=86400, precision=6)  # 1586399913600
+len(str(max_value)) == 13
+len(max_value.as_b64()) == 8  # AXFczaaA
+len(f'autotest_object_{max_value.as_b64()}') == 23  # autotest_object_AXFczaaA
 ```
 
 It can be also used as an utility from command-line:
 
 ``` shell
 $ uuid05
 61503153
@@ -90,15 +104,16 @@
 
 ## When UUID05 is useless
 
 - If your system isn't distributed. Local counter in memory or file will work better.
 - If your objects are persistent - you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid). 
 - If you need to generate multiple UIDs for multiple object really _quick_:
   - generate one and reuse it, using a semantic or loop variable as a suffix;
-  - pass **precision** argument to `uuid05()`. It scales automatically with worker count, but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
+  - pass **precision** argument to `uuid05()`. It scales automatically with worker count,
+    but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
     - `precision=3` argument will use milliseconds.
     - `precision=6` for microseconds.
   - if `precision=6` is not enough stop trying to make your identifier compact.
 - If you believe that semi-persistent data is a testing antipattern,
   and it should be cleared by testing system before or after each run.
 
 ## Development
```

