# Comparing `tmp/fppy-0.0.8.tar.gz` & `tmp/fppy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fppy-0.0.8.tar", last modified: Thu Aug 19 16:09:56 2021, max compression
+gzip compressed data, was "fppy-0.0.9.tar", last modified: Tue Feb  8 05:08:44 2022, max compression
```

## Comparing `fppy-0.0.8.tar` & `fppy-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxr-x   0 zshang    (1000) zshang    (1000)        0 2021-08-19 16:09:56.784757 fppy-0.0.8/
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     6859 2021-08-19 16:09:56.784757 fppy-0.0.8/PKG-INFO
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     4810 2021-07-29 13:16:32.000000 fppy-0.0.8/README.md
-drwxrwxr-x   0 zshang    (1000) zshang    (1000)        0 2021-08-19 16:09:56.780758 fppy-0.0.8/fppy.egg-info/
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     6859 2021-08-19 16:09:56.000000 fppy-0.0.8/fppy.egg-info/PKG-INFO
--rw-rw-r--   0 zshang    (1000) zshang    (1000)      942 2021-08-19 16:09:56.000000 fppy-0.0.8/fppy.egg-info/SOURCES.txt
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        1 2021-08-19 16:09:56.000000 fppy-0.0.8/fppy.egg-info/dependency_links.txt
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        9 2021-08-19 16:09:56.000000 fppy-0.0.8/fppy.egg-info/requires.txt
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        4 2021-08-19 16:09:56.000000 fppy-0.0.8/fppy.egg-info/top_level.txt
-drwxrwxr-x   0 zshang    (1000) zshang    (1000)        0 2021-08-19 16:09:56.780758 fppy-0.0.8/fpy/
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        0 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/__init__.py
-drwxrwxr-x   0 zshang    (1000) zshang    (1000)        0 2021-08-19 16:09:56.780758 fppy-0.0.8/fpy/composable/
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        0 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/composable/__init__.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     3295 2021-08-19 16:07:49.000000 fppy-0.0.8/fpy/composable/collections.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)      258 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/composable/composable.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     1937 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/composable/function.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)      366 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/composable/transparent.py
-drwxrwxr-x   0 zshang    (1000) zshang    (1000)        0 2021-08-19 16:09:56.780758 fppy-0.0.8/fpy/control/
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        0 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/control/__init__.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)      633 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/control/applicative.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     1316 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/control/functor.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)      405 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/control/monad.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)      630 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/control/natural_transform.py
-drwxrwxr-x   0 zshang    (1000) zshang    (1000)        0 2021-08-19 16:09:56.780758 fppy-0.0.8/fpy/data/
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        0 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/data/__init__.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     1877 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/data/cont.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     2370 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/data/either.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)      697 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/data/forgetful.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)      512 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/data/function.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     1671 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/data/maybe.py
-drwxrwxr-x   0 zshang    (1000) zshang    (1000)        0 2021-08-19 16:09:56.780758 fppy-0.0.8/fpy/debug/
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        0 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/debug/__init__.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)      385 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/debug/debug.py
-drwxrwxr-x   0 zshang    (1000) zshang    (1000)        0 2021-08-19 16:09:56.780758 fppy-0.0.8/fpy/experimental/
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        0 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/experimental/__init__.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     9899 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/experimental/do.py
-drwxrwxr-x   0 zshang    (1000) zshang    (1000)        0 2021-08-19 16:09:56.780758 fppy-0.0.8/fpy/parsec/
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        0 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/parsec/__init__.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     3610 2021-08-01 03:48:14.000000 fppy-0.0.8/fpy/parsec/parsec.py
-drwxrwxr-x   0 zshang    (1000) zshang    (1000)        0 2021-08-19 16:09:56.784757 fppy-0.0.8/fpy/tests/
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        0 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/tests/__init__.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     2618 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/tests/test_composable.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)      755 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/tests/test_cont.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     2133 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/tests/test_do.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     1838 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/tests/test_either.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)      772 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/tests/test_function.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     1812 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/tests/test_maybe.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     1854 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/tests/test_parsec.py
-drwxrwxr-x   0 zshang    (1000) zshang    (1000)        0 2021-08-19 16:09:56.784757 fppy-0.0.8/fpy/utils/
--rw-rw-r--   0 zshang    (1000) zshang    (1000)        0 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/utils/__init__.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     2399 2021-07-29 13:16:32.000000 fppy-0.0.8/fpy/utils/placeholder.py
--rw-rw-r--   0 zshang    (1000) zshang    (1000)       38 2021-08-19 16:09:56.784757 fppy-0.0.8/setup.cfg
--rw-rw-r--   0 zshang    (1000) zshang    (1000)     1377 2021-08-19 16:09:34.000000 fppy-0.0.8/setup.py
+drwxr-xr-x   0 zshang     (502) staff       (20)        0 2022-02-08 05:08:44.918680 fppy-0.0.9/
+-rw-r--r--   0 zshang     (502) staff       (20)    35149 2022-01-17 01:52:17.000000 fppy-0.0.9/LICENSE.txt
+-rw-r--r--   0 zshang     (502) staff       (20)     5474 2022-02-08 05:08:44.918556 fppy-0.0.9/PKG-INFO
+-rw-r--r--   0 zshang     (502) staff       (20)     4850 2022-02-08 05:07:37.000000 fppy-0.0.9/README.md
+drwxr-xr-x   0 zshang     (502) staff       (20)        0 2022-02-08 05:08:44.914965 fppy-0.0.9/fppy.egg-info/
+-rw-r--r--   0 zshang     (502) staff       (20)     5474 2022-02-08 05:08:44.000000 fppy-0.0.9/fppy.egg-info/PKG-INFO
+-rw-r--r--   0 zshang     (502) staff       (20)      954 2022-02-08 05:08:44.000000 fppy-0.0.9/fppy.egg-info/SOURCES.txt
+-rw-r--r--   0 zshang     (502) staff       (20)        1 2022-02-08 05:08:44.000000 fppy-0.0.9/fppy.egg-info/dependency_links.txt
+-rw-r--r--   0 zshang     (502) staff       (20)        9 2022-02-08 05:08:44.000000 fppy-0.0.9/fppy.egg-info/requires.txt
+-rw-r--r--   0 zshang     (502) staff       (20)        4 2022-02-08 05:08:44.000000 fppy-0.0.9/fppy.egg-info/top_level.txt
+drwxr-xr-x   0 zshang     (502) staff       (20)        0 2022-02-08 05:08:44.915079 fppy-0.0.9/fpy/
+-rw-r--r--   0 zshang     (502) staff       (20)        0 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/__init__.py
+drwxr-xr-x   0 zshang     (502) staff       (20)        0 2022-02-08 05:08:44.915594 fppy-0.0.9/fpy/composable/
+-rw-r--r--   0 zshang     (502) staff       (20)        0 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/composable/__init__.py
+-rw-r--r--   0 zshang     (502) staff       (20)     3295 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/composable/collections.py
+-rw-r--r--   0 zshang     (502) staff       (20)      258 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/composable/composable.py
+-rw-r--r--   0 zshang     (502) staff       (20)     1937 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/composable/function.py
+-rw-r--r--   0 zshang     (502) staff       (20)      366 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/composable/transparent.py
+drwxr-xr-x   0 zshang     (502) staff       (20)        0 2022-02-08 05:08:44.916140 fppy-0.0.9/fpy/control/
+-rw-r--r--   0 zshang     (502) staff       (20)        0 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/control/__init__.py
+-rw-r--r--   0 zshang     (502) staff       (20)      633 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/control/applicative.py
+-rw-r--r--   0 zshang     (502) staff       (20)     1316 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/control/functor.py
+-rw-r--r--   0 zshang     (502) staff       (20)      405 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/control/monad.py
+-rw-r--r--   0 zshang     (502) staff       (20)      630 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/control/natural_transform.py
+drwxr-xr-x   0 zshang     (502) staff       (20)        0 2022-02-08 05:08:44.916792 fppy-0.0.9/fpy/data/
+-rw-r--r--   0 zshang     (502) staff       (20)        0 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/data/__init__.py
+-rw-r--r--   0 zshang     (502) staff       (20)     1877 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/data/cont.py
+-rw-r--r--   0 zshang     (502) staff       (20)     2370 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/data/either.py
+-rw-r--r--   0 zshang     (502) staff       (20)      697 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/data/forgetful.py
+-rw-r--r--   0 zshang     (502) staff       (20)      512 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/data/function.py
+-rw-r--r--   0 zshang     (502) staff       (20)     1671 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/data/maybe.py
+drwxr-xr-x   0 zshang     (502) staff       (20)        0 2022-02-08 05:08:44.916983 fppy-0.0.9/fpy/debug/
+-rw-r--r--   0 zshang     (502) staff       (20)        0 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/debug/__init__.py
+-rw-r--r--   0 zshang     (502) staff       (20)      385 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/debug/debug.py
+drwxr-xr-x   0 zshang     (502) staff       (20)        0 2022-02-08 05:08:44.917176 fppy-0.0.9/fpy/experimental/
+-rw-r--r--   0 zshang     (502) staff       (20)        0 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/experimental/__init__.py
+-rw-r--r--   0 zshang     (502) staff       (20)     9899 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/experimental/do.py
+drwxr-xr-x   0 zshang     (502) staff       (20)        0 2022-02-08 05:08:44.917378 fppy-0.0.9/fpy/parsec/
+-rw-r--r--   0 zshang     (502) staff       (20)        0 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/parsec/__init__.py
+-rw-r--r--   0 zshang     (502) staff       (20)     3758 2022-02-08 05:07:46.000000 fppy-0.0.9/fpy/parsec/parsec.py
+drwxr-xr-x   0 zshang     (502) staff       (20)        0 2022-02-08 05:08:44.918199 fppy-0.0.9/fpy/tests/
+-rw-r--r--   0 zshang     (502) staff       (20)        0 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/tests/__init__.py
+-rw-r--r--   0 zshang     (502) staff       (20)     2618 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/tests/test_composable.py
+-rw-r--r--   0 zshang     (502) staff       (20)      755 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/tests/test_cont.py
+-rw-r--r--   0 zshang     (502) staff       (20)     2133 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/tests/test_do.py
+-rw-r--r--   0 zshang     (502) staff       (20)     1838 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/tests/test_either.py
+-rw-r--r--   0 zshang     (502) staff       (20)      772 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/tests/test_function.py
+-rw-r--r--   0 zshang     (502) staff       (20)     1812 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/tests/test_maybe.py
+-rw-r--r--   0 zshang     (502) staff       (20)     2037 2022-02-08 05:06:43.000000 fppy-0.0.9/fpy/tests/test_parsec.py
+drwxr-xr-x   0 zshang     (502) staff       (20)        0 2022-02-08 05:08:44.918391 fppy-0.0.9/fpy/utils/
+-rw-r--r--   0 zshang     (502) staff       (20)        0 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/utils/__init__.py
+-rw-r--r--   0 zshang     (502) staff       (20)     2399 2022-01-17 01:52:17.000000 fppy-0.0.9/fpy/utils/placeholder.py
+-rw-r--r--   0 zshang     (502) staff       (20)       38 2022-02-08 05:08:44.918722 fppy-0.0.9/setup.cfg
+-rw-r--r--   0 zshang     (502) staff       (20)     1377 2022-02-08 05:07:57.000000 fppy-0.0.9/setup.py
```

### Comparing `fppy-0.0.8/README.md` & `fppy-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -169,13 +169,14 @@
 * `pmaybe :: parser[S, T] -> parser[S, T]`
 * `many :: parser[S, T] -> parser[S, T]`
 * `many1 :: parser[S, T] -> parser[S, T]`
 * `ptrans :: parser[S, T] -> (T -> Y) -> parser[S, Y]`
 * `peek :: parser[S, T] -> parser[S, T]`
 * `skip :: parser[S, T] -> parser[S, T]`
 * `pseq :: [S] -> parser[S, T]`
