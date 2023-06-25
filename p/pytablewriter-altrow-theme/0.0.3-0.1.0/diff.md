# Comparing `tmp/pytablewriter-altrow-theme-0.0.3.tar.gz` & `tmp/pytablewriter-altrow-theme-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytablewriter-altrow-theme-0.0.3.tar", last modified: Sun Oct 31 13:43:30 2021, max compression
+gzip compressed data, was "pytablewriter-altrow-theme-0.1.0.tar", last modified: Sun Jun 25 10:53:33 2023, max compression
```

## Comparing `pytablewriter-altrow-theme-0.0.3.tar` & `pytablewriter-altrow-theme-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-10-31 13:43:30.880000 pytablewriter-altrow-theme-0.0.3/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:01.000000 pytablewriter-altrow-theme-0.0.3/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      203 2021-03-20 04:14:01.000000 pytablewriter-altrow-theme-0.0.3/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     4648 2021-10-31 13:43:30.880000 pytablewriter-altrow-theme-0.0.3/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     3120 2021-10-31 10:45:55.000000 pytablewriter-altrow-theme-0.0.3/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)     1295 2021-10-31 13:02:05.000000 pytablewriter-altrow-theme-0.0.3/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-10-31 13:43:30.880000 pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme/
--rw-r--r--   0 toor      (1000) toor      (1000)     1422 2021-10-31 13:05:41.000000 pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2021-10-31 13:06:09.000000 pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme/__version__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-10-31 13:43:30.880000 pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     4648 2021-10-31 13:43:30.000000 pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      527 2021-10-31 13:43:30.000000 pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2021-10-31 13:43:30.000000 pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2021-10-31 13:43:14.000000 pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)       88 2021-10-31 13:43:30.000000 pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       27 2021-10-31 13:43:30.000000 pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-10-31 13:43:30.880000 pytablewriter-altrow-theme-0.0.3/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       44 2021-06-02 02:36:48.000000 pytablewriter-altrow-theme-0.0.3/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       36 2021-03-20 16:47:46.000000 pytablewriter-altrow-theme-0.0.3/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2021-10-31 13:43:30.880000 pytablewriter-altrow-theme-0.0.3/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2622 2021-10-31 11:05:19.000000 pytablewriter-altrow-theme-0.0.3/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-10-31 13:43:30.880000 pytablewriter-altrow-theme-0.0.3/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)     1072 2021-06-02 02:38:27.000000 pytablewriter-altrow-theme-0.0.3/tests/test_altrow.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1081 2021-10-31 11:03:51.000000 pytablewriter-altrow-theme-0.0.3/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 10:53:32.999514 pytablewriter-altrow-theme-0.1.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:01.000000 pytablewriter-altrow-theme-0.1.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      203 2021-03-20 04:14:01.000000 pytablewriter-altrow-theme-0.1.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     4634 2023-06-25 10:53:32.999514 pytablewriter-altrow-theme-0.1.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     3126 2023-06-25 10:46:40.000000 pytablewriter-altrow-theme-0.1.0/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)     1392 2023-06-25 10:44:04.000000 pytablewriter-altrow-theme-0.1.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 10:53:32.989514 pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1422 2021-10-31 13:05:41.000000 pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-25 10:50:18.000000 pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme/__version__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 10:53:32.999514 pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     4634 2023-06-25 10:53:32.000000 pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      527 2023-06-25 10:53:32.000000 pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 10:53:32.000000 pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 10:52:55.000000 pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)       88 2023-06-25 10:53:32.000000 pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       27 2023-06-25 10:53:32.000000 pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 10:53:32.999514 pytablewriter-altrow-theme-0.1.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       44 2023-06-25 10:00:39.000000 pytablewriter-altrow-theme-0.1.0/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       36 2023-02-05 15:15:20.000000 pytablewriter-altrow-theme-0.1.0/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-25 10:53:32.999514 pytablewriter-altrow-theme-0.1.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2634 2023-06-25 10:43:40.000000 pytablewriter-altrow-theme-0.1.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 10:53:32.999514 pytablewriter-altrow-theme-0.1.0/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1072 2021-06-02 02:38:27.000000 pytablewriter-altrow-theme-0.1.0/tests/test_altrow.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      981 2023-06-25 10:43:53.000000 pytablewriter-altrow-theme-0.1.0/tox.ini
```

### Comparing `pytablewriter-altrow-theme-0.0.3/LICENSE` & `pytablewriter-altrow-theme-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytablewriter-altrow-theme-0.0.3/PKG-INFO` & `pytablewriter-altrow-theme-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: pytablewriter-altrow-theme
-Version: 0.0.3
+Version: 0.1.0
 Summary: A pytablewriter plugin to provide a theme that colored rows alternatively.
 Home-page: https://github.com/thombashi/pytablewriter-altrow-theme
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytablewriter-altrow-theme
 Project-URL: Tracker, https://github.com/thombashi/pytablewriter-altrow-theme/issues
 Keywords: pytablewriter,plugin
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **pytablewriter-altrow-theme**
    :backlinks: top
    :depth: 2
