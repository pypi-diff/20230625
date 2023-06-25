# Comparing `tmp/catflow-worker-0.1.5.tar.gz` & `tmp/catflow-worker-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catflow-worker-0.1.5.tar", last modified: Sun Jun 25 17:12:04 2023, max compression
+gzip compressed data, was "catflow-worker-0.1.6.tar", last modified: Sun Jun 25 18:56:18 2023, max compression
```

## Comparing `catflow-worker-0.1.5.tar` & `catflow-worker-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/catflow_worker/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/catflow_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/catflow_worker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/catflow_worker/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/catflow_worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/catflow_worker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-25 17:12:04.000000 catflow-worker-0.1.5/catflow_worker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:12:04.148526 catflow-worker-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/tests/mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-25 17:10:13.000000 catflow-worker-0.1.5/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:56:18.038006 catflow-worker-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:56:18.038006 catflow-worker-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:56:18.038006 catflow-worker-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-25 18:56:18.038006 catflow-worker-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:56:18.038006 catflow-worker-0.1.6/catflow_worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/catflow_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/catflow_worker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-25 18:56:17.000000 catflow-worker-0.1.6/catflow_worker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/catflow_worker/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/catflow_worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:56:18.038006 catflow-worker-0.1.6/catflow_worker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-25 18:56:18.000000 catflow-worker-0.1.6/catflow_worker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-25 18:56:18.000000 catflow-worker-0.1.6/catflow_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:56:18.000000 catflow-worker-0.1.6/catflow_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-25 18:56:18.000000 catflow-worker-0.1.6/catflow_worker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-25 18:56:18.000000 catflow-worker-0.1.6/catflow_worker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 18:56:18.038006 catflow-worker-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:56:18.038006 catflow-worker-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/tests/mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-25 18:54:58.000000 catflow-worker-0.1.6/tests/test_worker.py
```

### Comparing `catflow-worker-0.1.5/.github/workflows/ci.yml` & `catflow-worker-0.1.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.5/.gitignore` & `catflow-worker-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.5/LICENSE` & `catflow-worker-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.5/PKG-INFO` & `catflow-worker-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catflow-worker
-Version: 0.1.5
+Version: 0.1.6
 Summary: Consumer/publisher loop for workers in an object recognition pipeline
 Author-email: Ian Kilgore <iank@iank.org>
 License: MIT License
         
         Copyright (c) 2023 Ian Kilgore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `catflow-worker-0.1.5/README.md` & `catflow-worker-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.5/catflow_worker/main.py` & `catflow-worker-0.1.6/catflow_worker/main.py`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.5/catflow_worker/worker.py` & `catflow-worker-0.1.6/catflow_worker/worker.py`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.5/catflow_worker.egg-info/PKG-INFO` & `catflow-worker-0.1.6/catflow_worker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catflow-worker
-Version: 0.1.5
+Version: 0.1.6
 Summary: Consumer/publisher loop for workers in an object recognition pipeline
 Author-email: Ian Kilgore <iank@iank.org>
 License: MIT License
         
         Copyright (c) 2023 Ian Kilgore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `catflow-worker-0.1.5/pyproject.toml` & `catflow-worker-0.1.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 dynamic = ["version"]
 readme = "README.md"
 description = "Consumer/publisher loop for workers in an object recognition pipeline"
 authors = [{ name = "Ian Kilgore", email = "iank@iank.org"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 dependencies = [
-  "aio_pika",
-  "aioboto3",
+  "aio_pika>=9.1.3",
+  "aioboto3>=11.2.0",
+  "aiobotocore>=2.5.0",
+  "boto3>=1.26.76",
+  "botocore>=1.29.76",
 ]
 
 [tool.setuptools]
 packages = ["catflow_worker"]
 
 [project.optional-dependencies]
 dev = [
   "pytest",
   "pytest-asyncio",
   "pytest-rabbitmq",
-  "moto[server]",
+  "moto[server]>=4.1.11",
   "aiofile",
 ]
 
 [tool.setuptools_scm]
 write_to = "catflow_worker/_version.py"
 
 [tool.pytest.ini_options]
```

### Comparing `catflow-worker-0.1.5/tests/mock_server.py` & `catflow-worker-0.1.6/tests/mock_server.py`

 * *Files identical despite different names*

### Comparing `catflow-worker-0.1.5/tests/test_worker.py` & `catflow-worker-0.1.6/tests/test_worker.py`

 * *Files identical despite different names*

