# Comparing `tmp/decorator-parser-1.0.1.tar.gz` & `tmp/decorator_parser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorator-parser-1.0.1.tar", last modified: Sun Jun 25 15:38:43 2023, max compression
+gzip compressed data, was "decorator_parser-1.0.2.tar", last modified: Sun Jun 25 15:46:29 2023, max compression
```

## Comparing `decorator-parser-1.0.1.tar` & `decorator_parser-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      519 2023-06-25 14:29:47.000000 decorator-parser-1.0.1/LICENSE
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4288 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/PKG-INFO
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     3778 2023-06-25 15:36:36.000000 decorator-parser-1.0.1/README.md
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      587 2023-06-25 15:38:34.000000 decorator-parser-1.0.1/pyproject.toml
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       38 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/setup.cfg
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/src/
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/src/decorator-parser/
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 14:21:25.000000 decorator-parser-1.0.1/src/decorator-parser/__init__.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     1093 2023-06-25 15:29:08.000000 decorator-parser-1.0.1/src/decorator-parser/errors.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4468 2023-06-25 15:28:37.000000 decorator-parser-1.0.1/src/decorator-parser/parse.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      280 2023-06-24 15:49:57.000000 decorator-parser-1.0.1/src/decorator-parser/parse_task.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      522 2023-06-25 14:48:43.000000 decorator-parser-1.0.1/src/decorator-parser/test.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      240 2023-06-25 14:46:06.000000 decorator-parser-1.0.1/src/decorator-parser/utils.py
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/src/decorator_parser.egg-info/
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4288 2023-06-25 15:38:43.000000 decorator-parser-1.0.1/src/decorator_parser.egg-info/PKG-INFO
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      396 2023-06-25 15:38:43.000000 decorator-parser-1.0.1/src/decorator_parser.egg-info/SOURCES.txt
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        1 2023-06-25 15:38:43.000000 decorator-parser-1.0.1/src/decorator_parser.egg-info/dependency_links.txt
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       17 2023-06-25 15:38:43.000000 decorator-parser-1.0.1/src/decorator_parser.egg-info/top_level.txt
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:46:29.128250 decorator_parser-1.0.2/
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      519 2023-06-25 14:29:47.000000 decorator_parser-1.0.2/LICENSE
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4288 2023-06-25 15:46:29.128250 decorator_parser-1.0.2/PKG-INFO
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     3778 2023-06-25 15:45:31.000000 decorator_parser-1.0.2/README.md
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      587 2023-06-25 15:45:43.000000 decorator_parser-1.0.2/pyproject.toml
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       38 2023-06-25 15:46:29.128250 decorator_parser-1.0.2/setup.cfg
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:46:29.118250 decorator_parser-1.0.2/src/
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:46:29.128250 decorator_parser-1.0.2/src/decorator_parser/
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 14:21:25.000000 decorator_parser-1.0.2/src/decorator_parser/__init__.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     1093 2023-06-25 15:29:08.000000 decorator_parser-1.0.2/src/decorator_parser/errors.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4468 2023-06-25 15:46:07.000000 decorator_parser-1.0.2/src/decorator_parser/parse.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      280 2023-06-25 15:42:15.000000 decorator_parser-1.0.2/src/decorator_parser/parse_task.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      522 2023-06-25 14:48:43.000000 decorator_parser-1.0.2/src/decorator_parser/test.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      240 2023-06-25 15:46:10.000000 decorator_parser-1.0.2/src/decorator_parser/utils.py
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:46:29.128250 decorator_parser-1.0.2/src/decorator_parser.egg-info/
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4288 2023-06-25 15:46:29.000000 decorator_parser-1.0.2/src/decorator_parser.egg-info/PKG-INFO
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      396 2023-06-25 15:46:29.000000 decorator_parser-1.0.2/src/decorator_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        1 2023-06-25 15:46:29.000000 decorator_parser-1.0.2/src/decorator_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       17 2023-06-25 15:46:29.000000 decorator_parser-1.0.2/src/decorator_parser.egg-info/top_level.txt
```

### Comparing `decorator-parser-1.0.1/LICENSE` & `decorator_parser-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decorator-parser-1.0.1/PKG-INFO` & `decorator_parser-1.0.2/src/decorator_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator-parser
-Version: 1.0.1
+Version: 1.0.2
 Summary: Parser for text files with decorators into Python dictionaries
 Author-email: Michal Kostyk <m.kostyk22@gmail.com>
 Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
 Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -15,15 +15,15 @@
 
 ### License
 © 2023 Smartschool Inc. All rights reserved.
 
 ### Installation guide
 1. Install Python 3.7 or newer from [https://www.python.org/downloads/](https://www.python.org/downloads/)
 2. Install PIP using [this guide](https://pip.pypa.io/en/stable/installation/)
-3. Run `pip install decorator-parser` in your command line
+3. Run `pip install decorator_parser` in your command line
 
 ### Decorators format
 Decorator name can be any string that does not contain '@' character or a newline character. There should be no whitespaces after the decorator name nor after its closing parenthesis. Decorator can, but does not have to end with a newline. If a decorator does not satisfy these requirements `InvalidDecoratorException` will be thrown.
 
 #### Example:
 ```
 @decorator(some nice value)
```

### Comparing `decorator-parser-1.0.1/README.md` & `decorator_parser-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ### License
 © 2023 Smartschool Inc. All rights reserved.
 
 ### Installation guide
 1. Install Python 3.7 or newer from [https://www.python.org/downloads/](https://www.python.org/downloads/)
 2. Install PIP using [this guide](https://pip.pypa.io/en/stable/installation/)
-3. Run `pip install decorator-parser` in your command line
+3. Run `pip install decorator_parser` in your command line
 
 ### Decorators format
 Decorator name can be any string that does not contain '@' character or a newline character. There should be no whitespaces after the decorator name nor after its closing parenthesis. Decorator can, but does not have to end with a newline. If a decorator does not satisfy these requirements `InvalidDecoratorException` will be thrown.
 
 #### Example:
 ```
 @decorator(some nice value)
```

### Comparing `decorator-parser-1.0.1/pyproject.toml` & `decorator_parser-1.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "decorator-parser"
-version = "1.0.1"
+name = "decorator_parser"
+version = "1.0.2"
 authors = [
   { name="Michal Kostyk", email="m.kostyk22@gmail.com" },
 ]
 description = "Parser for text files with decorators into Python dictionaries"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `decorator-parser-1.0.1/src/decorator-parser/errors.py` & `decorator_parser-1.0.2/src/decorator_parser/errors.py`

 * *Files identical despite different names*

### Comparing `decorator-parser-1.0.1/src/decorator-parser/parse.py` & `decorator_parser-1.0.2/src/decorator_parser/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Author: Michał Kostyk for Smartschool Inc.
 # Date: 2023
-# Version: 1.0.0
+# Version: 1.0.2
 
 from errors import *
 from utils import *
 import re
 
 
 class Parser:
```

### Comparing `decorator-parser-1.0.1/src/decorator-parser/test.py` & `decorator_parser-1.0.2/src/decorator_parser/test.py`

 * *Files identical despite different names*

### Comparing `decorator-parser-1.0.1/src/decorator_parser.egg-info/PKG-INFO` & `decorator_parser-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: decorator-parser
-Version: 1.0.1
+Name: decorator_parser
+Version: 1.0.2
 Summary: Parser for text files with decorators into Python dictionaries
 Author-email: Michal Kostyk <m.kostyk22@gmail.com>
 Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
 Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -15,15 +15,15 @@
 
 ### License
 © 2023 Smartschool Inc. All rights reserved.
 
 ### Installation guide
 1. Install Python 3.7 or newer from [https://www.python.org/downloads/](https://www.python.org/downloads/)
 2. Install PIP using [this guide](https://pip.pypa.io/en/stable/installation/)
-3. Run `pip install decorator-parser` in your command line
+3. Run `pip install decorator_parser` in your command line
 
 ### Decorators format
 Decorator name can be any string that does not contain '@' character or a newline character. There should be no whitespaces after the decorator name nor after its closing parenthesis. Decorator can, but does not have to end with a newline. If a decorator does not satisfy these requirements `InvalidDecoratorException` will be thrown.
 
 #### Example:
 ```
 @decorator(some nice value)
```

