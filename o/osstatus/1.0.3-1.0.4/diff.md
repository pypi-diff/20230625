# Comparing `tmp/osstatus-1.0.3.tar.gz` & `tmp/osstatus-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osstatus-1.0.3.tar", last modified: Sun May 14 06:31:05 2023, max compression
+gzip compressed data, was "osstatus-1.0.4.tar", last modified: Sun Jun 25 16:43:57 2023, max compression
```

## Comparing `osstatus-1.0.3.tar` & `osstatus-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:31:05.172983 osstatus-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-14 06:30:45.000000 osstatus-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43698 2023-05-14 06:31:05.172983 osstatus-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-14 06:30:45.000000 osstatus-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:31:05.172983 osstatus-1.0.3/osstatus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:30:45.000000 osstatus-1.0.3/osstatus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-14 06:30:45.000000 osstatus-1.0.3/osstatus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-14 06:30:45.000000 osstatus-1.0.3/osstatus/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:31:05.172983 osstatus-1.0.3/osstatus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43698 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-14 06:30:45.000000 osstatus-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-14 06:30:45.000000 osstatus-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 06:31:05.172983 osstatus-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:43:57.329117 osstatus-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-25 16:43:39.000000 osstatus-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43698 2023-06-25 16:43:57.329117 osstatus-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-25 16:43:39.000000 osstatus-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:43:57.329117 osstatus-1.0.4/osstatus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 16:43:39.000000 osstatus-1.0.4/osstatus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-25 16:43:39.000000 osstatus-1.0.4/osstatus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   626961 2023-06-25 16:43:39.000000 osstatus-1.0.4/osstatus/cache.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-25 16:43:39.000000 osstatus-1.0.4/osstatus/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:43:57.329117 osstatus-1.0.4/osstatus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43698 2023-06-25 16:43:57.000000 osstatus-1.0.4/osstatus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-25 16:43:57.000000 osstatus-1.0.4/osstatus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 16:43:57.000000 osstatus-1.0.4/osstatus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-25 16:43:57.000000 osstatus-1.0.4/osstatus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-25 16:43:57.000000 osstatus-1.0.4/osstatus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 16:43:57.000000 osstatus-1.0.4/osstatus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-25 16:43:39.000000 osstatus-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 16:43:39.000000 osstatus-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 16:43:57.329117 osstatus-1.0.4/setup.cfg
```

### Comparing `osstatus-1.0.3/LICENSE` & `osstatus-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `osstatus-1.0.3/PKG-INFO` & `osstatus-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osstatus
-Version: 1.0.3
+Version: 1.0.4
 Summary: Get os status from the OSStatus website
 Author-email: yotam <yotamolenik@gmail.com>
 Maintainer-email: yotam <yotamolenik@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `osstatus-1.0.3/README.md` & `osstatus-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `osstatus-1.0.3/osstatus/__main__.py` & `osstatus-1.0.4/osstatus/__main__.py`

 * *Files identical despite different names*

### Comparing `osstatus-1.0.3/osstatus/cache.py` & `osstatus-1.0.4/osstatus/cache.py`

 * *Files identical despite different names*

### Comparing `osstatus-1.0.3/osstatus.egg-info/PKG-INFO` & `osstatus-1.0.4/osstatus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osstatus
-Version: 1.0.3
+Version: 1.0.4
 Summary: Get os status from the OSStatus website
 Author-email: yotam <yotamolenik@gmail.com>
 Maintainer-email: yotam <yotamolenik@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `osstatus-1.0.3/pyproject.toml` & `osstatus-1.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "osstatus"
-version = "1.0.3"
+version = "1.0.4"
 description = "Get os status from the OSStatus website"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["ios", "error", "parser"]
 authors = [
     { name = "yotam", email = "yotamolenik@gmail.com" }
@@ -31,14 +31,17 @@
 [project.urls]
 "Homepage" = "https://github.com/yotamolenik/osstatus"
 "Bug Reports" = "https://github.com/yotamolenik/osstatus/issues"
 
 [project.scripts]
 rpcclient = "osstatus.__main__:cli"
 
+[tool.setuptools]
+package-data = { "osstatus" = ["cache.pickle"] }
+
 [tool.setuptools.packages.find]
 exclude = ["docs*", "tests*"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
 
 [build-system]
```

