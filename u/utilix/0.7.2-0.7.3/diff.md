# Comparing `tmp/utilix-0.7.2.tar.gz` & `tmp/utilix-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/utilix-0.7.2.tar", last modified: Thu Sep  1 20:45:19 2022, max compression
+gzip compressed data, was "utilix-0.7.3.tar", last modified: Sat Jun 24 23:05:08 2023, max compression
```

## Comparing `utilix-0.7.2.tar` & `utilix-0.7.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 20:45:19.000000 utilix-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-09-01 20:45:10.000000 utilix-0.7.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-01 20:45:19.000000 utilix-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 20:45:19.000000 utilix-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     6163 2022-09-01 20:45:10.000000 utilix-0.7.2/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-09-01 20:45:10.000000 utilix-0.7.2/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-01 20:45:10.000000 utilix-0.7.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-09-01 20:45:10.000000 utilix-0.7.2/tests/test_get.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-09-01 20:45:10.000000 utilix-0.7.2/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 20:45:10.000000 utilix-0.7.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 20:45:19.000000 utilix-0.7.2/utilix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-01 20:45:19.000000 utilix-0.7.2/utilix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-01 20:45:18.000000 utilix-0.7.2/utilix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 20:45:18.000000 utilix-0.7.2/utilix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-01 20:45:18.000000 utilix-0.7.2/utilix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13426 2022-09-01 20:45:18.000000 utilix-0.7.2/utilix.egg-info/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 20:45:19.000000 utilix-0.7.2/utilix/
--rw-r--r--   0 runner    (1001) docker     (121)     4437 2022-09-01 20:45:10.000000 utilix-0.7.2/utilix/batchq.py
--rw-r--r--   0 runner    (1001) docker     (121)     3815 2022-09-01 20:45:10.000000 utilix-0.7.2/utilix/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    23294 2022-09-01 20:45:10.000000 utilix-0.7.2/utilix/mongo_files.py
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-09-01 20:45:10.000000 utilix-0.7.2/utilix/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    23315 2022-09-01 20:45:10.000000 utilix-0.7.2/utilix/rundb.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-01 20:45:10.000000 utilix-0.7.2/utilix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10247 2022-09-01 20:45:10.000000 utilix-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    13426 2022-09-01 20:45:19.000000 utilix-0.7.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 23:05:08.786452 utilix-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-06-24 23:05:08.786452 utilix-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-06-24 23:05:03.000000 utilix-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 23:05:08.786452 utilix-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-24 23:05:03.000000 utilix-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 23:05:08.786452 utilix-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 23:05:08.786452 utilix-0.7.3/utilix/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/batchq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23294 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/mongo_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23315 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/rundb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 23:05:08.786452 utilix-0.7.3/utilix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-06-24 23:05:08.000000 utilix-0.7.3/utilix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-24 23:05:08.000000 utilix-0.7.3/utilix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 23:05:08.000000 utilix-0.7.3/utilix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-24 23:05:08.000000 utilix-0.7.3/utilix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 23:05:08.000000 utilix-0.7.3/utilix.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `utilix-0.7.2/setup.py` & `utilix-0.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setup(
     name="utilix",
-    version="0.7.2",
+    version="0.7.3",
     url='https://github.com/XENONnT/utilix',
     description="User-friendly interface to various utilities for XENON users",
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=requires,
     python_requires=">=3.6",
     long_description=readme + '\n\n' + history,
```

