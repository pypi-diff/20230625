# Comparing `tmp/hardened-steel-0.0.7.tar.gz` & `tmp/hardened-steel-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardened-steel-0.0.7.tar", last modified: Thu Jun 22 12:13:32 2023, max compression
+gzip compressed data, was "hardened-steel-0.0.8.tar", last modified: Sun Jun 25 15:46:28 2023, max compression
```

## Comparing `hardened-steel-0.0.7.tar` & `hardened-steel-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.257771 hardened-steel-0.0.7/HardenedSteel/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.257771 hardened-steel-0.0.7/HardenedSteel/facades/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.257771 hardened-steel-0.0.7/HardenedSteel/facades/booleans/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/booleans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/booleans/random_boolean_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.257771 hardened-steel-0.0.7/HardenedSteel/facades/integers/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/integers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/integers/random_number_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.257771 hardened-steel-0.0.7/HardenedSteel/facades/texts/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/texts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/HardenedSteel/facades/texts/characters/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/texts/characters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/texts/characters/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/texts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/texts/random_text_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/HardenedSteel/globals/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/globals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/HardenedSteel/globals/singletons/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/globals/singletons/SingletonSystenRandom.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/globals/singletons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/HardenedSteel/globals/vars/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/globals/vars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/globals/vars/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/License.md
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/hardened_steel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-22 12:13:32.000000 hardened-steel-0.0.7/hardened_steel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 12:13:32.000000 hardened-steel-0.0.7/hardened_steel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:13:32.000000 hardened-steel-0.0.7/hardened_steel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 12:13:32.000000 hardened-steel-0.0.7/hardened_steel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/tests/test_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.044695 hardened-steel-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.040696 hardened-steel-0.0.8/HardenedSteel/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.040696 hardened-steel-0.0.8/HardenedSteel/facades/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.040696 hardened-steel-0.0.8/HardenedSteel/facades/binaries/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/binaries/random_binary_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.040696 hardened-steel-0.0.8/HardenedSteel/facades/booleans/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/booleans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/booleans/random_boolean_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.040696 hardened-steel-0.0.8/HardenedSteel/facades/integers/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/integers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/integers/random_number_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/integers/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.040696 hardened-steel-0.0.8/HardenedSteel/facades/texts/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/texts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.040696 hardened-steel-0.0.8/HardenedSteel/facades/texts/characters/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/texts/characters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/texts/characters/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/texts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/texts/random_text_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.040696 hardened-steel-0.0.8/HardenedSteel/facades/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/facades/types/by_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.040696 hardened-steel-0.0.8/HardenedSteel/globals/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/globals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.044695 hardened-steel-0.0.8/HardenedSteel/globals/singletons/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/globals/singletons/SingletonSystenRandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/globals/singletons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.044695 hardened-steel-0.0.8/HardenedSteel/globals/vars/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/globals/vars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/globals/vars/bits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/globals/vars/integer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.044695 hardened-steel-0.0.8/HardenedSteel/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.044695 hardened-steel-0.0.8/HardenedSteel/objects/counters/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/objects/counters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/HardenedSteel/objects/counters/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/License.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-25 15:46:28.044695 hardened-steel-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.044695 hardened-steel-0.0.8/hardened_steel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-25 15:46:28.000000 hardened-steel-0.0.8/hardened_steel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-25 15:46:28.000000 hardened-steel-0.0.8/hardened_steel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:46:28.000000 hardened-steel-0.0.8/hardened_steel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 15:46:28.000000 hardened-steel-0.0.8/hardened_steel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 15:46:28.044695 hardened-steel-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:46:28.044695 hardened-steel-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 15:46:16.000000 hardened-steel-0.0.8/tests/test_singleton.py
```

### Comparing `hardened-steel-0.0.7/HardenedSteel/facades/integers/random_number_generation.py` & `hardened-steel-0.0.8/HardenedSteel/facades/integers/random_number_generation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from HardenedSteel.globals                          \
     import                                          \
     get_minimum_size_of_integer,                    \
     get_maximum_size_of_integer,                    \
-    get_zero,                                       \
+    get_integer_zero,                                       \
     get_maximum_size_of_unsigned_integer,           \
     get_system_random
 
 
 def generate_unsigned_integer(
-        begin: int = get_zero(),
+        begin: int = get_integer_zero(),
         end: int = get_maximum_size_of_unsigned_integer()
 ) -> int:
     return get_system_random().randint(
         begin,
         end
     )
```

### Comparing `hardened-steel-0.0.7/HardenedSteel/facades/texts/characters/ranges.py` & `hardened-steel-0.0.8/HardenedSteel/facades/texts/characters/ranges.py`

 * *Files identical despite different names*

### Comparing `hardened-steel-0.0.7/HardenedSteel/facades/texts/random_text_generation.py` & `hardened-steel-0.0.8/HardenedSteel/facades/texts/random_text_generation.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 from HardenedSteel.facades.texts.exceptions                                 \
     import raise_out_of_boundary_exception
 
 from HardenedSteel.globals                                                  \
     import                                                                  \
     get_maximum_size_of_integer,                                            \
-    get_zero
+    get_integer_zero
 
 
 def detect_outside_boundary_exception(
         index: int
 ):
     raise_out_of_boundary_exception(
         index,
-        get_zero(),
+        get_integer_zero(),
         get_maximum_size_of_integer()
     )
 
 
 def generate_lowercase_label_by_size(
         length_of_label: int
 ) -> str:
