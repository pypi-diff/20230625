# Comparing `tmp/gardena_bluetooth-0.3.1.tar.gz` & `tmp/gardena_bluetooth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardena_bluetooth-0.3.1.tar", max compression
+gzip compressed data, was "gardena_bluetooth-0.4.0.tar", max compression
```

## Comparing `gardena_bluetooth-0.3.1.tar` & `gardena_bluetooth-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0      704 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/README.rst
--rw-r--r--   0        0        0     3013 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/gardena_bluetooth/__init__.py
--rw-r--r--   0        0        0     2234 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/gardena_bluetooth/__main__.py
--rw-r--r--   0        0        0     4938 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/gardena_bluetooth/const.py
--rw-r--r--   0        0        0      186 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/gardena_bluetooth/exceptions.py
--rw-r--r--   0        0        0     5094 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/gardena_bluetooth/parse.py
--rw-r--r--   0        0        0      739 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 gardena_bluetooth-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      704 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/README.rst
+-rw-r--r--   0        0        0     2976 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/__init__.py
+-rw-r--r--   0        0        0     2234 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/__main__.py
+-rw-r--r--   0        0        0     3180 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/client.py
+-rw-r--r--   0        0        0     4938 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/const.py
+-rw-r--r--   0        0        0      186 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/exceptions.py
+-rw-r--r--   0        0        0     5094 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/parse.py
+-rw-r--r--   0        0        0      739 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 gardena_bluetooth-0.4.0/PKG-INFO
```

### Comparing `gardena_bluetooth-0.3.1/LICENSE.txt` & `gardena_bluetooth-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.3.1/README.rst` & `gardena_bluetooth-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.3.1/gardena_bluetooth/__init__.py` & `gardena_bluetooth-0.4.0/gardena_bluetooth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import logging
-from collections.abc import Iterable
 from datetime import datetime
 
 from bleak import BleakClient
 from bleak.uuids import register_uuids
 
 from .const import DeviceConfiguration, ScanService
 from .exceptions import CharacteristicNoAccess, CharacteristicNotFound
```

### Comparing `gardena_bluetooth-0.3.1/gardena_bluetooth/__main__.py` & `gardena_bluetooth-0.4.0/gardena_bluetooth/__main__.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.3.1/gardena_bluetooth/const.py` & `gardena_bluetooth-0.4.0/gardena_bluetooth/const.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.3.1/gardena_bluetooth/parse.py` & `gardena_bluetooth-0.4.0/gardena_bluetooth/parse.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.3.1/pyproject.toml` & `gardena_bluetooth-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gardena-bluetooth"
-version = "0.3.1"
+version = "0.4.0"
 description = ""
 authors = ["Joakim Plate <elupus@ecce.se>"]
 readme = "README.rst"
 packages = [{include = "gardena_bluetooth"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gardena_bluetooth-0.3.1/PKG-INFO` & `gardena_bluetooth-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gardena-bluetooth
-Version: 0.3.1
+Version: 0.4.0
 Summary: 
 Author: Joakim Plate
 Author-email: elupus@ecce.se
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

