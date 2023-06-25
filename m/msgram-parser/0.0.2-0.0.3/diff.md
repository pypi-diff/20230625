# Comparing `tmp/msgram-parser-0.0.2.tar.gz` & `tmp/msgram-parser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram-parser-0.0.2.tar", last modified: Thu Jun 22 01:18:18 2023, max compression
+gzip compressed data, was "msgram-parser-0.0.3.tar", last modified: Sun Jun 25 04:32:08 2023, max compression
```

## Comparing `msgram-parser-0.0.2.tar` & `msgram-parser-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:18.728373 msgram-parser-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 01:18:01.000000 msgram-parser-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-22 01:18:18.728373 msgram-parser-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-22 01:18:01.000000 msgram-parser-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-22 01:18:01.000000 msgram-parser-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:18:18.728373 msgram-parser-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:18.724373 msgram-parser-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-22 01:18:01.000000 msgram-parser-0.0.2/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:18.724373 msgram-parser-0.0.2/src/msgram_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-22 01:18:18.000000 msgram-parser-0.0.2/src/msgram_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 01:18:18.000000 msgram-parser-0.0.2/src/msgram_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:18:18.000000 msgram-parser-0.0.2/src/msgram_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-22 01:18:18.000000 msgram-parser-0.0.2/src/msgram_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 01:18:18.000000 msgram-parser-0.0.2/src/msgram_parser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:18.724373 msgram-parser-0.0.2/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:01.000000 msgram-parser-0.0.2/src/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:18.728373 msgram-parser-0.0.2/src/plugins/dinamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:01.000000 msgram-parser-0.0.2/src/plugins/dinamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:18.728373 msgram-parser-0.0.2/src/plugins/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-22 01:18:01.000000 msgram-parser-0.0.2/src/plugins/domain/generic_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:18.728373 msgram-parser-0.0.2/src/plugins/statics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:01.000000 msgram-parser-0.0.2/src/plugins/statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-22 01:18:01.000000 msgram-parser-0.0.2/src/plugins/statics/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:18.728373 msgram-parser-0.0.2/src/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:01.000000 msgram-parser-0.0.2/src/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:18.728373 msgram-parser-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 01:18:01.000000 msgram-parser-0.0.2/tests/tests_main_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.963104 msgram-parser-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 04:32:08.963104 msgram-parser-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/accept_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/genericparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/plugins/dinamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/plugins/dinamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/plugins/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/plugins/domain/generic_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/plugins/statics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/plugins/statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/plugins/statics/sonarqube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.959104 msgram-parser-0.0.3/genericparser/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/genericparser/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.963104 msgram-parser-0.0.3/msgram_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 04:32:08.000000 msgram-parser-0.0.3/msgram_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 04:32:08.000000 msgram-parser-0.0.3/msgram_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 04:32:08.000000 msgram-parser-0.0.3/msgram_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-25 04:32:08.000000 msgram-parser-0.0.3/msgram_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 04:32:08.000000 msgram-parser-0.0.3/msgram_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 04:32:08.963104 msgram-parser-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:32:08.963104 msgram-parser-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/tests/test_extract_mettric_sonarqbe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-25 04:31:45.000000 msgram-parser-0.0.3/tests/tests_main_file.py
```

### Comparing `msgram-parser-0.0.2/LICENSE` & `msgram-parser-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.2/PKG-INFO` & `msgram-parser-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.2/README.md` & `msgram-parser-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.2/pyproject.toml` & `msgram-parser-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram-parser"
-version = "0.0.2"
+version = "0.0.3"
 description = "The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data."
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
@@ -18,18 +18,18 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Topic :: Utilities",
 ]
 keywords = ["parser", "measures", "quality", "algebraic model"]
 requires-python = ">=3.8"
 dependencies = [
-        "requests==2.26.0",
+        "requests==2.28.*",
         "wheel==0.37.0",
         "numpy==1.24",
-        "pandas==2.0.0",
+        "pandas==1.4.*",
     ]
 
 
 [tool.mypy]
 strict = true
 
 [project.optional-dependencies]
