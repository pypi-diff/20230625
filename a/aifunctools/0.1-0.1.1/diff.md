# Comparing `tmp/aifunctools-0.1.tar.gz` & `tmp/aifunctools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunctools-0.1.tar", last modified: Sat Jun 17 18:50:15 2023, max compression
+gzip compressed data, was "aifunctools-0.1.1.tar", last modified: Sun Jun 25 00:03:55 2023, max compression
```

## Comparing `aifunctools-0.1.tar` & `aifunctools-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-17 18:50:15.928997 aifunctools-0.1/
--rw-r--r--   0 changshe   (501) staff       (20)    11329 2023-06-17 16:31:19.000000 aifunctools-0.1/LICENSE.txt
--rw-r--r--   0 changshe   (501) staff       (20)    16479 2023-06-17 18:50:15.928872 aifunctools-0.1/PKG-INFO
--rw-r--r--   0 changshe   (501) staff       (20)     2504 2023-06-17 18:49:39.000000 aifunctools-0.1/README.md
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-17 18:50:15.928039 aifunctools-0.1/aifunctools/
--rw-r--r--   0 changshe   (501) staff       (20)        0 2023-06-17 16:23:48.000000 aifunctools-0.1/aifunctools/__init__.py
--rw-r--r--   0 changshe   (501) staff       (20)     3230 2023-06-17 18:32:47.000000 aifunctools-0.1/aifunctools/openai_funcs.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-17 18:50:15.928591 aifunctools-0.1/aifunctools.egg-info/
--rw-r--r--   0 changshe   (501) staff       (20)    16479 2023-06-17 18:50:15.000000 aifunctools-0.1/aifunctools.egg-info/PKG-INFO
--rw-r--r--   0 changshe   (501) staff       (20)      282 2023-06-17 18:50:15.000000 aifunctools-0.1/aifunctools.egg-info/SOURCES.txt
--rw-r--r--   0 changshe   (501) staff       (20)        1 2023-06-17 18:50:15.000000 aifunctools-0.1/aifunctools.egg-info/dependency_links.txt
--rw-r--r--   0 changshe   (501) staff       (20)       39 2023-06-17 18:50:15.000000 aifunctools-0.1/aifunctools.egg-info/requires.txt
--rw-r--r--   0 changshe   (501) staff       (20)       12 2023-06-17 18:50:15.000000 aifunctools-0.1/aifunctools.egg-info/top_level.txt
--rw-r--r--   0 changshe   (501) staff       (20)     1187 2023-06-17 18:50:10.000000 aifunctools-0.1/pyproject.toml
--rw-r--r--   0 changshe   (501) staff       (20)       38 2023-06-17 18:50:15.929028 aifunctools-0.1/setup.cfg
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-17 18:50:15.928709 aifunctools-0.1/tests/
--rw-r--r--   0 changshe   (501) staff       (20)      804 2023-06-17 18:43:52.000000 aifunctools-0.1/tests/test_basic.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-25 00:03:55.266947 aifunctools-0.1.1/
+-rw-r--r--   0 changshe   (501) staff       (20)    11329 2023-06-17 16:31:19.000000 aifunctools-0.1.1/LICENSE.txt
+-rw-r--r--   0 changshe   (501) staff       (20)    16481 2023-06-25 00:03:55.266811 aifunctools-0.1.1/PKG-INFO
+-rw-r--r--   0 changshe   (501) staff       (20)     2504 2023-06-17 18:49:39.000000 aifunctools-0.1.1/README.md
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-25 00:03:55.265718 aifunctools-0.1.1/aifunctools/
+-rw-r--r--   0 changshe   (501) staff       (20)        0 2023-06-17 16:23:48.000000 aifunctools-0.1.1/aifunctools/__init__.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1857 2023-06-25 00:03:03.000000 aifunctools-0.1.1/aifunctools/openai_funcs.py
+-rw-r--r--   0 changshe   (501) staff       (20)     2266 2023-06-25 00:03:03.000000 aifunctools-0.1.1/aifunctools/parser.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1440 2023-06-24 21:52:20.000000 aifunctools-0.1.1/aifunctools/utils.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-25 00:03:55.266427 aifunctools-0.1.1/aifunctools.egg-info/
+-rw-r--r--   0 changshe   (501) staff       (20)    16481 2023-06-25 00:03:55.000000 aifunctools-0.1.1/aifunctools.egg-info/PKG-INFO
+-rw-r--r--   0 changshe   (501) staff       (20)      346 2023-06-25 00:03:55.000000 aifunctools-0.1.1/aifunctools.egg-info/SOURCES.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        1 2023-06-25 00:03:55.000000 aifunctools-0.1.1/aifunctools.egg-info/dependency_links.txt
+-rw-r--r--   0 changshe   (501) staff       (20)       62 2023-06-25 00:03:55.000000 aifunctools-0.1.1/aifunctools.egg-info/requires.txt
+-rw-r--r--   0 changshe   (501) staff       (20)       12 2023-06-25 00:03:55.000000 aifunctools-0.1.1/aifunctools.egg-info/top_level.txt
+-rw-r--r--   0 changshe   (501) staff       (20)     1218 2023-06-24 22:27:15.000000 aifunctools-0.1.1/pyproject.toml
+-rw-r--r--   0 changshe   (501) staff       (20)       38 2023-06-25 00:03:55.266978 aifunctools-0.1.1/setup.cfg
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-25 00:03:55.266644 aifunctools-0.1.1/tests/
+-rw-r--r--   0 changshe   (501) staff       (20)      897 2023-06-25 00:03:03.000000 aifunctools-0.1.1/tests/test_basic.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1938 2023-06-24 22:13:22.000000 aifunctools-0.1.1/tests/test_parser.py
```

### Comparing `aifunctools-0.1/LICENSE.txt` & `aifunctools-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aifunctools-0.1/PKG-INFO` & `aifunctools-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aifunctools
-Version: 0.1
+Version: 0.1.1
 Summary: Utilities for AI functions
 Author-email: Chang She <chang@lancedb.com>
 License:       Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `aifunctools-0.1/README.md` & `aifunctools-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aifunctools-0.1/aifunctools.egg-info/PKG-INFO` & `aifunctools-0.1.1/aifunctools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aifunctools
-Version: 0.1
+Version: 0.1.1
 Summary: Utilities for AI functions
 Author-email: Chang She <chang@lancedb.com>
 License:       Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `aifunctools-0.1/pyproject.toml` & `aifunctools-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aifunctools"
-version = "0.1"
+version = "0.1.1"
 description = "Utilities for AI functions"
 readme = "README.md" # Optional
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 
 keywords = ["openai", "machine learning", "gpt functions"]
 
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [
-  "openai", "docstring-parser"
+  "openai", "docstring-parser", "pydantic>=2.0b3", "marvin"
 ]
 
 [project.optional-dependencies]
 test = ["pytest"]
 
 [project.urls]
 "Homepage" = "https://github.com/lancedb/aifunctools"
```