@@ -47,17 +46,17 @@
     :target: https://pypi.org/project/pytablewriter-altrow-theme
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/pypi/implementation/pytablewriter-altrow-theme.svg
     :target: https://pypi.org/project/pytablewriter-altrow-theme
     :alt: Supported Python implementations
 
-.. image:: https://github.com/thombashi/pytablewriter-altrow-theme/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/pytablewriter-altrow-theme/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. image:: https://github.com/thombashi/pytablewriter-altrow-theme/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/pytablewriter-altrow-theme/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
 .. image:: https://coveralls.io/repos/github/thombashi/pytablewriter-altrow-theme/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/pytablewriter-altrow-theme?branch=master
     :alt: Test coverage: coveralls
 
 pytablewriter-altrow-theme is a `pytablewriter <https://github.com/thombashi/pytablewriter>`__ plugin to provide a theme that colored rows alternatively.
 
@@ -120,12 +119,10 @@
     .. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytablewriter-altrow-theme@master/ss/ptw-altrow-theme_example_yellow.png
        :scale: 100%
        :alt: https://github.com/thombashi/pytablewriter-altrow-theme/blob/master/ss/ptw-altrow-theme_example_yellow.png
 
 
 Dependencies
 ============================================
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytablewriter-altrow-theme/network/dependencies>`__
 
-
-
```

### Comparing `pytablewriter-altrow-theme-0.0.3/README.rst` & `pytablewriter-altrow-theme-0.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     :target: https://pypi.org/project/pytablewriter-altrow-theme
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/pypi/implementation/pytablewriter-altrow-theme.svg
     :target: https://pypi.org/project/pytablewriter-altrow-theme
     :alt: Supported Python implementations
 
-.. image:: https://github.com/thombashi/pytablewriter-altrow-theme/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/pytablewriter-altrow-theme/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. image:: https://github.com/thombashi/pytablewriter-altrow-theme/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/pytablewriter-altrow-theme/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
 .. image:: https://coveralls.io/repos/github/thombashi/pytablewriter-altrow-theme/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/pytablewriter-altrow-theme?branch=master
     :alt: Test coverage: coveralls
 
 pytablewriter-altrow-theme is a `pytablewriter <https://github.com/thombashi/pytablewriter>`__ plugin to provide a theme that colored rows alternatively.
 
@@ -86,10 +86,10 @@
     .. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytablewriter-altrow-theme@master/ss/ptw-altrow-theme_example_yellow.png
        :scale: 100%
        :alt: https://github.com/thombashi/pytablewriter-altrow-theme/blob/master/ss/ptw-altrow-theme_example_yellow.png
 
 
 Dependencies
 ============================================
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytablewriter-altrow-theme/network/dependencies>`__
```

