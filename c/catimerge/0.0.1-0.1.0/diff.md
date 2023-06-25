# Comparing `tmp/catimerge-0.0.1.tar.gz` & `tmp/catimerge-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catimerge-0.0.1.tar", last modified: Fri Jun 23 17:52:43 2023, max compression
+gzip compressed data, was "catimerge-0.1.0.tar", last modified: Sun Jun 25 15:39:34 2023, max compression
```

## Comparing `catimerge-0.0.1.tar` & `catimerge-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 fay       (1000) fay       (1000)        0 2023-06-23 17:52:43.490541 catimerge-0.0.1/
--rw-------   0 fay       (1000) fay       (1000)    34523 2023-06-23 14:00:18.000000 catimerge-0.0.1/LICENSE.AGPLv3
--rw-------   0 fay       (1000) fay       (1000)       85 2023-06-23 17:01:34.000000 catimerge-0.0.1/MANIFEST.in
--rw-------   0 fay       (1000) fay       (1000)      798 2023-06-23 17:08:34.000000 catimerge-0.0.1/Makefile
--rw-------   0 fay       (1000) fay       (1000)     3509 2023-06-23 17:52:43.490541 catimerge-0.0.1/PKG-INFO
--rw-------   0 fay       (1000) fay       (1000)     2363 2023-06-23 17:37:45.000000 catimerge-0.0.1/README.md
-drwx------   0 fay       (1000) fay       (1000)        0 2023-06-23 17:52:43.490541 catimerge-0.0.1/catimerge/
--rwx------   0 fay       (1000) fay       (1000)     7964 2023-06-23 17:17:16.000000 catimerge-0.0.1/catimerge/__init__.py
--rw-------   0 fay       (1000) fay       (1000)        0 2023-06-23 16:53:48.000000 catimerge-0.0.1/catimerge/py.typed
-drwx------   0 fay       (1000) fay       (1000)        0 2023-06-23 17:52:43.490541 catimerge-0.0.1/catimerge.egg-info/
--rw-------   0 fay       (1000) fay       (1000)     3509 2023-06-23 17:52:43.000000 catimerge-0.0.1/catimerge.egg-info/PKG-INFO
--rw-------   0 fay       (1000) fay       (1000)      277 2023-06-23 17:52:43.000000 catimerge-0.0.1/catimerge.egg-info/SOURCES.txt
--rw-------   0 fay       (1000) fay       (1000)        1 2023-06-23 17:52:43.000000 catimerge-0.0.1/catimerge.egg-info/dependency_links.txt
--rw-------   0 fay       (1000) fay       (1000)       45 2023-06-23 17:52:43.000000 catimerge-0.0.1/catimerge.egg-info/entry_points.txt
--rw-------   0 fay       (1000) fay       (1000)       10 2023-06-23 17:52:43.000000 catimerge-0.0.1/catimerge.egg-info/top_level.txt
--rw-------   0 fay       (1000) fay       (1000)        0 2023-06-23 17:01:38.000000 catimerge-0.0.1/changelog.txt
--rw-------   0 fay       (1000) fay       (1000)       38 2023-06-23 17:52:43.490541 catimerge-0.0.1/setup.cfg
--rw-------   0 fay       (1000) fay       (1000)     1707 2023-06-23 16:54:57.000000 catimerge-0.0.1/setup.py
+drwx------   0 fay       (1000) fay       (1000)        0 2023-06-25 15:39:34.579613 catimerge-0.1.0/
+-rw-------   0 fay       (1000) fay       (1000)    34523 2023-06-23 14:00:18.000000 catimerge-0.1.0/LICENSE.AGPLv3
+-rw-------   0 fay       (1000) fay       (1000)       85 2023-06-23 17:01:34.000000 catimerge-0.1.0/MANIFEST.in
+-rw-------   0 fay       (1000) fay       (1000)      891 2023-06-25 14:54:10.000000 catimerge-0.1.0/Makefile
+-rw-------   0 fay       (1000) fay       (1000)     4941 2023-06-25 15:39:34.579613 catimerge-0.1.0/PKG-INFO
+-rw-------   0 fay       (1000) fay       (1000)     3795 2023-06-24 11:24:56.000000 catimerge-0.1.0/README.md
+drwx------   0 fay       (1000) fay       (1000)        0 2023-06-25 15:39:34.579613 catimerge-0.1.0/catimerge/
+-rwx------   0 fay       (1000) fay       (1000)    13668 2023-06-25 15:21:32.000000 catimerge-0.1.0/catimerge/__init__.py
+-rw-------   0 fay       (1000) fay       (1000)        0 2023-06-23 16:53:48.000000 catimerge-0.1.0/catimerge/py.typed
+drwx------   0 fay       (1000) fay       (1000)        0 2023-06-25 15:39:34.579613 catimerge-0.1.0/catimerge.egg-info/
+-rw-------   0 fay       (1000) fay       (1000)     4941 2023-06-25 15:39:34.000000 catimerge-0.1.0/catimerge.egg-info/PKG-INFO
+-rw-------   0 fay       (1000) fay       (1000)      277 2023-06-25 15:39:34.000000 catimerge-0.1.0/catimerge.egg-info/SOURCES.txt
+-rw-------   0 fay       (1000) fay       (1000)        1 2023-06-25 15:39:34.000000 catimerge-0.1.0/catimerge.egg-info/dependency_links.txt
+-rw-------   0 fay       (1000) fay       (1000)       45 2023-06-25 15:39:34.000000 catimerge-0.1.0/catimerge.egg-info/entry_points.txt
+-rw-------   0 fay       (1000) fay       (1000)       10 2023-06-25 15:39:34.000000 catimerge-0.1.0/catimerge.egg-info/top_level.txt
+-rw-------   0 fay       (1000) fay       (1000)      188 2023-06-25 15:26:25.000000 catimerge-0.1.0/changelog.txt
+-rw-------   0 fay       (1000) fay       (1000)       38 2023-06-25 15:39:34.579613 catimerge-0.1.0/setup.cfg
+-rw-------   0 fay       (1000) fay       (1000)     1707 2023-06-23 16:54:57.000000 catimerge-0.1.0/setup.py
```

### Comparing `catimerge-0.0.1/LICENSE.AGPLv3` & `catimerge-0.1.0/LICENSE.AGPLv3`

 * *Files identical despite different names*

### Comparing `catimerge-0.0.1/Makefile` & `catimerge-0.1.0/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 SHELL     := /bin/bash
 PYTHON    ?= python3
 
 export PYTHONWARNINGS := default
 
