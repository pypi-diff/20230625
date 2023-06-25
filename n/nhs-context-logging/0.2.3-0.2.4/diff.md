# Comparing `tmp/nhs_context_logging-0.2.3.tar.gz` & `tmp/nhs_context_logging-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhs_context_logging-0.2.3.tar", max compression
+gzip compressed data, was "nhs_context_logging-0.2.4.tar", max compression
```

## Comparing `nhs_context_logging-0.2.3.tar` & `nhs_context_logging-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1159 2023-06-25 21:05:32.135245 nhs_context_logging-0.2.3/LICENSE.md
--rw-r--r--   0        0        0     8193 2023-06-25 21:05:32.135245 nhs_context_logging-0.2.3/README.md
--rw-r--r--   0        0        0     1636 2023-06-25 21:05:49.443689 nhs_context_logging-0.2.3/nhs_context_logging/__init__.py
--rw-r--r--   0        0        0     1446 2023-06-25 21:05:32.139245 nhs_context_logging-0.2.3/nhs_context_logging/constants.py
--rw-r--r--   0        0        0     1076 2023-06-25 21:05:32.139245 nhs_context_logging-0.2.3/nhs_context_logging/fixtures.py
--rw-r--r--   0        0        0     5954 2023-06-25 21:05:32.139245 nhs_context_logging-0.2.3/nhs_context_logging/formatters.py
--rw-r--r--   0        0        0     1685 2023-06-25 21:05:32.139245 nhs_context_logging-0.2.3/nhs_context_logging/handlers.py
--rw-r--r--   0        0        0    34864 2023-06-25 21:05:32.139245 nhs_context_logging-0.2.3/nhs_context_logging/logger.py
--rw-r--r--   0        0        0        0 2023-06-25 21:05:32.139245 nhs_context_logging-0.2.3/nhs_context_logging/py.typed
--rw-r--r--   0        0        0     3830 2023-06-25 21:05:32.139245 nhs_context_logging-0.2.3/nhs_context_logging/utils.py
--rw-r--r--   0        0        0     2809 2023-06-25 21:05:49.439689 nhs_context_logging-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 21:05:32.139245 nhs_context_logging-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      486 2023-06-25 21:05:32.139245 nhs_context_logging-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0    36874 2023-06-25 21:05:32.139245 nhs_context_logging-0.2.3/tests/logger_tests.py
--rw-r--r--   0        0        0     4214 2023-06-25 21:05:32.139245 nhs_context_logging-0.2.3/tests/utils.py
--rw-r--r--   0        0        0     8615 1970-01-01 00:00:00.000000 nhs_context_logging-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1159 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0     7970 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/README.md
+-rw-r--r--   0        0        0     1636 2023-06-25 21:14:44.034891 nhs_context_logging-0.2.4/nhs_context_logging/__init__.py
+-rw-r--r--   0        0        0     1446 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/constants.py
+-rw-r--r--   0        0        0     1076 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/fixtures.py
+-rw-r--r--   0        0        0     5954 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/formatters.py
+-rw-r--r--   0        0        0     1685 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/handlers.py
+-rw-r--r--   0        0        0    34864 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/logger.py
+-rw-r--r--   0        0        0        0 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/py.typed
+-rw-r--r--   0        0        0     3830 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/utils.py
+-rw-r--r--   0        0        0     2809 2023-06-25 21:14:44.030891 nhs_context_logging-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 21:14:22.802491 nhs_context_logging-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      486 2023-06-25 21:14:22.802491 nhs_context_logging-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0    36874 2023-06-25 21:14:22.802491 nhs_context_logging-0.2.4/tests/logger_tests.py
+-rw-r--r--   0        0        0     4214 2023-06-25 21:14:22.802491 nhs_context_logging-0.2.4/tests/utils.py
+-rw-r--r--   0        0        0     8392 1970-01-01 00:00:00.000000 nhs_context_logging-0.2.4/PKG-INFO
```

### Comparing `nhs_context_logging-0.2.3/LICENSE.md` & `nhs_context_logging-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.3/README.md` & `nhs_context_logging-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 
 # quick start
 
 ### contributing
 contributors see [contributing](CONTRIBUTING.md)
 
 ### installing
-install using git + https
-see [releases](https://github.com/NHSDigital/nhs-context-logging/releases) for the latest release
+
 ```shell
-pip install https://github.com/NHSDigital/nhs-context-logging/releases/download/v0.1.13/nhs_context_logging-0.1.13-py3-none-any.whl
+pip install nhs-context-logging
 ```
 
 ### logging
 out of the box this framework will create structured logs with some default behaviours that we think work well
 
 ```python
 from nhs_context_logging import app_logger, log_action
```

### Comparing `nhs_context_logging-0.2.3/nhs_context_logging/__init__.py` & `nhs_context_logging-0.2.4/nhs_context_logging/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nhs_context_logging.logger import (
     LogActionContextManager,
     TemporaryGlobalFieldsContextManager,
 )
 from nhs_context_logging.logger import app_logger as _app_logger
 from nhs_context_logging.logger import logging_context
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 DEFAULT_LOG_LEVEL = Constants.DEFAULT_LOG_LEVEL
 LOG_AT_LEVEL = Constants.LOG_AT_LEVEL
 LOG_LEVEL = Constants.LOG_LEVEL
 
 CRITICAL = _app_logger.CRITICAL
 FATAL = _app_logger.FATAL
```

### Comparing `nhs_context_logging-0.2.3/nhs_context_logging/constants.py` & `nhs_context_logging-0.2.4/nhs_context_logging/constants.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.3/nhs_context_logging/fixtures.py` & `nhs_context_logging-0.2.4/nhs_context_logging/fixtures.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.3/nhs_context_logging/formatters.py` & `nhs_context_logging-0.2.4/nhs_context_logging/formatters.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.3/nhs_context_logging/handlers.py` & `nhs_context_logging-0.2.4/nhs_context_logging/handlers.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.3/nhs_context_logging/logger.py` & `nhs_context_logging-0.2.4/nhs_context_logging/logger.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.3/nhs_context_logging/utils.py` & `nhs_context_logging-0.2.4/nhs_context_logging/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.3/pyproject.toml` & `nhs_context_logging-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhs_context_logging"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["spinecore"]
 license = "GPLv3"
 packages = [
     { include = "nhs_context_logging" },
     { include = "tests", format = "sdist" },
 ]
```

### Comparing `nhs_context_logging-0.2.3/tests/logger_tests.py` & `nhs_context_logging-0.2.4/tests/logger_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.3/tests/utils.py` & `nhs_context_logging-0.2.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.3/PKG-INFO` & `nhs_context_logging-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhs-context-logging
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 License: GPLv3
 Author: spinecore
 Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -19,18 +19,17 @@
 
 # quick start
 
 ### contributing
 contributors see [contributing](CONTRIBUTING.md)
 
 ### installing
-install using git + https
-see [releases](https://github.com/NHSDigital/nhs-context-logging/releases) for the latest release
+
 ```shell
-pip install https://github.com/NHSDigital/nhs-context-logging/releases/download/v0.1.13/nhs_context_logging-0.1.13-py3-none-any.whl
+pip install nhs-context-logging
 ```
 
 ### logging
 out of the box this framework will create structured logs with some default behaviours that we think work well
 
 ```python
 from nhs_context_logging import app_logger, log_action
```

