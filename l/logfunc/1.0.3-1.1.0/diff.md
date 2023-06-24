# Comparing `tmp/logfunc-1.0.3.tar.gz` & `tmp/logfunc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfunc-1.0.3.tar", last modified: Fri Jun 23 18:06:24 2023, max compression
+gzip compressed data, was "logfunc-1.1.0.tar", last modified: Sat Jun 24 23:19:46 2023, max compression
```

## Comparing `logfunc-1.0.3.tar` & `logfunc-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-23 18:06:24.959863 logfunc-1.0.3/
--rw-r--r--   0 work       (501) staff       (20)     1068 2023-06-23 16:56:28.000000 logfunc-1.0.3/LICENSE
--rw-r--r--   0 work       (501) staff       (20)     2556 2023-06-23 18:06:24.959745 logfunc-1.0.3/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     1742 2023-06-23 17:56:54.000000 logfunc-1.0.3/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-23 18:06:24.959051 logfunc-1.0.3/logfunc/
--rw-r--r--   0 work       (501) staff       (20)     3513 2023-06-23 17:51:50.000000 logfunc-1.0.3/logfunc/__init__.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-23 18:06:24.959592 logfunc-1.0.3/logfunc.egg-info/
--rw-r--r--   0 work       (501) staff       (20)     2556 2023-06-23 18:06:24.000000 logfunc-1.0.3/logfunc.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      170 2023-06-23 18:06:24.000000 logfunc-1.0.3/logfunc.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-06-23 18:06:24.000000 logfunc-1.0.3/logfunc.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)        8 2023-06-23 18:06:24.000000 logfunc-1.0.3/logfunc.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       38 2023-06-23 18:06:24.959899 logfunc-1.0.3/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)     1071 2023-06-23 18:06:00.000000 logfunc-1.0.3/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-24 23:19:46.444924 logfunc-1.1.0/
+-rw-r--r--   0 work       (501) staff       (20)     1068 2023-06-23 16:56:28.000000 logfunc-1.1.0/LICENSE
+-rw-r--r--   0 work       (501) staff       (20)     3326 2023-06-24 23:19:46.444804 logfunc-1.1.0/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     2512 2023-06-24 22:57:55.000000 logfunc-1.1.0/README.md
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-24 23:19:46.444175 logfunc-1.1.0/logfunc/
+-rw-r--r--   0 work       (501) staff       (20)     3664 2023-06-24 23:05:14.000000 logfunc-1.1.0/logfunc/__init__.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-24 23:19:46.444654 logfunc-1.1.0/logfunc.egg-info/
+-rw-r--r--   0 work       (501) staff       (20)     3326 2023-06-24 23:19:46.000000 logfunc-1.1.0/logfunc.egg-info/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)      170 2023-06-24 23:19:46.000000 logfunc-1.1.0/logfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (501) staff       (20)        1 2023-06-24 23:19:46.000000 logfunc-1.1.0/logfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (501) staff       (20)        8 2023-06-24 23:19:46.000000 logfunc-1.1.0/logfunc.egg-info/top_level.txt
+-rw-r--r--   0 work       (501) staff       (20)       38 2023-06-24 23:19:46.444963 logfunc-1.1.0/setup.cfg
+-rw-r--r--   0 work       (501) staff       (20)     1071 2023-06-24 23:18:12.000000 logfunc-1.1.0/setup.py
```

### Comparing `logfunc-1.0.3/LICENSE` & `logfunc-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfunc-1.0.3/PKG-INFO` & `logfunc-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.0.3
+Version: 1.1.0
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/tree/main
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,26 +16,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # logf
 
-the @logf() decorator i previously had as part of the myfuncs pip package, decided to make it standalone pip package this is the repo for it
+The `@logf()` decorator, previously a part of the myfuncs pip package, is now a standalone pip package. This repository is dedicated to its development and maintenance.
 
 ## Usage
 
