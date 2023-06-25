# Comparing `tmp/pytest-playwright-async-0.0.6.tar.gz` & `tmp/pytest-playwright-async-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-playwright-async-0.0.6.tar", last modified: Sun Jun 25 15:59:05 2023, max compression
+gzip compressed data, was "pytest-playwright-async-0.0.7.tar", last modified: Sun Jun 25 20:43:23 2023, max compression
```

## Comparing `pytest-playwright-async-0.0.6.tar` & `pytest-playwright-async-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:59:05.620319 pytest-playwright-async-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-25 15:59:05.620319 pytest-playwright-async-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-25 15:58:45.000000 pytest-playwright-async-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-25 15:58:45.000000 pytest-playwright-async-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 15:59:05.620319 pytest-playwright-async-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:59:05.616319 pytest-playwright-async-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:45.000000 pytest-playwright-async-0.0.6/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:59:05.616319 pytest-playwright-async-0.0.6/src/pytest_playwright_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-25 15:59:05.000000 pytest-playwright-async-0.0.6/src/pytest_playwright_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-25 15:59:05.000000 pytest-playwright-async-0.0.6/src/pytest_playwright_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:59:05.000000 pytest-playwright-async-0.0.6/src/pytest_playwright_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 15:59:05.000000 pytest-playwright-async-0.0.6/src/pytest_playwright_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-25 15:59:05.000000 pytest-playwright-async-0.0.6/src/pytest_playwright_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-25 15:59:05.000000 pytest-playwright-async-0.0.6/src/pytest_playwright_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-25 15:58:45.000000 pytest-playwright-async-0.0.6/src/pytest_playwright_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:59:05.620319 pytest-playwright-async-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-25 15:58:45.000000 pytest-playwright-async-0.0.6/tests/test_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:43:23.937043 pytest-playwright-async-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-25 20:43:23.937043 pytest-playwright-async-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-25 20:43:08.000000 pytest-playwright-async-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-25 20:43:08.000000 pytest-playwright-async-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 20:43:23.937043 pytest-playwright-async-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:43:23.937043 pytest-playwright-async-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 20:43:08.000000 pytest-playwright-async-0.0.7/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:43:23.937043 pytest-playwright-async-0.0.7/src/pytest_playwright_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-25 20:43:23.000000 pytest-playwright-async-0.0.7/src/pytest_playwright_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-25 20:43:23.000000 pytest-playwright-async-0.0.7/src/pytest_playwright_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 20:43:23.000000 pytest-playwright-async-0.0.7/src/pytest_playwright_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 20:43:23.000000 pytest-playwright-async-0.0.7/src/pytest_playwright_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-25 20:43:23.000000 pytest-playwright-async-0.0.7/src/pytest_playwright_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-25 20:43:23.000000 pytest-playwright-async-0.0.7/src/pytest_playwright_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-25 20:43:08.000000 pytest-playwright-async-0.0.7/src/pytest_playwright_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:43:23.937043 pytest-playwright-async-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-25 20:43:08.000000 pytest-playwright-async-0.0.7/tests/test_playwright.py
```

### Comparing `pytest-playwright-async-0.0.6/PKG-INFO` & `pytest-playwright-async-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: pytest-playwright-async
-Version: 0.0.6
+Version: 0.0.7
 Summary: ASYNC Pytest plugin for Playwright
 Author-email: m9810223 <m9810223@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/m9810223/playwright-async-pytest
 Project-URL: Source, https://github.com/m9810223/playwright-async-pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # ASYNC Pytest plugin for Playwright [![PyPI](https://img.shields.io/pypi/v/pytest-playwright-async)](https://pypi.org/project/pytest-playwright-async/)
 
+There an official playwright plugin for pytest: [PyPI](https://pypi.org/project/pytest-playwright/) / [playwright-pytest](https://github.com/microsoft/playwright-pytest) / [intro](https://playwright.dev/python/docs/intro).
+But if you need an async version, here is it!
+
 ## Installation
 
 ```shell
 pip install pytest-playwright-async
 ```
 
 ## Example
 
+[Here](https://github.com/m9810223/playwright-async-pytest/blob/master/tests/test_playwright.py) you can find more examples.
+
 ```py
 # conftest.py
 import asyncio
 
 import pytest_asyncio
```

### Comparing `pytest-playwright-async-0.0.6/README.md` & `pytest-playwright-async-0.0.7/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # ASYNC Pytest plugin for Playwright [![PyPI](https://img.shields.io/pypi/v/pytest-playwright-async)](https://pypi.org/project/pytest-playwright-async/)
 
+There an official playwright plugin for pytest: [PyPI](https://pypi.org/project/pytest-playwright/) / [playwright-pytest](https://github.com/microsoft/playwright-pytest) / [intro](https://playwright.dev/python/docs/intro).
+But if you need an async version, here is it!
+
 ## Installation
 
 ```shell
 pip install pytest-playwright-async
 ```
 
 ## Example
 
+[Here](https://github.com/m9810223/playwright-async-pytest/blob/master/tests/test_playwright.py) you can find more examples.
+
 ```py
 # conftest.py
 import asyncio
 
 import pytest_asyncio
```

### Comparing `pytest-playwright-async-0.0.6/pyproject.toml` & `pytest-playwright-async-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "pytest-asyncio==0.20.3", # https://github.com/microsoft/playwright-python/blob/main/local-requirements.txt
 ]
 description = "ASYNC Pytest plugin for Playwright"
 license = {text = "MIT"}
 name = "pytest-playwright-async"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.0.6"
+version = "0.0.7"
 
 [project.urls]
 Homepage = "https://github.com/m9810223/playwright-async-pytest"
 Source = "https://github.com/m9810223/playwright-async-pytest"
 
 [project.entry-points.pytest11]
 playwright_async = "pytest_playwright_async"
```

### Comparing `pytest-playwright-async-0.0.6/src/pytest_playwright_async.egg-info/PKG-INFO` & `pytest-playwright-async-0.0.7/src/pytest_playwright_async.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: pytest-playwright-async
-Version: 0.0.6
+Version: 0.0.7
 Summary: ASYNC Pytest plugin for Playwright
 Author-email: m9810223 <m9810223@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/m9810223/playwright-async-pytest
 Project-URL: Source, https://github.com/m9810223/playwright-async-pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # ASYNC Pytest plugin for Playwright [![PyPI](https://img.shields.io/pypi/v/pytest-playwright-async)](https://pypi.org/project/pytest-playwright-async/)
 
+There an official playwright plugin for pytest: [PyPI](https://pypi.org/project/pytest-playwright/) / [playwright-pytest](https://github.com/microsoft/playwright-pytest) / [intro](https://playwright.dev/python/docs/intro).
+But if you need an async version, here is it!
+
 ## Installation
 
 ```shell
 pip install pytest-playwright-async
 ```
 
 ## Example
 
+[Here](https://github.com/m9810223/playwright-async-pytest/blob/master/tests/test_playwright.py) you can find more examples.
+
 ```py
 # conftest.py
 import asyncio
 
 import pytest_asyncio
```

### Comparing `pytest-playwright-async-0.0.6/src/pytest_playwright_async.py` & `pytest-playwright-async-0.0.7/src/pytest_playwright_async.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-async-0.0.6/tests/test_playwright.py` & `pytest-playwright-async-0.0.7/tests/test_playwright.py`

 * *Files identical despite different names*

