# Comparing `tmp/yter-3.0.1.tar.gz` & `tmp/yter-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yter-3.0.1.tar", last modified: Sat Jun 24 02:29:29 2023, max compression
+gzip compressed data, was "yter-3.1.0.tar", last modified: Sun Jun 25 06:08:50 2023, max compression
```

## Comparing `yter-3.0.1.tar` & `yter-3.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 02:29:29.763522 yter-3.0.1/
--rw-rw-rw-   0        0        0     1081 2023-03-09 15:02:41.000000 yter-3.0.1/LICENSE
--rw-rw-rw-   0        0        0       18 2023-03-09 15:02:41.000000 yter-3.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2567 2023-06-24 02:29:29.762514 yter-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1921 2023-06-24 02:28:36.000000 yter-3.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 02:29:29.763522 yter-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      926 2023-03-09 15:02:41.000000 yter-3.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:29:29.742767 yter-3.0.1/test/
--rw-rw-rw-   0        0        0     3893 2023-05-29 14:39:48.000000 yter-3.0.1/test/test_fun.py
--rw-rw-rw-   0        0        0     1287 2023-06-14 05:23:52.000000 yter-3.0.1/test/test_key.py
--rw-rw-rw-   0        0        0      158 2023-03-09 15:02:41.000000 yter-3.0.1/test/test_star.py
--rw-rw-rw-   0        0        0     2142 2023-06-22 03:20:01.000000 yter-3.0.1/test/test_ytr.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:29:29.748007 yter-3.0.1/yter/
--rw-rw-rw-   0        0        0      419 2023-06-14 05:20:37.000000 yter-3.0.1/yter/__init__.py
--rw-rw-rw-   0        0        0    11952 2023-06-22 02:44:16.000000 yter-3.0.1/yter/_fun.py
--rw-rw-rw-   0        0        0     4692 2023-06-22 02:46:02.000000 yter-3.0.1/yter/_key.py
--rw-rw-rw-   0        0        0     7960 2023-06-24 02:26:42.000000 yter-3.0.1/yter/_ytr.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:29:29.762008 yter-3.0.1/yter.egg-info/
--rw-rw-rw-   0        0        0     2567 2023-06-24 02:29:29.000000 yter-3.0.1/yter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-24 02:29:29.000000 yter-3.0.1/yter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 02:29:29.000000 yter-3.0.1/yter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-24 02:29:29.000000 yter-3.0.1/yter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 15:10:32.000000 yter-3.0.1/yter.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-25 06:08:50.558651 yter-3.1.0/
+-rw-rw-rw-   0        0        0     1081 2023-03-09 15:02:41.000000 yter-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-03-09 15:02:41.000000 yter-3.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2566 2023-06-25 06:08:50.557642 yter-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1920 2023-06-25 05:48:44.000000 yter-3.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 06:08:50.558651 yter-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      926 2023-03-09 15:02:41.000000 yter-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:08:50.497688 yter-3.1.0/test/
+-rw-rw-rw-   0        0        0     3893 2023-05-29 14:39:48.000000 yter-3.1.0/test/test_fun.py
+-rw-rw-rw-   0        0        0     1287 2023-06-14 05:23:52.000000 yter-3.1.0/test/test_key.py
+-rw-rw-rw-   0        0        0      158 2023-03-09 15:02:41.000000 yter-3.1.0/test/test_star.py
+-rw-rw-rw-   0        0        0     2406 2023-06-25 06:01:16.000000 yter-3.1.0/test/test_ytr.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:08:50.538052 yter-3.1.0/yter/
+-rw-rw-rw-   0        0        0      434 2023-06-25 06:06:04.000000 yter-3.1.0/yter/__init__.py
+-rw-rw-rw-   0        0        0    11952 2023-06-22 02:44:16.000000 yter-3.1.0/yter/_fun.py
+-rw-rw-rw-   0        0        0     4846 2023-06-25 06:04:23.000000 yter-3.1.0/yter/_key.py
+-rw-rw-rw-   0        0        0     8539 2023-06-25 05:53:26.000000 yter-3.1.0/yter/_ytr.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:08:50.555649 yter-3.1.0/yter.egg-info/
+-rw-rw-rw-   0        0        0     2566 2023-06-25 06:08:50.000000 yter-3.1.0/yter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-25 06:08:50.000000 yter-3.1.0/yter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 06:08:50.000000 yter-3.1.0/yter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-25 06:08:50.000000 yter-3.1.0/yter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 15:10:32.000000 yter-3.1.0/yter.egg-info/zip-safe
```

### Comparing `yter-3.0.1/LICENSE` & `yter-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yter-3.0.1/PKG-INFO` & `yter-3.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yter
-Version: 3.0.1
+Version: 3.1.0
 Summary: Clever, quick iterators that make your smile whiter
 Home-page: https://gitlab.com/shredwheat/yter
 Author: Peter Shinners
 Author-email: pete@shinners.org
 License: MIT
 Keywords: iterator itertools
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 # yter
 
-Version 3.0.1`
+Version 3.1.0
 2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
 This will work with versions of Python 2.6+ and 3.2+.
```

### Comparing `yter-3.0.1/README.md` & `yter-3.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # yter
 
