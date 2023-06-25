# Comparing `tmp/asv_runner-0.0.5.tar.gz` & `tmp/asv_runner-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asv_runner-0.0.5.tar", last modified: Sun Jun 25 19:16:14 2023, max compression
+gzip compressed data, was "asv_runner-0.0.6.tar", last modified: Sun Jun 25 19:32:29 2023, max compression
```

## Comparing `asv_runner-0.0.5.tar` & `asv_runner-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      286 2023-06-25 19:16:04.758892 asv_runner-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-25 19:16:04.758892 asv_runner-0.0.5/asv_runner/__init__.py
--rw-r--r--   0        0        0     6718 2023-06-25 19:16:04.758892 asv_runner-0.0.5/asv_runner/_aux.py
--rw-r--r--   0        0        0     1825 2023-06-25 19:16:04.758892 asv_runner-0.0.5/asv_runner/benchmarks/__init__.py
--rw-r--r--   0        0        0    22059 2023-06-25 19:16:04.758892 asv_runner-0.0.5/asv_runner/benchmarks/_base.py
--rw-r--r--   0        0        0     1095 2023-06-25 19:16:04.758892 asv_runner-0.0.5/asv_runner/benchmarks/_exceptions.py
--rw-r--r--   0        0        0     5683 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/_maxrss.py
--rw-r--r--   0        0        0     2248 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/mem.py
--rw-r--r--   0        0        0     1965 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/peakmem.py
--rw-r--r--   0        0        0     9895 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/time.py
--rw-r--r--   0        0        0     5071 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/timeraw.py
--rw-r--r--   0        0        0     1912 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/track.py
--rw-r--r--   0        0        0      915 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/check.py
--rw-r--r--   0        0        0    14462 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/console.py
--rw-r--r--   0        0        0    10852 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/discovery.py
--rw-r--r--   0        0        0     2456 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/run.py
--rw-r--r--   0        0        0     7956 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/server.py
--rw-r--r--   0        0        0     1450 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/setup_cache.py
--rw-r--r--   0        0        0    18701 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/statistics.py
--rw-r--r--   0        0        0     2744 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/timing.py
--rw-r--r--   0        0        0     4549 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/util.py
--rw-r--r--   0        0        0     1468 2023-06-25 19:16:14.542956 asv_runner-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 asv_runner-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      286 2023-06-25 19:32:21.958229 asv_runner-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/__init__.py
+-rw-r--r--   0        0        0     6718 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/_aux.py
+-rw-r--r--   0        0        0     1825 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/benchmarks/__init__.py
+-rw-r--r--   0        0        0    22059 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/benchmarks/_base.py
+-rw-r--r--   0        0        0     1095 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/benchmarks/_exceptions.py
+-rw-r--r--   0        0        0     5683 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/benchmarks/_maxrss.py
+-rw-r--r--   0        0        0     2248 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/benchmarks/mem.py
+-rw-r--r--   0        0        0     1965 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/benchmarks/peakmem.py
+-rw-r--r--   0        0        0     9895 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/benchmarks/time.py
+-rw-r--r--   0        0        0     5071 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/benchmarks/timeraw.py
+-rw-r--r--   0        0        0     1912 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/benchmarks/track.py
+-rw-r--r--   0        0        0      915 2023-06-25 19:32:21.958229 asv_runner-0.0.6/asv_runner/check.py
+-rw-r--r--   0        0        0    14462 2023-06-25 19:32:21.962229 asv_runner-0.0.6/asv_runner/console.py
+-rw-r--r--   0        0        0    10852 2023-06-25 19:32:21.962229 asv_runner-0.0.6/asv_runner/discovery.py
+-rw-r--r--   0        0        0     2456 2023-06-25 19:32:21.962229 asv_runner-0.0.6/asv_runner/run.py
+-rw-r--r--   0        0        0     7956 2023-06-25 19:32:21.962229 asv_runner-0.0.6/asv_runner/server.py
+-rw-r--r--   0        0        0     1450 2023-06-25 19:32:21.962229 asv_runner-0.0.6/asv_runner/setup_cache.py
+-rw-r--r--   0        0        0    18701 2023-06-25 19:32:21.962229 asv_runner-0.0.6/asv_runner/statistics.py
+-rw-r--r--   0        0        0     2744 2023-06-25 19:32:21.962229 asv_runner-0.0.6/asv_runner/timing.py
+-rw-r--r--   0        0        0     4549 2023-06-25 19:32:21.962229 asv_runner-0.0.6/asv_runner/util.py
+-rw-r--r--   0        0        0     1484 2023-06-25 19:32:29.874344 asv_runner-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 asv_runner-0.0.6/PKG-INFO
```

### Comparing `asv_runner-0.0.5/asv_runner/_aux.py` & `asv_runner-0.0.6/asv_runner/_aux.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/benchmarks/__init__.py` & `asv_runner-0.0.6/asv_runner/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/benchmarks/_base.py` & `asv_runner-0.0.6/asv_runner/benchmarks/_base.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/benchmarks/_exceptions.py` & `asv_runner-0.0.6/asv_runner/benchmarks/_exceptions.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/benchmarks/_maxrss.py` & `asv_runner-0.0.6/asv_runner/benchmarks/_maxrss.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/benchmarks/mem.py` & `asv_runner-0.0.6/asv_runner/benchmarks/mem.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/benchmarks/peakmem.py` & `asv_runner-0.0.6/asv_runner/benchmarks/peakmem.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/benchmarks/time.py` & `asv_runner-0.0.6/asv_runner/benchmarks/time.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/benchmarks/timeraw.py` & `asv_runner-0.0.6/asv_runner/benchmarks/timeraw.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/benchmarks/track.py` & `asv_runner-0.0.6/asv_runner/benchmarks/track.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/check.py` & `asv_runner-0.0.6/asv_runner/check.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/console.py` & `asv_runner-0.0.6/asv_runner/console.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/discovery.py` & `asv_runner-0.0.6/asv_runner/discovery.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/run.py` & `asv_runner-0.0.6/asv_runner/run.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/server.py` & `asv_runner-0.0.6/asv_runner/server.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/setup_cache.py` & `asv_runner-0.0.6/asv_runner/setup_cache.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/statistics.py` & `asv_runner-0.0.6/asv_runner/statistics.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/timing.py` & `asv_runner-0.0.6/asv_runner/timing.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/asv_runner/util.py` & `asv_runner-0.0.6/asv_runner/util.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.5/pyproject.toml` & `asv_runner-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -46,35 +46,37 @@
 
 [tool.setuptools_scm]
 write_to = "asv_runner/_version.py"
 
 [project]
 name = "asv_runner"
 description = "Core Python benchmark code for ASV"
