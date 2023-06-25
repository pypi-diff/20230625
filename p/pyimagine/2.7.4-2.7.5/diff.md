# Comparing `tmp/pyimagine-2.7.4.tar.gz` & `tmp/pyimagine-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimagine-2.7.4.tar", last modified: Sun Jun 25 17:43:29 2023, max compression
+gzip compressed data, was "pyimagine-2.7.5.tar", last modified: Sun Jun 25 17:47:32 2023, max compression
```

## Comparing `pyimagine-2.7.4.tar` & `pyimagine-2.7.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 17:43:29.650653 pyimagine-2.7.4/
--rw-rw-rw-   0        0        0    35823 2023-06-25 15:16:20.000000 pyimagine-2.7.4/LICENSE
--rw-rw-rw-   0        0        0     3866 2023-06-25 17:43:29.647678 pyimagine-2.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     2950 2023-06-25 15:16:20.000000 pyimagine-2.7.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 17:43:29.558097 pyimagine-2.7.4/pyimagine/
--rw-rw-rw-   0        0        0       66 2023-06-25 17:20:30.000000 pyimagine-2.7.4/pyimagine/__init__.py
--rw-rw-rw-   0        0        0    40825 2023-06-25 17:26:59.000000 pyimagine-2.7.4/pyimagine/constants.py
--rw-rw-rw-   0        0        0      340 2023-06-25 17:05:37.000000 pyimagine-2.7.4/pyimagine/exceptions.py
--rw-rw-rw-   0        0        0     1674 2023-06-25 16:29:46.000000 pyimagine-2.7.4/pyimagine/utils.py
--rw-rw-rw-   0        0        0     8505 2023-06-25 17:26:34.000000 pyimagine-2.7.4/pyimagine/vyroai.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:43:29.639622 pyimagine-2.7.4/pyimagine.egg-info/
--rw-rw-rw-   0        0        0     3866 2023-06-25 17:43:29.000000 pyimagine-2.7.4/pyimagine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-25 17:43:29.000000 pyimagine-2.7.4/pyimagine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 17:43:29.000000 pyimagine-2.7.4/pyimagine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-25 17:43:29.000000 pyimagine-2.7.4/pyimagine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-25 17:43:29.000000 pyimagine-2.7.4/pyimagine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 17:43:29.651679 pyimagine-2.7.4/setup.cfg
--rw-rw-rw-   0        0        0     1230 2023-06-25 17:20:30.000000 pyimagine-2.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:43:29.642633 pyimagine-2.7.4/test/
--rw-rw-rw-   0        0        0     2160 2023-06-25 17:16:47.000000 pyimagine-2.7.4/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:47:32.323470 pyimagine-2.7.5/
+-rw-rw-rw-   0        0        0    35823 2023-06-25 15:16:20.000000 pyimagine-2.7.5/LICENSE
+-rw-rw-rw-   0        0        0     3729 2023-06-25 17:47:32.321486 pyimagine-2.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2813 2023-06-25 17:47:27.000000 pyimagine-2.7.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 17:47:32.275450 pyimagine-2.7.5/pyimagine/
+-rw-rw-rw-   0        0        0       66 2023-06-25 17:45:38.000000 pyimagine-2.7.5/pyimagine/__init__.py
+-rw-rw-rw-   0        0        0    40825 2023-06-25 17:26:59.000000 pyimagine-2.7.5/pyimagine/constants.py
+-rw-rw-rw-   0        0        0      340 2023-06-25 17:05:37.000000 pyimagine-2.7.5/pyimagine/exceptions.py
+-rw-rw-rw-   0        0        0     1674 2023-06-25 16:29:46.000000 pyimagine-2.7.5/pyimagine/utils.py
+-rw-rw-rw-   0        0        0     8505 2023-06-25 17:26:34.000000 pyimagine-2.7.5/pyimagine/vyroai.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:47:32.313453 pyimagine-2.7.5/pyimagine.egg-info/
+-rw-rw-rw-   0        0        0     3729 2023-06-25 17:47:31.000000 pyimagine-2.7.5/pyimagine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-25 17:47:32.000000 pyimagine-2.7.5/pyimagine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 17:47:31.000000 pyimagine-2.7.5/pyimagine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-25 17:47:31.000000 pyimagine-2.7.5/pyimagine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-25 17:47:31.000000 pyimagine-2.7.5/pyimagine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 17:47:32.323470 pyimagine-2.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2023-06-25 17:45:57.000000 pyimagine-2.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:47:32.316469 pyimagine-2.7.5/test/
+-rw-rw-rw-   0        0        0     2160 2023-06-25 17:16:47.000000 pyimagine-2.7.5/test/test.py
```

### Comparing `pyimagine-2.7.4/LICENSE` & `pyimagine-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimagine-2.7.4/PKG-INFO` & `pyimagine-2.7.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimagine
-Version: 2.7.4
+Version: 2.7.5
 Summary: Python library for AI-powered image manipulation.
 Home-page: https://github.com/hyugogirubato/pyimagine
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: art,image,ai,stable-diffusion
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,27 +18,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<div align="center">
-
-<img src="https://github.com/hyugogirubato/pyimagine/blob/main/docs/images/icon.png" width="10%">
-
 # PyImagine
 
 [![License](https://img.shields.io/github/license/hyugogirubato/pyimagine)](https://github.com/hyugogirubato/pyimagine/blob/main/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pyimagine)](https://github.com/hyugogirubato/pyimagine/releases)
 [![Latest Version](https://img.shields.io/pypi/v/pyimagine)](https://pypi.org/project/pyimagine/)
 
-</div>
-
-
 PyImagine is a Python library for AI-powered image manipulation. It provides a simple interface to interact with an
 image manipulation service, allowing you to perform various operations on images.
 
 ## Features
 
 - Generate inspired images based on predefined prompts and styles.
 - Apply variations to images based on prompts, strengths, and styles.
```

### Comparing `pyimagine-2.7.4/README.md` & `pyimagine-2.7.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,13 @@
-<div align="center">
-
-<img src="https://github.com/hyugogirubato/pyimagine/blob/main/docs/images/icon.png" width="10%">
-
 # PyImagine
 
 [![License](https://img.shields.io/github/license/hyugogirubato/pyimagine)](https://github.com/hyugogirubato/pyimagine/blob/main/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pyimagine)](https://github.com/hyugogirubato/pyimagine/releases)
 [![Latest Version](https://img.shields.io/pypi/v/pyimagine)](https://pypi.org/project/pyimagine/)
 
-</div>
-
-
 PyImagine is a Python library for AI-powered image manipulation. It provides a simple interface to interact with an
 image manipulation service, allowing you to perform various operations on images.
 
 ## Features
 
 - Generate inspired images based on predefined prompts and styles.
 - Apply variations to images based on prompts, strengths, and styles.
```

### Comparing `pyimagine-2.7.4/pyimagine/constants.py` & `pyimagine-2.7.5/pyimagine/constants.py`

 * *Files identical despite different names*

### Comparing `pyimagine-2.7.4/pyimagine/utils.py` & `pyimagine-2.7.5/pyimagine/utils.py`

 * *Files identical despite different names*

### Comparing `pyimagine-2.7.4/pyimagine/vyroai.py` & `pyimagine-2.7.5/pyimagine/vyroai.py`

 * *Files identical despite different names*

### Comparing `pyimagine-2.7.4/pyimagine.egg-info/PKG-INFO` & `pyimagine-2.7.5/pyimagine.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimagine
-Version: 2.7.4
+Version: 2.7.5
 Summary: Python library for AI-powered image manipulation.
 Home-page: https://github.com/hyugogirubato/pyimagine
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: art,image,ai,stable-diffusion
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,27 +18,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<div align="center">
-
-<img src="https://github.com/hyugogirubato/pyimagine/blob/main/docs/images/icon.png" width="10%">
-
 # PyImagine
 
 [![License](https://img.shields.io/github/license/hyugogirubato/pyimagine)](https://github.com/hyugogirubato/pyimagine/blob/main/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pyimagine)](https://github.com/hyugogirubato/pyimagine/releases)
 [![Latest Version](https://img.shields.io/pypi/v/pyimagine)](https://pypi.org/project/pyimagine/)
 
-</div>
-
-
 PyImagine is a Python library for AI-powered image manipulation. It provides a simple interface to interact with an
 image manipulation service, allowing you to perform various operations on images.
 
 ## Features
 
 - Generate inspired images based on predefined prompts and styles.
 - Apply variations to images based on prompts, strengths, and styles.
```

### Comparing `pyimagine-2.7.4/setup.py` & `pyimagine-2.7.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pyimagine",
-    version="2.7.4",
+    version="2.7.5",
     author="hyugogirubato",
     author_email="hyugogirubato@gmail.com",
     description="Python library for AI-powered image manipulation.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hyugogirubato/pyimagine",
     packages=find_packages(),
```

### Comparing `pyimagine-2.7.4/test/test.py` & `pyimagine-2.7.5/test/test.py`

 * *Files identical despite different names*

