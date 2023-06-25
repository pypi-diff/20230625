# Comparing `tmp/instasave-0.2.0.tar.gz` & `tmp/instasave-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instasave-0.2.0.tar", last modified: Tue Dec 29 11:01:35 2020, max compression
+gzip compressed data, was "instasave-0.3.0.tar", max compression
```

## Comparing `instasave-0.2.0.tar` & `instasave-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1070 2020-05-17 18:56:26.814415 instasave-0.2.0/LICENSE
--rw-r--r--   0        0        0     1668 2020-12-29 11:01:23.585329 instasave-0.2.0/README.md
--rw-r--r--   0        0        0     1071 2020-05-17 13:36:30.954862 instasave-0.2.0/instasave/LICENSE
--rw-r--r--   0        0        0      545 2020-12-29 11:01:23.585690 instasave-0.2.0/instasave/__init__.py
--rw-r--r--   0        0        0     1287 2020-12-29 11:01:23.585998 instasave-0.2.0/instasave/__main__.py
--rw-r--r--   0        0        0     6664 2020-12-29 11:01:23.586347 instasave-0.2.0/instasave/save_post.py
--rw-r--r--   0        0        0     1073 2020-12-29 11:01:23.587287 instasave-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2590 2020-12-29 11:01:35.174294 instasave-0.2.0/setup.py
--rw-r--r--   0        0        0     2809 2020-12-29 11:01:35.174616 instasave-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-11-22 19:26:02.789486 instasave-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1760 2022-01-01 14:55:25.649577 instasave-0.3.0/README.md
+-rw-r--r--   0        0        0     1071 2021-11-22 19:26:02.789687 instasave-0.3.0/instasave/LICENSE
+-rw-r--r--   0        0        0      545 2021-11-22 19:26:02.789770 instasave-0.3.0/instasave/__init__.py
+-rw-r--r--   0        0        0     1302 2023-06-25 19:03:28.778134 instasave-0.3.0/instasave/__main__.py
+-rw-r--r--   0        0        0     6664 2021-11-22 19:26:02.790015 instasave-0.3.0/instasave/save_post.py
+-rw-r--r--   0        0        0     1065 2023-06-25 19:03:06.703616 instasave-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 instasave-0.3.0/PKG-INFO
```

### Comparing `instasave-0.2.0/LICENSE` & `instasave-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `instasave-0.2.0/README.md` & `instasave-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <b>instasave</b>
 </h1>
 
 A simple script to download media from Instagram posts.
 
 ## Install
 
-This script runs on Python3.6+.
+This script runs on `Python 3.7+`.
 You can install it from PyPI with:
 ```bash
 pip install instasave
 ```
 
 ## Usage
 
@@ -43,15 +43,21 @@
 ## TODO
 
 - [x] Implement proper logging.
 - [x] Make into a package.
 - [x] Make callable as a python module (`python -m instasave ...`).
 - [x] Improving the command line experience.
 
-## License
+---
+
+<div align="center">
+  <sub><strong>Made with ♥︎ by fsoubelet</strong></sub>
+  <br>
+  <sub><strong>MIT &copy 2020 Felix Soubelet</strong></sub>
+</div>
+
 
-Copyright &copy; 2020 Felix Soubelet. [MIT License][license]
 
 [license]: https://github.com/fsoubelet/InstaSave/blob/master/LICENSE
 [loguru_url]: https://github.com/Delgan/loguru
 [requests_url]: https://github.com/psf/requests
 [tqdm_url]: https://github.com/tqdm/tqdm
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `instasave-0.2.0/instasave/LICENSE` & `instasave-0.3.0/instasave/LICENSE`

 * *Files identical despite different names*

### Comparing `instasave-0.2.0/instasave/__init__.py` & `instasave-0.3.0/instasave/__init__.py`

 * *Files identical despite different names*

### Comparing `instasave-0.2.0/instasave/__main__.py` & `instasave-0.3.0/instasave/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Running directly from python module.
 """
-
+import requests
 import typer
 
 from instasave.save_post import (
     determine_media_type,
     download_image,
     download_video,
     is_connected,
```

### Comparing `instasave-0.2.0/instasave/save_post.py` & `instasave-0.3.0/instasave/save_post.py`

 * *Files identical despite different names*

### Comparing `instasave-0.2.0/pyproject.toml` & `instasave-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "instasave"
-version = "0.2.0"
+version = "0.3.0"
 description = "Download script for Instagram posts"
 authors = ["Felix Soubelet <felix.soubelet@liverpool.ac.uk>"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/fsoubelet/InstaSave"
 
@@ -19,19 +19,19 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-loguru = "^0.4.1"
-tqdm = "^4.46.0"
-requests = "^2.23.0"
-typer = "^0.3.2"
+python = "^3.8"
+loguru = "^0.4"
+tqdm = "^4.46"
+requests = "^2.23"
+typer = "^0.3"
 
 [tool.poetry.dev-dependencies]
 typer-cli = "^0.0.11"
 
 
 [tool.poetry.scripts]
 instasave = "instasave.__main__:app"
```

### Comparing `instasave-0.2.0/PKG-INFO` & `instasave-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: instasave
-Version: 0.2.0
+Version: 0.3.0
 Summary: Download script for Instagram posts
 Home-page: https://github.com/fsoubelet/InstaSave
 License: MIT
 Keywords: Download,Instagram,Utility
 Author: Felix Soubelet
 Author-email: felix.soubelet@liverpool.ac.uk
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
-Requires-Dist: loguru (>=0.4.1,<0.5.0)
-Requires-Dist: requests (>=2.23.0,<3.0.0)
-Requires-Dist: tqdm (>=4.46.0,<5.0.0)
-Requires-Dist: typer (>=0.3.2,<0.4.0)
+Requires-Dist: loguru (>=0.4,<0.5)
+Requires-Dist: requests (>=2.23,<3.0)
+Requires-Dist: tqdm (>=4.46,<5.0)
+Requires-Dist: typer (>=0.3,<0.4)
 Project-URL: Repository, https://github.com/fsoubelet/InstaSave
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <b>instasave</b>
 </h1>
 
 A simple script to download media from Instagram posts.
 
 ## Install
 
-This script runs on Python3.6+.
+This script runs on `Python 3.7+`.
 You can install it from PyPI with:
 ```bash
 pip install instasave
 ```
 
 ## Usage
 
@@ -72,16 +74,22 @@
 ## TODO
 
 - [x] Implement proper logging.
 - [x] Make into a package.
 - [x] Make callable as a python module (`python -m instasave ...`).
 - [x] Improving the command line experience.
 
-## License
+---
+
+<div align="center">
+  <sub><strong>Made with ♥︎ by fsoubelet</strong></sub>
+  <br>
+  <sub><strong>MIT &copy 2020 Felix Soubelet</strong></sub>
+</div>
+
 
-Copyright &copy; 2020 Felix Soubelet. [MIT License][license]
 
 [license]: https://github.com/fsoubelet/InstaSave/blob/master/LICENSE
 [loguru_url]: https://github.com/Delgan/loguru
 [requests_url]: https://github.com/psf/requests
 [tqdm_url]: https://github.com/tqdm/tqdm
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