-homepage = "https://haozeke.github.io/asv_runner/"
-repository = "https://github.com/HaoZeke/asv_runner"
-documentation = "https://haozeke.github.io/asv_runner/"
 authors = [
     { name = "Rohit Goswami", email = "rog32@hi.is" },
 ]
 maintainers = [
     { name = "Rohit Goswami", email = "rog32@hi.is" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
     "License :: OSI Approved :: MIT License",
     "Topic :: System :: Benchmark",
 ]
-version = "0.0.5"
+version = "0.0.6"
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
+[project.urls]
+homepage = "https://haozeke.github.io/asv_runner/"
+repository = "https://github.com/HaoZeke/asv_runner"
+documentation = "https://haozeke.github.io/asv_runner/"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `asv_runner-0.0.5/PKG-INFO` & `asv_runner-0.0.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: asv-runner
-Version: 0.0.5
+Version: 0.0.6
 Summary: Core Python benchmark code for ASV
+Home-page: https://haozeke.github.io/asv_runner/
 Author-Email: Rohit Goswami <rog32@hi.is>
 Maintainer-Email: Rohit Goswami <rog32@hi.is>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: System :: Benchmark
+Project-URL: Homepage, https://haozeke.github.io/asv_runner/
+Project-URL: Repository, https://github.com/HaoZeke/asv_runner
+Project-URL: Documentation, https://haozeke.github.io/asv_runner/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # About
 
 Core Python benchmark code for `asv`.
```