+* `inv :: parser[S, T] -> parser[S, T]`
 
 ## Dependencies
 * [bytecode](https://github.com/MatthieuDartiailh/bytecode)
 
 ## License
 GPL3+
```

### Comparing `fppy-0.0.8/fppy.egg-info/SOURCES.txt` & `fppy-0.0.9/fppy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.py
 fppy.egg-info/PKG-INFO
 fppy.egg-info/SOURCES.txt
 fppy.egg-info/dependency_links.txt
 fppy.egg-info/requires.txt
 fppy.egg-info/top_level.txt
```

### Comparing `fppy-0.0.8/fpy/composable/collections.py` & `fppy-0.0.9/fpy/composable/collections.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/composable/function.py` & `fppy-0.0.9/fpy/composable/function.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/control/applicative.py` & `fppy-0.0.9/fpy/control/applicative.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/control/functor.py` & `fppy-0.0.9/fpy/control/functor.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/control/natural_transform.py` & `fppy-0.0.9/fpy/control/natural_transform.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/data/cont.py` & `fppy-0.0.9/fpy/data/cont.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/data/either.py` & `fppy-0.0.9/fpy/data/either.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/data/forgetful.py` & `fppy-0.0.9/fpy/data/forgetful.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/data/function.py` & `fppy-0.0.9/fpy/data/function.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/data/maybe.py` & `fppy-0.0.9/fpy/data/maybe.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/experimental/do.py` & `fppy-0.0.9/fpy/experimental/do.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/parsec/parsec.py` & `fppy-0.0.9/fpy/parsec/parsec.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     trans0,
     trans1,
     or_,
     and_,
     set0,
     set1,
     get0,
+    get1,
 )
 
 import string
 from typing import TypeVar, List, Tuple, Callable, Generic
 from dataclasses import dataclass
 import collections.abc as cabc
 
