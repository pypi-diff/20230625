# Comparing `tmp/uuid05-0.0.3.tar.gz` & `tmp/uuid05-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uuid05-0.0.3.tar", last modified: Sun Jun 25 05:47:04 2023, max compression
+gzip compressed data, was "uuid05-0.0.4.tar", last modified: Sun Jun 25 15:40:10 2023, max compression
```

## Comparing `uuid05-0.0.3.tar` & `uuid05-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 05:47:04.127478 uuid05-0.0.3/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1097 2023-06-23 16:59:40.000000 uuid05-0.0.3/LICENSE
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     5110 2023-06-25 05:47:04.127478 uuid05-0.0.3/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4735 2023-06-25 05:44:07.000000 uuid05-0.0.3/README.md
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 05:47:04.127478 uuid05-0.0.3/cli/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1246 2023-06-25 05:45:22.000000 uuid05-0.0.3/cli/uuid05
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-06-25 05:47:04.127478 uuid05-0.0.3/setup.cfg
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      569 2023-06-25 05:42:31.000000 uuid05-0.0.3/setup.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 05:47:04.127478 uuid05-0.0.3/uuid05/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     3644 2023-06-25 05:44:00.000000 uuid05-0.0.3/uuid05/__init__.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 05:47:04.127478 uuid05-0.0.3/uuid05.egg-info/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     5110 2023-06-25 05:47:04.000000 uuid05-0.0.3/uuid05.egg-info/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      176 2023-06-25 05:47:04.000000 uuid05-0.0.3/uuid05.egg-info/SOURCES.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-06-25 05:47:04.000000 uuid05-0.0.3/uuid05.egg-info/dependency_links.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        7 2023-06-25 05:47:04.000000 uuid05-0.0.3/uuid05.egg-info/top_level.txt
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 15:40:10.125884 uuid05-0.0.4/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1097 2023-06-23 16:59:40.000000 uuid05-0.0.4/LICENSE
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6650 2023-06-25 15:40:10.125884 uuid05-0.0.4/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6275 2023-06-25 15:39:29.000000 uuid05-0.0.4/README.md
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 15:40:10.125884 uuid05-0.0.4/cli/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1418 2023-06-25 14:24:59.000000 uuid05-0.0.4/cli/uuid05
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-06-25 15:40:10.125884 uuid05-0.0.4/setup.cfg
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      569 2023-06-25 15:09:13.000000 uuid05-0.0.4/setup.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 15:40:10.125884 uuid05-0.0.4/uuid05/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3839 2023-06-25 15:30:02.000000 uuid05-0.0.4/uuid05/__init__.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 15:40:10.125884 uuid05-0.0.4/uuid05.egg-info/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6650 2023-06-25 15:40:10.000000 uuid05-0.0.4/uuid05.egg-info/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      176 2023-06-25 15:40:10.000000 uuid05-0.0.4/uuid05.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-06-25 15:40:10.000000 uuid05-0.0.4/uuid05.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        7 2023-06-25 15:40:10.000000 uuid05-0.0.4/uuid05.egg-info/top_level.txt
```

### Comparing `uuid05-0.0.3/LICENSE` & `uuid05-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uuid05-0.0.3/PKG-INFO` & `uuid05-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: uuid05
-Version: 0.0.3
+Version: 0.0.4
 Summary: Compact human-readable almost unique identifiers for temporary objects in small non-synchronizing distributed systems.
 Home-page: https://github.com/strizhechenko/uuid05
 Author: Oleg Strizhechenko
 Author-email: oleg.strizhechenko@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **UUID05** - compact human-readable almost unique identifiers for temporary objects
-in small non-synchronizing distributed systems.
+in small non-synchronizing distributed systems. Inspired by nanoid and mktemp utility.
 
 Well, it's not really unique (that's why 0.5) and collisions are possible
 but probability is low and it's probably acceptable.
 
-The library have zero dependencies and provides you with a class: `UUID05` based on `int` with two additional methods:
+The library have zero dependencies (well, you need python3 and pip) and provides you with `UUID05` class
+based on `int` with two additional methods:
 
 - `make()` - sort of constructor.
-- `as_b64() -> str` - alternative representation.
+- `as_b64() -> str` - alternative compact representation.
 
 **Examples** below explain how it works:
 