-Here is a brief guide on how to use the `logfunc` module.
+This is a brief guide on how to use the `logfunc` module.
 
 ### Installation
 
-First, you need to install the `logfunc` package. This can be done through pip:
+Firstly, you need to install the `logfunc` package. This can be done through pip:
 
 ```sh
-pip install myfuncs
+pip install logfunc
 ```
 
 ### Importing
 
 Once the package is installed, you can import the `logf` function from the `logfunc` module:
 
 ```python
@@ -58,21 +58,34 @@
 
 ### Customize Logging
 
 The `logf` function allows you to customize your logging:
 
 - You can set the log level with the `level` parameter.
 - Use `log_args` and `log_return` parameters to choose whether to log the arguments and the return value of the function.
-- `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values.
+- `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values. If `None` is passed, the entire args/kwargs/result are logged as their full-length strings.
 - You can choose whether to measure and log the function execution time with the `measure_time` parameter.
 
 Here is an example:
 
 ```python
 from logfunc import logf
 
-@logf(level='INFO', log_args=False, log_return=True, max_str_len=500, measure_time=True)
+@logf(level='INFO', log_args=False, log_return=True,
+    max_str_len=None, measure_time=True)
 def my_function(a, b):
     return a + b
 ```
 
-In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, trims logged strings to 500 characters, and it measures and logs the execution time.
+In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, logs the entire return string without any truncation, and it measures and logs the execution time.
+
+## Testing
+
+This module comes with a test suite which you can run to ensure that `logf` behaves as expected. The tests are implemented using Python's built-in `unittest` module.
+
+To run the tests, navigate to the directory where the `logfunc` package is installed and run:
+
+```sh
+python tests.py
+```
+
+The test suite includes tests for the default behavior of the `logf` decorator as well as its behavior when custom parameters are passed. The tests check whether the function name, arguments, return value, and execution time are correctly logged, and whether the `max_str_len` parameter correctly truncates the logged strings.
```

### Comparing `logfunc-1.0.3/README.md` & `logfunc-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # logf
 
-the @logf() decorator i previously had as part of the myfuncs pip package, decided to make it standalone pip package this is the repo for it
+The `@logf()` decorator, previously a part of the myfuncs pip package, is now a standalone pip package. This repository is dedicated to its development and maintenance.
 
 ## Usage
 
-Here is a brief guide on how to use the `logfunc` module.
+This is a brief guide on how to use the `logfunc` module.
 
 ### Installation
 
-First, you need to install the `logfunc` package. This can be done through pip:
+Firstly, you need to install the `logfunc` package. This can be done through pip:
 
 ```sh
-pip install myfuncs
+pip install logfunc
 ```
 
 ### Importing
 
 Once the package is installed, you can import the `logf` function from the `logfunc` module:
 
 ```python
@@ -38,21 +38,34 @@
 
 ### Customize Logging
 
 The `logf` function allows you to customize your logging:
 
 - You can set the log level with the `level` parameter.
 - Use `log_args` and `log_return` parameters to choose whether to log the arguments and the return value of the function.
-- `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values.
+- `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values. If `None` is passed, the entire args/kwargs/result are logged as their full-length strings.
 - You can choose whether to measure and log the function execution time with the `measure_time` parameter.
 
 Here is an example:
 
 ```python
 from logfunc import logf
 
-@logf(level='INFO', log_args=False, log_return=True, max_str_len=500, measure_time=True)
+@logf(level='INFO', log_args=False, log_return=True,
+    max_str_len=None, measure_time=True)
 def my_function(a, b):
     return a + b
 ```
 
-In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, trims logged strings to 500 characters, and it measures and logs the execution time.
+In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, logs the entire return string without any truncation, and it measures and logs the execution time.
+
+## Testing
+
+This module comes with a test suite which you can run to ensure that `logf` behaves as expected. The tests are implemented using Python's built-in `unittest` module.
+
+To run the tests, navigate to the directory where the `logfunc` package is installed and run:
+
+```sh
+python tests.py
+```
+
+The test suite includes tests for the default behavior of the `logf` decorator as well as its behavior when custom parameters are passed. The tests check whether the function name, arguments, return value, and execution time are correctly logged, and whether the `max_str_len` parameter correctly truncates the logged strings.
```

