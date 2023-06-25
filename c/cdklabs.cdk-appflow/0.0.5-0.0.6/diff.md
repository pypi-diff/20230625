# Comparing `tmp/cdklabs.cdk-appflow-0.0.5.tar.gz` & `tmp/cdklabs.cdk-appflow-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-appflow-0.0.5.tar", last modified: Fri Jun 23 00:39:08 2023, max compression
+gzip compressed data, was "cdklabs.cdk-appflow-0.0.6.tar", last modified: Sat Jun 24 00:34:58 2023, max compression
```

## Comparing `cdklabs.cdk-appflow-0.0.5.tar` & `cdklabs.cdk-appflow-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:39:08.384017 cdklabs.cdk-appflow-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-23 00:38:53.000000 cdklabs.cdk-appflow-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 00:38:53.000000 cdklabs.cdk-appflow-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-23 00:39:08.384017 cdklabs.cdk-appflow-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-06-23 00:38:53.000000 cdklabs.cdk-appflow-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-23 00:38:53.000000 cdklabs.cdk-appflow-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 00:39:08.384017 cdklabs.cdk-appflow-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-23 00:38:53.000000 cdklabs.cdk-appflow-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:39:08.380016 cdklabs.cdk-appflow-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:39:08.380016 cdklabs.cdk-appflow-0.0.5/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:39:08.384017 cdklabs.cdk-appflow-0.0.5/src/cdklabs/cdk_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)   504284 2023-06-23 00:38:53.000000 cdklabs.cdk-appflow-0.0.5/src/cdklabs/cdk_appflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:39:08.384017 cdklabs.cdk-appflow-0.0.5/src/cdklabs/cdk_appflow/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-23 00:38:53.000000 cdklabs.cdk-appflow-0.0.5/src/cdklabs/cdk_appflow/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179734 2023-06-23 00:38:53.000000 cdklabs.cdk-appflow-0.0.5/src/cdklabs/cdk_appflow/_jsii/cdk-appflow@0.0.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 00:38:53.000000 cdklabs.cdk-appflow-0.0.5/src/cdklabs/cdk_appflow/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:39:08.384017 cdklabs.cdk-appflow-0.0.5/src/cdklabs.cdk_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-23 00:39:08.000000 cdklabs.cdk-appflow-0.0.5/src/cdklabs.cdk_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-23 00:39:08.000000 cdklabs.cdk-appflow-0.0.5/src/cdklabs.cdk_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 00:39:08.000000 cdklabs.cdk-appflow-0.0.5/src/cdklabs.cdk_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 00:39:08.000000 cdklabs.cdk-appflow-0.0.5/src/cdklabs.cdk_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 00:39:08.000000 cdklabs.cdk-appflow-0.0.5/src/cdklabs.cdk_appflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:34:58.645852 cdklabs.cdk-appflow-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-24 00:34:43.000000 cdklabs.cdk-appflow-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-24 00:34:43.000000 cdklabs.cdk-appflow-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-24 00:34:58.645852 cdklabs.cdk-appflow-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-06-24 00:34:43.000000 cdklabs.cdk-appflow-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-24 00:34:43.000000 cdklabs.cdk-appflow-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 00:34:58.645852 cdklabs.cdk-appflow-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-24 00:34:43.000000 cdklabs.cdk-appflow-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:34:58.641852 cdklabs.cdk-appflow-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:34:58.641852 cdklabs.cdk-appflow-0.0.6/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:34:58.645852 cdklabs.cdk-appflow-0.0.6/src/cdklabs/cdk_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)   504284 2023-06-24 00:34:43.000000 cdklabs.cdk-appflow-0.0.6/src/cdklabs/cdk_appflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:34:58.645852 cdklabs.cdk-appflow-0.0.6/src/cdklabs/cdk_appflow/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-24 00:34:43.000000 cdklabs.cdk-appflow-0.0.6/src/cdklabs/cdk_appflow/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179741 2023-06-24 00:34:43.000000 cdklabs.cdk-appflow-0.0.6/src/cdklabs/cdk_appflow/_jsii/cdk-appflow@0.0.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 00:34:43.000000 cdklabs.cdk-appflow-0.0.6/src/cdklabs/cdk_appflow/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:34:58.645852 cdklabs.cdk-appflow-0.0.6/src/cdklabs.cdk_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-24 00:34:58.000000 cdklabs.cdk-appflow-0.0.6/src/cdklabs.cdk_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-24 00:34:58.000000 cdklabs.cdk-appflow-0.0.6/src/cdklabs.cdk_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 00:34:58.000000 cdklabs.cdk-appflow-0.0.6/src/cdklabs.cdk_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-24 00:34:58.000000 cdklabs.cdk-appflow-0.0.6/src/cdklabs.cdk_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-24 00:34:58.000000 cdklabs.cdk-appflow-0.0.6/src/cdklabs.cdk_appflow.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-appflow-0.0.5/LICENSE` & `cdklabs.cdk-appflow-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-appflow-0.0.5/PKG-INFO` & `cdklabs.cdk-appflow-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-appflow
-Version: 0.0.5
+Version: 0.0.6
 Summary: @cdklabs/cdk-appflow
 Home-page: https://github.com/cdklabs/cdk-appflow.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-appflow.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.cdk-appflow-0.0.5/README.md` & `cdklabs.cdk-appflow-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-appflow-0.0.5/setup.py` & `cdklabs.cdk-appflow-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-appflow",
-    "version": "0.0.5",
+    "version": "0.0.6",
     "description": "@cdklabs/cdk-appflow",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-appflow.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdklabs.cdk_appflow",
         "cdklabs.cdk_appflow._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_appflow._jsii": [
-            "cdk-appflow@0.0.5.jsii.tgz"
+            "cdk-appflow@0.0.6.jsii.tgz"
         ],
         "cdklabs.cdk_appflow": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdklabs.cdk-appflow-0.0.5/src/cdklabs/cdk_appflow/__init__.py` & `cdklabs.cdk-appflow-0.0.6/src/cdklabs/cdk_appflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-appflow-0.0.5/src/cdklabs.cdk_appflow.egg-info/PKG-INFO` & `cdklabs.cdk-appflow-0.0.6/src/cdklabs.cdk_appflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-appflow
-Version: 0.0.5
+Version: 0.0.6
 Summary: @cdklabs/cdk-appflow
 Home-page: https://github.com/cdklabs/cdk-appflow.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-appflow.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

