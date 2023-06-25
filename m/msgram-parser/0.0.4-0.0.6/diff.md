# Comparing `tmp/msgram-parser-0.0.4.tar.gz` & `tmp/msgram-parser-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram-parser-0.0.4.tar", last modified: Sun Jun 25 05:16:46 2023, max compression
+gzip compressed data, was "msgram-parser-0.0.6.tar", last modified: Sun Jun 25 06:24:26 2023, max compression
```

## Comparing `msgram-parser-0.0.4.tar` & `msgram-parser-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.082171 msgram-parser-0.0.4/genericparser/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/accept_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/genericparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.082171 msgram-parser-0.0.4/genericparser/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/genericparser/plugins/dinamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/plugins/dinamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/genericparser/plugins/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/plugins/domain/generic_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/genericparser/plugins/statics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/plugins/statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/plugins/statics/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/genericparser/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/msgram_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 05:16:46.000000 msgram-parser-0.0.4/msgram_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 05:16:46.000000 msgram-parser-0.0.4/msgram_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:16:46.000000 msgram-parser-0.0.4/msgram_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-25 05:16:46.000000 msgram-parser-0.0.4/msgram_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 05:16:46.000000 msgram-parser-0.0.4/msgram_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/tests/test_extract_mettric_sonarqbe.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/tests/tests_main_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/accept_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/genericparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/plugins/dinamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/plugins/dinamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/plugins/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/plugins/domain/generic_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/plugins/statics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/plugins/statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/plugins/statics/sonarqube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/msgram_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 06:24:26.000000 msgram-parser-0.0.6/msgram_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 06:24:26.000000 msgram-parser-0.0.6/msgram_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:24:26.000000 msgram-parser-0.0.6/msgram_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-25 06:24:26.000000 msgram-parser-0.0.6/msgram_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 06:24:26.000000 msgram-parser-0.0.6/msgram_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/tests/test_extract_mettric_sonarqbe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/tests/tests_main_file.py
```

### Comparing `msgram-parser-0.0.4/LICENSE` & `msgram-parser-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.4/PKG-INFO` & `msgram-parser-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.4
+Version: 0.0.6
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.4/README.md` & `msgram-parser-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.4/genericparser/genericparser.py` & `msgram-parser-0.0.6/genericparser/genericparser.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.4/genericparser/plugins/domain/generic_class.py` & `msgram-parser-0.0.6/genericparser/plugins/domain/generic_class.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.4/genericparser/plugins/statics/sonarqube.py` & `msgram-parser-0.0.6/genericparser/plugins/statics/sonarqube.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.4/msgram_parser.egg-info/PKG-INFO` & `msgram-parser-0.0.6/msgram_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.4
+Version: 0.0.6
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.4/msgram_parser.egg-info/SOURCES.txt` & `msgram-parser-0.0.6/msgram_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.4/pyproject.toml` & `msgram-parser-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram-parser"
-version = "0.0.4"
+version = "0.0.6"
 description = "The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data."
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
@@ -19,17 +19,16 @@
     "Programming Language :: Python :: 3.8",
     "Topic :: Utilities",
 ]
 keywords = ["parser", "measures", "quality", "algebraic model"]
 requires-python = ">=3.8"
 dependencies = [
         "requests==2.28.*",
-        "wheel==0.37.0",
-        "numpy==1.24",
-        "pandas==1.4.*",
+        "numpy==1.24.*",
+        "pandas==2.0.*",
     ]
 
 
 [tool.mypy]
 strict = true
 
 [project.optional-dependencies]
```

