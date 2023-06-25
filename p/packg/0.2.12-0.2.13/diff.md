# Comparing `tmp/packg-0.2.12.tar.gz` & `tmp/packg-0.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packg-0.2.12.tar", last modified: Wed Jun 21 10:46:28 2023, max compression
+gzip compressed data, was "packg-0.2.13.tar", last modified: Sun Jun 25 20:53:50 2023, max compression
```

## Comparing `packg-0.2.12.tar` & `packg-0.2.13.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:46:28.196900 packg-0.2.12/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.12/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     2102 2023-06-21 10:46:28.196900 packg-0.2.12/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1306 2023-06-21 10:46:12.000000 packg-0.2.12/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2317 2023-06-21 09:57:15.000000 packg-0.2.12/pyproject.toml
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 10:46:12.000000 packg-0.2.12/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-21 10:46:28.196900 packg-0.2.12/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:46:28.120899 packg-0.2.12/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:46:28.164900 packg-0.2.12/src/packg/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      129 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/caching.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5520 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/constclass.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/dtime.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      297 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/files.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     7270 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/import_from_source.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     4229 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/log.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/misc.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/system.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      472 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/typext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:46:28.192900 packg-0.2.12/src/packg.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     2102 2023-06-21 10:46:27.000000 packg-0.2.12/src/packg.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      453 2023-06-21 10:46:28.000000 packg-0.2.12/src/packg.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 10:46:27.000000 packg-0.2.12/src/packg.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 10:46:27.000000 packg-0.2.12/src/packg.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-06-21 10:46:27.000000 packg-0.2.12/src/packg.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 10:00:06.000000 packg-0.2.12/src/packg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-25 20:53:50.913319 packg-0.2.13/
+-rw-rw-rw-   0        0        0    11336 2023-04-24 08:52:38.000000 packg-0.2.13/LICENSE
+-rw-rw-rw-   0        0        0     2169 2023-06-25 20:53:50.911319 packg-0.2.13/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-06-25 20:52:47.000000 packg-0.2.13/README.md
+-rw-rw-rw-   0        0        0     2317 2023-06-21 09:57:15.000000 packg-0.2.13/pyproject.toml
+-rw-rw-rw-   0        0        0       66 2023-06-25 20:52:47.000000 packg-0.2.13/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 20:53:50.913319 packg-0.2.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 20:53:50.858319 packg-0.2.13/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 20:53:50.875319 packg-0.2.13/src/packg/
+-rw-rw-rw-   0        0        0      129 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/__init__.py
+-rw-rw-rw-   0        0        0     3107 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/caching.py
+-rw-rw-rw-   0        0        0     5520 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/constclass.py
+-rw-rw-rw-   0        0        0      470 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/dtime.py
+-rw-rw-rw-   0        0        0     7270 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/import_from_source.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:53:50.911319 packg-0.2.13/src/packg/iotools/
+-rw-rw-rw-   0        0        0      400 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/iotools/__init__.py
+-rw-rw-rw-   0        0        0      420 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/iotools/compressed.py
+-rw-rw-rw-   0        0        0     6028 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/iotools/jsonext.py
+-rw-rw-rw-   0        0        0    10555 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/iotools/jsonext_encoder.py
+-rw-rw-rw-   0        0        0     3779 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/iotools/misc.py
+-rw-rw-rw-   0        0        0     4229 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/log.py
+-rw-rw-rw-   0        0        0      394 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/misc.py
+-rw-rw-rw-   0        0        0     1988 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/system.py
+-rw-rw-rw-   0        0        0     1328 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/tensors.py
+-rw-rw-rw-   0        0        0      527 2023-06-25 20:52:47.000000 packg-0.2.13/src/packg/typext.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:53:50.903319 packg-0.2.13/src/packg.egg-info/
+-rw-rw-rw-   0        0        0     2169 2023-06-25 20:53:50.000000 packg-0.2.13/src/packg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-06-25 20:53:50.000000 packg-0.2.13/src/packg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 20:53:50.000000 packg-0.2.13/src/packg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-06-25 20:53:50.000000 packg-0.2.13/src/packg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-25 20:53:50.000000 packg-0.2.13/src/packg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-25 20:37:56.000000 packg-0.2.13/src/packg.egg-info/zip-safe
```

### Comparing `packg-0.2.12/LICENSE` & `packg-0.2.13/LICENSE`

 * *Files identical despite different names*

### Comparing `packg-0.2.12/PKG-INFO` & `packg-0.2.13/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-Metadata-Version: 2.1
-Name: packg
-Version: 0.2.12
-Summary: Collection of utilities used in other python projects.
-Author: gingsi
-License: Apache-2.0
-Project-URL: Project-URL, https://github.com/gingsi/packg
-Keywords: attrs,typing,dict,attr
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Version Control :: Git
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# packg
-
-<p align="center">
-<a href="https://github.com/gingsi/packg/actions/workflows/build_py37.yml">
-  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/packg/build_py37.yml?branch=main&label=build%203.7" />
-</a>
-<a href="https://github.com/gingsi/packg/actions/workflows/build_py39.yml">
-  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/packg/build_py39.yml?branch=main&label=build%203.9" />
-</a>
-<img alt="coverage" title="coverage" src="https://raw.githubusercontent.com/gingsi/packg/main/docs/coverage.svg" />
-<a href="https://pypi.org/project/packg/">
-  <img alt="version" title="version" src="https://img.shields.io/pypi/v/packg?color=success" />
-</a>
-</p>
-
-Collection of utilities used in other python projects. 
-
-## Features
-
-* `caching`: Cache objects to disk / to memory
-* `Const`: Base class for defining constants, as alternative to `enum.Enum` 
-* `typext`: Type definitions
-* etc
-
-## Install
-
-Requires `python>=3.7`
-
-```bash
-pip install packg
-```
-
-## Dev install
-
-Clone repository and cd into, then:
-
-~~~bash
-pip install -e .
-pip install pytest pytest-cov pylint pytest-lazy-fixture
-pylint packg
-
-# run tests
-python -m pytest --cov
-pylint tests
-~~~
+Metadata-Version: 2.1
+Name: packg
+Version: 0.2.13
+Summary: Collection of utilities used in other python projects.
+Author: gingsi
+License: Apache-2.0
+Project-URL: Project-URL, https://github.com/gingsi/packg
+Keywords: attrs,typing,dict,attr
+Platform: any
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Version Control :: Git
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# packg
+
+<p align="center">
+<a href="https://github.com/gingsi/packg/actions/workflows/build_py37.yml">
+  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/packg/build_py37.yml?branch=main&label=build%203.7" />
+</a>
+<a href="https://github.com/gingsi/packg/actions/workflows/build_py39.yml">
+  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/packg/build_py39.yml?branch=main&label=build%203.9" />
+</a>
+<img alt="coverage" title="coverage" src="https://raw.githubusercontent.com/gingsi/packg/main/docs/coverage.svg" />
+<a href="https://pypi.org/project/packg/">
+  <img alt="version" title="version" src="https://img.shields.io/pypi/v/packg?color=success" />
+</a>
+</p>
+
+Collection of utilities used in other python projects. 
+
+## Features
+
+* `caching`: Cache objects to disk / to memory
+* `Const`: Base class for defining constants, as alternative to `enum.Enum` 
+* `typext`: Type definitions
+* etc
+
+## Install
+
+Requires `python>=3.7`
+
+```bash
+pip install packg
+```
+
+## Dev install
+
+Clone repository and cd into, then:
+
+~~~bash
+pip install -e .
+pip install pytest pytest-cov pylint pytest-lazy-fixture
+pylint packg
+
+# run tests
+python -m pytest --cov
+pylint tests
+~~~
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.12 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.13 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.12/README.md` & `packg-0.2.13/README.md`

 * *Files identical despite different names*

### Comparing `packg-0.2.12/pyproject.toml` & `packg-0.2.13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packg-0.2.12/src/packg/caching.py` & `packg-0.2.13/src/packg/caching.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.12/src/packg/constclass.py` & `packg-0.2.13/src/packg/constclass.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.12/src/packg/import_from_source.py` & `packg-0.2.13/src/packg/import_from_source.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.12/src/packg/log.py` & `packg-0.2.13/src/packg/log.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.12/src/packg/system.py` & `packg-0.2.13/src/packg/system.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.12/src/packg.egg-info/PKG-INFO` & `packg-0.2.13/src/packg.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-Metadata-Version: 2.1
-Name: packg
-Version: 0.2.12
-Summary: Collection of utilities used in other python projects.
-Author: gingsi
-License: Apache-2.0
-Project-URL: Project-URL, https://github.com/gingsi/packg
-Keywords: attrs,typing,dict,attr
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Version Control :: Git
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# packg
-
-<p align="center">
-<a href="https://github.com/gingsi/packg/actions/workflows/build_py37.yml">
-  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/packg/build_py37.yml?branch=main&label=build%203.7" />
-</a>
-<a href="https://github.com/gingsi/packg/actions/workflows/build_py39.yml">
-  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/packg/build_py39.yml?branch=main&label=build%203.9" />
-</a>
-<img alt="coverage" title="coverage" src="https://raw.githubusercontent.com/gingsi/packg/main/docs/coverage.svg" />
-<a href="https://pypi.org/project/packg/">
-  <img alt="version" title="version" src="https://img.shields.io/pypi/v/packg?color=success" />
-</a>
-</p>
-
-Collection of utilities used in other python projects. 
-
-## Features
-
-* `caching`: Cache objects to disk / to memory
-* `Const`: Base class for defining constants, as alternative to `enum.Enum` 
-* `typext`: Type definitions
-* etc
-
-## Install
-
-Requires `python>=3.7`
-
-```bash
-pip install packg
-```
-
-## Dev install
-
-Clone repository and cd into, then:
-
-~~~bash
-pip install -e .
-pip install pytest pytest-cov pylint pytest-lazy-fixture
-pylint packg
-
-# run tests
-python -m pytest --cov
-pylint tests
-~~~
+Metadata-Version: 2.1
+Name: packg
+Version: 0.2.13
+Summary: Collection of utilities used in other python projects.
+Author: gingsi
+License: Apache-2.0
+Project-URL: Project-URL, https://github.com/gingsi/packg
+Keywords: attrs,typing,dict,attr
+Platform: any
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Version Control :: Git
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# packg
+
+<p align="center">
+<a href="https://github.com/gingsi/packg/actions/workflows/build_py37.yml">
+  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/packg/build_py37.yml?branch=main&label=build%203.7" />
+</a>
+<a href="https://github.com/gingsi/packg/actions/workflows/build_py39.yml">
+  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/packg/build_py39.yml?branch=main&label=build%203.9" />
+</a>
+<img alt="coverage" title="coverage" src="https://raw.githubusercontent.com/gingsi/packg/main/docs/coverage.svg" />
+<a href="https://pypi.org/project/packg/">
+  <img alt="version" title="version" src="https://img.shields.io/pypi/v/packg?color=success" />
+</a>
+</p>
+
+Collection of utilities used in other python projects. 
+
+## Features
+
+* `caching`: Cache objects to disk / to memory
+* `Const`: Base class for defining constants, as alternative to `enum.Enum` 
+* `typext`: Type definitions
+* etc
+
+## Install
+
+Requires `python>=3.7`
+
+```bash
+pip install packg
+```
+
+## Dev install
+
+Clone repository and cd into, then:
+
+~~~bash
+pip install -e .
+pip install pytest pytest-cov pylint pytest-lazy-fixture
+pylint packg
+
+# run tests
+python -m pytest --cov
+pylint tests
+~~~
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.12 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.13 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