### Comparing `logfunc-1.0.3/logfunc/__init__.py` & `logfunc-1.1.0/logfunc/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,92 +11,97 @@
 import logging
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T", bound=Callable[..., Any])
 
 
-def trunc_str(string: str, max_length: int) -> str:
+def trunc_str(string: str, max_length: Optional[int] = 1000) -> str:
     """
     Truncates a string if its length exceeds the specified maximum length.
-    If the string is truncated, it appends '...' to indicate the truncation.
+    If the string is truncated, it appends '...' to indicate the truncation. If
+    no max_length is specified, the string is returned as-is.
 
     Args:
         string (str): The string to truncate.
-        max_length (int): The maximum length of the truncated string.
+        max_length (int): The maximum length of the truncated string. Defaults to 1000.
 
     Returns:
         str: The truncated string.
     """
+    if max_length is None: # None was explictly passed as an arg, return str as-is
+        return string
+
     if len(string) > max_length:
-        return string[:max_length - 3] + "..."
+        return string[:max_length - 3] + '...'
     return string
 
 
 def logf(
     level: Optional[Union[int, str]] = logging.DEBUG,
     log_args: bool = True,
     log_return: bool = True,
-    max_str_len: int = 1000,
-    measure_time: bool = True
+    max_str_len: Optional[int] = 1000,
+    log_exec_time: bool = True,
+    **kwargs
 ) -> Callable[[T], T]:
     """
     A decorator that logs the execution time, function name, arguments, keyword arguments,
     and return value of a function using a specified log level.
 
     Args:
         level (Union[int, str], optional): The log level to use for logging. Defaults to logging.DEBUG.
         log_args (bool, optional): Should the function arguments be logged? Defaults to True.
         log_return (bool, optional): Should function return be logged? Defaults to True.
-        max_str_len (int, optional): Maximum length of the logged arguments and return values. Defaults to 1000.
-        measure_time (bool, optional): Should the function execution time be measured? Defaults to True.
+        max_str_len (Optional[int]): Maximum length of the logged arguments and return values. Defaults to 1000.
+        log_exec_time (bool, optional): Should the function execution time be measured? Defaults to True.
 
     Returns:
         Callable[[T], T]: The wrapped function.
     """
     if isinstance(level, str):
         level_int = logging.getLevelName(level.upper())
     else:
         level_int = int(level)
 
+    # for backwards compatability, override log_exec_time using
+    # the measure_time kwarg if present
+    if 'measure_time' in kwargs:
+        log_exec_time = kwargs['measure_time']
+
     def decorator(func: T) -> T:
         @wraps(func)
-        def wrapper(*args: Any, **kwargs: Any) -> Any:
+        def wrapper(*args, **kwargs):
             # Start the timer if required and execute the function.
-            start_time = time.time() if measure_time else None
+            start_time = time.time() if log_exec_time else None
+
+            fname = f'{func.__name__}()' # shorthand reference
 
             # Log function arguments if required
             if log_args:
-                arg_str = f"{func.__name__}() | {str(args)[:max_str_len]} {str(kwargs)[:max_str_len]}"
+                argstr = f'{trunc_str(str(args), max_str_len)} {trunc_str(str(kwargs), max_str_len)}'
+                logmsg_enter = f'{fname} | {argstr}'
             else:
-                arg_str = f"{func.__name__}()"
+                logmsg_enter = fname # only log function name on entry
 
-            logger.log(level_int, arg_str)
+            logger.log(level_int, logmsg_enter)
 
             # Execute the function
             result = func(*args, **kwargs)
 