@@ -179,7 +180,16 @@
 def pseq(s):
     if not s:
         return just_nothing
     p = just_nothing
     for e in s:
         p = p + one(__ == e)
     return p
+
+def inv(p):
+    @parser
+    def __inv(s):
+        _r = p(s)
+        if _r:
+            return None
+        return [], s
+    return __inv
```

### Comparing `fppy-0.0.8/fpy/tests/test_composable.py` & `fppy-0.0.9/fpy/tests/test_composable.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/tests/test_cont.py` & `fppy-0.0.9/fpy/tests/test_cont.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/tests/test_do.py` & `fppy-0.0.9/fpy/tests/test_do.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/tests/test_either.py` & `fppy-0.0.9/fpy/tests/test_either.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/tests/test_function.py` & `fppy-0.0.9/fpy/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/tests/test_maybe.py` & `fppy-0.0.9/fpy/tests/test_maybe.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/fpy/tests/test_parsec.py` & `fppy-0.0.9/fpy/tests/test_parsec.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     pmaybe,
     many,
     many1,
     ptrans,
     peek,
     skip,
     pseq,
+    inv,
 )
 from fpy.data.either import fromRight
 
 import unittest
 
 toks = [1, 2, 3]
 
@@ -84,7 +85,14 @@
         self.assertIs(toks, rest)
 
     def testTimeN(self):
         p1 = one(odd)
         p2 = one(even)
         p = p1 | p2
         self.assertTrue((p * 2)(toks))
+
+    def testInv(self):
+        p1 = pseq("abc")
+        p2 = inv(p1)
+        p3 = pseq("cba")
+        self.assertFalse(p2("abc"))
+        self.assertTrue((p2 >> p3)("cba"))
```

### Comparing `fppy-0.0.8/fpy/utils/placeholder.py` & `fppy-0.0.9/fpy/utils/placeholder.py`

 * *Files identical despite different names*

### Comparing `fppy-0.0.8/setup.py` & `fppy-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 DESCRIPTION = "Python module for composing computations"
 CLASSIFIERS = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Natural Language :: English",
     "Operating System :: OS Independent",
```