```

### Comparing `hardened-steel-0.0.7/HardenedSteel/globals/__init__.py` & `hardened-steel-0.0.8/HardenedSteel/globals/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,11 +2,12 @@
     import                                          \
     get_system_random,                              \
     set_system_random
 
 from HardenedSteel.globals.vars                     \
     import                                          \
     get_maximum_size_of_integer,                    \
-    get_zero,                                       \
-    get_one,                                        \
+    get_integer_zero,                                       \
+    get_integer_one,                                        \
     get_minimum_size_of_integer,                    \
-    get_maximum_size_of_unsigned_integer
+    get_maximum_size_of_unsigned_integer,           \
+    get_conversion_of_a_byte_to_bits
```

### Comparing `hardened-steel-0.0.7/HardenedSteel/globals/singletons/SingletonSystenRandom.py` & `hardened-steel-0.0.8/HardenedSteel/globals/singletons/SingletonSystenRandom.py`

 * *Files identical despite different names*

### Comparing `hardened-steel-0.0.7/HardenedSteel/globals/vars/integer.py` & `hardened-steel-0.0.8/HardenedSteel/globals/vars/integer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 from HardenedSteel.globals.vars \
     import maxsize
 
 zero: int = 0
 one: int = 1
+two: int = 2
+three: int = 3
+four: int = 4
+five: int = 5
+six: int = 6
+seven: int = 7
+eight: int = 8
+nine: int = 9
 
 unsigned_max_size: int = 4294967295
 
 integer_max_size: int = maxsize
 integer_min_size: int = -maxsize - one
 
 
@@ -21,15 +29,15 @@
 
 
 def get_maximum_size_of_integer() -> int:
     global integer_max_size
     return integer_max_size
 
 
-def get_zero() -> int:
+def get_integer_zero() -> int:
     global zero
     return zero
 
 
-def get_one() -> int:
+def get_integer_one() -> int:
     global one
     return one
```

### Comparing `hardened-steel-0.0.7/License.md` & `hardened-steel-0.0.8/License.md`

 * *Files identical despite different names*

### Comparing `hardened-steel-0.0.7/PKG-INFO` & `hardened-steel-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardened-steel
-Version: 0.0.7
+Version: 0.0.8
 Summary: Framework for helping to test projects with the generation of random data during TDD
 Author-email: IO Jægers <support@cloud.iojaegers.com>, Kent Madsen <kent.vejrup.madsen@outlook.com>
 License: # MIT License
         
         Copyright (c) 2023 IO Jægers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hardened-steel-0.0.7/Readme.md` & `hardened-steel-0.0.8/Readme.md`

 * *Files identical despite different names*

### Comparing `hardened-steel-0.0.7/hardened_steel.egg-info/PKG-INFO` & `hardened-steel-0.0.8/hardened_steel.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardened-steel
-Version: 0.0.7
+Version: 0.0.8
 Summary: Framework for helping to test projects with the generation of random data during TDD
 Author-email: IO Jægers <support@cloud.iojaegers.com>, Kent Madsen <kent.vejrup.madsen@outlook.com>
 License: # MIT License
         
         Copyright (c) 2023 IO Jægers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hardened-steel-0.0.7/hardened_steel.egg-info/SOURCES.txt` & `hardened-steel-0.0.8/hardened_steel.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 License.md
 Readme.md
 pyproject.toml
 HardenedSteel/__init__.py
 HardenedSteel/facades/__init__.py
+HardenedSteel/facades/binaries/__init__.py
+HardenedSteel/facades/binaries/random_binary_generation.py
 HardenedSteel/facades/booleans/__init__.py
 HardenedSteel/facades/booleans/random_boolean_generation.py
 HardenedSteel/facades/integers/__init__.py
 HardenedSteel/facades/integers/random_number_generation.py
+HardenedSteel/facades/integers/states.py
 HardenedSteel/facades/texts/__init__.py
 HardenedSteel/facades/texts/exceptions.py
 HardenedSteel/facades/texts/random_text_generation.py
 HardenedSteel/facades/texts/characters/__init__.py
 HardenedSteel/facades/texts/characters/ranges.py
+HardenedSteel/facades/types/__init__.py
+HardenedSteel/facades/types/by_types.py
 HardenedSteel/globals/__init__.py
 HardenedSteel/globals/singletons/SingletonSystenRandom.py
 HardenedSteel/globals/singletons/__init__.py
 HardenedSteel/globals/vars/__init__.py
+HardenedSteel/globals/vars/bits.py
 HardenedSteel/globals/vars/integer.py
+HardenedSteel/objects/__init__.py
+HardenedSteel/objects/counters/__init__.py
+HardenedSteel/objects/counters/counter.py
 hardened_steel.egg-info/PKG-INFO
 hardened_steel.egg-info/SOURCES.txt
 hardened_steel.egg-info/dependency_links.txt
 hardened_steel.egg-info/top_level.txt
 tests/test_default.py
 tests/test_singleton.py
```

### Comparing `hardened-steel-0.0.7/pyproject.toml` & `hardened-steel-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.10"
 
 name = "hardened-steel"
-version = "0.0.7"
+version = "0.0.8"
 
 authors = [
   { name="IO Jægers", email="support@cloud.iojaegers.com" },
   { name="Kent Madsen", email="kent.vejrup.madsen@outlook.com" },
 ]
 
 description = "Framework for helping to test projects with the generation of random data during TDD"
```