-.PHONY: all install test lint lint-extra clean cleanup
+.PHONY: all install test doctest lint lint-extra clean cleanup
 
 all:
 
 install:
 	$(PYTHON) -mpip install -e .
 
-test: lint lint-extra
+test: doctest lint lint-extra
+
+doctest:
+	# NB: uses test/*.zip
+	$(PYTHON) -m doctest catimerge/__init__.py
 
 lint:
 	flake8 catimerge/__init__.py
 	pylint catimerge/__init__.py
 
 lint-extra:
 	mypy --strict --disallow-any-unimported catimerge/__init__.py
```

### Comparing `catimerge-0.0.1/PKG-INFO` & `catimerge-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: catimerge
-Version: 0.0.1
-Summary: merge two catima.zip exports
-Home-page: https://github.com/obfusk/catimerge
-Author: FC Stegerman
-Author-email: flx@obfusk.net
-License: AGPLv3+
-Keywords: catima export merge
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.AGPLv3
-
 <!-- SPDX-FileCopyrightText: 2023 FC Stegerman <flx@obfusk.net> -->
 <!-- SPDX-License-Identifier: AGPL-3.0-or-later -->
 
 [![GitHub Release](https://img.shields.io/github/release/obfusk/catimerge.svg?logo=github)](https://github.com/obfusk/catimerge/releases)
 [![PyPI Version](https://img.shields.io/pypi/v/catimerge.svg)](https://pypi.python.org/pypi/catimerge)
 [![Python Versions](https://img.shields.io/pypi/pyversions/catimerge.svg)](https://pypi.python.org/pypi/catimerge)
 [![CI](https://github.com/obfusk/catimerge/workflows/CI/badge.svg)](https://github.com/obfusk/catimerge/actions?query=workflow%3ACI)
@@ -49,26 +20,86 @@
 -->
 
 # catimerge
 
 Merge two [Catima](https://catima.app) `.zip` exports.
 
 ```sh
+$ catimerge --help
+usage: catimerge [-h] [-v] [--version] FIRST_ZIP SECOND_ZIP OUTPUT_ZIP
+
+positional arguments:
+  FIRST_ZIP
+  SECOND_ZIP
+  OUTPUT_ZIP
+
+options:
+  -h, --help     show this help message and exit
+  -v, --verbose
+  --version      show program's version number and exit
 $ catimerge -v catima1.zip catima2.zip out.zip
 Merging 'catima1.zip' and 'catima2.zip' into 'out.zip'...
 Parsing...
 Version: 2
 ZIP #1 has   1 group(s),   9 card(s),   2 card group(s),   5 image file(s)
 ZIP #2 has   2 group(s),   5 card(s),   3 card group(s),   3 image file(s)
 Merging...
 Output has   3 group(s),  14 card(s),   5 card group(s),   8 image file(s)
 Writing...
 ```
 
-NB: does not support password-protected exports.
+## CAVEATS
+
+Unfortunately, Python does not support the password-protected ZIP
+files created by Catima.  You can either export your data without a
+password, or use a tool like 7-Zip to create a temporary passwordless
+ZIP file for the merge process.
+
+For example, if you have two password-protected ZIP files as input and
+want a password-protected output ZIP file as well:
+
+<details>
+
+```sh
+$ ls
+catima1.zip
+catima2.zip
+$ 7z -ocatima1 x catima1.zip            # extract into catima1/
+[...]
+$ 7z -ocatima2 x catima2.zip            # extract into catima2/
+[...]
+$ cd catima1
+$ 7z a ../catima1-nopass.zip *          # create passwordless ZIP
+[...]
+$ cd ..
+$ cd catima2
+$ 7z a ../catima2-nopass.zip *          # create passwordless ZIP
+[...]
+$ cd ..
+$ catimerge -v catima1-nopass.zip catima2-nopass.zip out-nopass.zip
+Merging 'catima1-nopass.zip' and 'catima2-nopass.zip' into 'out-nopass.zip'...
+[...]
+$ 7z -oout-nopass x out-nopass.zip      # extract into out-nopass/
+$ cd out-nopass
+$ 7z -p a ../out.zip *                  # create password-protected ZIP
+[...]
+$ cd ..
+$ ls
+catima1
+catima1-nopass.zip
+catima1.zip
+catima2
+catima2-nopass.zip
+catima2.zip
+out-nopass
+out-nopass.zip
+out.zip
+```
+
+</details>
 
 ## Installing
 
 ### Using pip
 
 ```bash
 $ pip install catimerge
```

#### html2text {}

```diff
@@ -1,39 +1,41 @@
-Metadata-Version: 2.1 Name: catimerge Version: 0.0.1 Summary: merge two
-catima.zip exports Home-page: https://github.com/obfusk/catimerge Author: FC
-Stegerman Author-email: flx@obfusk.net License: AGPLv3+ Keywords: catima export
-merge Classifier: Development Status :: 3 - Alpha Classifier: Environment ::
-Console Classifier: Intended Audience :: End Users/Desktop Classifier: License
-:: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Operating System :: POSIX Classifier: Operating
-System :: Unix Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Programming Language :: Python
-:: Implementation :: PyPy Classifier: Topic :: Utilities Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.AGPLv3   [!
-[GitHub Release](https://img.shields.io/github/release/obfusk/
+  [![GitHub Release](https://img.shields.io/github/release/obfusk/
 catimerge.svg?logo=github)](https://github.com/obfusk/catimerge/releases) [!
 [PyPI Version](https://img.shields.io/pypi/v/catimerge.svg)](https://
 pypi.python.org/pypi/catimerge) [![Python Versions](https://img.shields.io/
 pypi/pyversions/catimerge.svg)](https://pypi.python.org/pypi/catimerge) [![CI]
 (https://github.com/obfusk/catimerge/workflows/CI/badge.svg)](https://
 github.com/obfusk/catimerge/actions?query=workflow%3ACI) [![AGPLv3+](https://
 img.shields.io/badge/license-AGPLv3+-blue.svg)](https://www.gnu.org/licenses/
 agpl-3.0.html)  # catimerge Merge two [Catima](https://catima.app) `.zip`
-exports. ```sh $ catimerge -v catima1.zip catima2.zip out.zip Merging
-'catima1.zip' and 'catima2.zip' into 'out.zip'... Parsing... Version: 2 ZIP #1
-has 1 group(s), 9 card(s), 2 card group(s), 5 image file(s) ZIP #2 has 2 group
-(s), 5 card(s), 3 card group(s), 3 image file(s) Merging... Output has 3 group
-(s), 14 card(s), 5 card group(s), 8 image file(s) Writing... ``` NB: does not
-support password-protected exports. ## Installing ### Using pip ```bash $ pip
-install catimerge ``` NB: depending on your system you may need to use e.g.
-`pip3 --user` instead of just `pip`. ### From git NB: this installs the latest
-development version, not the latest release. ```bash $ git clone https://
-github.com/obfusk/catimerge.git $ cd catimerge $ pip install -e . ``` NB: you
-may need to add e.g. `~/.local/bin` to your `$PATH` in order to run
+exports. ```sh $ catimerge --help usage: catimerge [-h] [-v] [--version]
+FIRST_ZIP SECOND_ZIP OUTPUT_ZIP positional arguments: FIRST_ZIP SECOND_ZIP
+OUTPUT_ZIP options: -h, --help show this help message and exit -v, --verbose --
+version show program's version number and exit $ catimerge -v catima1.zip
+catima2.zip out.zip Merging 'catima1.zip' and 'catima2.zip' into 'out.zip'...
+Parsing... Version: 2 ZIP #1 has 1 group(s), 9 card(s), 2 card group(s), 5
+image file(s) ZIP #2 has 2 group(s), 5 card(s), 3 card group(s), 3 image file
+(s) Merging... Output has 3 group(s), 14 card(s), 5 card group(s), 8 image file
+(s) Writing... ``` ## CAVEATS Unfortunately, Python does not support the
+password-protected ZIP files created by Catima. You can either export your data
+without a password, or use a tool like 7-Zip to create a temporary passwordless
+ZIP file for the merge process. For example, if you have two password-protected
+ZIP files as input and want a password-protected output ZIP file as well:
+```sh $ ls catima1.zip catima2.zip $ 7z -ocatima1 x catima1.zip # extract into
+catima1/ [...] $ 7z -ocatima2 x catima2.zip # extract into catima2/ [...] $ cd
+catima1 $ 7z a ../catima1-nopass.zip * # create passwordless ZIP [...] $ cd ..
+$ cd catima2 $ 7z a ../catima2-nopass.zip * # create passwordless ZIP [...] $
+cd .. $ catimerge -v catima1-nopass.zip catima2-nopass.zip out-nopass.zip
+Merging 'catima1-nopass.zip' and 'catima2-nopass.zip' into 'out-nopass.zip'...
+[...] $ 7z -oout-nopass x out-nopass.zip # extract into out-nopass/ $ cd out-
+nopass $ 7z -p a ../out.zip * # create password-protected ZIP [...] $ cd .. $
+ls catima1 catima1-nopass.zip catima1.zip catima2 catima2-nopass.zip
+catima2.zip out-nopass out-nopass.zip out.zip ```  ## Installing ### Using pip
+```bash $ pip install catimerge ``` NB: depending on your system you may need
+to use e.g. `pip3 --user` instead of just `pip`. ### From git NB: this installs
+the latest development version, not the latest release. ```bash $ git clone
+https://github.com/obfusk/catimerge.git $ cd catimerge $ pip install -e . ```
+NB: you may need to add e.g. `~/.local/bin` to your `$PATH` in order to run
 `catimerge`. To update to the latest development version: ```bash $ cd
 catimerge $ git pull --rebase ``` ## Dependencies * Python >= 3.8. ## License
 [![AGPLv3+](https://www.gnu.org/graphics/agplv3-155x51.png)](https://
 www.gnu.org/licenses/agpl-3.0.html)
```

### Comparing `catimerge-0.0.1/setup.py` & `catimerge-0.1.0/setup.py`

 * *Files identical despite different names*