-| TTL <br/>(seconds) | Workers | Worker ID | Example value |     Max value | int2b64(max_value) |
+| TTL <br/>(seconds) | Workers | Worker ID | Example value |     Max value | .as_b64(max_value) |
 |-------------------:|--------:|----------:|--------------:|--------------:|--------------------|
 |        (hour) 3600 |       2 |         1 |          9589 |        132400 | AgUw               |
 |               3600 |       4 |         2 |         29589 |        332400 | BRJw               |
 |               3600 |      10 |         4 |         49589 |        932400 | Djow               |
 |               3600 |      16 |         1 |        195893 |      15356400 | 6lHw               |
 |               3600 |      32 |        11 |       1195893 |      31356400 | Ad518A             |
 |               3600 |     256 |        53 |     539589397 |   25535996400 | BfIQYfA            |
@@ -36,15 +37,15 @@
 |             172800 |      16 |         4 |     414495893 |    1517107200 | Wm04AA             |
 |             172800 |      32 |        14 |    1414495893 |    3117107200 | uctIAA             |
 |             172800 |     256 |       179 | 1791449589397 | 2551727827200 | AlIe1KkA           |
 
 ## Installing
 
 ``` shell
-pip install uuid05
+pip3 install uuid05
 ```
 
 ## Using
 
 ``` python
 from uuid05 import UUID05
 
@@ -90,33 +91,51 @@
 ```
 
 ## Where UUID05 is useful
 
 In E2E/UI-testing. It's slow, and sometimes you need to check a data created by tests _after_ run.
 
 Or, more generally, in staging environments where you aren't sure that your _testing_ system 
-will delete data after runs, but _tested_ system is aware of such a data and deletes it after some time.
+will delete data after runs, but the _tested_ system is aware of such a data and deletes it after some time.
 There's also be multiple testing systems instances running simultaneously, and you don't want them to affect each other.
 
 You also may want identifiers to be more or less rememberable for at least 10-15 seconds while you switching tabs.
 
 Oh, and you _don't_ want to synchronize workers via network.
 Otherwise Redis, Memcached or another database with a single INCRementing counter would do the trick.
 
 ## When UUID05 is useless
 
-- If your system isn't distributed. Local counter in memory or file will work better.
-- If your objects are persistent - you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid). 
+- If your system isn't distributed, local counter in memory or file will work better.
+- If your objects are persistent, you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid).
 - If you need to generate multiple UIDs for multiple object really _quick_:
   - generate one and reuse it, using a semantic or loop variable as a suffix;
+  - well, there's a simple collision preventing mechanism, allowing _small_ "bursts" of loops;
+    - If you seek for performance, disable it (`uuid05.disable_cache = True`) to win ~32% time.
   - pass **precision** argument to `uuid05()`. It scales automatically with worker count,
     but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
     - `precision=3` argument will use milliseconds.
     - `precision=6` for microseconds.
-  - if `precision=6` is not enough stop trying to make your identifier compact.
+  - if `precision=6` is not enough, stop trying to make your identifier compact.
 - If you believe that semi-persistent data is a testing antipattern,
-  and it should be cleared by testing system before or after each run.
+  and it should be cleared by the testing system before or after each run.
+
+## Benchmarks
+
+| Function                | CPU Frequency (GHz) | Collision prevening mechanism enabled | Mean time, ns |
+|:------------------------|--------------------:|---------------------------------------|--------------:|
+| `UUID05.make()`         |              3.8GHz | True                                  |           868 |
+| `UUID05.make()`         |              3.8GHz | False                                 |          1300 |
+| `uuid.uuid4()`          |              3.8GHz | n/a                                   |          1500 |
+| `UUID05.make()`         |              4.7GHz | True                                  |           779 |
+| `UUID05.make()`         |              4.7GHz | False                                 |          1070 |
+| `UUID05(1333).as_b64()` |              3.8GHz | n/a                                   |           596 |
+| `str(uuid.UUID)`        |              3.8GHz | n/a                                   |           570 |
 
 ## Development
 
 - Tests are doctests and may be run by `pytest`.
+- Benchmarks - use `%timeit` in `ipython`
 - Documentation - look at code, it's just two files.
+- Build - `python3 -m build --sdist --wheel`.
+- Release `twine check dist/uuid05-<version>* && twine upload dist/uuid05-<version>*`.
+- Design - `UUID05` class doesn't try to copy `uuid` module methods, properties and behavior. Speed also isn't a goal.
```

### Comparing `uuid05-0.0.3/README.md` & `uuid05-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 **UUID05** - compact human-readable almost unique identifiers for temporary objects
-in small non-synchronizing distributed systems.
+in small non-synchronizing distributed systems. Inspired by nanoid and mktemp utility.
 
 Well, it's not really unique (that's why 0.5) and collisions are possible
 but probability is low and it's probably acceptable.
 
