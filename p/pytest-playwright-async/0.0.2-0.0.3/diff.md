# Comparing `tmp/pytest-playwright-async-0.0.2.tar.gz` & `tmp/pytest-playwright-async-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-playwright-async-0.0.2.tar", last modified: Sun Jun 25 12:02:54 2023, max compression
+gzip compressed data, was "pytest-playwright-async-0.0.3.tar", last modified: Sun Jun 25 12:24:29 2023, max compression
```

## Comparing `pytest-playwright-async-0.0.2.tar` & `pytest-playwright-async-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-25 12:02:54.928639 pytest-playwright-async-0.0.2/
--rw-r--r--   0 michael    (501) staff       (20)      385 2023-06-25 12:02:54.928510 pytest-playwright-async-0.0.2/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      153 2023-06-25 11:52:50.000000 pytest-playwright-async-0.0.2/README.md
--rw-r--r--   0 michael    (501) staff       (20)     1299 2023-06-25 12:00:58.000000 pytest-playwright-async-0.0.2/pyproject.toml
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-25 12:02:54.928687 pytest-playwright-async-0.0.2/setup.cfg
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-25 12:02:54.927003 pytest-playwright-async-0.0.2/src/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-06-25 08:46:36.000000 pytest-playwright-async-0.0.2/src/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-25 12:02:54.927987 pytest-playwright-async-0.0.2/src/pytest_playwright_async.egg-info/
--rw-rw-rw-   0 michael    (501) staff       (20)      385 2023-06-25 12:02:54.000000 pytest-playwright-async-0.0.2/src/pytest_playwright_async.egg-info/PKG-INFO
--rw-rw-rw-   0 michael    (501) staff       (20)      404 2023-06-25 12:02:54.000000 pytest-playwright-async-0.0.2/src/pytest_playwright_async.egg-info/SOURCES.txt
--rw-rw-rw-   0 michael    (501) staff       (20)        1 2023-06-25 12:02:54.000000 pytest-playwright-async-0.0.2/src/pytest_playwright_async.egg-info/dependency_links.txt
--rw-rw-rw-   0 michael    (501) staff       (20)       54 2023-06-25 12:02:54.000000 pytest-playwright-async-0.0.2/src/pytest_playwright_async.egg-info/entry_points.txt
--rw-rw-rw-   0 michael    (501) staff       (20)       48 2023-06-25 12:02:54.000000 pytest-playwright-async-0.0.2/src/pytest_playwright_async.egg-info/requires.txt
--rw-rw-rw-   0 michael    (501) staff       (20)       33 2023-06-25 12:02:54.000000 pytest-playwright-async-0.0.2/src/pytest_playwright_async.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)     5958 2023-06-25 11:39:57.000000 pytest-playwright-async-0.0.2/src/pytest_playwright_async.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-25 12:02:54.928128 pytest-playwright-async-0.0.2/tests/
--rw-r--r--   0 michael    (501) staff       (20)     4759 2023-06-25 11:36:42.000000 pytest-playwright-async-0.0.2/tests/test_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:24:29.987428 pytest-playwright-async-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-25 12:24:29.987428 pytest-playwright-async-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-25 12:24:11.000000 pytest-playwright-async-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-25 12:24:11.000000 pytest-playwright-async-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 12:24:29.987428 pytest-playwright-async-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:24:29.983428 pytest-playwright-async-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 12:24:11.000000 pytest-playwright-async-0.0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:24:29.983428 pytest-playwright-async-0.0.3/src/pytest_playwright_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-25 12:24:29.000000 pytest-playwright-async-0.0.3/src/pytest_playwright_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-25 12:24:29.000000 pytest-playwright-async-0.0.3/src/pytest_playwright_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 12:24:29.000000 pytest-playwright-async-0.0.3/src/pytest_playwright_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 12:24:29.000000 pytest-playwright-async-0.0.3/src/pytest_playwright_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-25 12:24:29.000000 pytest-playwright-async-0.0.3/src/pytest_playwright_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-25 12:24:29.000000 pytest-playwright-async-0.0.3/src/pytest_playwright_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-25 12:24:11.000000 pytest-playwright-async-0.0.3/src/pytest_playwright_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:24:29.987428 pytest-playwright-async-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-25 12:24:11.000000 pytest-playwright-async-0.0.3/tests/test_playwright.py
```

### Comparing `pytest-playwright-async-0.0.2/pyproject.toml` & `pytest-playwright-async-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "pytest-asyncio==0.20.3", # https://github.com/microsoft/playwright-python/blob/main/local-requirements.txt
 ]
 description = "ASYNC Pytest plugin for Playwright"
 license = {text = "MIT"}
 name = "pytest-playwright-async"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.0.2"
+version = "0.0.3"
 
 # [project.urls]
 # Homepage = "https://github.com/m9810223/playwright-async-pytest"
 # Source = "https://github.com/m9810223/playwright-async-pytest"
 
 [project.entry-points.pytest11]
 playwright_async = "pytest_playwright_async"
```

### Comparing `pytest-playwright-async-0.0.2/src/pytest_playwright_async.py` & `pytest-playwright-async-0.0.3/src/pytest_playwright_async.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-async-0.0.2/tests/test_playwright.py` & `pytest-playwright-async-0.0.3/tests/test_playwright.py`

 * *Files identical despite different names*

