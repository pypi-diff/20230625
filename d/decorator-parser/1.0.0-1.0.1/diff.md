# Comparing `tmp/decorator-parser-1.0.0.tar.gz` & `tmp/decorator-parser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorator-parser-1.0.0.tar", last modified: Sun Jun 25 14:40:13 2023, max compression
+gzip compressed data, was "decorator-parser-1.0.1.tar", last modified: Sun Jun 25 15:38:43 2023, max compression
```

## Comparing `decorator-parser-1.0.0.tar` & `decorator-parser-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 14:40:13.748254 decorator-parser-1.0.0/
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      519 2023-06-25 14:29:47.000000 decorator-parser-1.0.0/LICENSE
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     3192 2023-06-25 14:40:13.748254 decorator-parser-1.0.0/PKG-INFO
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     2682 2023-06-24 22:54:21.000000 decorator-parser-1.0.0/README.md
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      587 2023-06-25 14:40:07.000000 decorator-parser-1.0.0/pyproject.toml
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       38 2023-06-25 14:40:13.748254 decorator-parser-1.0.0/setup.cfg
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 14:40:13.738254 decorator-parser-1.0.0/src/
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 14:40:13.738254 decorator-parser-1.0.0/src/decorator-parser/
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 14:21:25.000000 decorator-parser-1.0.0/src/decorator-parser/__init__.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     1059 2023-06-24 22:43:14.000000 decorator-parser-1.0.0/src/decorator-parser/errors.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     3748 2023-06-24 22:31:23.000000 decorator-parser-1.0.0/src/decorator-parser/parse.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      240 2023-06-24 22:38:30.000000 decorator-parser-1.0.0/src/decorator-parser/utils.py
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 14:40:13.738254 decorator-parser-1.0.0/src/decorator_parser.egg-info/
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     3192 2023-06-25 14:40:13.000000 decorator-parser-1.0.0/src/decorator_parser.egg-info/PKG-INFO
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      362 2023-06-25 14:40:13.000000 decorator-parser-1.0.0/src/decorator_parser.egg-info/SOURCES.txt
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        1 2023-06-25 14:40:13.000000 decorator-parser-1.0.0/src/decorator_parser.egg-info/dependency_links.txt
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       33 2023-06-25 14:40:13.000000 decorator-parser-1.0.0/src/decorator_parser.egg-info/top_level.txt
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      280 2023-06-24 15:49:57.000000 decorator-parser-1.0.0/src/parse_task.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      522 2023-06-24 21:39:07.000000 decorator-parser-1.0.0/src/test.py
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      519 2023-06-25 14:29:47.000000 decorator-parser-1.0.1/LICENSE
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4288 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/PKG-INFO
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     3778 2023-06-25 15:36:36.000000 decorator-parser-1.0.1/README.md
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      587 2023-06-25 15:38:34.000000 decorator-parser-1.0.1/pyproject.toml
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       38 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/setup.cfg
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/src/
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/src/decorator-parser/
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 14:21:25.000000 decorator-parser-1.0.1/src/decorator-parser/__init__.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     1093 2023-06-25 15:29:08.000000 decorator-parser-1.0.1/src/decorator-parser/errors.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4468 2023-06-25 15:28:37.000000 decorator-parser-1.0.1/src/decorator-parser/parse.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      280 2023-06-24 15:49:57.000000 decorator-parser-1.0.1/src/decorator-parser/parse_task.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      522 2023-06-25 14:48:43.000000 decorator-parser-1.0.1/src/decorator-parser/test.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      240 2023-06-25 14:46:06.000000 decorator-parser-1.0.1/src/decorator-parser/utils.py
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:38:43.038260 decorator-parser-1.0.1/src/decorator_parser.egg-info/
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4288 2023-06-25 15:38:43.000000 decorator-parser-1.0.1/src/decorator_parser.egg-info/PKG-INFO
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      396 2023-06-25 15:38:43.000000 decorator-parser-1.0.1/src/decorator_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        1 2023-06-25 15:38:43.000000 decorator-parser-1.0.1/src/decorator_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       17 2023-06-25 15:38:43.000000 decorator-parser-1.0.1/src/decorator_parser.egg-info/top_level.txt
```

### Comparing `decorator-parser-1.0.0/LICENSE` & `decorator-parser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decorator-parser-1.0.0/PKG-INFO` & `decorator-parser-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,51 @@
-Metadata-Version: 2.1
-Name: decorator-parser
-Version: 1.0.0
-Summary: Parser for text files with decorators into Python dictionaries
-Author-email: Michal Kostyk <m.kostyk22@gmail.com>
-Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
-Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Decorators Parser
 
 ### License
 © 2023 Smartschool Inc. All rights reserved.
 