-            if measure_time:
-                end_time = time.time()
-                # Calculate the execution time and format the log message.
-                exec_time = end_time - start_time
-                exec_time_str = f"{exec_time:.5f}s"
-
-            # Log the return value and execution time if required
-            if log_return and measure_time:
-                result_str = trunc_str(str(result), max_str_len)
-                log_message = f"{func.__name__}() {exec_time_str} | {result_str}"
-            elif log_return:
-                result_str = trunc_str(str(result), max_str_len)
-                log_message = f"{func.__name__}() | {result_str}"
-            elif measure_time:
-                log_message = f"{func.__name__}() {exec_time_str}"
+            # include execution time if log_exec_time=True
+            if log_exec_time:
+                exec_time = time.time() - start_time
+                logmsg_exit = f'{fname} {exec_time:.5f}s'
             else:
-                log_message = None
+                logmsg_exit = fname # only use func name
+
+            # if log_return=True include returned obj str in logmsg
+            if log_return:
+                logmsg_exit = f'{logmsg_exit} | {trunc_str(str(result), max_str_len)}'
 
-            if log_message is not None:
-                # Log the message using the specified level.
-                logger.log(level_int, log_message)
+            # Log the return value and execution time if required
+            logger.log(level_int, logmsg_exit)
 
             return result
         return wrapper
     return decorator
```

### Comparing `logfunc-1.0.3/logfunc.egg-info/PKG-INFO` & `logfunc-1.1.0/logfunc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.0.3
+Version: 1.1.0
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/tree/main
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,26 +16,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # logf
 
-the @logf() decorator i previously had as part of the myfuncs pip package, decided to make it standalone pip package this is the repo for it
+The `@logf()` decorator, previously a part of the myfuncs pip package, is now a standalone pip package. This repository is dedicated to its development and maintenance.
 
 ## Usage
 
-Here is a brief guide on how to use the `logfunc` module.
+This is a brief guide on how to use the `logfunc` module.
 
 ### Installation
 
-First, you need to install the `logfunc` package. This can be done through pip:
+Firstly, you need to install the `logfunc` package. This can be done through pip:
 
 ```sh
-pip install myfuncs
+pip install logfunc
 ```
 
 ### Importing
 
 Once the package is installed, you can import the `logf` function from the `logfunc` module:
 
 ```python
@@ -58,21 +58,34 @@
 
 ### Customize Logging
 
 The `logf` function allows you to customize your logging:
 
 - You can set the log level with the `level` parameter.
 - Use `log_args` and `log_return` parameters to choose whether to log the arguments and the return value of the function.
-- `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values.
+- `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values. If `None` is passed, the entire args/kwargs/result are logged as their full-length strings.
 - You can choose whether to measure and log the function execution time with the `measure_time` parameter.
 
 Here is an example:
 
 ```python
 from logfunc import logf
 
-@logf(level='INFO', log_args=False, log_return=True, max_str_len=500, measure_time=True)
+@logf(level='INFO', log_args=False, log_return=True,
+    max_str_len=None, measure_time=True)
 def my_function(a, b):
     return a + b
 ```
 
-In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, trims logged strings to 500 characters, and it measures and logs the execution time.
+In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, logs the entire return string without any truncation, and it measures and logs the execution time.
+
+## Testing
+
+This module comes with a test suite which you can run to ensure that `logf` behaves as expected. The tests are implemented using Python's built-in `unittest` module.
+
+To run the tests, navigate to the directory where the `logfunc` package is installed and run:
+
+```sh
+python tests.py
+```
+
+The test suite includes tests for the default behavior of the `logf` decorator as well as its behavior when custom parameters are passed. The tests check whether the function name, arguments, return value, and execution time are correctly logged, and whether the `max_str_len` parameter correctly truncates the logged strings.
```

### Comparing `logfunc-1.0.3/setup.py` & `logfunc-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='logfunc',
-    version='1.0.3',
+    version='1.1.0',
     packages=find_packages(),
     install_requires=[],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description='An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