-The library have zero dependencies and provides you with a class: `UUID05` based on `int` with two additional methods:
+The library have zero dependencies (well, you need python3 and pip) and provides you with `UUID05` class
+based on `int` with two additional methods:
 
 - `make()` - sort of constructor.
-- `as_b64() -> str` - alternative representation.
+- `as_b64() -> str` - alternative compact representation.
 
 **Examples** below explain how it works:
 
-| TTL <br/>(seconds) | Workers | Worker ID | Example value |     Max value | int2b64(max_value) |
+| TTL <br/>(seconds) | Workers | Worker ID | Example value |     Max value | .as_b64(max_value) |
 |-------------------:|--------:|----------:|--------------:|--------------:|--------------------|
 |        (hour) 3600 |       2 |         1 |          9589 |        132400 | AgUw               |
 |               3600 |       4 |         2 |         29589 |        332400 | BRJw               |
 |               3600 |      10 |         4 |         49589 |        932400 | Djow               |
 |               3600 |      16 |         1 |        195893 |      15356400 | 6lHw               |
 |               3600 |      32 |        11 |       1195893 |      31356400 | Ad518A             |
 |               3600 |     256 |        53 |     539589397 |   25535996400 | BfIQYfA            |
@@ -25,15 +26,15 @@
 |             172800 |      16 |         4 |     414495893 |    1517107200 | Wm04AA             |
 |             172800 |      32 |        14 |    1414495893 |    3117107200 | uctIAA             |
 |             172800 |     256 |       179 | 1791449589397 | 2551727827200 | AlIe1KkA           |
 
 ## Installing
 
 ``` shell
-pip install uuid05
+pip3 install uuid05
 ```
 
 ## Using
 
 ``` python
 from uuid05 import UUID05
 
@@ -79,33 +80,51 @@
 ```
 
 ## Where UUID05 is useful
 
 In E2E/UI-testing. It's slow, and sometimes you need to check a data created by tests _after_ run.
 
 Or, more generally, in staging environments where you aren't sure that your _testing_ system 
-will delete data after runs, but _tested_ system is aware of such a data and deletes it after some time.
+will delete data after runs, but the _tested_ system is aware of such a data and deletes it after some time.
 There's also be multiple testing systems instances running simultaneously, and you don't want them to affect each other.
 
 You also may want identifiers to be more or less rememberable for at least 10-15 seconds while you switching tabs.
 
 Oh, and you _don't_ want to synchronize workers via network.
 Otherwise Redis, Memcached or another database with a single INCRementing counter would do the trick.
 
 ## When UUID05 is useless
 
-- If your system isn't distributed. Local counter in memory or file will work better.
-- If your objects are persistent - you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid). 
+- If your system isn't distributed, local counter in memory or file will work better.
+- If your objects are persistent, you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid).
 - If you need to generate multiple UIDs for multiple object really _quick_:
   - generate one and reuse it, using a semantic or loop variable as a suffix;
+  - well, there's a simple collision preventing mechanism, allowing _small_ "bursts" of loops;
+    - If you seek for performance, disable it (`uuid05.disable_cache = True`) to win ~32% time.
   - pass **precision** argument to `uuid05()`. It scales automatically with worker count,
     but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
     - `precision=3` argument will use milliseconds.
     - `precision=6` for microseconds.
-  - if `precision=6` is not enough stop trying to make your identifier compact.
+  - if `precision=6` is not enough, stop trying to make your identifier compact.
 - If you believe that semi-persistent data is a testing antipattern,
-  and it should be cleared by testing system before or after each run.
+  and it should be cleared by the testing system before or after each run.
+
+## Benchmarks
+
+| Function                | CPU Frequency (GHz) | Collision prevening mechanism enabled | Mean time, ns |
+|:------------------------|--------------------:|---------------------------------------|--------------:|
+| `UUID05.make()`         |              3.8GHz | True                                  |           868 |
+| `UUID05.make()`         |              3.8GHz | False                                 |          1300 |
+| `uuid.uuid4()`          |              3.8GHz | n/a                                   |          1500 |
+| `UUID05.make()`         |              4.7GHz | True                                  |           779 |
+| `UUID05.make()`         |              4.7GHz | False                                 |          1070 |
+| `UUID05(1333).as_b64()` |              3.8GHz | n/a                                   |           596 |
+| `str(uuid.UUID)`        |              3.8GHz | n/a                                   |           570 |
 
 ## Development
 
 - Tests are doctests and may be run by `pytest`.
