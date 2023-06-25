# Comparing `tmp/msgram-parser-0.0.3.tar.gz` & `tmp/msgram-parser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram-parser-0.0.3.tar", last modified: Sun Jun 25 04:32:08 2023, max compression
+gzip compressed data, was "msgram-parser-0.0.4.tar", last modified: Sun Jun 25 05:16:46 2023, max compression
```

## Comparing `msgram-parser-0.0.3.tar` & `msgram-parser-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.963104 msgram-parser-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 04:32:08.963104 msgram-parser-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/accept_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/genericparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/plugins/dinamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/plugins/dinamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/plugins/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/plugins/domain/generic_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/plugins/statics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/plugins/statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/plugins/statics/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.963104 msgram-parser-0.0.3/msgram_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 04:32:08.000000 msgram-parser-0.0.3/msgram_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 04:32:08.000000 msgram-parser-0.0.3/msgram_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 04:32:08.000000 msgram-parser-0.0.3/msgram_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-25 04:32:08.000000 msgram-parser-0.0.3/msgram_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 04:32:08.000000 msgram-parser-0.0.3/msgram_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 04:32:08.963104 msgram-parser-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.963104 msgram-parser-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/tests/test_extract_mettric_sonarqbe.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/tests/tests_main_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.082171 msgram-parser-0.0.4/genericparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/accept_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/genericparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.082171 msgram-parser-0.0.4/genericparser/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/genericparser/plugins/dinamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/plugins/dinamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/genericparser/plugins/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/plugins/domain/generic_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/genericparser/plugins/statics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/plugins/statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/plugins/statics/sonarqube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/genericparser/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/genericparser/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/msgram_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 05:16:46.000000 msgram-parser-0.0.4/msgram_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 05:16:46.000000 msgram-parser-0.0.4/msgram_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:16:46.000000 msgram-parser-0.0.4/msgram_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-25 05:16:46.000000 msgram-parser-0.0.4/msgram_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 05:16:46.000000 msgram-parser-0.0.4/msgram_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:16:46.086171 msgram-parser-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/tests/test_extract_mettric_sonarqbe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-25 05:16:28.000000 msgram-parser-0.0.4/tests/tests_main_file.py
```

### Comparing `msgram-parser-0.0.3/LICENSE` & `msgram-parser-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.3/PKG-INFO` & `msgram-parser-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.3
+Version: 0.0.4
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.3/README.md` & `msgram-parser-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.3/genericparser/genericparser.py` & `msgram-parser-0.0.4/genericparser/genericparser.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.3/genericparser/plugins/domain/generic_class.py` & `msgram-parser-0.0.4/genericparser/plugins/domain/generic_class.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.3/genericparser/plugins/statics/sonarqube.py` & `msgram-parser-0.0.4/genericparser/plugins/statics/sonarqube.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.3/msgram_parser.egg-info/PKG-INFO` & `msgram-parser-0.0.4/msgram_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.3
+Version: 0.0.4
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.3/msgram_parser.egg-info/SOURCES.txt` & `msgram-parser-0.0.4/msgram_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.3/pyproject.toml` & `msgram-parser-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram-parser"
-version = "0.0.3"
+version = "0.0.4"
 description = "The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data."
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

