# Comparing `tmp/logfunc-1.1.1.tar.gz` & `tmp/logfunc-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfunc-1.1.1.tar", last modified: Sun Jun 25 00:37:58 2023, max compression
+gzip compressed data, was "logfunc-1.2.0.tar", last modified: Sun Jun 25 17:49:24 2023, max compression
```

## Comparing `logfunc-1.1.1.tar` & `logfunc-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-25 00:37:58.126246 logfunc-1.1.1/
--rw-r--r--   0 work       (501) staff       (20)     1068 2023-06-23 16:56:28.000000 logfunc-1.1.1/LICENSE
--rw-r--r--   0 work       (501) staff       (20)     3328 2023-06-25 00:37:58.126123 logfunc-1.1.1/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     2514 2023-06-25 00:37:16.000000 logfunc-1.1.1/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-25 00:37:58.125517 logfunc-1.1.1/logfunc/
--rw-r--r--   0 work       (501) staff       (20)     3781 2023-06-25 00:37:18.000000 logfunc-1.1.1/logfunc/__init__.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-25 00:37:58.125978 logfunc-1.1.1/logfunc.egg-info/
--rw-r--r--   0 work       (501) staff       (20)     3328 2023-06-25 00:37:58.000000 logfunc-1.1.1/logfunc.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      170 2023-06-25 00:37:58.000000 logfunc-1.1.1/logfunc.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-06-25 00:37:58.000000 logfunc-1.1.1/logfunc.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)        8 2023-06-25 00:37:58.000000 logfunc-1.1.1/logfunc.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       38 2023-06-25 00:37:58.126292 logfunc-1.1.1/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)     1071 2023-06-25 00:37:40.000000 logfunc-1.1.1/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-25 17:49:24.485170 logfunc-1.2.0/
+-rw-r--r--   0 work       (501) staff       (20)     1068 2023-06-23 16:56:28.000000 logfunc-1.2.0/LICENSE
+-rw-r--r--   0 work       (501) staff       (20)     3581 2023-06-25 17:49:24.485051 logfunc-1.2.0/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     2716 2023-06-25 17:48:43.000000 logfunc-1.2.0/README.md
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-25 17:49:24.484419 logfunc-1.2.0/logfunc/
+-rw-r--r--   0 work       (501) staff       (20)     4245 2023-06-25 17:34:56.000000 logfunc-1.2.0/logfunc/__init__.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-25 17:49:24.484883 logfunc-1.2.0/logfunc.egg-info/
+-rw-r--r--   0 work       (501) staff       (20)     3581 2023-06-25 17:49:24.000000 logfunc-1.2.0/logfunc.egg-info/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)      170 2023-06-25 17:49:24.000000 logfunc-1.2.0/logfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (501) staff       (20)        1 2023-06-25 17:49:24.000000 logfunc-1.2.0/logfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (501) staff       (20)        8 2023-06-25 17:49:24.000000 logfunc-1.2.0/logfunc.egg-info/top_level.txt
+-rw-r--r--   0 work       (501) staff       (20)       38 2023-06-25 17:49:24.485208 logfunc-1.2.0/setup.cfg
+-rw-r--r--   0 work       (501) staff       (20)     1121 2023-06-25 17:46:53.000000 logfunc-1.2.0/setup.py
```

### Comparing `logfunc-1.1.1/LICENSE` & `logfunc-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfunc-1.1.1/PKG-INFO` & `logfunc-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.1.1
+Version: 1.2.0
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/tree/main
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # logf
 
 The `@logf()` decorator, previously a part of the myfuncs pip package, is now a standalone pip package. This repository is dedicated to its development and maintenance.
 
