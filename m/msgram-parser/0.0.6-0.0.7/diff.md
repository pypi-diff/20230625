# Comparing `tmp/msgram-parser-0.0.6.tar.gz` & `tmp/msgram-parser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram-parser-0.0.6.tar", last modified: Sun Jun 25 06:24:26 2023, max compression
+gzip compressed data, was "msgram-parser-0.0.7.tar", last modified: Sun Jun 25 21:40:59 2023, max compression
```

## Comparing `msgram-parser-0.0.6.tar` & `msgram-parser-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/accept_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/genericparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/plugins/dinamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/plugins/dinamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/plugins/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/plugins/domain/generic_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/plugins/statics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/plugins/statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/plugins/statics/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/genericparser/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/genericparser/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/msgram_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 06:24:26.000000 msgram-parser-0.0.6/msgram_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 06:24:26.000000 msgram-parser-0.0.6/msgram_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:24:26.000000 msgram-parser-0.0.6/msgram_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-25 06:24:26.000000 msgram-parser-0.0.6/msgram_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 06:24:26.000000 msgram-parser-0.0.6/msgram_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:24:26.848220 msgram-parser-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/tests/test_extract_mettric_sonarqbe.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-25 06:24:03.000000 msgram-parser-0.0.6/tests/tests_main_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.681420 msgram-parser-0.0.7/genericparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/accept_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/genericparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.681420 msgram-parser-0.0.7/genericparser/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.681420 msgram-parser-0.0.7/genericparser/plugins/dinamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/plugins/dinamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.681420 msgram-parser-0.0.7/genericparser/plugins/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/plugins/domain/generic_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/genericparser/plugins/statics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/plugins/statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/plugins/statics/sonarqube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/genericparser/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/msgram_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 21:40:59.000000 msgram-parser-0.0.7/msgram_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 21:40:59.000000 msgram-parser-0.0.7/msgram_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:40:59.000000 msgram-parser-0.0.7/msgram_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-25 21:40:59.000000 msgram-parser-0.0.7/msgram_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 21:40:59.000000 msgram-parser-0.0.7/msgram_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/tests/test_extract_mettric_sonarqbe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/tests/tests_main_file.py
```

### Comparing `msgram-parser-0.0.6/LICENSE` & `msgram-parser-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.6/PKG-INFO` & `msgram-parser-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.6
+Version: 0.0.7
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.6/README.md` & `msgram-parser-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.6/genericparser/genericparser.py` & `msgram-parser-0.0.7/genericparser/genericparser.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.6/genericparser/plugins/domain/generic_class.py` & `msgram-parser-0.0.7/genericparser/plugins/domain/generic_class.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,20 +13,28 @@
             raise Exception("kwargs must have input_value key")
         input_value = kwargs.get("input_value")
         input_value_imported = self.get_if_input_is_file_or_str(input_value)
         return_value = self.extract(input_value_imported)
         return self.validate_return_type(return_value)
 
     def get_if_input_is_file_or_str(self, input_value):
-        if isinstance(input_value, dict):
+        if isinstance(input_value, list) or isinstance(input_value, dict):
             return input_value
-        if os.path.isfile(input_value):
+        if type(input_value) == str and os.path.isfile(input_value):
             path = os.path.abspath(input_value)
             with open(path, "r") as file:
-                return json.load(file)
+                load = json.load(file)
+                if isinstance(load, list) or isinstance(load, dict):
+                    return_value = []
+                    for keys in load:
+                        if type(load.get(keys, {})) == list:
+                            return_value.extend(load.get(keys, []))
+                        else:
+                            return_value.append(load.get(keys, {}))
+                return return_value
         else:
             return input_value
 
     def validate_return_type(self, return_value):
         if not isinstance(return_value, dict):
             raise Exception("Return from parser type must be a list")
         if return_value.get("file_paths") is None:
```

### Comparing `msgram-parser-0.0.6/genericparser/plugins/statics/sonarqube.py` & `msgram-parser-0.0.7/genericparser/plugins/statics/sonarqube.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,15 @@
 
 
 class ParserSonarQube(GenericStaticABC):
     def extract(self, input_file):
         metrics = []
         keys = []
         values = []
-
-        input_interable = []
         for entry in input_file:
-            if type(input_file[entry]) == list:
-                input_interable.extend(input_file[entry])
-            else:
-                input_interable.append(input_file[entry])
-
-        for entry in input_interable:
             key = entry.get("key", {})
             measures = entry.get("measures", [])
             for measure in measures:
                 metric = measure.get("metric", None)
                 value = measure.get("value", None)
                 metrics.append(metric)
                 keys.append(key)
```

### Comparing `msgram-parser-0.0.6/msgram_parser.egg-info/PKG-INFO` & `msgram-parser-0.0.7/msgram_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.6
+Version: 0.0.7
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.6/msgram_parser.egg-info/SOURCES.txt` & `msgram-parser-0.0.7/msgram_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.6/pyproject.toml` & `msgram-parser-0.0.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram-parser"
-version = "0.0.6"
+version = "0.0.7"
 description = "The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data."
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

