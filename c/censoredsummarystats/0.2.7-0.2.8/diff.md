# Comparing `tmp/censoredsummarystats-0.2.7.tar.gz` & `tmp/censoredsummarystats-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredsummarystats-0.2.7.tar", max compression
+gzip compressed data, was "censoredsummarystats-0.2.8.tar", max compression
```

## Comparing `censoredsummarystats-0.2.7.tar` & `censoredsummarystats-0.2.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       58 2023-06-21 09:23:06.539217 censoredsummarystats-0.2.7/censoredsummarystats/__init__.py
--rw-r--r--   0        0        0     7707 2023-06-24 22:57:00.053048 censoredsummarystats-0.2.7/censoredsummarystats/interval_to_result.py
--rw-r--r--   0        0        0     3347 2023-06-24 15:44:48.413793 censoredsummarystats-0.2.7/censoredsummarystats/merge_count_info.py
--rw-r--r--   0        0        0     5009 2023-06-24 15:44:48.419795 censoredsummarystats-0.2.7/censoredsummarystats/percent_exceedance.py
--rw-r--r--   0        0        0     2466 2023-06-24 15:44:48.428794 censoredsummarystats-0.2.7/censoredsummarystats/precision.py
--rw-r--r--   0        0        0    15228 2023-06-24 15:44:48.435796 censoredsummarystats-0.2.7/censoredsummarystats/stat_interval_aggregation.py
--rw-r--r--   0        0        0    14298 2023-06-24 22:57:00.060493 censoredsummarystats-0.2.7/censoredsummarystats/statistics.py
--rw-r--r--   0        0        0     6055 2023-06-24 15:44:48.450797 censoredsummarystats-0.2.7/censoredsummarystats/validation.py
--rw-r--r--   0        0        0    11558 2023-06-21 07:54:57.796594 censoredsummarystats-0.2.7/LICENSE
--rw-r--r--   0        0        0      558 2023-06-24 22:57:00.067491 censoredsummarystats-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     8600 2023-06-24 15:44:48.385792 censoredsummarystats-0.2.7/README.md
--rw-r--r--   0        0        0     9230 1970-01-01 00:00:00.000000 censoredsummarystats-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-06-21 09:23:06.539217 censoredsummarystats-0.2.8/censoredsummarystats/__init__.py
+-rw-r--r--   0        0        0     7707 2023-06-24 22:57:00.053048 censoredsummarystats-0.2.8/censoredsummarystats/interval_to_result.py
+-rw-r--r--   0        0        0     3347 2023-06-24 15:44:48.413793 censoredsummarystats-0.2.8/censoredsummarystats/merge_count_info.py
+-rw-r--r--   0        0        0     5009 2023-06-24 15:44:48.419795 censoredsummarystats-0.2.8/censoredsummarystats/percent_exceedance.py
+-rw-r--r--   0        0        0     2466 2023-06-24 15:44:48.428794 censoredsummarystats-0.2.8/censoredsummarystats/precision.py
+-rw-r--r--   0        0        0    15228 2023-06-24 15:44:48.435796 censoredsummarystats-0.2.8/censoredsummarystats/stat_interval_aggregation.py
+-rw-r--r--   0        0        0    14298 2023-06-24 22:57:00.060493 censoredsummarystats-0.2.8/censoredsummarystats/statistics.py
+-rw-r--r--   0        0        0     6055 2023-06-24 15:44:48.450797 censoredsummarystats-0.2.8/censoredsummarystats/validation.py
+-rw-r--r--   0        0        0    11558 2023-06-21 07:54:57.796594 censoredsummarystats-0.2.8/LICENSE
+-rw-r--r--   0        0        0      575 2023-06-24 23:04:34.640492 censoredsummarystats-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     8600 2023-06-24 15:44:48.385792 censoredsummarystats-0.2.8/README.md
+-rw-r--r--   0        0        0     9265 1970-01-01 00:00:00.000000 censoredsummarystats-0.2.8/PKG-INFO
```

### Comparing `censoredsummarystats-0.2.7/censoredsummarystats/interval_to_result.py` & `censoredsummarystats-0.2.8/censoredsummarystats/interval_to_result.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.7/censoredsummarystats/merge_count_info.py` & `censoredsummarystats-0.2.8/censoredsummarystats/merge_count_info.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.7/censoredsummarystats/percent_exceedance.py` & `censoredsummarystats-0.2.8/censoredsummarystats/percent_exceedance.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.7/censoredsummarystats/precision.py` & `censoredsummarystats-0.2.8/censoredsummarystats/precision.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.7/censoredsummarystats/stat_interval_aggregation.py` & `censoredsummarystats-0.2.8/censoredsummarystats/stat_interval_aggregation.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.7/censoredsummarystats/statistics.py` & `censoredsummarystats-0.2.8/censoredsummarystats/statistics.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.7/censoredsummarystats/validation.py` & `censoredsummarystats-0.2.8/censoredsummarystats/validation.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.7/LICENSE` & `censoredsummarystats-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.7/pyproject.toml` & `censoredsummarystats-0.2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "censoredsummarystats"
-version = "0.2.7"
+version = "0.2.8"
 description = "A python package for calculating summary stats on censored data (data that contains < and > symbols)."
 authors = ["Kurt van Ness <vanness.kurt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kurtvanness/CensoredSummaryStats"
 license = "Apache-2.0"
 packages = [{include = "censoredsummarystats"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.24.0"
+pandas = "^2.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `censoredsummarystats-0.2.7/README.md` & `censoredsummarystats-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.7/PKG-INFO` & `censoredsummarystats-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: censoredsummarystats
-Version: 0.2.7
+Version: 0.2.8
 Summary: A python package for calculating summary stats on censored data (data that contains < and > symbols).
 Home-page: https://github.com/kurtvanness/CensoredSummaryStats
 License: Apache-2.0
 Author: Kurt van Ness
 Author-email: vanness.kurt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Requires-Dist: pandas (>=2.0,<3.0)
 Project-URL: Repository, https://github.com/kurtvanness/CensoredSummaryStats
 Description-Content-Type: text/markdown
 
 # censoredsummarystats
 A repository that contains a CensoredData class for analyzing censored data for basic stats.
 
 ## Class settings:
```

