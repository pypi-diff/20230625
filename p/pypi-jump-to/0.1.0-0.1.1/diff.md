# Comparing `tmp/pypi_jump_to-0.1.0.tar.gz` & `tmp/pypi_jump_to-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_jump_to-0.1.0.tar", max compression
+gzip compressed data, was "pypi_jump_to-0.1.1.tar", max compression
```

## Comparing `pypi_jump_to-0.1.0.tar` & `pypi_jump_to-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/LICENSE
--rw-r--r--   0        0        0     5954 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/README.md
--rw-r--r--   0        0        0     5245 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      422 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/src/pjt/__init__.py
--rw-r--r--   0        0        0      462 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/src/pjt/app.py
--rw-r--r--   0        0        0      118 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/src/pjt/cli/__init__.py
--rw-r--r--   0        0        0     5057 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/src/pjt/cli/application.py
--rw-r--r--   0        0        0     1524 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/src/pjt/cli/commands.py
--rw-r--r--   0        0        0      110 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/src/pjt/core/__init__.py
--rw-r--r--   0        0        0     1414 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/src/pjt/core/entities.py
--rw-r--r--   0        0        0     2099 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/src/pjt/core/pypi.py
--rw-r--r--   0        0        0        0 2023-06-25 20:18:12.943593 pypi_jump_to-0.1.0/src/pjt/py.typed
--rw-r--r--   0        0        0     7724 1970-01-01 00:00:00.000000 pypi_jump_to-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-25 20:21:39.287752 pypi_jump_to-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5954 2023-06-25 20:21:39.287752 pypi_jump_to-0.1.1/README.md
+-rw-r--r--   0        0        0     5245 2023-06-25 20:22:07.164134 pypi_jump_to-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      425 2023-06-25 20:22:07.080133 pypi_jump_to-0.1.1/src/pjt/__init__.py
+-rw-r--r--   0        0        0      499 2023-06-25 20:21:39.287752 pypi_jump_to-0.1.1/src/pjt/app.py
+-rw-r--r--   0        0        0      118 2023-06-25 20:21:39.287752 pypi_jump_to-0.1.1/src/pjt/cli/__init__.py
+-rw-r--r--   0        0        0     5057 2023-06-25 20:21:39.287752 pypi_jump_to-0.1.1/src/pjt/cli/application.py
+-rw-r--r--   0        0        0     1524 2023-06-25 20:21:39.287752 pypi_jump_to-0.1.1/src/pjt/cli/commands.py
+-rw-r--r--   0        0        0      110 2023-06-25 20:21:39.287752 pypi_jump_to-0.1.1/src/pjt/core/__init__.py
+-rw-r--r--   0        0        0     1414 2023-06-25 20:21:39.287752 pypi_jump_to-0.1.1/src/pjt/core/entities.py
+-rw-r--r--   0        0        0     2099 2023-06-25 20:21:39.287752 pypi_jump_to-0.1.1/src/pjt/core/pypi.py
+-rw-r--r--   0        0        0        0 2023-06-25 20:21:39.287752 pypi_jump_to-0.1.1/src/pjt/py.typed
+-rw-r--r--   0        0        0     7724 1970-01-01 00:00:00.000000 pypi_jump_to-0.1.1/PKG-INFO
```

### Comparing `pypi_jump_to-0.1.0/LICENSE` & `pypi_jump_to-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi_jump_to-0.1.0/README.md` & `pypi_jump_to-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pypi_jump_to-0.1.0/pyproject.toml` & `pypi_jump_to-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypi-jump-to"
-version = "0.1.0"
+version = "0.1.1"
 description = "pjt (pypi-jump-to) - a quick navigation tool for the PyPI packages."
 license = "MIT"
 authors = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 maintainers = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 keywords = [
     "python",
     "pypi",
```

### Comparing `pypi_jump_to-0.1.0/src/pjt/cli/application.py` & `pypi_jump_to-0.1.1/src/pjt/cli/application.py`

 * *Files identical despite different names*

### Comparing `pypi_jump_to-0.1.0/src/pjt/cli/commands.py` & `pypi_jump_to-0.1.1/src/pjt/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pypi_jump_to-0.1.0/src/pjt/core/entities.py` & `pypi_jump_to-0.1.1/src/pjt/core/entities.py`

 * *Files identical despite different names*

### Comparing `pypi_jump_to-0.1.0/src/pjt/core/pypi.py` & `pypi_jump_to-0.1.1/src/pjt/core/pypi.py`

 * *Files identical despite different names*

### Comparing `pypi_jump_to-0.1.0/PKG-INFO` & `pypi_jump_to-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-jump-to
-Version: 0.1.0
+Version: 0.1.1
 Summary: pjt (pypi-jump-to) - a quick navigation tool for the PyPI packages.
 Home-page: https://github.com/volopivoshenko/pypi-jump-to
 License: MIT
 Keywords: python,pypi,pip,packages,search,productivity,jump,shortcuts,cli,command-line-tool,cross-platform,hacktoberfest
 Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com
 Maintainer: Volodymyr Pivoshenko
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypi-jump-to Version: 0.1.0 Summary: pjt (pypi-
+Metadata-Version: 2.1 Name: pypi-jump-to Version: 0.1.1 Summary: pjt (pypi-
 jump-to) - a quick navigation tool for the PyPI packages. Home-page: https://
 github.com/volopivoshenko/pypi-jump-to License: MIT Keywords:
 python,pypi,pip,packages,search,productivity,jump,shortcuts,cli,command-line-
 tool,cross-platform,hacktoberfest Author: Volodymyr Pivoshenko Author-email:
 volodymyr.pivoshenko@gmail.com Maintainer: Volodymyr Pivoshenko Maintainer-
 email: volodymyr.pivoshenko@gmail.com Requires-Python: >=3.8.1,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Other
```

