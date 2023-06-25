# Comparing `tmp/netsim-tools-1.5.4.tar.gz` & `tmp/netsim-tools-1.5.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsim-tools-1.5.4.tar", last modified: Sat Jun 10 16:47:35 2023, max compression
+gzip compressed data, was "netsim-tools-1.5.4.post1.tar", last modified: Sun Jun 25 16:16:50 2023, max compression
```

## Comparing `netsim-tools-1.5.4.tar` & `netsim-tools-1.5.4.post1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:35.097739 netsim-tools-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-10 16:47:35.093739 netsim-tools-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-10 16:47:05.000000 netsim-tools-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:35.093739 netsim-tools-1.5.4/netsim_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-10 16:47:35.000000 netsim-tools-1.5.4/netsim_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-10 16:47:35.000000 netsim-tools-1.5.4/netsim_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:47:35.000000 netsim-tools-1.5.4/netsim_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-10 16:47:35.000000 netsim-tools-1.5.4/netsim_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:47:35.000000 netsim-tools-1.5.4/netsim_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:47:35.097739 netsim-tools-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-10 16:47:05.000000 netsim-tools-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:50.413871 netsim-tools-1.5.4.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-25 16:16:50.413871 netsim-tools-1.5.4.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-25 16:16:20.000000 netsim-tools-1.5.4.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:50.413871 netsim-tools-1.5.4.post1/netsim_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-25 16:16:50.000000 netsim-tools-1.5.4.post1/netsim_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-25 16:16:50.000000 netsim-tools-1.5.4.post1/netsim_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 16:16:50.000000 netsim-tools-1.5.4.post1/netsim_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-25 16:16:50.000000 netsim-tools-1.5.4.post1/netsim_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 16:16:50.000000 netsim-tools-1.5.4.post1/netsim_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 16:16:50.413871 netsim-tools-1.5.4.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-25 16:16:20.000000 netsim-tools-1.5.4.post1/setup.py
```

### Comparing `netsim-tools-1.5.4/PKG-INFO` & `netsim-tools-1.5.4.post1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsim-tools
-Version: 1.5.4
+Version: 1.5.4.post1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netsim-tools-1.5.4/netsim_tools.egg-info/PKG-INFO` & `netsim-tools-1.5.4.post1/netsim_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsim-tools
-Version: 1.5.4
+Version: 1.5.4.post1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netsim-tools-1.5.4/setup.py` & `netsim-tools-1.5.4.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ redirect netsim-tools to networklab """
 import sys
 from setuptools import setup, find_packages
 from pathlib import Path
 
 sys.path.append('..')
 
-version="1.5.4"
+version="1.5.4-post1"
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
   name="netsim-tools",
   version=version,
   packages=[],
```

