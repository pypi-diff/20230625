# Comparing `tmp/data_ecosystem_flask-202306.0.28.tar.gz` & `tmp/data_ecosystem_flask-202306.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_flask-202306.0.28.tar", max compression
+gzip compressed data, was "data_ecosystem_flask-202306.0.29.tar", max compression
```

## Comparing `data_ecosystem_flask-202306.0.28.tar` & `data_ecosystem_flask-202306.0.29.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     9758 2023-06-25 18:56:20.986650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/Makefile
--rw-r--r--   0        0        0    55368 2023-06-25 18:56:20.986650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/app.py
--rw-r--r--   0        0        0    10937 2023-06-25 18:56:20.986650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/app_startup.py
--rw-r--r--   0        0        0   145583 2023-06-25 18:56:20.986650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json
--rw-r--r--   0        0        0   145583 2023-06-25 18:56:20.986650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json
--rw-r--r--   0        0        0   325863 2023-06-25 18:56:20.986650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json
--rw-r--r--   0        0        0   325863 2023-06-25 18:56:20.986650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json
--rw-r--r--   0        0        0   145835 2023-06-25 18:56:20.986650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json
--rw-r--r--   0        0        0     1692 2023-06-25 18:56:20.986650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_posit_manifests/manifest.json
--rw-r--r--   0        0        0    12165 2023-06-25 18:56:20.986650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json
--rw-r--r--   0        0        0     2082 2023-06-25 18:56:20.986650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/manifest.json
--rw-r--r--   0        0        0     5321 2023-06-25 18:56:20.990650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json
--rw-r--r--   0        0        0     5240 2023-06-25 18:56:20.990650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json
--rw-r--r--   0        0        0      374 2023-06-25 18:56:20.990650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/ocio/ocio_pade_dev/config/manifest.json
--rw-r--r--   0        0        0    17169 2023-06-25 18:56:20.990650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/requirements.txt
--rw-r--r--   0        0        0    14015 2023-06-25 18:56:20.990650 data_ecosystem_flask-202306.0.28/data_ecosystem_flask/schema/manifest.schema.json
--rw-r--r--   0        0        0    11357 2023-06-25 18:56:20.990650 data_ecosystem_flask-202306.0.28/license.md
--rw-r--r--   0        0        0     2430 2023-06-25 19:07:05.176861 data_ecosystem_flask-202306.0.28/pyproject.toml
--rw-r--r--   0        0        0    14911 2023-06-25 18:56:20.990650 data_ecosystem_flask-202306.0.28/readme.md
--rw-r--r--   0        0        0      126 2023-06-25 18:56:20.990650 data_ecosystem_flask-202306.0.28/setup.cfg
--rw-r--r--   0        0        0      127 2023-06-25 18:56:20.990650 data_ecosystem_flask-202306.0.28/setup.py
--rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 data_ecosystem_flask-202306.0.28/PKG-INFO
+-rw-r--r--   0        0        0     9758 2023-06-25 21:21:57.445355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/Makefile
+-rw-r--r--   0        0        0    55368 2023-06-25 21:21:57.445355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/app.py
+-rw-r--r--   0        0        0    10937 2023-06-25 21:21:57.445355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/app_startup.py
+-rw-r--r--   0        0        0   145583 2023-06-25 21:21:57.445355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json
+-rw-r--r--   0        0        0   145583 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json
+-rw-r--r--   0        0        0   325863 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json
+-rw-r--r--   0        0        0   325863 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json
+-rw-r--r--   0        0        0   145835 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json
+-rw-r--r--   0        0        0     1692 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_posit_manifests/manifest.json
+-rw-r--r--   0        0        0    12165 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json
+-rw-r--r--   0        0        0     2082 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/manifest.json
+-rw-r--r--   0        0        0     5321 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json
+-rw-r--r--   0        0        0     5240 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json
+-rw-r--r--   0        0        0      374 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/ocio/ocio_pade_dev/config/manifest.json
+-rw-r--r--   0        0        0    17169 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/requirements.txt
+-rw-r--r--   0        0        0    14015 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/schema/manifest.schema.json
+-rw-r--r--   0        0        0    11357 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/license.md
+-rw-r--r--   0        0        0     2442 2023-06-25 21:33:08.081480 data_ecosystem_flask-202306.0.29/pyproject.toml
+-rw-r--r--   0        0        0    14911 2023-06-25 21:21:57.453355 data_ecosystem_flask-202306.0.29/readme.md
+-rw-r--r--   0        0        0      126 2023-06-25 21:21:57.453355 data_ecosystem_flask-202306.0.29/setup.cfg
+-rw-r--r--   0        0        0      127 2023-06-25 21:21:57.453355 data_ecosystem_flask-202306.0.29/setup.py
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 data_ecosystem_flask-202306.0.29/PKG-INFO
```

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/Makefile` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/Makefile`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/app.py` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/app.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/app_startup.py` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/app_startup.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_posit_manifests/manifest.json` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_posit_manifests/manifest.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/manifest.json` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/manifest.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/requirements.txt` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/requirements.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/data_ecosystem_flask/schema/manifest.schema.json` & `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/schema/manifest.schema.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/license.md` & `data_ecosystem_flask-202306.0.29/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/pyproject.toml` & `data_ecosystem_flask-202306.0.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name = "data_ecosystem_flask"
-version="202306.0.28"
+version="202306.0.29"
 description = "Program Agnostic Data Ecosystem (PADE) - Flask Web Service"
 authors = ["John Bowyer <zfi4@cdc.gov>"]
 license = "Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
     "Development Status :: 4 - Beta",
@@ -72,15 +72,15 @@
 flaskapp = "app:app"
 
 
 [tool.pytest.ini_options]
 minversion="6.0"
 addopts="-ra -q --cov --cov-report html --cov-report term-missing --cov-fail-under 15"
 testpaths=[
-    "tests"
+    "pade_python/tests"
 ]
 
 [tool.mypy]
 warn_unused_configs=true
 namespace_packages=true
 explicit_package_bases=true
 ignore_missing_imports=true
```

### Comparing `data_ecosystem_flask-202306.0.28/readme.md` & `data_ecosystem_flask-202306.0.29/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.28/PKG-INFO` & `data_ecosystem_flask-202306.0.29/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-flask
-Version: 202306.0.28
+Version: 202306.0.29
 Summary: Program Agnostic Data Ecosystem (PADE) - Flask Web Service
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