@@ -60,27 +61,28 @@
 
 The `logf` function allows you to customize your logging:
 
 - You can set the log level with the `level` parameter.
 - Use `log_args` and `log_return` parameters to choose whether to log the arguments and the return value of the function.
 - `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values. If `None` is passed, the entire args/kwargs/result are logged as their full-length strings.
 - You can choose whether to measure and log the function execution time with the `log_exec_time` parameter.
+- You can include the execution time, args, and return value in a single message with the `single_msg` parameter.
 
 Here is an example:
 
 ```python
 from logfunc import logf
 
 @logf(level='INFO', log_args=False, log_return=True,
-    max_str_len=None, log_exec_time=True)
+    max_str_len=None, log_exec_time=True, single_msg=True)
 def my_function(a, b):
     return a + b
 ```
 
-In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, logs the entire return string without any truncation, and it measures and logs the execution time.
+In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, logs the entire return string without any truncation, and it measures and logs the execution time, and it only uses a single log message as opposed to two on enter/exit.
 
 ## Testing
 
 This module comes with a test suite which you can run to ensure that `logf` behaves as expected. The tests are implemented using Python's built-in `unittest` module.
 
 To run the tests, navigate to the directory where the `logfunc` package is installed and run:
```

### Comparing `logfunc-1.1.1/README.md` & `logfunc-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -40,27 +40,28 @@
 
 The `logf` function allows you to customize your logging:
 
 - You can set the log level with the `level` parameter.
 - Use `log_args` and `log_return` parameters to choose whether to log the arguments and the return value of the function.
 - `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values. If `None` is passed, the entire args/kwargs/result are logged as their full-length strings.
 - You can choose whether to measure and log the function execution time with the `log_exec_time` parameter.
+- You can include the execution time, args, and return value in a single message with the `single_msg` parameter.
 
 Here is an example:
 
 ```python
 from logfunc import logf
 
 @logf(level='INFO', log_args=False, log_return=True,
-    max_str_len=None, log_exec_time=True)
+    max_str_len=None, log_exec_time=True, single_msg=True)
 def my_function(a, b):
     return a + b
 ```
 
-In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, logs the entire return string without any truncation, and it measures and logs the execution time.
+In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, logs the entire return string without any truncation, and it measures and logs the execution time, and it only uses a single log message as opposed to two on enter/exit.
 
 ## Testing
 
 This module comes with a test suite which you can run to ensure that `logf` behaves as expected. The tests are implemented using Python's built-in `unittest` module.
 
 To run the tests, navigate to the directory where the `logfunc` package is installed and run:
```

### Comparing `logfunc-1.1.1/logfunc.egg-info/PKG-INFO` & `logfunc-1.2.0/logfunc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.1.1
+Version: 1.2.0
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/tree/main
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # logf
 
 The `@logf()` decorator, previously a part of the myfuncs pip package, is now a standalone pip package. This repository is dedicated to its development and maintenance.
 
@@ -60,27 +61,28 @@
 
 The `logf` function allows you to customize your logging:
 
 - You can set the log level with the `level` parameter.
 - Use `log_args` and `log_return` parameters to choose whether to log the arguments and the return value of the function.
 - `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values. If `None` is passed, the entire args/kwargs/result are logged as their full-length strings.
 - You can choose whether to measure and log the function execution time with the `log_exec_time` parameter.
+- You can include the execution time, args, and return value in a single message with the `single_msg` parameter.
 
 Here is an example:
 
 ```python
 from logfunc import logf
 
 @logf(level='INFO', log_args=False, log_return=True,
-    max_str_len=None, log_exec_time=True)
+    max_str_len=None, log_exec_time=True, single_msg=True)
 def my_function(a, b):
     return a + b
 ```
 
-In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, logs the entire return string without any truncation, and it measures and logs the execution time.
+In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, logs the entire return string without any truncation, and it measures and logs the execution time, and it only uses a single log message as opposed to two on enter/exit.
 
 ## Testing
 
 This module comes with a test suite which you can run to ensure that `logf` behaves as expected. The tests are implemented using Python's built-in `unittest` module.
 
 To run the tests, navigate to the directory where the `logfunc` package is installed and run:
```

### Comparing `logfunc-1.1.1/setup.py` & `logfunc-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='logfunc',
-    version='1.1.1',
+    version='1.2.0',
     packages=find_packages(),
     install_requires=[],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description='An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -22,9 +22,10 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

