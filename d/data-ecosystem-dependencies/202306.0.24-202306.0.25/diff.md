# Comparing `tmp/data_ecosystem_dependencies-202306.0.24.tar.gz` & `tmp/data_ecosystem_dependencies-202306.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_dependencies-202306.0.24.tar", max compression
+gzip compressed data, was "data_ecosystem_dependencies-202306.0.25.tar", max compression
```

## Comparing `data_ecosystem_dependencies-202306.0.24.tar` & `data_ecosystem_dependencies-202306.0.25.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      842 2023-06-24 10:46:35.646370 data_ecosystem_dependencies-202306.0.24/data_ecosystem_dependencies/__init__.py
--rw-r--r--   0        0        0    11357 2023-06-24 10:46:35.646370 data_ecosystem_dependencies-202306.0.24/license.md
--rw-r--r--   0        0        0     2740 2023-06-24 10:53:45.208361 data_ecosystem_dependencies-202306.0.24/pyproject.toml
--rw-r--r--   0        0        0      341 2023-06-24 10:46:35.646370 data_ecosystem_dependencies-202306.0.24/readme.md
--rw-r--r--   0        0        0      160 2023-06-24 10:46:35.646370 data_ecosystem_dependencies-202306.0.24/setup.cfg
--rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202306.0.24/PKG-INFO
+-rw-r--r--   0        0        0      842 2023-06-25 15:42:42.780705 data_ecosystem_dependencies-202306.0.25/data_ecosystem_dependencies/__init__.py
+-rw-r--r--   0        0        0    11357 2023-06-25 15:42:42.780705 data_ecosystem_dependencies-202306.0.25/license.md
+-rw-r--r--   0        0        0     2740 2023-06-25 15:48:43.141689 data_ecosystem_dependencies-202306.0.25/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-06-25 15:42:42.780705 data_ecosystem_dependencies-202306.0.25/readme.md
+-rw-r--r--   0        0        0      160 2023-06-25 15:42:42.780705 data_ecosystem_dependencies-202306.0.25/setup.cfg
+-rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202306.0.25/PKG-INFO
```

### Comparing `data_ecosystem_dependencies-202306.0.24/data_ecosystem_dependencies/__init__.py` & `data_ecosystem_dependencies-202306.0.25/data_ecosystem_dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202306.0.24/license.md` & `data_ecosystem_dependencies-202306.0.25/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202306.0.24/pyproject.toml` & `data_ecosystem_dependencies-202306.0.25/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="data_ecosystem_dependencies"
-version="202306.0.24"
+version="202306.0.25"
 description="Data Ecosystem  Dependencies - Python (PADE)"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://github.com/cdcent/data_ecosystem_services"
 repository="https://github.com/cdcent/data_ecosystem_services"
 classifiers=[
```

### Comparing `data_ecosystem_dependencies-202306.0.24/PKG-INFO` & `data_ecosystem_dependencies-202306.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-dependencies
-Version: 202306.0.24
+Version: 202306.0.25
 Summary: Data Ecosystem  Dependencies - Python (PADE)
 Home-page: https://github.com/cdcent/data_ecosystem_services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

