# Comparing `tmp/jaraco.collections-4.2.0.tar.gz` & `tmp/jaraco.collections-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.collections-4.2.0.tar", last modified: Thu Jun  1 14:09:51 2023, max compression
+gzip compressed data, was "jaraco.collections-4.3.0.tar", last modified: Sun Jun 25 18:18:22 2023, max compression
```

## Comparing `jaraco.collections-4.2.0.tar` & `jaraco.collections-4.3.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (123)    26928 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/jaraco/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/jaraco.collections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-01 14:09:51.000000 jaraco.collections-4.2.0/jaraco.collections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-01 14:09:51.000000 jaraco.collections-4.2.0/jaraco.collections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:09:51.000000 jaraco.collections-4.2.0/jaraco.collections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-01 14:09:51.000000 jaraco.collections-4.2.0/jaraco.collections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 14:09:51.000000 jaraco.collections-4.2.0/jaraco.collections.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 14:09:51.867082 jaraco.collections-4.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:18:22.361285 jaraco.collections-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:18:22.357285 jaraco.collections-4.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:18:22.357285 jaraco.collections-4.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-25 18:18:22.361285 jaraco.collections-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:18:22.357285 jaraco.collections-4.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:18:22.357285 jaraco.collections-4.3.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (123)    26928 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/jaraco/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:18:22.361285 jaraco.collections-4.3.0/jaraco.collections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-25 18:18:22.000000 jaraco.collections-4.3.0/jaraco.collections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-25 18:18:22.000000 jaraco.collections-4.3.0/jaraco.collections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:18:22.000000 jaraco.collections-4.3.0/jaraco.collections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-25 18:18:22.000000 jaraco.collections-4.3.0/jaraco.collections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-25 18:18:22.000000 jaraco.collections-4.3.0/jaraco.collections.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-25 18:18:22.361285 jaraco.collections-4.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:18:22.361285 jaraco.collections-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-25 18:18:01.000000 jaraco.collections-4.3.0/tox.ini
```

### Comparing `jaraco.collections-4.2.0/.github/workflows/main.yml` & `jaraco.collections-4.3.0/.github/workflows/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -38,57 +38,51 @@
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - "3.7"
+        - "3.8"
         - "3.11"
         - "3.12"
-        # Workaround for actions/setup-python#508
-        dev:
-        - -dev
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
-        - python: "3.8"
-          platform: ubuntu-latest
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         - python: pypy3.9
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.12' }}
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
```

### Comparing `jaraco.collections-4.2.0/CHANGES.rst` & `jaraco.collections-4.3.0/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v4.3.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v4.2.0
 ======
 
 Added ``Mask``, the inverse of a ``Projection``.
 
 v4.1.0
 ======
```

### Comparing `jaraco.collections-4.2.0/LICENSE` & `jaraco.collections-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.collections-4.2.0/PKG-INFO` & `jaraco.collections-4.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: jaraco.collections
-Version: 4.2.0
+Version: 4.3.0
 Summary: Collection objects similar to those in stdlib by jaraco
 Home-page: https://github.com/jaraco/jaraco.collections
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.collections.svg
    :target: https://pypi.org/project/jaraco.collections
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.collections.svg
 
 .. image:: https://github.com/jaraco/jaraco.collections/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.collections/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracocollections/badge/?version=latest
    :target: https://jaracocollections.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.collections-4.2.0/README.rst` & `jaraco.collections-4.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.collections.svg
 
 .. image:: https://github.com/jaraco/jaraco.collections/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.collections/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracocollections/badge/?version=latest
    :target: https://jaracocollections.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.collections-4.2.0/docs/conf.py` & `jaraco.collections-4.3.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 master_doc = "index"
 html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
```

### Comparing `jaraco.collections-4.2.0/jaraco/collections.py` & `jaraco.collections-4.3.0/jaraco/collections.py`

 * *Files identical despite different names*

### Comparing `jaraco.collections-4.2.0/jaraco.collections.egg-info/PKG-INFO` & `jaraco.collections-4.3.0/jaraco.collections.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: jaraco.collections
-Version: 4.2.0
+Version: 4.3.0
 Summary: Collection objects similar to those in stdlib by jaraco
 Home-page: https://github.com/jaraco/jaraco.collections
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.collections.svg
    :target: https://pypi.org/project/jaraco.collections
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.collections.svg
 
 .. image:: https://github.com/jaraco/jaraco.collections/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.collections/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracocollections/badge/?version=latest
    :target: https://jaracocollections.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.collections-4.2.0/pytest.ini` & `jaraco.collections-4.3.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.collections-4.2.0/setup.cfg` & `jaraco.collections-4.3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	jaraco.text
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
```

### Comparing `jaraco.collections-4.2.0/tests/test_collections.py` & `jaraco.collections-4.3.0/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `jaraco.collections-4.2.0/tox.ini` & `jaraco.collections-4.3.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 [tox]
-envlist = python
-minversion = 3.2
-# https://github.com/jaraco/skeleton/issues/6
-tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
 setenv =
 	PYTHONWARNDEFAULTENCODING = 1
@@ -21,14 +17,24 @@
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
 	python -m sphinxlint
 
+[testenv:finalize]
+skip_install = True
+deps =
+	towncrier
+	jaraco.develop >= 7.23
+passenv = *
+commands =
+	python -m jaraco.develop.finalize
+
+
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
 passenv =
```