+- Benchmarks - use `%timeit` in `ipython`
 - Documentation - look at code, it's just two files.
+- Build - `python3 -m build --sdist --wheel`.
+- Release `twine check dist/uuid05-<version>* && twine upload dist/uuid05-<version>*`.
+- Design - `UUID05` class doesn't try to copy `uuid` module methods, properties and behavior. Speed also isn't a goal.
```

### Comparing `uuid05-0.0.3/cli/uuid05` & `uuid05-0.0.4/cli/uuid05`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 #!/usr/bin/env python3
 
 from argparse import ArgumentParser
 
-from uuid05 import UUID05
+import uuid05
 
 
 def main():
     parser = ArgumentParser()
     parser.add_argument('-w', '--workers', type=int, help='Amount of worker processes.')
+    parser.add_argument('-i', '--worker-id', type=int, help='Identifier of current worker (int)')
     parser.add_argument('-t', '--ttl', type=int, help='How many seconds an object lives before being deleted.')
     parser.add_argument('-p', '--precision', type=int, help='Increase up to 6 if you create objects frequently.')
     parser.add_argument('-b', '--base64', action='store_true', help='Use base64 to compact it event more')
     parser.add_argument('-a', '--altchars', type=str, help='Alternative characters for b64encode')
     parser.add_argument('-m', '--max-value', action='store_true', help='Return maximum possible value for given params')
     args = parser.parse_args()
     kwargs = {}
     if args.workers:
         kwargs['workers'] = args.workers
     if args.ttl:
         kwargs['ttl'] = args.ttl
     if args.precision:
         kwargs['precision'] = args.precision
-    uid: UUID05 = UUID05.max_value(**kwargs) if args.max_value else UUID05.make(**kwargs)
+    if args.worker_id:
+        uuid05.worker_id = args.worker_id
+    uid: uuid05.UUID05 = uuid05.UUID05.max_value(**kwargs) if args.max_value else uuid05.UUID05.make(**kwargs)
     print((uid.as_b64(altchars=args.altchars.encode()) if args.altchars else uid.as_b64()) if args.base64 else uid)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `uuid05-0.0.3/setup.py` & `uuid05-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import setup
 
 setup(
     name='uuid05',
-    version='0.0.3',
+    version='0.0.4',
     packages=['uuid05'],
     url='https://github.com/strizhechenko/uuid05',
     license='MIT',
     author='Oleg Strizhechenko',
     author_email='oleg.strizhechenko@gmail.com',
     description='Compact human-readable almost unique identifiers for temporary objects in '
                 'small non-synchronizing distributed systems.',
```

### Comparing `uuid05-0.0.3/uuid05/__init__.py` & `uuid05-0.0.4/uuid05/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from base64 import b64encode
 from time import time
 import os
 
 day = 86400
+disable_cache = False
+
 
 worker_id = os.getpid()
 if worker_id == 1:  # prevent collisions while running in multiple containers
     import socket
     hostname = socket.gethostname()
     worker_id = ord(hostname[0]) + ord(hostname[-1])
 
 
 class UUID05(int):
+    previous_values = dict()
+
     def as_b64(self, *args, **kwargs) -> str:
         """
-        If you're using uuid05 results as strings and want it to be more compact, and being integer or not doesn't matter
-        you may use this function to encode it to base64. You can transparently pass arguments of b64encode function here.
-        As there's not decoding assumed padding symbols are removed.
-        %timeit UUID05.make().as_b64() - 2.87 µs ± 13.9 ns per loop @ 3.2 GHz
-        %timeit UUID05.make().as_b64() - 1.54 µs ± 5.25 ns per loop @ 3.8 GHz
-        %timeit UUID05(1333).as_b64() - 608 ns ± 2.68 ns per loop (with static UUID (skips generation))
+        If you're using uuid05 results as strings and want it to be more compact, and being integer or not
+        doesn't matter you may use this function to encode it to base64. You can transparently pass
+        arguments of b64encode function here. As there's not decoding assumed padding symbols are removed.
         >>> UUID05(34714).as_b64(altchars=b'_-')
         'h5o'
         >>> UUID05(11402098).as_b64(altchars=b'_-')
         'rfty'
         >>> UUID05(3136979908).as_b64(altchars=b'_-')
         'uvqDxA'
         >>> UUID05(29136919548).as_b64(altchars=b'_-')
@@ -31,34 +32,48 @@
         """
         uid_as_bytes = self.to_bytes((self.bit_length() + 7) // 8, byteorder='big')
         return b64encode(uid_as_bytes, *args, **kwargs).decode().replace('=', '')
 
     @classmethod
     def make(cls, workers=10, ttl=2 * day, precision=0) -> 'UUID05':
         """
-        Compact human-readable unique identifiers for temporary objects in small non-synchronizing distributed systems.
-        If your objects are persistent - you'd better use nanoid.
-        If you need to generate multiple UIDs for multiple object at once - generate one and use loop variable as suffix.
-        %timeit UUID05.make() - 2.1 µs ± 2.08 ns per loop @ 3.2GHz
-        %timeit UUID05.make() - 849 ns ± 1.73 ns per loop @ 3.8GHz
-        %timeit UUID05.make() - 717 ns ± 1.76 ns per loop @ 4.7GHz
         :arg workers - count of hosts in a system;
         :arg ttl - how many seconds a temporary object lives in a system (maximum) before being deleted;
         :arg precision (optional) - you can override (increase) a precision if objects are created frequently (max - 6);
         >>> assert UUID05.make(2, 3600) <= 132400
         >>> assert UUID05.make(10, 3600) <= 932400
         >>> assert UUID05.make(10, 3600, precision=2) <= 9356400
         >>> assert UUID05.make(10, 2 * 86400) <= 91555200
         >>> assert UUID05.make(16, 3600) <= 15356400
         >>> assert UUID05.make(16, 1800) <= 15178200
+        >>> assert UUID05.make() != UUID05.make()
         """
         precision = min(6, precision or int(workers ** (1 / 4)))
         run_id = worker_id % (workers - 1)
-        time_id = int((time() % ttl) * 10 ** precision)
-        return UUID05(f'{run_id}{time_id}')
+        now = time()
+        time_id = int((now % ttl) * 10 ** precision)
+        result = UUID05(f'{run_id}{time_id}')
+
+        if disable_cache:
+            return result
+
+        if (previous := cls.previous_values.get((workers, ttl, precision))) is None:
+            cls.previous_values[(workers, ttl, precision)] = result, now
+            return result
+
+        value, calculated_at = previous
+        # value < result -> enough time passed since .make() was used in for loop
+        # now - calculated_at > ttl / 2 -> such usage is abusing collision preventing mechanism
+        if value < result or now - calculated_at > ttl / 2:
+            cls.previous_values[(workers, ttl, precision)] = result, now
+            return result
+
+        # We're probably called in a cycle. Trying to handle it by incrementing previous value.
+        cls.previous_values[(workers, ttl, precision)] = value + 1, now
+        return cls.previous_values[(workers, ttl, precision)][0]
 
     @classmethod
     def max_value(cls, workers=10, ttl=2 * day, precision=0) -> 'UUID05':
         """:returns - maximum value of an uuid05 with given params"""
         precision = min(precision or int(workers ** (1 / 4)), 6)
         run_id = workers - 1
         time_id = ttl * ((10 ** precision) - 1)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `uuid05-0.0.3/uuid05.egg-info/PKG-INFO` & `uuid05-0.0.4/uuid05.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: uuid05
-Version: 0.0.3
+Version: 0.0.4
 Summary: Compact human-readable almost unique identifiers for temporary objects in small non-synchronizing distributed systems.
 Home-page: https://github.com/strizhechenko/uuid05
 Author: Oleg Strizhechenko
 Author-email: oleg.strizhechenko@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **UUID05** - compact human-readable almost unique identifiers for temporary objects
-in small non-synchronizing distributed systems.
+in small non-synchronizing distributed systems. Inspired by nanoid and mktemp utility.
 
 Well, it's not really unique (that's why 0.5) and collisions are possible
 but probability is low and it's probably acceptable.
 
-The library have zero dependencies and provides you with a class: `UUID05` based on `int` with two additional methods:
+The library have zero dependencies (well, you need python3 and pip) and provides you with `UUID05` class
+based on `int` with two additional methods:
 
 - `make()` - sort of constructor.
-- `as_b64() -> str` - alternative representation.
+- `as_b64() -> str` - alternative compact representation.
 
 **Examples** below explain how it works:
 
-| TTL <br/>(seconds) | Workers | Worker ID | Example value |     Max value | int2b64(max_value) |
+| TTL <br/>(seconds) | Workers | Worker ID | Example value |     Max value | .as_b64(max_value) |
 |-------------------:|--------:|----------:|--------------:|--------------:|--------------------|
 |        (hour) 3600 |       2 |         1 |          9589 |        132400 | AgUw               |
 |               3600 |       4 |         2 |         29589 |        332400 | BRJw               |
 |               3600 |      10 |         4 |         49589 |        932400 | Djow               |
 |               3600 |      16 |         1 |        195893 |      15356400 | 6lHw               |
 |               3600 |      32 |        11 |       1195893 |      31356400 | Ad518A             |
 |               3600 |     256 |        53 |     539589397 |   25535996400 | BfIQYfA            |
@@ -36,15 +37,15 @@
 |             172800 |      16 |         4 |     414495893 |    1517107200 | Wm04AA             |
 |             172800 |      32 |        14 |    1414495893 |    3117107200 | uctIAA             |
 |             172800 |     256 |       179 | 1791449589397 | 2551727827200 | AlIe1KkA           |
 
 ## Installing
 
 ``` shell
-pip install uuid05
+pip3 install uuid05
 ```
 
 ## Using
 
 ``` python
 from uuid05 import UUID05
 
@@ -90,33 +91,51 @@
 ```
 
 ## Where UUID05 is useful
 
 In E2E/UI-testing. It's slow, and sometimes you need to check a data created by tests _after_ run.
 
 Or, more generally, in staging environments where you aren't sure that your _testing_ system 
-will delete data after runs, but _tested_ system is aware of such a data and deletes it after some time.
+will delete data after runs, but the _tested_ system is aware of such a data and deletes it after some time.
 There's also be multiple testing systems instances running simultaneously, and you don't want them to affect each other.
 
 You also may want identifiers to be more or less rememberable for at least 10-15 seconds while you switching tabs.
 
 Oh, and you _don't_ want to synchronize workers via network.
 Otherwise Redis, Memcached or another database with a single INCRementing counter would do the trick.
 
 ## When UUID05 is useless
 
-- If your system isn't distributed. Local counter in memory or file will work better.
-- If your objects are persistent - you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid). 
+- If your system isn't distributed, local counter in memory or file will work better.
+- If your objects are persistent, you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid).
 - If you need to generate multiple UIDs for multiple object really _quick_:
   - generate one and reuse it, using a semantic or loop variable as a suffix;
+  - well, there's a simple collision preventing mechanism, allowing _small_ "bursts" of loops;
+    - If you seek for performance, disable it (`uuid05.disable_cache = True`) to win ~32% time.
   - pass **precision** argument to `uuid05()`. It scales automatically with worker count,
     but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
     - `precision=3` argument will use milliseconds.
     - `precision=6` for microseconds.
-  - if `precision=6` is not enough stop trying to make your identifier compact.
+  - if `precision=6` is not enough, stop trying to make your identifier compact.
 - If you believe that semi-persistent data is a testing antipattern,
-  and it should be cleared by testing system before or after each run.
+  and it should be cleared by the testing system before or after each run.
+
+## Benchmarks
+
+| Function                | CPU Frequency (GHz) | Collision prevening mechanism enabled | Mean time, ns |
+|:------------------------|--------------------:|---------------------------------------|--------------:|
+| `UUID05.make()`         |              3.8GHz | True                                  |           868 |
+| `UUID05.make()`         |              3.8GHz | False                                 |          1300 |
+| `uuid.uuid4()`          |              3.8GHz | n/a                                   |          1500 |
+| `UUID05.make()`         |              4.7GHz | True                                  |           779 |
+| `UUID05.make()`         |              4.7GHz | False                                 |          1070 |
+| `UUID05(1333).as_b64()` |              3.8GHz | n/a                                   |           596 |
+| `str(uuid.UUID)`        |              3.8GHz | n/a                                   |           570 |
 
 ## Development
 
 - Tests are doctests and may be run by `pytest`.
+- Benchmarks - use `%timeit` in `ipython`
 - Documentation - look at code, it's just two files.
+- Build - `python3 -m build --sdist --wheel`.
+- Release `twine check dist/uuid05-<version>* && twine upload dist/uuid05-<version>*`.
+- Design - `UUID05` class doesn't try to copy `uuid` module methods, properties and behavior. Speed also isn't a goal.
```