-Version 3.0.1`
+Version 3.1.0
 2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
 This will work with versions of Python 2.6+ and 3.2+.
```

### Comparing `yter-3.0.1/setup.py` & `yter-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `yter-3.0.1/test/test_fun.py` & `yter-3.1.0/test/test_fun.py`

 * *Files identical despite different names*

### Comparing `yter-3.0.1/test/test_key.py` & `yter-3.1.0/test/test_key.py`

 * *Files identical despite different names*

### Comparing `yter-3.0.1/test/test_ytr.py` & `yter-3.1.0/test/test_ytr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import itertools
 import yter
+import pytest
 
 
 def test_call():
     assert tuple(yter.call((0, 1, lambda: 2))) == (0, 1, 2)
     assert tuple(yter.call(())) == ()
 
 
@@ -66,8 +67,14 @@
        "alice": ["bob", "terry"], 
        "bob": ["edward", "dave"],
        "dave": ["alice", "bob"],
        "edward": ["dave", "alice"],
        "gary": ["dave", "bob"],
     }
     data = list(yter.recurse(["alice"], friends.get))
-    assert data == ['alice', 'bob', 'terry', 'edward', 'dave']
+    assert data == ['alice', 'bob', 'terry', 'edward', 'dave']
+
+    data = list(yter.recurse(["alice"], friends.__getitem__, filter=friends.__contains__))
+    assert data == ['alice', 'bob', 'terry', 'edward', 'dave']
+
+    with pytest.raises(KeyError):
+        list(yter.recurse(["alice"], friends.__getitem__))
```

### Comparing `yter-3.0.1/yter/_fun.py` & `yter-3.1.0/yter/_fun.py`

 * *Files identical despite different names*

### Comparing `yter-3.0.1/yter/_key.py` & `yter-3.1.0/yter/_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 import re
 import operator
 
 
 def format(fmt, **kwargs):
     """Create a function that formats given values into strings.
 
+    This is similar to converting each value into a string, but is more
+    convenient to define a function that will do more advanced formattting.
+    
     Additional keywoard arguments can be given that will also be passed to the
     format function.
 
     The value passed to the function will be given as the first argument to
     format, which is referenced as {0}.
 
     # Examples
 
     >>> pct = yter.format("{:!<5.0%} odds")
     >>> list(pct(v) for v in (.25, .5, 1))
     ['25%!! odds', '50%!! odds', '100%! odds']
+
     >>> renamer = yter.format("{0.stem}.{ext}, ext="py")
     >>> {p: renamer(p) for p in paths}
 
     """
     def formatted(val):
         return fmt.format(val, **kwargs)
     return formatted
```

### Comparing `yter-3.0.1/yter/_ytr.py` & `yter-3.1.0/yter/_ytr.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,46 +250,59 @@
         for val in y:
             if val not in seen:
                 seenadd(val)
             else:
                 yield val
 
 
-def recurse(y, call):
+def recurse(y, call, filter=None):
     """Recurse values from a callable.
     
     Iterate a breadth first recursion using the given callable and an
     initial iterator of values. The callable is expected to return its
     own iterable of children or None, while taking an argument of a single
     item from the iterators.
 
     This will ensure only unique values are iterated, which avoids typical
     infinite recursion problems with recursive data structures.
 
+    The `filt` argument is an optional callable that will be called with
+    each value. Values generated by the callable will only be recursed
+    when the filter returns True. The filter will also be called on the
+    initial iterator argument.
+    
     # Examples
 
     >>> friends = {
     ...    "alice": ["bob", "terry"], 
     ...    "bob": ["edward", "dave"],
     ...    "dave": ["alice", "bob"],
     ...    "edward": ["dave", "alice"],
     ...    "gary": ["dave", "bob"],
     ... }
     >>> list(yter.recurse(["alice"], friends.get))
     ['alice', 'bob', 'terry', 'edward', 'dave']
 
+    >>> entries = os.scandir(".")
+    >>> def ispath(e): return e.is_dir() and not e.name.startswith(".")
+    >>> for entry in yter.recurse(entries, os.scandir, filter=ispath):
+    ...    if entry.name.endswith(".py"):
+    ...        print(entry.path)
+
     # Implementation notes
 
     The callable results are treated as an iterator and will not be
     iterated until the caller reaches that data.
 
     This does not use function recursion, which avoids Python's typical
     stack limits encountered with deep data structures.
     
     """
     iters = [iter(y)] # Will iterate while modifying this list
     recursion = itertools.chain.from_iterable(iters)
     for item in unique(recursion):
         yield item
+        if filter and not filter(item):
+            continue
         kids = call(item)
         if kids:
             iters.append(kids)
```

### Comparing `yter-3.0.1/yter.egg-info/PKG-INFO` & `yter-3.1.0/yter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yter
-Version: 3.0.1
+Version: 3.1.0
 Summary: Clever, quick iterators that make your smile whiter
 Home-page: https://gitlab.com/shredwheat/yter
 Author: Peter Shinners
 Author-email: pete@shinners.org
 License: MIT
 Keywords: iterator itertools
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 # yter
 
-Version 3.0.1`
+Version 3.1.0
 2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
 This will work with versions of Python 2.6+ and 3.2+.
```

