# Comparing `tmp/csup_analyzer-0.1.0.tar.gz` & `tmp/csup_analyzer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csup_analyzer-0.1.0.tar", last modified: Sun Jun 25 16:51:17 2023, max compression
+gzip compressed data, was "csup_analyzer-0.1.1.tar", last modified: Sun Jun 25 17:04:49 2023, max compression
```

## Comparing `csup_analyzer-0.1.0.tar` & `csup_analyzer-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-06-22 17:30:13.797630 csup_analyzer-0.1.0/LICENSE
--rw-r--r--   0        0        0     3238 2023-06-25 14:15:51.741459 csup_analyzer-0.1.0/README.md
--rw-r--r--   0        0        0      564 2023-06-25 16:51:17.834031 csup_analyzer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      655 2023-06-25 13:04:30.742025 csup_analyzer-0.1.0/run.py
--rw-r--r--   0        0        0     3645 1970-01-01 00:00:00.000000 csup_analyzer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-22 17:30:13.797630 csup_analyzer-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3238 2023-06-25 14:15:51.741459 csup_analyzer-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 17:04:13.213877 csup_analyzer-0.1.1/csup_analyzer/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-24 10:42:39.455239 csup_analyzer-0.1.1/csup_analyzer/event/Driver.py
+-rw-r--r--   0        0        0     6195 2023-06-25 11:28:00.122788 csup_analyzer-0.1.1/csup_analyzer/event/Event.py
+-rw-r--r--   0        0        0      438 2023-06-24 08:34:34.445951 csup_analyzer-0.1.1/csup_analyzer/event/LineUp.py
+-rw-r--r--   0        0        0    10866 2023-06-25 16:48:37.404077 csup_analyzer-0.1.1/csup_analyzer/event/Result.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:43:11.091718 csup_analyzer-0.1.1/csup_analyzer/event/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-25 13:44:36.861708 csup_analyzer-0.1.1/csup_analyzer/plots/Plots.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:43:18.531717 csup_analyzer-0.1.1/csup_analyzer/plots/__init__.py
+-rw-r--r--   0        0        0     1862 2023-06-23 10:03:47.753255 csup_analyzer-0.1.1/csup_analyzer/replay/FileHandler.py
+-rw-r--r--   0        0        0     1950 2023-06-22 18:44:16.696831 csup_analyzer-0.1.1/csup_analyzer/replay/ReplayFile.py
+-rw-r--r--   0        0        0        0 2023-06-22 18:33:34.336945 csup_analyzer-0.1.1/csup_analyzer/replay/__init__.py
+-rw-r--r--   0        0        0      564 2023-06-25 17:04:49.393877 csup_analyzer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3645 1970-01-01 00:00:00.000000 csup_analyzer-0.1.1/PKG-INFO
```

### Comparing `csup_analyzer-0.1.0/LICENSE` & `csup_analyzer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csup_analyzer-0.1.0/README.md` & `csup_analyzer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `csup_analyzer-0.1.0/pyproject.toml` & `csup_analyzer-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "csup_analyzer"
-version = "0.1.0"
+version = "0.1.1"
 description = "Reads replay files from the game Circuit Superstars and offers tools to analyze the extracted data"
 authors = [
     { name = "Andre Petersen", email = "info@csup.app" },
 ]
 dependencies = [
     "pandas>=2.0.2",
     "numpy>=1.25.0",
```

### Comparing `csup_analyzer-0.1.0/PKG-INFO` & `csup_analyzer-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csup-analyzer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Reads replay files from the game Circuit Superstars and offers tools to analyze the extracted data
 Author-Email: Andre Petersen <info@csup.app>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: pandas>=2.0.2
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: matplotlib>=3.7.1
```

