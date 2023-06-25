# Comparing `tmp/delfino_core-5.0.0.tar.gz` & `tmp/delfino_core-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delfino_core-5.0.0.tar", max compression
+gzip compressed data, was "delfino_core-5.1.0.tar", max compression
```

## Comparing `delfino_core-5.0.0.tar` & `delfino_core-5.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1078 2023-06-25 11:49:06.204935 delfino_core-5.0.0/LICENSE.md
--rw-r--r--   0        0        0     5291 2023-06-25 11:49:06.204935 delfino_core-5.0.0/README.md
--rw-r--r--   0        0        0     4197 2023-06-25 11:49:06.204935 delfino_core-5.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/__init__.py
--rw-r--r--   0        0        0      293 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/backports.py
--rw-r--r--   0        0        0        0 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/__init__.py
--rw-r--r--   0        0        0     9055 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/dependencies_update.py
--rw-r--r--   0        0        0     2737 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/format.py
--rw-r--r--   0        0        0     6681 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/lint.py
--rw-r--r--   0        0        0     3471 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/switch_python_version.py
--rw-r--r--   0        0        0     7883 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/test.py
--rw-r--r--   0        0        0     3392 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/typecheck.py
--rw-r--r--   0        0        0      748 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/verify_all.py
--rw-r--r--   0        0        0      904 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/config.py
--rw-r--r--   0        0        0     1720 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/utils.py
--rw-r--r--   0        0        0     7463 1970-01-01 00:00:00.000000 delfino_core-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-25 12:57:57.859073 delfino_core-5.1.0/LICENSE.md
+-rw-r--r--   0        0        0     5291 2023-06-25 12:57:57.859073 delfino_core-5.1.0/README.md
+-rw-r--r--   0        0        0     4291 2023-06-25 12:57:57.859073 delfino_core-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/__init__.py
+-rw-r--r--   0        0        0      293 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/backports.py
+-rw-r--r--   0        0        0        0 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/__init__.py
+-rw-r--r--   0        0        0     9055 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/dependencies_update.py
+-rw-r--r--   0        0        0     4253 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/format.py
+-rw-r--r--   0        0        0     6681 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/lint.py
+-rw-r--r--   0        0        0     3471 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/switch_python_version.py
+-rw-r--r--   0        0        0     7883 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/test.py
+-rw-r--r--   0        0        0     3392 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/typecheck.py
+-rw-r--r--   0        0        0      748 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/verify_all.py
+-rw-r--r--   0        0        0      904 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/config.py
+-rw-r--r--   0        0        0     1720 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/utils.py
+-rw-r--r--   0        0        0     7551 1970-01-01 00:00:00.000000 delfino_core-5.1.0/PKG-INFO
```

### Comparing `delfino_core-5.0.0/LICENSE.md` & `delfino_core-5.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `delfino_core-5.0.0/README.md` & `delfino_core-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `delfino_core-5.0.0/pyproject.toml` & `delfino_core-5.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="delfino-core"
-version="5.0.0"
+version="5.1.0"
 authors = ["Radek Lát <radek.lat@gmail.com>"]
 description="Delfino core plugin"
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/radeklat/delfino-core"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -25,14 +25,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 delfino = ">=0.29.0"
 
 black = {version = "*", optional = true}
 isort = {version = "*", optional = true}
+pyupgrade = {version = "*", optional = true}
 pre-commit = {version = "*", optional = true}
 pytest = {version = "*", optional = true}
 coverage = {version = "*", optional = true}
 pytest-cov = {version = "*", optional = true}
 mypy = {version = "*", optional = true}
 pylint = {version = "*", optional = true}
 pycodestyle = {version = "*", optional = true}
@@ -56,24 +57,25 @@
 pytest = "^7.1"
 pytest-cov = "^4.0"
 pytest-mock = "^3.6"
 pre-commit = "^3.3"
 pycodestyle = "^2.8"
 pydocstyle = "^6.1"
 shellingham = "^1.4"
-psutil = "^5.9.4"
+psutil = "^5.9"
 types-termcolor = "*"
 types-toml = "^0.10.8.1"
-types-psutil = "^5.9.5.5"
-gitpython = "^3.1.29"
+types-psutil = "^5.9"
+gitpython = "^3.1"
+pyupgrade = "^3.7"
 
 [tool.poetry.extras]
-all = ["black", "isort", "pre-commit", "pytest", "coverage", "pytest-cov", "mypy", "pylint", "pycodestyle", "pydocstyle", "psutil", "gitpython"]
-verify_all = ["black", "isort", "pre-commit", "pytest", "coverage", "pytest-cov", "mypy", "pylint", "pycodestyle", "pydocstyle", "psutil"]
-format = ["black", "isort", "pre-commit"]
+all = ["black", "isort", "pyupgrade", "pre-commit", "pytest", "coverage", "pytest-cov", "mypy", "pylint", "pycodestyle", "pydocstyle", "psutil", "gitpython"]
+verify_all = ["black", "isort", "pyupgrade", "pre-commit", "pytest", "coverage", "pytest-cov", "mypy", "pylint", "pycodestyle", "pydocstyle", "psutil"]
+format = ["black", "isort", "pyupgrade", "pre-commit"]
 test = ["pytest", "coverage", "pytest-cov"]
 typecheck = ["mypy"]
 lint = ["pylint", "pycodestyle", "pydocstyle", "psutil"]
 dependencies_update = ["gitpython"]
 
 [tool.isort]
 # Setting compatible with black. See https://black.readthedocs.io/en/stable/compatible_configs.html