```

### Comparing `msgram-parser-0.0.2/src/main.py` & `msgram-parser-0.0.3/genericparser/genericparser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import importlib
-import os
-import json
+import math
 import pandas as pd
+from genericparser.accept_plugins import ACCEPT_PLUGINS
 
 
-class ParserGeneric:
-    file_path_configuration = os.path.join(os.path.dirname(__file__), "plugins.json")
+class GenericParser:
+    file_path_configuration = ACCEPT_PLUGINS
     df = None
 
     def __init__(self, file_path_configuration=None):
         self.file_path = file_path_configuration or self.file_path_configuration
 
     def parse(self, **kwargs):
         input_value = kwargs.get("input_value")
         type_input = kwargs.get("type_input")
-        accepted_types = self.get_acepted_types()
+        accepted_types = self.get_accepted_types()
         if type_input not in accepted_types:
-            raise Exception("Type not acepted")
+            raise Exception("Type not accepted by parser")
 
         path_plugin = self.get_path_plugin(type_input)
         return_from_plugin = self.call_plugin(path_plugin, input_value)
 
         if isinstance(return_from_plugin, pd.DataFrame):
             self.df = return_from_plugin
         else:
@@ -28,27 +28,28 @@
         return self.transform_df_to_python_dict(self.df)
 
     def get_df_from_parser(self, dict_input: dict):
         df = pd.DataFrame(dict_input)
         df_pivot = df.pivot(index="metrics", columns="file_paths", values="values")
         return df_pivot
 
-    def get_acepted_types(self):
-        full_json = json.load(open(self.file_path, "r"))
-        return full_json.keys()
+    def get_accepted_types(self):
+        return ACCEPT_PLUGINS.keys()
 
     def get_path_plugin(self, type_input):
-        full_json = json.load(open(self.file_path, "r"))
-        return full_json.get(type_input)
+        return ACCEPT_PLUGINS.get(type_input)
 
     def call_plugin(self, path_plugin, file_input):
         plugin = importlib.import_module(path_plugin)
         object = plugin.main()
         return object.parser(**{"input_value": file_input})
 
     def transform_df_to_python_dict(self, pandas_dataframe: pd.DataFrame):
         returned_dict = {}
+        pandas_dataframe.replace(math.nan, None, inplace=True)
         for column in pandas_dataframe.columns:
             returned_dict[column] = []
             for index, value in pandas_dataframe[column].items():
-                returned_dict[column].append({"metric": index, "value": value})
+                returned_dict[column].append(
+                    {"metric": index, "value": value}
+                ) if value is not None else None
         return returned_dict
```

### Comparing `msgram-parser-0.0.2/src/msgram_parser.egg-info/PKG-INFO` & `msgram-parser-0.0.3/msgram_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.2/src/plugins/domain/generic_class.py` & `msgram-parser-0.0.3/genericparser/plugins/domain/generic_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,16 @@
             raise Exception("kwargs must have input_value key")
         input_value = kwargs.get("input_value")
         input_value_imported = self.get_if_input_is_file_or_str(input_value)
         return_value = self.extract(input_value_imported)
         return self.validate_return_type(return_value)
 
     def get_if_input_is_file_or_str(self, input_value):
+        if isinstance(input_value, dict):
+            return input_value
         if os.path.isfile(input_value):
             path = os.path.abspath(input_value)
             with open(path, "r") as file:
                 return json.load(file)
         else:
             return input_value
```

### Comparing `msgram-parser-0.0.2/src/plugins/statics/sonarqube.py` & `msgram-parser-0.0.3/genericparser/plugins/statics/sonarqube.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from plugins.domain.generic_class import GenericStaticABC
+from genericparser.plugins.domain.generic_class import GenericStaticABC
 
 
 class ParserSonarQube(GenericStaticABC):
     def extract(self, input_file):
         metrics = []
         keys = []
         values = []
```

