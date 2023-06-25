# Comparing `tmp/pytest-playwright-async-0.0.4.tar.gz` & `tmp/pytest-playwright-async-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-playwright-async-0.0.4.tar", last modified: Sun Jun 25 13:22:06 2023, max compression
+gzip compressed data, was "pytest-playwright-async-0.0.5.tar", last modified: Sun Jun 25 13:31:58 2023, max compression
```

## Comparing `pytest-playwright-async-0.0.4.tar` & `pytest-playwright-async-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:22:06.401234 pytest-playwright-async-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-25 13:22:06.401234 pytest-playwright-async-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-25 13:21:49.000000 pytest-playwright-async-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-25 13:21:49.000000 pytest-playwright-async-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 13:22:06.401234 pytest-playwright-async-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:22:06.397234 pytest-playwright-async-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 13:21:49.000000 pytest-playwright-async-0.0.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:22:06.401234 pytest-playwright-async-0.0.4/src/pytest_playwright_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-25 13:22:06.000000 pytest-playwright-async-0.0.4/src/pytest_playwright_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-25 13:22:06.000000 pytest-playwright-async-0.0.4/src/pytest_playwright_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 13:22:06.000000 pytest-playwright-async-0.0.4/src/pytest_playwright_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 13:22:06.000000 pytest-playwright-async-0.0.4/src/pytest_playwright_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-25 13:22:06.000000 pytest-playwright-async-0.0.4/src/pytest_playwright_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-25 13:22:06.000000 pytest-playwright-async-0.0.4/src/pytest_playwright_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-25 13:21:49.000000 pytest-playwright-async-0.0.4/src/pytest_playwright_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:22:06.401234 pytest-playwright-async-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-25 13:21:49.000000 pytest-playwright-async-0.0.4/tests/test_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:31:58.890817 pytest-playwright-async-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-25 13:31:58.890817 pytest-playwright-async-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-25 13:31:35.000000 pytest-playwright-async-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-25 13:31:35.000000 pytest-playwright-async-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 13:31:58.890817 pytest-playwright-async-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:31:58.890817 pytest-playwright-async-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 13:31:35.000000 pytest-playwright-async-0.0.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:31:58.890817 pytest-playwright-async-0.0.5/src/pytest_playwright_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-25 13:31:58.000000 pytest-playwright-async-0.0.5/src/pytest_playwright_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-25 13:31:58.000000 pytest-playwright-async-0.0.5/src/pytest_playwright_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 13:31:58.000000 pytest-playwright-async-0.0.5/src/pytest_playwright_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 13:31:58.000000 pytest-playwright-async-0.0.5/src/pytest_playwright_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-25 13:31:58.000000 pytest-playwright-async-0.0.5/src/pytest_playwright_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-25 13:31:58.000000 pytest-playwright-async-0.0.5/src/pytest_playwright_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-25 13:31:35.000000 pytest-playwright-async-0.0.5/src/pytest_playwright_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:31:58.890817 pytest-playwright-async-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-25 13:31:35.000000 pytest-playwright-async-0.0.5/tests/test_playwright.py
```

### Comparing `pytest-playwright-async-0.0.4/PKG-INFO` & `pytest-playwright-async-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-playwright-async
-Version: 0.0.4
+Version: 0.0.5
 Summary: ASYNC Pytest plugin for Playwright
 Author-email: m9810223 <m9810223@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/m9810223/playwright-async-pytest
 Project-URL: Source, https://github.com/m9810223/playwright-async-pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pytest-playwright-async-0.0.4/README.md` & `pytest-playwright-async-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-async-0.0.4/pyproject.toml` & `pytest-playwright-async-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "pytest-asyncio==0.20.3", # https://github.com/microsoft/playwright-python/blob/main/local-requirements.txt
 ]
 description = "ASYNC Pytest plugin for Playwright"
 license = {text = "MIT"}
 name = "pytest-playwright-async"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.0.4"
+version = "0.0.5"
 
 [project.urls]
 Homepage = "https://github.com/m9810223/playwright-async-pytest"
 Source = "https://github.com/m9810223/playwright-async-pytest"
 
 [project.entry-points.pytest11]
 playwright_async = "pytest_playwright_async"
```

### Comparing `pytest-playwright-async-0.0.4/src/pytest_playwright_async.egg-info/PKG-INFO` & `pytest-playwright-async-0.0.5/src/pytest_playwright_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-playwright-async
-Version: 0.0.4
+Version: 0.0.5
 Summary: ASYNC Pytest plugin for Playwright
 Author-email: m9810223 <m9810223@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/m9810223/playwright-async-pytest
 Project-URL: Source, https://github.com/m9810223/playwright-async-pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pytest-playwright-async-0.0.4/src/pytest_playwright_async.py` & `pytest-playwright-async-0.0.5/src/pytest_playwright_async.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-async-0.0.4/tests/test_playwright.py` & `pytest-playwright-async-0.0.5/tests/test_playwright.py`

 * *Files identical despite different names*