### Comparing `utilix-0.7.2/tests/test_update.py` & `utilix-0.7.3/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.2/tests/test_url.py` & `utilix-0.7.3/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.2/tests/test_get.py` & `utilix-0.7.3/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.2/tests/test_query.py` & `utilix-0.7.3/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.2/utilix.egg-info/PKG-INFO` & `utilix-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: utilix
-Version: 0.7.2
+Version: 0.7.3
 Summary: User-friendly interface to various utilities for XENON users
 Home-page: https://github.com/XENONnT/utilix
 License: UNKNOWN
 Description: # utilix
         [![PyPI version shields.io](https://img.shields.io/pypi/v/utilix.svg)](https://pypi.python.org/pypi/utilix/)
         
         ``utilix`` is a utility package for XENON software, mainly relating to analysis. It currently has two main features: (1) a general XENON configuration framework and (2) easy access to the runsDB by wrapping python calls to a RESTful API. Eventually, we would like to include easy functions for interacting with the Midway and OSG batch queues. 
         
+        ## Installation
+        `git clone` this repo and:
+        ```
+        # at top level of utilix
+        pip install -e ./ --user
+        ```
+        
         ## Configuration file
         
         This tool expects a configuration file given by the environment variable `XENON_CONFIG`, defaulting to `$HOME/.xenon_config` if it is empty. Note that
         environment variables can be used in the form `$HOME`. Example:
         
             [RunDB]
-            rundb_api_url = [ask Evan]
-            rundb_api_user = [ask Evan]
-            rundb_api_password = [ask Evan]
+            rundb_api_url = [ask teamA]
+            rundb_api_user = [ask teamA]
+            rundb_api_password = [ask teamA]
         
         
         The idea is that analysts could use this single config for multiple purposes/analyses.
         You just need to add a (unique) section for your own purpose and then you can use the `utilix.Config` 
         easily. For example, if you made a new section called `WIMP` with `detected = yes` under it:
         
             from utilix.config import Config
@@ -49,15 +56,15 @@
         #### Setting up the runDB
         The goal of utilix is to make access to the runDB trivial. If using the runDB API, all you need to do to setup the runDB in your local script/shell is
         
             from utilix import db
             
         This instantiates the RunDB class, allowing for easy queries. Below we go through some examples of the type of queries currently supported by the runDB API wrapper in utilix. 
         
-        **If there is functionality missing that you think would be useful, please contact Evan or make a new issue (or even better, a pull request).**
+        **If there is functionality missing that you think would be useful, please contact teamA or make a new issue (or even better, a pull request).**
         
         
         
         #### Query for runs by source
         
         Note that the interface returns pages of 1,000 entries, with the first page being 1.
```

### Comparing `utilix-0.7.2/utilix/config.py` & `utilix-0.7.3/utilix/config.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.2/utilix/mongo_files.py` & `utilix-0.7.3/utilix/mongo_files.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.2/utilix/io.py` & `utilix-0.7.3/utilix/io.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.2/utilix/rundb.py` & `utilix-0.7.3/utilix/rundb.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.2/README.md` & `utilix-0.7.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # utilix
 [![PyPI version shields.io](https://img.shields.io/pypi/v/utilix.svg)](https://pypi.python.org/pypi/utilix/)
 
 ``utilix`` is a utility package for XENON software, mainly relating to analysis. It currently has two main features: (1) a general XENON configuration framework and (2) easy access to the runsDB by wrapping python calls to a RESTful API. Eventually, we would like to include easy functions for interacting with the Midway and OSG batch queues. 
 
+## Installation
+`git clone` this repo and:
+```
+# at top level of utilix
+pip install -e ./ --user
+```
+
 ## Configuration file
 
 This tool expects a configuration file given by the environment variable `XENON_CONFIG`, defaulting to `$HOME/.xenon_config` if it is empty. Note that
 environment variables can be used in the form `$HOME`. Example:
 
     [RunDB]
-    rundb_api_url = [ask Evan]
-    rundb_api_user = [ask Evan]
-    rundb_api_password = [ask Evan]
+    rundb_api_url = [ask teamA]
+    rundb_api_user = [ask teamA]
+    rundb_api_password = [ask teamA]
 
 
 The idea is that analysts could use this single config for multiple purposes/analyses.
 You just need to add a (unique) section for your own purpose and then you can use the `utilix.Config` 
 easily. For example, if you made a new section called `WIMP` with `detected = yes` under it:
 
     from utilix.config import Config
@@ -43,15 +50,15 @@
 #### Setting up the runDB
 The goal of utilix is to make access to the runDB trivial. If using the runDB API, all you need to do to setup the runDB in your local script/shell is
 
     from utilix import db
     
 This instantiates the RunDB class, allowing for easy queries. Below we go through some examples of the type of queries currently supported by the runDB API wrapper in utilix. 
 
-**If there is functionality missing that you think would be useful, please contact Evan or make a new issue (or even better, a pull request).**
+**If there is functionality missing that you think would be useful, please contact teamA or make a new issue (or even better, a pull request).**
 
 
 
 #### Query for runs by source
 
 Note that the interface returns pages of 1,000 entries, with the first page being 1.
```

### Comparing `utilix-0.7.2/PKG-INFO` & `utilix-0.7.3/utilix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: utilix
-Version: 0.7.2
+Version: 0.7.3
 Summary: User-friendly interface to various utilities for XENON users
 Home-page: https://github.com/XENONnT/utilix
 License: UNKNOWN
 Description: # utilix
         [![PyPI version shields.io](https://img.shields.io/pypi/v/utilix.svg)](https://pypi.python.org/pypi/utilix/)
         
         ``utilix`` is a utility package for XENON software, mainly relating to analysis. It currently has two main features: (1) a general XENON configuration framework and (2) easy access to the runsDB by wrapping python calls to a RESTful API. Eventually, we would like to include easy functions for interacting with the Midway and OSG batch queues. 
         
+        ## Installation
+        `git clone` this repo and:
+        ```
+        # at top level of utilix
+        pip install -e ./ --user
+        ```
+        
         ## Configuration file
         
         This tool expects a configuration file given by the environment variable `XENON_CONFIG`, defaulting to `$HOME/.xenon_config` if it is empty. Note that
         environment variables can be used in the form `$HOME`. Example:
         
             [RunDB]
-            rundb_api_url = [ask Evan]
-            rundb_api_user = [ask Evan]
-            rundb_api_password = [ask Evan]
+            rundb_api_url = [ask teamA]
+            rundb_api_user = [ask teamA]
+            rundb_api_password = [ask teamA]
         
         
         The idea is that analysts could use this single config for multiple purposes/analyses.
         You just need to add a (unique) section for your own purpose and then you can use the `utilix.Config` 
         easily. For example, if you made a new section called `WIMP` with `detected = yes` under it:
         
             from utilix.config import Config
@@ -49,15 +56,15 @@
         #### Setting up the runDB
         The goal of utilix is to make access to the runDB trivial. If using the runDB API, all you need to do to setup the runDB in your local script/shell is
         
             from utilix import db
             
         This instantiates the RunDB class, allowing for easy queries. Below we go through some examples of the type of queries currently supported by the runDB API wrapper in utilix. 
         
-        **If there is functionality missing that you think would be useful, please contact Evan or make a new issue (or even better, a pull request).**
+        **If there is functionality missing that you think would be useful, please contact teamA or make a new issue (or even better, a pull request).**
         
         
         
         #### Query for runs by source
         
         Note that the interface returns pages of 1,000 entries, with the first page being 1.
```