```

### Comparing `delfino_core-5.0.0/src/delfino_core/commands/dependencies_update.py` & `delfino_core-5.1.0/src/delfino_core/commands/dependencies_update.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.0.0/src/delfino_core/commands/lint.py` & `delfino_core-5.1.0/src/delfino_core/commands/lint.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.0.0/src/delfino_core/commands/switch_python_version.py` & `delfino_core-5.1.0/src/delfino_core/commands/switch_python_version.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.0.0/src/delfino_core/commands/test.py` & `delfino_core-5.1.0/src/delfino_core/commands/test.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.0.0/src/delfino_core/commands/typecheck.py` & `delfino_core-5.1.0/src/delfino_core/commands/typecheck.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.0.0/src/delfino_core/commands/verify_all.py` & `delfino_core-5.1.0/src/delfino_core/commands/verify_all.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.0.0/src/delfino_core/config.py` & `delfino_core-5.1.0/src/delfino_core/config.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.0.0/src/delfino_core/utils.py` & `delfino_core-5.1.0/src/delfino_core/utils.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.0.0/PKG-INFO` & `delfino_core-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delfino-core
-Version: 5.0.0
+Version: 5.1.0
 Summary: Delfino core plugin
 Home-page: https://github.com/radeklat/delfino-core
 License: MIT
 Author: Radek Lát
 Author-email: radek.lat@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -37,14 +37,15 @@
 Requires-Dist: pre-commit ; extra == "all" or extra == "verify-all" or extra == "format"
 Requires-Dist: psutil ; extra == "all" or extra == "verify-all" or extra == "lint"
 Requires-Dist: pycodestyle ; extra == "all" or extra == "verify-all" or extra == "lint"
 Requires-Dist: pydocstyle ; extra == "all" or extra == "verify-all" or extra == "lint"
 Requires-Dist: pylint ; extra == "all" or extra == "verify-all" or extra == "lint"
 Requires-Dist: pytest ; extra == "all" or extra == "verify-all" or extra == "test"
 Requires-Dist: pytest-cov ; extra == "all" or extra == "verify-all" or extra == "test"
+Requires-Dist: pyupgrade ; extra == "all" or extra == "verify-all" or extra == "format"
 Requires-Dist: shellingham
 Description-Content-Type: text/markdown
 
 <h1 align="center" style="border-bottom: none;"> 🔌&nbsp;&nbsp;Delfino Core&nbsp;&nbsp; 🔌</h1>
 <h3 align="center">A <a href="https://github.com/radeklat/delfino">Delfino</a> plugin with core functionality.</h3>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: delfino-core Version: 5.0.0 Summary: Delfino core
+Metadata-Version: 2.1 Name: delfino-core Version: 5.1.0 Summary: Delfino core
 plugin Home-page: https://github.com/radeklat/delfino-core License: MIT Author:
 Radek LÃ¡t Author-email: radek.lat@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -21,16 +21,17 @@
 "all" or extra == "verify-all" or extra == "format" Requires-Dist: psutil ;
 extra == "all" or extra == "verify-all" or extra == "lint" Requires-Dist:
 pycodestyle ; extra == "all" or extra == "verify-all" or extra == "lint"
 Requires-Dist: pydocstyle ; extra == "all" or extra == "verify-all" or extra ==
 "lint" Requires-Dist: pylint ; extra == "all" or extra == "verify-all" or extra
 == "lint" Requires-Dist: pytest ; extra == "all" or extra == "verify-all" or
 extra == "test" Requires-Dist: pytest-cov ; extra == "all" or extra == "verify-
-all" or extra == "test" Requires-Dist: shellingham Description-Content-Type:
-text/markdown
+all" or extra == "test" Requires-Dist: pyupgrade ; extra == "all" or extra ==
+"verify-all" or extra == "format" Requires-Dist: shellingham Description-
+Content-Type: text/markdown
                     ****** ð  Delfino Core   ð ******
               **** A Delfino plugin with core functionality. ****
  [CircleCI] [Codecov] [GitHub_tag_(latest_SemVer)] [Maintenance] [GitHub_last
                   commit] [PyPI_-_Python_Version] [Downloads]
 # Commands | Command | Description | |-----------------------|-----------------
 ------------------------------------| | coverage-open | Open coverage results
 in default browser. | | coverage-report | Analyse coverage and generate a term/
```