### Comparing `pytablewriter-altrow-theme-0.0.3/pyproject.toml` & `pytablewriter-altrow-theme-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
@@ -14,14 +15,15 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 | docs/conf.py
 '''
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.coverage.run]
 source = ['pytablewriter_altrow_theme']
 branch = true
 
 [tool.coverage.report]
 show_missing = true
@@ -49,15 +51,15 @@
     '*/.eggs/*',
     '*/.pytype/*',
     '*/.tox/*',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.6
+python_version = 3.7
 pretty = true
 
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 no_implicit_optional = true
 show_error_codes = true
```

### Comparing `pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme/__init__.py` & `pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme.egg-info/PKG-INFO` & `pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: pytablewriter-altrow-theme
-Version: 0.0.3
+Version: 0.1.0
 Summary: A pytablewriter plugin to provide a theme that colored rows alternatively.
 Home-page: https://github.com/thombashi/pytablewriter-altrow-theme
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytablewriter-altrow-theme
 Project-URL: Tracker, https://github.com/thombashi/pytablewriter-altrow-theme/issues
 Keywords: pytablewriter,plugin
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **pytablewriter-altrow-theme**
    :backlinks: top
    :depth: 2
@@ -47,17 +46,17 @@
     :target: https://pypi.org/project/pytablewriter-altrow-theme
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/pypi/implementation/pytablewriter-altrow-theme.svg
     :target: https://pypi.org/project/pytablewriter-altrow-theme
     :alt: Supported Python implementations
 
-.. image:: https://github.com/thombashi/pytablewriter-altrow-theme/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/pytablewriter-altrow-theme/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. image:: https://github.com/thombashi/pytablewriter-altrow-theme/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/pytablewriter-altrow-theme/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
 .. image:: https://coveralls.io/repos/github/thombashi/pytablewriter-altrow-theme/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/pytablewriter-altrow-theme?branch=master
     :alt: Test coverage: coveralls
 
 pytablewriter-altrow-theme is a `pytablewriter <https://github.com/thombashi/pytablewriter>`__ plugin to provide a theme that colored rows alternatively.
 
@@ -120,12 +119,10 @@
     .. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytablewriter-altrow-theme@master/ss/ptw-altrow-theme_example_yellow.png
        :scale: 100%
        :alt: https://github.com/thombashi/pytablewriter-altrow-theme/blob/master/ss/ptw-altrow-theme_example_yellow.png
 
 
 Dependencies
 ============================================
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytablewriter-altrow-theme/network/dependencies>`__
 
-
-
```

### Comparing `pytablewriter-altrow-theme-0.0.3/pytablewriter_altrow_theme.egg-info/SOURCES.txt` & `pytablewriter-altrow-theme-0.1.0/pytablewriter_altrow_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytablewriter-altrow-theme-0.0.3/setup.py` & `pytablewriter-altrow-theme-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "pytablewriter-altrow-theme"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -44,30 +44,30 @@
     include_package_data=True,
     keywords=["pytablewriter", "plugin"],
     license=pkg_info["__license__"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["tests*"]),
     project_urls={"Source": REPOSITORY_URL, "Tracker": f"{REPOSITORY_URL:s}/issues"},
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=INSTALL_REQUIRES,
     extras_require={"test": TESTS_REQUIRES},
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Environment :: Plugins",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     cmdclass=get_release_command_class(),
```

### Comparing `pytablewriter-altrow-theme-0.0.3/tests/test_altrow.py` & `pytablewriter-altrow-theme-0.1.0/tests/test_altrow.py`

 * *Files identical despite different names*

### Comparing `pytablewriter-altrow-theme-0.0.3/tox.ini` & `pytablewriter-altrow-theme-0.1.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,62 @@
 [tox]
 envlist =
-    py{35,36,37,38,39,310}
+    py{37,38,39,310,311}
     pypy3
     build
-    clean
     cov
     fmt
     lint
 
 [testenv]
 passenv = *
-deps =
-    .[test]
+extras =
+    test
 commands =
     pytest {posargs}
 
 [testenv:build]
-basepython = python3.8
 deps =
+    build>=0.10
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
+    python -m build
     twine check dist/*.whl dist/*.tar.gz
-    python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
-    cleanpy>=0.3.1
+    cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
 
 [testenv:cov]
 passenv = *
+extras =
+    test
 deps =
-    .[test]
     coverage[toml]>=5
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
 [testenv:fmt]
-basepython = python3.8
 skip_install = true
 deps =
-    autoflake
-    black
+    autoflake>=2
+    black>=23.1
     isort>=5
 commands =
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
     isort .
     black setup.py examples tests pytablewriter_altrow_theme
 
 [testenv:lint]
-basepython = python3.8
 skip_install = true
 deps =
-    mypy>=0.910
-    pylama
+    mypy>=1
+    pylama>=8.4.1
 commands =
     python setup.py check
     mypy pytablewriter_altrow_theme setup.py
     pylama
```