+### Installation guide
+1. Install Python 3.7 or newer from [https://www.python.org/downloads/](https://www.python.org/downloads/)
+2. Install PIP using [this guide](https://pip.pypa.io/en/stable/installation/)
+3. Run `pip install decorator-parser` in your command line
+
+### Decorators format
+Decorator name can be any string that does not contain '@' character or a newline character. There should be no whitespaces after the decorator name nor after its closing parenthesis. Decorator can, but does not have to end with a newline. If a decorator does not satisfy these requirements `InvalidDecoratorException` will be thrown.
+
+#### Example:
+```
+@decorator(some nice value)
+```
+
 ### Standard decorators
-Decorators can be used in one of two ways:
+Decorators can be used in one of three ways:
 ```
 @decorator(value)
 ```
 or
 ```
 @decorator()
 Some very long and complicated value that would be hard to read if it were in parenthesis like the value above.
 ```
+or
+```
+@decorator
+Some very long and complicated value that would be hard to read if it were in parenthesis like the value above.
+```
 
-Both of these create Python dictionary like this:
+All of these create Python dictionary like this:
 ```python
 {
     'decorator': 'value'
 }
 ```
 
 ### @new decorator
 
-Using @new decorator starts a new dictionary and adds it to the current list of dictionaries
+Using @new decorator starts a new dictionary and adds it to the current list of dictionaries. In a single piece of text between two @new decorators (which correspond to a single Python dictionary) there can not be two decorators with the same name. Using a same name without an appropriate @new decorator will result in `DuplicateDecoratorException` being thrown.
 
 #### Example:
 task.txt:
 ```
 @question()
 Who is Lincoln?
 
@@ -149,11 +154,11 @@
 ```
 correct(1)
 ```
 
 The output will be:
 ```python
 [
-	{
-		'correct': '1'
-	}
+    {
+        'correct': '1'
+    }
 ]
```

### Comparing `decorator-parser-1.0.0/README.md` & `decorator-parser-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,64 @@
+Metadata-Version: 2.1
+Name: decorator-parser
+Version: 1.0.1
+Summary: Parser for text files with decorators into Python dictionaries
+Author-email: Michal Kostyk <m.kostyk22@gmail.com>
+Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
+Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Decorators Parser
 
 ### License
 © 2023 Smartschool Inc. All rights reserved.
 
+### Installation guide
+1. Install Python 3.7 or newer from [https://www.python.org/downloads/](https://www.python.org/downloads/)
+2. Install PIP using [this guide](https://pip.pypa.io/en/stable/installation/)
+3. Run `pip install decorator-parser` in your command line
+
+### Decorators format
+Decorator name can be any string that does not contain '@' character or a newline character. There should be no whitespaces after the decorator name nor after its closing parenthesis. Decorator can, but does not have to end with a newline. If a decorator does not satisfy these requirements `InvalidDecoratorException` will be thrown.
+
+#### Example:
+```
+@decorator(some nice value)
+```
+
 ### Standard decorators
-Decorators can be used in one of two ways:
+Decorators can be used in one of three ways:
 ```
 @decorator(value)
 ```
 or
 ```
 @decorator()
 Some very long and complicated value that would be hard to read if it were in parenthesis like the value above.
 ```
+or
+```
+@decorator
+Some very long and complicated value that would be hard to read if it were in parenthesis like the value above.
+```
 
-Both of these create Python dictionary like this:
+All of these create Python dictionary like this:
 ```python
 {
     'decorator': 'value'
 }
 ```
 
 ### @new decorator
 
-Using @new decorator starts a new dictionary and adds it to the current list of dictionaries
+Using @new decorator starts a new dictionary and adds it to the current list of dictionaries. In a single piece of text between two @new decorators (which correspond to a single Python dictionary) there can not be two decorators with the same name. Using a same name without an appropriate @new decorator will result in `DuplicateDecoratorException` being thrown.
 
 #### Example:
 task.txt:
 ```
 @question()
 Who is Lincoln?
 
@@ -136,11 +167,11 @@
 ```
 correct(1)
 ```
 
 The output will be:
 ```python
 [
-	{
-		'correct': '1'
-	}
+    {
+        'correct': '1'
+    }
 ]
```

### Comparing `decorator-parser-1.0.0/pyproject.toml` & `decorator-parser-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "decorator-parser"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Michal Kostyk", email="m.kostyk22@gmail.com" },
 ]
 description = "Parser for text files with decorators into Python dictionaries"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `decorator-parser-1.0.0/src/decorator-parser/errors.py` & `decorator-parser-1.0.1/src/decorator-parser/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 # Author: Michał Kostyk for Smartschool Inc.
 # Date: 2023
 # Version: 1.0.0
 # Description: Custom errors for the project.
 
 from utils import FAIL, ENDC, BOLD
 
-# TODO: this is not perfect
 def line_number(data, line):
     matches = data.split(line)
     return len(matches[0].split('\n'))
 
 
 # Exception class that adds coloring to the message
 class FailException(Exception):
     def __init__(self, message):
-        self.message = FAIL + message + ENDC
+        self.message = BOLD + FAIL + message + ENDC
         super().__init__(self.message)
 
 
 # Exception class that adds line number to the message
 class ExceptionWithLine(FailException):
     def __init__(self, data, value, message):
         self.line = line_number(data, value)
-        self.message = BOLD + FAIL + f"Line {self.line}: " + message
+        self.message = f"Line {self.line}: " + message
         super().__init__(self.message)
 
 
 class DecoratorNotFoundException(FailException):
     ...
     pass
 
 
 class InvalidConstraintException(FailException):
     ...
     pass
 
 
+class DuplicateDecoratorException(FailException):
+    ...
+    pass
+
+
 class InvalidDecoratorException(ExceptionWithLine):
     ...
     pass
 
 
 class InvalidValueException(ExceptionWithLine):
     ...
```

### Comparing `decorator-parser-1.0.0/src/decorator-parser/parse.py` & `decorator-parser-1.0.1/src/decorator-parser/parse.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,47 +41,65 @@
     def split_by_new(self, data):
         return data.split('@new')
 
 
     # Removes decorator and its value from data
     def remove_decorator(self, data):
         splitted = data.split('@')
-        if len(splitted) < 2:
+        # This means that splitted looks like ['', decorator] right now, so it
+        # is the last decorator, and after deletion we want it to be ""
+        if len(splitted) <= 2:
             return ""
 
         data = '@' + '@'.join(data.split('@')[2:])
 
         return data
 
 
     # Handles a single decorator.
-    def handle_decorator(self, data, result):      
-        decorator = re.search(r'(@[^\s]*\([^\s]*\))', data)
-        if decorator is None:
+    def handle_decorator(self, data, result):
+        # Look for the first @ in the file - it is a candidate for a decorator
+        candidate = re.search(r'(@[^\n]*$)', data, re.MULTILINE)
+        if candidate is None:
             raise DecoratorNotFoundException("No more decorators found")
+        candidate = candidate.group(0)
+        
+        # Look for a legit decorator
+        decorator = re.search(r'(@[^\s]*$)', data, re.MULTILINE)
+        if decorator is None:
+            raise InvalidDecoratorException(self.original_data, candidate, "Invalid decorator")
         decorator = decorator.group(0)
+
+        # Check if decorator is the same as candidate
+        if not decorator == candidate:
+            raise InvalidDecoratorException(self.original_data, candidate, "Invalid decorator")
         
         name = decorator.split('(')[0].split('@')[1]
+        decor_with_val = decorator # For error messages
+        value = ""
 
-        # There are two options how to put value: @decorator(value) or @decorator() value
-        # Regex validation guarantees that neither this nor the next line will throw IndexError
-        value = decorator.split('(')[1].split(')')[0].strip()
+        # Value can be put in brackets or after decorator
+        try:
+            value = decorator.split('(')[1].split(')')[0].strip()
+        except IndexError:
+            pass
 
         if value == "":
             value = data.split(decorator)[1].split('@')[0].strip()
+            decor_with_val += value
 
         if name in result:
-            raise InvalidDecoratorException(self.original_data, decorator, f"Duplicate decorator '{name}'")
+            raise DuplicateDecoratorException(f"Duplicate decorator '{name}'")
 
         if name in self.constraints:
             description = self.constraints[name]['description']
 
             # Checking constraint match
             if not re.fullmatch(self.constraints[name]['regex'], value):
-                raise InvalidValueException(self.original_data, value, f"'{name}' should be {description} but is {value}")
+                raise InvalidValueException(self.original_data, decor_with_val, f"'{name}' should be {description} but is {value}")
             
         result[name] = value
 
         return result
 
 
     # Handles all decorators in a single @new object
```

### Comparing `decorator-parser-1.0.0/src/decorator_parser.egg-info/PKG-INFO` & `decorator-parser-1.0.1/src/decorator_parser.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator-parser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Parser for text files with decorators into Python dictionaries
 Author-email: Michal Kostyk <m.kostyk22@gmail.com>
 Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
 Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -12,35 +12,53 @@
 License-File: LICENSE
 
 ## Decorators Parser
 
 ### License
 © 2023 Smartschool Inc. All rights reserved.
 
+### Installation guide
+1. Install Python 3.7 or newer from [https://www.python.org/downloads/](https://www.python.org/downloads/)
+2. Install PIP using [this guide](https://pip.pypa.io/en/stable/installation/)
+3. Run `pip install decorator-parser` in your command line
+
+### Decorators format
+Decorator name can be any string that does not contain '@' character or a newline character. There should be no whitespaces after the decorator name nor after its closing parenthesis. Decorator can, but does not have to end with a newline. If a decorator does not satisfy these requirements `InvalidDecoratorException` will be thrown.
+
+#### Example:
+```
+@decorator(some nice value)
+```
+
 ### Standard decorators
-Decorators can be used in one of two ways:
+Decorators can be used in one of three ways:
 ```
 @decorator(value)
 ```
 or
 ```
 @decorator()
 Some very long and complicated value that would be hard to read if it were in parenthesis like the value above.
 ```
+or
+```
+@decorator
+Some very long and complicated value that would be hard to read if it were in parenthesis like the value above.
+```
 
-Both of these create Python dictionary like this:
+All of these create Python dictionary like this:
 ```python
 {
     'decorator': 'value'
 }
 ```
 
 ### @new decorator
 
-Using @new decorator starts a new dictionary and adds it to the current list of dictionaries
+Using @new decorator starts a new dictionary and adds it to the current list of dictionaries. In a single piece of text between two @new decorators (which correspond to a single Python dictionary) there can not be two decorators with the same name. Using a same name without an appropriate @new decorator will result in `DuplicateDecoratorException` being thrown.
 
 #### Example:
 task.txt:
 ```
 @question()
 Who is Lincoln?
 
@@ -149,11 +167,11 @@
 ```
 correct(1)
 ```
 
 The output will be:
 ```python
 [
-	{
-		'correct': '1'
-	}
+    {
+        'correct': '1'
+    }
 ]
```

### Comparing `decorator-parser-1.0.0/src/test.py` & `decorator-parser-1.0.1/src/decorator-parser/test.py`

 * *Files identical despite different names*

